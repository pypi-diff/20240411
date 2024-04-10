# Comparing `tmp/rastervision_core-0.21.3.tar.gz` & `tmp/rastervision_core-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastervision_core-0.21.3.tar", last modified: Tue Oct 17 19:14:42 2023, max compression
+gzip compressed data, was "rastervision_core-0.30.0.tar", last modified: Wed Apr 10 22:11:08 2024, max compression
```

## Comparing `rastervision_core-0.21.3.tar` & `rastervision_core-0.30.0.tar`

### file list

```diff
@@ -1,165 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/
--rw-r--r--   0 root         (0) root         (0)       24 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      564 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/
--rw-rw-r--   0 root         (0) root         (0)      682 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/analyzer/
--rw-rw-r--   0 root         (0) root         (0)      371 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/analyzer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      417 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/analyzer/analyzer.py
--rw-rw-r--   0 root         (0) root         (0)      776 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/analyzer/analyzer_config.py
--rw-rw-r--   0 root         (0) root         (0)     1214 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/analyzer/stats_analyzer.py
--rw-rw-r--   0 root         (0) root         (0)     2351 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/analyzer/stats_analyzer_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/backend/
--rw-rw-r--   0 root         (0) root         (0)      184 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/backend/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1684 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/backend/backend.py
--rw-rw-r--   0 root         (0) root         (0)     1078 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/backend/backend_config.py
--rw-rw-r--   0 root         (0) root         (0)    17592 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/box.py
--rw-rw-r--   0 root         (0) root         (0)     3066 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/data/
--rw-rw-r--   0 root         (0) root         (0)      663 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5316 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/class_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/data/crs_transformer/
--rw-rw-r--   0 root         (0) root         (0)      359 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/crs_transformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6600 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/crs_transformer/crs_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      745 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/crs_transformer/identity_crs_transformer.py
--rw-rw-r--   0 root         (0) root         (0)     4861 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py
--rw-rw-r--   0 root         (0) root         (0)     3477 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/dataset_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/data/label/
--rw-rw-r--   0 root         (0) root         (0)      606 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6038 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label/chip_classification_labels.py
--rw-rw-r--   0 root         (0) root         (0)     2549 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label/labels.py
--rw-rw-r--   0 root         (0) root         (0)    12458 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label/object_detection_labels.py
--rw-rw-r--   0 root         (0) root         (0)    25695 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label/semantic_segmentation_labels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.007319 rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/
--rw-rw-r--   0 root         (0) root         (0)       15 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4366 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_list.py
--rw-rw-r--   0 root         (0) root         (0)    23023 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_list_ops.py
--rw-rw-r--   0 root         (0) root         (0)     3498 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_ops.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/label_source/
--rw-rw-r--   0 root         (0) root         (0)     1019 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10172 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/chip_classification_label_source.py
--rw-rw-r--   0 root         (0) root         (0)     4762 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/chip_classification_label_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     1787 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/label_source.py
--rw-rw-r--   0 root         (0) root         (0)      897 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/label_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     5106 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/object_detection_label_source.py
--rw-rw-r--   0 root         (0) root         (0)     1817 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/object_detection_label_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     4641 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/semantic_segmentation_label_source.py
--rw-rw-r--   0 root         (0) root         (0)     1376 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/label_store/
--rw-rw-r--   0 root         (0) root         (0)     1211 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2799 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/chip_classification_geojson_store.py
--rw-rw-r--   0 root         (0) root         (0)     1085 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/chip_classification_geojson_store_config.py
--rw-rw-r--   0 root         (0) root         (0)     1074 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/label_store.py
--rw-rw-r--   0 root         (0) root         (0)      892 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/label_store_config.py
--rw-rw-r--   0 root         (0) root         (0)     2825 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/object_detection_geojson_store.py
--rw-rw-r--   0 root         (0) root         (0)     1119 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/object_detection_geojson_store_config.py
--rw-rw-r--   0 root         (0) root         (0)    15122 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/semantic_segmentation_label_store.py
--rw-rw-r--   0 root         (0) root         (0)     6549 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py
--rw-rw-r--   0 root         (0) root         (0)     2897 2023-10-16 20:21:46.000000 rastervision_core-0.21.3/rastervision/core/data/label_store/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/raster_source/
--rw-rw-r--   0 root         (0) root         (0)     1107 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8577 2023-10-12 15:13:45.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/multi_raster_source.py
--rw-rw-r--   0 root         (0) root         (0)     3658 2023-09-26 17:05:06.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/multi_raster_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     6605 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/raster_source.py
--rw-rw-r--   0 root         (0) root         (0)     1983 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/raster_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     8741 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterio_source.py
--rw-rw-r--   0 root         (0) root         (0)     1920 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterio_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     5570 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterized_source.py
--rw-rw-r--   0 root         (0) root         (0)     2876 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterized_source_config.py
--rw-r--r--   0 root         (0) root         (0)     5103 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/temporal_multi_raster_source.py
--rw-r--r--   0 root         (0) root         (0)     8275 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_source/xarray_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/
--rw-rw-r--   0 root         (0) root         (0)     1612 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      922 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/cast_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      662 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/cast_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)      712 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/min_max_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      417 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/min_max_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)      956 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/nan_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      634 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/nan_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)      850 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/raster_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      550 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/raster_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)     1405 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/reclass_transformer.py
--rw-rw-r--   0 root         (0) root         (0)      593 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/reclass_transformer_config.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/rgb_class_transformer.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)     5835 2023-10-16 20:22:05.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/stats_transformer.py
--rw-rw-r--   0 root         (0) root         (0)     2311 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/raster_transformer/stats_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)     2814 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/scene.py
--rw-rw-r--   0 root         (0) root         (0)     3656 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/scene_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/utils/
--rw-r--r--   0 root         (0) root         (0)      325 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14881 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/utils/factory.py
--rw-r--r--   0 root         (0) root         (0)    13147 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/utils/geojson.py
--rw-r--r--   0 root         (0) root         (0)     8785 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)     2414 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/data/utils/raster.py
--rw-r--r--   0 root         (0) root         (0)     8270 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/utils/rasterio.py
--rw-r--r--   0 root         (0) root         (0)     6264 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/utils/vectorization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.011319 rastervision_core-0.21.3/rastervision/core/data/vector_source/
--rw-rw-r--   0 root         (0) root         (0)      455 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_source/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3532 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/vector_source/geojson_vector_source.py
--rw-rw-r--   0 root         (0) root         (0)     1497 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_source/geojson_vector_source_config.py
--rw-rw-r--   0 root         (0) root         (0)     6449 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/vector_source/vector_source.py
--rw-rw-r--   0 root         (0) root         (0)     2291 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_source/vector_source_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/
--rw-r--r--   0 root         (0) root         (0)      968 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/buffer_transformer.py
--rw-r--r--   0 root         (0) root         (0)     1834 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/buffer_transformer_config.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/class_inference_transformer.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/class_inference_transformer_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/label_maker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/label_maker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3488 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/label_maker/filter.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/shift_transformer.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/shift_transformer_config.py
--rw-r--r--   0 root         (0) root         (0)     1226 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/vector_transformer.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/data/vector_transformer/vector_transformer_config.py
--rw-rw-r--   0 root         (0) root         (0)      385 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/data_sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision/core/evaluation/
--rw-rw-r--   0 root         (0) root         (0)     1792 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1596 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/chip_classification_evaluation.py
--rw-rw-r--   0 root         (0) root         (0)      458 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/evaluation/chip_classification_evaluator.py
--rw-rw-r--   0 root         (0) root         (0)     1030 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/chip_classification_evaluator_config.py
--rw-rw-r--   0 root         (0) root         (0)     6285 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/evaluation/class_evaluation_item.py
--rw-rw-r--   0 root         (0) root         (0)     5523 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/evaluation/classification_evaluation.py
--rw-rw-r--   0 root         (0) root         (0)     1989 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/classification_evaluator.py
--rw-rw-r--   0 root         (0) root         (0)      299 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/classification_evaluator_config.py
--rw-rw-r--   0 root         (0) root         (0)      509 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/evaluation_item.py
--rw-rw-r--   0 root         (0) root         (0)     1289 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/evaluator.py
--rw-rw-r--   0 root         (0) root         (0)     1414 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/evaluator_config.py
--rw-rw-r--   0 root         (0) root         (0)     4339 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/object_detection_evaluation.py
--rw-rw-r--   0 root         (0) root         (0)      342 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/object_detection_evaluator.py
--rw-rw-r--   0 root         (0) root         (0)     1011 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/object_detection_evaluator_config.py
--rw-rw-r--   0 root         (0) root         (0)     1826 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluation.py
--rw-rw-r--   0 root         (0) root         (0)     1263 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluator.py
--rw-rw-r--   0 root         (0) root         (0)     1369 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py
--rw-rw-r--   0 root         (0) root         (0)     5506 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/predictor.py
--rw-rw-r--   0 root         (0) root         (0)    10644 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/raster_stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision/core/rv_pipeline/
--rw-rw-r--   0 root         (0) root         (0)     1184 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1533 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/chip_classification.py
--rw-rw-r--   0 root         (0) root         (0)      794 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/chip_classification_config.py
--rw-rw-r--   0 root         (0) root         (0)     7668 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/object_detection.py
--rw-rw-r--   0 root         (0) root         (0)     2865 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/object_detection_config.py
--rw-rw-r--   0 root         (0) root         (0)    10619 2023-10-16 20:21:53.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/rv_pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     5505 2023-09-14 17:47:42.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/rv_pipeline_config.py
--rw-rw-r--   0 root         (0) root         (0)     6157 2023-09-08 19:48:40.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/semantic_segmentation.py
--rw-rw-r--   0 root         (0) root         (0)     4734 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/semantic_segmentation_config.py
--rw-rw-r--   0 root         (0) root         (0)      794 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/rv_pipeline/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision/core/utils/
--rw-rw-r--   0 root         (0) root         (0)      102 2023-08-24 18:41:21.000000 rastervision_core-0.21.3/rastervision/core/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3261 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/utils/cog.py
--rw-rw-r--   0 root         (0) root         (0)      981 2023-08-22 15:58:07.000000 rastervision_core-0.21.3/rastervision/core/utils/filter_geojson.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/utils/misc.py
--rw-rw-r--   0 root         (0) root         (0)     6240 2023-09-26 14:00:58.000000 rastervision_core-0.21.3/rastervision/core/utils/stac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/rastervision_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      564 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7649 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      268 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-17 19:14:41.000000 rastervision_core-0.21.3/rastervision_core.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      268 2023-10-17 13:37:07.000000 rastervision_core-0.21.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-17 19:14:42.015319 rastervision_core-0.21.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1143 2023-10-17 13:37:07.000000 rastervision_core-0.21.3/setup.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.951692 rastervision_core-0.30.0/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       24 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/MANIFEST.in
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/PKG-INFO
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      744 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/__init__.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/analyzer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      371 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/analyzer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      404 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/analyzer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      776 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/analyzer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1214 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2351 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/backend/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      184 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/backend/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2143 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/backend/backend.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1078 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/backend/backend_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    18054 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/box.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3880 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/cli.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/data/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      663 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5315 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/class_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.939692 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      359 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6574 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      745 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/identity_crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4873 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3477 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/dataset_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      606 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6026 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label/chip_classification_labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2506 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label/labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    12458 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/object_detection_labels.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    26544 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/semantic_segmentation_labels.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       15 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4365 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    23023 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list_ops.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3498 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_ops.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1091 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1019 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10328 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4782 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      897 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5107 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1817 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3711 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1376 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/label_store/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1211 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2799 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1085 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1116 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/label_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      892 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/label_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2825 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1119 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    15901 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7087 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2897 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/label_store/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/raster_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1343 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8218 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3717 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6584 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2026 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8740 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1976 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5570 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2876 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1760 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/stac_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5030 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/temporal_multi_raster_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    11943 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2225 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.943692 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1612 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      922 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      662 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      712 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      417 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      956 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      634 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      837 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      550 2023-09-08 19:48:40.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1405 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      593 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2334 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      715 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5835 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2311 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2814 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/scene.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3656 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/scene_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      380 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7993 2024-04-09 23:04:37.000000 rastervision_core-0.30.0/rastervision/core/data/utils/aoi_sampler.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    14755 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/utils/factory.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    13266 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/utils/geojson.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8785 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/misc.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2415 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/raster.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8271 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/rasterio.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6264 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/utils/vectorization.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_source/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      455 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2024 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1491 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6518 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2345 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      968 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1834 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8483 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     2144 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer_config.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)        0 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/__init__.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     3488 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/filter.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     2290 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)     1153 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1213 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)      760 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      402 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/data_sample.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/evaluation/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1792 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1596 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      458 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1030 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6285 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/class_evaluation_item.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5510 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1989 2024-04-03 20:58:32.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      289 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      496 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluation_item.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1250 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1414 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     4340 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      342 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1011 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1826 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1263 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1366 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     8333 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/predictor.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)    10644 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/raster_stats.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/rv_pipeline/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1328 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      114 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      794 2024-02-06 21:37:22.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6655 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_options.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       99 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3509 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     9327 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6672 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      104 2024-04-06 20:13:30.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     5691 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation_config.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      798 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/rv_pipeline/utils.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision/core/utils/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      102 2023-08-24 18:41:21.000000 rastervision_core-0.30.0/rastervision/core/utils/__init__.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     3261 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/utils/cog.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      981 2023-08-22 15:58:07.000000 rastervision_core-0.30.0/rastervision/core/utils/filter_geojson.py
+-rw-r--r--   0 ahassan   (1001) ahassan   (1001)       65 2023-09-26 14:00:58.000000 rastervision_core-0.30.0/rastervision/core/utils/misc.py
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     6240 2024-04-07 00:38:15.000000 rastervision_core-0.30.0/rastervision/core/utils/stac.py
+drwxrwxr-x   0 ahassan   (1001) ahassan   (1001)        0 2024-04-10 22:11:08.947692 rastervision_core-0.30.0/rastervision_core.egg-info/
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      564 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/PKG-INFO
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     7852 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)        1 2024-04-10 21:24:48.000000 rastervision_core-0.30.0/rastervision_core.egg-info/not-zip-safe
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      168 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/requires.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       24 2024-04-10 22:11:08.000000 rastervision_core-0.30.0/rastervision_core.egg-info/top_level.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)      308 2024-04-10 21:55:37.000000 rastervision_core-0.30.0/requirements.txt
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)       38 2024-04-10 22:11:08.951692 rastervision_core-0.30.0/setup.cfg
+-rw-rw-r--   0 ahassan   (1001) ahassan   (1001)     1731 2024-04-10 21:55:10.000000 rastervision_core-0.30.0/setup.py
```

### Comparing `rastervision_core-0.21.3/PKG-INFO` & `rastervision_core-0.30.0/rastervision_core.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rastervision_core
-Version: 0.21.3
+Name: rastervision-core
+Version: 0.30.0
 Summary: A rastervision plugin that adds geospatial machine learning pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_core-0.21.3/rastervision/core/__init__.py` & `rastervision_core-0.30.0/rastervision/core/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # flake8: noqa
 
 
 def register_plugin(registry):
-    registry.set_plugin_version('rastervision.core', 10)
-    from rastervision.core.cli import predict
+    registry.set_plugin_version('rastervision.core', 13)
+    from rastervision.core.cli import predict, predict_scene
     registry.add_plugin_command(predict)
+    registry.add_plugin_command(predict_scene)
 
 
 import rastervision.pipeline
 from rastervision.core.box import *
 from rastervision.core.data_sample import *
 from rastervision.core.predictor import *
 from rastervision.core.raster_stats import *
```

### Comparing `rastervision_core-0.21.3/rastervision/core/analyzer/analyzer_config.py` & `rastervision_core-0.30.0/rastervision/core/analyzer/analyzer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/analyzer/stats_analyzer.py` & `rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/analyzer/stats_analyzer_config.py` & `rastervision_core-0.30.0/rastervision/core/analyzer/stats_analyzer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/backend/backend.py` & `rastervision_core-0.30.0/rastervision/core/backend/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,70 @@
+from typing import TYPE_CHECKING, Optional
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING
 from contextlib import AbstractContextManager
 
 if TYPE_CHECKING:
     from rastervision.core.data_sample import DataSample
