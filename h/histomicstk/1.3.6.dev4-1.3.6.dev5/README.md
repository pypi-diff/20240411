# Comparing `tmp/histomicstk-1.3.6.dev4.tar.gz` & `tmp/histomicstk-1.3.6.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histomicstk-1.3.6.dev4.tar", last modified: Thu Apr  4 16:11:56 2024, max compression
+gzip compressed data, was "histomicstk-1.3.6.dev5.tar", last modified: Tue Apr  9 15:55:45 2024, max compression
```

## Comparing `histomicstk-1.3.6.dev4.tar` & `histomicstk-1.3.6.dev5.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     9710 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.734270 histomicstk-1.3.6.dev4/histomicstk/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.734270 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotation_and_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotation_database_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    37211 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotations_to_masks_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/masks_to_annotations_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/polygon_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/polygon_merger_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.738271 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/rect.py
--rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/rtree.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/review_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.738271 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_polygon_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_review_gallery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.738271 histomicstk-1.3.6.dev4/histomicstk/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.738271 histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.738271 histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/NucleiClassification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/NucleiClassification.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/
--rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/NucleiDetection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/NucleiDetection.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/PositivePixelCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.742271 histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/dask_config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/docker-entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/slicer_cli_list.json
--rw-r--r--   0 runner    (1001) docker     (127)    16959 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/features/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_fsd_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_global_cell_graph_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_gradient_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_haralick_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_intensity_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_morphometry_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/compute_nuclei_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/features/graycomatrixext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/filters/edge/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/edge/gaussian_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/filters/shape/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/shape/cdog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/shape/clog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/shape/glog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/filters/shape/vesselness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.746271 histomicstk-1.3.6.dev4/histomicstk/preprocessing/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/augmentation/color_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.750270 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/lab_mean_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/lab_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/od_to_rgb.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_lab.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_sda.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/sda_to_rgb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.750270 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/_linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/color_convolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/find_stain_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/stain_color_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.750270 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/background_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/reinhard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/reinhard_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.750270 histomicstk-1.3.6.dev4/histomicstk/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.754270 histomicstk-1.3.6.dev4/histomicstk/saliency/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/saliency/cellularity_detection_superpixels.py
--rw-r--r--   0 runner    (1001) docker     (127)    26865 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/saliency/cellularity_detection_thresholding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.754270 histomicstk-1.3.6.dev4/histomicstk/saliency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/saliency/tests/test_saliency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/saliency/tissue_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.754270 histomicstk-1.3.6.dev4/histomicstk/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/embed_boundaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.758270 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/area_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/compact.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/condense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete_border.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/dilate_xor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/perimeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/remove_overlap_nuclei.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/split.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/trace_object_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/label/width_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.758270 histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/chan_vese.py
--rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/reg_edge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.758270 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/detect_tile_nuclei.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/gaussian_voting.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/gvf_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/max_clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/min_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/positive_pixel_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/rag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/rag_add_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/segmentation/rag_color.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/histomicstk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/compute_tile_foreground_fraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/convert_image_to_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/convert_matrix_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/del2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/eigen.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/exclude_nonfinite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/fit_poisson_mixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/general_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/girder_convenience_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/gradient_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/merge_colinear.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/sample_pixels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/simple_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/histomicstk/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/utils/tests/test_girder_convenience_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/histomicstk/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/workflows/specific_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/histomicstk/workflows/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/workflows/tests/test_workflow_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/histomicstk/workflows/workflow_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/histomicstk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-04 16:11:56.000000 histomicstk-1.3.6.dev4/histomicstk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:11:56.762270 histomicstk-1.3.6.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-04 16:11:49.000000 histomicstk-1.3.6.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8046 2024-04-09 15:55:37.000000 histomicstk-1.3.6.dev5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.506588 histomicstk-1.3.6.dev5/histomicstk/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.506588 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotation_and_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotation_database_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37211 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotations_to_masks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28174 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24653 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/masks_to_annotations_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/polygon_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/polygon_merger_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.510588 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15078 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/rtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/review_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.510588 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_polygon_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_review_gallery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.510588 histomicstk-1.3.6.dev5/histomicstk/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.510588 histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.510588 histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12746 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/NucleiClassification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/NucleiClassification.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/
+-rw-r--r--   0 runner    (1001) docker     (127)    12276 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/NucleiDetection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11008 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/NucleiDetection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/PositivePixelCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6373 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.514587 histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/dask_config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      423 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/docker-entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/slicer_cli_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16959 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7331 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_fsd_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_global_cell_graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_gradient_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13389 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_haralick_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_intensity_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_morphometry_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/compute_nuclei_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/features/graycomatrixext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/filters/edge/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/edge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/edge/gaussian_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/filters/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/shape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/shape/cdog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/shape/clog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/shape/glog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/filters/shape/vesselness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.518587 histomicstk-1.3.6.dev5/histomicstk/preprocessing/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/augmentation/color_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.522588 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/lab_mean_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/lab_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/od_to_rgb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_sda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/sda_to_rgb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.522588 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/_linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/color_convolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/find_stain_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/stain_color_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.522588 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/background_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/reinhard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/reinhard_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.522588 histomicstk-1.3.6.dev5/histomicstk/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.526588 histomicstk-1.3.6.dev5/histomicstk/saliency/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23723 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/saliency/cellularity_detection_superpixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26865 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/saliency/cellularity_detection_thresholding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.526588 histomicstk-1.3.6.dev5/histomicstk/saliency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/saliency/tests/test_saliency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/saliency/tissue_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.526588 histomicstk-1.3.6.dev5/histomicstk/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/embed_boundaries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.530588 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/area_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/compact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/condense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete_border.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/dilate_xor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/perimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/remove_overlap_nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/trace_object_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/label/width_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.530588 histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/chan_vese.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5610 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/reg_edge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.530588 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/detect_tile_nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/gaussian_voting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/gvf_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/max_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/min_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/positive_pixel_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/rag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/rag_add_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/segmentation/rag_color.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/histomicstk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/compute_tile_foreground_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/convert_image_to_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/convert_matrix_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/del2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/eigen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/exclude_nonfinite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/fit_poisson_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/girder_convenience_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/gradient_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/merge_colinear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/sample_pixels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/simple_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/histomicstk/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/utils/tests/test_girder_convenience_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/histomicstk/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/workflows/specific_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/histomicstk/workflows/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/workflows/tests/test_workflow_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/histomicstk/workflows/workflow_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/histomicstk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-09 15:55:45.000000 histomicstk-1.3.6.dev5/histomicstk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:55:45.534587 histomicstk-1.3.6.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-09 15:55:38.000000 histomicstk-1.3.6.dev5/setup.py
```

### Comparing `histomicstk-1.3.6.dev4/CONTRIBUTING.rst` & `histomicstk-1.3.6.dev5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/LICENSE` & `histomicstk-1.3.6.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/NOTICE` & `histomicstk-1.3.6.dev5/NOTICE`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/PKG-INFO` & `histomicstk-1.3.6.dev5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histomicstk
-Version: 1.3.6.dev4
+Version: 1.3.6.dev5
 Summary: A Python toolkit for Histopathology Image Analysis
 Home-page: https://github.com/DigitalSlideArchive/HistomicsTK
 Author: Kitware, Inc.
 Author-email: developers@digitalslidearchive.net
 License: Apache Software License 2.0
 Keywords: histomicstk
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,14 +35,15 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: matplotlib
 Requires-Dist: pyvips
 Requires-Dist: dask[dataframe]
 Requires-Dist: distributed
 Requires-Dist: large-image[sources]; sys_platform == "linux" or sys_platform == "linux2"
 Requires-Dist: large-image[common]; sys_platform != "linux" and sys_platform != "linux2"
+Requires-Dist: large-image-converter; sys_platform == "linux" or sys_platform == "linux2"
 Requires-Dist: girder-slicer-cli-web
 Requires-Dist: ctk-cli
 Requires-Dist: opencv-python-headless
 
 ========================
 HistomicsTK |codecov-io|
 ========================
```

