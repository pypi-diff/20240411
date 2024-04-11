# Comparing `tmp/autogluon.core-1.1.0b20240409.tar.gz` & `tmp/autogluon.core-1.1.0b20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-1.1.0b20240409.tar", last modified: Tue Apr  9 09:05:08 2024, max compression
+gzip compressed data, was "autogluon.core-1.1.0b20240410.tar", last modified: Wed Apr 10 09:05:43 2024, max compression
```

## Comparing `autogluon.core-1.1.0b20240409.tar` & `autogluon.core-1.1.0b20240410.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.273961 autogluon.core-1.1.0b20240409/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.273961 autogluon.core-1.1.0b20240409/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.277961 autogluon.core-1.1.0b20240409/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7069 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.277961 autogluon.core-1.1.0b20240409/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.277961 autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.277961 autogluon.core-1.1.0b20240409/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    99982 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.281961 autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    66393 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/searcher_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/stacked_overfitting/
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/stacked_overfitting/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.285961 autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   198790 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.289961 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-09 09:04:42.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 09:05:08.277961 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 09:05:08.000000 autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.159259 autogluon.core-1.1.0b20240410/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.159259 autogluon.core-1.1.0b20240410/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.163260 autogluon.core-1.1.0b20240410/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.163260 autogluon.core-1.1.0b20240410/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.163260 autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.163260 autogluon.core-1.1.0b20240410/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21154 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17849 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99982 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.167260 autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66393 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44862 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10488 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12138 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9388 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/searcher_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.171259 autogluon.core-1.1.0b20240410/src/autogluon/core/stacked_overfitting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/stacked_overfitting/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   198790 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36049 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12230 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.175259 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50695 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-10 09:05:21.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:05:43.163260 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:05:43.000000 autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-1.1.0b20240409/PKG-INFO` & `autogluon.core-1.1.0b20240410/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

### Comparing `autogluon.core-1.1.0b20240409/setup.py` & `autogluon.core-1.1.0b20240410/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/_setup_utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/_setup_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     else:
         development_status = "Development Status :: 4 - Beta"
     setup_args = dict(
         name=name,
         version=version,
         author="AutoGluon Community",
         url="https://github.com/autogluon/autogluon",
-        description="AutoML for Image, Text, and Tabular Data",
+        description="Fast and Accurate ML in 3 Lines of Code",
         long_description=long_description,
         long_description_content_type="text/markdown",
         license="Apache-2.0",
         license_files=("../LICENSE", "../NOTICE"),
         # Package info
         packages=find_namespace_packages("src", include=["autogluon.*"]),
         package_dir={"": "src"},
```

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/constants.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/data/cleaner.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/dataset.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/executors.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/__init__.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/_utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/problem_type.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/stacked_overfitting/utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/stacked_overfitting/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/trainer/utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/decorators.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/files.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/plots.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/time.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon/core/utils/version_utils.py` & `autogluon.core-1.1.0b20240410/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 1.1.0b20240409
-Summary: AutoML for Image, Text, and Tabular Data
+Version: 1.1.0b20240410
+Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
 Project-URL: Contribute!, https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md
 Description: 
         
         <div align="center">
         <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
         
-        ## AutoML for Image, Text, Time Series, and Tabular Data
+        ## Fast and Accurate ML in 3 Lines of Code
         
         [![Latest Release](https://img.shields.io/github/v/release/autogluon/autogluon)](https://github.com/autogluon/autogluon/releases)
         [![Conda Forge](https://img.shields.io/conda/vn/conda-forge/autogluon.svg)](https://anaconda.org/conda-forge/autogluon)
         [![Python Versions](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://pypi.org/project/autogluon/)
         [![Downloads](https://pepy.tech/badge/autogluon/month)](https://pepy.tech/project/autogluon)
         [![GitHub license](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](./LICENSE)
         [![Discord](https://img.shields.io/discord/1043248669505368144?logo=discord&style=flat)](https://discord.gg/wjUmjqAc2N)
```

### Comparing `autogluon.core-1.1.0b20240409/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-1.1.0b20240410/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