-    from rastervision.core.data import Labels, Scene
+    from rastervision.core.data import DatasetConfig, Labels, Scene
+    from rastervision.core.rv_pipeline import ChipOptions, PredictOptions
 
 
 class SampleWriter(AbstractContextManager):
     """Writes DataSamples in a streaming fashion.
 
     This is a context manager used for creating training and validation chips, and
     should be subclassed for each Backend.
     """
 
     @abstractmethod
     def write_sample(self, sample: 'DataSample'):
         """Writes a single sample."""
-        pass
 
 
 class Backend(ABC):
     """Abstraction around core ML functionality used by an RVPipeline.
 
     This should be subclassed to enable use of a third party ML library with an
     RVPipeline. There is a one-to-many relationship from RVPipeline to Backend.
     """
 
     @abstractmethod
     def get_sample_writer(self):
         """Returns a SampleWriter for this Backend."""
-        pass
 
     @abstractmethod
     def train(self):
         """Train a model.
 
         This should download chips created by the SampleWriter, train the model, and
         then saving it to disk.
         """
-        pass
 
     @abstractmethod
-    def load_model(self):
-        """Load the model in preparation for one or more prediction calls."""
-        pass
+    def load_model(self, uri: Optional[str] = None):
+        """Load the model in preparation for one or more prediction calls.
+
+        Args:
+            uri: Optional URI to load the model from.
+        """
 
     @abstractmethod
-    def predict_scene(self, scene: 'Scene', chip_sz: int,
-                      stride: int) -> 'Labels':
+    def predict_scene(self, scene: 'Scene',
+                      predict_options: 'PredictOptions') -> 'Labels':
         """Return predictions for an entire scene using the model.
 
         Args:
-            scene (Scene): Scene to run inference on.
+            scene: Scene to run inference on.
+            predict_options: Prediction options.
 
         Return:
             Labels object containing predictions
         """
-        pass
+
+    @abstractmethod
+    def chip_dataset(self, dataset: 'DatasetConfig',
+                     chip_options: 'ChipOptions') -> None:
+        """Create and write chips for scenes in a :class:`.DatasetConfig`.
+
+        Args:
+            scenes: Scenes to chip.
+        """
```

### Comparing `rastervision_core-0.21.3/rastervision/core/backend/backend_config.py` & `rastervision_core-0.30.0/rastervision/core/backend/backend_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/box.py` & `rastervision_core-0.30.0/rastervision/core/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import (TYPE_CHECKING, Callable, Dict, List, Optional, Sequence,
-                    Tuple, Union)
-from typing_extensions import Literal
+from typing import (TYPE_CHECKING, Callable, Dict, List, Literal, Optional,
+                    Sequence, Tuple, Union)
 from pydantic import PositiveInt as PosInt, conint
 import math
 import random
 
 import numpy as np
 from shapely.geometry import Polygon
+from shapely.ops import unary_union
 from rasterio.windows import Window as RioWindow
 
 from rastervision.pipeline.utils import repr_with_args
 
 NonNegInt = conint(ge=0)
 
 if TYPE_CHECKING:
-    pass
+    from shapely.geometry import MultiPolygon
 
 
 class BoxSizeError(ValueError):
     pass
 
 
 class Box():
@@ -365,32 +365,32 @@
                     pad_direction: Literal['both', 'start', 'end'] = 'end'
                     ) -> List['Box']:
         """Returns a list of boxes representing windows generated using a
         sliding window traversal with the specified size, stride, and
         padding.
 
         Each of size, stride, and padding can be either a positive int or
-        a tuple `(vertical-componet, horizontal-component)` of positive ints.
+        a tuple `(vertical-component, horizontal-component)` of positive ints.
 
         Padding currently only applies to the right and bottom edges.
 
         Args:
             size (Union[PosInt, Tuple[PosInt, PosInt]]): Size (h, w) of the
                 windows.
             stride (Union[PosInt, Tuple[PosInt, PosInt]]): Step size between
                 windows. Can be 2-tuple (h_step, w_step) or positive int.
             padding (Optional[Union[PosInt, Tuple[PosInt, PosInt]]], optional):
-                Optional padding to accomodate windows that overflow the
+                Optional padding to accommodate windows that overflow the
                 extent. Can be 2-tuple (h_pad, w_pad) or non-negative int.
                 If None, will be set to (size[0]//2, size[1]//2).
                 Defaults to None.
             pad_direction (Literal['both', 'start', 'end']): If 'end', only pad
                 ymax and xmax (bottom and right). If 'start', only pad ymin and
                 xmin (top and left). If 'both', pad all sides. Has no effect if
-                paddiong is zero. Defaults to 'end'.
+                padding is zero. Defaults to 'end'.
 
         Returns:
             List[Box]: List of Box objects.
         """
         if not isinstance(size, tuple):
             size = (size, size)
 
@@ -456,36 +456,45 @@
     def filter_by_aoi(windows: List['Box'],
                       aoi_polygons: List[Polygon],
                       within: bool = True) -> List['Box']:
         """Filters windows by a list of AOI polygons
 
         Args:
             within: if True, windows are only kept if they lie fully within an
-                AOI polygon. Otherwise, windows are kept if they intersect an AOI
-                polygon.
+                AOI polygon. Otherwise, windows are kept if they intersect an
+                AOI polygon.
         """
-        result = []
-        for window in windows:
-            w = window.to_shapely()
-            for polygon in aoi_polygons:
-                if ((within and w.within(polygon))
-                        or ((not within) and w.intersects(polygon))):
-                    result.append(window)
-                    break
+        # merge overlapping polygons, if any
+        aoi_polygons: Polygon | MultiPolygon = unary_union(aoi_polygons)
+
+        if within:
+            keep_window = aoi_polygons.contains
+        else:
+            keep_window = aoi_polygons.intersects
 
-        return result
+        out = [w for w in windows if keep_window(w.to_shapely())]
+        return out
+
+    @staticmethod
+    def within_aoi(window: 'Box',
+                   aoi_polygons: Polygon | List[Polygon]) -> bool:
+        """Check if window is within the union of given AOI polygons."""
+        aoi_polygons: Polygon | MultiPolygon = unary_union(aoi_polygons)
+        w = window.to_shapely()
+        out = aoi_polygons.contains(w)
+        return out
 
     @staticmethod
-    def within_aoi(window: 'Box', aoi_polygons: List[Polygon]) -> bool:
-        """Check if window is within a list of AOI polygons."""
+    def intersects_aoi(window: 'Box',
+                       aoi_polygons: Polygon | List[Polygon]) -> bool:
+        """Check if window intersects with the union of given AOI polygons."""
+        aoi_polygons: Polygon | MultiPolygon = unary_union(aoi_polygons)
         w = window.to_shapely()
-        for polygon in aoi_polygons:
-            if w.within(polygon):
-                return True
-        return False
+        out = aoi_polygons.intersects(w)
+        return out
 
     def __contains__(self, query: Union['Box', Sequence]) -> bool:
         """Check if box or point is contained within this box.
 
         Args:
             query: Box or single point (x, y).
```

### Comparing `rastervision_core-0.21.3/rastervision/core/cli.py` & `rastervision_core-0.30.0/rastervision/core/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional
 import click
 
 from rastervision.pipeline.file_system import get_tmp_dir
-from rastervision.core.predictor import Predictor
+from rastervision.core.predictor import Predictor, ScenePredictor
 
 
 # https://stackoverflow.com/questions/48391777/nargs-equivalent-for-options-in-click
 class OptionEatAll(click.Option):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._previous_parser_process = None
@@ -76,7 +76,30 @@
     if channel_order is not None:
         channel_order: List[int] = [int(i) for i in channel_order]
 
     with get_tmp_dir() as tmp_dir:
         predictor = Predictor(model_bundle, tmp_dir, update_stats,
                               channel_order, scene_group)
         predictor.predict([image_uri], label_uri)
+
+
+@click.command(
+    'predict_scene',
+    short_help='Use a model bundle to predict on a new scene.')
+@click.argument('model_bundle_uri')
+@click.argument('scene_config_uri')
+@click.option(
+    '--predict_options_uri',
+    type=str,
+    default=None,
+    help='Optional URI to serialized Raster Vision PredictOptions config.')
+def predict_scene(model_bundle_uri: str,
+                  scene_config_uri: str,
+                  predict_options_uri: Optional[str] = None):
+    """Use a model-bundle to make predictions on a scene.
+
+    \b
+    MODEL_BUNDLE_URI    URI to a serialized Raster Vision model-bundle.
+    SCENE_CONFIG_URI    URI to a serialized Raster Vision SceneConfig.
+    """
+    predictor = ScenePredictor(model_bundle_uri, predict_options_uri)
+    predictor.predict(scene_config_uri)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/class_config.py` & `rastervision_core-0.30.0/rastervision/core/data/class_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         """Add a null class if one isn't set. This method is idempotent."""
         if self.null_class is not None:
             return
 
         null_class_name = DEFAULT_NULL_CLASS_NAME
         null_class_color = DEFAULT_NULL_CLASS_COLOR
 
-        # This might seeem redundant given the null class validator above, but
+        # This might seem redundant given the null class validator above, but
         # is actually important. Sometimes there can be multiple ClassConfig
         # instances that reference the same list objects for names and colors
         # (not clear why this happens). This means that
         # each ensure_null_class() call will add to names and colors in each
         # copy of ClassConfig but only set its own null_class, which makes this
         # method() non-idempotent.
         if null_class_name in self.names:
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/crs_transformer/crs_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/crs_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,21 +163,19 @@
         Args:
             map_point: (x, y) tuple in map coordinates (eg. lon/lat). x and y
             can be single values or array-like.
 
         Returns:
             Tuple[int, int]: (x, y) tuple in pixel coordinates.
         """
-        pass
 
     @abstractmethod
     def _pixel_to_map(self, point: Tuple[float, float]) -> Tuple[float, float]:
         """Transform point from pixel to map coordinates.
 
         Args:
             pixel_point: (x, y) tuple in pixel coordinates. x and y can be
             single values or array-like.
 
         Returns:
             Tuple[float, float]: (x, y) tuple in map coordinates (eg. lon/lat).
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/crs_transformer/identity_crs_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/identity_crs_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/crs_transformer/rasterio_crs_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import Any, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 from pyproj import Transformer
 
 import numpy as np
 import rasterio as rio
 from rasterio.transform import (rowcol, xy)
 from rasterio import Affine
 
 from rastervision.core.data.crs_transformer import (CRSTransformer,
                                                     IdentityCRSTransformer)
 
+if TYPE_CHECKING:
+    from typing import Self
+
 
 class RasterioCRSTransformer(CRSTransformer):
     """Transformer for a RasterioRasterSource."""
 
     def __init__(self,
                  transform: Affine,
                  image_crs: Any,
@@ -120,16 +123,16 @@
 
         if transform is None:
             transform = Affine.identity()
 
         return cls(transform, image_crs, map_crs, **kwargs)
 
     @classmethod
-    def from_uri(cls, uri: str, map_crs: Optional[str] = 'epsg:4326', **kwargs
-                 ) -> Union[IdentityCRSTransformer, 'RasterioCRSTransformer']:
+    def from_uri(cls, uri: str, map_crs: Optional[str] = 'epsg:4326',
+                 **kwargs) -> 'Self':
         """Build from raster URI.
 
         Args:
             uri (Any): Raster URI.
             map_crs (Optional[str]): Target map CRS. Defaults to 'epsg:4326'.
             **kwargs: Extra args for :meth:`.__init__`.
         """
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/dataset_config.py` & `rastervision_core-0.30.0/rastervision/core/data/dataset_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/label/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/chip_classification_labels.py` & `rastervision_core-0.30.0/rastervision/core/data/label/chip_classification_labels.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def __setitem__(self, window: Box,
                     value: Tuple[int, Optional[Sequence[float]]]):
         class_id, scores = value
         self.set_cell(window, class_id, scores=scores)
 
     @classmethod
     def from_predictions(cls, windows: Iterable['Box'],
-                         predictions: Iterable[Any]) -> 'Labels':
+                         predictions: Iterable[Any]):
         """Overrid to convert predictions to (class_id, scores) pairs."""
         predictions = ((np.argmax(p), p) for p in predictions)
         return super().from_predictions(windows, predictions)
 
     @classmethod
     def make_empty(cls) -> 'ChipClassificationLabels':
         return ChipClassificationLabels()
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/labels.py` & `rastervision_core-0.30.0/rastervision/core/data/label/labels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 """Defines the abstract Labels class."""
 
 from typing import TYPE_CHECKING, Any, Iterable, List
-from abc import (ABC, abstractclassmethod, abstractmethod)
+from abc import ABC, abstractmethod
 
 if TYPE_CHECKING:
+    from typing import Self
     from shapely.geometry import Polygon
     from rastervision.core.box import Box
 
 
 class Labels(ABC):
     """A source-agnostic, in-memory representation of labels in a scene.
 
     This class can represent labels obtained via a ``LabelSource``, a
     ``LabelStore``, or directly from model predictions.
     """
 
     @abstractmethod
-    def __add__(self, other: 'Labels'):
+    def __add__(self, other: 'Self'):
         """Add labels to these labels.
 
         Returns a concatenation of this and the other labels.
         """
-        pass
 
     @abstractmethod
-    def filter_by_aoi(self, aoi_polygons: List['Polygon']) -> 'Labels':
+    def filter_by_aoi(self, aoi_polygons: List['Polygon']) -> 'Self':
         """Return a copy of these labels filtered by given AOI polygons.
 
         Args:
           aoi_polygons: List of AOI polygons to filter by, in pixel
             coordinates.
         """
-        pass
 
     @abstractmethod
     def __eq__(self, other: 'Labels'):
         pass
 
     @abstractmethod
     def __setitem__(self, key, value):
         pass
 
-    @abstractclassmethod
-    def make_empty(cls) -> 'Labels':
+    @classmethod
+    @abstractmethod
+    def make_empty(cls) -> 'Self':
         """Instantiate an empty instance of this class.
 
         Returns:
             Labels: An object of the Label subclass on which this method is
             called.
         """
-        pass
 
     @classmethod
     def from_predictions(cls, windows: Iterable['Box'],
-                         predictions: Iterable[Any]) -> 'Labels':
+                         predictions: Iterable[Any]) -> 'Self':
         """Instantiate from windows and their corresponding predictions.
 
         This makes no assumptions about the type or format of the predictions.
         Subclasses should implement the __setitem__ method to correctly handle
         the predictions.
 
         Args:
@@ -76,8 +75,7 @@
         for prediction, window in zip(predictions, windows):
             labels[window] = prediction
         return labels
 
     @abstractmethod
     def save(self, uri: str) -> None:
         """Save to file."""
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/object_detection_labels.py` & `rastervision_core-0.30.0/rastervision/core/data/label/object_detection_labels.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/semantic_segmentation_labels.py` & `rastervision_core-0.30.0/rastervision/core/data/label/semantic_segmentation_labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,44 +31,55 @@
         self.ymin, self.xmin, self.width, self.height = extent.to_xywh()
         self.dtype = dtype
 
     @abstractmethod
     def __add__(self, other: 'SemanticSegmentationLabels'
                 ) -> 'SemanticSegmentationLabels':
         """Merge self with other labels."""
-        pass
 
     def __setitem__(self, window: Box, values: np.ndarray) -> None:
         """Set labels for the given window."""
         self.add_window(window, values)
 
     @abstractmethod
     def __delitem__(self, window: Box) -> None:
         """Delete labels for the given window."""
-        pass
 
     @abstractmethod
     def __getitem__(self, window: Box) -> np.ndarray:
         """Get labels for the given window."""
-        pass
 
     @abstractmethod
     def add_window(self, window: Box, values: np.ndarray) -> List[Box]:
         """Set labels for the given window."""
-        pass
 
     @abstractmethod
     def get_label_arr(self, window: Box,
                       null_class_id: int = -1) -> np.ndarray:
         """Get labels as a 2D array of class IDs.
 
         Note: The returned array is not guaranteed to be the same size as the
         input window.
         """
-        pass
+
+    @abstractmethod
+    def get_score_arr(self, window: Box,
+                      null_class_id: int = -1) -> np.ndarray:
+        """Get (C, H, W) array of pixel scores."""
+
+    def get_class_mask(self,
+                       window: Box,
+                       class_id: int,
+                       threshold: Optional[float] = None) -> np.ndarray:
+        """Get a binary mask representing all pixels of a class."""
+        scores = self.get_score_arr(window)
+        if threshold is None:
+            threshold = (1 / self.num_classes)
+        mask = scores[class_id] >= threshold
+        return mask
 
     def get_windows(self, **kwargs) -> List[Box]:
         """Generate sliding windows over the local extent.
 
         The keyword args are passed to :meth:`.Box.get_windows` and can
         therefore be used to control the specifications of the windows.
 
