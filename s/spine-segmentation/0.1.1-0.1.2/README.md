# Comparing `tmp/spine_segmentation-0.1.1.tar.gz` & `tmp/spine_segmentation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_segmentation-0.1.1.tar", max compression
+gzip compressed data, was "spine_segmentation-0.1.2.tar", max compression
```

## Comparing `spine_segmentation-0.1.1.tar` & `spine_segmentation-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.1.1/README.md
--rw-r--r--   0        0        0     2384 2024-04-11 15:14:35.104645 spine_segmentation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.1.1/spine_segmentation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/annotators/__init__.py
--rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.1.1/spine_segmentation/annotators/annotator_base.py
--rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.1.1/spine_segmentation/annotators/vector_annotator.py
--rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.1.1/spine_segmentation/cli/cli.py
--rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/dataloader/statistics.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/datasets/__init__.py
--rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/datasets/augmentation.py
--rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.1.1/spine_segmentation/datasets/feature_dataset.py
--rw-r--r--   0        0        0     6705 2024-04-11 12:53:48.902194 spine_segmentation-0.1.1/spine_segmentation/datasets/metadata_prediction_dataset.py
--rw-r--r--   0        0        0     6381 2024-04-11 12:53:48.762192 spine_segmentation-0.1.1/spine_segmentation/datasets/patch_segmentation_dataset.py
--rw-r--r--   0        0        0    14739 2024-04-11 12:53:48.922194 spine_segmentation-0.1.1/spine_segmentation/datasets/sample.py
--rw-r--r--   0        0        0    16055 2024-04-11 12:53:48.926194 spine_segmentation-0.1.1/spine_segmentation/datasets/segmentation_dataset.py
--rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.1.1/spine_segmentation/datasets/vector_table_graphs_dataset.py
--rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.1.1/spine_segmentation/evaluate/analyze_edge_cases.py
--rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.1.1/spine_segmentation/evaluate/analyze_index_list.py
--rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.1.1/spine_segmentation/evaluate/classic_ml.py
--rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_created_stats.py
--rw-r--r--   0        0        0    15476 2024-04-11 12:53:48.810193 spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_instance_seg_model.py
--rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_splitting.py
--rw-r--r--   0        0        0     6058 2024-04-11 12:53:48.910194 spine_segmentation-0.1.1/spine_segmentation/evaluate/load_model.py
--rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.1.1/spine_segmentation/evaluate/metadata.py
--rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.1.1/spine_segmentation/evaluate/volume_size_in_gt.py
--rw-r--r--   0        0        0    15646 2024-04-11 14:48:08.453915 spine_segmentation-0.1.1/spine_segmentation/inference/instance_segmentation.py
--rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.1.1/spine_segmentation/inference/onnx_model.py
--rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.1.1/spine_segmentation/instance_separation/instance_separation.py
--rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/losses/diffis1.py
--rw-r--r--   0        0        0     2080 2024-04-11 12:31:31.109485 spine_segmentation-0.1.1/spine_segmentation/model_downloader/model_downloader.py
--rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.1.1/spine_segmentation/plotting/bmi.py
--rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.1.1/spine_segmentation/plotting/classification_correlation.py
--rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.1.1/spine_segmentation/plotting/patient_metadata.py
--rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.1.1/spine_segmentation/plotting/plot_slice.py
--rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.1.1/spine_segmentation/plotting/plot_statistics.py
--rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.1.1/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
--rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.1.1/spine_segmentation/plotting/show_plane_splitting_3d.py
--rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.1.1/spine_segmentation/plotting/ydata_profile_report.py
--rw-r--r--   0        0        0      883 2024-04-11 12:39:30.017665 spine_segmentation-0.1.1/spine_segmentation/resources/paths.py
--rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.1.1/spine_segmentation/resources/preloaded.py
--rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.1.1/spine_segmentation/run.py
--rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/scripts/format_results.py
--rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.1.1/spine_segmentation/scripts/split_train_val_test.py
--rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/scripts/test_patient_ids.txt
--rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.1.1/spine_segmentation/spine_types/disc.py
--rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/spine_types/labels.py
--rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/spine_types/line_segment.py
--rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/spine_types/plane.py
--rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/spine_types/roi.py
--rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/spine_types/spine.py
--rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.1.1/spine_segmentation/spine_types/vertebra.py
--rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.1.1/spine_segmentation/trainer/learning_rate_finder.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/__init__.py
--rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/fix_validations_step_bar.py
--rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/globals.py
--rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/log_dir.py
--rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/profiling.py
--rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/utils/proxy_class.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/visualisation/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/__init__.py
--rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/blender_script.py
--rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/gen_obj.py
--rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/open_in_blender.py
--rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.1.1/spine_segmentation/visualisation/color.py
--rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.1.1/spine_segmentation/visualisation/color_palettes.py
--rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 spine_segmentation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-11 11:32:29.446351 spine_segmentation-0.1.2/README.md
+-rw-r--r--   0        0        0     2382 2024-04-11 15:48:29.945986 spine_segmentation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-11 12:53:48.914194 spine_segmentation-0.1.2/spine_segmentation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/annotators/__init__.py
+-rw-r--r--   0        0        0    16308 2024-04-11 12:53:48.934194 spine_segmentation-0.1.2/spine_segmentation/annotators/annotator_base.py
+-rw-r--r--   0        0        0     8225 2024-04-11 12:53:48.814193 spine_segmentation-0.1.2/spine_segmentation/annotators/vector_annotator.py
+-rw-r--r--   0        0        0     2190 2024-04-11 12:53:48.766192 spine_segmentation-0.1.2/spine_segmentation/cli/cli.py
+-rw-r--r--   0        0        0    12072 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/dataloader/statistics.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/datasets/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/datasets/augmentation.py
+-rw-r--r--   0        0        0     4312 2024-04-11 12:53:48.806193 spine_segmentation-0.1.2/spine_segmentation/datasets/feature_dataset.py
+-rw-r--r--   0        0        0     6696 2024-04-11 15:53:29.418496 spine_segmentation-0.1.2/spine_segmentation/datasets/metadata_prediction_dataset.py
+-rw-r--r--   0        0        0     6372 2024-04-11 15:53:29.430496 spine_segmentation-0.1.2/spine_segmentation/datasets/patch_segmentation_dataset.py
+-rw-r--r--   0        0        0     1360 2024-04-11 15:53:29.410496 spine_segmentation-0.1.2/spine_segmentation/datasets/path_helper.py
+-rw-r--r--   0        0        0    14744 2024-04-11 15:47:48.534212 spine_segmentation-0.1.2/spine_segmentation/datasets/sample.py
+-rw-r--r--   0        0        0    14989 2024-04-11 15:53:29.422496 spine_segmentation-0.1.2/spine_segmentation/datasets/segmentation_dataset.py
+-rw-r--r--   0        0        0     2037 2024-04-11 12:53:48.782192 spine_segmentation-0.1.2/spine_segmentation/datasets/vector_table_graphs_dataset.py
+-rw-r--r--   0        0        0     2581 2024-04-11 12:53:48.890194 spine_segmentation-0.1.2/spine_segmentation/evaluate/analyze_edge_cases.py
+-rw-r--r--   0        0        0     2520 2024-04-11 12:53:48.798193 spine_segmentation-0.1.2/spine_segmentation/evaluate/analyze_index_list.py
+-rw-r--r--   0        0        0     1659 2024-04-11 12:53:48.854193 spine_segmentation-0.1.2/spine_segmentation/evaluate/classic_ml.py
+-rw-r--r--   0        0        0     1108 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_created_stats.py
+-rw-r--r--   0        0        0    15527 2024-04-11 15:52:07.339228 spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_instance_seg_model.py
+-rw-r--r--   0        0        0     8215 2024-04-11 12:53:48.746192 spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_splitting.py
+-rw-r--r--   0        0        0     6109 2024-04-11 15:52:07.363228 spine_segmentation-0.1.2/spine_segmentation/evaluate/load_model.py
+-rw-r--r--   0        0        0     4885 2024-04-11 12:53:48.882194 spine_segmentation-0.1.2/spine_segmentation/evaluate/metadata.py
+-rw-r--r--   0        0        0     1627 2024-04-11 12:53:48.894194 spine_segmentation-0.1.2/spine_segmentation/evaluate/volume_size_in_gt.py
+-rw-r--r--   0        0        0    15726 2024-04-11 15:52:07.351228 spine_segmentation-0.1.2/spine_segmentation/inference/instance_segmentation.py
+-rw-r--r--   0        0        0     6761 2024-04-11 12:53:48.846193 spine_segmentation-0.1.2/spine_segmentation/inference/onnx_model.py
+-rw-r--r--   0        0        0     7515 2024-04-11 12:53:48.906194 spine_segmentation-0.1.2/spine_segmentation/instance_separation/instance_separation.py
+-rw-r--r--   0        0        0      304 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/losses/diffis1.py
+-rw-r--r--   0        0        0     2080 2024-04-11 15:40:00.222464 spine_segmentation-0.1.2/spine_segmentation/model_downloader/model_downloader.py
+-rw-r--r--   0        0        0      712 2024-04-11 12:53:48.850193 spine_segmentation-0.1.2/spine_segmentation/plotting/bmi.py
+-rw-r--r--   0        0        0     8132 2024-04-11 12:53:48.778192 spine_segmentation-0.1.2/spine_segmentation/plotting/classification_correlation.py
+-rw-r--r--   0        0        0     2566 2024-04-11 12:53:48.886194 spine_segmentation-0.1.2/spine_segmentation/plotting/patient_metadata.py
+-rw-r--r--   0        0        0    10404 2024-04-11 12:53:48.826193 spine_segmentation-0.1.2/spine_segmentation/plotting/plot_slice.py
+-rw-r--r--   0        0        0     1795 2024-04-11 12:53:48.938195 spine_segmentation-0.1.2/spine_segmentation/plotting/plot_statistics.py
+-rw-r--r--   0        0        0     5823 2024-04-11 12:53:48.834193 spine_segmentation-0.1.2/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py
+-rw-r--r--   0        0        0     5767 2024-04-11 12:53:48.786192 spine_segmentation-0.1.2/spine_segmentation/plotting/show_plane_splitting_3d.py
+-rw-r--r--   0        0        0      266 2024-04-11 12:53:48.858193 spine_segmentation-0.1.2/spine_segmentation/plotting/ydata_profile_report.py
+-rw-r--r--   0        0        0      930 2024-04-11 15:55:12.773382 spine_segmentation-0.1.2/spine_segmentation/resources/paths.py
+-rw-r--r--   0        0        0      933 2024-04-11 12:53:48.842193 spine_segmentation-0.1.2/spine_segmentation/resources/preloaded.py
+-rw-r--r--   0        0        0       63 2024-04-11 09:34:14.336647 spine_segmentation-0.1.2/spine_segmentation/run.py
+-rw-r--r--   0        0        0     4575 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/scripts/format_results.py
+-rw-r--r--   0        0        0     4546 2024-04-11 12:53:48.866193 spine_segmentation-0.1.2/spine_segmentation/scripts/split_train_val_test.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/scripts/test_patient_ids.txt
+-rw-r--r--   0        0        0      112 2024-04-10 18:52:49.798849 spine_segmentation-0.1.2/spine_segmentation/spine_types/disc.py
+-rw-r--r--   0        0        0     1033 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/spine_types/labels.py
+-rw-r--r--   0        0        0      219 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/spine_types/line_segment.py
+-rw-r--r--   0        0        0     2409 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/spine_types/plane.py
+-rw-r--r--   0        0        0       67 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/spine_types/roi.py
+-rw-r--r--   0        0        0      246 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/spine_types/spine.py
+-rw-r--r--   0        0        0      116 2024-04-10 18:52:49.974852 spine_segmentation-0.1.2/spine_segmentation/spine_types/vertebra.py
+-rw-r--r--   0        0        0     1190 2024-04-11 12:53:48.874194 spine_segmentation-0.1.2/spine_segmentation/trainer/learning_rate_finder.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/fix_validations_step_bar.py
+-rw-r--r--   0        0        0      218 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/globals.py
+-rw-r--r--   0        0        0      552 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/log_dir.py
+-rw-r--r--   0        0        0      690 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/profiling.py
+-rw-r--r--   0        0        0      930 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/utils/proxy_class.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/visualisation/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/__init__.py
+-rw-r--r--   0        0        0    11971 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/blender_script.py
+-rw-r--r--   0        0        0     9179 2024-04-11 12:53:48.830193 spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/gen_obj.py
+-rw-r--r--   0        0        0     8158 2024-04-11 12:53:48.822193 spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/open_in_blender.py
+-rw-r--r--   0        0        0    12036 2024-04-10 12:31:20.207512 spine_segmentation-0.1.2/spine_segmentation/visualisation/color.py
+-rw-r--r--   0        0        0     1705 2024-04-11 12:53:48.794192 spine_segmentation-0.1.2/spine_segmentation/visualisation/color_palettes.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 spine_segmentation-0.1.2/PKG-INFO
```

### Comparing `spine_segmentation-0.1.1/README.md` & `spine_segmentation-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/pyproject.toml` & `spine_segmentation-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spine-segmentation"
-version = "0.1.1"
+version = "0.1.2"
 description = "Anatomical labeling of the spine in small field-of-view MRI scans"
 authors = [
     "Brutenis Gliwa <brutenis@gmail.com>",
 ]
 readme = "README.md"
 
 classifiers = [
@@ -17,49 +17,53 @@
   "Programming Language :: Python :: 3.9",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.13.0"
-#pandas = "<2"                           # basic
 numpy = "^1.23.0"                       # basic
-#loguru = "^0.7.0"                       # logging
 #torch = "^2.1.1"
 #torch-geometric = "^2.3.1"              # gnn in pytorch
 #lightning = "^2.2.1"
 # onnx = "^1.14.1"
 onnxruntime = "^1.15.1"
 onnxruntime-gpu = "^1.15.1"
 #torchvision = "^0.17.2"
 tqdm = "^4.66.2"
 requests = "^2.31.0"
+xxhash = "^3.4.1"
+connected-components-3d = "^3.12.1"     # algorithms for finding connected compoents
+pandas = "<2.0"
+scikit-learn = "^1.2.2"                 # ML
+seaborn = "^0.13.0"
+nibabel = "^5.1.0"                      # load nifti images
+pydicom = "^2.4.3"
+loguru = "^0.7.2"
+
+[tool.poetry.group.training]
+optional = true
 
 [tool.poetry.group.training.dependencies]
 vispy = "^0.13.0"                       # plotting 3D
 matplotlib = "^3.7.1"                   # plotting
-nibabel = "^5.1.0"                      # load nifti images
 mlflow = "^2.4.0"                       # logging online
 tabulate = "^0.9.0"                     # pretty print tables in markdown
 pyside6 = "^6.5.0"                      # required for vispy plotting
-scikit-learn = "^1.2.2"                 # ML
 datasets = "^2.12.0"                    # datasets for gnn
 segmentation-models-pytorch = "^0.3.3"  # pretrained models in pytorch
-connected-components-3d = "^3.12.1"     # algorithms for finding connected compoents
 websockets = "^11.0.3"                  # otherwise there is an error with pydantic if the version is too new
 fastapi = ">=0.80"                      # otherwise there is an error with pydantic if the version is too new
 jsonargparse = {extras = ["signatures"], version = "^4.23.1"}
 kornia = "^0.6.12"
 monai = "^1.2.0"
 openmim = "^0.3.9"
 netron = "^7.1.5"
 xgboost = "^1.7.6"
 pyqt6 = "^6.5.2"
-pydicom = "^2.4.3"
-seaborn = "^0.13.0"
 efficientnet-pytorch-3d = {git = "https://github.com/shijianjian/EfficientNet-PyTorch-3D"}
 
 [build-system]
 requires = ["poetry-core"]
 
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/annotators/annotator_base.py` & `spine_segmentation-0.1.2/spine_segmentation/annotators/annotator_base.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/annotators/vector_annotator.py` & `spine_segmentation-0.1.2/spine_segmentation/annotators/vector_annotator.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/cli/cli.py` & `spine_segmentation-0.1.2/spine_segmentation/cli/cli.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/dataloader/statistics.py` & `spine_segmentation-0.1.2/spine_segmentation/dataloader/statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/augmentation.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/augmentation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/feature_dataset.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/feature_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/metadata_prediction_dataset.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/metadata_prediction_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset
 
 from spine_segmentation.datasets.sample import GTFormat, MetadataSample, MetadataTypes, get_pid_to_index_lookup
-from spine_segmentation.datasets.segmentation_dataset import get_potential_data_dirs
+from spine_segmentation.datasets.path_helper import get_potential_data_dirs
 from spine_segmentation.resources.paths import NAKO_DATASET_PATH
 
 
 class MetadataPredictionDataset(Dataset):
     def __init__(self, data_dirs: Iterable[Path], transform=None, gt_type: MetadataTypes = ["weight", "size", "age"]):
         super().__init__()
         self.target_shape = (18, 320, 896)
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/patch_segmentation_dataset.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/patch_segmentation_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import lightning.pytorch as pl
 import numpy as np
 import torch
 from torch.utils.data import DataLoader, Dataset
 
 from spine_segmentation.datasets.augmentation import ImageAugmentation
 from spine_segmentation.datasets.sample import GTFormat, Sample
-from spine_segmentation.datasets.segmentation_dataset import get_potential_data_dirs
+from spine_segmentation.datasets.path_helper import get_potential_data_dirs
 from spine_segmentation.resources.paths import NAKO_DATASET_PATH
 
 
 class PatchSegmentationDataset(Dataset):
     def __init__(
         self, data_dirs: Iterable[Path], transform=None, subset_size: int = 20, mode: Literal["val", "train"] = "val"
     ):
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/sample.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from io import BytesIO
 from pathlib import Path
 from typing import Dict, Iterable, List, Literal, Optional, Set, Tuple, Union
 
 import nibabel as nib
 import numpy as np
 import pydicom
-import torch
 
 from spine_segmentation.instance_separation.instance_separation import separate_rois_with_labels
 from spine_segmentation.resources.preloaded import get_measure_statistics
 
 MetadataType = Literal["age", "sex", "weight", "size"]
 MetadataTypes = Union[MetadataType, Iterable[MetadataType]]
 
@@ -83,16 +82,15 @@
     nifti = nib.load(path).get_fdata()
     img = _normalize_image(nifti, *args, **kwargs)
     if return_nifti:
         return img, nifti
     return img
 
 
-class MissingGTError(Exception):
-    ...
+class MissingGTError(Exception): ...
 
 
 @lru_cache
 def get_pid_to_index_lookup():
     stats = get_measure_statistics()
     ids = stats.dicom_metadata["DICOM;PatientID"]
     return {pid.split("_")[0]: i for i, pid in enumerate(ids)}
@@ -116,14 +114,16 @@
         self.pid = path.name
         self.image, self.nifti = _load_and_normalize(path / f"{self.pid}.nii.gz", target_shape, return_nifti=True)
         # self.wk = _load_and_normalize(path / f"{pid}_WK.nii.gz", is_gt=True)
         # self.bs = _load_and_normalize(path / f"{pid}_BS.nii.gz", is_gt=True)
         self.gt = self._compose_groundtruth(gt_type)
 
     def _compose_groundtruth(self, gt_types: MetadataTypes):
+        import torch
+
         stats = get_measure_statistics()
         lookup = get_pid_to_index_lookup()
         try:
             row = stats.dicom_metadata.iloc[lookup[self.pid]]
         except KeyError:
             raise MissingGTError(f"Missing ground truth for this sample {self.pid=}")
         gt = []
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/segmentation_dataset.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/segmentation_dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import numpy as np
 import pandas as pd
 import torch
 from torch import Tensor
 from torch.utils.data import DataLoader, Dataset
 
 from spine_segmentation.datasets.augmentation import ImageAugmentation
+from spine_segmentation.datasets.path_helper import expand_path_to_data_dirs
 from spine_segmentation.datasets.sample import GTFormat, Sample
 from spine_segmentation.resources.paths import NAKO_DATASET_PATH
 from spine_segmentation.resources.other_paths import RAW_NAKO_DATASET_PATH
 
 
 class SegmentationDataset(Dataset):
     def __init__(
@@ -201,51 +202,14 @@
         plt.tight_layout(pad=0)
         self.gt_format = previous_gt_format
         # plt.title(f"Image ({index=}) ({image.shape=}) ")
         plt.gcf().set_dpi(300)
         plt.show()
 
 
-def get_potential_data_dirs(data_dir, required_suffixes=("", "_BS", "_WK", "_NR"), intersection_with=None):
-    if intersection_with is None:
-
-        class AlwaysTrue:
-            def __contains__(self, _):
-                return True
-
-        intersection_with = AlwaysTrue()
-    paths = []
-    for path in Path(data_dir).glob("*"):
-        if path.name in intersection_with:
-            if all((path / f"{path.name}{suffix}.nii.gz").exists() for suffix in required_suffixes):
-                paths.append(path)
-    return paths
-
-
-def expand_path_to_data_dirs(path: Union[Path, str]) -> List[Path]:
-    path = Path(path)
-    if path.suffix == ".npz":
-        npz = np.load(path, allow_pickle=True)
-        return list(npz["index_to_zip_path"].item().values())
-
-    if path.suffix == ".csv":
-        import pandas as pd
-
-        csv = pd.read_csv(path)
-        return list(csv["Path"])
-
-    if path == RAW_NAKO_DATASET_PATH:
-        return list(RAW_NAKO_DATASET_PATH.glob("*.zip"))
-
-    if path == NAKO_DATASET_PATH:
-        return get_potential_data_dirs(path, required_suffixes=("", "_WK"))
-
-    raise ValueError(f"Invalid path {path=}")
-
-
 class SegmentationDataModule(pl.LightningDataModule):
     def __init__(
         self,
         data_dir: Union[str, Path, List[str], Tuple[str]] = NAKO_DATASET_PATH,
         batch_size=1,
         num_workers=2,
         gt_format: GTFormat = GTFormat(),
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/datasets/vector_table_graphs_dataset.py` & `spine_segmentation-0.1.2/spine_segmentation/datasets/vector_table_graphs_dataset.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/analyze_edge_cases.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/analyze_edge_cases.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/analyze_index_list.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/analyze_index_list.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/classic_ml.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/classic_ml.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_created_stats.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_created_stats.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_instance_seg_model.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_instance_seg_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 from spine_segmentation.utils.log_dir import get_next_log_dir
 from spine_segmentation.visualisation.blender.open_in_blender import open_in_blender
 
 colored_tracebacks()
 
 import numpy as np
 
-from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule, expand_path_to_data_dirs
+from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule
+from spine_segmentation.datasets.path_helper import expand_path_to_data_dirs
 
 
 def get_dataloader(
     train_or_val: Literal["train", "val"], path: Union[Path, str] = None, *, bs: int = 16, crop_height: int = None
 ):
     args = [] if path is None else [path]
     data_module = SegmentationDataModule(
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/eval_splitting.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/eval_splitting.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/load_model.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/load_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 
 colored_tracebacks()
 
 import numpy as np
 import onnx
 from loguru import logger
 
-from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule, expand_path_to_data_dirs
+from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule
+from spine_segmentation.datasets.path_helper import expand_path_to_data_dirs
 
 # onnx_model_path = "models/segmentation/2023-08-31_Seg_Unet_mit.onnx"
 onnx_model_path = "models/segmentation/2023-09-12_Seg_Unet_mitb5.onnx"
 
 
 def get_dataloader(train_or_val: Literal["train", "val"], path: Union[Path, str] = None, *, bs: int = 16):
     args = [] if path is None else [path]
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/metadata.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/evaluate/volume_size_in_gt.py` & `spine_segmentation-0.1.2/spine_segmentation/evaluate/volume_size_in_gt.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/inference/instance_segmentation.py` & `spine_segmentation-0.1.2/spine_segmentation/inference/instance_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 import random
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Literal, Union, Dict
 
-import torch
 
-from spine_segmentation.cli.cli import colored_tracebacks
-from spine_segmentation.datasets.sample import SampleIterator, get_random_crop_slice
 from spine_segmentation.inference.onnx_model import ONNXInferenceModel
 from spine_segmentation.instance_separation.instance_separation import (
     get_planes_from_rois,
     mask_rare_rois,
     separate_rois_with_labels,
     separate_segmented_rois_by_planes,
 )
-from spine_segmentation.plotting.plot_slice import get_stats, plot_npz, single_plot
 from spine_segmentation.resources.paths import TRAIN_SPLIT_CSV_PATH, VAL_SPLIT_CSV_PATH
 from spine_segmentation.resources.other_paths import RAW_NAKO_DATASET_PATH
 from spine_segmentation.spine_types.labels import get_labels_for_n_classes
 from spine_segmentation.utils.log_dir import get_next_log_dir
 from spine_segmentation.visualisation.blender.open_in_blender import open_in_blender
 
-colored_tracebacks()
-
 import numpy as np
 
-from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule, expand_path_to_data_dirs
-
 
 def get_dataloader(
     train_or_val: Literal["train", "val"], path: Union[Path, str] = None, *, bs: int = 16, crop_height: int = None
 ):
+    from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule
+
     args = [] if path is None else [path]
     data_module = SegmentationDataModule(
         *args,
         # add_bs_wk_as_channels=True,
         add_adjacent_slices=True,
         batch_size=bs,
         num_workers=4,
@@ -185,14 +179,20 @@
         if stat:
             correct_sum += stat["correct"]
             correct_no_edges_sum += stat["correct_no_edges"]
     print(f"{correct_sum=} / {len(stats)}, {correct_no_edges_sum=} / {len(stats)}")
 
 
 def plot_every_val_dataset(directory=None, device=3, model_height=896, cropped_height=None, cropped_V=None):
+    import torch
+    from spine_segmentation.datasets.sample import SampleIterator, get_random_crop_slice
+    from spine_segmentation.plotting.plot_slice import get_stats, plot_npz, single_plot
+    from spine_segmentation.datasets.segmentation_dataset import SegmentationDataModule
+    from spine_segmentation.datasets.path_helper import expand_path_to_data_dirs
+
     if directory is None:
         directory = get_next_log_dir()
     directory = Path(directory)
 
     if cropped_V is not None:
         assert 1 <= cropped_V <= 49
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/inference/onnx_model.py` & `spine_segmentation-0.1.2/spine_segmentation/inference/onnx_model.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/instance_separation/instance_separation.py` & `spine_segmentation-0.1.2/spine_segmentation/instance_separation/instance_separation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/model_downloader/model_downloader.py` & `spine_segmentation-0.1.2/spine_segmentation/model_downloader/model_downloader.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Optional
+from pathlib import Path
 
 import requests
 from tqdm import tqdm
-from pathlib import Path
 
 
 def _get_config_path(program_name="spine") -> Path:
     """Get OS-agnostic path for program configuration."""
 
     home = Path.home().absolute()
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/bmi.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/bmi.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/classification_correlation.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/classification_correlation.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/patient_metadata.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/patient_metadata.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/plot_slice.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/plot_slice.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/plot_statistics.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/plot_statistics.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/read_npz_eval_per_roi_accuracy.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/plotting/show_plane_splitting_3d.py` & `spine_segmentation-0.1.2/spine_segmentation/plotting/show_plane_splitting_3d.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/resources/paths.py` & `spine_segmentation-0.1.2/spine_segmentation/resources/paths.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from pathlib import Path
 
 PROJECT_PATH = Path(__file__).absolute().parent.parent.parent
 
-CACHE_PATH = PROJECT_PATH / "cache"
-
 DATASETS_PATH = PROJECT_PATH / "datasets"
 REPORTS_PATH = PROJECT_PATH / "reports"
 MODELS_PATH = PROJECT_PATH / "models"
 SECRETS_PATH = PROJECT_PATH / "secrets"
 LOGS_PATH = PROJECT_PATH / "logs"
 
 PLOTS_PATH = REPORTS_PATH / "plots"
 RESULTS_PATH = REPORTS_PATH / "results"
 
 MEASURE_STATISTICS_PATH = DATASETS_PATH / "measure_statistics_new.csv"
 VECTOR_TABLE_PATH = DATASETS_PATH / "vector_table_new.npz"
 
 # Paths outside repository
 
+CACHE_PATH = Path("/tmp/spine-segmentation-cache")
+CACHE_PATH.mkdir(exist_ok=True)
+
 NAS_RESEARCH_PATH = Path("~/devel/data_remote/nas_research").expanduser().resolve()
 NAKO_DATASET_PATH = NAS_RESEARCH_PATH / "path"
 
 LOCAL_NAKO_DATASET_PATH = Path.home() / "Data/nako/2022-08-22"
 
 VAL_SPLIT_CSV_PATH = DATASETS_PATH / "nako_splits/val_seg.csv"
 TRAIN_SPLIT_CSV_PATH = DATASETS_PATH / "nako_splits/train_seg.csv"
```

### Comparing `spine_segmentation-0.1.1/spine_segmentation/resources/preloaded.py` & `spine_segmentation-0.1.2/spine_segmentation/resources/preloaded.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/scripts/format_results.py` & `spine_segmentation-0.1.2/spine_segmentation/scripts/format_results.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/scripts/split_train_val_test.py` & `spine_segmentation-0.1.2/spine_segmentation/scripts/split_train_val_test.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/spine_types/labels.py` & `spine_segmentation-0.1.2/spine_segmentation/spine_types/labels.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/spine_types/plane.py` & `spine_segmentation-0.1.2/spine_segmentation/spine_types/plane.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/trainer/learning_rate_finder.py` & `spine_segmentation-0.1.2/spine_segmentation/trainer/learning_rate_finder.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/utils/fix_validations_step_bar.py` & `spine_segmentation-0.1.2/spine_segmentation/utils/fix_validations_step_bar.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/utils/log_dir.py` & `spine_segmentation-0.1.2/spine_segmentation/utils/log_dir.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/utils/profiling.py` & `spine_segmentation-0.1.2/spine_segmentation/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/utils/proxy_class.py` & `spine_segmentation-0.1.2/spine_segmentation/utils/proxy_class.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/blender_script.py` & `spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/blender_script.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/gen_obj.py` & `spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/gen_obj.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/visualisation/blender/open_in_blender.py` & `spine_segmentation-0.1.2/spine_segmentation/visualisation/blender/open_in_blender.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/visualisation/color.py` & `spine_segmentation-0.1.2/spine_segmentation/visualisation/color.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/spine_segmentation/visualisation/color_palettes.py` & `spine_segmentation-0.1.2/spine_segmentation/visualisation/color_palettes.py`

 * *Files identical despite different names*

### Comparing `spine_segmentation-0.1.1/PKG-INFO` & `spine_segmentation-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spine-segmentation
-Version: 0.1.1
+Version: 0.1.2
 Summary: Anatomical labeling of the spine in small field-of-view MRI scans
 Author: Brutenis Gliwa
 Author-email: brutenis@gmail.com
 Requires-Python: >=3.8.1,<3.13.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -13,19 +13,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: connected-components-3d (>=3.12.1,<4.0.0)
+Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0)
 Requires-Dist: onnxruntime-gpu (>=1.15.1,<2.0.0)
+Requires-Dist: pandas (<2.0)
+Requires-Dist: pydicom (>=2.4.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
+Requires-Dist: seaborn (>=0.13.0,<0.14.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: xxhash (>=3.4.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">Spine</h1>
 
 A python library including pretrained models in order to annotate vertebrae and IVDs (intevertebral discs) on small FOV (field-of-view) MRIs. This was created as part of my [master's thesis](https://brutenis.net/master-thesis) which was submitted on 9 November 2023.
 
 ## Showcase
```

