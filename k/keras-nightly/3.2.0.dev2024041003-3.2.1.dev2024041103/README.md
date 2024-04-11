# Comparing `tmp/keras-nightly-3.2.0.dev2024041003.tar.gz` & `tmp/keras-nightly-3.2.1.dev2024041103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-nightly-3.2.0.dev2024041003.tar", last modified: Wed Apr 10 03:22:04 2024, max compression
+gzip compressed data, was "keras-nightly-3.2.1.dev2024041103.tar", last modified: Thu Apr 11 03:22:43 2024, max compression
```

## Comparing `keras-nightly-3.2.0.dev2024041003.tar` & `keras-nightly-3.2.1.dev2024041103.tar`

### file list

```diff
@@ -1,691 +1,691 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.321130 keras-nightly-3.2.0.dev2024041003/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-10 03:22:04.321130 keras-nightly-3.2.0.dev2024041003/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.225129 keras-nightly-3.2.0.dev2024041003/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.225129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.229129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.233129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.237129 keras-nightly-3.2.0.dev2024041003/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.241129 keras-nightly-3.2.0.dev2024041003/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.245129 keras-nightly-3.2.0.dev2024041003/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.249129 keras-nightly-3.2.0.dev2024041003/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.249129 keras-nightly-3.2.0.dev2024041003/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.249129 keras-nightly-3.2.0.dev2024041003/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.249129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.253129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.253129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.257129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.261129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.261129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.265129 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.269129 keras-nightly-3.2.0.dev2024041003/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.273129 keras-nightly-3.2.0.dev2024041003/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.273129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.273129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.273129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.277129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.281129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    62806 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.281129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.281129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.285129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.289129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.293129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.293129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.297129 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.297129 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.297129 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.301129 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.301129 keras-nightly-3.2.0.dev2024041003/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.301129 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.305129 keras-nightly-3.2.0.dev2024041003/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.305129 keras-nightly-3.2.0.dev2024041003/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   190019 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    36189 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.309130 keras-nightly-3.2.0.dev2024041003/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.313130 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.313130 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45200 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.317130 keras-nightly-3.2.0.dev2024041003/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26577 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-10 03:21:58.000000 keras-nightly-3.2.0.dev2024041003/keras/src/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 03:21:57.000000 keras-nightly-3.2.0.dev2024041003/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.317130 keras-nightly-3.2.0.dev2024041003/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.317130 keras-nightly-3.2.0.dev2024041003/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.317130 keras-nightly-3.2.0.dev2024041003/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:22:04.321130 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-10 03:22:04.000000 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-10 03:22:04.000000 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:22:04.000000 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-10 03:22:04.000000 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 03:22:04.000000 keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:22:04.321130 keras-nightly-3.2.0.dev2024041003/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-10 03:22:02.000000 keras-nightly-3.2.0.dev2024041003/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.599718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6809 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.603718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.607718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.611718 keras-nightly-3.2.1.dev2024041103/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.615718 keras-nightly-3.2.1.dev2024041103/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.619718 keras-nightly-3.2.1.dev2024041103/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24920 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25275 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40461 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16035 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23522 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.623718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9738 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.627718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18796 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30090 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36171 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.627718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17760 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27723 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.631718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11446 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26462 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67409 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34607 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32141 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33608 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.635718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16169 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9756 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15074 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24038 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45949 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.635718 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26400 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31208 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.639718 keras-nightly-3.2.1.dev2024041103/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32837 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23463 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.643718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17953 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27410 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.647718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10696 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12644 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6451 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.647718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16970 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15723 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62881 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.651718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.651718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.655718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.659718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10937 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41400 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18459 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13921 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27821 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.659718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4647 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13204 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27249 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27708 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18875 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4950 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.663718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70242 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65546 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11173 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11111 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22746 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66376 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.667718 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15605 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61580 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19819 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.671718 keras-nightly-3.2.1.dev2024041103/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13020 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.671718 keras-nightly-3.2.1.dev2024041103/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15341 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31490 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17411 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30619 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62114 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190163 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13766 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36783 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35508 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13439 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.675718 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27009 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25825 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.679718 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17068 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9724 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45200 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14203 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28538 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16624 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26577 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15206 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20703 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-11 03:22:38.000000 keras-nightly-3.2.1.dev2024041103/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:22:43.000000 keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:22:43.687718 keras-nightly-3.2.1.dev2024041103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-11 03:22:41.000000 keras-nightly-3.2.1.dev2024041103/setup.py
```

### Comparing `keras-nightly-3.2.0.dev2024041003/PKG-INFO` & `keras-nightly-3.2.1.dev2024041103/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024041003
+Version: 3.2.1.dev2024041103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024041003/README.md` & `keras-nightly-3.2.1.dev2024041103/README.md`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 from keras.src.optimizers.optimizer import Optimizer
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.regularizers.regularizers import Regularizer
 from keras.src.version import version
 
 
-__version__ = "3.2.0.dev2024041003"
+__version__ = "3.2.1.dev2024041103"
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/config/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/random/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/tree/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/_tf_keras/keras/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/applications/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/applications/convnext/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/applications/efficientnet_v2/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/config/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/mixed_precision/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/ops/linalg/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/ops/nn/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/ops/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/optimizers/legacy/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/random/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/activations/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/activations/activations.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/activations/activations.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,17 +353,17 @@
 
 @keras_export("keras.activations.hard_sigmoid")
 def hard_sigmoid(x):
     """Hard sigmoid activation function.
 
     The hard sigmoid activation is defined as:
 
-    - `0` if `if x < -2.5`
-    - `1` if `x > 2.5`
-    - `0.2 * x + 0.5` if `-2.5 <= x <= 2.5`
+    - `0` if `if x <= -3`
+    - `1` if `x >= 3`
+    - `(x/6) + 0.5` if `-3 < x < 3`
 
     It's a faster, piecewise linear approximation
     of the sigmoid activation.
 
     Args:
         x: Input tensor.
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/api_export.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/convnext.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/densenet.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/efficientnet.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/efficientnet_v2.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/imagenet_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/inception_resnet_v2.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/inception_v3.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet_v2.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/mobilenet_v3.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/nasnet.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/resnet.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/resnet_v2.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/vgg16.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/vgg19.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/applications/xception.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/backend_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/dtypes.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/global_state.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/keras_tensor.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/name_scope.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/stateless_scope.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/common/variables.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/config.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/exports.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/core.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/linalg.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/math.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/nn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/numpy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,35 @@
 def add(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.add(x1, x2)
 
 
 def bincount(x, weights=None, minlength=0, sparse=False):
-    if sparse:
+    # Note: bincount is never tracable / jittable because the output shape
+    # depends on the values in x.
+    if sparse or isinstance(x, jax_sparse.BCOO):
+        if isinstance(x, jax_sparse.BCOO):
+            if weights is not None:
+                if not isinstance(weights, jax_sparse.BCOO):
+                    raise ValueError("`x` and `weights` must both be BCOOs")
+                if x.indices is not weights.indices:
+                    # This test works in eager mode only
+                    if not jnp.all(jnp.equal(x.indices, weights.indices)):
+                        raise ValueError(
+                            "`x` and `weights` BCOOs must have the same indices"
+                        )
+                weights = weights.data
+            x = x.data
         reduction_axis = 1 if len(x.shape) > 1 else 0
         maxlength = jnp.maximum(jnp.max(x) + 1, minlength)
-        one_hot_encoding = nn.one_hot(x, maxlength, sparse=sparse)
+        one_hot_encoding = nn.one_hot(x, maxlength, sparse=True)
         if weights is not None:
-            split_weights = split(
-                weights,
-                weights.shape[reduction_axis],
-                reduction_axis,
-            )
-            stacked_weights = stack(split_weights, axis=reduction_axis)
-            one_hot_encoding = one_hot_encoding * stacked_weights
+            expanded_weights = jnp.expand_dims(weights, reduction_axis + 1)
+            one_hot_encoding = one_hot_encoding * expanded_weights
 
         outputs = jax_sparse.bcoo_reduce_sum(
             one_hot_encoding,
             axes=(reduction_axis,),
         )
         return outputs
     if len(x.shape) == 2:
@@ -481,14 +490,15 @@
 
 
 def diff(a, n=1, axis=-1):
     a = convert_to_tensor(a)
     return jnp.diff(a, n=n, axis=axis)
 
 
+@sparse.elementwise_unary(linear=False)
 def digitize(x, bins):
     x = convert_to_tensor(x)
     bins = convert_to_tensor(bins)
     return jnp.digitize(x, bins)
 
 
 def dot(x, y):
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/random.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/sparse.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/jax/trainer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/core.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/linalg.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/math.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/nn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/numpy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/random.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/numpy/trainer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/core.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,21 +19,30 @@
         device_type: string of `"cpu"`, `"gpu"` or `"tpu"`. Default to `gpu` or
         `tpu` if available when device_type is not provided. Otherwise will
         return the `cpu` devices.
 
     Return:
         List of devices that are available for distribute computation.
     """
-    device_type = device_type.upper() if device_type else "CPU"
+    device_type = device_type.upper() if device_type else None
 
     # DTensor doesn't support getting global devices, even when knowing the
     # Mesh. Use TF API instead to get global devices. Coordinator service is
     # enabled by default with DTensor, so that list_logical_devices() returns
     # a list of global devices. More context can be found in b/254911601.
     tf_devices = tf.config.list_logical_devices(device_type=device_type)
+    cpu_devices = []
+    other_devices = []
+    for device in tf_devices:
+        if device.device_type.lower() == "cpu":
+            cpu_devices.append(device)
+        else:
+            other_devices.append(device)
+    if device_type is None:
+        tf_devices = other_devices if len(other_devices) > 0 else cpu_devices
     return [
         f"{device.device_type.lower()}:{device.name.split(':')[-1]}"
         for device in tf_devices
     ]
 
 
 def distribute_value(value, tensor_layout):
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/linalg.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/math.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/nn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/numpy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,23 @@
         )
 
     def _distributed_tf_update_step(
         self, distribution, grads_and_vars, learning_rate
     ):
         grads_and_vars = self._all_reduce_sum_gradients(grads_and_vars)
 
-        def apply_grad_to_update_var(var, grad):
+        def apply_grad_to_update_var(var, grad, learning_rate):
             return self.update_step(grad, var, learning_rate)
 
         for grad, var in grads_and_vars:
             distribution.extended.update(
-                var, apply_grad_to_update_var, args=(grad,), group=False
+                var,
+                apply_grad_to_update_var,
+                args=(grad, learning_rate),
+                group=False,
             )
 
     def _all_reduce_sum_gradients(self, grads_and_vars):
         """Returns all-reduced gradients aggregated via summation.
 
         Args:
             grads_and_vars: List of (gradient, variable) pairs.
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/random.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/sparse.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/trackable.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/tensorflow/trainer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/core.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/linalg.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/math.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/nn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/numpy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/random.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/backend/torch/trainer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/backup_and_restore.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/callback.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/callback_list.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/csv_logger.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/early_stopping.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/history.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/lambda_callback.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/learning_rate_scheduler.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/model_checkpoint.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/progbar_logger.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/remote_monitor.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/swap_ema_weights.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/tensorboard.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/callbacks/terminate_on_nan.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/constraints/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/constraints/constraints.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/boston_housing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/california_housing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar10.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/cifar100.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/fashion_mnist.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/imdb.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/mnist.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/datasets/reuters.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/distribution/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/distribution/distribution_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/dtype_policies/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/dtype_policies/dtype_policy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/export/export_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/initializers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/initializers/constant_initializers.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/initializers/initializer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/initializers/random_initializers.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/activation.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/elu.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/leaky_relu.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/prelu.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/relu.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/activations/softmax.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/additive_attention.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/attention.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/grouped_query_attention.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/attention/multi_head_attention.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_conv.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/base_separable_conv.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/separable_conv1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/convolutional/separable_conv2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/dense.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/einsum_dense.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/embedding.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/identity.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/input_layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/lambda_layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/masking.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/core/wrapper.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/input_spec.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,18 +288,18 @@
         self._convert_input_args = True
         # Whether to allow non-tensors as positional arguments in `call()`.
         self._allow_non_tensor_positional_args = False
         # Dict of shapes that were used to call `build()`.
         self._build_shapes_dict = None
         # Parent path
         self._parent_path = None
-        self._initializer_tracker()
+        self._initialize_tracker()
 
     @tracking.no_automatic_dependency_tracking
-    def _initializer_tracker(self):
+    def _initialize_tracker(self):
         if hasattr(self, "_tracker"):
             return
 
         trainable_variables = []
         non_trainable_variables = []
         layers = []
         metrics = []
@@ -321,15 +321,16 @@
                     and not isinstance(x, Metric),
                     layers,
                 ),
                 "seed_generators": (
                     lambda x: isinstance(x, backend.random.SeedGenerator),
                     seed_generators,
                 ),
-            }
+            },
+            exclusions={"non_trainable_variables": ["trainable_variables"]},
         )
         if backend.backend() == "tensorflow":
             # Remove attribute tracking for lists (TF-specific attribute)
             _self_setattr_tracking = getattr(
                 self, "_self_setattr_tracking", True
             )
             self._self_setattr_tracking = False
@@ -1318,15 +1319,15 @@
 
     def __setattr__(self, name, value):
         # Track Variables, Layers, Metrics, SeedGenerators.
         name, value = self._setattr_hook(name, value)
         if hasattr(self, "_tracker"):
             value = self._tracker.track(value)
         elif name != "_tracker":
-            self._initializer_tracker()
+            self._initialize_tracker()
         return super().__setattr__(name, value)
 
     def _check_super_called(self):
         if getattr(self, "_lock", True):
             raise RuntimeError(
                 f"In layer '{self.__class__.__name__}', you forgot to call "
                 "`super().__init__()` as the first statement "
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/add.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/average.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/base_merge.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/concatenate.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/dot.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/maximum.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/minimum.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/multiply.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/merging/subtract.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/batch_normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/group_normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/layer_normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/spectral_normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/normalization/unit_normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/average_pooling3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/base_global_pooling.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/base_pooling.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/pooling/max_pooling3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/category_encoding.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/center_crop.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/discretization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/feature_space.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/hashing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/index_lookup.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/integer_lookup.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/normalization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_brightness.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_contrast.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_crop.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_flip.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_rotation.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_translation.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/random_zoom.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/rescaling.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/resizing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/string_lookup.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/text_vectorization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/activity_regularization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/alpha_dropout.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/dropout.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/gaussian_dropout.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/gaussian_noise.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/regularization/spatial_dropout.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/cropping3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/flatten.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/permute.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/repeat_vector.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/reshape.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/up_sampling3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/reshaping/zero_padding3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/bidirectional.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm1d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm2d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/conv_lstm3d.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/gru.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/lstm.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/simple_rnn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/layers/rnn/time_distributed.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/backend.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/layers.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/losses.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/sequence.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/preprocessing/text.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/json_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/legacy_h5_format.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/saving_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/legacy/saving/serialization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/losses/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/losses/loss.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/losses/losses.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/accuracy_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/confusion_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/f_score_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/hinge_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/iou_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/metric.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/metrics_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/probabilistic_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/reduction_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/metrics/regression_metrics.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/models/cloning.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/models/functional.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/models/model.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/models/sequential.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/models/variable_mapping.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/core.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/function.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/image.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/linalg.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/math.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/nn.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/node.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/numpy.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1259,16 +1259,19 @@
         dtypes_to_resolve = [x.dtype]
         if self.weights is not None:
             weights = backend.convert_to_tensor(self.weights)
             dtypes_to_resolve.append(weights.dtype)
             dtype = dtypes.result_type(*dtypes_to_resolve)
         else:
             dtype = "int32"
+        x_sparse = getattr(x, "sparse", False)
         return KerasTensor(
-            list(x.shape[:-1]) + [None], dtype=dtype, sparse=self.sparse
+            list(x.shape[:-1]) + [None],
+            dtype=dtype,
+            sparse=x_sparse or self.sparse,
         )
 
 
 @keras_export(["keras.ops.bincount", "keras.ops.numpy.bincount"])
 def bincount(x, weights=None, minlength=0, sparse=False):
     """Count the number of occurrences of each value in a tensor of integers.
 
@@ -2068,15 +2071,16 @@
     def compute_output_spec(self, x, bins):
         bins_shape = bins.shape
         if len(bins_shape) > 1:
             raise ValueError(
                 f"`bins` must be a 1D array. Received: bins={bins} "
                 f"with shape bins.shape={bins_shape}"
             )
-        return KerasTensor(x.shape, dtype="int32")
+        sparse = getattr(x, "sparse", False)
+        return KerasTensor(x.shape, dtype="int32", sparse=sparse)
 
 
 @keras_export(["keras.ops.digitize", "keras.ops.numpy.digitize"])
 def digitize(x, bins):
     """Returns the indices of the bins to which each value in `x` belongs.
 
     Args:
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/operation.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/operation_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/ops/symbolic_arguments.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adadelta.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adafactor.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adagrad.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adam.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adamax.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/adamw.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/base_optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/base_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,22 @@
                     "`ema_overwrite_frequency` must be an integer >= 1 or "
                     "None. Received: ema_overwrite_frequency="
                     f"{ema_overwrite_frequency}"
                 )
         self.ema_momentum = ema_momentum
         self.ema_overwrite_frequency = ema_overwrite_frequency
 
-        if self.clipnorm is not None and self.global_clipnorm is not None:
+        clip_args_sum = sum(
+            a is not None for a in [clipnorm, clipvalue, global_clipnorm]
+        )
+        if clip_args_sum > 1:
             raise ValueError(
-                "Only one of `clipnorm` and `global_clipnorm` can "
-                f"be set. Received: clipnorm={self.clipnorm}, "
-                f"global_clipnorm={self.global_clipnorm}"
+                "Only one of `clipnorm`, `clipvalue` and `global_clipnorm` can "
+                f"be set. Received: clipnorm={clipnorm}, "
+                f"clipvalue={clipvalue}, global_clipnorm={global_clipnorm}"
             )
         self.built = False
 
         # Set up variable tracking.
         self._variables = []
         self._trainable_variables = []
         self._tracker = tracking.Tracker(
@@ -560,107 +563,120 @@
 
     def _get_current_learning_rate(self):
         if isinstance(
             self._learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             return self._learning_rate(self.iterations)
         elif callable(self._learning_rate):
-            return self._learning_rate(self.iterations)
+            return self._learning_rate()
         return self._learning_rate
 
     def _filter_empty_gradients(self, grads, vars):
-        for grad in grads:
-            if grad is None:
-                # Filtering is required.
-                filtered = [
-                    (g, v) for g, v in zip(grads, vars) if g is not None
-                ]
-                if not filtered:
-                    raise ValueError("No gradients provided for any variable.")
-                if len(filtered) < len(grads):
-                    missing_grad_vars = [
-                        v for g, v in zip(grads, vars) if g is None
-                    ]
-                    warnings.warn(
-                        "Gradients do not exist for variables "
-                        f"{[v.name for v in missing_grad_vars]} when "
-                        "minimizing the loss. If using `model.compile()`, "
-                        "did you forget to provide a `loss` argument?"
-                    )
-                return zip(*filtered)
-        return grads, vars
+        filtered_grads = list(grads)
+        filtered_vars = list(vars)
+        missing_grad_vars = []
+
+        # Iterate from right to left for safe popping
+        for i in range(len(filtered_grads) - 1, -1, -1):
+            if filtered_grads[i] is None:
+                filtered_grads.pop(i)
+                v = filtered_vars.pop(i)
+                missing_grad_vars.append(v.name)
+
+        if not filtered_grads:
+            raise ValueError("No gradients provided for any variable.")
+        if missing_grad_vars:
+            warnings.warn(
+                "Gradients do not exist for variables "
+                f"{list(reversed(missing_grad_vars))} when minimizing the loss."
+                " If using `model.compile()`, did you forget to provide a "
+                "`loss` argument?"
+            )
+        return filtered_grads, filtered_vars
 
     def _clip_gradients(self, grads):
         if self.clipnorm and self.clipnorm > 0:
-            clipped_grads = []
-            for g in grads:
-                if g is None:
-                    clipped_grads.append(g)
-                else:
-                    clipped_grads.append(self._clip_by_norm(g))
-            return clipped_grads
-
-        if self.global_clipnorm and self.global_clipnorm > 0:
+            return [
+                self._clip_by_norm(g) if g is not None else g for g in grads
+            ]
+        elif self.global_clipnorm and self.global_clipnorm > 0:
             return clip_by_global_norm(grads, self.global_clipnorm)
-
-        if self.clipvalue and self.clipvalue > 0:
-            clipped_grads = []
-            for g in grads:
-                if g is None:
-                    clipped_grads.append(g)
-                else:
-                    clipped_grads.append(
-                        ops.clip(g, -self.clipvalue, self.clipvalue)
-                    )
-            return clipped_grads
-        return grads
+        elif self.clipvalue and self.clipvalue > 0:
+            v = self.clipvalue
+            return [ops.clip(g, -v, v) if g is not None else g for g in grads]
+        else:
+            return grads
 
     def exclude_from_weight_decay(self, var_list=None, var_names=None):
         """Exclude variables from weight decay.
 
         This method must be called before the optimizer's `build` method is
         called. You can set specific variables to exclude out, or set a list of
         strings as the anchor words, if any of which appear in a variable's
         name, then the variable is excluded.
 
         Args:
-            var_list: A list of `tf.Variable`s to exclude from weight decay.
+            var_list: A list of `Variable`s to exclude from weight decay.
             var_names: A list of strings. If any string in `var_names` appear
                 in the model variable's name, then this model variable is
                 excluded from weight decay. For example, `var_names=['bias']`
                 excludes all bias variables from weight decay.
         """
         if hasattr(self, "_built") and self._built:
             raise ValueError(
                 "`exclude_from_weight_decay()` can only be configued before "
                 "the optimizer is built."
             )
 
+        # Use a `set` for the ids of `var_list` to speed up the searching
         if var_list:
-            self._exclude_from_weight_decay = [
+            self._exclude_from_weight_decay = set(
                 self._var_key(variable) for variable in var_list
-            ]
+            )
         else:
-            self._exclude_from_weight_decay = []
-        self._exclude_from_weight_decay_names = var_names or []
+            self._exclude_from_weight_decay = set()
+
+        # Precompile the pattern for `var_names` to speed up the searching
+        if var_names and len(var_names) > 0:
+            self._exclude_from_weight_decay_pattern = re.compile(
+                "|".join(set(var_names))
+            )
+        else:
+            self._exclude_from_weight_decay_pattern = None
+
+        # Reset cache
+        self._exclude_from_weight_decay_cache = dict()
 
     def _use_weight_decay(self, variable):
+        variable_id = self._var_key(variable)
+
+        # Immediately return the value if `variable_id` hits the cache
+        if not hasattr(self, "_exclude_from_weight_decay_cache"):
+            self._exclude_from_weight_decay_cache = dict()
+        if variable_id in self._exclude_from_weight_decay_cache:
+            return self._exclude_from_weight_decay_cache[variable_id]
+
+        # Determine whether the variable should apply weight decay or not
         exclude_from_weight_decay = getattr(
-            self, "_exclude_from_weight_decay", []
+            self, "_exclude_from_weight_decay", set()
         )
-        exclude_from_weight_decay_names = getattr(
-            self, "_exclude_from_weight_decay_names", []
+        exclude_from_weight_decay_pattern = getattr(
+            self, "_exclude_from_weight_decay_pattern", None
         )
-        variable_id = self._var_key(variable)
-        for exclude_id in exclude_from_weight_decay:
-            if variable_id == exclude_id:
-                return False
-        for name in exclude_from_weight_decay_names:
-            if re.search(name, variable.name) is not None:
+        if variable_id in exclude_from_weight_decay:
+            self._exclude_from_weight_decay_cache[variable_id] = False
+            return False
+        if exclude_from_weight_decay_pattern is not None:
+            if (
+                re.search(exclude_from_weight_decay_pattern, variable.name)
+                is not None
+            ):
+                self._exclude_from_weight_decay_cache[variable_id] = False
                 return False
+        self._exclude_from_weight_decay_cache[variable_id] = True
         return True
 
     def _apply_weight_decay(self, variables):
         if self.weight_decay is None:
             return
         for variable in variables:
             if self._use_weight_decay(variable):
@@ -864,30 +880,23 @@
             when your batch size is very small, in order to reduce gradient
             noise at each update step.
 """
 
 
 def global_norm(value_list):
     """Computes the global norm of multiple tensors."""
-    squared_norms = []
-    for v in value_list:
-        if v is not None:
-            squared_norms.append(ops.sum(ops.square(v)))
+    squared_norms = [
+        ops.sum(ops.square(v)) for v in value_list if v is not None
+    ]
     squared_norm = ops.sum(ops.stack(squared_norms))
     return ops.sqrt(squared_norm)
 
 
 def clip_by_global_norm(value_list, clip_norm):
     use_norm = global_norm(value_list)
     # Calculate L2-norm, clip elements by ratio of clip_norm to L2-norm
     scale_for_finite = clip_norm * ops.minimum(1.0 / use_norm, 1.0 / clip_norm)
     # If use_norm is any finite number, this is a no-op. For inf/-inf/NaN,
     # this will make scale NaN.
     scale = scale_for_finite + (use_norm - use_norm)
-    values_clipped = []
-    for v in value_list:
-        if v is None:
-            values_clipped.append(None)
-        else:
-            values_clipped.append(v * scale)
-    return values_clipped
+    return [v * scale if v is not None else v for v in value_list]
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/ftrl.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/lion.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/loss_scale_optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/nadam.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/optimizer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/optimizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.optimizers import base_optimizer
 
 if backend.backend() == "tensorflow":
-    from keras.src.backend.tensorflow.optimizer import TFOptimizer
-
-    BackendOptimizer = TFOptimizer
+    from keras.src.backend.tensorflow.optimizer import (
+        TFOptimizer as BackendOptimizer,
+    )
 elif backend.backend() == "torch":
-    from keras.src.backend.torch.optimizers import TorchOptimizer
-
-    BackendOptimizer = TorchOptimizer
+    from keras.src.backend.torch.optimizers import (
+        TorchOptimizer as BackendOptimizer,
+    )
 elif backend.backend() == "jax":
-    from keras.src.backend.jax.optimizer import JaxOptimizer
-
-    BackendOptimizer = JaxOptimizer
+    from keras.src.backend.jax.optimizer import JaxOptimizer as BackendOptimizer
 else:
-    BackendOptimizer = base_optimizer.BaseOptimizer
+
+    class BackendOptimizer(base_optimizer.BaseOptimizer):
+        pass
 
 
 @keras_export(["keras.Optimizer", "keras.optimizers.Optimizer"])
-class Optimizer(BackendOptimizer):
+class Optimizer(BackendOptimizer, base_optimizer.BaseOptimizer):
     pass
 
 
 base_optimizer_keyword_args = base_optimizer.base_optimizer_keyword_args
-Optimizer.__doc__ = base_optimizer.BaseOptimizer.__doc__
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/rmsprop.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/schedules/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/optimizers/sgd.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/quantizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/quantizers/quantizers.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/random/random.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/random/seed_generator.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/regularizers/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/regularizers/regularizers.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/saving/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/saving/object_registration.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/saving/saving_api.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/saving/saving_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/saving/serialization_lib.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/testing/test_case.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/testing/test_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/compile_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/array_slicing.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/data_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/epoch_iterator.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/trainers/trainer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/argument_validation.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/audio_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/backend_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/code_stats.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/dataset_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/dtype_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/file_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/image_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/image_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/io_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/jax_layer.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/model_visualization.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/module_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/naming.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/numerical_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/progbar.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/python_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/rng_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/sequence_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/summary_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/text_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/tf_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/timeseries_dataset_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/torch_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/traceback_utils.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/tracking.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tracking.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,27 +58,32 @@
     def __setattr__(self, name, value):
         if hasattr(self, "_tracker"):
             value = self._tracker.track(value)
         return super().__setattr__(name, value)
     ```
     """
 
-    def __init__(self, config):
+    def __init__(self, config, exclusions=None):
         self.config = config
         self.stored_ids = {name: set() for name in self.config.keys()}
         self.locked = False
         self._lock_violation_msg = None
+        self.exclusions = exclusions or {}
 
     def track(self, attr):
         if not is_tracking_enabled():
             return attr
 
         for store_name, (is_attr_type, _) in self.config.items():
             if is_attr_type(attr):
-                if id(attr) not in self.stored_ids[store_name]:
+                if store_name in self.exclusions:
+                    for excl in self.exclusions[store_name]:
+                        if self.is_in_store(excl, attr):
+                            return attr
+                if not self.is_in_store(store_name, attr):
                     self.add_to_store(store_name, attr)
                 return attr
         if isinstance(attr, tuple):
             wrapped_attr = []
             for e in attr:
                 wrapped_attr.append(self.track(e))
             # This should cover tuples and nametuples
@@ -108,14 +113,17 @@
 
     def add_to_store(self, store_name, value):
         if self.locked:
             raise ValueError(self._lock_violation_msg)
         self.config[store_name][1].append(value)
         self.stored_ids[store_name].add(id(value))
 
+    def is_in_store(self, store_name, value):
+        return id(value) in self.stored_ids[store_name]
+
 
 @optree.register_pytree_node_class(namespace="keras")
 class TrackedList(list):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = [tracker.track(v) for v in values]
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/src/utils/tree.py` & `keras-nightly-3.2.1.dev2024041103/keras/src/utils/tree.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/tree/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras/utils/__init__.py` & `keras-nightly-3.2.1.dev2024041103/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/PKG-INFO` & `keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.2.0.dev2024041003
+Version: 3.2.1.dev2024041103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras-nightly-3.2.0.dev2024041003/keras_nightly.egg-info/SOURCES.txt` & `keras-nightly-3.2.1.dev2024041103/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras-nightly-3.2.0.dev2024041003/setup.py` & `keras-nightly-3.2.1.dev2024041103/setup.py`

 * *Files identical despite different names*