@@ -105,15 +116,14 @@
 
     @abstractmethod
     def mask_fill(self, window: Box, mask: np.ndarray,
                   fill_value: Any) -> None:
         """Given a window and a binary mask, set all the pixels in the window
         for which the mask is ON to the fill_value.
         """
-        pass
 
     def _filter_window_by_aoi(self, window: Box, aoi_polygons: List['Polygon'],
                               null_class_id: int) -> None:
         window_geom = window.to_shapely()
         label_arr = self[window]
 
         # For each aoi_polygon, intersect with window, and
@@ -125,15 +135,15 @@
 
                 def transform_shape(x, y, z=None):
                     return (x - window.xmin, y - window.ymin)
 
                 window_aoi = transform(transform_shape, window_aoi)
                 window_aois.append(window_aoi)
 
-        # If window does't overlap with any AOI, then it won't be in
+        # If window doesn't overlap with any AOI, then it won't be in
         # new_labels.
         if window_aois:
             # If window intersects with AOI, set pixels outside the
             # AOI polygon to 0 so they are ignored during eval.
             mask = rasterize(
                 [(p, 0) for p in window_aois],
                 out_shape=label_arr.shape[-2:],
@@ -289,23 +299,28 @@
         self.pixel_counts[..., y0:y1, x0:x1] = 0
         self.hit_mask[y0:y1, x0:x1] = False
 
     def __getitem__(self, window: Box) -> np.ndarray:
         return self.get_label_arr(window)
 
     def add_window(self, window: Box, pixel_class_ids: np.ndarray) -> None:
+        # sub-window in self.extent coords to write to
         window_dst = window.intersection(self.extent)
-        dst_yslice, dst_xslice = window_dst.to_slices()
-        # pixel_class_scores coords
+
+        # sub-window in pixel_class_ids coords to read from
         window_src = window_dst.to_global_coords(
             self.extent).to_local_coords(window)
-        src_yslice, src_xslice = window_src.to_slices()
 
+        # read sub-window from source array
+        src_yslice, src_xslice = window_src.to_slices()
         pixel_class_ids = pixel_class_ids.astype(self.dtype)
         pixel_class_ids = pixel_class_ids[..., src_yslice, src_xslice]
+
+        # write sub-window in destination array
+        dst_yslice, dst_xslice = window_dst.to_slices()
         window_pixel_counts = self.pixel_counts[:, dst_yslice, dst_xslice]
         for ch_class_id, ch in enumerate(window_pixel_counts):
             ch[pixel_class_ids == ch_class_id] += 1
         self.hit_mask[dst_yslice, dst_xslice] = True
 
     def get_label_arr(self, window: Box,
                       null_class_id: int = -1) -> np.ndarray:
@@ -464,24 +479,28 @@
         self.pixel_scores[..., y0:y1, x0:x1] = 0
         self.pixel_hits[..., y0:y1, x0:x1] = 0
 
     def __getitem__(self, window: Box) -> np.ndarray:
         return self.get_score_arr(window)
 
     def add_window(self, window: Box, pixel_class_scores: np.ndarray) -> None:
-        # self.extent coords
+        # sub-window in self.extent coords to write to
         window_dst = window.intersection(self.extent)
-        dst_yslice, dst_xslice = window_dst.to_slices()
-        # pixel_class_scores coords
+
+        # sub-window in pixel_class_scores coords to read from
         window_src = window_dst.to_global_coords(
             self.extent).to_local_coords(window)
-        src_yslice, src_xslice = window_src.to_slices()
 
+        # read sub-window from source array
+        src_yslice, src_xslice = window_src.to_slices()
         pixel_class_scores = pixel_class_scores.astype(self.dtype)
         pixel_class_scores = pixel_class_scores[..., src_yslice, src_xslice]
+
+        # write sub-window in destination array
+        dst_yslice, dst_xslice = window_dst.to_slices()
         self.pixel_scores[..., dst_yslice, dst_xslice] += pixel_class_scores
         self.pixel_hits[dst_yslice, dst_xslice] += 1
 
     def get_score_arr(self, window: Box) -> np.ndarray:
         """Get array of pixel scores."""
         y0, x0, y1, x1 = window.intersection(self.extent)
         scores = self.pixel_scores[..., y0:y1, x0:x1]
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_list.py` & `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]: a 4-tuple
             of 1-d numpy arrays [y_min, x_min, y_max, x_max].
         """
         boxes = self.get_field('boxes')
         return tuple(boxes.T)
 
     def _is_valid_boxes(self, data: np.ndarray) -> bool:
-        """Check whether data fullfills the format of N*[ymin, xmin, ymax, xmin].
+        """Check whether data fulfills the format of N*[ymin, xmin, ymax, xmin].
 
         Args:
             data (np.ndarray): Box coords as a [N, 4] numpy array.
 
         Returns:
             bool: Whether ymin <= ymax and xmin <= xmax.
         """
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_list_ops.py` & `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_list_ops.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/tfod_utils/np_box_ops.py` & `rastervision_core-0.30.0/rastervision/core/data/label/tfod_utils/np_box_ops.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label/utils.py` & `rastervision_core-0.30.0/rastervision/core/data/label/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/chip_classification_label_source.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,17 +109,21 @@
     Returns:
        ChipClassificationLabels
     """
     boxes = [Box.from_shapely(g).to_int() for g in labels_df.geometry]
     if bbox is not None:
         boxes = [b for b in boxes if b.intersects(bbox)]
     class_ids = labels_df['class_id'].astype(int)
+    if 'scores' in labels_df.columns:
+        scores = labels_df['scores']
+    else:
+        scores = [None] * len(class_ids)
     cells_to_class_id = {
-        cell: (class_id, None)
-        for cell, class_id in zip(boxes, class_ids)
+        cell: (class_id, class_scores)
+        for cell, class_id, class_scores in zip(boxes, class_ids, scores)
     }
     labels = ChipClassificationLabels(cells_to_class_id)
     return labels
 
 
 class ChipClassificationLabelSource(LabelSource):
     """A source of chip classification labels.
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/chip_classification_label_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/chip_classification_label_source_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     infer_cells: bool = Field(
         False,
         description='If True, infers a grid of cells based on the cell_sz.')
     cell_sz: Optional[int] = Field(
         None,
         description=
         ('Size of a cell to use in pixels. If None, and this Config is part '
-         'of an RVPipeline, this field will be set from RVPipeline.train_chip_sz.'
+         'of an RVPipeline, this field will be set from RVPipeline.chip_options.'
          ))
     lazy: bool = Field(
         False,
         description='If True, labels will not be populated automatically '
         'during initialization of the label source.')
 
     @validator('vector_source')
@@ -103,10 +103,10 @@
         vector_source = self.vector_source.build(class_config, crs_transformer)
         return ChipClassificationLabelSource(
             self, vector_source, bbox=bbox, lazy=self.lazy)
 
     def update(self, pipeline=None, scene=None):
         super().update(pipeline, scene)
         if self.cell_sz is None and pipeline is not None:
-            self.cell_sz = pipeline.train_chip_sz
+            self.cell_sz = pipeline.chip_options.get_chip_sz(scene.id)
         if self.vector_source is not None:
             self.vector_source.update(pipeline, scene)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/label_source.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/label_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TYPE_CHECKING, Any, Optional
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 
 from rastervision.core.box import Box
 from rastervision.core.data.utils import parse_array_slices_2d
 
 if TYPE_CHECKING:
     from rastervision.core.data import CRSTransformer, Labels
 
@@ -24,39 +24,38 @@
         Args:
             window: Box
 
         Returns:
             Labels overlapping with window. If window is None, returns all
             labels.
         """
-        pass
 
     @property
     def extent(self) -> 'Box':
         """Extent of the ``LabelSource``."""
         return self.bbox.extent
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def bbox(self) -> 'Box':
         """Bounding box applied to the source."""
-        pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def crs_transformer(self) -> 'CRSTransformer':
-        pass
+        """Associated :class:`.CRSTransformer`."""
 
     @abstractmethod
     def set_bbox(self, extent: 'Box') -> None:
         """Set self.extent to the given value.
 
         .. note:: This method is idempotent.
 
         Args:
             extent (Box): User-specified extent in pixel coordinates.
         """
-        pass
 
     def __getitem__(self, key: Any) -> Any:
         if isinstance(key, Box):
             raise NotImplementedError()
         window, _ = parse_array_slices_2d(key, extent=self.extent)
         return self[window]
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/label_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/object_detection_label_source.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         """Constructor.
 
         Args:
             vector_source (VectorSource): A VectorSource.
             bbox (Optional[Box], optional): User-specified crop of the extent.
                 If None, the full extent available in the source file is used.
             ioa_thresh (Optional[float], optional): IOA threshold to apply when
-                retieving labels for a window. Defaults to None.
+                retrieving labels for a window. Defaults to None.
             clip (bool, optional): Clip bounding boxes to window limits when
                 retrieving labels for a window. Defaults to False.
         """
         self.vector_source = vector_source
         geojson = self.vector_source.get_geojson()
         self.validate_geojson(geojson)
         self.labels = ObjectDetectionLabels.from_geojson(geojson, bbox=bbox)
@@ -48,15 +48,15 @@
         """Get labels (in global coords) for a window.
 
         Args:
             window (Box): Window coords.
 
         Returns:
             ObjectDetectionLabels: Labels with sufficient overlap with the