### Comparing `histomicstk-1.3.6.dev4/README.rst` & `histomicstk-1.3.6.dev5/README.rst`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotation_and_mask_utils.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotation_and_mask_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotation_database_parser.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotation_database_parser.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotations_to_masks_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotations_to_masks_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/annotations_to_object_mask_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/masks_to_annotations_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/masks_to_annotations_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/polygon_merger.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/polygon_merger.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/polygon_merger_v2.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/polygon_merger_v2.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/rect.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/rect.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/pyrtree/rtree.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/pyrtree/rtree.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/review_gallery.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/review_gallery.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotation_and_mask_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotation_database_parser.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotations_to_masks_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_annotations_to_object_mask_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_masks_to_annotations_handler.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_polygon_merger.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_polygon_merger.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/annotations_and_masks/tests/test_review_gallery.py` & `histomicstk-1.3.6.dev5/histomicstk/annotations_and_masks/tests/test_review_gallery.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/BackgroundIntensity/BackgroundIntensity.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/ColorDeconvolution/ColorDeconvolution.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/ComputeNucleiFeatures.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/ComputeNucleiFeatures/README.md` & `histomicstk-1.3.6.dev5/histomicstk/cli/ComputeNucleiFeatures/README.md`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/NucleiClassification.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/NucleiClassification.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/NucleiClassification/NucleiClassification.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/NucleiClassification/NucleiClassification.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/NucleiDetection.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/NucleiDetection.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/NucleiDetection/NucleiDetection.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/NucleiDetection/NucleiDetection.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/PositivePixelCount.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/PositivePixelCount.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/PositivePixelCount/PositivePixelCount.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsMacenkoPCA/SeparateStainsMacenkoPCA.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/SeparateStainsXuSnmf/SeparateStainsXuSnmf.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml` & `histomicstk-1.3.6.dev5/histomicstk/cli/SuperpixelSegmentation/SuperpixelSegmentation.xml`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/slicer_cli_list.json` & `histomicstk-1.3.6.dev5/histomicstk/cli/slicer_cli_list.json`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/cli/utils.py` & `histomicstk-1.3.6.dev5/histomicstk/cli/utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/features/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx` & `histomicstk-1.3.6.dev5/histomicstk/features/_compute_marginal_glcm_probs_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_fsd_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_fsd_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_global_cell_graph_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_global_cell_graph_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_gradient_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_gradient_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_haralick_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_haralick_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_intensity_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_intensity_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_morphometry_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_morphometry_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/compute_nuclei_features.py` & `histomicstk-1.3.6.dev5/histomicstk/features/compute_nuclei_features.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/features/graycomatrixext.py` & `histomicstk-1.3.6.dev5/histomicstk/features/graycomatrixext.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/filters/edge/gaussian_grad.py` & `histomicstk-1.3.6.dev5/histomicstk/filters/edge/gaussian_grad.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/filters/shape/cdog.py` & `histomicstk-1.3.6.dev5/histomicstk/filters/shape/cdog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/filters/shape/clog.py` & `histomicstk-1.3.6.dev5/histomicstk/filters/shape/clog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/filters/shape/glog.py` & `histomicstk-1.3.6.dev5/histomicstk/filters/shape/glog.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/filters/shape/vesselness.py` & `histomicstk-1.3.6.dev5/histomicstk/filters/shape/vesselness.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/augmentation/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/augmentation/color_augmentation.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/augmentation/color_augmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/lab_mean_std.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/lab_mean_std.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/lab_to_rgb.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/lab_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/od_to_rgb.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/od_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_hsi.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_lab.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_lab.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_od.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_od.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/rgb_to_sda.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/rgb_to_sda.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_conversion/sda_to_rgb.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_conversion/sda_to_rgb.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/color_convolution.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/color_convolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/color_deconvolution.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/complement_stain_matrix.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/find_stain_index.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/find_stain_index.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_macenko_pca.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/rgb_separate_stains_xu_snmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/separate_stains_macenko_pca.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_deconvolution/separate_stains_xu_snmf.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/background_intensity.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/background_intensity.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/deconvolution_based_normalization.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/reinhard.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/reinhard.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/color_normalization/reinhard_stats.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/color_normalization/reinhard_stats.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py` & `histomicstk-1.3.6.dev5/histomicstk/preprocessing/tests/test_normalization_and_augmentation.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/saliency/cellularity_detection_superpixels.py` & `histomicstk-1.3.6.dev5/histomicstk/saliency/cellularity_detection_superpixels.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/saliency/cellularity_detection_thresholding.py` & `histomicstk-1.3.6.dev5/histomicstk/saliency/cellularity_detection_thresholding.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/saliency/tests/test_saliency.py` & `histomicstk-1.3.6.dev5/histomicstk/saliency/tests/test_saliency.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/saliency/tissue_detection.py` & `histomicstk-1.3.6.dev5/histomicstk/saliency/tissue_detection.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/embed_boundaries.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/embed_boundaries.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/_trace_object_boundaries_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/area_open.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/area_open.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/compact.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/compact.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/condense.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/condense.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete_border.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete_border.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/delete_overlap.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/delete_overlap.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/dilate_xor.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/dilate_xor.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/perimeter.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/perimeter.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/remove_overlap_nuclei.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/remove_overlap_nuclei.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/shuffle.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/shuffle.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/split.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/split.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/trace_object_boundaries.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/trace_object_boundaries.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/label/width_open.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/label/width_open.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/chan_vese.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/chan_vese.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/level_set/reg_edge.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/level_set/reg_edge.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/_max_clustering_cython.pyx`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/detect_nuclei_kofahi.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/detect_tile_nuclei.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/detect_tile_nuclei.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/gaussian_voting.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/gaussian_voting.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/gvf_tracking.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/gvf_tracking.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/max_clustering.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/max_clustering.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/nuclear/min_model.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/nuclear/min_model.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/positive_pixel_count.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/positive_pixel_count.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/rag.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/rag.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/rag_add_layer.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/rag_add_layer.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/segmentation/rag_color.py` & `histomicstk-1.3.6.dev5/histomicstk/segmentation/rag_color.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/__init__.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/compute_tile_foreground_fraction.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/compute_tile_foreground_fraction.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/del2.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/del2.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/eigen.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/fit_poisson_mixture.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/fit_poisson_mixture.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/general_utils.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/girder_convenience_utils.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/girder_convenience_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/gradient_diffusion.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/gradient_diffusion.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/hessian.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/hessian.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/merge_colinear.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/merge_colinear.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/sample_pixels.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/sample_pixels.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/simple_mask.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/simple_mask.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/utils/tests/test_girder_convenience_utils.py` & `histomicstk-1.3.6.dev5/histomicstk/utils/tests/test_girder_convenience_utils.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/workflows/specific_workflows.py` & `histomicstk-1.3.6.dev5/histomicstk/workflows/specific_workflows.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/workflows/tests/test_workflow_runner.py` & `histomicstk-1.3.6.dev5/histomicstk/workflows/tests/test_workflow_runner.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk/workflows/workflow_runner.py` & `histomicstk-1.3.6.dev5/histomicstk/workflows/workflow_runner.py`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/histomicstk.egg-info/SOURCES.txt` & `histomicstk-1.3.6.dev5/histomicstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `histomicstk-1.3.6.dev4/setup.py` & `histomicstk-1.3.6.dev5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         # dask packages
         'dask[dataframe]',
         'distributed',
         # large image; for non-linux systems only install the PIL tile source
         # by default.
         'large-image[sources];sys.platform=="linux" or sys.platform=="linux2"',
         'large-image[common];sys.platform!="linux" and sys.platform!="linux2"',
+        'large-image-converter;sys.platform=="linux" or sys.platform=="linux2"',
         'girder-slicer-cli-web',
         # cli
         'ctk-cli',
     ] + (
         # Only require opencv if it isn't installed.  This can allow alternate
         # forms to be in the environment (such as a headed form) without
         # causing conflicts
```