-            window. The returned labels are in global coods (i.e. coords wihtin
+            window. The returned labels are in global coods (i.e. coords within
             the full extent of the source).
         """
         if window is None:
             return self.labels
         window = window.to_global_coords(self.bbox)
         return ObjectDetectionLabels.get_overlapping(
             self.labels, window, ioa_thresh=ioa_thresh, clip=clip)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/object_detection_label_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/object_detection_label_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/semantic_segmentation_label_source.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, List, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 import numpy as np
 
 from rastervision.core.box import Box
 from rastervision.core.data import ClassConfig
 from rastervision.core.data.label import SemanticSegmentationLabels
 from rastervision.core.data.label_source.label_source import LabelSource
@@ -32,36 +32,14 @@
                 If None, the full extent available in the source file is used.
         """
         self.raster_source = raster_source
         self.class_config = class_config
         if bbox is not None:
             self.set_bbox(bbox)
 
-    def enough_target_pixels(self, window: Box, target_count_threshold: int,
-                             target_classes: List[int]) -> bool:
-        """Check if window contains enough pixels of the given target classes.
-
-        Args:
-             window: The larger window from-which the sub-window will
-                  be clipped.
-             target_count_threshold:  Minimum number of target pixels.
-             target_classes: The classes of interest.  The given
-                  window is examined to make sure that it contains a
-                  sufficient number of target pixels.
-        Returns:
-             True (the window does contain interesting pixels) or False.
-        """
-        label_arr = self.get_label_arr(window)
-
-        target_count = 0
-        for class_id in target_classes:
-            target_count += (label_arr == class_id).sum()
-
-        return target_count >= target_count_threshold
-
     def get_labels(self,
                    window: Optional[Box] = None) -> SemanticSegmentationLabels:
         """Get labels for a window.
 
         Args:
             window (Optional[Box], optional): Window to get labels for. If
             None, returns labels covering the full extent of the scene.
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_source/semantic_segmentation_label_source_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 from rastervision.core.data.raster_source import (RasterSourceConfig,
                                                   RasterizedSourceConfig)
 from rastervision.core.data.label_source import (
     LabelSourceConfig, SemanticSegmentationLabelSource)
 from rastervision.pipeline.config import (register_config, Field)
 
 
-def ss_label_source_config_upgrader(cfg_dict: dict, version: int) -> dict:
-    if version < 4:
-        try:
-            # removed in version 4
-            del cfg_dict['rgb_class_config']
-        except KeyError:
-            pass
+def ss_label_source_config_upgrader(cfg_dict: dict,
+                                    version: int) -> dict:  # pragma: no cover
+    if version == 3:
+        # removed in version 4
+        cfg_dict.pop('rgb_class_config', None)
     return cfg_dict
 
 
 @register_config(
     'semantic_segmentation_label_source',
     upgrader=ss_label_source_config_upgrader)
 class SemanticSegmentationLabelSourceConfig(LabelSourceConfig):
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/chip_classification_geojson_store.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/chip_classification_geojson_store_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/chip_classification_geojson_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/label_store.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/label_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 from typing import TYPE_CHECKING, Optional
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 
 if TYPE_CHECKING:
     from rastervision.core.box import Box
     from rastervision.core.data import CRSTransformer
 
 
 class LabelStore(ABC):
     """This defines how to store prediction labels for a scene."""
 
     @abstractmethod
     def save(self, labels):
         """Save.
 
         Args:
-           labels - Labels to be saved, the type of which will be dependant on the type
+           labels - Labels to be saved, the type of which will be dependent on the type
                     of pipeline.
         """
-        pass
 
     @abstractmethod
     def get_labels(self):
         """Loads Labels from this label store."""
-        pass
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def bbox(self) -> Optional['Box']:
-        pass
+        """Bounding box applied to the source."""
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def crs_transformer(self) -> 'CRSTransformer':
-        pass
+        """Associated :class:`.CRSTransformer`."""
 
     @abstractmethod
     def set_bbox(self, extent: 'Box') -> None:
         """Set self.extent to the given value.
 
         .. note:: This method is idempotent.
 
         Args:
             extent (Box): User-specified extent in pixel coordinates.
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/label_store_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/label_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/object_detection_geojson_store.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/object_detection_geojson_store_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/object_detection_geojson_store_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/semantic_segmentation_label_store.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,18 +79,14 @@
                 scores as np.uint8 (0-255) values rather than as np.float32
                 discrete labels, to help save memory/disk space.
                 Defaults to False.
             rasterio_block_size (int, optional): Value to set blockxsize and
                 blockysize to. Defaults to 512.
         """
         self.root_uri = uri
-        self.label_uri = join(uri, 'labels.tif')
-        self.score_uri = join(uri, 'scores.tif')
-        self.hits_uri = join(uri, 'pixel_hits.npy')
-        self.vector_output_uri = join(uri, 'vector_output')
 
         self.tmp_dir = tmp_dir
         if self.tmp_dir is None:
             self._tmp_dir = get_tmp_dir()
             self.tmp_dir = self._tmp_dir.name
 
         self.vector_outputs = vector_outputs
@@ -201,65 +197,71 @@
         More info on rasterio IO:
         - https://github.com/mapbox/rasterio/blob/master/docs/quickstart.rst
         - https://rasterio.readthedocs.io/en/latest/topics/windowed-rw.html
 
         Args:
             labels - (SemanticSegmentationLabels) labels to be saved
         """
-        local_root = get_local_path(self.root_uri, self.tmp_dir)
-        make_dir(local_root)
+        make_dir(self.root_uri_local)
 
-        height, width = labels.extent.size
-        if self.bbox is not None:
-            bbox_rio_window = self.bbox.rasterio_format()
-            transform = rio_windows.transform(bbox_rio_window,
-                                              self.crs_transformer.transform)
-        else:
-            transform = self.crs_transformer.transform
-        out_profile = dict(
-            driver='GTiff',
-            height=height,
-            width=width,
-            transform=transform,
-            crs=self.crs_transformer.image_crs,
-            blockxsize=min(self.rasterio_block_size, width),
-            blockysize=min(self.rasterio_block_size, height))
+        out_profile = self.build_rasterio_gtiff_profile(labels)
         if profile is not None:
             out_profile.update(profile)
 
         if self.discrete_output:
             labels_path = get_local_path(self.label_uri, self.tmp_dir)
             self.write_discrete_raster_output(out_profile, labels_path, labels)
 
         if self.smooth_output:
             # if old scores exist, combine them with the new ones
             if self.score_source is not None:
                 log.info('Old scores found. '
                          'Attempting to merge with current scores.')
-                old_extent = self.score_source.extent
-                new_extent = labels.extent
-                if old_extent != new_extent:
-                    raise ValueError('Cannot merge with old sores. '
-                                     'Non-identical extents:\n'
-                                     f'old extent: {old_extent}\n'
-                                     f'new extent: {new_extent}')
-                old_labels = self.get_scores()
-                labels += old_labels
-
+                labels = self.merge_with_old_scores(labels)
             scores_path = get_local_path(self.score_uri, self.tmp_dir)
             hits_path = get_local_path(self.hits_uri, self.tmp_dir)
             self.write_smooth_raster_output(out_profile, scores_path,
                                             hits_path, labels)
 
-        if self.vector_outputs is not None:
-            vector_output_dir = get_local_path(self.vector_output_uri,
-                                               self.tmp_dir)
-            self.write_vector_outputs(labels, vector_output_dir)
+        if self.vector_outputs:
+            self.write_vector_outputs(labels, self.vector_output_dir_local)
 
-        sync_to_dir(local_root, self.root_uri)
+        sync_to_dir(self.root_uri_local, self.root_uri)
+
+    def build_rasterio_gtiff_profile(
+            self, labels: SemanticSegmentationLabels) -> dict:
+        height, width = labels.extent.size
+        if self.bbox is not None:
+            bbox_rio_window = self.bbox.rasterio_format()
+            transform = rio_windows.transform(bbox_rio_window,
+                                              self.crs_transformer.transform)
+        else:
+            transform = self.crs_transformer.transform
+        out_profile = dict(
+            driver='GTiff',
+            height=height,
+            width=width,
+            transform=transform,
+            crs=self.crs_transformer.image_crs,
+            blockxsize=min(self.rasterio_block_size, width),
+            blockysize=min(self.rasterio_block_size, height))
+        return out_profile
+
+    def merge_with_old_scores(self, labels: SemanticSegmentationSmoothLabels
+                              ) -> SemanticSegmentationSmoothLabels:
+        old_extent = self.score_source.extent
+        new_extent = labels.extent
+        if old_extent != new_extent:
+            raise ValueError('Cannot merge with old sores. '
+                             'Non-identical extents:\n'
+                             f'old extent: {old_extent}\n'
+                             f'new extent: {new_extent}')
+        old_labels = self.get_scores()
+        labels += old_labels
+        return labels
 
     def write_smooth_raster_output(
             self, out_profile: dict, scores_path: str, hits_path: str,
             labels: SemanticSegmentationSmoothLabels) -> None:
         num_bands = labels.num_classes
         dtype = np.uint8 if self.smooth_as_uint8 else np.float32
         out_profile.update(dict(count=num_bands, dtype=dtype))
@@ -303,33 +305,36 @@
                         label_arr = self.class_transformer.class_to_rgb(
                             label_arr)
                     write_window(ds, label_arr, window)
 
     def write_vector_outputs(self, labels: SemanticSegmentationLabels,
                              vector_output_dir: str) -> None:
         """Write vectorized outputs for all configs in self.vector_outputs."""
-        from rastervision.core.data.utils import geoms_to_geojson
-
         log.info('Writing vector outputs to disk.')
 
-        label_arr = labels.get_label_arr(labels.extent,
-                                         self.class_config.null_class_id)
-
         with tqdm(self.vector_outputs, desc='Vectorizing predictions') as bar:
             for vo in bar:
                 bar.set_postfix(vo.dict())
-                class_mask = (label_arr == vo.class_id).astype(np.uint8)
-                polys = vo.vectorize(class_mask)
-                polys = [
-                    self.crs_transformer.pixel_to_map(p, bbox=self.bbox)
-                    for p in polys
-                ]
-                geojson = geoms_to_geojson(polys)
-                out_uri = vo.get_uri(vector_output_dir, self.class_config)
-                json_to_file(geojson, out_uri)
+                class_mask = labels.get_class_mask(labels.extent, vo.class_id,
+                                                   vo.threshold)
+                self.write_vector_output(vo, class_mask, vector_output_dir)
+
+    def write_vector_output(self, vo: 'VectorOutputConfig', mask: np.ndarray,
+                            vector_output_dir: str) -> None:
+        """Write vector output for a single ``VectorOutputConfig``."""
+        from rastervision.core.data.utils import geoms_to_geojson
+
+        mask = mask.astype(np.uint8)
+        polys = vo.vectorize(mask)
+        polys = [
+            self.crs_transformer.pixel_to_map(p, bbox=self.bbox) for p in polys
+        ]
+        geojson = geoms_to_geojson(polys)
+        out_uri = vo.get_uri(vector_output_dir, self.class_config)
+        json_to_file(geojson, out_uri)
 
     def _clip_to_extent(self,
                         extent: Box,
                         window: Box,
                         arr: Optional[np.ndarray] = None
                         ) -> Tuple[Box, Optional[np.ndarray]]:
         clipped_window = window.intersection(extent)
@@ -349,9 +354,33 @@
     def bbox(self) -> 'Box':
         return self._bbox
 
     @property
     def crs_transformer(self) -> 'CRSTransformer':
         return self._crs_transformer
 
+    @property
+    def label_uri(self) -> str:
+        return join(self.root_uri, 'labels.tif')
+
+    @property
+    def score_uri(self) -> str:
+        return join(self.root_uri, 'scores.tif')
+
+    @property
+    def hits_uri(self) -> str:
+        return join(self.root_uri, 'pixel_hits.npy')
+
+    @property
+    def vector_output_uri(self) -> str:
+        return join(self.root_uri, 'vector_output')
+
+    @property
+    def root_uri_local(self) -> str:
+        return get_local_path(self.root_uri, self.tmp_dir)
+
+    @property
+    def vector_output_dir_local(self) -> str:
+        return get_local_path(self.vector_output_uri, self.tmp_dir)
+
     def set_bbox(self, bbox: 'Box') -> None:
         self._bbox = bbox
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/semantic_segmentation_label_store_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,23 @@
         8,
         description='Diameter of the circular structural element used to '
         'remove high-frequency signals from the image. Smaller values will '
         'reduce less noise and make vectorization slower and more memory '
         'intensive (especially for large images). Larger values will remove '
         'more noise and make vectorization faster but might also remove '
         'legitimate detections.')
+    threshold: Optional[float] = Field(
+        None,
+        description='Probability threshold for creating the binary mask for '
+        'the pixels of this class. Pixels will be considered to belong to '
+        'this class if their probability for this class is >= ``threshold``. '
+        'Note that Raster Vision treats classes as mutually exclusive so the '
+        'threshold should vary with the number of total classes. '
+        '``None`` is equivalent to setting this to (1 / num_classes). '
+        'Defaults to ``None``.')
 
     def vectorize(self, mask: 'np.ndarray') -> Iterator['BaseGeometry']:
         """Vectorize binary mask representing the target class into polygons.
         """
         raise NotImplementedError()
 
     def get_uri(self, root: str,
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/label_store/utils.py` & `rastervision_core-0.30.0/rastervision/core/data/label_store/utils.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 from rastervision.core.data.raster_source.rasterio_source import *
 from rastervision.core.data.raster_source.rasterio_source_config import *
 from rastervision.core.data.raster_source.rasterized_source import *
 from rastervision.core.data.raster_source.rasterized_source_config import *
 from rastervision.core.data.raster_source.multi_raster_source import *
 from rastervision.core.data.raster_source.multi_raster_source_config import *
 from rastervision.core.data.raster_source.xarray_source import *
+from rastervision.core.data.raster_source.xarray_source_config import *
 from rastervision.core.data.raster_source.temporal_multi_raster_source import *
+from rastervision.core.data.raster_source.stac_config import *
 
 __all__ = [
     RasterSource.__name__,
     RasterSourceConfig.__name__,
     RasterioSource.__name__,
     RasterioSourceConfig.__name__,
     RasterizedSource.__name__,
     RasterizedSourceConfig.__name__,
     RasterizerConfig.__name__,
     MultiRasterSource.__name__,
     MultiRasterSourceConfig.__name__,
     XarraySource.__name__,
+    XarraySourceConfig.__name__,
     TemporalMultiRasterSource.__name__,
+    STACItemConfig.__name__,
+    STACItemCollectionConfig.__name__,
 ]
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/multi_raster_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             raster_transformers (Sequence, optional): Sequence of transformers.
                 Defaults to [].
             bbox (Optional[Box], optional): User-specified crop of the extent.
                 If given, the primary raster source's bbox is set to this.
                 If None, the full extent available in the source file of the
                 primary raster source is used.
         """
-        num_channels_raw = sum(rs.num_channels_raw for rs in raster_sources)
+        num_channels_raw = sum(rs.num_channels for rs in raster_sources)
         if not channel_order:
             num_channels = sum(rs.num_channels for rs in raster_sources)
             channel_order = list(range(num_channels))
 
         # validate primary_source_idx
         if not (0 <= primary_source_idx < len(raster_sources)):
             raise IndexError('primary_source_idx must be in range '
@@ -100,20 +100,21 @@
     def dtype(self) -> np.dtype:
         return self.primary_source.dtype
 
     @property
     def crs_transformer(self) -> CRSTransformer:
         return self.primary_source.crs_transformer
 
-    def _get_sub_chips(
-            self,
-            window: Box,
-            raw: bool = False,
-            out_shape: Optional[Tuple[int, int]] = None) -> List[np.ndarray]:
-        """If all extents are identical, simply retrieves chips from each sub
+    def _get_sub_chips(self,
+                       window: Box,
+                       out_shape: Optional[Tuple[int, int]] = None
+                       ) -> List[np.ndarray]:
+        """Return chips from sub raster sources as a list.
+
+        If all extents are identical, simply retrieves chips from each sub
         raster source. Otherwise, follows the following algorithm
             - using pixel-coords window, get chip from the primary sub raster
             source
             - convert window to world coords using the CRS of the primary sub
             raster source
             - for each remaining sub raster source
                 - convert world-coords window to pixel coords using the sub
@@ -121,38 +122,30 @@
                 - get chip from the sub raster source using this window;
                 specify `out_shape` when reading to ensure shape matches
                 reference chip from the primary sub raster source
 
         Args:
             window (Box): The window for which to get the chip, in pixel
                 coordinates.
-            raw (bool, optional): If True, uses RasterSource._get_chip.
-                Otherwise, RasterSource.get_chip. Defaults to False.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             List[np.ndarray]: List of chips from each sub raster source.
         """
 
         def get_chip(
                 rs: RasterSource,
                 window: Box,
                 map: bool = False,
                 out_shape: Optional[Tuple[int, int]] = None) -> np.ndarray:
-            if raw:
-                if map:
-                    func = rs._get_chip_by_map_window
-                else:
-                    func = rs._get_chip
+            if map:
+                func = rs.get_chip_by_map_window
             else:
-                if map:
-                    func = rs.get_chip_by_map_window
-                else:
-                    func = rs.get_chip
+                func = rs.get_chip
             return func(window, out_shape=out_shape)
 
         primary_rs = self.primary_source
         other_rses = self.non_primary_sources
 
         primary_sub_chip = get_chip(primary_rs, window, out_shape=out_shape)
         if out_shape is None:
@@ -170,28 +163,26 @@
             sub_chips = [chip.astype(dtype) for chip in sub_chips]
 
         return sub_chips
 
     def _get_chip(self,
                   window: Box,
                   out_shape: Optional[Tuple[int, int]] = None) -> np.ndarray:
-        """Return the raw chip located in the window.
-
-        Get raw chips from sub raster sources and concatenate them.
+        """Get chip w/o applying channel_order and transformers.
 
         Args:
             window (Box): The window for which to get the chip, in pixel
                 coordinates.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             [height, width, channels] numpy array
         """
-        sub_chips = self._get_sub_chips(window, raw=True, out_shape=out_shape)
+        sub_chips = self._get_sub_chips(window, out_shape=out_shape)
         chip = np.concatenate(sub_chips, axis=-1)
         return chip
 
     def get_chip(self,
                  window: Box,
                  out_shape: Optional[Tuple[int, int]] = None) -> np.ndarray:
         """Return the transformed chip in the window.
@@ -205,15 +196,15 @@
                 coordinates.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             np.ndarray with shape [height, width, channels]
         """
-        sub_chips = self._get_sub_chips(window, raw=False, out_shape=out_shape)
+        sub_chips = self._get_sub_chips(window, out_shape=out_shape)
         chip = np.concatenate(sub_chips, axis=-1)
         chip = chip[..., self.channel_order]
 
         for transformer in self.raster_transformers:
             chip = transformer.transform(chip, self.channel_order)
 
         return chip
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/multi_raster_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/multi_raster_source_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from pydantic import conint, conlist
 
 from rastervision.pipeline.config import (Field, register_config, validator)
 from rastervision.core.box import Box
 from rastervision.core.data.raster_source import (RasterSourceConfig,
                                                   MultiRasterSource)
 
@@ -53,15 +54,16 @@
     def validate_temporal(cls, v: int, values: dict):
         channel_order = values.get('channel_order')
         if v and channel_order is not None:
             raise ValueError(
                 'Setting channel_order is not allowed if temporal=True.')
         return v
 
-    def build(self, tmp_dir: str,
+    def build(self,
+              tmp_dir: Optional[str] = None,
               use_transformers: bool = True) -> MultiRasterSource:
         if use_transformers:
             raster_transformers = [t.build() for t in self.transformers]
         else:
             raster_transformers = []
 
         built_raster_sources = [
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/raster_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TYPE_CHECKING, Any, List, Optional, Tuple
-from abc import ABC, abstractmethod, abstractproperty
+from abc import ABC, abstractmethod
 
 import numpy as np
 from skimage.transform import resize
 
 from rastervision.core.box import Box
 from rastervision.core.data.utils import parse_array_slices_Nd
 
@@ -61,33 +61,33 @@
 
     @property
     def shape(self) -> Tuple[int, int, int]:
         """Shape of the raster as a (height, width, num_channels) tuple."""
         H, W = self.bbox.size
         return H, W, self.num_channels
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def dtype(self) -> 'np.dtype':
         """``numpy.dtype`` of the chips read from this source."""
-        pass
 
     @property
     def bbox(self) -> 'Box':
         """Bounding box applied to the source imagery."""
         return self._bbox
 
     @property
     def extent(self) -> 'Box':
         """Extent of the ``RasterSource``."""
         return self.bbox.extent
 
-    @abstractproperty
+    @property
+    @abstractmethod
     def crs_transformer(self) -> 'CRSTransformer':
         """Associated :class:`.CRSTransformer`."""
-        pass
 
     def set_bbox(self, bbox: 'Box') -> None:
         """Set self.bbox to the given value.
 
         .. note:: This method is idempotent.
 
         Args:
@@ -105,15 +105,14 @@
             window (Box): The window for which to get the chip.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             [height, width, channels] numpy array
         """
-        pass
 
     def __getitem__(self, key: Any) -> 'np.ndarray':
         if isinstance(key, Box):
             return self.get_chip(key)
 
         window, (h, w, c) = parse_array_slices_Nd(
             key, extent=self.extent, dims=3)
@@ -150,15 +149,15 @@
 
     def get_chip_by_map_window(
             self,
             window_map_coords: 'Box',
             out_shape: Optional[Tuple[int, int]] = None) -> 'np.ndarray':
         """Same as get_chip(), but input is a window in map coords. """
         window_pixel_coords = self.crs_transformer.map_to_pixel(
-            window_map_coords, bbox=self.bbox)
+            window_map_coords, bbox=self.bbox).normalize()
         chip = self.get_chip(window_pixel_coords, out_shape=out_shape)
         return chip
 
     def _get_chip_by_map_window(
             self,
             window_map_coords: 'Box',
             out_shape: Optional[Tuple[int, int]] = None) -> 'np.ndarray':
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/raster_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/raster_source_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from rastervision.core.data.raster_transformer import RasterTransformerConfig
 
 if TYPE_CHECKING:
     from rastervision.core.data import (RasterSource, SceneConfig)
     from rastervision.core.rv_pipeline import RVPipelineConfig
 
 
-def rs_config_upgrader(cfg_dict: dict, version: int) -> dict:
+def rs_config_upgrader(cfg_dict: dict,
+                       version: int) -> dict:  # pragma: no cover
     if version == 6:
         # removed in version 7
         if cfg_dict.get('extent_crop') is not None:
             raise ConfigError('RasterSourceConfig.extent_crop is deprecated.')
         try:
             del cfg_dict['extent_crop']
         except KeyError:
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterio_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         return self._dtype
 
     @property
     def crs_transformer(self) -> RasterioCRSTransformer:
         return self._crs_transformer
 
     def _set_info_from_chip(self):
-        """Read 1x1 chip to get info not statically inferrable."""
+        """Read 1x1 chip to get info not statically inferable."""
         test_chip = self.get_chip(Box(0, 0, 1, 1))
         self._dtype = test_chip.dtype
         self._num_channels = test_chip.shape[-1]
 
     def download_data(self,
                       vrt_dir: Optional[str] = None,
                       stream: bool = False) -> str:
@@ -179,15 +179,15 @@
         Args:
             window (Box): Bounding box of chip in pixel coordinates.
             bands (Optional[Union[Sequence[int], slice]], optional): Subset of
                 bands to read. Note that this will be applied on top of the
                 channel_order (if specified). So if this is an RGB image and
                 channel_order=[2, 1, 0], then using bands=[0] will return the
                 B-channel. Defaults to None.
-            out_shape (Optional[Tuple[int, ...]], optional): (hieght, width) of
+            out_shape (Optional[Tuple[int, ...]], optional): (height, width) of
                 the output chip. If None, no resizing is done.
                 Defaults to None.
 
         Returns:
             np.ndarray: A chip of shape (height, width, channels).
         """
         if bands is None or bands == slice(None):
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterio_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterio_source_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import List, Union
 
 from rastervision.core.box import Box
 from rastervision.core.data.raster_source import RasterSourceConfig, RasterioSource
 from rastervision.pipeline.config import ConfigError, Field, register_config
 
 
-def rasterio_source_config_upgrader(cfg_dict: dict, version: int) -> dict:
+def rasterio_source_config_upgrader(cfg_dict: dict,
+                                    version: int) -> dict:  # pragma: no cover
     if version == 5:
         # removed in version 6
         x_shift = cfg_dict.get('x_shift', 0)
         y_shift = cfg_dict.get('y_shift', 0)
         if x_shift != 0 or y_shift != 0:
             raise ConfigError('x_shift and y_shift are deprecated. '
                               'Use the ShiftTransformer instead.')
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterized_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/rasterized_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/rasterized_source_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/temporal_multi_raster_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/temporal_multi_raster_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,28 +69,26 @@
         ]
 
         self.validate_raster_sources()
 
     def _get_chip(self,
                   window: Box,
                   out_shape: Optional[Tuple[int, int]] = None) -> np.ndarray:
-        """Return the raw chip located in the window.
-
-        Get raw chips from sub raster sources and stack them.
+        """Get chip w/o applying channel_order and transformers.
 
         Args:
             window (Box): The window for which to get the chip, in pixel
                 coordinates.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             np.ndarray: 4D array of shape (T, H, W, C).
         """
-        sub_chips = self._get_sub_chips(window, raw=True, out_shape=out_shape)
+        sub_chips = self._get_sub_chips(window, out_shape=out_shape)
         chip = np.stack(sub_chips)
         return chip
 
     def get_chip(self,
                  window: Box,
                  out_shape: Optional[Tuple[int, int]] = None) -> np.ndarray:
         """Return the transformed chip in the window.
@@ -104,15 +102,15 @@
                 coordinates.
             out_shape (Optional[Tuple[int, int]]): (height, width) to resize
                 the chip to.
 
         Returns:
             np.ndarray: 4D array of shape (T, H, W, C).
         """
-        sub_chips = self._get_sub_chips(window, raw=False, out_shape=out_shape)
+        sub_chips = self._get_sub_chips(window, out_shape=out_shape)
         chip = np.stack(sub_chips)
 
         for transformer in self.raster_transformers:
             chip = transformer.transform(chip, self.channel_order)
 
         return chip
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_source/xarray_source.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_source/xarray_source.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from rastervision.core.box import Box
 from rastervision.core.data.crs_transformer import RasterioCRSTransformer
 from rastervision.core.data.raster_source import RasterSource
 from rastervision.core.data.utils import parse_array_slices_Nd, fill_overflow
 
 if TYPE_CHECKING:
+    from pystac import Item, ItemCollection
     from rastervision.core.data import RasterTransformer, CRSTransformer
 
 log = logging.getLogger(__name__)
 
 
 class XarraySource(RasterSource):
     """A RasterSource for reading an Xarry DataArray.
@@ -22,15 +23,14 @@
     """
 
     def __init__(self,
                  data_array: DataArray,
                  crs_transformer: 'CRSTransformer',
                  raster_transformers: List['RasterTransformer'] = [],
                  channel_order: Optional[Sequence[int]] = None,
-                 num_channels_raw: Optional[int] = None,
                  bbox: Optional[Box] = None,
                  temporal: bool = False):
         """Constructor.
 
         Args:
             uris (Union[str, List[str]]): One or more URIs of images. If more
                 than one, the images will be mosaiced together using GDAL.
@@ -59,37 +59,115 @@
                     'If temporal=False, data_array must have 3 dimensions: '
                     '"x", "y", and "band" (in any order).')
 
         self.data_array = data_array.transpose(..., 'y', 'x', 'band')
         self.ndim = data_array.ndim
         self._crs_transformer = crs_transformer
 
-        if num_channels_raw is None:
-            num_channels_raw = len(data_array.band)
+        num_channels_raw = len(data_array.band)
         if channel_order is None:
             channel_order = np.arange(num_channels_raw, dtype=int)
         else:
             channel_order = np.array(channel_order, dtype=int)
         self._num_channels = None
         self._dtype = None
         if len(raster_transformers) == 0:
             self._num_channels = len(channel_order)
             self._dtype = data_array.dtype
 
         height, width = len(data_array.y), len(data_array.x)
         self.full_extent = Box(0, 0, height, width)
         if bbox is None:
             bbox = self.full_extent
+        else:
+            if bbox not in self.full_extent:
+                new_bbox = bbox.intersection(self.full_extent)
+                log.warning(f'Clipping ({bbox}) to the DataArray\'s '
+                            f'full extent ({self.full_extent}). '
+                            f'New bbox={new_bbox}')
+                bbox = new_bbox
 
         super().__init__(
             channel_order,
             num_channels_raw,
             raster_transformers=raster_transformers,
             bbox=bbox)
 
+    @classmethod
+    def from_stac(
+            cls,
+            item_or_item_collection: Union['Item', 'ItemCollection'],
+            raster_transformers: List['RasterTransformer'] = [],
+            channel_order: Optional[Sequence[int]] = None,
+            bbox: Optional[Box] = None,
+            bbox_map_coords: Optional[Box] = None,
+            temporal: bool = False,
+            allow_streaming: bool = False,
+            stackstac_args: dict = dict(rescale=False)) -> 'XarraySource':
+        """Construct an ``XarraySource`` from a STAC Item or ItemCollection.
+
+        Args:
+            item_or_item_collection: STAC Item or ItemCollection.
+            raster_transformers: RasterTransformers to use to transform chips
+                after they are read.
+            channel_order: List of indices of channels to extract from raw
+                imagery. Can be a subset of the available channels. If None,
+                all channels available in the image will be read.
+                Defaults to None.
+            bbox: User-specified crop of the extent. If None, the full extent
+                available in the source file is used. Mutually exclusive with
+                ``bbox_map_coords``. Defaults to ``None``.
+            bbox_map_coords: User-specified bbox in EPSG:4326 coords of the
+                form (ymin, xmin, ymax, xmax). Useful for cropping the raster
+                source so that only part of the raster is read from. Mutually
+                exclusive with ``bbox``. Defaults to ``None``.
+            temporal: If True, data_array is expected to have a "time"
+                dimension and the chips returned will be of shape (T, H, W, C).
+            allow_streaming: If False, load the entire DataArray into memory.
+                Defaults to True.
+            stackstac_args: Optional arguments to pass to stackstac.stack().
+        """
+        import stackstac
+
+        data_array = stackstac.stack(item_or_item_collection, **stackstac_args)
+
+        if not temporal and 'time' in data_array.dims:
+            if len(data_array.time) > 1:
+                raise ValueError('temporal=False but len(data_array.time) > 1')
+            data_array = data_array.isel(time=0)
+
+        if not allow_streaming:
+            from humanize import naturalsize
+            log.info('Loading the full DataArray into memory '
+                     f'({naturalsize(data_array.nbytes)}).')
+            data_array.load()
+
+        crs_transformer = RasterioCRSTransformer(
+            transform=data_array.transform, image_crs=data_array.crs)
+
+        if bbox is not None:
+            if bbox_map_coords is not None:
+                raise ValueError('Specify either bbox or bbox_map_coords, '
+                                 'but not both.')
+            bbox = Box(*bbox)
+        elif bbox_map_coords is not None:
+            bbox_map_coords = Box(*bbox_map_coords)
+            bbox = crs_transformer.map_to_pixel(bbox_map_coords).normalize()
+        else:
+            bbox = None
+
+        raster_source = XarraySource(
+            data_array,
+            crs_transformer=crs_transformer,
+            raster_transformers=raster_transformers,
+            channel_order=channel_order,
+            bbox=bbox,
+            temporal=temporal)
+        return raster_source
+
     @property
     def shape(self) -> Tuple[int, int, int]:
         """Shape of the raster as a (height, width, num_channels) tuple."""
         H, W = self.bbox.size
         if self.temporal:
             T = len(self.data_array.time)
             return T, H, W, self.num_channels
@@ -117,40 +195,43 @@
         return self._dtype
 
     @property
     def crs_transformer(self) -> RasterioCRSTransformer:
         return self._crs_transformer
 
     def _set_info_from_chip(self):
-        """Read 1x1 chip to get info not statically inferrable."""
+        """Read 1x1 chip to get info not statically inferable."""
         test_chip = self.get_chip(Box(0, 0, 1, 1))
         self._dtype = test_chip.dtype
         self._num_channels = test_chip.shape[-1]
 
     def _get_chip(self,
                   window: Box,
                   bands: Union[int, Sequence[int], slice] = slice(None),
                   time: Union[int, Sequence[int], slice] = slice(None),
                   out_shape: Optional[Tuple[int, ...]] = None) -> np.ndarray:
         window = window.to_global_coords(self.bbox)
 
-        yslice, xsclice = window.to_slices()
+        window_within_bbox = window.intersection(self.bbox)
+
+        yslice, xslice = window_within_bbox.to_slices()
         if self.temporal:
             chip = self.data_array.isel(
-                x=xsclice, y=yslice, band=bands, time=time).to_numpy()
+                x=xslice, y=yslice, band=bands, time=time).to_numpy()
         else:
             chip = self.data_array.isel(
-                x=xsclice, y=yslice, band=bands).to_numpy()
+                x=xslice, y=yslice, band=bands).to_numpy()
 
-        *batch_dims, h, w, c = chip.shape
-        if window.size != (h, w):
-            window_actual = window.intersection(self.full_extent)
-            yslice, xsclice = window_actual.to_local_coords(window).to_slices()
+        if window != window_within_bbox:
+            *batch_dims, h, w, c = chip.shape
+            # coords of window_within_bbox within window
+            yslice, xslice = window_within_bbox.to_local_coords(
+                window).to_slices()
             tmp = np.zeros((*batch_dims, *window.size, c))
-            tmp[..., yslice, xsclice, :] = chip
+            tmp[..., yslice, xslice, :] = chip
             chip = tmp
 
         chip = fill_overflow(self.bbox, window, chip)
         if out_shape is not None:
             chip = self.resize(chip, out_shape)
         return chip
 
@@ -164,15 +245,15 @@
         Args:
             window (Box): Bounding box of chip in pixel coordinates.
             bands (Optional[Union[Sequence[int], slice]], optional): Subset of
                 bands to read. Note that this will be applied on top of the
                 channel_order (if specified). So if this is an RGB image and
                 channel_order=[2, 1, 0], then using bands=[0] will return the
                 B-channel. Defaults to None.
-            out_shape (Optional[Tuple[int, ...]], optional): (hieght, width) of
+            out_shape (Optional[Tuple[int, ...]], optional): (height, width) of
                 the output chip. If None, no resizing is done.
                 Defaults to None.
 
         Returns:
             np.ndarray: A chip of shape (height, width, channels).
         """
         if bands is None or bands == slice(None):
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/cast_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/cast_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/cast_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/min_max_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/min_max_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/nan_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/nan_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/nan_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/raster_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,7 @@
                 words, channels should be equal to len(channel_order).
             channel_order: list of indices of channels that were extracted from the
                 raw imagery.
 
         Returns:
             (np.ndarray): Array of shape (..., H, W, C)
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/raster_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/raster_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/reclass_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/reclass_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/reclass_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/rgb_class_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/rgb_class_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/stats_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/raster_transformer/stats_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/raster_transformer/stats_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/scene.py` & `rastervision_core-0.30.0/rastervision/core/data/scene.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/scene_config.py` & `rastervision_core-0.30.0/rastervision/core/data/scene_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/factory.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             Defaults to None.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for label data, if label_raster_uri is
@@ -95,15 +95,14 @@
             class_inf_tf = ClassInferenceTransformer(
                 default_class_id=label_vector_default_class_id)
             vector_tfs = label_vector_source_kw.get('vector_transformers', [])
             label_vector_source_kw['vector_transformers'] = (
                 [class_inf_tf] + vector_tfs)
         vector_source = GeoJSONVectorSource(
             uris=label_vector_uri,
-            ignore_crs_field=True,
             crs_transformer=crs_transformer,
             **label_vector_source_kw)
         label_raster_source = RasterizedSource(
             vector_source=vector_source,
             background_class_id=label_raster_source_kw.pop(
                 'background_class_id', class_config.null_class_id),
             bbox=bbox,
@@ -148,15 +147,15 @@
             Defaults to None.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_vector_source_kw (dict, optional): Additional arguments to pass
             to the GeoJSONVectorSourceConfig used for label data, if
@@ -192,17 +191,15 @@
             # add a ClassInferenceTransformer to the VectorSource
             class_inf_tf = ClassInferenceTransformerConfig(
                 default_class_id=label_vector_default_class_id)
             vector_tfs = label_vector_source_kw.get('transformers', [])
             label_vector_source_kw['transformers'] = (
                 [class_inf_tf] + vector_tfs)
         geojson_cfg = GeoJSONVectorSourceConfig(
-            uris=label_vector_uri,
-            ignore_crs_field=True,
-            **label_vector_source_kw)
+            uris=label_vector_uri, **label_vector_source_kw)
         # use config to ensure required transformers are auto added
         label_source_cfg = ChipClassificationLabelSourceConfig(
             vector_source=geojson_cfg, **label_source_kw)
         label_source = label_source_cfg.build(
             class_config, crs_transformer, bbox=bbox)
 
     aoi_polygons = get_polygons_from_uris(aoi_uri, crs_transformer)
@@ -239,15 +236,15 @@
             Defaults to None.
         aoi_uri (Union[str, List[str]], optional): URI or list of URIs of
             GeoJSONs that specify the area-of-interest. If provided, the
             dataset will only access data from this area. Defaults to [].
         label_vector_default_class_id (Optional[int], optional): If using
             label_vector_uri and all polygons in that file belong to the same
             class and they do not contain a `class_id` property, then use this
-            argument to map all of the polgons to the appropriate class ID.
+            argument to map all of the polygons to the appropriate class ID.
             See docs for ClassInferenceTransformer for more details.
             Defaults to None.
         image_raster_source_kw (dict, optional): Additional arguments to pass
             to the RasterioSource used for image data. See docs for
             RasterioSource for more details. Defaults to {}.
         label_vector_source_kw (dict, optional): Additional arguments to pass
             to the GeoJSONVectorSourceConfig used for label data, if
@@ -283,17 +280,15 @@
             # add a ClassInferenceTransformer to the VectorSource
             class_inf_tf = ClassInferenceTransformerConfig(
                 default_class_id=label_vector_default_class_id)
             vector_tfs = label_vector_source_kw.get('transformers', [])
             label_vector_source_kw['transformers'] = (
                 [class_inf_tf] + vector_tfs)
         geojson_cfg = GeoJSONVectorSourceConfig(
-            uris=label_vector_uri,
-            ignore_crs_field=True,
-            **label_vector_source_kw)
+            uris=label_vector_uri, **label_vector_source_kw)
         # use config to ensure required transformers are auto added
         label_source_cfg = ObjectDetectionLabelSourceConfig(
             vector_source=geojson_cfg, **label_source_kw)
         label_source = label_source_cfg.build(
             class_config, crs_transformer, bbox=bbox)
 
     aoi_polygons = get_polygons_from_uris(aoi_uri, crs_transformer)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/geojson.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/geojson.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,27 +104,32 @@
     geoms = (shape(f['geometry']) for f in geojson['features'])
     return geoms
 
 
 def geoms_to_geojson(geoms: Iterable['BaseGeometry'],
                      properties: Optional[Iterable[dict]] = None) -> dict:
     """Serialize shapely geometries to GeoJSON."""
-    if properties is None:
-        features = [geom_to_feature(g) for g in geoms]
-    else:
-        features = [geom_to_feature(g, p) for g, p in zip(geoms, properties)]
+    with tqdm(
+            geoms,
+            delay=PROGRESSBAR_DELAY_SEC,
+            mininterval=0.5,
+            desc='Serializing geoms') as bar:
+        if properties is None:
+            features = [geom_to_feature(g) for g in bar]
+        else:
+            features = [geom_to_feature(g, p) for g, p in zip(bar, properties)]
     geojson = features_to_geojson(features)
     return geojson
 
 
 def geom_to_feature(geom: 'BaseGeometry',
                     properties: Optional[dict] = None) -> dict:
-    """Serialize a single shapely geomety to a GeoJSON Feature."""
-    geomety = mapping(geom)
-    feature = geometry_to_feature(geomety, properties=properties)
+    """Serialize a single shapely geometry to a GeoJSON Feature."""
+    geometry = mapping(geom)
+    feature = geometry_to_feature(geometry, properties=properties)
     return feature
 
 
 def filter_features(func: Callable,
                     geojson: dict,
                     progressbar_kw: Optional[dict] = None) -> dict:
     """Filter GeoJSON features. Returns a new GeoJSON dict."""
@@ -247,15 +252,15 @@
         geojson,
         progressbar_kw=dict(desc='Transforming to map coords'))
 
 
 def simplify_polygons(geojson: dict) -> dict:
     """Simplify polygon geometries by applying ``.buffer(0)``.
 
-    For Polygon geomtries, ``.buffer(0)`` can do the following:
+    For Polygon geometries, ``.buffer(0)`` can do the following:
 
     1.  *Sometimes* break up a polygon with "bowties" into multiple polygons.
         (See https://github.com/shapely/shapely/issues/599.)
     2.  *Sometimes* "simplify" polygons. See shapely documentation for
         :meth:`.BaseGeometry.buffer`.
 
     Args:
@@ -339,18 +344,15 @@
                            map_coords: bool = False) -> List['BaseGeometry']:
     """Load and return polygons (in pixel coords) from one or more URIs."""
 
     # use local imports to avoid circular import problems
     from rastervision.core.data import GeoJSONVectorSource
 
     source = GeoJSONVectorSource(
-        uris=uris,
-        ignore_crs_field=True,
-        crs_transformer=crs_transformer,
-        bbox=bbox)
+        uris=uris, crs_transformer=crs_transformer, bbox=bbox)
     polygons = source.get_geoms(to_map_coords=map_coords)
     return polygons
 
 
 def merge_geojsons(geojsons: Iterable[dict]) -> dict:
     """Merge features from all given GeoJSONs into one GeoJSON."""
     features = sum([g.get('features', []) for g in geojsons], [])
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/misc.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/misc.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/raster.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                   fill_value: int = 0) -> np.ndarray:
     """Where ``chip``'s ``window`` overflows bbox, fill with ``fill_value``.
 
     Args:
         bbox (Box): Bounding box.
         window (Box): Window corresponding to the ``chip``.
         chip (np.ndarray): (H, W, C) array.
-        fill_value (int, optional): Value to set oveflowing pixels to.
+        fill_value (int, optional): Value to set overflowing pixels to.
             Defaults to 0.
 
     Returns:
         np.ndarray: Chip with overflowing regions filled with ``fill_value``.
     """
     top_overflow = max(0, bbox.ymin - window.ymin)
     bottom_overflow = max(0, window.ymax - bbox.ymax)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/rasterio.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/rasterio.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 def write_bbox(path: str, arr: np.ndarray, bbox: Box, crs_wkt: str, **kwargs):
     """Write a (H, W[, C]) array to a GeoTIFF, georeferenced to the given bbox.
 
     Args:
         path (str): GeoTiff path.
         arr (np.ndarray): (H, W[, C]) Array to write.
-        bbox (Box): Bouding box in map coords to georeference the GeoTiff to.
+        bbox (Box): Bounding box in map coords to georeference the GeoTiff to.
         crs_wkt (str): CRS in WKT format.
     """
     if arr.ndim == 2:
         h_arr, w_arr = arr.shape
         num_channels = 1
     else:
         h_arr, w_arr, num_channels = arr.shape
@@ -178,15 +178,15 @@
             read. Must be 1-indexed.
         window (Optional[Tuple[Tuple[int, int], Tuple[int, int]]]):
             ((row_start, row_stop), (col_start, col_stop)) or
             ((y_min, y_max), (x_min, x_max)). If None, reads the entire raster.
             Defaults to None.
         is_masked (bool): If True, read a masked array from rasterio.
             Defaults to False.
-        out_shape (Optional[Tuple[int, int]]): (hieght, width) of the output
+        out_shape (Optional[Tuple[int, int]]): (height, width) of the output
             chip. If None, no resizing is done. Defaults to None.
 
     Returns:
         np.ndarray: array of shape (height, width, channels).
     """
     if bands is not None:
         bands = tuple(bands)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/utils/vectorization.py` & `rastervision_core-0.30.0/rastervision/core/data/utils/vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def mask_to_polygons(mask: np.ndarray, transform: Optional[rio.Affine] = None
                      ) -> Iterator['BaseGeometry']:
     """Polygonize a raster mask. Wrapper around rasterio.features.shapes.
 
     Args:
         mask (np.ndarray): The mask containing buildings to polygonize.
         transform (Optional[rio.Affine]): Affine transform to use during
-            polygonization. Deafults to None (i.e. identity transform).
+            polygonization. Defaults to None (i.e. identity transform).
 
     Returns:
         Iterator[BaseGeometry]: Generator of shapely polygons.
     """
     if transform is None:
         transform = rio.Affine.identity()
     shapes = rio.features.shapes(mask, mask=(mask == 1), transform=transform)
@@ -57,15 +57,15 @@
 
             1. Apply morphological dilation using the kernel from above.
             2. Polygonize using ``mask_to_polygons()``.
 
     Args:
         mask (np.ndarray): The mask containing buildings to polygonize.
         transform (Optional[rio.Affine]): Affine transform to use during
-            polygonization. Deafults to None (i.e. identity transform).
+            polygonization. Defaults to None (i.e. identity transform).
         min_area (float): Minimum area (in pixels^2) of anything that can be
             considered to be a building or cluster of buildings. The goal is to
             distinguish between buildings and artifacts. Components with area
             less than this value will be discarded. Defaults to 100.
         width_factor (float): Width of the structural element used to break
             building clusters as a fraction of the width of the cluster.
         thickness (float): Thickness of the structural element that is used to
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_source/geojson_vector_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_source/geojson_vector_source_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 if TYPE_CHECKING:
     from rastervision.core.data import (ClassConfig, CRSTransformer)
 
 
 def geojson_vector_source_config_upgrader(cfg_dict: dict,
                                           version: int) -> dict:
     if version == 7:
-        cfg_dict['uris'] = cfg_dict['uri']
-        del cfg_dict['uri']
+        cfg_dict['uris'] = cfg_dict.pop('uri', [])
+    if version == 12:
+        # removed in version 13
+        cfg_dict.pop('ignore_crs_field', None)
     return cfg_dict
 
 
 @register_config(
     'geojson_vector_source', upgrader=geojson_vector_source_config_upgrader)
 class GeoJSONVectorSourceConfig(VectorSourceConfig):
     """Configure a :class:`.GeoJSONVectorSource`."""
 
     uris: Union[str, List[str]] = Field(
         ..., description='URI(s) of GeoJSON file(s).')
-    ignore_crs_field: bool = False
 
     def build(self,
               class_config: 'ClassConfig',
               crs_transformer: 'CRSTransformer',
               use_transformers: bool = True) -> GeoJSONVectorSource:
         if use_transformers:
             transformers = [
                 tf.build(class_config=class_config) for tf in self.transformers
             ]
         else:
             transformers = []
 
         return GeoJSONVectorSource(
             uris=self.uris,
-            ignore_crs_field=self.ignore_crs_field,
             crs_transformer=crs_transformer,
             vector_transformers=transformers)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_source/vector_source.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         """
         geojson = self.get_geojson(window=window, to_map_coords=to_map_coords)
         return list(geojson_to_geoms(geojson))
 
     @abstractmethod
     def _get_geojson(self) -> dict:
         """Return raw GeoJSON."""
-        pass
 
     def get_dataframe(self,
                       window: Optional[Box] = None,
                       to_map_coords: bool = False) -> gpd.GeoDataFrame:
         """Return geometries as a :class:`~geopandas.GeoDataFrame`.
 
         Arguments:
@@ -137,14 +136,18 @@
     @property
     def bbox(self) -> 'Box':
         """Bounding box applied to the source data."""
         if self._bbox is None:
             self._bbox = self.extent
         return self._bbox
 
+    @property
+    def __geo_interface__(self):
+        return self.get_geojson()
+
 
 def sanitize_geojson(geojson: dict,
                      crs_transformer: 'CRSTransformer',
                      to_map_coords: bool = False) -> dict:
     """Apply some basic transformations (listed below) to a GeoJSON.
 
     The following transformations are applied:
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_source/vector_source_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_source/vector_source_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 if TYPE_CHECKING:
     from rastervision.core.rv_pipeline import RVPipelineConfig
     from rastervision.core.data import (ClassConfig, CRSTransformer,
                                         SceneConfig, VectorSource)
 
 
-def vector_source_config_upgrader(cfg_dict: dict, version: int) -> dict:
+def vector_source_config_upgrader(cfg_dict: dict,
+                                  version: int) -> dict:  # pragma: no cover
     if version == 4:
         from rastervision.core.data.vector_transformer import (
             ClassInferenceTransformerConfig, BufferTransformerConfig)
 
         class_inf_tf = ClassInferenceTransformerConfig(
             default_class_id=cfg_dict.get('default_class_id'),
             class_id_to_filter=cfg_dict.get('class_id_to_filter')).dict()
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/__init__.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/buffer_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/buffer_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/buffer_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/class_inference_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/class_inference_transformer_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,26 +10,36 @@
 
 @register_config('class_inference_transformer')
 class ClassInferenceTransformerConfig(VectorTransformerConfig):
     """Configure a :class:`.ClassInferenceTransformer`."""
 
     default_class_id: Optional[int] = Field(
         None,
-        description='The default class_id to use if class cannot be inferred '
-        'using other mechanisms. If a feature has an inferred class_id of '
-        'None, then it will be deleted.')
+        description='The default ``class_id`` to use if class cannot be '
+        'inferred using other mechanisms. If a feature has an inferred '
+        '``class_id`` of ``None``, then it will be deleted. '
+        'Defaults to ``None``.')
     class_id_to_filter: Optional[Dict[int, list]] = Field(
         None,
-        description='Map from class_id to JSON filter used to infer missing '
-        'class_ids. Each key should be a class id, and its value should be a '
-        'boolean expression which is run against the property field for each '
-        'feature. This allows matching different features to different '
-        'class IDs based on its properties. The expression schema is that '
-        'described by '
-        'https://docs.mapbox.com/mapbox-gl-js/style-spec/other/#other-filter')
+        description='Map from ``class_id`` to JSON filter used to infer '
+        'missing class IDs. Each key should be a class ID, and its value '
+        'should be a boolean expression which is run against the property '
+        'field for each feature. This allows matching different features to '
+        'different class IDs based on its properties. The expression schema '
+        'is that described by '
+        'https://docs.mapbox.com/mapbox-gl-js/style-spec/other/#other-filter. '
+        'Defaults to ``None``.')
+    class_name_mapping: dict[str, str] = Field(
+        None,
+        description='``old_name --> new_name`` mapping for values in the '
+        '``class_name`` or ``label`` property of the GeoJSON features. The '
+        '``new_name`` must be a valid class name in the ``ClassConfig``. This '
+        'can also be used to merge multiple classes into one e.g.: '
+        '``dict(car="vehicle", truck="vehicle")``. Defaults to None.')
 
     def build(self, class_config: Optional['ClassConfig'] = None
               ) -> ClassInferenceTransformer:
         return ClassInferenceTransformer(
             self.default_class_id,
             class_config=class_config,
-            class_id_to_filter=self.class_id_to_filter)
+            class_id_to_filter=self.class_id_to_filter,
+            class_name_mapping=self.class_name_mapping)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/label_maker/filter.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/label_maker/filter.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/shift_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/shift_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/shift_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/vector_transformer.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,8 +34,7 @@
 
         Args:
             geojson (dict): A GeoJSON-like mapping of a FeatureCollection.
 
         Returns:
             dict: Transformed GeoJSON.
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/data/vector_transformer/vector_transformer_config.py` & `rastervision_core-0.30.0/rastervision/core/data/vector_transformer/vector_transformer_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/__init__.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/chip_classification_evaluation.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/chip_classification_evaluator_config.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/chip_classification_evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/class_evaluation_item.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/class_evaluation_item.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/classification_evaluation.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
         This is useful for computing the average metrics of a set of scenes.
         The results of the averaging are stored in this Evaluation.
 
         Args:
             other (ClassificationEvaluation): Evaluation to merge into this one
             scene_id (Optional[str], optional): ID of scene. If specified,
-                (a copy of) ``other`` will be saved and be availabel in
+                (a copy of) ``other`` will be saved and be available in
                 ``to_json()``'s output. Defaults to None.
         """
         if self.conf_mat is None:
             self.conf_mat = other.conf_mat
         else:
             self.conf_mat += other.conf_mat
 
@@ -147,8 +147,7 @@
     def compute(self, ground_truth_labels, prediction_labels):
         """Compute metrics for a single scene.
 
         Args:
             ground_truth_labels: Ground Truth labels to evaluate against.
             prediction_labels: The predicted labels to evaluate.
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/classification_evaluator.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/classification_evaluator.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/evaluator.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/evaluator.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,37 +11,34 @@
     @abstractmethod
     def process(self, scenes: Iterable['Scene']) -> None:
         """Evaluate all given scenes and save the evaluations.
 
         Args:
             scenes (Iterable[Scene]): Scenes to evaluate.
         """
-        pass
 
     @abstractmethod
     def evaluate_scene(self, scene: 'Scene') -> Any:
         """Evaluate predictions from a scene's labels store.
 
         The predictions are evalated against ground truth labels from the
         scene's label source.
 
         Args:
             scene (Scene): A scene with a label source and a label store.
 
         Returns:
             ClassificationEvaluation: The evaluation.
         """
-        pass
 
     @abstractmethod
     def evaluate_predictions(self, ground_truth: 'Labels',
                              predictions: 'Labels') -> Any:
         """Evaluate predictions against ground truth.
 
         Args:
             ground_truth (Labels): Ground truth labels.
             predictions (Labels): Predictions.
 
         Returns:
             Any: The evaluation.
         """
-        pass
```

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/evaluator_config.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/object_detection_evaluation.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def compute_metrics(
         gt_labels: 'ObjectDetectionLabels',
         pred_labels: 'ObjectDetectionLabels',
         num_classes: int,
         iou_thresh: float = 0.5) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """Compute per-class true positves, false positives, and false negatives.
+    """Compute per-class true positives, false positives, and false negatives.
 
     Does the following:
 
     1.  Spatially join ground truth (GT) boxes with predicted boxes.
     2.  Compute intersection-overo-union (IoU) for each matched box-pair.
     3.  Filter matches by ``iou_thresh``.
     4.  For each GT box >1 matches, keep only the max-IoU one.
```

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/object_detection_evaluator_config.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/object_detection_evaluator_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluation.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluation.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluator.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py` & `rastervision_core-0.30.0/rastervision/core/evaluation/semantic_segmentation_evaluator_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 from rastervision.core.evaluation.semantic_segmentation_evaluator import (
     SemanticSegmentationEvaluator)
 
 if TYPE_CHECKING:
     from rastervision.core.data import ClassConfig
 
 
-def ss_evaluator_config_upgrader(cfg_dict: dict, version: int) -> dict:
-    if version < 3:
-        try:
-            # removed in version 3
-            del cfg_dict['vector_output_uri']
-        except KeyError:
-            pass
+def ss_evaluator_config_upgrader(cfg_dict: dict,
+                                 version: int) -> dict:  # pragma: no cover
+    if version == 2:
+        # removed in version 3
+        cfg_dict.pop('vector_output_uri', None)
     return cfg_dict
 
 
 @register_config(
     'semantic_segmentation_evaluator', upgrader=ss_evaluator_config_upgrader)
 class SemanticSegmentationEvaluatorConfig(ClassificationEvaluatorConfig):
     """Configure a :class:`.SemanticSegmentationEvaluator`."""
```

### Comparing `rastervision_core-0.21.3/rastervision/core/raster_stats.py` & `rastervision_core-0.30.0/rastervision/core/raster_stats.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/__init__.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # flake8: noqa
 
 TRAIN = 'train'
 VALIDATION = 'validation'
 
+from rastervision.core.rv_pipeline.chip_options import *
 from rastervision.core.rv_pipeline.rv_pipeline import *
 from rastervision.core.rv_pipeline.rv_pipeline_config import *
 from rastervision.core.rv_pipeline.chip_classification import *
 from rastervision.core.rv_pipeline.chip_classification_config import *
 from rastervision.core.rv_pipeline.semantic_segmentation import *
 from rastervision.core.rv_pipeline.semantic_segmentation_config import *
 from rastervision.core.rv_pipeline.object_detection import *
@@ -18,14 +19,17 @@
     RVPipelineConfig.__name__,
     ChipClassification.__name__,
     ChipClassificationConfig.__name__,
     SemanticSegmentation.__name__,
     SemanticSegmentationConfig.__name__,
     SemanticSegmentationChipOptions.__name__,
     SemanticSegmentationPredictOptions.__name__,
-    SemanticSegmentationWindowMethod.__name__,
     ObjectDetection.__name__,
     ObjectDetectionConfig.__name__,
-    ObjectDetectionChipOptions.__name__,
+    ObjectDetectionWindowSamplingConfig.__name__,
     ObjectDetectionChipOptions.__name__,
     ObjectDetectionPredictOptions.__name__,
+    ChipOptions.__name__,
+    WindowSamplingConfig.__name__,
+    WindowSamplingMethod.__name__,
+    PredictOptions.__name__,
 ]
```

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/chip_classification_config.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/chip_classification_config.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/object_detection_config.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/object_detection_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-from enum import Enum
 from typing import Optional
 
-from rastervision.pipeline.config import register_config, Config, Field
-from rastervision.core.rv_pipeline import RVPipelineConfig, PredictOptions
+from rastervision.pipeline.config import Field, register_config, validator
+from rastervision.core.rv_pipeline import (
+    ChipOptions, RVPipelineConfig, PredictOptions, WindowSamplingConfig)
 from rastervision.core.data.label_store import ObjectDetectionGeoJSONStoreConfig
 from rastervision.core.evaluation import ObjectDetectionEvaluatorConfig
 
 
-class ObjectDetectionWindowMethod(Enum):
-    """Enum for window methods
-
-    Attributes:
-        chip: the default method
-    """
-    chip = 'chip'
-    label = 'label'
-    image = 'image'
-    sliding = 'sliding'
+@register_config('object_detection_window_sampling')
+class ObjectDetectionWindowSamplingConfig(WindowSamplingConfig):
+    ioa_thresh: float = Field(
+        0.8,
+        description='When a box is partially outside of a training chip, it '
+        'is not clear if (a clipped version) of the box should be included in '
+        'the chip. If the IOA (intersection over area) of the box with the '
+        'chip is greater than ioa_thresh, it is included in the chip. '
+        'Defaults to 0.8.')
+    clip: bool = Field(
+        False,
+        description='Clip bounding boxes to window limits when retrieving '
+        'labels for a window.')
+    neg_ratio: Optional[float] = Field(
+        None,
+        description='The ratio of negative chips (those containing no '
+        'bounding boxes) to positive chips. This can be useful if the '
+        'statistics of the background is different in positive chips. For '
+        'example, in car detection, the positive chips will always contain '
+        'roads, but no examples of rooftops since cars tend to not be near '
+        'rooftops. Defaults to None.')
+    neg_ioa_thresh: float = Field(
+        0.2,
+        description='A window will be considered negative if its max IoA with '
+        'any bounding box is less than this threshold. Defaults to 0.2.')
 
 
 @register_config('object_detection_chip_options')
-class ObjectDetectionChipOptions(Config):
-    neg_ratio: float = Field(
-        1.0,
-        description=
-        ('The ratio of negative chips (those containing no bounding '
-         'boxes) to positive chips. This can be useful if the statistics '
-         'of the background is different in positive chips. For example, '
-         'in car detection, the positive chips will always contain roads, '
-         'but no examples of rooftops since cars tend to not be near rooftops.'
-         ))
-    ioa_thresh: float = Field(
-        0.8,
-        description=
-        ('When a box is partially outside of a training chip, it is not clear if (a '
-         'clipped version) of the box should be included in the chip. If the IOA '
-         '(intersection over area) of the box with the chip is greater than ioa_thresh, '
-         'it is included in the chip.'))
-    window_method: ObjectDetectionWindowMethod = ObjectDetectionWindowMethod.chip
-    label_buffer: Optional[int] = None
+class ObjectDetectionChipOptions(ChipOptions):
+    sampling: ObjectDetectionWindowSamplingConfig = Field(
+        ..., description='Window sampling config.')
 
 
 @register_config('object_detection_predict_options')
 class ObjectDetectionPredictOptions(PredictOptions):
+    stride: Optional[int] = Field(
+        None,
+        description='Stride of the sliding window for generating chips. '
+        'Defaults to half of ``chip_sz``.')
     merge_thresh: float = Field(
         0.5,
         description=
         ('If predicted boxes have an IOA (intersection over area) greater than '
          'merge_thresh, then they are merged into a single box during postprocessing. '
          'This is needed since the sliding window approach results in some false '
          'duplicates.'))
     score_thresh: float = Field(
         0.5,
         description=
         ('Predicted boxes are only output if their score is above score_thresh.'
          ))
 
+    @validator('stride', always=True)
+    def validate_stride(cls, v: Optional[int], values: dict) -> dict:
+        if v is None:
+            chip_sz: int = values['chip_sz']
+            return chip_sz // 2
+        return v
+
 
 @register_config('object_detection')
 class ObjectDetectionConfig(RVPipelineConfig):
     """Configure an :class:`.ObjectDetection` pipeline."""
 
-    chip_options: ObjectDetectionChipOptions = ObjectDetectionChipOptions()
-    predict_options: ObjectDetectionPredictOptions = ObjectDetectionPredictOptions(
-    )
+    chip_options: Optional[ObjectDetectionChipOptions]
+    predict_options: Optional[ObjectDetectionPredictOptions]
 
     def build(self, tmp_dir):
         from rastervision.core.rv_pipeline.object_detection import ObjectDetection
         return ObjectDetection(self, tmp_dir)
 
     def get_default_label_store(self, scene):
         return ObjectDetectionGeoJSONStoreConfig()
```

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/rv_pipeline.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/rv_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import tempfile
 import shutil
 from typing import TYPE_CHECKING, Optional, List
 from functools import lru_cache
 
 import click
 import numpy as np
-from tqdm.auto import tqdm
 
 from rastervision.pipeline.pipeline import Pipeline
 from rastervision.core.box import Box
 from rastervision.core.data_sample import DataSample
 from rastervision.core.data import Scene, Labels
 from rastervision.core.backend import Backend
-from rastervision.core.rv_pipeline import TRAIN, VALIDATION
 from rastervision.pipeline.file_system.utils import (
     download_if_needed, zipdir, get_local_path, upload_or_copy, make_dir,
     sync_from_dir, file_exists)
 
 log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
@@ -113,47 +111,20 @@
             Labels that lie within window
         """
         raise NotImplementedError()
 
     def chip(self, split_ind: int = 0, num_splits: int = 1):
         """Save training and validation chips."""
         cfg = self.config
-        backend = cfg.backend.build(cfg, self.tmp_dir)
+        log.info(f'Chip options: {cfg.chip_options}')
         dataset = cfg.dataset.get_split_config(split_ind, num_splits)
         if not dataset.train_scenes and not dataset.validation_scenes:
             return
-
-        class_cfg = dataset.class_config
-        with backend.get_sample_writer() as writer:
-
-            def chip_scene(scene, split):
-                windows = self.get_train_windows(scene)
-                if len(windows) == 0:
-                    log.warning(f'Scene {scene.id} produced no windows')
-                    return
-                with tqdm(
-                        windows,
-                        desc=f'Making {split} chips from scene {scene.id}',
-                        mininterval=0.5) as bar:
-                    for window in bar:
-                        chip = scene.raster_source.get_chip(window)
-                        labels = self.get_train_labels(window, scene)
-                        sample = DataSample(
-                            chip=chip,
-                            window=window,
-                            labels=labels,
-                            scene_id=str(scene.id),
-                            is_train=split == TRAIN)
-                        sample = self.post_process_sample(sample)
-                        writer.write_sample(sample)
-
-            for s in dataset.train_scenes:
-                chip_scene(s.build(class_cfg, self.tmp_dir), TRAIN)
-            for s in dataset.validation_scenes:
-                chip_scene(s.build(class_cfg, self.tmp_dir), VALIDATION)
+        backend = cfg.backend.build(cfg, self.tmp_dir)
+        backend.chip_dataset(dataset, cfg.chip_options)
 
     def train(self):
         """Train a model and save it."""
         backend = self.config.backend.build(self.config, self.tmp_dir)
         backend.train(source_bundle_uri=self.config.source_bundle_uri)
 
     def post_process_sample(self, sample: DataSample) -> DataSample:
@@ -173,33 +144,32 @@
         return labels
 
     def predict(self, split_ind=0, num_splits=1):
         """Make predictions over each validation and test scene.
 
         This uses a sliding window.
         """
-        # Cache backend so subsquent calls will be faster. This is useful for
-        # the predictor.
         if self.backend is None:
-            self.backend = self.config.backend.build(self.config, self.tmp_dir)
-            self.backend.load_model()
+            self.build_backend()
 
         class_config = self.config.dataset.class_config
         dataset = self.config.dataset.get_split_config(split_ind, num_splits)
 
         for scene_config in (dataset.validation_scenes + dataset.test_scenes):
             scene = scene_config.build(class_config, self.tmp_dir)
-            labels = self.predict_scene(scene, self.backend)
-            labels = self.post_process_predictions(labels, scene)
+            labels = self.predict_scene(scene)
             scene.label_store.save(labels)
 
-    def predict_scene(self, scene: Scene, backend: Backend) -> Labels:
-        chip_sz = self.config.predict_chip_sz
-        stride = chip_sz
-        return backend.predict_scene(scene, chip_sz=chip_sz, stride=stride)
+    def predict_scene(self, scene: Scene) -> Labels:
+        if self.backend is None:
+            self.build_backend()
+        labels = self.backend.predict_scene(
+            scene, predict_options=self.config.predict_options)
+        labels = self.post_process_predictions(labels, scene)
+        return labels
 
     def eval(self):
         """Evaluate predictions against ground truth."""
         dataset = self.config.dataset
         class_config = dataset.class_config
         # it might make sense to make excluded_groups a field in an EvalConfig
         # in the future
@@ -258,7 +228,11 @@
             path = download_if_needed(self.config.get_config_uri(), tmp_dir)
             shutil.copy(path, join(bundle_dir, 'pipeline-config.json'))
 
             model_bundle_uri = self.config.get_model_bundle_uri()
             model_bundle_path = get_local_path(model_bundle_uri, self.tmp_dir)
             zipdir(bundle_dir, model_bundle_path)
             upload_or_copy(model_bundle_path, model_bundle_uri)
+
+    def build_backend(self, uri: Optional[str] = None) -> None:
+        self.backend = self.config.backend.build(self.config, self.tmp_dir)
+        self.backend.load_model(uri)
```

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/rv_pipeline_config.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/semantic_segmentation_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,139 +1,146 @@
-from os.path import join
-from typing import List, TYPE_CHECKING, Optional
-
-from rastervision.pipeline.pipeline_config import PipelineConfig
-from rastervision.core.data import (DatasetConfig, StatsTransformerConfig,
-                                    LabelStoreConfig, SceneConfig)
-from rastervision.core.utils.misc import Proportion
-from rastervision.core.analyzer import StatsAnalyzerConfig
-from rastervision.core.backend import BackendConfig
-from rastervision.core.evaluation import EvaluatorConfig
-from rastervision.core.analyzer import AnalyzerConfig
-from rastervision.pipeline.config import (register_config, Field, Config)
-
-if TYPE_CHECKING:
-    from rastervision.core.backend.backend import Backend  # noqa
-
-
-@register_config('predict_options')
-class PredictOptions(Config):
-    # TODO: predict_chip_sz and predict_batch_sz should probably be moved here
-    pass
-
-
-@register_config('rv_pipeline')
-class RVPipelineConfig(PipelineConfig):
-    """Configure an :class:`.RVPipeline`."""
-
-    dataset: DatasetConfig = Field(
-        ...,
+from typing import (List, Literal, Optional, Union)
+from pydantic import conint
+import logging
+
+import numpy as np
+
+from rastervision.pipeline.config import (register_config, Field, validator)
+from rastervision.core.rv_pipeline.rv_pipeline_config import (PredictOptions,
+                                                              RVPipelineConfig)
+from rastervision.core.rv_pipeline.chip_options import (ChipOptions,
+                                                        WindowSamplingConfig)
+from rastervision.core.data import SemanticSegmentationLabelStoreConfig
+from rastervision.core.evaluation import SemanticSegmentationEvaluatorConfig
+
+log = logging.getLogger(__name__)
+
+
+def ss_chip_options_upgrader(cfg_dict: dict, version: int) -> dict:
+    if version == 10:
+        sampling = WindowSamplingConfig(
+            method=cfg_dict.pop('window_method', None),
+            size=300,
+            stride=cfg_dict.pop('stride', None),
+            max_windows=cfg_dict.pop('chips_per_scene', None),
+        )
+        cfg_dict['sampling'] = sampling.dict()
+    return cfg_dict
+
+
+@register_config(
+    'semantic_segmentation_chip_options', upgrader=ss_chip_options_upgrader)
+class SemanticSegmentationChipOptions(ChipOptions):
+    """Chipping options for semantic segmentation."""
+    target_class_ids: Optional[List[int]] = Field(
+        None,
         description=
-        'Dataset containing train, validation, and optional test scenes.')
-    backend: BackendConfig = Field(
-        ..., description='Backend to use for interfacing with ML library.')
-    evaluators: List[EvaluatorConfig] = Field(
-        [],
-        description=(
-            'Evaluators to run during analyzer command. If list is empty '
-            'the default evaluator is added.'))
-    analyzers: List[AnalyzerConfig] = Field(
-        [],
+        ('List of class ids considered as targets (ie. those to prioritize when '
+         'creating chips) which is only used in conjunction with the '
+         'target_count_threshold and negative_survival_probability options. Applies '
+         'to the random_sample window method.'))
+    negative_survival_prob: float = Field(
+        1.0, description='Probability of keeping a negative chip.')
+    target_count_threshold: int = Field(
+        1000,
         description=
-        ('Analyzers to run during analyzer command. A StatsAnalyzer will be added '
-         'automatically if any scenes have a RasterTransformer.'))
-
-    train_chip_sz: int = Field(
-        300, description='Size of training chips in pixels.')
-    predict_chip_sz: int = Field(
-        300, description='Size of predictions chips in pixels.')
-    predict_batch_sz: int = Field(
-        8, description='Batch size to use during prediction.')
-    chip_nodata_threshold: Proportion = Field(
-        1,
-        description='Discard chips where the proportion of NODATA values is '
-        'greater than or equal to this value. Might result in false positives '
-        'if there are many legitimate black pixels in the chip. Use with '
-        'caution.')
+        ('Minimum number of pixels covering target_classes that a chip must have. '
+         'Applies to the random_sample window method.'))
 
-    analyze_uri: Optional[str] = Field(
+    def keep_chip(self, chip: np.ndarray, label: np.ndarray) -> bool:
+        keep = super().keep_chip(chip, label)
+        if not keep:
+            return False
+        if self.target_class_ids is not None:
+            if self.enough_target_pixels(label):
+                return True
+            if np.random.sample() <= self.negative_survival_prob:
+                return True
+            return False
+        return keep
+
+    def enough_target_pixels(self, label_arr: np.ndarray) -> bool:
+        """Check if label raster has enough pixels of the target classes.
+
+        Args:
+             label_arr: The label raster for a chip.
+
+        Returns:
+             True (the window does contain interesting pixels) or False.
+        """
+        target_count = 0
+        for class_id in self.target_class_ids:
+            target_count += (label_arr == class_id).sum()
+        enough_target_pixels = target_count >= self.target_count_threshold
+        return enough_target_pixels
+
+
+@register_config('semantic_segmentation_predict_options')
+class SemanticSegmentationPredictOptions(PredictOptions):
+    stride: Optional[int] = Field(
+        None,
+        description='Stride of the sliding window for generating chips. '
+        'Allows aggregating multiple predictions for each pixel if less than '
+        'the chip size. Defaults to ``chip_sz``.')
+    crop_sz: Optional[Union[conint(gt=0), Literal['auto']]] = Field(
         None,
         description=
-        'URI for output of analyze. If None, will be auto-generated.')
-    chip_uri: Optional[str] = Field(
-        None,
-        description='URI for output of chip. If None, will be auto-generated.')
-    train_uri: Optional[str] = Field(
-        None,
-        description='URI for output of train. If None, will be auto-generated.'
-    )
-    predict_uri: Optional[str] = Field(
-        None,
-        description=
-        'URI for output of predict. If None, will be auto-generated.')
-    eval_uri: Optional[str] = Field(
-        None,
-        description='URI for output of eval. If None, will be auto-generated.')
-    bundle_uri: Optional[str] = Field(
-        None,
-        description='URI for output of bundle. If None, will be auto-generated.'
-    )
-    source_bundle_uri: Optional[str] = Field(
-        None,
-        description='If provided, the model will be loaded from this bundle '
-        'for the train stage. Useful for fine-tuning.')
+        'Number of rows/columns of pixels from the edge of prediction '
+        'windows to discard. This is useful because predictions near edges '
+        'tend to be lower quality and can result in very visible artifacts '
+        'near the edges of chips. If "auto", will be set to half the stride '
+        'if stride is less than chip_sz. Defaults to None.')
+
+    @validator('crop_sz')
+    def validate_crop_sz(cls,
+                         v: Optional[Union[conint(gt=0), Literal['auto']]],
+                         values: dict) -> dict:
+        crop_sz = v
+        if crop_sz == 'auto':
+            chip_sz: int = values['chip_sz']
+            stride: int = values['stride']
+            overlap_sz = chip_sz - stride
+            if overlap_sz % 2 == 1:
+                log.warning(
+                    'Using crop_sz="auto" but overlap size (chip_sz minus '
+                    'stride) is odd. This means that one pixel row/col will '
+                    'still overlap after cropping.')
+            crop_sz = overlap_sz // 2
+        return crop_sz
+
+
+def ss_config_upgrader(cfg_dict: dict, version: int) -> dict:
+    if version == 0:
+        try:
+            # removed in version 1
+            del cfg_dict['channel_display_groups']
+            del cfg_dict['img_format']
+            del cfg_dict['label_format']
+        except KeyError:
+            pass
+    return cfg_dict
+
+
+@register_config('semantic_segmentation', upgrader=ss_config_upgrader)
+class SemanticSegmentationConfig(RVPipelineConfig):
+    """Configure a :class:`.SemanticSegmentation` pipeline."""
+
+    chip_options: Optional[SemanticSegmentationChipOptions]
+    predict_options: Optional[SemanticSegmentationPredictOptions]
+
+    def build(self, tmp_dir):
+        from rastervision.core.rv_pipeline.semantic_segmentation import (
+            SemanticSegmentation)
+        return SemanticSegmentation(self, tmp_dir)
 
     def update(self):
+        self.dataset.class_config.ensure_null_class()
         super().update()
 
-        if self.analyze_uri is None:
-            self.analyze_uri = join(self.root_uri, 'analyze')
-        if self.chip_uri is None:
-            self.chip_uri = join(self.root_uri, 'chip')
-        if self.train_uri is None:
-            self.train_uri = join(self.root_uri, 'train')
-        if self.predict_uri is None:
-            self.predict_uri = join(self.root_uri, 'predict')
-        if self.eval_uri is None:
-            self.eval_uri = join(self.root_uri, 'eval')
-        if self.bundle_uri is None:
-            self.bundle_uri = join(self.root_uri, 'bundle')
-
-        self.dataset.update(pipeline=self)
-        self.backend.update(pipeline=self)
-        if not self.evaluators:
-            self.evaluators.append(self.get_default_evaluator())
-        for evaluator in self.evaluators:
-            evaluator.update(pipeline=self)
-
-        self._insert_analyzers()
-        for analyzer in self.analyzers:
-            analyzer.update(pipeline=self)
-
-    def get_model_bundle_uri(self):
-        return join(self.bundle_uri, 'model-bundle.zip')
-
-    def _insert_analyzers(self):
-        # Inserts StatsAnalyzer if it's needed because a RasterSource has a
-        # StatsTransformer, but there isn't a StatsAnalyzer in the list of Analyzers.
-        has_stats_transformer = False
-        for s in self.dataset.all_scenes:
-            for t in s.raster_source.transformers:
-                if isinstance(t, StatsTransformerConfig):
-                    has_stats_transformer = True
-
-        has_stats_analyzer = False
-        for a in self.analyzers:
-            if isinstance(a, StatsAnalyzerConfig):
-                has_stats_analyzer = True
-                break
-
-        if has_stats_transformer and not has_stats_analyzer:
-            self.analyzers.append(StatsAnalyzerConfig())
-
-    def get_default_label_store(self, scene: SceneConfig) -> LabelStoreConfig:
-        """Returns a default LabelStoreConfig to fill in any missing ones."""
-        raise NotImplementedError()
-
-    def get_default_evaluator(self) -> EvaluatorConfig:
-        """Returns a default EvaluatorConfig to use if one isn't set."""
-        raise NotImplementedError()
+    def validate_config(self):
+        super().validate_config()
+
+    def get_default_label_store(self, scene):
+        return SemanticSegmentationLabelStoreConfig()
+
+    def get_default_evaluator(self):
+        return SemanticSegmentationEvaluatorConfig()
```

### Comparing `rastervision_core-0.21.3/rastervision/core/rv_pipeline/utils.py` & `rastervision_core-0.30.0/rastervision/core/rv_pipeline/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 
 
 def nodata_below_threshold(chip: np.ndarray,
                            threshold: float,
                            nodata_val: int = 0) -> bool:
-    """Check if proportion of nodata pixels is below the threshold.
+    """Check if fraction of nodata pixels is below the threshold.
 
     Args:
-        chip (np.ndarray): Raster as (H, W) or (H, W, C) numpy array.
+        chip (np.ndarray): Raster as (..., H, W[, C]) numpy array.
         threshold (float): Threshold to check the fraction of NODATA pixels
             against.
         nodata_val (int, optional): Value that represents NODATA pixels.
             Defaults to 0.
 
     Returns:
         bool: Whether the fraction of NODATA pixels is below the given
         threshold.
     """
-    if chip.ndim == 3:
-        # (H, W, C) --> (H, W)
+    if chip.ndim > 2:
+        # (..., w, h, c) --> (..., w, h)
         chip = chip.sum(axis=-1)
-    nodata_prop = (chip == nodata_val).mean()
-    return nodata_prop < threshold
+    nodata_frac = (chip == nodata_val).mean()
+    return nodata_frac < threshold
```

### Comparing `rastervision_core-0.21.3/rastervision/core/utils/cog.py` & `rastervision_core-0.30.0/rastervision/core/utils/cog.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/utils/filter_geojson.py` & `rastervision_core-0.30.0/rastervision/core/utils/filter_geojson.py`

 * *Files identical despite different names*

### Comparing `rastervision_core-0.21.3/rastervision/core/utils/stac.py` & `rastervision_core-0.30.0/rastervision/core/utils/stac.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     Note: This has been tested to be compatible with STAC version 1.0.0 but
     not any other versions.
 
     Args:
         stac_uri (str): Path to the STAC catalog JSON file.
 
     Returns:
-        List[dict]: A lsit of dicts with keys: "label_uri", "image_uris",
+        List[dict]: A list of dicts with keys: "label_uri", "image_uris",
         "label_bbox", "image_bbox", "bboxes_intersect", and "aoi_geometry".
         Each dict corresponds to one label item and its associated image
         assets in the STAC catalog.
     """
     setup_stac_io()
     cat = Catalog.from_file(stac_uri)
     version: str = cat.to_dict()['stac_version']
@@ -141,15 +141,15 @@
         **kwargs: Extra args for :func:`.parse_stac`.
 
     Raises:
         FileNotFoundError: If catalog.json is not found inside the zip file.
         Exception: If multiple catalog.json's are found inside the zip file.
 
     Returns:
-        List[dict]: A lsit of dicts with keys: "label_uri", "image_uris",
+        List[dict]: A list of dicts with keys: "label_uri", "image_uris",
         "label_bbox", "image_bbox", "bboxes_intersect", and "aoi_geometry".
         Each dict corresponds to one label item and its associated image
         assets in the STAC catalog.
     """
     from pathlib import Path
     from rastervision.pipeline.file_system.utils import (download_if_needed,
                                                          is_archive, extract)
```

### Comparing `rastervision_core-0.21.3/rastervision_core.egg-info/PKG-INFO` & `rastervision_core-0.30.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rastervision-core
-Version: 0.21.3
+Name: rastervision_core
+Version: 0.30.0
 Summary: A rastervision plugin that adds geospatial machine learning pipelines
 Home-page: https://github.com/azavea/raster-vision
 Author: Azavea
 Author-email: info@azavea.com
 License: Apache License 2.0
 Keywords: raster deep-learning ml computer-vision earth-observation geospatial geospatial-processing
 Classifier: Intended Audience :: Developers
```

### Comparing `rastervision_core-0.21.3/rastervision_core.egg-info/SOURCES.txt` & `rastervision_core-0.30.0/rastervision_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,18 @@
 rastervision/core/data/raster_source/multi_raster_source_config.py
 rastervision/core/data/raster_source/raster_source.py
 rastervision/core/data/raster_source/raster_source_config.py
 rastervision/core/data/raster_source/rasterio_source.py
 rastervision/core/data/raster_source/rasterio_source_config.py
 rastervision/core/data/raster_source/rasterized_source.py
 rastervision/core/data/raster_source/rasterized_source_config.py
+rastervision/core/data/raster_source/stac_config.py
 rastervision/core/data/raster_source/temporal_multi_raster_source.py
 rastervision/core/data/raster_source/xarray_source.py
+rastervision/core/data/raster_source/xarray_source_config.py
 rastervision/core/data/raster_transformer/__init__.py
 rastervision/core/data/raster_transformer/cast_transformer.py
 rastervision/core/data/raster_transformer/cast_transformer_config.py
 rastervision/core/data/raster_transformer/min_max_transformer.py
 rastervision/core/data/raster_transformer/min_max_transformer_config.py
 rastervision/core/data/raster_transformer/nan_transformer.py
 rastervision/core/data/raster_transformer/nan_transformer_config.py
@@ -76,14 +78,15 @@
 rastervision/core/data/raster_transformer/reclass_transformer.py
 rastervision/core/data/raster_transformer/reclass_transformer_config.py
 rastervision/core/data/raster_transformer/rgb_class_transformer.py
 rastervision/core/data/raster_transformer/rgb_class_transformer_config.py
 rastervision/core/data/raster_transformer/stats_transformer.py
 rastervision/core/data/raster_transformer/stats_transformer_config.py
 rastervision/core/data/utils/__init__.py
+rastervision/core/data/utils/aoi_sampler.py
 rastervision/core/data/utils/factory.py
 rastervision/core/data/utils/geojson.py
 rastervision/core/data/utils/misc.py
 rastervision/core/data/utils/raster.py
 rastervision/core/data/utils/rasterio.py
 rastervision/core/data/utils/vectorization.py
 rastervision/core/data/vector_source/__init__.py
@@ -118,14 +121,15 @@
 rastervision/core/evaluation/object_detection_evaluator_config.py
 rastervision/core/evaluation/semantic_segmentation_evaluation.py
 rastervision/core/evaluation/semantic_segmentation_evaluator.py
 rastervision/core/evaluation/semantic_segmentation_evaluator_config.py
 rastervision/core/rv_pipeline/__init__.py
 rastervision/core/rv_pipeline/chip_classification.py
 rastervision/core/rv_pipeline/chip_classification_config.py
+rastervision/core/rv_pipeline/chip_options.py
 rastervision/core/rv_pipeline/object_detection.py
 rastervision/core/rv_pipeline/object_detection_config.py
 rastervision/core/rv_pipeline/rv_pipeline.py
 rastervision/core/rv_pipeline/rv_pipeline_config.py
 rastervision/core/rv_pipeline/semantic_segmentation.py
 rastervision/core/rv_pipeline/semantic_segmentation_config.py
 rastervision/core/rv_pipeline/utils.py
```

