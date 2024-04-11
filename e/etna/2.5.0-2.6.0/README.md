# Comparing `tmp/etna-2.5.0.tar.gz` & `tmp/etna-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etna-2.5.0.tar", max compression
+gzip compressed data, was "etna-2.6.0.tar", max compression
```

## Comparing `etna-2.5.0.tar` & `etna-2.6.0.tar`

### file list

```diff
@@ -1,228 +1,232 @@
--rw-r--r--   0        0        0    11244 2024-03-21 09:57:35.733574 etna-2.5.0/LICENSE
--rw-r--r--   0        0        0    17117 2024-03-21 09:57:35.733574 etna-2.5.0/README.md
--rw-r--r--   0        0        0       49 2024-03-21 09:57:35.737574 etna-2.5.0/etna/__init__.py
--rw-r--r--   0        0        0     2676 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/__init__.py
--rw-r--r--   0        0        0      599 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/decomposition/__init__.py
--rw-r--r--   0        0        0    16581 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/decomposition/plots.py
--rw-r--r--   0        0        0     1161 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/decomposition/search.py
--rw-r--r--   0        0        0     9950 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/decomposition/utils.py
--rw-r--r--   0        0        0      475 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/eda/__init__.py
--rw-r--r--   0        0        0    26096 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/eda/plots.py
--rw-r--r--   0        0        0     4113 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/eda/utils.py
--rw-r--r--   0        0        0      472 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_relevance/__init__.py
--rw-r--r--   0        0        0     6004 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_relevance/plots.py
--rw-r--r--   0        0        0     4340 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_relevance/relevance.py
--rw-r--r--   0        0        0     4095 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_relevance/relevance_table.py
--rw-r--r--   0        0        0      654 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_relevance/utils.py
--rw-r--r--   0        0        0      213 2024-03-21 09:57:35.737574 etna-2.5.0/etna/analysis/feature_selection/__init__.py
--rw-r--r--   0        0        0     5377 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/feature_selection/mrmr_selection.py
--rw-r--r--   0        0        0      737 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/forecast/__init__.py
--rw-r--r--   0        0        0    36919 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/forecast/plots.py
--rw-r--r--   0        0        0     4227 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/forecast/utils.py
--rw-r--r--   0        0        0      517 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/__init__.py
--rw-r--r--   0        0        0     6827 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/density_outliers.py
--rw-r--r--   0        0        0    13578 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/hist_outliers.py
--rw-r--r--   0        0        0     2186 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/median_outliers.py
--rw-r--r--   0        0        0     5359 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/plots.py
--rw-r--r--   0        0        0     4291 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/outliers/prediction_interval_outliers.py
--rw-r--r--   0        0        0     1471 2024-03-21 09:57:35.741574 etna-2.5.0/etna/analysis/utils.py
--rw-r--r--   0        0        0     1083 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/__init__.py
--rw-r--r--   0        0        0    32050 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/auto.py
--rw-r--r--   0        0        0      102 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/optuna/__init__.py
--rw-r--r--   0        0        0     4737 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/optuna/config_sampler.py
--rw-r--r--   0        0        0     2828 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/optuna/wrapper.py
--rw-r--r--   0        0        0       93 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/pool/__init__.py
--rw-r--r--   0        0        0     1719 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/pool/generator.py
--rw-r--r--   0        0        0     5348 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/pool/templates.py
--rw-r--r--   0        0        0      495 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/pool/utils.py
--rw-r--r--   0        0        0      217 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/runner/__init__.py
--rw-r--r--   0        0        0      604 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/runner/base.py
--rw-r--r--   0        0        0     2531 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/runner/local.py
--rw-r--r--   0        0        0      171 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/runner/utils.py
--rw-r--r--   0        0        0     1664 2024-03-21 09:57:35.741574 etna-2.5.0/etna/auto/utils.py
--rw-r--r--   0        0        0      632 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/__init__.py
--rw-r--r--   0        0        0      686 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/base.py
--rw-r--r--   0        0        0      259 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/distances/__init__.py
--rw-r--r--   0        0        0     3756 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/distances/base.py
--rw-r--r--   0        0        0     4508 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/distances/distance_matrix.py
--rw-r--r--   0        0        0     5597 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/distances/dtw_distance.py
--rw-r--r--   0        0        0     1705 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/distances/euclidean_distance.py
--rw-r--r--   0        0        0      289 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/hierarchical/__init__.py
--rw-r--r--   0        0        0     6251 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/hierarchical/base.py
--rw-r--r--   0        0        0     1501 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/hierarchical/dtw_clustering.py
--rw-r--r--   0        0        0     1561 2024-03-21 09:57:35.741574 etna-2.5.0/etna/clustering/hierarchical/euclidean_clustering.py
--rw-r--r--   0        0        0      422 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/__init__.py
--rw-r--r--   0        0        0      197 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/__main__.py
--rw-r--r--   0        0        0     4832 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/backtest_command.py
--rw-r--r--   0        0        0     7210 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/forecast_command.py
--rw-r--r--   0        0        0      281 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/resolvers.py
--rw-r--r--   0        0        0     4415 2024-03-21 09:57:35.741574 etna-2.5.0/etna/commands/utils.py
--rw-r--r--   0        0        0      257 2024-03-21 09:57:35.741574 etna-2.5.0/etna/core/__init__.py
--rw-r--r--   0        0        0    12396 2024-03-21 09:57:35.741574 etna-2.5.0/etna/core/mixins.py
--rw-r--r--   0        0        0      631 2024-03-21 09:57:35.741574 etna-2.5.0/etna/core/saving.py
--rw-r--r--   0        0        0     2540 2024-03-21 09:57:35.741574 etna-2.5.0/etna/core/utils.py
--rw-r--r--   0        0        0      651 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/__init__.py
--rw-r--r--   0        0        0     8274 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/datasets_generation.py
--rw-r--r--   0        0        0     7778 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/hierarchical_structure.py
--rw-r--r--   0        0        0    39945 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/internal_datasets.py
--rw-r--r--   0        0        0    68438 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/tsdataset.py
--rw-r--r--   0        0        0    10234 2024-03-21 09:57:35.741574 etna-2.5.0/etna/datasets/utils.py
--rw-r--r--   0        0        0      351 2024-03-21 09:57:35.741574 etna-2.5.0/etna/distributions/__init__.py
--rw-r--r--   0        0        0     1812 2024-03-21 09:57:35.741574 etna-2.5.0/etna/distributions/distributions.py
--rw-r--r--   0        0        0      269 2024-03-21 09:57:35.741574 etna-2.5.0/etna/ensembles/__init__.py
--rw-r--r--   0        0        0     6792 2024-03-21 09:57:35.741574 etna-2.5.0/etna/ensembles/direct_ensemble.py
--rw-r--r--   0        0        0     4751 2024-03-21 09:57:35.741574 etna-2.5.0/etna/ensembles/mixins.py
--rw-r--r--   0        0        0    11884 2024-03-21 09:57:35.741574 etna-2.5.0/etna/ensembles/stacking_ensemble.py
--rw-r--r--   0        0        0     9767 2024-03-21 09:57:35.741574 etna-2.5.0/etna/ensembles/voting_ensemble.py
--rw-r--r--   0        0        0       94 2024-03-21 09:57:35.741574 etna-2.5.0/etna/experimental/change_points/__init__.py
--rw-r--r--   0        0        0     5558 2024-03-21 09:57:35.741574 etna-2.5.0/etna/experimental/change_points/regularization_search.py
--rw-r--r--   0        0        0      242 2024-03-21 09:57:35.741574 etna-2.5.0/etna/experimental/classification/__init__.py
--rw-r--r--   0        0        0      794 2024-03-21 09:57:35.741574 etna-2.5.0/etna/experimental/classification/base.py
--rw-r--r--   0        0        0     5089 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/classification.py
--rw-r--r--   0        0        0      366 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/feature_extraction/__init__.py
--rw-r--r--   0        0        0     1543 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/feature_extraction/base.py
--rw-r--r--   0        0        0     2573 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/feature_extraction/tsfresh.py
--rw-r--r--   0        0        0    15413 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/feature_extraction/weasel.py
--rw-r--r--   0        0        0     3404 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/predictability.py
--rw-r--r--   0        0        0      874 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/classification/utils.py
--rw-r--r--   0        0        0      359 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/__init__.py
--rw-r--r--   0        0        0     6728 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/base.py
--rw-r--r--   0        0        0     3556 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/conformal.py
--rw-r--r--   0        0        0     3512 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/empirical.py
--rw-r--r--   0        0        0     2455 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/mixins.py
--rw-r--r--   0        0        0     3368 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/naive_variance.py
--rw-r--r--   0        0        0     1313 2024-03-21 09:57:35.745574 etna-2.5.0/etna/experimental/prediction_intervals/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/__init__.py
--rw-r--r--   0        0        0       79 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/pmdarima_utils/__init__.py
--rw-r--r--   0        0        0     7455 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/pmdarima_utils/arima.py
--rw-r--r--   0        0        0      415 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/pmdarima_utils/arima.pyi
--rw-r--r--   0        0        0        0 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      472 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/pytorch_lightning/callbacks.py
--rw-r--r--   0        0        0       48 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/statsforecast/__init__.py
--rw-r--r--   0        0        0    20329 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/statsforecast/arima.py
--rw-r--r--   0        0        0      341 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/__init__.py
--rw-r--r--   0        0        0     1840 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/defaults.py
--rw-r--r--   0        0        0     1801 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/distribution.py
--rw-r--r--   0        0        0       69 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/distribution.pyi
--rw-r--r--   0        0        0    16549 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/relevance.py
--rw-r--r--   0        0        0      823 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/relevance.pyi
--rw-r--r--   0        0        0     8470 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/significance_tests.py
--rw-r--r--   0        0        0      344 2024-03-21 09:57:35.745574 etna-2.5.0/etna/libs/tsfresh/significance_tests.pyi
--rw-r--r--   0        0        0      805 2024-03-21 09:57:35.745574 etna-2.5.0/etna/loggers/__init__.py
--rw-r--r--   0        0        0     4993 2024-03-21 09:57:35.745574 etna-2.5.0/etna/loggers/base.py
--rw-r--r--   0        0        0     2643 2024-03-21 09:57:35.745574 etna-2.5.0/etna/loggers/console_logger.py
--rw-r--r--   0        0        0    15309 2024-03-21 09:57:35.745574 etna-2.5.0/etna/loggers/file_logger.py
--rw-r--r--   0        0        0     7853 2024-03-21 09:57:35.745574 etna-2.5.0/etna/loggers/wandb_logger.py
--rw-r--r--   0        0        0     1529 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/__init__.py
--rw-r--r--   0        0        0    10851 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/base.py
--rw-r--r--   0        0        0     8094 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/functional_metrics.py
--rw-r--r--   0        0        0     9698 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/intervals_metrics.py
--rw-r--r--   0        0        0    11173 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/metrics.py
--rw-r--r--   0        0        0     2539 2024-03-21 09:57:35.745574 etna-2.5.0/etna/metrics/utils.py
--rw-r--r--   0        0        0     3165 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/__init__.py
--rw-r--r--   0        0        0     2521 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/autoarima.py
--rw-r--r--   0        0        0    23409 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/base.py
--rw-r--r--   0        0        0    16504 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/catboost.py
--rw-r--r--   0        0        0    14515 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/deadline_ma.py
--rw-r--r--   0        0        0      557 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/decorators.py
--rw-r--r--   0        0        0    33500 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/holt_winters.py
--rw-r--r--   0        0        0     8556 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/linear.py
--rw-r--r--   0        0        0    27361 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/mixins.py
--rw-r--r--   0        0        0      828 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/moving_average.py
--rw-r--r--   0        0        0     1031 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/naive.py
--rw-r--r--   0        0        0      608 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/__init__.py
--rw-r--r--   0        0        0    10227 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepar.py
--rw-r--r--   0        0        0      125 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepar_native/__init__.py
--rw-r--r--   0        0        0    14831 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepar_native/deepar.py
--rw-r--r--   0        0        0     7276 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepar_native/loss.py
--rw-r--r--   0        0        0      561 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepstate/__init__.py
--rw-r--r--   0        0        0    13611 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepstate/deepstate.py
--rw-r--r--   0        0        0     8808 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepstate/linear_dynamic_system.py
--rw-r--r--   0        0        0    13269 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/deepstate/state_space_model.py
--rw-r--r--   0        0        0     9353 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/mlp.py
--rw-r--r--   0        0        0      189 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/nbeats/__init__.py
--rw-r--r--   0        0        0     7345 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/nbeats/blocks.py
--rw-r--r--   0        0        0     3115 2024-03-21 09:57:35.745574 etna-2.5.0/etna/models/nn/nbeats/metrics.py
--rw-r--r--   0        0        0    16147 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/nbeats/nbeats.py
--rw-r--r--   0        0        0     8706 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/nbeats/nets.py
--rw-r--r--   0        0        0     3337 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/nbeats/utils.py
--rw-r--r--   0        0        0    13402 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/patchts.py
--rw-r--r--   0        0        0    11426 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/rnn.py
--rw-r--r--   0        0        0    11676 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/tft.py
--rw-r--r--   0        0        0    13005 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/nn/utils.py
--rw-r--r--   0        0        0    22013 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/prophet.py
--rw-r--r--   0        0        0    35545 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/sarimax.py
--rw-r--r--   0        0        0     9064 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/seasonal_ma.py
--rw-r--r--   0        0        0     4963 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/sklearn.py
--rw-r--r--   0        0        0    27518 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/statsforecast.py
--rw-r--r--   0        0        0    21339 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/tbats.py
--rw-r--r--   0        0        0     3673 2024-03-21 09:57:35.749574 etna-2.5.0/etna/models/utils.py
--rw-r--r--   0        0        0      394 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/__init__.py
--rw-r--r--   0        0        0     5460 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/assembling_pipelines.py
--rw-r--r--   0        0        0     7460 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/autoregressive_pipeline.py
--rw-r--r--   0        0        0    42109 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/base.py
--rw-r--r--   0        0        0    12284 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/hierarchical_pipeline.py
--rw-r--r--   0        0        0     8523 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/mixins.py
--rw-r--r--   0        0        0     5794 2024-03-21 09:57:35.749574 etna-2.5.0/etna/pipeline/pipeline.py
--rw-r--r--   0        0        0        0 2024-03-21 09:57:35.749574 etna-2.5.0/etna/py.typed
--rw-r--r--   0        0        0      243 2024-03-21 09:57:35.749574 etna-2.5.0/etna/reconciliation/__init__.py
--rw-r--r--   0        0        0     3999 2024-03-21 09:57:35.749574 etna-2.5.0/etna/reconciliation/base.py
--rw-r--r--   0        0        0     1899 2024-03-21 09:57:35.749574 etna-2.5.0/etna/reconciliation/bottom_up.py
--rw-r--r--   0        0        0     5742 2024-03-21 09:57:35.749574 etna-2.5.0/etna/reconciliation/top_down.py
--rw-r--r--   0        0        0    11101 2024-03-21 09:57:35.749574 etna-2.5.0/etna/settings.py
--rw-r--r--   0        0        0     3496 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/__init__.py
--rw-r--r--   0        0        0    12808 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/base.py
--rw-r--r--   0        0        0     1618 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/__init__.py
--rw-r--r--   0        0        0     1549 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/__init__.py
--rw-r--r--   0        0        0     7935 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/base.py
--rw-r--r--   0        0        0      250 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
--rw-r--r--   0        0        0     1886 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
--rw-r--r--   0        0        0     2168 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
--rw-r--r--   0        0        0     5435 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/detrend.py
--rw-r--r--   0        0        0     5175 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/level.py
--rw-r--r--   0        0        0      887 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
--rw-r--r--   0        0        0      732 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
--rw-r--r--   0        0        0     1311 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
--rw-r--r--   0        0        0     3397 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
--rw-r--r--   0        0        0     2500 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
--rw-r--r--   0        0        0     5480 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/segmentation.py
--rw-r--r--   0        0        0     5799 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/change_points_based/trend.py
--rw-r--r--   0        0        0     6966 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/deseasonal.py
--rw-r--r--   0        0        0     8236 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/detrend.py
--rw-r--r--   0        0        0     8021 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/decomposition/stl.py
--rw-r--r--   0        0        0      306 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/encoders/__init__.py
--rw-r--r--   0        0        0     7512 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/encoders/categorical.py
--rw-r--r--   0        0        0     2778 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/encoders/mean_segment_encoder.py
--rw-r--r--   0        0        0     2467 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/encoders/segment_encoder.py
--rw-r--r--   0        0        0      444 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/feature_selection/__init__.py
--rw-r--r--   0        0        0     2469 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/feature_selection/base.py
--rw-r--r--   0        0        0    10388 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/feature_selection/feature_importance.py
--rw-r--r--   0        0        0     3434 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/feature_selection/filter.py
--rw-r--r--   0        0        0    15799 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/feature_selection/gale_shapley.py
--rw-r--r--   0        0        0     1437 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/math/__init__.py
--rw-r--r--   0        0        0     4098 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/math/add_constant.py
--rw-r--r--   0        0        0     4764 2024-03-21 09:57:35.749574 etna-2.5.0/etna/transforms/math/apply_lambda.py
--rw-r--r--   0        0        0    16895 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/differencing.py
--rw-r--r--   0        0        0     9918 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/lags.py
--rw-r--r--   0        0        0     4918 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/limit.py
--rw-r--r--   0        0        0     4262 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/log.py
--rw-r--r--   0        0        0     4748 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/power.py
--rw-r--r--   0        0        0    10377 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/scalers.py
--rw-r--r--   0        0        0    11663 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/sklearn.py
--rw-r--r--   0        0        0    22831 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/math/statistics.py
--rw-r--r--   0        0        0      233 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/missing_values/__init__.py
--rw-r--r--   0        0        0    11493 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/missing_values/imputation.py
--rw-r--r--   0        0        0     6738 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/missing_values/resample.py
--rw-r--r--   0        0        0      301 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/outliers/__init__.py
--rw-r--r--   0        0        0     5548 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/outliers/base.py
--rw-r--r--   0        0        0     8251 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/outliers/point_outliers.py
--rw-r--r--   0        0        0      393 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/__init__.py
--rw-r--r--   0        0        0    15689 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/date_flags.py
--rw-r--r--   0        0        0     7306 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/event.py
--rw-r--r--   0        0        0     5744 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/fourier.py
--rw-r--r--   0        0        0     7887 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/holiday.py
--rw-r--r--   0        0        0     9021 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/special_days.py
--rw-r--r--   0        0        0     9420 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/timestamp/time_flags.py
--rw-r--r--   0        0        0      746 2024-03-21 09:57:35.753574 etna-2.5.0/etna/transforms/utils.py
--rw-r--r--   0        0        0    10540 2024-03-21 09:57:35.985574 etna-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    22900 1970-01-01 00:00:00.000000 etna-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11244 2024-04-11 16:02:17.919556 etna-2.6.0/LICENSE
+-rw-r--r--   0        0        0    17384 2024-04-11 16:02:17.919556 etna-2.6.0/README.md
+-rw-r--r--   0        0        0       49 2024-04-11 16:02:17.923556 etna-2.6.0/etna/__init__.py
+-rw-r--r--   0        0        0     2676 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/decomposition/__init__.py
+-rw-r--r--   0        0        0    17465 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/decomposition/plots.py
+-rw-r--r--   0        0        0     1198 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/decomposition/search.py
+-rw-r--r--   0        0        0    10721 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/decomposition/utils.py
+-rw-r--r--   0        0        0      475 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/eda/__init__.py
+-rw-r--r--   0        0        0    27177 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/eda/plots.py
+-rw-r--r--   0        0        0     4606 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/eda/utils.py
+-rw-r--r--   0        0        0      472 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_relevance/__init__.py
+-rw-r--r--   0        0        0     6004 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_relevance/plots.py
+-rw-r--r--   0        0        0     4340 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_relevance/relevance.py
+-rw-r--r--   0        0        0     4095 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_relevance/relevance_table.py
+-rw-r--r--   0        0        0      654 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_relevance/utils.py
+-rw-r--r--   0        0        0      213 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_selection/__init__.py
+-rw-r--r--   0        0        0     5377 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/feature_selection/mrmr_selection.py
+-rw-r--r--   0        0        0      737 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/forecast/__init__.py
+-rw-r--r--   0        0        0    37002 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/forecast/plots.py
+-rw-r--r--   0        0        0     4227 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/forecast/utils.py
+-rw-r--r--   0        0        0      517 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/__init__.py
+-rw-r--r--   0        0        0     6838 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/density_outliers.py
+-rw-r--r--   0        0        0    13589 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/hist_outliers.py
+-rw-r--r--   0        0        0     2197 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/median_outliers.py
+-rw-r--r--   0        0        0     5673 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/plots.py
+-rw-r--r--   0        0        0     4420 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/outliers/prediction_interval_outliers.py
+-rw-r--r--   0        0        0     1793 2024-04-11 16:02:17.923556 etna-2.6.0/etna/analysis/utils.py
+-rw-r--r--   0        0        0     1046 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/__init__.py
+-rw-r--r--   0        0        0    32050 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/auto.py
+-rw-r--r--   0        0        0      102 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/optuna/__init__.py
+-rw-r--r--   0        0        0     4737 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/optuna/config_sampler.py
+-rw-r--r--   0        0        0     2828 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/optuna/wrapper.py
+-rw-r--r--   0        0        0       93 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/pool/__init__.py
+-rw-r--r--   0        0        0     1719 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/pool/generator.py
+-rw-r--r--   0        0        0     5348 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/pool/templates.py
+-rw-r--r--   0        0        0      495 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/pool/utils.py
+-rw-r--r--   0        0        0      217 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/runner/__init__.py
+-rw-r--r--   0        0        0      604 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/runner/base.py
+-rw-r--r--   0        0        0     2531 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/runner/local.py
+-rw-r--r--   0        0        0      171 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/runner/utils.py
+-rw-r--r--   0        0        0     1664 2024-04-11 16:02:17.923556 etna-2.6.0/etna/auto/utils.py
+-rw-r--r--   0        0        0      632 2024-04-11 16:02:17.923556 etna-2.6.0/etna/clustering/__init__.py
+-rw-r--r--   0        0        0      686 2024-04-11 16:02:17.923556 etna-2.6.0/etna/clustering/base.py
+-rw-r--r--   0        0        0      259 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/distances/__init__.py
+-rw-r--r--   0        0        0     3756 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/distances/base.py
+-rw-r--r--   0        0        0     4508 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/distances/distance_matrix.py
+-rw-r--r--   0        0        0     5597 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/distances/dtw_distance.py
+-rw-r--r--   0        0        0     1705 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/distances/euclidean_distance.py
+-rw-r--r--   0        0        0      289 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/hierarchical/__init__.py
+-rw-r--r--   0        0        0     6251 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/hierarchical/base.py
+-rw-r--r--   0        0        0     1501 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/hierarchical/dtw_clustering.py
+-rw-r--r--   0        0        0     1561 2024-04-11 16:02:17.927556 etna-2.6.0/etna/clustering/hierarchical/euclidean_clustering.py
+-rw-r--r--   0        0        0      422 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/__main__.py
+-rw-r--r--   0        0        0     5026 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/backtest_command.py
+-rw-r--r--   0        0        0     7642 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/forecast_command.py
+-rw-r--r--   0        0        0      281 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/resolvers.py
+-rw-r--r--   0        0        0     4415 2024-04-11 16:02:17.927556 etna-2.6.0/etna/commands/utils.py
+-rw-r--r--   0        0        0      257 2024-04-11 16:02:17.927556 etna-2.6.0/etna/core/__init__.py
+-rw-r--r--   0        0        0    12396 2024-04-11 16:02:17.927556 etna-2.6.0/etna/core/mixins.py
+-rw-r--r--   0        0        0      631 2024-04-11 16:02:17.927556 etna-2.6.0/etna/core/saving.py
+-rw-r--r--   0        0        0     2540 2024-04-11 16:02:17.927556 etna-2.6.0/etna/core/utils.py
+-rw-r--r--   0        0        0      860 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/__init__.py
+-rw-r--r--   0        0        0     9661 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/datasets_generation.py
+-rw-r--r--   0        0        0     7778 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/hierarchical_structure.py
+-rw-r--r--   0        0        0    41238 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/internal_datasets.py
+-rw-r--r--   0        0        0    75842 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/tsdataset.py
+-rw-r--r--   0        0        0    25502 2024-04-11 16:02:17.927556 etna-2.6.0/etna/datasets/utils.py
+-rw-r--r--   0        0        0      351 2024-04-11 16:02:17.927556 etna-2.6.0/etna/distributions/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-11 16:02:17.927556 etna-2.6.0/etna/distributions/distributions.py
+-rw-r--r--   0        0        0      269 2024-04-11 16:02:17.927556 etna-2.6.0/etna/ensembles/__init__.py
+-rw-r--r--   0        0        0     6783 2024-04-11 16:02:17.927556 etna-2.6.0/etna/ensembles/direct_ensemble.py
+-rw-r--r--   0        0        0     4802 2024-04-11 16:02:17.927556 etna-2.6.0/etna/ensembles/mixins.py
+-rw-r--r--   0        0        0    11850 2024-04-11 16:02:17.927556 etna-2.6.0/etna/ensembles/stacking_ensemble.py
+-rw-r--r--   0        0        0     9733 2024-04-11 16:02:17.927556 etna-2.6.0/etna/ensembles/voting_ensemble.py
+-rw-r--r--   0        0        0       94 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/change_points/__init__.py
+-rw-r--r--   0        0        0     5558 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/change_points/regularization_search.py
+-rw-r--r--   0        0        0      242 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/__init__.py
+-rw-r--r--   0        0        0      794 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/base.py
+-rw-r--r--   0        0        0     5089 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/classification.py
+-rw-r--r--   0        0        0      366 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/feature_extraction/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/feature_extraction/base.py
+-rw-r--r--   0        0        0     2573 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/feature_extraction/tsfresh.py
+-rw-r--r--   0        0        0    15413 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/feature_extraction/weasel.py
+-rw-r--r--   0        0        0     3404 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/predictability.py
+-rw-r--r--   0        0        0      874 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/classification/utils.py
+-rw-r--r--   0        0        0      359 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/__init__.py
+-rw-r--r--   0        0        0     6728 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/base.py
+-rw-r--r--   0        0        0     3556 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/conformal.py
+-rw-r--r--   0        0        0     3512 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/empirical.py
+-rw-r--r--   0        0        0     2455 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/mixins.py
+-rw-r--r--   0        0        0     3368 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/naive_variance.py
+-rw-r--r--   0        0        0     1313 2024-04-11 16:02:17.927556 etna-2.6.0/etna/experimental/prediction_intervals/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/pmdarima_utils/__init__.py
+-rw-r--r--   0        0        0     7455 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/pmdarima_utils/arima.py
+-rw-r--r--   0        0        0      415 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/pmdarima_utils/arima.pyi
+-rw-r--r--   0        0        0        0 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      472 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/pytorch_lightning/callbacks.py
+-rw-r--r--   0        0        0       48 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/statsforecast/__init__.py
+-rw-r--r--   0        0        0    20329 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/statsforecast/arima.py
+-rw-r--r--   0        0        0      341 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/defaults.py
+-rw-r--r--   0        0        0     1801 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/distribution.py
+-rw-r--r--   0        0        0       69 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/distribution.pyi
+-rw-r--r--   0        0        0    16549 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/relevance.py
+-rw-r--r--   0        0        0      823 2024-04-11 16:02:17.927556 etna-2.6.0/etna/libs/tsfresh/relevance.pyi
+-rw-r--r--   0        0        0     8470 2024-04-11 16:02:17.931557 etna-2.6.0/etna/libs/tsfresh/significance_tests.py
+-rw-r--r--   0        0        0      344 2024-04-11 16:02:17.931557 etna-2.6.0/etna/libs/tsfresh/significance_tests.pyi
+-rw-r--r--   0        0        0      805 2024-04-11 16:02:17.931557 etna-2.6.0/etna/loggers/__init__.py
+-rw-r--r--   0        0        0     4993 2024-04-11 16:02:17.931557 etna-2.6.0/etna/loggers/base.py
+-rw-r--r--   0        0        0     2643 2024-04-11 16:02:17.931557 etna-2.6.0/etna/loggers/console_logger.py
+-rw-r--r--   0        0        0    15309 2024-04-11 16:02:17.931557 etna-2.6.0/etna/loggers/file_logger.py
+-rw-r--r--   0        0        0     7853 2024-04-11 16:02:17.931557 etna-2.6.0/etna/loggers/wandb_logger.py
+-rw-r--r--   0        0        0     1529 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/__init__.py
+-rw-r--r--   0        0        0    10851 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/base.py
+-rw-r--r--   0        0        0     8094 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/functional_metrics.py
+-rw-r--r--   0        0        0     9698 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/intervals_metrics.py
+-rw-r--r--   0        0        0    11173 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/metrics.py
+-rw-r--r--   0        0        0     2539 2024-04-11 16:02:17.931557 etna-2.6.0/etna/metrics/utils.py
+-rw-r--r--   0        0        0     3143 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/__init__.py
+-rw-r--r--   0        0        0     2521 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/autoarima.py
+-rw-r--r--   0        0        0    23409 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/base.py
+-rw-r--r--   0        0        0    16390 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/catboost.py
+-rw-r--r--   0        0        0    14515 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/deadline_ma.py
+-rw-r--r--   0        0        0      557 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/decorators.py
+-rw-r--r--   0        0        0    34171 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/holt_winters.py
+-rw-r--r--   0        0        0     8556 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/linear.py
+-rw-r--r--   0        0        0    27361 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/mixins.py
+-rw-r--r--   0        0        0      828 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/moving_average.py
+-rw-r--r--   0        0        0     1031 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/naive.py
+-rw-r--r--   0        0        0      665 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/__init__.py
+-rw-r--r--   0        0        0    10227 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepar.py
+-rw-r--r--   0        0        0      125 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepar_native/__init__.py
+-rw-r--r--   0        0        0    14883 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepar_native/deepar.py
+-rw-r--r--   0        0        0     7276 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepar_native/loss.py
+-rw-r--r--   0        0        0      561 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepstate/__init__.py
+-rw-r--r--   0        0        0    13647 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepstate/deepstate.py
+-rw-r--r--   0        0        0     8808 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepstate/linear_dynamic_system.py
+-rw-r--r--   0        0        0    13269 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/deepstate/state_space_model.py
+-rw-r--r--   0        0        0     9319 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/mlp.py
+-rw-r--r--   0        0        0      189 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/__init__.py
+-rw-r--r--   0        0        0     7345 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/blocks.py
+-rw-r--r--   0        0        0     3115 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/metrics.py
+-rw-r--r--   0        0        0    16147 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/nbeats.py
+-rw-r--r--   0        0        0     8706 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/nets.py
+-rw-r--r--   0        0        0     3337 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/nbeats/utils.py
+-rw-r--r--   0        0        0    13441 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/patchts.py
+-rw-r--r--   0        0        0    11478 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/rnn.py
+-rw-r--r--   0        0        0    11799 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/tft.py
+-rw-r--r--   0        0        0      116 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/tft_native/__init__.py
+-rw-r--r--   0        0        0    11923 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/tft_native/layers.py
+-rw-r--r--   0        0        0    27449 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/tft_native/tft.py
+-rw-r--r--   0        0        0    13075 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/nn/utils.py
+-rw-r--r--   0        0        0    23639 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/prophet.py
+-rw-r--r--   0        0        0    35763 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/sarimax.py
+-rw-r--r--   0        0        0     9064 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/seasonal_ma.py
+-rw-r--r--   0        0        0     4963 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/sklearn.py
+-rw-r--r--   0        0        0    27526 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/statsforecast.py
+-rw-r--r--   0        0        0    21545 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/tbats.py
+-rw-r--r--   0        0        0     1746 2024-04-11 16:02:17.931557 etna-2.6.0/etna/models/utils.py
+-rw-r--r--   0        0        0      394 2024-04-11 16:02:17.931557 etna-2.6.0/etna/pipeline/__init__.py
+-rw-r--r--   0        0        0     5478 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/assembling_pipelines.py
+-rw-r--r--   0        0        0     7000 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/autoregressive_pipeline.py
+-rw-r--r--   0        0        0    46826 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/base.py
+-rw-r--r--   0        0        0    12284 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/hierarchical_pipeline.py
+-rw-r--r--   0        0        0     8650 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/mixins.py
+-rw-r--r--   0        0        0     5794 2024-04-11 16:02:17.935557 etna-2.6.0/etna/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:02:17.935557 etna-2.6.0/etna/py.typed
+-rw-r--r--   0        0        0      243 2024-04-11 16:02:17.935557 etna-2.6.0/etna/reconciliation/__init__.py
+-rw-r--r--   0        0        0     3999 2024-04-11 16:02:17.935557 etna-2.6.0/etna/reconciliation/base.py
+-rw-r--r--   0        0        0     1899 2024-04-11 16:02:17.935557 etna-2.6.0/etna/reconciliation/bottom_up.py
+-rw-r--r--   0        0        0     5742 2024-04-11 16:02:17.935557 etna-2.6.0/etna/reconciliation/top_down.py
+-rw-r--r--   0        0        0    11101 2024-04-11 16:02:17.935557 etna-2.6.0/etna/settings.py
+-rw-r--r--   0        0        0     3602 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/__init__.py
+-rw-r--r--   0        0        0    12808 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/base.py
+-rw-r--r--   0        0        0     1618 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/__init__.py
+-rw-r--r--   0        0        0     1549 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/__init__.py
+-rw-r--r--   0        0        0     7943 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/base.py
+-rw-r--r--   0        0        0      250 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/change_points_models/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py
+-rw-r--r--   0        0        0     2168 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py
+-rw-r--r--   0        0        0     5612 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/detrend.py
+-rw-r--r--   0        0        0     5175 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/level.py
+-rw-r--r--   0        0        0      887 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py
+-rw-r--r--   0        0        0     1311 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py
+-rw-r--r--   0        0        0     3397 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py
+-rw-r--r--   0        0        0     2500 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py
+-rw-r--r--   0        0        0     5480 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/segmentation.py
+-rw-r--r--   0        0        0     5799 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/change_points_based/trend.py
+-rw-r--r--   0        0        0     7268 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/deseasonal.py
+-rw-r--r--   0        0        0     8151 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/detrend.py
+-rw-r--r--   0        0        0     8982 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/decomposition/stl.py
+-rw-r--r--   0        0        0      306 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/encoders/__init__.py
+-rw-r--r--   0        0        0     7512 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/encoders/categorical.py
+-rw-r--r--   0        0        0     2778 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/encoders/mean_segment_encoder.py
+-rw-r--r--   0        0        0     2467 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/encoders/segment_encoder.py
+-rw-r--r--   0        0        0      444 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/feature_selection/__init__.py
+-rw-r--r--   0        0        0     2469 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/feature_selection/base.py
+-rw-r--r--   0        0        0    10564 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/feature_selection/feature_importance.py
+-rw-r--r--   0        0        0     3434 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/feature_selection/filter.py
+-rw-r--r--   0        0        0    15799 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/feature_selection/gale_shapley.py
+-rw-r--r--   0        0        0     1575 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/__init__.py
+-rw-r--r--   0        0        0     4098 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/add_constant.py
+-rw-r--r--   0        0        0     4764 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/apply_lambda.py
+-rw-r--r--   0        0        0     8817 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/binary_operator.py
+-rw-r--r--   0        0        0    17192 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/differencing.py
+-rw-r--r--   0        0        0    10450 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/lags.py
+-rw-r--r--   0        0        0     4918 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/limit.py
+-rw-r--r--   0        0        0     4262 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/log.py
+-rw-r--r--   0        0        0     4748 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/power.py
+-rw-r--r--   0        0        0    10377 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/scalers.py
+-rw-r--r--   0        0        0    11663 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/sklearn.py
+-rw-r--r--   0        0        0    22831 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/math/statistics.py
+-rw-r--r--   0        0        0      233 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/missing_values/__init__.py
+-rw-r--r--   0        0        0    11493 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/missing_values/imputation.py
+-rw-r--r--   0        0        0     7603 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/missing_values/resample.py
+-rw-r--r--   0        0        0      301 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/outliers/__init__.py
+-rw-r--r--   0        0        0     7027 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/outliers/base.py
+-rw-r--r--   0        0        0     8857 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/outliers/point_outliers.py
+-rw-r--r--   0        0        0      393 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/timestamp/__init__.py
+-rw-r--r--   0        0        0    17656 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/timestamp/date_flags.py
+-rw-r--r--   0        0        0     7306 2024-04-11 16:02:17.935557 etna-2.6.0/etna/transforms/timestamp/event.py
+-rw-r--r--   0        0        0    14558 2024-04-11 16:02:17.939556 etna-2.6.0/etna/transforms/timestamp/fourier.py
+-rw-r--r--   0        0        0    13622 2024-04-11 16:02:17.939556 etna-2.6.0/etna/transforms/timestamp/holiday.py
+-rw-r--r--   0        0        0    11091 2024-04-11 16:02:17.939556 etna-2.6.0/etna/transforms/timestamp/special_days.py
+-rw-r--r--   0        0        0    11271 2024-04-11 16:02:17.939556 etna-2.6.0/etna/transforms/timestamp/time_flags.py
+-rw-r--r--   0        0        0      746 2024-04-11 16:02:17.939556 etna-2.6.0/etna/transforms/utils.py
+-rw-r--r--   0        0        0    10608 2024-04-11 16:02:18.179556 etna-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23210 1970-01-01 00:00:00.000000 etna-2.6.0/PKG-INFO
```

### Comparing `etna-2.5.0/LICENSE` & `etna-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/README.md` & `etna-2.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 import pandas as pd
 from etna.datasets import TSDataset
 
 # Read the data
 df = pd.read_csv("examples/data/example_dataset.csv")
 
 # Create a TSDataset
-df = TSDataset.to_dataset(df)
 ts = TSDataset(df, freq="D")
 
 # Choose a horizon
 HORIZON = 14
 
 # Make train/test split
 train_ts, test_ts = ts.train_test_split(test_size=HORIZON)
@@ -189,17 +188,18 @@
 | [Clustering](https://github.com/etna-team/etna/tree/master/examples/206-clustering.ipynb)                                   |                 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/206-clustering.ipynb) |
 | [Feature selection](https://github.com/etna-team/etna/blob/master/examples/207-feature_selection.ipynb)                     |          [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/207-feature_selection.ipynb) |
 | [Forecasting strategies](https://github.com/etna-team/etna/tree/master/examples/208-forecasting_strategies.ipynb)           |     [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/208-forecasting_strategies.ipynb) |
 | [Mechanics of forecasting](https://github.com/etna-team/etna/blob/master/examples/209-mechanics_of_forecasting.ipynb)       |   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/209-mechanics_of_forecasting.ipynb) |
 | [Custom model and transform](https://github.com/etna-team/etna/tree/master/examples/301-custom_transform_and_model.ipynb)   | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/301-custom_transform_and_model.ipynb) |
 | [Inference: using saved pipeline on a new data](https://github.com/etna-team/etna/tree/master/examples/302-inference.ipynb) |                  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/302-inference.ipynb) |
 | [Hierarchical time series](https://github.com/etna-team/etna/blob/master/examples/303-hierarchical_pipeline.ipynb)          |      [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/303-hierarchical_pipeline.ipynb) |
-| [Forecast interpretation](https://github.com/etna-team/etna/tree/master/examples/304-forecasting_interpretation.ipynb)         |    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/304-forecasting_interpretation.ipynb) |
+| [Forecast interpretation](https://github.com/etna-team/etna/tree/master/examples/304-forecasting_interpretation.ipynb)      |    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/304-forecasting_interpretation.ipynb) |
 | [Classification](https://github.com/etna-team/etna/blob/master/examples/305-classification.ipynb)                           |             [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/305-classification.ipynb) |
 | [Prediction intervals](https://github.com/etna-team/etna/tree/master/examples/306-prediction_intervals.ipynb)               |       [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/306-prediction_intervals.ipynb) |
+| [Working with misaligned data](https://github.com/etna-team/etna/tree/master/examples/307-working_with_misaligned_data.ipynb)       |       [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/307-working_with_misaligned_data.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://docs.etna.ai/stable/).
 
 ## Community
```

#### html2text {}

```diff
@@ -12,22 +12,22 @@
 the first python open source framework of [Tinkoff.ru](https://www.tinkoff.ru/
 eng/) Artificial Intelligence Center. The library started as an internal
 product in our company - we use it in over 10+ projects now, so we often
 release updates. Contributions are welcome - check our [Contribution Guide]
 (https://github.com/etna-team/etna/blob/master/CONTRIBUTING.md). ## Quickstart
 Let's load and prepare the data. ```python import pandas as pd from
 etna.datasets import TSDataset # Read the data df = pd.read_csv("examples/data/
-example_dataset.csv") # Create a TSDataset df = TSDataset.to_dataset(df) ts =
-TSDataset(df, freq="D") # Choose a horizon HORIZON = 14 # Make train/test split
-train_ts, test_ts = ts.train_test_split(test_size=HORIZON) ``` Define
-transformations and model: ```python from etna.models import
-CatBoostMultiSegmentModel from etna.transforms import DateFlagsTransform from
-etna.transforms import DensityOutliersTransform from etna.transforms import
-FourierTransform from etna.transforms import LagTransform from etna.transforms
-import LinearTrendTransform from etna.transforms import MeanTransform from
+example_dataset.csv") # Create a TSDataset ts = TSDataset(df, freq="D") #
+Choose a horizon HORIZON = 14 # Make train/test split train_ts, test_ts =
+ts.train_test_split(test_size=HORIZON) ``` Define transformations and model:
+```python from etna.models import CatBoostMultiSegmentModel from
+etna.transforms import DateFlagsTransform from etna.transforms import
+DensityOutliersTransform from etna.transforms import FourierTransform from
+etna.transforms import LagTransform from etna.transforms import
+LinearTrendTransform from etna.transforms import MeanTransform from
 etna.transforms import SegmentEncoderTransform from etna.transforms import
 TimeSeriesImputerTransform from etna.transforms import TrendTransform # Prepare
 transforms transforms = [ DensityOutliersTransform(in_column="target",
 distance_coef=3.0), TimeSeriesImputerTransform(in_column="target",
 strategy="forward_fill"), LinearTrendTransform(in_column="target"),
 TrendTransform(in_column="target", out_column="trend"), LagTransform
 (in_column="target", lags=list(range(HORIZON, 122)), out_column="target_lag"),
@@ -132,19 +132,23 @@
 team/etna/master?filepath=examples/304-forecasting_interpretation.ipynb) | |
 [Classification](https://github.com/etna-team/etna/blob/master/examples/305-
 classification.ipynb) | [![Binder](https://mybinder.org/badge_logo.svg)](https:
 //mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/305-
 classification.ipynb) | | [Prediction intervals](https://github.com/etna-team/
 etna/tree/master/examples/306-prediction_intervals.ipynb) | [![Binder](https://
 mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/
-master?filepath=examples/306-prediction_intervals.ipynb) | ## Documentation
-ETNA documentation is available [here](https://docs.etna.ai/stable/). ##
-Community To ask the questions or discuss the library you can join our
-[telegram chat](https://t.me/etna_support). ## Resources - [Forecasting using
-ETNA library | 60 lines Catboost](https://www.kaggle.com/code/goolmonika/
+master?filepath=examples/306-prediction_intervals.ipynb) | | [Working with
+misaligned data](https://github.com/etna-team/etna/tree/master/examples/307-
+working_with_misaligned_data.ipynb) | [![Binder](https://mybinder.org/
+badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/
+master?filepath=examples/307-working_with_misaligned_data.ipynb) | ##
+Documentation ETNA documentation is available [here](https://docs.etna.ai/
+stable/). ## Community To ask the questions or discuss the library you can join
+our [telegram chat](https://t.me/etna_support). ## Resources - [Forecasting
+using ETNA library | 60 lines Catboost](https://www.kaggle.com/code/goolmonika/
 forecasting-using-etna-library-60-lines-catboost) on Kaggle -
 [ÐÑÐ¸ÐºÐ»Ð°Ð´Ð½ÑÐµ Ð·Ð°Ð´Ð°ÑÐ¸ Ð°Ð½Ð°Ð»Ð¸Ð·Ð° Ð´Ð°Ð½Ð½ÑÑ, Ð»ÐµÐºÑÐ¸Ñ 8
 â ÐÑÐµÐ¼ÐµÐ½Ð½ÑÐµ ÑÑÐ´Ñ 2](https://youtu.be/1gXVbidDZck) on YouTube -
 [Time Series Forecasting Strategies in ETNA](https://medium.com/its-tinkoff/
 time-series-forecasting-strategies-in-etna-93d7d2f8a911) on Medium - [ETNA:
 Time Series Analysis. What, why and how?](https://medium.com/its-tinkoff/etna-
 time-series-analysis-what-why-and-how-e45557af4f6c) on Medium - [ETNA Meetup
```

### Comparing `etna-2.5.0/etna/analysis/__init__.py` & `etna-2.6.0/etna/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/decomposition/__init__.py` & `etna-2.6.0/etna/analysis/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/decomposition/plots.py` & `etna-2.6.0/etna/analysis/decomposition/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from copy import deepcopy
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
+from typing import Type
 from typing import Union
+from typing import cast
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from ruptures.base import BaseCost
 from ruptures.base import BaseEstimator
 from ruptures.exceptions import BadSegmentationParameters
@@ -80,20 +82,20 @@
         ax[i].set_title(segment)
         ax[i].tick_params("x", rotation=45)
         ax[i].legend()
 
 
 def plot_time_series_with_change_points(
     ts: "TSDataset",
-    change_points: Dict[str, List[pd.Timestamp]],
+    change_points: Dict[str, List[Union[pd.Timestamp, int]]],
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
 ):
     """Plot segments with their trend change points.
 
     Parameters
     ----------
     ts:
         TSDataset with timeseries
@@ -106,14 +108,19 @@
         number of subplots columns
     figsize:
         size of the figure per subplot with one segment in inches
     start:
         start timestamp for plot
     end:
         end timestamp for plot
+
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
     """
     start, end = _get_borders_ts(ts, start, end)
 
     if segments is None:
         segments = sorted(ts.segments)
 
     _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
@@ -143,25 +150,25 @@
 
         ax[i].set_title(segment)
         ax[i].tick_params("x", rotation=45)
 
 
 def plot_change_points_interactive(
     ts,
-    change_point_model: BaseEstimator,
-    model: BaseCost,
+    change_point_model: Type[BaseEstimator],
+    model: Union[str, BaseCost],
     params_bounds: Dict[str, Tuple[Union[int, float], Union[int, float], Union[int, float]]],
     model_params: List[str],
     predict_params: List[str],
     in_column: str = "target",
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
 ):
     """Plot a time series with indicated change points.
 
     Change points are obtained using the specified method. The method parameters values
     can be changed using the corresponding sliders.
 
     Parameters
@@ -192,30 +199,36 @@
         end timestamp for plot
 
     Notes
     -----
     Jupyter notebook might display the results incorrectly,
     in this case try to use ``!jupyter nbextension enable --py widgetsnbextension``.
 
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
+
     Examples
     --------
     >>> from etna.datasets import TSDataset
     >>> from etna.datasets import generate_ar_df
     >>> from etna.analysis import plot_change_points_interactive
     >>> from ruptures.detection import Binseg
-    >>> classic_df = generate_ar_df(periods=1000, start_time="2021-08-01", n_segments=2)
-    >>> df = TSDataset.to_dataset(classic_df)
+    >>> df = generate_ar_df(periods=1000, start_time="2021-08-01", n_segments=2)
     >>> ts = TSDataset(df, "D")
     >>> params_bounds = {"n_bkps": [0, 5, 1], "min_size":[1,10,3]}
     >>> plot_change_points_interactive(ts=ts, change_point_model=Binseg, model="l2", params_bounds=params_bounds, model_params=["min_size"], predict_params=["n_bkps"], figsize=(20, 10)) # doctest: +SKIP
     """
     from ipywidgets import FloatSlider
     from ipywidgets import IntSlider
     from ipywidgets import interact
 
+    start, end = _get_borders_ts(ts, start, end)
+
     if segments is None:
         segments = sorted(ts.segments)
 
     cache = {}
 
     sliders = dict()
     style = {"description_width": "initial"}
@@ -325,15 +338,15 @@
     figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
     fig = plt.figure(figsize=figsize, constrained_layout=True)
     subfigs = fig.subfigures(rows_num, columns_num, squeeze=False)
 
     df = ts.to_pandas()
     for i, segment in enumerate(segments):
         segment_df = df.loc[:, pd.IndexSlice[segment, :]][segment]
-        segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+        segment_df = segment_df.loc[segment_df.first_valid_index() : segment_df.last_valid_index()]
         decompose_result = STL(endog=segment_df[in_column], period=period, **stl_kwargs).fit()
 
         # start plotting
         subfigs.flat[i].suptitle(segment)
         axs = subfigs.flat[i].subplots(4, 1, sharex=True)
 
         # plot observed
@@ -356,15 +369,15 @@
         axs.flat[3].set_ylabel("Residual")
         axs.flat[3].tick_params("x", rotation=45)
         axs.flat[3].grid()
 
 
 def seasonal_plot(
     ts: "TSDataset",
-    freq: Optional[str] = None,
+    freq: Union[Optional[str], Literal["not_given"]] = "not_given",
     cycle: Union[
         Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
     ] = "year",
     alignment: Union[Literal["first"], Literal["last"]] = "last",
     aggregation: Union[Literal["sum"], Literal["mean"]] = "sum",
     in_column: str = "target",
     plot_params: Optional[Dict[str, Any]] = None,
@@ -382,14 +395,15 @@
     freq:
         frequency to analyze seasons:
 
         * if isn't set, the frequency of ``ts`` will be used;
 
         * if set, resampling will be made using ``aggregation`` parameter.
           If given frequency is too low, then the frequency of ``ts`` will be used.
+          This option isn't supported for data with integer timestamp.
 
     cycle:
         period of seasonality to capture (see :class:`~etna.analysis.decomposition.utils.SeasonalPlotCycle`)
     alignment:
         how to align dataframe in case of integer cycle (see :py:class:`~etna.analysis.decomposition.utils.SeasonalPlotAlignment`)
     aggregation:
         how to aggregate values during resampling (see :py:class:`~etna.analysis.decomposition.utils.SeasonalPlotAggregation`)
@@ -402,19 +416,29 @@
         dictionary with parameters for plotting, :py:meth:`matplotlib.axes.Axes.plot` is used
     segments:
         segments to use
     columns_num:
         number of columns in subplots
     figsize:
         size of the figure per subplot with one segment in inches
+
+    Raises
+    ------
+    ValueError:
+        Resampling isn't supported for data with integer timestamp
+    ValueError:
+        Setting non-integer cycle isn't supported for data with integer timestamp
+    ValueError:
+        Value None for freq parameter isn't supported for data with datetime timestamp
     """
     if plot_params is None:
         plot_params = {}
-    if freq is None:
+    if freq == "not_given":
         freq = ts.freq
+        freq = cast(Optional[str], freq)
     if segments is None:
         segments = sorted(ts.segments)
 
     df = _prepare_seasonal_plot_df(
         ts=ts,
         freq=freq,
         cycle=cycle,
```

### Comparing `etna-2.5.0/etna/analysis/decomposition/search.py` & `etna-2.6.0/etna/analysis/decomposition/search.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Dict
 from typing import List
+from typing import Union
 
 import pandas as pd
 from ruptures.base import BaseEstimator
 
 from etna.datasets import TSDataset
 
 
 def find_change_points(
     ts: TSDataset, in_column: str, change_point_model: BaseEstimator, **model_predict_params
-) -> Dict[str, List[pd.Timestamp]]:
+) -> Dict[str, List[Union[int, pd.Timestamp]]]:
     """Find trend change points using ruptures models.
 
     Parameters
     ----------
     ts:
         dataset to work with
     in_column:
```

### Comparing `etna-2.5.0/etna/analysis/decomposition/utils.py` & `etna-2.6.0/etna/analysis/decomposition/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from enum import Enum
 from typing import TYPE_CHECKING
 from typing import Callable
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Tuple
 from typing import Union
+from typing import cast
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Literal
+from typing_extensions import assert_never
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 def _get_labels_names(trend_transform, segments):
     """If only unique transform classes are used then show their short names (without parameters). Otherwise show their full repr as label."""
@@ -141,15 +144,15 @@
 
 def _get_seasonal_in_cycle_num(
     timestamp: pd.Series,
     cycle_name: pd.Series,
     cycle: Union[
         Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
     ],
-    freq: str,
+    freq: Optional[str],
 ) -> pd.Series:
     """Get number for each point within cycle in a series of timestamps."""
     cycle_functions: Dict[Tuple[SeasonalPlotCycle, str], Callable[[pd.Series], pd.Series]] = {
         (SeasonalPlotCycle.hour, "T"): lambda x: x.dt.minute,
         (SeasonalPlotCycle.day, "H"): lambda x: x.dt.hour,
         (SeasonalPlotCycle.week, "D"): lambda x: x.dt.weekday,
         (SeasonalPlotCycle.month, "D"): lambda x: x.dt.day,
@@ -160,14 +163,15 @@
         (SeasonalPlotCycle.year, "M"): lambda x: x.dt.month,
         (SeasonalPlotCycle.year, "MS"): lambda x: x.dt.month,
     }
 
     if isinstance(cycle, int):
         pass
     else:
+        freq = cast(str, freq)
         key = (SeasonalPlotCycle(cycle), freq)
         if key in cycle_functions:
             return cycle_functions[key](timestamp)
 
     # in all other cases we can use numbers within each group
     cycle_df = pd.DataFrame({"timestamp": timestamp.tolist(), "cycle_name": cycle_name.tolist()})
     return cycle_df.sort_values("timestamp").groupby("cycle_name").cumcount()
@@ -175,33 +179,35 @@
 
 def _get_seasonal_in_cycle_name(
     timestamp: pd.Series,
     in_cycle_num: pd.Series,
     cycle: Union[
         Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
     ],
-    freq: str,
+    freq: Optional[str],
 ) -> pd.Series:
     """Get unique name for each point within the cycle in a series of timestamps."""
     if isinstance(cycle, int):
         pass
     elif SeasonalPlotCycle(cycle) == SeasonalPlotCycle.week:
+        freq = cast(str, freq)
         if freq == "D":
             return timestamp.dt.strftime("%a")
     elif SeasonalPlotCycle(cycle) == SeasonalPlotCycle.year:
+        freq = cast(str, freq)
         if freq == "M" or freq == "MS":
             return timestamp.dt.strftime("%b")
 
     # in all other cases we can use numbers from cycle_num
     return in_cycle_num.astype(str)
 
 
 def _seasonal_split(
     timestamp: pd.Series,
-    freq: str,
+    freq: Optional[str],
     cycle: Union[
         Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
     ],
 ) -> pd.DataFrame:
     """Create a seasonal split into cycles of a given timestamp.
 
     Parameters
@@ -242,42 +248,58 @@
     )
     df = TSDataset.to_dataset(df_flat)
     return df
 
 
 def _prepare_seasonal_plot_df(
     ts: "TSDataset",
-    freq: str,
+    freq: Optional[str],
     cycle: Union[
         Literal["hour"], Literal["day"], Literal["week"], Literal["month"], Literal["quarter"], Literal["year"], int
     ],
     alignment: Union[Literal["first"], Literal["last"]],
     aggregation: Union[Literal["sum"], Literal["mean"]],
     in_column: str,
     segments: List[str],
 ):
+    from etna.datasets.utils import timestamp_range
+
     # for simplicity we will rename our column to target
     df = ts.to_pandas().loc[:, pd.IndexSlice[segments, in_column]]
     df.rename(columns={in_column: "target"}, inplace=True)
 
     # remove timestamps with only nans, it is possible if in_column != "target"
     df = df[(~df.isna()).sum(axis=1) > 0]
 
     # make resampling if necessary
     if ts.freq != freq:
+        if ts.freq is None:
+            raise ValueError("Resampling isn't supported for data with integer timestamp!")
+        elif freq is None:
+            raise ValueError("Value None for freq parameter isn't supported for data with datetime timestamp!")
+
         df = _resample(df=df, freq=freq, aggregation=aggregation)
 
     # process alignment
     if isinstance(cycle, int):
         timestamp = df.index
         num_to_add = -len(timestamp) % cycle
-        # if we want align by the first value, then we should append NaNs to timestamp
-        to_add_index = None
-        if SeasonalPlotAlignment(alignment) == SeasonalPlotAlignment.first:
-            to_add_index = pd.date_range(start=timestamp.max(), periods=num_to_add + 1, closed="right", freq=freq)
+
+        alignment_enum = SeasonalPlotAlignment(alignment)
+        # if we want to align by the first value, then we should append NaNs to timestamp
+        if alignment_enum is SeasonalPlotAlignment.first:
+            to_add_index = timestamp_range(start=timestamp[-1], periods=num_to_add + 1, freq=freq)[1:]
         # if we want to align by the last value, then we should prepend NaNs to timestamp
-        elif SeasonalPlotAlignment(alignment) == SeasonalPlotAlignment.last:
-            to_add_index = pd.date_range(end=timestamp.min(), periods=num_to_add + 1, closed="left", freq=freq)
+        elif alignment_enum is SeasonalPlotAlignment.last:
+            to_add_index = timestamp_range(end=timestamp[0], periods=num_to_add + 1, freq=freq)[:-1]
+        else:
+            assert_never(alignment_enum)
+
+        new_index = df.index.append(to_add_index)
+        index_name = df.index.name
+        df = df.reindex(new_index)
+        df.index.name = index_name
 
-        df = pd.concat((df, pd.DataFrame(None, index=to_add_index))).sort_index()
+    elif freq is None:
+        raise ValueError("Setting non-integer cycle isn't supported for data with integer timestamp!")
 
     return df
```

### Comparing `etna-2.5.0/etna/analysis/eda/plots.py` & `etna-2.6.0/etna/analysis/eda/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     df = ts.to_pandas()
 
     # plot periodograms
     if amplitude_aggregation_mode == "per-segment":
         _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
         for i, segment in enumerate(segments):
             segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
-            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+            segment_df = segment_df.loc[segment_df.first_valid_index() : segment_df.last_valid_index()]
             if segment_df.isna().any():
                 raise ValueError(f"Periodogram can't be calculated on segment with NaNs inside: {segment}")
             frequencies, spectrum = periodogram(x=segment_df, fs=period, **periodogram_params)
             spectrum = spectrum[frequencies >= 1]
             frequencies = frequencies[frequencies >= 1]
             ax[i].step(frequencies, spectrum)
             ax[i].set_xscale("log")
@@ -229,26 +229,26 @@
                 ax[i].set_xticks(ticks=xticks, labels=xticks)
             ax[i].set_title(f"Periodogram: {segment}")
     else:
         # find length of each segment
         lengths_segments = []
         for segment in segments:
             segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
-            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+            segment_df = segment_df.loc[segment_df.first_valid_index() : segment_df.last_valid_index()]
             if segment_df.isna().any():
                 raise ValueError(f"Periodogram can't be calculated on segment with NaNs inside: {segment}")
             lengths_segments.append(len(segment_df))
         cut_length = min(lengths_segments)
 
         # cut each segment to `cut_length` last elements and find periodogram for each segment
         frequencies_segments = []
         spectrums_segments = []
         for segment in segments:
             segment_df = df.loc[:, pd.IndexSlice[segment, "target"]]
-            segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()][-cut_length:]
+            segment_df = segment_df.loc[segment_df.first_valid_index() : segment_df.last_valid_index()][-cut_length:]
             frequencies, spectrum = periodogram(x=segment_df, fs=period, **periodogram_params)
             frequencies_segments.append(frequencies)
             spectrums_segments.append(spectrum)
 
         frequencies = frequencies_segments[0]
         amplitude_aggregation_fn = AGGREGATION_FN[AggregationMode(amplitude_aggregation_mode)]
         spectrum = amplitude_aggregation_fn(spectrums_segments, axis=0)  # type: ignore
@@ -267,16 +267,16 @@
 
 def plot_holidays(
     ts: "TSDataset",
     holidays: Union[str, pd.DataFrame],
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
     as_is: bool = False,
 ):
     """Plot holidays for segments.
 
     Sequence of timestamps with one holiday is drawn as a colored region.
     Individual holiday is drawn like a colored point.
 
@@ -288,38 +288,45 @@
     ts:
         TSDataset with timeseries data
     holidays:
         there are several options:
 
         * if str, then this is code of the country in `holidays <https://pypi.org/project/holidays/>`_ library;
 
-        * if DataFrame, then dataframe is expected to be in prophet`s holiday format;
+        * if DataFrame and ``as_is == False``, then dataframe is expected to be in prophet`s holiday format;
+
+        * if DataFrame and ``as_is == True``, then dataframe is expected to be
+          in a format with a timestamp index and holiday names columns.
+          In a holiday column values 0 represent absence of holiday in that timestamp, 1 represent the presence.
 
     segments:
         segments to use
     columns_num:
         number of columns in subplots
     figsize:
         size of the figure per subplot with one segment in inches
     as_is:
-        Use this option if DataFrame is represented as a dataframe with a timestamp index and holiday names columns.
-        In a holiday column values 0 represent absence of holiday in that timestamp, 1 represent the presence.
+        See ``holidays`` parameter
     start:
         start timestamp for plot
     end:
         end timestamp for plot
 
     Raises
     ------
     ValueError:
-        Holiday nor ``pd.DataFrame`` or ``str``.
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
+    ValueError:
+        If ``holidays`` nor ``pd.DataFrame`` or ``str``.
     ValueError:
         Holiday is an empty ``pd.DataFrame``.
     ValueError:
         If ``as_is=True`` while holiday is string.
+    ValueError
+        If ``holiday`` is ``str`` and data has integer timestamp
     ValueError:
         If ``upper_window`` is negative.
     ValueError:
         If ``lower_window`` is positive.
     """
     start, end = _get_borders_ts(ts, start, end)
 
@@ -330,15 +337,15 @@
 
     _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
 
     df = ts.to_pandas()
 
     for i, segment in enumerate(segments):
         segment_df = df.loc[start:end, pd.IndexSlice[segment, "target"]]  # type: ignore
-        segment_df = segment_df[segment_df.first_valid_index() : segment_df.last_valid_index()]
+        segment_df = segment_df.loc[segment_df.first_valid_index() : segment_df.last_valid_index()]
 
         # plot target on segment
         target_plot = ax[i].plot(segment_df.index, segment_df)
         target_color = target_plot[0].get_color()
 
         # plot holidays on segment
         # remember color of each holiday to reuse it
@@ -590,15 +597,15 @@
 
 def distribution_plot(
     ts: "TSDataset",
     n_segments: int = 10,
     segments: Optional[List[str]] = None,
     shift: int = 30,
     window: int = 30,
-    freq: str = "1M",
+    freq: Optional[Union[str, int]] = None,
     n_rows: int = 10,
     figsize: Tuple[int, int] = (10, 5),
 ):
     """Distribution of z-values grouped by segments and time frequency.
 
     Mean is calculated by the windows:
 
@@ -616,15 +623,22 @@
     segments:
         segments to plot
     shift:
         number of timeseries shifts for statistics calc
     window:
         number of points for statistics calc
     freq:
-        group for z-values
+        how z-values should be grouped:
+
+        * frequency string for data with datetime timestamp, groups are formed by a given frequency,
+          default value is "1M"
+
+        * integer for data with integer timestamp, groups are formed by ``timestamp // freq``,
+          default value is ``ts.index.max() + 1``
+
     n_rows:
         maximum number of rows to plot
     figsize:
         size of the figure per subplot with one segment in inches
     """
     df_pd = ts.to_pandas(flatten=True)
 
@@ -636,15 +650,24 @@
     df_full.loc[:, "mean"] = (
         df_full.groupby("segment").target.shift(shift).transform(lambda s: s.rolling(window).mean())
     )
     df_full.loc[:, "std"] = df_full.groupby("segment").target.shift(shift).transform(lambda s: s.rolling(window).std())
     df_full = df_full.dropna()
     df_full.loc[:, "z"] = (df_full["target"] - df_full["mean"]) / df_full["std"]
 
-    grouped_data = df_full.groupby([df_full.timestamp.dt.to_period(freq)])
+    if ts.freq is None:
+        # make only one group
+        if freq is None:
+            freq = ts.index.max() + 1
+        grouped_data = df_full.groupby(df_full.timestamp // freq)
+    else:
+        if freq is None:
+            freq = "1M"
+        grouped_data = df_full.groupby(df_full.timestamp.dt.to_period(freq))
+
     columns_num = min(2, len(grouped_data))
     rows_num = min(n_rows, math.ceil(len(grouped_data) / columns_num))
     groups = set(list(grouped_data.groups.keys())[-rows_num * columns_num :])
 
     figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
     fig, ax = plt.subplots(rows_num, columns_num, figsize=figsize, constrained_layout=True, squeeze=False)
     fig.suptitle(f"Z statistic shift: {shift} window: {window}", fontsize=16)
@@ -661,16 +684,16 @@
 
 def plot_imputation(
     ts: "TSDataset",
     imputer: "TimeSeriesImputerTransform",
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
 ):
     """Plot the result of imputation by a given imputer.
 
     Parameters
     ----------
     ts:
         TSDataset with timeseries data
@@ -682,14 +705,19 @@
         number of columns in subplots
     figsize:
         size of the figure per subplot with one segment in inches
     start:
         start timestamp for plot
     end:
         end timestamp for plot
+
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
     """
     start, end = _get_borders_ts(ts, start, end)
 
     if segments is None:
         segments = sorted(ts.segments)
 
     _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
```

### Comparing `etna-2.5.0/etna/analysis/eda/utils.py` & `etna-2.6.0/etna/analysis/eda/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -50,22 +50,24 @@
         columns = list(set(ts.df.columns.get_level_values("feature")))
 
     correlation_matrix = ts[:, segments, columns].corr(method=method).values
     return correlation_matrix
 
 
 @singledispatch
-def _create_holidays_df(holidays, index: pd.core.indexes.datetimes.DatetimeIndex, as_is: bool) -> pd.DataFrame:
+def _create_holidays_df(holidays, index: pd.Index, as_is: bool) -> pd.DataFrame:
     raise ValueError("Parameter holidays is expected as str or pd.DataFrame")
 
 
 @_create_holidays_df.register
-def _create_holidays_df_str(holidays: str, index, as_is):
+def _create_holidays_df_str(holidays: str, index: pd.Index, as_is: bool):
     if as_is:
-        raise ValueError("Parameter `as_is` should be used with `holiday`: pd.DataFrame, not string.")
+        raise ValueError("Parameter `as_is` should be used with `holidays`: pd.DataFrame, not string.")
+    if pd.api.types.is_integer_dtype(index.dtype):
+        raise ValueError("Parameter `holidays` should be pd.DataFrame for data with integer timestamp!")
     timestamp = index.tolist()
     country_holidays = holidays_lib.country_holidays(country=holidays)
     holiday_names = {country_holidays.get(timestamp_value) for timestamp_value in timestamp}
     holiday_names = holiday_names.difference({None})
 
     holidays_dict = {}
     for holiday_name in holiday_names:
@@ -76,42 +78,53 @@
 
     holidays_df = pd.DataFrame(holidays_dict)
     holidays_df.index = timestamp
     return holidays_df
 
 
 @_create_holidays_df.register
-def _create_holidays_df_dataframe(holidays: pd.DataFrame, index, as_is):
+def _create_holidays_df_dataframe(holidays: pd.DataFrame, index: pd.Index, as_is: bool):
     if holidays.empty:
         raise ValueError("Got empty `holiday` pd.DataFrame.")
 
     if as_is:
         holidays_df = pd.DataFrame(index=index, columns=holidays.columns, data=False)
         dt = holidays_df.index.intersection(holidays.index)
         holidays_df.loc[dt, :] = holidays.loc[dt, :]
         return holidays_df
 
     holidays_df = pd.DataFrame(index=index, columns=holidays["holiday"].unique(), data=False)
     for name in holidays["holiday"].unique():
-        freq = pd.infer_freq(index)
         ds = holidays[holidays["holiday"] == name]["ds"]
         dt = [ds]
         if "upper_window" in holidays.columns:
             periods = holidays[holidays["holiday"] == name]["upper_window"].fillna(0).tolist()[0]
             if periods < 0:
                 raise ValueError("Upper windows should be non-negative.")
-            ds_upper_bound = pd.timedelta_range(start=0, periods=periods + 1, freq=freq)
+
+            if pd.api.types.is_integer_dtype(index.dtype):
+                ds_upper_bound = np.arange(periods + 1)
+            else:
+                freq = pd.infer_freq(index)
+                ds_upper_bound = pd.timedelta_range(start=0, periods=periods + 1, freq=freq)
+
             for bound in ds_upper_bound:
                 ds_add = ds + bound
                 dt.append(ds_add)
         if "lower_window" in holidays.columns:
             periods = holidays[holidays["holiday"] == name]["lower_window"].fillna(0).tolist()[0]
             if periods > 0:
                 raise ValueError("Lower windows should be non-positive.")
-            ds_lower_bound = pd.timedelta_range(start=0, periods=abs(periods) + 1, freq=freq)
+
+            if pd.api.types.is_integer_dtype(index.dtype):
+                ds_lower_bound = np.arange(abs(periods) + 1)
+            else:
+                freq = pd.infer_freq(index)
+                ds_lower_bound = pd.timedelta_range(start=0, periods=abs(periods) + 1, freq=freq)
+
             for bound in ds_lower_bound:
                 ds_add = ds - bound
                 dt.append(ds_add)
         dt = pd.concat(dt)
         dt = holidays_df.index.intersection(dt)
         holidays_df.loc[dt, name] = True
     return holidays_df
```

### Comparing `etna-2.5.0/etna/analysis/feature_relevance/plots.py` & `etna-2.6.0/etna/analysis/feature_relevance/plots.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/feature_relevance/relevance.py` & `etna-2.6.0/etna/analysis/feature_relevance/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/feature_relevance/relevance_table.py` & `etna-2.6.0/etna/analysis/feature_relevance/relevance_table.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/feature_relevance/utils.py` & `etna-2.6.0/etna/analysis/feature_relevance/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/feature_selection/mrmr_selection.py` & `etna-2.6.0/etna/analysis/feature_selection/mrmr_selection.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/forecast/__init__.py` & `etna-2.6.0/etna/analysis/forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/forecast/plots.py` & `etna-2.6.0/etna/analysis/forecast/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from etna.analysis.forecast.utils import _prepare_forecast_results
 from etna.analysis.forecast.utils import _select_prediction_intervals_names
 from etna.analysis.forecast.utils import _validate_intersecting_segments
 from etna.analysis.forecast.utils import get_residuals
 from etna.analysis.utils import _prepare_axes
 from etna.datasets.utils import match_target_components
+from etna.datasets.utils import timestamp_range
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
     from etna.transforms import Transform
 
 
 def _get_borders_comparator(segment_borders: pd.DataFrame) -> Callable[[str, str], int]:
@@ -138,15 +139,15 @@
             segment_test_df = test_ts[:, segment, :][segment]
         else:
             segment_test_df = pd.DataFrame(columns=["timestamp", "target", "segment"])
 
         if n_train_samples is None:
             plot_df = segment_train_df
         elif n_train_samples != 0:
-            plot_df = segment_train_df[-n_train_samples:]
+            plot_df = segment_train_df.iloc[-n_train_samples:]
         else:
             plot_df = pd.DataFrame(columns=["timestamp", "target", "segment"])
 
         if (train_ts is not None) and (n_train_samples != 0):
             ax[i].plot(plot_df.index.values, plot_df.target.values, label="train")
         if test_ts is not None:
             ax[i].plot(segment_test_df.index.values, segment_test_df.target.values, color="purple", label="test")
@@ -300,26 +301,26 @@
         else:
             plot_df = segment_backtest_df
         ax[i].plot(plot_df.index, plot_df.target, color=lines_colors["history"])
 
         for fold_number in folds:
             start_fold = fold_numbers[fold_numbers == fold_number].index.min()
             end_fold = fold_numbers[fold_numbers == fold_number].index.max()
-            end_fold_exclusive = pd.date_range(start=end_fold, periods=2, freq=ts.freq)[1]
+            end_fold_exclusive = timestamp_range(start=end_fold, periods=2, freq=ts.freq)[-1]
 
             # draw test
-            backtest_df_slice_fold = segment_backtest_df[start_fold:end_fold_exclusive]
+            backtest_df_slice_fold = segment_backtest_df.loc[start_fold:end_fold_exclusive]
             ax[i].plot(backtest_df_slice_fold.index, backtest_df_slice_fold.target, color=lines_colors["test"])
 
             if draw_only_lines:
                 # draw forecast
-                forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold_exclusive]
+                forecast_df_slice_fold = segment_forecast_df.loc[start_fold:end_fold_exclusive]
                 ax[i].plot(forecast_df_slice_fold.index, forecast_df_slice_fold.target, color=lines_colors["forecast"])
             else:
-                forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold]
+                forecast_df_slice_fold = segment_forecast_df.loc[start_fold:end_fold]
                 backtest_df_slice_fold = backtest_df_slice_fold.loc[forecast_df_slice_fold.index]
 
                 # draw points on test
                 ax[i].scatter(backtest_df_slice_fold.index, backtest_df_slice_fold.target, color=lines_colors["test"])
 
                 # draw forecast
                 ax[i].scatter(
@@ -426,18 +427,18 @@
                 line=dict(width=2, dash="dash"),
             )
         )
 
         for fold_number in folds:
             start_fold = fold_numbers[fold_numbers == fold_number].index.min()
             end_fold = fold_numbers[fold_numbers == fold_number].index.max()
-            end_fold_exclusive = pd.date_range(start=end_fold, periods=2, freq=ts.freq)[1]
+            end_fold_exclusive = timestamp_range(start=end_fold, periods=2, freq=ts.freq)[-1]
 
             # draw test
-            backtest_df_slice_fold = segment_backtest_df[start_fold:end_fold_exclusive]
+            backtest_df_slice_fold = segment_backtest_df.loc[start_fold:end_fold_exclusive]
             fig.add_trace(
                 go.Scattergl(
                     x=backtest_df_slice_fold.index,
                     y=backtest_df_slice_fold.target,
                     legendgroup=f"{segment}",
                     name=f"Test: {segment}",
                     mode="lines",
@@ -445,29 +446,29 @@
                     showlegend=False,
                     line=dict(width=2, dash="solid"),
                 )
             )
 
             if draw_only_lines:
                 # draw forecast
-                forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold_exclusive]
+                forecast_df_slice_fold = segment_forecast_df.loc[start_fold:end_fold_exclusive]
                 fig.add_trace(
                     go.Scattergl(
                         x=forecast_df_slice_fold.index,
                         y=forecast_df_slice_fold.target,
                         legendgroup=f"{segment}",
                         name=f"Forecast: {segment}",
                         mode="lines",
                         marker_color=colors[i % len(colors)],
                         showlegend=False,
                         line=dict(width=2, dash="dot"),
                     )
                 )
             else:
-                forecast_df_slice_fold = segment_forecast_df[start_fold:end_fold]
+                forecast_df_slice_fold = segment_forecast_df.loc[start_fold:end_fold]
                 backtest_df_slice_fold = backtest_df_slice_fold.loc[forecast_df_slice_fold.index]
 
                 # draw points on test
                 fig.add_trace(
                     go.Scattergl(
                         x=backtest_df_slice_fold.index,
                         y=backtest_df_slice_fold.target,
```

### Comparing `etna-2.5.0/etna/analysis/forecast/utils.py` & `etna-2.6.0/etna/analysis/forecast/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/outliers/__init__.py` & `etna-2.6.0/etna/analysis/outliers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/analysis/outliers/density_outliers.py` & `etna-2.6.0/etna/analysis/outliers/density_outliers.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     ts: "TSDataset",
     in_column: str = "target",
     window_size: int = 15,
     distance_coef: float = 3,
     n_neighbors: int = 3,
     distance_func: Union[Literal["absolute_difference"], Callable[[float, float], float]] = "absolute_difference",
     index_only: bool = True,
-) -> Dict[str, Union[List[pd.Timestamp], pd.Series]]:
+) -> Dict[str, Union[List[pd.Timestamp], List[int], pd.Series]]:
     """Compute outliers according to density rule.
 
     For each element in the series build all the windows of size ``window_size`` containing this point.
     If any of the windows contains at least ``n_neighbors`` that are closer than ``distance_coef * std(series)``
     to target point according to ``distance_func`` target point is not an outlier.
 
     Parameters
```

### Comparing `etna-2.5.0/etna/analysis/outliers/hist_outliers.py` & `etna-2.6.0/etna/analysis/outliers/hist_outliers.py`

 * *Files identical despite different names*

```diff
@@ -297,15 +297,15 @@
             count = outlier_number
             now_min = approximation_error[-1][approximation_error.shape[1] - 1 - outlier_number][outlier_number]
     return np.array(sorted(anomalies[-1][approximation_error.shape[1] - 1 - count][count]))
 
 
 def get_anomalies_hist(
     ts: "TSDataset", in_column: str = "target", bins_number: int = 10, index_only: bool = True
-) -> typing.Dict[str, Union[List[pd.Timestamp], pd.Series]]:
+) -> typing.Dict[str, Union[List[pd.Timestamp], List[int], pd.Series]]:
     """
     Get point outliers in time series using histogram model.
 
     Outliers are all points that, when removed, result in a histogram with a lower approximation error,
     even with the number of bins less than the number of outliers.
 
     Parameters
```

### Comparing `etna-2.5.0/etna/analysis/outliers/median_outliers.py` & `etna-2.6.0/etna/analysis/outliers/median_outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 if typing.TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 def get_anomalies_median(
     ts: "TSDataset", in_column: str = "target", window_size: int = 10, alpha: float = 3, index_only: bool = True
-) -> Dict[str, Union[List[pd.Timestamp], pd.Series]]:
+) -> Dict[str, Union[List[pd.Timestamp], List[int], pd.Series]]:
     """
     Get point outliers in time series using median model (estimation model-based method).
 
     Outliers are all points deviating from the median by more than alpha * std,
     where std is the sample standard deviation in the window.
 
     Parameters
```

### Comparing `etna-2.5.0/etna/analysis/outliers/plots.py` & `etna-2.6.0/etna/analysis/outliers/plots.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 def plot_anomalies(
     ts: "TSDataset",
-    anomaly_dict: Dict[str, List[pd.Timestamp]],
+    anomaly_dict: Dict[str, List[Union[pd.Timestamp, int]]],
     in_column: str = "target",
     segments: Optional[List[str]] = None,
     columns_num: int = 2,
     figsize: Tuple[int, int] = (10, 5),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
 ):
     """Plot a time series with indicated anomalies.
 
     Parameters
     ----------
     ts:
         TSDataset of timeseries that was used for detect anomalies
@@ -43,14 +43,19 @@
         number of subplots columns
     figsize:
         size of the figure per subplot with one segment in inches
     start:
         start timestamp for plot
     end:
         end timestamp for plot
+
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
     """
     start, end = _get_borders_ts(ts, start, end)
 
     if segments is None:
         segments = sorted(ts.segments)
 
     _, ax = _prepare_axes(num_plots=len(segments), columns_num=columns_num, figsize=figsize)
@@ -67,20 +72,20 @@
 
         ax[i].tick_params("x", rotation=45)
 
 
 def plot_anomalies_interactive(
     ts: "TSDataset",
     segment: str,
-    method: Callable[..., Dict[str, List[pd.Timestamp]]],
+    method: Callable[..., Dict[str, List[Union[pd.Timestamp, int]]]],
     params_bounds: Dict[str, Tuple[Union[int, float], Union[int, float], Union[int, float]]],
     in_column: str = "target",
     figsize: Tuple[int, int] = (20, 10),
-    start: Optional[str] = None,
-    end: Optional[str] = None,
+    start: Optional[Union[pd.Timestamp, int, str]] = None,
+    end: Optional[Union[pd.Timestamp, int, str]] = None,
 ):
     """Plot a time series with indicated anomalies.
 
     Anomalies are obtained using the specified method. The method parameters values
     can be changed using the corresponding sliders.
 
     Parameters
@@ -103,21 +108,25 @@
         end timestamp for plot
 
     Notes
     -----
     Jupyter notebook might display the results incorrectly,
     in this case try to use ``!jupyter nbextension enable --py widgetsnbextension``.
 
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start`` or ``end`` is used according to ``ts.freq``.
+
     Examples
     --------
     >>> from etna.datasets import TSDataset
     >>> from etna.datasets import generate_ar_df
     >>> from etna.analysis import plot_anomalies_interactive, get_anomalies_density
-    >>> classic_df = generate_ar_df(periods=1000, start_time="2021-08-01", n_segments=2)
-    >>> df = TSDataset.to_dataset(classic_df)
+    >>> df = generate_ar_df(periods=1000, start_time="2021-08-01", n_segments=2)
     >>> ts = TSDataset(df, "D")
     >>> params_bounds = {"window_size": (5, 20, 1), "distance_coef": (0.1, 3, 0.25)}
     >>> method = get_anomalies_density
     >>> plot_anomalies_interactive(ts=ts, segment="segment_1", method=method, params_bounds=params_bounds, figsize=(20, 10)) # doctest: +SKIP
     """
     from ipywidgets import FloatSlider
     from ipywidgets import IntSlider
```

### Comparing `etna-2.5.0/etna/analysis/outliers/prediction_interval_outliers.py` & `etna-2.6.0/etna/analysis/outliers/prediction_interval_outliers.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,33 +46,37 @@
         list with segments names
 
     Returns
     -------
     result: TSDataset
         dataset with selected column.
     """
-    df = ts.raw_df.loc[:, pd.IndexSlice[segments, :]].copy()
+    df = ts.df.loc[:, pd.IndexSlice[segments, :]].copy()
     df = df.dropna()
     df_exog = ts.df_exog
     if df_exog is not None:
-        df_exog = df_exog.loc[df.index, pd.IndexSlice[segments, :]].copy()
+        df_exog = df_exog.loc[:, pd.IndexSlice[segments, :]].copy()
     known_future = ts.known_future
     freq = ts.freq
+
+    if df_exog is not None:
+        df = df.drop(df_exog.columns.get_level_values("feature").values.tolist(), axis=1, level=1)
+
     subset_ts = TSDataset(df=df, df_exog=df_exog, known_future=known_future, freq=freq)
     return subset_ts
 
 
 def get_anomalies_prediction_interval(
     ts: TSDataset,
     model: Union[Type["ProphetModel"], Type["SARIMAXModel"]],
     interval_width: float = 0.95,
     in_column: str = "target",
     index_only: bool = True,
     **model_params,
-) -> Dict[str, Union[List[pd.Timestamp], pd.Series]]:
+) -> Dict[str, Union[List[pd.Timestamp], List[int], pd.Series]]:
     """
     Get point outliers in time series using prediction intervals (estimation model-based method).
 
     Outliers are all points out of the prediction interval predicted with the model.
 
     Parameters
     ----------
```

### Comparing `etna-2.5.0/etna/analysis/utils.py` & `etna-2.6.0/etna/analysis/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import math
 from typing import TYPE_CHECKING
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
+from typing import Union
 
 import matplotlib.axes
 import matplotlib.figure
 import matplotlib.pyplot as plt
 import numpy as np
+import pandas as pd
 
 if TYPE_CHECKING:
     from etna.datasets import TSDataset
 
 
 def _prepare_axes(
     num_plots: int, columns_num: int, figsize: Tuple[int, int], set_grid: bool = True
@@ -27,16 +29,23 @@
     if set_grid:
         for cur_ax in ax:
             cur_ax.grid()
 
     return fig, ax
 
 
-def _get_borders_ts(ts: "TSDataset", start: Optional[str], end: Optional[str]) -> Tuple[str, str]:
+def _get_borders_ts(
+    ts: "TSDataset", start: Optional[Union[pd.Timestamp, int, str]], end: Optional[Union[pd.Timestamp, int, str]]
+) -> Tuple[str, str]:
     """Get start and end parameters according to given TSDataset."""
+    from etna.datasets.utils import _check_timestamp_param
+
+    start = _check_timestamp_param(param=start, param_name="start", freq=ts.freq)
+    end = _check_timestamp_param(param=end, param_name="end", freq=ts.freq)
+
     if start is not None:
         start_idx = ts.df.index.get_loc(start)
     else:
         start_idx = 0
 
     if end is not None:
         end_idx = ts.df.index.get_loc(end)
```

### Comparing `etna-2.5.0/etna/auto/__init__.py` & `etna-2.6.0/etna/auto/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,17 +14,15 @@
    from etna.datasets import TSDataset
    from etna.metrics import SMAPE
 
    CURRENT_DIR_PATH = pathlib.Path(__file__).parent
 
    if __name__ == "__main__":
       df = pd.read_csv(CURRENT_DIR_PATH / "data" / "example_dataset.csv")
-
-      ts = TSDataset.to_dataset(df)
-      ts = TSDataset(ts, freq="D")
+      ts = TSDataset(df, freq="D")
 
       # Create Auto object for greedy search
       # All trials will be saved in sqlite database
       # You can use it later for analysis with ``Auto.summary``
       auto = Auto(
          target_metric=SMAPE(),
          horizon=14,
```

### Comparing `etna-2.5.0/etna/auto/auto.py` & `etna-2.6.0/etna/auto/auto.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/optuna/config_sampler.py` & `etna-2.6.0/etna/auto/optuna/config_sampler.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/optuna/wrapper.py` & `etna-2.6.0/etna/auto/optuna/wrapper.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/pool/generator.py` & `etna-2.6.0/etna/auto/pool/generator.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/pool/templates.py` & `etna-2.6.0/etna/auto/pool/templates.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/runner/base.py` & `etna-2.6.0/etna/auto/runner/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/runner/local.py` & `etna-2.6.0/etna/auto/runner/local.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/auto/utils.py` & `etna-2.6.0/etna/auto/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/__init__.py` & `etna-2.6.0/etna/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/base.py` & `etna-2.6.0/etna/clustering/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/distances/base.py` & `etna-2.6.0/etna/clustering/distances/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/distances/distance_matrix.py` & `etna-2.6.0/etna/clustering/distances/distance_matrix.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/distances/dtw_distance.py` & `etna-2.6.0/etna/clustering/distances/dtw_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/distances/euclidean_distance.py` & `etna-2.6.0/etna/clustering/distances/euclidean_distance.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/hierarchical/base.py` & `etna-2.6.0/etna/clustering/hierarchical/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/hierarchical/dtw_clustering.py` & `etna-2.6.0/etna/clustering/hierarchical/dtw_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/clustering/hierarchical/euclidean_clustering.py` & `etna-2.6.0/etna/clustering/hierarchical/euclidean_clustering.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/commands/backtest_command.py` & `etna-2.6.0/etna/commands/backtest_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 ADDITIONAL_PIPELINE_PARAMETERS = {"context_size"}
 
 
 def backtest(
     config_path: Path = typer.Argument(..., help="path to yaml config with desired pipeline"),
     backtest_config_path: Path = typer.Argument(..., help="path to backtest config file"),
     target_path: Path = typer.Argument(..., help="path to csv with data to forecast"),
-    freq: str = typer.Argument(..., help="frequency of timestamp in files in pandas format"),
+    freq: str = typer.Argument(
+        ..., help="frequency of timestamp in files in pandas format or 'None' for integer timestamps"
+    ),
     output_path: Path = typer.Argument(..., help="where to save forecast"),
     exog_path: Optional[Path] = typer.Argument(default=None, help="path to csv with exog data"),
     known_future: Optional[List[str]] = typer.Argument(
         None,
         help="list of all known_future columns (regressor "
         "columns). If not specified then all exog_columns "
         "considered known_future.",
@@ -69,26 +71,32 @@
     =============  ===========  ===============  ===============
     """
     pipeline_configs = OmegaConf.to_object(OmegaConf.load(config_path))
     pipeline_configs = cast(Dict[str, Any], pipeline_configs)
 
     backtest_configs = OmegaConf.to_object(OmegaConf.load(backtest_config_path))
 
-    df_timeseries = pd.read_csv(target_path, parse_dates=["timestamp"])
+    if freq == "None":
+        freq_init = None
+        parse_dates = None
+    else:
+        freq_init = freq
+        parse_dates = ["timestamp"]
 
+    df_timeseries = pd.read_csv(target_path, parse_dates=parse_dates)
     df_timeseries = TSDataset.to_dataset(df_timeseries)
 
     df_exog = None
     k_f: Union[Literal["all"], Sequence[Any]] = ()
     if exog_path:
-        df_exog = pd.read_csv(exog_path, parse_dates=["timestamp"])
+        df_exog = pd.read_csv(exog_path, parse_dates=parse_dates)
         df_exog = TSDataset.to_dataset(df_exog)
         k_f = "all" if not known_future else known_future
 
-    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog, known_future=k_f)
+    tsdataset = TSDataset(df=df_timeseries, freq=freq_init, df_exog=df_exog, known_future=k_f)
 
     pipeline_args = remove_params(params=pipeline_configs, to_remove=ADDITIONAL_PIPELINE_PARAMETERS)
     pipeline: Pipeline = hydra_slayer.get_from_params(**pipeline_args)
     backtest_configs_hydra_slayer: Dict[str, Any] = hydra_slayer.get_from_params(**backtest_configs)
 
     # estimate number of folds if parameters set
     if backtest_configs_hydra_slayer.get("estimate_n_folds", False):
```

### Comparing `etna-2.5.0/etna/commands/forecast_command.py` & `etna-2.6.0/etna/commands/forecast_command.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 import typer
 from omegaconf import OmegaConf
 from typing_extensions import Literal
 
 from etna.commands.utils import estimate_max_n_folds
 from etna.commands.utils import remove_params
 from etna.datasets import TSDataset
-from etna.models.utils import determine_num_steps
+from etna.datasets.utils import _check_timestamp_param
+from etna.datasets.utils import determine_num_steps
 from etna.pipeline import Pipeline
 
 ADDITIONAL_FORECAST_PARAMETERS = {"start_timestamp", "estimate_n_folds"}
 ADDITIONAL_PIPELINE_PARAMETERS = {"context_size"}
 
 
 def compute_horizon(horizon: int, forecast_params: Dict[str, Any], tsdataset: TSDataset) -> int:
     """Compute new pipeline horizon if `start_timestamp` presented in `forecast_params`."""
     if "start_timestamp" in forecast_params:
-        forecast_start_timestamp = pd.Timestamp(forecast_params["start_timestamp"])
+        forecast_start_timestamp = _check_timestamp_param(
+            param=forecast_params["start_timestamp"], param_name="start_timestamp", freq=tsdataset.freq
+        )
         train_end_timestamp = tsdataset.index.max()
 
         if forecast_start_timestamp <= train_end_timestamp:
             raise ValueError("Parameter `start_timestamp` should greater than end of training dataset!")
 
         delta = determine_num_steps(
             start_timestamp=train_end_timestamp, end_timestamp=forecast_start_timestamp, freq=tsdataset.freq
@@ -49,24 +52,28 @@
         horizon = compute_horizon(horizon=horizon, forecast_params=forecast_params, tsdataset=tsdataset)
         config["horizon"] = horizon  # type: ignore
 
 
 def filter_forecast(forecast_ts: TSDataset, forecast_params: Dict[str, Any]) -> TSDataset:
     """Filter out forecasts before `start_timestamp` if `start_timestamp` presented in `forecast_params`."""
     if "start_timestamp" in forecast_params:
-        forecast_start_timestamp = pd.Timestamp(forecast_params["start_timestamp"])
+        forecast_start_timestamp = _check_timestamp_param(
+            param=forecast_params["start_timestamp"], param_name="start_timestamp", freq=forecast_ts.freq
+        )
         forecast_ts.df = forecast_ts.df.loc[forecast_start_timestamp:, :]
 
     return forecast_ts
 
 
 def forecast(
     config_path: Path = typer.Argument(..., help="path to yaml config with desired pipeline"),
     target_path: Path = typer.Argument(..., help="path to csv with data to forecast"),
-    freq: str = typer.Argument(..., help="frequency of timestamp in files in pandas format"),
+    freq: str = typer.Argument(
+        ..., help="frequency of timestamp in files in pandas format or 'None' for integer timestamps"
+    ),
     output_path: Path = typer.Argument(..., help="where to save forecast"),
     exog_path: Optional[Path] = typer.Argument(None, help="path to csv with exog data"),
     forecast_config_path: Optional[Path] = typer.Argument(None, help="path to yaml config with forecast params"),
     raw_output: bool = typer.Argument(False, help="by default we return only forecast without features"),
     known_future: Optional[List[str]] = typer.Argument(
         None,
         help="list of all known_future columns (regressor "
@@ -111,26 +118,33 @@
 
     if forecast_config_path:
         forecast_params_config = OmegaConf.to_object(OmegaConf.load(forecast_config_path))
     else:
         forecast_params_config = {}
     forecast_params: Dict[str, Any] = hydra_slayer.get_from_params(**forecast_params_config)
 
-    df_timeseries = pd.read_csv(target_path, parse_dates=["timestamp"])
+    if freq == "None":
+        freq_init = None
+        parse_dates = None
+    else:
+        freq_init = freq
+        parse_dates = ["timestamp"]
+
+    df_timeseries = pd.read_csv(target_path, parse_dates=parse_dates)
 
     df_timeseries = TSDataset.to_dataset(df_timeseries)
 
     df_exog = None
     k_f: Union[Literal["all"], Sequence[Any]] = ()
     if exog_path:
-        df_exog = pd.read_csv(exog_path, parse_dates=["timestamp"])
+        df_exog = pd.read_csv(exog_path, parse_dates=parse_dates)
         df_exog = TSDataset.to_dataset(df_exog)
         k_f = "all" if not known_future else known_future
 
-    tsdataset = TSDataset(df=df_timeseries, freq=freq, df_exog=df_exog, known_future=k_f)
+    tsdataset = TSDataset(df=df_timeseries, freq=freq_init, df_exog=df_exog, known_future=k_f)
 
     update_horizon(pipeline_configs=pipeline_configs, forecast_params=forecast_params, tsdataset=tsdataset)
 
     pipeline_args = remove_params(params=pipeline_configs, to_remove=ADDITIONAL_PIPELINE_PARAMETERS)
     pipeline: Pipeline = hydra_slayer.get_from_params(**pipeline_args)
     pipeline.fit(tsdataset)
```

### Comparing `etna-2.5.0/etna/commands/utils.py` & `etna-2.6.0/etna/commands/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/core/mixins.py` & `etna-2.6.0/etna/core/mixins.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/core/saving.py` & `etna-2.6.0/etna/core/saving.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/core/utils.py` & `etna-2.6.0/etna/core/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/datasets/datasets_generation.py` & `etna-2.6.0/etna/datasets/datasets_generation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 from typing import List
 from typing import Optional
+from typing import Sequence
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from numpy.random import RandomState
 from statsmodels.tsa.arima_process import arma_generate_sample
 
+from etna.datasets.utils import _check_timestamp_param
+from etna.datasets.utils import timestamp_range
+
+
+def _create_timestamp(
+    start_time: Optional[Union[pd.Timestamp, int, str]], freq: Optional[str], periods: int
+) -> Sequence[Union[pd.Timestamp, int]]:
+    if freq is None and start_time is None:
+        start_time = 0
+    if freq is not None and start_time is None:
+        start_time = pd.Timestamp("2000-01-01")
+    _check_timestamp_param(param=start_time, param_name="start_time", freq=freq)
+    return timestamp_range(start=start_time, periods=periods, freq=freq)
+
 
 def generate_ar_df(
     periods: int,
-    start_time: str,
+    start_time: Optional[Union[pd.Timestamp, int, str]] = None,
     ar_coef: Optional[list] = None,
     sigma: float = 1,
     n_segments: int = 1,
-    freq: str = "1D",
+    freq: Optional[str] = "D",
     random_seed: int = 1,
 ) -> pd.DataFrame:
     """
     Create DataFrame with AR process data.
 
     Parameters
     ----------
@@ -31,35 +47,40 @@
         scale of AR noise
     n_segments:
         number of segments
     freq:
         pandas frequency string for :py:func:`pandas.date_range` that is used to generate timestamp
     random_seed:
         random seed
+
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start_time`` is used according to ``freq``
     """
     if ar_coef is None:
         ar_coef = [1]
     random_sampler = RandomState(seed=random_seed).normal
     ar_coef = np.r_[1, -np.array(ar_coef)]
     ar_samples = arma_generate_sample(
         ar=ar_coef, ma=[1], nsample=(n_segments, periods), axis=1, distrvs=random_sampler, scale=sigma
     )
     df = pd.DataFrame(data=ar_samples.T, columns=[f"segment_{i}" for i in range(n_segments)])
-    df["timestamp"] = pd.date_range(start=start_time, freq=freq, periods=periods)
+    df["timestamp"] = _create_timestamp(start_time=start_time, freq=freq, periods=periods)
     df = df.melt(id_vars=["timestamp"], value_name="target", var_name="segment")
     return df
 
 
 def generate_periodic_df(
     periods: int,
-    start_time: str,
+    start_time: Optional[Union[pd.Timestamp, int, str]] = None,
     scale: float = 10,
     period: int = 1,
     n_segments: int = 1,
-    freq: str = "1D",
+    freq: Optional[str] = "D",
     add_noise: bool = False,
     sigma: float = 1,
     random_seed: int = 1,
 ) -> pd.DataFrame:
     """
     Create DataFrame with periodic data.
 
@@ -79,14 +100,19 @@
         pandas frequency string for :py:func:`pandas.date_range` that is used to generate timestamp
     add_noise:
         if True we add noise to final samples
     sigma:
         scale of added noise
     random_seed:
         random seed
+
+    Raises
+    ------
+    ValueError:
+        Non-integer timestamp parameter is used for integer-indexed timestamp.
     """
     samples = RandomState(seed=random_seed).randint(int(scale), size=(n_segments, period))
     patterns = [list(ar) for ar in samples]
     df = generate_from_patterns_df(
         periods=periods,
         start_time=start_time,
         patterns=patterns,
@@ -96,18 +122,18 @@
         add_noise=add_noise,
     )
     return df
 
 
 def generate_const_df(
     periods: int,
-    start_time: str,
-    scale: float,
+    start_time: Optional[Union[pd.Timestamp, int, str]] = None,
+    scale: float = 10,
     n_segments: int = 1,
-    freq: str = "1D",
+    freq: Optional[str] = "D",
     add_noise: bool = False,
     sigma: float = 1,
     random_seed: int = 1,
 ) -> pd.DataFrame:
     """
     Create DataFrame with const data.
 
@@ -115,26 +141,29 @@
     ----------
     periods:
         number of timestamps
     start_time:
         start timestamp
     scale:
         const value to fill
-    period:
-        data frequency -- x[i+period] = x[i]
     n_segments:
         number of segments
     freq:
         pandas frequency string for :py:func:`pandas.date_range` that is used to generate timestamp
     add_noise:
         if True we add noise to final samples
     sigma:
         scale of added noise
     random_seed:
         random seed
+
+    Raises
+    ------
+    ValueError:
+        Non-integer timestamp parameter is used for integer-indexed timestamp.
     """
     patterns = [[scale] for _ in range(n_segments)]
     df = generate_from_patterns_df(
         periods=periods,
         start_time=start_time,
         patterns=patterns,
         sigma=sigma,
@@ -143,17 +172,17 @@
         add_noise=add_noise,
     )
     return df
 
 
 def generate_from_patterns_df(
     periods: int,
-    start_time: str,
+    start_time: Optional[Union[pd.Timestamp, int, str]],
     patterns: List[List[float]],
-    freq: str = "1D",
+    freq: Optional[str] = "D",
     add_noise=False,
     sigma: float = 1,
     random_seed: int = 1,
 ) -> pd.DataFrame:
     """
     Create DataFrame from patterns.
 
@@ -169,34 +198,39 @@
         pandas frequency string for :py:func:`pandas.date_range` that is used to generate timestamp
     add_noise:
         if True we add noise to final samples
     sigma:
         scale of added noise
     random_seed:
         random seed
+
+    Raises
+    ------
+    ValueError:
+        Incorrect type of ``start_time`` is used according to ``freq``
     """
     n_segments = len(patterns)
     if add_noise:
         noise = RandomState(seed=random_seed).normal(scale=sigma, size=(n_segments, periods))
     else:
         noise = np.zeros(shape=(n_segments, periods))
     samples = noise
     for idx, pattern in enumerate(patterns):
         samples[idx, :] += np.array(pattern * (periods // len(pattern) + 1))[:periods]
     df = pd.DataFrame(data=samples.T, columns=[f"segment_{i}" for i in range(n_segments)])
-    df["timestamp"] = pd.date_range(start=start_time, freq=freq, periods=periods)
+    df["timestamp"] = _create_timestamp(start_time=start_time, freq=freq, periods=periods)
     df = df.melt(id_vars=["timestamp"], value_name="target", var_name="segment")
     return df
 
 
 def generate_hierarchical_df(
     periods: int,
     n_segments: List[int],
-    freq: str = "D",
-    start_time: str = "2000-01-01",
+    freq: Optional[str] = "D",
+    start_time: Optional[Union[pd.Timestamp, int, str]] = None,
     ar_coef: Optional[list] = None,
     sigma: float = 1,
     random_seed: int = 1,
 ) -> pd.DataFrame:
     """
     Create DataFrame with hierarchical structure and AR process data.
 
@@ -231,14 +265,16 @@
     ------
     ValueError:
         ``n_segments`` is empty
     ValueError:
         ``n_segments`` contains not positive integers
     ValueError:
         ``n_segments`` represents not non-decreasing sequence
+    ValueError:
+        Non-integer timestamp parameter is used for integer-indexed timestamp.
     """
     if len(n_segments) == 0:
         raise ValueError("`n_segments` should contain at least one positive integer!")
 
     if (np.less_equal(n_segments, 0)).any():
         raise ValueError("All `n_segments` elements should be positive!")
```

### Comparing `etna-2.5.0/etna/datasets/hierarchical_structure.py` & `etna-2.6.0/etna/datasets/hierarchical_structure.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/datasets/internal_datasets.py` & `etna-2.6.0/etna/datasets/internal_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,19 @@
             df_exog = pd.read_csv(
                 dataset_dir / EXOG_SUBDIRECTORY / f"{name}_{part}_exog.csv.gz",
                 compression="gzip",
                 header=[0, 1],
                 index_col=[0],
                 parse_dates=[0],
             )
+            # For some datasets there are real dates that we cannot use directly, so we save them in exog data. When we
+            # load dataset, we convert this dates into datetime so that the user can apply transforms to them.
+            if "exog_datetime_columns" in dataset_params:
+                dt_columns = [col for col in df_exog.columns if col[1] in dataset_params["exog_datetime_columns"]]
+                df_exog[dt_columns] = df_exog[dt_columns].astype("datetime64[ns]")
             ts = TSDataset(data, df_exog=df_exog, freq=freq)
         else:
             ts = TSDataset(data, freq=freq)
         ts_out.append(ts)
 
     if len(ts_out) == 1:
         return ts_out[0]
@@ -243,40 +248,42 @@
     ----------
     .. [1] https://github.com/Mcompetitions/M4-methods
     """
     get_freq = {"Hourly": "H", "Daily": "D", "Weekly": "W-MON", "Monthly": "M", "Quarterly": "QS-OCT", "Yearly": "D"}
     url_data = (
         "https://raw.githubusercontent.com/Mcompetitions/M4-methods/6c1067e5a57161249b17289a565178dc7a3fb3ca/Dataset/"
     )
-    end_date = "2022-01-01"
     freq = get_freq[dataset_freq]
 
     dataset_dir.mkdir(exist_ok=True, parents=True)
 
     data_train = pd.read_csv(f"{url_data}/Train/{dataset_freq}-train.csv", index_col=0)
     data_test = pd.read_csv(f"{url_data}/Test/{dataset_freq}-test.csv", index_col=0)
 
     segments = data_test.index
     test_target = data_test.values
+    test_len = test_target.shape[1]
+    train_target = [x[~np.isnan(x)] for x in data_train.values]
+
+    max_len = test_len + max([len(target) for target in train_target])
 
     df_list = []
-    test_timestamps = pd.date_range(end=end_date, freq=freq, periods=test_target.shape[1])
+    test_timestamps = np.arange(start=max_len - test_len, stop=max_len)
     for segment, target in zip(segments, test_target):
         df_segment = pd.DataFrame({"target": target})
         df_segment["segment"] = segment
         df_segment["timestamp"] = test_timestamps
         df_list.append(df_segment)
     df_test = pd.concat(df_list, axis=0)
 
-    train_target = [x[~np.isnan(x)] for x in data_train.values]
     df_list = []
     for segment, target in zip(segments, train_target):
         df_segment = pd.DataFrame({"target": target})
         df_segment["segment"] = segment
-        df_segment["timestamp"] = pd.date_range(end=test_timestamps[0], freq=freq, periods=len(target) + 1)[:-1]
+        df_segment["timestamp"] = np.arange(start=max_len - test_target.shape[1] - len(target), stop=max_len - test_len)
         df_list.append(df_segment)
     df_train = pd.concat(df_list, axis=0)
 
     df_full = pd.concat([df_train, df_test], axis=0)
 
     TSDataset.to_dataset(df_full).to_csv(
         dataset_dir / f"m4_{dataset_freq.lower()}_full.csv.gz", index=True, compression="gzip", float_format="%.8f"
@@ -441,50 +448,48 @@
     Download and save M3 dataset in different frequency modes.
 
     The M3 dataset is a collection of 3,003 time series used for the third edition of the Makridakis forecasting
     Competition. The M3 dataset consists of time series of yearly, quarterly, monthly and other data. Dataset with other
     data originally does not have any particular frequency, but we assume it as a quarterly data. Each frequency mode
     has its own specific prediction horizon: 6 for yearly, 8 for quarterly, 18 for monthly, and 8 for other.
 
-    M3 dataset has series ending on different dates. As to the specificity of TSDataset we should add custom dates
-    to make series end on one date. Original dates are added as an exogenous data. For example, ``df_exog`` of train
-    dataset has dates for train and test and ``df_exog`` of test dataset has dates only for test.
+    M3 dataset has series ending on different dates. As to the specificity of TSDataset we use integer index use integer
+    index to make series end on one timestamp. Original dates are added as an exogenous data. For example, ``df_exog``
+    of train dataset has dates for train and test and ``df_exog`` of test dataset has dates only for test.
 
     Parameters
     ----------
     dataset_dir:
         The path for saving dataset locally.
     dataset_freq:
         Frequency mode.
 
     References
     ----------
     .. [1] https://forvis.github.io/datasets/m3-data/
     .. [2] https://forecasters.org/resources/time-series-data/m3-competition/
     """
-    get_freq = {"monthly": "M", "quarterly": "Q-DEC", "yearly": "A-DEC", "other": "Q-DEC"}
     get_horizon = {"monthly": 18, "quarterly": 8, "yearly": 6, "other": 8}
     url_data = "https://forvis.github.io/data"
-    end_date = "2022-01-01"
-    freq = get_freq[dataset_freq]
+    horizon = get_horizon[dataset_freq]
     exog_dir = dataset_dir / EXOG_SUBDIRECTORY
 
     exog_dir.mkdir(exist_ok=True, parents=True)
 
     data = pd.read_csv(f"{url_data}/M3_{dataset_freq}_TSTS.csv")
+    max_len = data.groupby("series_id")["timestamp"].count().max()
 
     df_full = pd.DataFrame()
     df_train = pd.DataFrame()
     df_test = pd.DataFrame()
 
     df_full_exog = pd.DataFrame()
     df_test_exog = pd.DataFrame()
-    horizon = get_horizon[dataset_freq]
     for _, group in data.groupby("series_id"):
-        timestamps = pd.date_range(end=end_date, freq=freq, periods=group.shape[0])
+        timestamps = np.arange(start=max_len - group.shape[0], stop=max_len)
         group.rename(columns={"timestamp": "origin_timestamp", "series_id": "segment", "value": "target"}, inplace=True)
         group["segment"] = group["segment"] + "_" + group["category"]
         group.drop(columns=["category"], inplace=True)
         group["timestamp"] = timestamps
 
         df_full_part_exog = group.copy()
         df_full_part_exog.drop(columns=["target"], inplace=True)
@@ -496,23 +501,31 @@
 
         df_full = pd.concat([df_full, group])
         df_train = pd.concat([df_train, train_part])
         df_test = pd.concat([df_test, test_part])
         df_full_exog = pd.concat([df_full_exog, df_full_part_exog])
         df_test_exog = pd.concat([df_test_exog, df_test_part_exog])
 
+    if dataset_freq == "yearly":
+        df_full_exog["origin_timestamp"] = pd.to_datetime(df_full_exog["origin_timestamp"], format="%Y")
+        df_test_exog["origin_timestamp"] = pd.to_datetime(df_test_exog["origin_timestamp"], format="%Y")
+    elif dataset_freq != "other":
+        df_full_exog["origin_timestamp"] = pd.to_datetime(df_full_exog["origin_timestamp"])
+        df_test_exog["origin_timestamp"] = pd.to_datetime(df_test_exog["origin_timestamp"])
+
     TSDataset.to_dataset(df_full).to_csv(
         dataset_dir / f"m3_{dataset_freq.lower()}_full.csv.gz", index=True, compression="gzip", float_format="%.8f"
     )
     TSDataset.to_dataset(df_train).to_csv(
         dataset_dir / f"m3_{dataset_freq.lower()}_train.csv.gz", index=True, compression="gzip", float_format="%.8f"
     )
     TSDataset.to_dataset(df_test).to_csv(
         dataset_dir / f"m3_{dataset_freq.lower()}_test.csv.gz", index=True, compression="gzip", float_format="%.8f"
     )
+
     TSDataset.to_dataset(df_full_exog).to_csv(
         dataset_dir / EXOG_SUBDIRECTORY / f"m3_{dataset_freq.lower()}_full_exog.csv.gz",
         index=True,
         compression="gzip",
         float_format="%.8f",
     )
     TSDataset.to_dataset(df_full_exog).to_csv(
@@ -534,37 +547,36 @@
     Download and save tourism dataset in different frequency modes.
 
     Dataset contains 1311 series in three frequency modes: monthly, quarterly, yearly. They were supplied by both
     tourism bodies (such as Tourism Australia, the Hong Kong Tourism Board and Tourism New Zealand) and various
     academics, who had used them in previous tourism forecasting studies. Each frequency mode has its own specific
     prediction horizon: 4 for yearly, 8 for quarterly, 24 for monthly.
 
-    Tourism dataset has series ending on different dates. As to the specificity of TSDataset we should add custom dates
-    to make series end on one date. Original dates are added as an exogenous data. For example, ``df_exog`` of train
+    Tourism dataset has series ending on different dates. As to the specificity of TSDataset we use integer index to
+    make series end on one timestamp. Original dates are added as an exogenous data. For example, ``df_exog`` of train
     dataset has dates for train and test and ``df_exog`` of test dataset has dates only for test.
 
     References
     ----------
     .. [1] https://robjhyndman.com/publications/the-tourism-forecasting-competition/
     """
     get_freq = {"monthly": "MS", "quarterly": "Q-DEC", "yearly": "A-DEC"}
     start_index_target_rows = {"monthly": 3, "quarterly": 3, "yearly": 2}
-    end_date = "2022-01-01"
     freq = get_freq[dataset_freq]
     target_index = start_index_target_rows[dataset_freq]
     exog_dir = dataset_dir / EXOG_SUBDIRECTORY
 
     exog_dir.mkdir(exist_ok=True, parents=True)
 
     data_train, data_test = _download_dataset_zip(
         "https://robjhyndman.com/data/27-3-Athanasopoulos1.zip",
         file_names=(f"{dataset_freq}_in.csv", f"{dataset_freq}_oos.csv"),
         read_functions=(partial(pd.read_csv, sep=","), partial(pd.read_csv, sep=",")),
     )
-
+    max_len = int(data_train.iloc[0].max() + data_test.iloc[0].max())
     segments = data_train.columns
 
     df_full = pd.DataFrame()
     df_train = pd.DataFrame()
     df_test = pd.DataFrame()
 
     df_full_exog = pd.DataFrame()
@@ -579,15 +591,15 @@
         date_params = list(map(int, data_train_[~np.isnan(data_train_)][1:target_index]))
         initial_date = date(date_params[0], date_params[1], 1) if len(date_params) == 2 else date(date_params[0], 1, 1)
 
         target_train = data_train_[~np.isnan(data_train_)][target_index : target_index + train_size]
         target_test = data_test_[target_index : target_index + test_size]
         target_full = np.concatenate([target_train, target_test])
 
-        new_timestamps = pd.date_range(end=end_date, freq=freq, periods=len(target_full))
+        new_timestamps = np.arange(start=max_len - len(target_full), stop=max_len)
         initial_timestamps = pd.date_range(start=initial_date, periods=len(target_full), freq=freq)
 
         df_full_ = pd.DataFrame(
             {"timestamp": new_timestamps, "segment": [seg] * len(target_full), "target": target_full}
         )
         df_train_ = df_full_.head(train_size)
         df_test_ = df_full_.tail(test_size)
@@ -748,15 +760,15 @@
     df["timestamp"] = pd.to_datetime(df["timestamp"], dayfirst=True)
     df = df.drop(["Date", "Time"], axis=1).melt("timestamp", var_name="segment", value_name="target")
     df_full = TSDataset.to_dataset(df)
 
     df_full.to_csv(dataset_dir / f"IHEPC_T_full.csv.gz", index=True, compression="gzip", float_format="%.8f")
 
 
-def get_australian_wine_sales_daataset(dataset_dir: Path) -> None:
+def get_australian_wine_sales_dataset(dataset_dir: Path) -> None:
     """
     Download and save Australian total wine sales by wine makers in bottles.
 
     This dataset consists of wine sales by Australian wine makers between Jan 1980 – Aug 1994.
 
     References
     ----------
@@ -795,110 +807,113 @@
             "train": "a3148ff2119a29f9d4c5f33bb0f7897d",
             "test": "df98e934e70e9b1dcfb0a3ee6858d76f",
             "full": "97209d3727630e6533776ce027048f71",
         },
     },
     "m3_monthly": {
         "get_dataset_function": partial(get_m3_dataset, dataset_freq="monthly"),
-        "freq": "M",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "cfa58e9c2caf28849f5397ba159887b2",
-            "test": "9d8f9871e418239f0efc23550dbe2e91",
-            "full": "d1a8bad4aba489d04063dd48cedb96a5",
+            "train": "36535626a98157ccbfe3d1f5b2d964ac",
+            "test": "09af36fa503b41ea5283db6ec6063ae1",
+            "full": "4babb773e580501b4918557555157f34",
         },
     },
     "m3_quarterly": {
         "get_dataset_function": partial(get_m3_dataset, dataset_freq="quarterly"),
-        "freq": "Q-DEC",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "f944dd06aa47a495f18b40f0a1dab6a5",
-            "test": "d29138ea613c8a4945cbd421754254e0",
-            "full": "fdfdd5400dce06530d576f4136d13421",
+            "train": "fb4286f519a6aa9385937c47dde6ddf4",
+            "test": "a27614afc474472f842a152a6ceb95e6",
+            "full": "dba2451b2aac7fc397c1cff5ad32a3dd",
         },
     },
     "m3_yearly": {
         "get_dataset_function": partial(get_m3_dataset, dataset_freq="yearly"),
-        "freq": "A-DEC",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "6eb14930144e2012d0132f0b809cf2d8",
-            "test": "15ad9304aa9d0a3acf6496e7e5e03176",
-            "full": "d41fadf624a61645c545847e2154c4a9",
+            "train": "1d14eb24b2dd7bc9796a5758c6b215f1",
+            "test": "ad83bafa0533557a65e124aed9b1c381",
+            "full": "62fc772fe16c1e0eb53401f088f82b6a",
         },
     },
     "m3_other": {
         "get_dataset_function": partial(get_m3_dataset, dataset_freq="other"),
-        "freq": "Q-DEC",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "9132a834a7edb7f7c10215f753c0d68c",
-            "test": "d489b43229c7498c937f38fa465e8734",
-            "full": "9b55fd0bc336120e3756e022f5beade3",
+            "train": "37316d0cc7eb45c653719aea0be53880",
+            "test": "a63258ce320d3f2e68c019c9f23767b1",
+            "full": "81b024a7ef1b6be31e748c47edb057be",
         },
     },
     "m4_hourly": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Hourly"),
-        "freq": "H",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "61dcfc17181fdeb67821fc3a9ff4b509",
-            "test": "53768f5aa63d5c99eb6841fbd14fa42f",
-            "full": "1bf6e9a9f5ae7e19261bb01a9a24da6f",
+            "train": "239f11e69086ee0ef9c39fcb0bb89286",
+            "test": "36cc4ae564342a361695c402e6812074",
+            "full": "fd299eaaa9ef3deadabb0197c37ba8b2",
         },
     },
     "m4_daily": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Daily"),
-        "freq": "D",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "dbf8a576d00f1e523f01f8a72af6c0da",
-            "test": "294ad20e7c6f0a1dddb4f749b7473dc0",
-            "full": "11e60a29e9ea7c4f9672e77bd107e4d8",
+            "train": "7878f1485a779da34848f900c58ca991",
+            "test": "e26d4a1bc0b45428a52f1ba8be3bf510",
+            "full": "7a1ce18e378fb8c69f02757547ccab4c",
         },
     },
     "m4_weekly": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Weekly"),
-        "freq": "W-MON",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "26821e9fd21cac965bbedc35a137f18a",
-            "test": "6798cae75181c5f0c1a608eb0e59e23f",
-            "full": "5bdbaff1a011ef8723f09a38e0266fcf",
+            "train": "6dedd34a04fefb7f6da626b37fcf0ad2",
+            "test": "69f807a621b864d7e2d51f6daca147d8",
+            "full": "9954d2341af9615472f58afcc9dae2fd",
         },
     },
     "m4_monthly": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Monthly"),
-        "freq": "M",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "f625bc066e42299132aaad2a79e54537",
-            "test": "9e2dc5262ca01b5d2c0a6d2993039735",
-            "full": "78a96c47ee4335bd59e33a1e7b26c3b3",
+            "train": "6c1f5212132429c24279c583d8350ec3",
+            "test": "8495595ea49766f94855e2275adf41e8",
+            "full": "69e4479c83174eddf22b9c125de086b8",
         },
     },
     "m4_quarterly": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Quarterly"),
-        "freq": "QS-JAN",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "540c397f52a13dd17f5158ab799a93f9",
-            "test": "8a145e44f9ce19ffe004d867ac7899d4",
-            "full": "745c6e679a600dcd96211c7717605d72",
+            "train": "a82abe6bb3d471ae23dc8de0c28d62c2",
+            "test": "2469cf58fea2468c30ffc4ad5891b67c",
+            "full": "bc076efa89d65cb5ce35d867b9bfcb3b",
         },
     },
     "m4_yearly": {
         "get_dataset_function": partial(get_m4_dataset, dataset_freq="Yearly"),
-        "freq": "D",
+        "freq": None,
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "67d73db6245af5c5551f38d315e290f9",
-            "test": "806d1f2257162fe95c98718db2f04ab7",
-            "full": "011bef4ab44721a99288d502ccb2bc98",
+            "train": "b44199b886507abd9118e0f756527af9",
+            "test": "676c705384b67d4ffad6d5b25873501e",
+            "full": "1ee536a16c9d505f5411de5fc8e0e265",
         },
     },
     "traffic_2008_10T": {
         "get_dataset_function": partial(get_traffic_2008_dataset, dataset_freq="10T"),
         "freq": "10T",
         "parts": ("train", "test", "full"),
         "hash": {
@@ -925,40 +940,43 @@
             "train": "838f0b7b012cf0bf3427fb5b1a4c053f",
             "test": "67b2d13ec809f3ce58834932460793e5",
             "full": "4edf42371f28685137ac402c6a7ad2cd",
         },
     },
     "tourism_monthly": {
         "get_dataset_function": partial(get_tourism_dataset, dataset_freq="monthly"),
-        "freq": "MS",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "2a32e030b783a0de3e74f9d412e6e70c",
-            "test": "c5d4f520692d000cd6517e1cd67f2345",
-            "full": "f1d8b9bf506d49f6c902c97624fe23bd",
+            "train": "eb65658979dcf20254df2e27793c4a2f",
+            "test": "4413d427fb1c7fd161a2ae896a9f2e17",
+            "full": "ccb8fd049488568af81c9fe341d05470",
         },
     },
     "tourism_quarterly": {
         "get_dataset_function": partial(get_tourism_dataset, dataset_freq="quarterly"),
-        "freq": "Q-DEC",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "9840d4875899d81349321aae6f859c21",
-            "test": "17e193090a32c91fc482db9993f5db28",
-            "full": "645822fcb6a46dfe7375d2eb6f117ef2",
+            "train": "380fe61422a5333043b714c22bcb6725",
+            "test": "0cea851864a96c344778037d3baaedf5",
+            "full": "a58fd54e937182b52220c7e733b982ca",
         },
     },
     "tourism_yearly": {
         "get_dataset_function": partial(get_tourism_dataset, dataset_freq="yearly"),
-        "freq": "A-DEC",
+        "freq": None,
+        "exog_datetime_columns": ("origin_timestamp",),
         "parts": ("train", "test", "full"),
         "hash": {
-            "train": "d0781023602223cc9b9c2dca1981c0fb",
-            "test": "a5461b2fcbf6bac12591d657b1b930f9",
-            "full": "9032dbd5d0a7e0f696d6a5c005a493e0",
+            "train": "62ccbd0a636fd8797d20eab58d78e503",
+            "test": "52d826295bf39cca8ab067c04e0fb883",
+            "full": "33bc585db54a4b965149ff9b991c2def",
         },
     },
     "weather_10T": {
         "get_dataset_function": get_weather_dataset,
         "freq": "10T",
         "parts": ("train", "test", "full"),
         "hash": {
@@ -1010,13 +1028,13 @@
     "IHEPC_T": {
         "get_dataset_function": get_ihepc_dataset,
         "freq": "T",
         "parts": ("full",),
         "hash": {"full": "8909138462ea130b9809907e947ffae6"},
     },
     "australian_wine_sales_monthly": {
-        "get_dataset_function": get_australian_wine_sales_daataset,
+        "get_dataset_function": get_australian_wine_sales_dataset,
         "freq": "MS",
         "parts": ("full",),
         "hash": {"full": "2dd34b5306d5e5372727e4d610b713be"},
     },
 }
```

### Comparing `etna-2.5.0/etna/datasets/tsdataset.py` & `etna-2.6.0/etna/datasets/tsdataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,27 +18,31 @@
 import pandas as pd
 from deprecated import deprecated
 from matplotlib import pyplot as plt
 from typing_extensions import Literal
 
 from etna import SETTINGS
 from etna.datasets.hierarchical_structure import HierarchicalStructure
+from etna.datasets.utils import DataFrameFormat
+from etna.datasets.utils import _check_timestamp_param
 from etna.datasets.utils import _TorchDataset
+from etna.datasets.utils import apply_alignment
 from etna.datasets.utils import get_level_dataframe
+from etna.datasets.utils import infer_alignment
 from etna.datasets.utils import inverse_transform_target_components
+from etna.datasets.utils import make_timestamp_df_from_alignment
+from etna.datasets.utils import timestamp_range
 from etna.loggers import tslogger
 
 if TYPE_CHECKING:
     from etna.transforms.base import Transform
 
 if SETTINGS.torch_required:
     from torch.utils.data import Dataset
 
-TTimestamp = Union[str, pd.Timestamp]
-
 
 class TSDataset:
     """TSDataset is the main class to handle your time series data.
 
     It prepares the series for exploration analyzing, implements feature generation with Transforms
     and generation of future points.
 
@@ -50,16 +54,15 @@
 
     During creation segment is casted to string type.
 
     Examples
     --------
     >>> from etna.datasets import generate_const_df
     >>> df = generate_const_df(periods=30, start_time="2021-06-01", n_segments=2, scale=1)
-    >>> df_ts_format = TSDataset.to_dataset(df)
-    >>> ts = TSDataset(df_ts_format, "D")
+    >>> ts = TSDataset(df, "D")
     >>> ts["2021-06-01":"2021-06-07", "segment_0", "target"]
     timestamp
     2021-06-01    1.0
     2021-06-02    1.0
     2021-06-03    1.0
     2021-06-04    1.0
     2021-06-05    1.0
@@ -70,16 +73,14 @@
     >>> from etna.datasets import generate_ar_df
     >>> pd.options.display.float_format = '{:,.2f}'.format
     >>> df_to_forecast = generate_ar_df(100, start_time="2021-01-01", n_segments=1)
     >>> df_regressors = generate_ar_df(120, start_time="2021-01-01", n_segments=5)
     >>> df_regressors = df_regressors.pivot(index="timestamp", columns="segment").reset_index()
     >>> df_regressors.columns = ["timestamp"] + [f"regressor_{i}" for i in range(5)]
     >>> df_regressors["segment"] = "segment_0"
-    >>> df_to_forecast = TSDataset.to_dataset(df_to_forecast)
-    >>> df_regressors = TSDataset.to_dataset(df_regressors)
     >>> tsdataset = TSDataset(df=df_to_forecast, freq="D", df_exog=df_regressors, known_future="all")
     >>> tsdataset.df.head(5)
     segment      segment_0
     feature    regressor_0 regressor_1 regressor_2 regressor_3 regressor_4 target
     timestamp
     2021-01-01        1.62       -0.02       -0.50       -0.56        0.52   1.62
     2021-01-02        1.01       -0.80       -0.81        0.38       -0.60   1.01
@@ -105,76 +106,172 @@
 
     #: Shortcut for :py:class:`pd.core.indexing.IndexSlice`
     idx = pd.IndexSlice
 
     def __init__(
         self,
         df: pd.DataFrame,
-        freq: str,
+        freq: Optional[str],
         df_exog: Optional[pd.DataFrame] = None,
         known_future: Union[Literal["all"], Sequence] = (),
         hierarchical_structure: Optional[HierarchicalStructure] = None,
     ):
         """Init TSDataset.
 
         Parameters
         ----------
         df:
-            dataframe with timeseries
+            dataframe with timeseries in a wide or long format: :py:class:`~etna.datasets.utils.DataFrameFormat`;
+            it is expected that ``df`` has feature named "target"
         freq:
-            frequency of timestamp in df
+            frequency of timestamp in df, possible values:
+
+            - `pandas offset aliases <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases>`_
+              for datetime timestamp
+
+            - None for integer timestamp
+
         df_exog:
-            dataframe with exogenous data;
+            dataframe with exogenous data in a wide or long format: :py:class:`~etna.datasets.utils.DataFrameFormat`
         known_future:
             columns in ``df_exog[known_future]`` that are regressors,
             if "all" value is given, all columns are meant to be regressors
         hierarchical_structure:
             Structure of the levels in the hierarchy. If None, there is no hierarchical structure in the dataset.
         """
-        self.raw_df = self._prepare_df(df)
-        self.raw_df.index = pd.to_datetime(self.raw_df.index)
         self.freq = freq
         self.df_exog = None
-
-        self.raw_df.index = pd.to_datetime(self.raw_df.index)
-
-        try:
-            inferred_freq = pd.infer_freq(self.raw_df.index)
-        except ValueError:
-            warnings.warn("TSDataset freq can't be inferred")
-            inferred_freq = None
-
-        if inferred_freq != self.freq:
-            warnings.warn(
-                f"You probably set wrong freq. Discovered freq in you data is {inferred_freq}, you set {self.freq}"
-            )
-
-        self.raw_df = self.raw_df.asfreq(self.freq)
-
+        self.raw_df = self._prepare_df(df=df.copy(deep=True), freq=freq)
         self.df = self.raw_df.copy(deep=True)
 
-        self.known_future = self._check_known_future(known_future, df_exog)
-        self._regressors = copy(self.known_future)
-
         self.hierarchical_structure = hierarchical_structure
         self.current_df_level: Optional[str] = self._get_dataframe_level(df=self.df)
         self.current_df_exog_level: Optional[str] = None
 
         if df_exog is not None:
-            self.df_exog = df_exog.copy(deep=True)
-            self.df_exog.index = pd.to_datetime(self.df_exog.index)
+            self.df_exog = self._prepare_df_exog(df_exog=df_exog.copy(deep=True), freq=freq)
+
+            self.known_future = self._check_known_future(known_future, self.df_exog)
+            self._regressors = copy(self.known_future)
+
             self.current_df_exog_level = self._get_dataframe_level(df=self.df_exog)
             if self.current_df_level == self.current_df_exog_level:
-                self.df = self._merge_exog(self.df)
+                self.df = self._merge_exog(df=self.df)
+        else:
+            self.known_future = self._check_known_future(known_future, df_exog)
+            self._regressors = copy(self.known_future)
 
         self._target_components_names: Tuple[str, ...] = tuple()
         self._prediction_intervals_names: Tuple[str, ...] = tuple()
 
         self.df = self.df.sort_index(axis=1, level=("segment", "feature"))
 
+    @classmethod
+    def create_from_misaligned(
+        cls,
+        df: pd.DataFrame,
+        freq: Optional[str],
+        df_exog: Optional[pd.DataFrame] = None,
+        known_future: Union[Literal["all"], Sequence] = (),
+        future_steps: int = 1,
+        original_timestamp_name: str = "external_timestamp",
+    ) -> "TSDataset":
+        """Make TSDataset from misaligned data by realigning it according to inferred alignment in ``df``.
+
+        This method:
+        - Infers alignment using :py:func:`~etna.datasets.utils.infer_alignment`;
+        - Realigns ``df`` and ``df_exog`` using inferred alignment using :py:func:`~etna.datasets.utils.apply_alignment`;
+        - Creates exog feature with original timestamp using :py:func:`~etna.datasets.utils.make_timestamp_df_from_alignment`;
+        - Creates TSDataset from these data.
+
+        This method doesn't work with ``hierarchical_structure``, because it doesn't make much sense.
+
+        Parameters
+        ----------
+        df:
+            dataframe with timeseries in a long format: :py:class:`~etna.datasets.utils.DataFrameFormat`;
+            it is expected that ``df`` has feature named "target"
+        freq:
+            frequency of timestamp in df, possible values:
+
+            - `pandas offset aliases <https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#offset-aliases>`_
+              for datetime timestamp
+
+            - None for integer timestamp
+
+        df_exog:
+            dataframe with exogenous data in a long format: :py:class:`~etna.datasets.utils.DataFrameFormat`
+        known_future:
+            columns in ``df_exog[known_future]`` that are regressors,
+            if "all" value is given, all columns are meant to be regressors
+        future_steps:
+            determines on how many steps original timestamp should be extended into the future
+            before adding into ``df_exog``; expected to be positive
+        original_timestamp_name:
+            name for original timestamp column to add it into ``df_exog``
+
+        Returns
+        -------
+        :
+            Created TSDataset.
+
+        Raises
+        ------
+        ValueError:
+            If ``future_steps`` is not positive.
+        ValueError:
+            If ``original_timestamp_name`` intersects with columns in ``df_exog``.
+        ValueError:
+            Parameter ``df`` isn't in a long format.
+        ValueError:
+            Parameter ``df_exog`` isn't in a long format if it set.
+        """
+        if future_steps <= 0:
+            raise ValueError("Parameter future_steps should be positive!")
+        if df_exog is not None and original_timestamp_name in df_exog.columns:
+            raise ValueError("Parameter original_timestamp_name shouldn't intersect with columns in df_exog!")
+
+        alignment = infer_alignment(df)
+        df_realigned = apply_alignment(df=df, alignment=alignment)
+        df_realigned = TSDataset.to_dataset(df_realigned)
+
+        timestamp_start = df_realigned.index[0]
+        periods = len(df_realigned) + future_steps
+        timestamp_df = make_timestamp_df_from_alignment(
+            alignment=alignment,
+            start=timestamp_start,
+            periods=periods,
+            freq=freq,
+            timestamp_name=original_timestamp_name,
+        )
+        timestamp_df = TSDataset.to_dataset(timestamp_df)
+
+        if df_exog is not None:
+            df_exog_realigned = apply_alignment(df=df_exog, alignment=alignment)
+            df_exog_realigned = TSDataset.to_dataset(df_exog_realigned)
+
+            df_exog_realigned = df_exog_realigned.join(timestamp_df, how="outer")
+        else:
+            df_exog_realigned = timestamp_df
+
+        known_future_realigned: Union[Literal["all"], Sequence]
+        if known_future != "all":
+            known_future_realigned = list(known_future)
+            known_future_realigned.append(original_timestamp_name)
+        else:
+            known_future_realigned = "all"
+
+        return TSDataset(
+            df=df_realigned,
+            df_exog=df_exog_realigned,
+            freq=None,
+            known_future=known_future_realigned,
+            hierarchical_structure=None,
+        )
+
     def _get_dataframe_level(self, df: pd.DataFrame) -> Optional[str]:
         """Return the level of the passed dataframe in hierarchical structure."""
         if self.hierarchical_structure is None:
             return None
 
         df_segments = df.columns.get_level_values("segment").unique()
         segment_levels = {self.hierarchical_structure.get_segment_level(segment=segment) for segment in df_segments}
@@ -199,21 +296,82 @@
         """Fit and apply given transforms to the data."""
         self._check_endings(warning=True)
         for transform in transforms:
             tslogger.log(f"Transform {repr(transform)} is applied to dataset")
             transform.fit_transform(self)
 
     @staticmethod
-    def _prepare_df(df: pd.DataFrame) -> pd.DataFrame:
-        # cast segment to str type
-        df_copy = df.copy(deep=True)
+    def _cast_segment_to_str(df: pd.DataFrame) -> pd.DataFrame:
         columns_frame = df.columns.to_frame()
-        columns_frame["segment"] = columns_frame["segment"].astype(str)
-        df_copy.columns = pd.MultiIndex.from_frame(columns_frame)
-        return df_copy
+        dtype = columns_frame["segment"].dtype
+        if not pd.api.types.is_object_dtype(dtype):
+            warnings.warn(
+                f"Segment values doesn't have string type, given type is {dtype}. "
+                f"Segments will be converted to string."
+            )
+            columns_frame["segment"] = columns_frame["segment"].astype(str)
+        df.columns = pd.MultiIndex.from_frame(columns_frame)
+        return df
+
+    @staticmethod
+    def _cast_index_to_datetime(df: pd.DataFrame, freq: str) -> pd.DataFrame:
+        if pd.api.types.is_numeric_dtype(df.index):
+            warnings.warn(
+                f"Timestamp contains numeric values, and given freq is {freq}. Timestamp will be converted to datetime."
+            )
+        df.index = pd.to_datetime(df.index)
+        return df
+
+    @classmethod
+    def _prepare_df(cls, df: pd.DataFrame, freq: Optional[str]) -> pd.DataFrame:
+        df_format = DataFrameFormat.determine(df)
+        if df_format is DataFrameFormat.long:
+            df = cls.to_dataset(df)
+
+        # cast segment to str type
+        cls._cast_segment_to_str(df)
+
+        # handle freq
+        if freq is None:
+            if not pd.api.types.is_integer_dtype(df.index.dtype):
+                raise ValueError("You set wrong freq. Data contains datetime index, not integer.")
+
+            new_index = np.arange(df.index.min(), df.index.max() + 1)
+            index_name = df.index.name
+            df = df.reindex(new_index)
+            df.index.name = index_name
+
+        else:
+            cls._cast_index_to_datetime(df, freq)
+            try:
+                inferred_freq = pd.infer_freq(df.index)
+            except ValueError:
+                warnings.warn("TSDataset freq can't be inferred")
+                inferred_freq = None
+
+            if inferred_freq is not None and inferred_freq != freq:
+                warnings.warn(
+                    f"You probably set wrong freq. Discovered freq in you data is {inferred_freq}, you set {freq}"
+                )
+
+            df = df.asfreq(freq)
+
+        return df
+
+    @classmethod
+    def _prepare_df_exog(cls, df_exog: pd.DataFrame, freq: Optional[str]) -> pd.DataFrame:
+        df_format = DataFrameFormat.determine(df_exog)
+        if df_format is DataFrameFormat.long:
+            df_exog = cls.to_dataset(df_exog)
+
+        df_exog = cls._cast_segment_to_str(df=df_exog)
+        if freq is not None:
+            cls._cast_index_to_datetime(df_exog, freq)
+
+        return df_exog
 
     def __repr__(self):
         return self.df.__repr__()
 
     def _repr_html_(self):
         return self.df._repr_html_()
 
@@ -226,14 +384,23 @@
             df = self.df.loc[self.idx[item[0]]]
         else:
             df = self.df.loc[self.idx[item[0]], self.idx[item[1], item[2]]]
         first_valid_idx = df.first_valid_index()
         df = df.loc[first_valid_idx:]
         return df
 
+    @staticmethod
+    def _expand_index(df: pd.DataFrame, freq: Optional[str], future_steps: int) -> pd.DataFrame:
+        to_add_index = timestamp_range(start=df.index[-1], periods=future_steps + 1, freq=freq)[1:]
+        new_index = df.index.append(to_add_index)
+        index_name = df.index.name
+        df = df.reindex(new_index)
+        df.index.name = index_name
+        return df
+
     def make_future(
         self, future_steps: int, transforms: Sequence["Transform"] = (), tail_steps: int = 0
     ) -> "TSDataset":
         """Return new TSDataset with features extended into the future.
 
         The result dataset doesn't contain quantiles and target components.
 
@@ -259,46 +426,39 @@
         ...    n_segments=2, scale=1
         ... )
         >>> df_regressors = pd.DataFrame({
         ...     "timestamp": list(pd.date_range("2021-06-01", periods=40))*2,
         ...     "regressor_1": np.arange(80), "regressor_2": np.arange(80) + 5,
         ...     "segment": ["segment_0"]*40 + ["segment_1"]*40
         ... })
-        >>> df_ts_format = TSDataset.to_dataset(df)
-        >>> df_regressors_ts_format = TSDataset.to_dataset(df_regressors)
         >>> ts = TSDataset(
-        ...     df_ts_format, "D", df_exog=df_regressors_ts_format, known_future="all"
+        ...     df, "D", df_exog=df_regressors, known_future="all"
         ... )
         >>> ts.make_future(4)
         segment      segment_0                      segment_1
         feature    regressor_1 regressor_2 target regressor_1 regressor_2 target
         timestamp
         2021-07-01          30          35    NaN          70          75    NaN
         2021-07-02          31          36    NaN          71          76    NaN
         2021-07-03          32          37    NaN          72          77    NaN
         2021-07-04          33          38    NaN          73          78    NaN
         """
         self._check_endings(warning=True)
-        max_date_in_dataset = self.df.index.max()
-        future_dates = pd.date_range(
-            start=max_date_in_dataset, periods=future_steps + 1, freq=self.freq, closed="right"
-        )
-
-        new_index = self.raw_df.index.append(future_dates)
-        df = self.raw_df.reindex(new_index)
-        df.index.name = "timestamp"
+        df = self._expand_index(df=self.raw_df, freq=self.freq, future_steps=future_steps)
 
         if self.df_exog is not None and self.current_df_level == self.current_df_exog_level:
-            df = self._merge_exog(df)
+            df = self._merge_exog(df=df)
 
             # check if we have enough values in regressors
+            # TODO: check performance
             if self.regressors:
+                future_index = df.index.difference(self.index)
                 for segment in self.segments:
                     regressors_index = self.df_exog.loc[:, pd.IndexSlice[segment, self.regressors]].index
-                    if not np.all(future_dates.isin(regressors_index)):
+                    if not np.all(future_index.isin(regressors_index)):
                         warnings.warn(
                             f"Some regressors don't have enough values in segment {segment}, "
                             f"NaN-s will be used for missing values"
                         )
 
         # remove components and quantiles
         # it should be done if we have quantiles and components in raw_df
@@ -337,17 +497,17 @@
 
     def tsdataset_idx_slice(self, start_idx: Optional[int] = None, end_idx: Optional[int] = None) -> "TSDataset":
         """Return new TSDataset with integer-location based indexing.
 
         Parameters
         ----------
         start_idx:
-            starting index of the slice.
+            starting integer index (counting from 0) of the slice.
         end_idx:
-            last index of the slice.
+            last integer index (counting from 0) of the slice.
 
         Returns
         -------
         :
             TSDataset based on indexing slice.
         """
         df_slice = self.df.iloc[start_idx:end_idx].copy(deep=True)
@@ -415,28 +575,31 @@
                     f"Series of segment {segment} have not enough history: "
                     f"{target_max} >= {exog_series_max}."
                 )
 
     def _merge_exog(self, df: pd.DataFrame) -> pd.DataFrame:
         if self.df_exog is None:
             raise ValueError("Something went wrong, Trying to merge df_exog which is None!")
+
+        # TODO: this check could probably be skipped at make_future
         df_regressors = self.df_exog.loc[:, pd.IndexSlice[:, self.known_future]]
         self._check_regressors(df=df, df_regressors=df_regressors)
+
         df = pd.concat((df, self.df_exog), axis=1).loc[df.index].sort_index(axis=1, level=(0, 1))
         return df
 
     def _check_endings(self, warning=False):
         """Check that all targets ends at the same timestamp."""
         max_index = self.df.index.max()
         if np.any(pd.isna(self.df.loc[max_index, pd.IndexSlice[:, "target"]])):
             if warning:
                 warnings.warn(
-                    "Segments contains NaNs in the last timestamps."
-                    "Some of the transforms might work incorrectly or even fail."
-                    "Make sure that you use the imputer before making the forecast."
+                    "Segments contains NaNs in the last timestamps. "
+                    "Some of the transforms might work incorrectly or even fail. "
+                    "Try to start using integer timestamp and align the segments."
                 )
             else:
                 raise ValueError("All segments should end at the same timestamp")
 
     def _inverse_transform_target_components(self, target_components_df: pd.DataFrame, target_df: pd.DataFrame):
         """Inverse transform target components in dataset with inverse transformed target."""
         self.drop_target_components()
@@ -479,16 +642,15 @@
         Examples
         --------
         >>> from etna.datasets import generate_const_df
         >>> df = generate_const_df(
         ...    periods=30, start_time="2021-06-01",
         ...    n_segments=2, scale=1
         ... )
-        >>> df_ts_format = TSDataset.to_dataset(df)
-        >>> ts = TSDataset(df_ts_format, "D")
+        >>> ts = TSDataset(df, "D")
         >>> ts.segments
         ['segment_0', 'segment_1']
         """
         return self.df.columns.get_level_values("segment").unique().tolist()
 
     @property
     def regressors(self) -> List[str]:
@@ -497,26 +659,24 @@
         Examples
         --------
         >>> from etna.datasets import generate_const_df
         >>> df = generate_const_df(
         ...    periods=30, start_time="2021-06-01",
         ...    n_segments=2, scale=1
         ... )
-        >>> df_ts_format = TSDataset.to_dataset(df)
         >>> regressors_timestamp = pd.date_range(start="2021-06-01", periods=50)
         >>> df_regressors_1 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 1, "segment": "segment_0"}
         ... )
         >>> df_regressors_2 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 2, "segment": "segment_1"}
         ... )
         >>> df_exog = pd.concat([df_regressors_1, df_regressors_2], ignore_index=True)
-        >>> df_exog_ts_format = TSDataset.to_dataset(df_exog)
         >>> ts = TSDataset(
-        ...     df_ts_format, df_exog=df_exog_ts_format, freq="D", known_future="all"
+        ...     df, df_exog=df_exog, freq="D", known_future="all"
         ... )
         >>> ts.regressors
         ['regressor_1']
         """
         return self._regressors
 
     @property
@@ -539,16 +699,16 @@
         return self._prediction_intervals_names
 
     def plot(
         self,
         n_segments: int = 10,
         column: str = "target",
         segments: Optional[Sequence[str]] = None,
-        start: Optional[str] = None,
-        end: Optional[str] = None,
+        start: Union[pd.Timestamp, int, str, None] = None,
+        end: Union[pd.Timestamp, int, str, None] = None,
         seed: int = 1,
         figsize: Tuple[int, int] = (10, 5),
     ):
         """Plot of random or chosen segments.
 
         Parameters
         ----------
@@ -562,38 +722,47 @@
             seed for local random state
         start:
             start plot from this timestamp
         end:
             end plot at this timestamp
         figsize:
             size of the figure per subplot with one segment in inches
+
+        Raises
+        ------
+        ValueError:
+            Incorrect type of ``start`` or ``end`` is used according to ``freq``
         """
         if segments is None:
             segments = self.segments
             k = min(n_segments, len(segments))
         else:
             k = len(segments)
         columns_num = min(2, k)
         rows_num = math.ceil(k / columns_num)
-        start = self.df.index.min() if start is None else pd.Timestamp(start)
-        end = self.df.index.max() if end is None else pd.Timestamp(end)
+
+        start = _check_timestamp_param(param=start, param_name="start", freq=self.freq)
+        end = _check_timestamp_param(param=end, param_name="end", freq=self.freq)
+
+        start = self.df.index.min() if start is None else start
+        end = self.df.index.max() if end is None else end
 
         figsize = (figsize[0] * columns_num, figsize[1] * rows_num)
         _, ax = plt.subplots(rows_num, columns_num, figsize=figsize, squeeze=False)
         ax = ax.ravel()
         rnd_state = np.random.RandomState(seed)
         for i, segment in enumerate(sorted(rnd_state.choice(segments, size=k, replace=False))):
             df_slice = self[start:end, segment, column]  # type: ignore
             ax[i].plot(df_slice.index, df_slice.values)
             ax[i].set_title(segment)
             ax[i].grid()
 
     @staticmethod
     def to_flatten(df: pd.DataFrame, features: Union[Literal["all"], Sequence[str]] = "all") -> pd.DataFrame:
-        """Return pandas DataFrame with flatten index.
+        """Return pandas DataFrame in a long format.
 
         The order of columns is (timestamp, segment, target,
         features in alphabetical order).
 
         Parameters
         ----------
         df:
@@ -617,16 +786,16 @@
         >>> df.head(5)
             timestamp    segment  target
         0  2021-06-01  segment_0    1.00
         1  2021-06-02  segment_0    1.00
         2  2021-06-03  segment_0    1.00
         3  2021-06-04  segment_0    1.00
         4  2021-06-05  segment_0    1.00
-        >>> df_ts_format = TSDataset.to_dataset(df)
-        >>> TSDataset.to_flatten(df_ts_format).head(5)
+        >>> df_wide = TSDataset.to_dataset(df)
+        >>> TSDataset.to_flatten(df_wide).head(5)
            timestamp    segment  target
         0 2021-06-01  segment_0    1.0
         1 2021-06-02  segment_0    1.0
         2 2021-06-03  segment_0    1.0
         3 2021-06-04  segment_0    1.0
         4 2021-06-05  segment_0    1.0
         """
@@ -662,17 +831,17 @@
 
     def to_pandas(self, flatten: bool = False, features: Union[Literal["all"], Sequence[str]] = "all") -> pd.DataFrame:
         """Return pandas DataFrame.
 
         Parameters
         ----------
         flatten:
-            * If False, return pd.DataFrame with multiindex
+            * If False, return dataframe in a wide format
 
-            * If True, return with flatten index,
+            * If True, return dataframe in a long format,
               its order of columns is (timestamp, segment, target,
               features in alphabetical order).
 
         features:
             List of features to return.
             If "all", return all the features in the dataset.
         Returns
@@ -690,16 +859,15 @@
         >>> df.head(5)
             timestamp    segment  target
         0  2021-06-01  segment_0    1.00
         1  2021-06-02  segment_0    1.00
         2  2021-06-03  segment_0    1.00
         3  2021-06-04  segment_0    1.00
         4  2021-06-05  segment_0    1.00
-        >>> df_ts_format = TSDataset.to_dataset(df)
-        >>> ts = TSDataset(df_ts_format, "D")
+        >>> ts = TSDataset(df, "D")
         >>> ts.to_pandas(True).head(5)
             timestamp    segment  target
         0  2021-06-01  segment_0    1.00
         1  2021-06-02  segment_0    1.00
         2  2021-06-03  segment_0    1.00
         3  2021-06-04  segment_0    1.00
         4  2021-06-05  segment_0    1.00
@@ -720,22 +888,23 @@
                 raise ValueError("The only possible literal is 'all'")
             segments = self.columns.get_level_values("segment").unique().tolist()
             return self.df.loc[:, self.idx[segments, features]].copy()
         return self.to_flatten(self.df, features=features)
 
     @staticmethod
     def to_dataset(df: pd.DataFrame) -> pd.DataFrame:
-        """Convert pandas dataframe to ETNA Dataset format.
+        """Convert pandas dataframe to wide format.
 
         Columns "timestamp" and "segment" are required.
 
         Parameters
         ----------
         df:
             DataFrame with columns ["timestamp", "segment"]. Other columns considered features.
+            Columns "timestamp" is expected to be one of two types: integer or timestamp.
 
         Notes
         -----
         During conversion segment is casted to string type.
 
         Examples
         --------
@@ -747,16 +916,16 @@
         >>> df.head(5)
            timestamp    segment  target
         0 2021-06-01  segment_0    1.00
         1 2021-06-02  segment_0    1.00
         2 2021-06-03  segment_0    1.00
         3 2021-06-04  segment_0    1.00
         4 2021-06-05  segment_0    1.00
-        >>> df_ts_format = TSDataset.to_dataset(df)
-        >>> df_ts_format.head(5)
+        >>> df_wide = TSDataset.to_dataset(df)
+        >>> df_wide.head(5)
         segment    segment_0 segment_1
         feature       target    target
         timestamp
         2021-06-01      1.00      1.00
         2021-06-02      1.00      1.00
         2021-06-03      1.00      1.00
         2021-06-04      1.00      1.00
@@ -774,19 +943,24 @@
         2021-01-01           0           5
         2021-01-02           1           6
         2021-01-03           2           7
         2021-01-04           3           8
         2021-01-05           4           9
         """
         df_copy = df.copy(deep=True)
-        df_copy["timestamp"] = pd.to_datetime(df_copy["timestamp"])
+
+        if not pd.api.types.is_integer_dtype(df_copy["timestamp"]):
+            df_copy["timestamp"] = pd.to_datetime(df_copy["timestamp"])
+
         df_copy["segment"] = df_copy["segment"].astype(str)
+
         feature_columns = df_copy.columns.tolist()
         feature_columns.remove("timestamp")
         feature_columns.remove("segment")
+
         df_copy = df_copy.pivot(index="timestamp", columns="segment")
         df_copy = df_copy.reorder_levels([1, 0], axis=1)
         df_copy.columns.names = ["segment", "feature"]
         df_copy = df_copy.sort_index(axis=1, level=(0, 1))
         return df_copy
 
     @staticmethod
@@ -869,21 +1043,27 @@
                 df=df, level_columns=level_columns, sep=sep
             )
 
         return df_copy, hierarchical_structure
 
     def _find_all_borders(
         self,
-        train_start: Optional[TTimestamp],
-        train_end: Optional[TTimestamp],
-        test_start: Optional[TTimestamp],
-        test_end: Optional[TTimestamp],
+        train_start: Union[pd.Timestamp, int, str, None],
+        train_end: Union[pd.Timestamp, int, str, None],
+        test_start: Union[pd.Timestamp, int, str, None],
+        test_end: Union[pd.Timestamp, int, str, None],
         test_size: Optional[int],
-    ) -> Tuple[TTimestamp, TTimestamp, TTimestamp, TTimestamp]:
+    ) -> Tuple[Union[pd.Timestamp, int], Union[pd.Timestamp, int], Union[pd.Timestamp, int], Union[pd.Timestamp, int]]:
         """Find borders for train_test_split if some values wasn't specified."""
+        # prepare and validate values
+        train_start = _check_timestamp_param(param=train_start, param_name="train_start", freq=self.freq)
+        train_end = _check_timestamp_param(param=train_end, param_name="train_end", freq=self.freq)
+        test_start = _check_timestamp_param(param=test_start, param_name="test_start", freq=self.freq)
+        test_end = _check_timestamp_param(param=test_end, param_name="test_end", freq=self.freq)
+
         if test_end is not None and test_start is not None and test_size is not None:
             warnings.warn(
                 "test_size, test_start and test_end cannot be applied at the same time. test_size will be ignored"
             )
 
         if test_end is None:
             if test_start is not None and test_size is not None:
@@ -931,25 +1111,25 @@
 
             if train_end is None:
                 test_start_idx = self.df.index.get_loc(test_start_defined)
                 train_end_defined = self.df.index[test_start_idx - 1]
             else:
                 train_end_defined = train_end
 
-        if np.datetime64(test_start_defined) < np.datetime64(train_end_defined):
+        if test_start_defined < train_end_defined:
             raise ValueError("The beginning of the test goes before the end of the train")
 
         return train_start_defined, train_end_defined, test_start_defined, test_end_defined
 
     def train_test_split(
         self,
-        train_start: Optional[TTimestamp] = None,
-        train_end: Optional[TTimestamp] = None,
-        test_start: Optional[TTimestamp] = None,
-        test_end: Optional[TTimestamp] = None,
+        train_start: Union[pd.Timestamp, int, str, None] = None,
+        train_end: Union[pd.Timestamp, int, str, None] = None,
+        test_start: Union[pd.Timestamp, int, str, None] = None,
+        test_end: Union[pd.Timestamp, int, str, None] = None,
         test_size: Optional[int] = None,
     ) -> Tuple["TSDataset", "TSDataset"]:
         """Split given df with train-test timestamp indices or size of test set.
 
         In case of inconsistencies between ``test_size`` and (``test_start``, ``test_end``), ``test_size`` is ignored
 
         Parameters
@@ -966,20 +1146,25 @@
             number of timestamps to use in test set
 
         Returns
         -------
         train, test:
             generated datasets
 
+        Raises
+        ------
+        ValueError:
+            Incorrect type of ``train_start`` or ``train_end`` or ``test_start`` or ``test_end``
+            is used according to ``ts.freq``
+
         Examples
         --------
         >>> from etna.datasets import generate_ar_df
         >>> pd.options.display.float_format = '{:,.2f}'.format
         >>> df = generate_ar_df(100, start_time="2021-01-01", n_segments=3)
-        >>> df = TSDataset.to_dataset(df)
         >>> ts = TSDataset(df, "D")
         >>> train_ts, test_ts = ts.train_test_split(
         ...     train_start="2021-01-01", train_end="2021-02-01",
         ...     test_start="2021-02-02", test_end="2021-02-07"
         ... )
         >>> train_ts.df.tail(5)
         segment    segment_0 segment_1 segment_2
@@ -1000,35 +1185,35 @@
         2021-02-05     -5.10      0.40      2.15
         2021-02-06     -6.22      0.92      0.97
         """
         train_start_defined, train_end_defined, test_start_defined, test_end_defined = self._find_all_borders(
             train_start, train_end, test_start, test_end, test_size
         )
 
-        if pd.Timestamp(test_end_defined) > self.df.index.max():
+        if test_end_defined > self.df.index.max():
             warnings.warn(f"Max timestamp in df is {self.df.index.max()}.")
-        if pd.Timestamp(train_start_defined) < self.df.index.min():
+        if train_start_defined < self.df.index.min():
             warnings.warn(f"Min timestamp in df is {self.df.index.min()}.")
 
-        train_df = self.df[train_start_defined:train_end_defined][self.raw_df.columns]  # type: ignore
-        train_raw_df = self.raw_df[train_start_defined:train_end_defined]  # type: ignore
+        train_df = self.df.loc[train_start_defined:train_end_defined][self.raw_df.columns]  # type: ignore
+        train_raw_df = self.raw_df.loc[train_start_defined:train_end_defined]  # type: ignore
         train = TSDataset(
             df=train_df,
             df_exog=self.df_exog,
             freq=self.freq,
             known_future=self.known_future,
             hierarchical_structure=self.hierarchical_structure,
         )
         train.raw_df = train_raw_df
         train._regressors = deepcopy(self.regressors)
         train._target_components_names = deepcopy(self.target_components_names)
         train._prediction_intervals_names = deepcopy(self._prediction_intervals_names)
 
-        test_df = self.df[test_start_defined:test_end_defined][self.raw_df.columns]  # type: ignore
-        test_raw_df = self.raw_df[train_start_defined:test_end_defined]  # type: ignore
+        test_df = self.df.loc[test_start_defined:test_end_defined][self.raw_df.columns]  # type: ignore
+        test_raw_df = self.raw_df.loc[train_start_defined:test_end_defined]  # type: ignore
         test = TSDataset(
             df=test_df,
             df_exog=self.df_exog,
             freq=self.freq,
             known_future=self.known_future,
             hierarchical_structure=self.hierarchical_structure,
         )
@@ -1068,15 +1253,15 @@
             Dataframe with the new columns in wide ETNA format.
         update_exog:
              If True, update columns also in df_exog.
              If you wish to add new regressors in the dataset it is recommended to turn on this flag.
         regressors:
             List of regressors in the passed dataframe.
         """
-        self.df = pd.concat((self.df, df_update[: self.df.index.max()]), axis=1).sort_index(axis=1)
+        self.df = pd.concat((self.df, df_update.loc[: self.df.index.max()]), axis=1).sort_index(axis=1)
         if update_exog:
             if self.df_exog is None:
                 self.df_exog = df_update
             else:
                 self.df_exog = pd.concat((self.df_exog, df_update), axis=1).sort_index(axis=1)
         if regressors is not None:
             self._regressors = list(set(self._regressors) | set(regressors))
@@ -1122,20 +1307,20 @@
             if len(unknown_columns) > 0:
                 warnings.warn(f"Features {unknown_columns} are not present in {name}!")
             if len(columns_to_remove) > 0:
                 df.drop(columns=columns_to_remove, level="feature", inplace=True)
         self._regressors = list(set(self._regressors) - features_set)
 
     @property
-    def index(self) -> pd.core.indexes.datetimes.DatetimeIndex:
+    def index(self) -> pd.Index:
         """Return TSDataset timestamp index.
 
         Returns
         -------
-        pd.core.indexes.datetimes.DatetimeIndex
+        :
             timestamp index of TSDataset
         """
         return self.df.index
 
     def level_names(self) -> Optional[List[str]]:
         """Return names of the levels in the hierarchical structure."""
         if self.hierarchical_structure is None:
@@ -1214,15 +1399,15 @@
 
     def add_target_components(self, target_components_df: pd.DataFrame):
         """Add target components into dataset.
 
         Parameters
         ----------
         target_components_df:
-            Dataframe in etna wide format with target components
+            Dataframe in a wide format with target components
 
         Raises
         ------
         ValueError:
             If dataset already contains target components
         ValueError:
             If target components names differ between segments
@@ -1271,15 +1456,15 @@
 
     def add_prediction_intervals(self, prediction_intervals_df: pd.DataFrame):
         """Add target components into dataset.
 
         Parameters
         ----------
         prediction_intervals_df:
-            Dataframe in etna wide format with prediction intervals
+            Dataframe in a wide format with prediction intervals
 
         Raises
         ------
         ValueError:
             If dataset already contains prediction intervals
         ValueError:
             If prediction intervals names differ between segments
@@ -1486,25 +1671,23 @@
         --------
         >>> from etna.datasets import generate_const_df
         >>> pd.options.display.expand_frame_repr = False
         >>> df = generate_const_df(
         ...    periods=30, start_time="2021-06-01",
         ...    n_segments=2, scale=1
         ... )
-        >>> df_ts_format = TSDataset.to_dataset(df)
         >>> regressors_timestamp = pd.date_range(start="2021-06-01", periods=50)
         >>> df_regressors_1 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 1, "segment": "segment_0"}
         ... )
         >>> df_regressors_2 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 2, "segment": "segment_1"}
         ... )
         >>> df_exog = pd.concat([df_regressors_1, df_regressors_2], ignore_index=True)
-        >>> df_exog_ts_format = TSDataset.to_dataset(df_exog)
-        >>> ts = TSDataset(df_ts_format, df_exog=df_exog_ts_format, freq="D", known_future="all")
+        >>> ts = TSDataset(df, df_exog=df_exog, freq="D", known_future="all")
         >>> ts.describe()
                   start_timestamp end_timestamp  length  num_missing  num_segments  num_exogs  num_regressors  num_known_future freq
         segments
         segment_0      2021-06-01    2021-06-30      30            0             2          1               1                 1    D
         segment_1      2021-06-01    2021-06-30      30            0             2          1               1                 1    D
         """
         # gather common information
@@ -1574,25 +1757,23 @@
         Examples
         --------
         >>> from etna.datasets import generate_const_df
         >>> df = generate_const_df(
         ...    periods=30, start_time="2021-06-01",
         ...    n_segments=2, scale=1
         ... )
-        >>> df_ts_format = TSDataset.to_dataset(df)
         >>> regressors_timestamp = pd.date_range(start="2021-06-01", periods=50)
         >>> df_regressors_1 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 1, "segment": "segment_0"}
         ... )
         >>> df_regressors_2 = pd.DataFrame(
         ...     {"timestamp": regressors_timestamp, "regressor_1": 2, "segment": "segment_1"}
         ... )
         >>> df_exog = pd.concat([df_regressors_1, df_regressors_2], ignore_index=True)
-        >>> df_exog_ts_format = TSDataset.to_dataset(df_exog)
-        >>> ts = TSDataset(df_ts_format, df_exog=df_exog_ts_format, freq="D", known_future="all")
+        >>> ts = TSDataset(df, df_exog=df_exog, freq="D", known_future="all")
         >>> ts.info()
         <class 'etna.datasets.TSDataset'>
         num_segments: 2
         num_exogs: 1
         num_regressors: 1
         num_known_future: 1
         freq: D
```

### Comparing `etna-2.5.0/etna/distributions/distributions.py` & `etna-2.6.0/etna/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/ensembles/direct_ensemble.py` & `etna-2.6.0/etna/ensembles/direct_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel
 from joblib import delayed
 
 from etna.datasets import TSDataset
@@ -29,16 +30,15 @@
     >>> from etna.datasets import generate_ar_df
     >>> from etna.datasets import TSDataset
     >>> from etna.ensembles import DirectEnsemble
     >>> from etna.models import NaiveModel
     >>> from etna.models import ProphetModel
     >>> from etna.pipeline import Pipeline
     >>> df = generate_ar_df(periods=30, start_time="2021-06-01", ar_coef=[1.2], n_segments=3)
-    >>> df_ts_format = TSDataset.to_dataset(df)
-    >>> ts = TSDataset(df_ts_format, "D")
+    >>> ts = TSDataset(df, "D")
     >>> prophet_pipeline = Pipeline(model=ProphetModel(), transforms=[], horizon=3)
     >>> naive_pipeline = Pipeline(model=NaiveModel(lag=10), transforms=[], horizon=5)
     >>> ensemble = DirectEnsemble(pipelines=[prophet_pipeline, naive_pipeline])
     >>> _ = ensemble.fit(ts=ts)
     >>> forecast = ensemble.forecast()
     >>> forecast
     segment    segment_0 segment_1 segment_2
@@ -144,16 +144,16 @@
         )
         forecast = self._merge(forecasts=forecasts)
         return forecast
 
     def _predict(
         self,
         ts: TSDataset,
-        start_timestamp: pd.Timestamp,
-        end_timestamp: pd.Timestamp,
+        start_timestamp: Union[pd.Timestamp, int],
+        end_timestamp: Union[pd.Timestamp, int],
         prediction_interval: bool,
         quantiles: Sequence[float],
         return_components: bool,
     ) -> TSDataset:
         if prediction_interval:
             raise NotImplementedError(f"Ensemble {self.__class__.__name__} doesn't support prediction intervals!")
         if return_components:
```

### Comparing `etna-2.5.0/etna/ensembles/mixins.py` & `etna-2.6.0/etna/ensembles/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pathlib
 import tempfile
 import zipfile
 from copy import deepcopy
 from typing import List
 from typing import Optional
+from typing import Union
 
 import pandas as pd
 from typing_extensions import Self
 
 from etna.core import SaveMixin
 from etna.core import load
 from etna.datasets import TSDataset
@@ -48,16 +49,16 @@
         tslogger.log(msg=f"Forecast is done with {pipeline}.")
         return forecast
 
     @staticmethod
     def _predict_pipeline(
         ts: TSDataset,
         pipeline: BasePipeline,
-        start_timestamp: Optional[pd.Timestamp],
-        end_timestamp: Optional[pd.Timestamp],
+        start_timestamp: Union[pd.Timestamp, int, str, None],
+        end_timestamp: Union[pd.Timestamp, int, str, None],
     ) -> TSDataset:
         """Make predict with given pipeline."""
         tslogger.log(msg=f"Start prediction with {pipeline}.")
         prediction = pipeline.predict(ts=ts, start_timestamp=start_timestamp, end_timestamp=end_timestamp)
         tslogger.log(msg=f"Prediction is done with {pipeline}.")
         return prediction
```

### Comparing `etna-2.5.0/etna/ensembles/stacking_ensemble.py` & `etna-2.6.0/etna/ensembles/stacking_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
     >>> from etna.ensembles import VotingEnsemble
     >>> from etna.models import NaiveModel
     >>> from etna.models import MovingAverageModel
     >>> from etna.pipeline import Pipeline
     >>> import pandas as pd
     >>> pd.options.display.float_format = '{:,.2f}'.format
     >>> df = generate_ar_df(periods=100, start_time="2021-06-01", ar_coef=[0.8], n_segments=3)
-    >>> df_ts_format = TSDataset.to_dataset(df)
-    >>> ts = TSDataset(df_ts_format, "D")
+    >>> ts = TSDataset(df, "D")
     >>> ma_pipeline = Pipeline(model=MovingAverageModel(window=5), transforms=[], horizon=7)
     >>> naive_pipeline = Pipeline(model=NaiveModel(lag=10), transforms=[], horizon=7)
     >>> ensemble = StackingEnsemble(pipelines=[ma_pipeline, naive_pipeline])
     >>> _ = ensemble.fit(ts=ts)
     >>> forecast = ensemble.forecast()
     >>> forecast[:,:,"target"]
     segment    segment_0 segment_1 segment_2
@@ -252,16 +251,16 @@
         )
         forecast = self._process_forecasts(ts=ts, forecasts=forecasts)
         return forecast
 
     def _predict(
         self,
         ts: TSDataset,
-        start_timestamp: pd.Timestamp,
-        end_timestamp: pd.Timestamp,
+        start_timestamp: Union[pd.Timestamp, int],
+        end_timestamp: Union[pd.Timestamp, int],
         prediction_interval: bool,
         quantiles: Sequence[float],
         return_components: bool,
     ) -> TSDataset:
         if prediction_interval:
             raise NotImplementedError(f"Ensemble {self.__class__.__name__} doesn't support prediction intervals!")
         if return_components:
```

### Comparing `etna-2.5.0/etna/ensembles/voting_ensemble.py` & `etna-2.6.0/etna/ensembles/voting_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     >>> from etna.datasets import generate_ar_df
     >>> from etna.datasets import TSDataset
     >>> from etna.ensembles import VotingEnsemble
     >>> from etna.models import NaiveModel
     >>> from etna.models import ProphetModel
     >>> from etna.pipeline import Pipeline
     >>> df = generate_ar_df(periods=30, start_time="2021-06-01", ar_coef=[1.2], n_segments=3)
-    >>> df_ts_format = TSDataset.to_dataset(df)
-    >>> ts = TSDataset(df_ts_format, "D")
+    >>> ts = TSDataset(df, "D")
     >>> prophet_pipeline = Pipeline(model=ProphetModel(), transforms=[], horizon=7)
     >>> naive_pipeline = Pipeline(model=NaiveModel(lag=10), transforms=[], horizon=7)
     >>> ensemble = VotingEnsemble(
     ...     pipelines=[prophet_pipeline, naive_pipeline],
     ...     weights=[0.7, 0.3]
     ... )
     >>> _ = ensemble.fit(ts=ts)
@@ -210,16 +209,16 @@
         )
         forecast = self._vote(forecasts=forecasts)
         return forecast
 
     def _predict(
         self,
         ts: TSDataset,
-        start_timestamp: pd.Timestamp,
-        end_timestamp: pd.Timestamp,
+        start_timestamp: Union[pd.Timestamp, int],
+        end_timestamp: Union[pd.Timestamp, int],
         prediction_interval: bool,
         quantiles: Sequence[float],
         return_components: bool,
     ) -> TSDataset:
         if prediction_interval:
             raise NotImplementedError(f"Ensemble {self.__class__.__name__} doesn't support prediction intervals!")
         if return_components:
```

### Comparing `etna-2.5.0/etna/experimental/change_points/regularization_search.py` & `etna-2.6.0/etna/experimental/change_points/regularization_search.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/base.py` & `etna-2.6.0/etna/experimental/classification/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/classification.py` & `etna-2.6.0/etna/experimental/classification/classification.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/feature_extraction/base.py` & `etna-2.6.0/etna/experimental/classification/feature_extraction/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/feature_extraction/tsfresh.py` & `etna-2.6.0/etna/experimental/classification/feature_extraction/tsfresh.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/feature_extraction/weasel.py` & `etna-2.6.0/etna/experimental/classification/feature_extraction/weasel.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/predictability.py` & `etna-2.6.0/etna/experimental/classification/predictability.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/classification/utils.py` & `etna-2.6.0/etna/experimental/classification/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/base.py` & `etna-2.6.0/etna/experimental/prediction_intervals/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/conformal.py` & `etna-2.6.0/etna/experimental/prediction_intervals/conformal.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/empirical.py` & `etna-2.6.0/etna/experimental/prediction_intervals/empirical.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/mixins.py` & `etna-2.6.0/etna/experimental/prediction_intervals/mixins.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/naive_variance.py` & `etna-2.6.0/etna/experimental/prediction_intervals/naive_variance.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/experimental/prediction_intervals/utils.py` & `etna-2.6.0/etna/experimental/prediction_intervals/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/pmdarima_utils/arima.py` & `etna-2.6.0/etna/libs/pmdarima_utils/arima.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/statsforecast/arima.py` & `etna-2.6.0/etna/libs/statsforecast/arima.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/tsfresh/defaults.py` & `etna-2.6.0/etna/libs/tsfresh/defaults.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/tsfresh/distribution.py` & `etna-2.6.0/etna/libs/tsfresh/distribution.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/tsfresh/relevance.py` & `etna-2.6.0/etna/libs/tsfresh/relevance.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/tsfresh/relevance.pyi` & `etna-2.6.0/etna/libs/tsfresh/relevance.pyi`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/libs/tsfresh/significance_tests.py` & `etna-2.6.0/etna/libs/tsfresh/significance_tests.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/loggers/__init__.py` & `etna-2.6.0/etna/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/loggers/base.py` & `etna-2.6.0/etna/loggers/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/loggers/console_logger.py` & `etna-2.6.0/etna/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/loggers/file_logger.py` & `etna-2.6.0/etna/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/loggers/wandb_logger.py` & `etna-2.6.0/etna/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/__init__.py` & `etna-2.6.0/etna/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/base.py` & `etna-2.6.0/etna/metrics/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/functional_metrics.py` & `etna-2.6.0/etna/metrics/functional_metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/intervals_metrics.py` & `etna-2.6.0/etna/metrics/intervals_metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/metrics.py` & `etna-2.6.0/etna/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/metrics/utils.py` & `etna-2.6.0/etna/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/__init__.py` & `etna-2.6.0/etna/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 >>> import pandas as pd
 >>> from etna.datasets import TSDataset, generate_ar_df
 >>> from etna.transforms import LagTransform
 >>> from etna.models import LinearPerSegmentModel
 >>>
 >>> df = generate_ar_df(periods=100, start_time="2021-01-01", ar_coef=[1/2], n_segments=2)
->>> ts = TSDataset(TSDataset.to_dataset(df), freq="D")
+>>> ts = TSDataset(df, freq="D")
 >>> lag_transform = LagTransform(in_column="target", lags=[3, 4, 5])
 >>> ts.fit_transform(transforms=[lag_transform])
 >>> future_ts = ts.make_future(future_steps=3, transforms=[lag_transform])
 >>> model = LinearPerSegmentModel()
 >>> model.fit(ts)
 LinearPerSegmentModel(fit_intercept = True, )
 >>> forecast_ts = model.forecast(future_ts)
```

### Comparing `etna-2.5.0/etna/models/autoarima.py` & `etna-2.6.0/etna/models/autoarima.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/base.py` & `etna-2.6.0/etna/models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/catboost.py` & `etna-2.6.0/etna/models/catboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,22 +187,21 @@
 
     Examples
     --------
     >>> from etna.datasets import generate_periodic_df
     >>> from etna.datasets import TSDataset
     >>> from etna.models import CatBoostPerSegmentModel
     >>> from etna.transforms import LagTransform
-    >>> classic_df = generate_periodic_df(
+    >>> df = generate_periodic_df(
     ...     periods=100,
     ...     start_time="2020-01-01",
     ...     n_segments=4,
     ...     period=7,
     ...     sigma=3
     ... )
-    >>> df = TSDataset.to_dataset(df=classic_df)
     >>> ts = TSDataset(df, freq="D")
     >>> horizon = 7
     >>> transforms = [
     ...     LagTransform(in_column="target", lags=[horizon, horizon+1, horizon+2])
     ... ]
     >>> ts.fit_transform(transforms=transforms)
     >>> future = ts.make_future(horizon, transforms=transforms)
@@ -327,22 +326,21 @@
 
     Examples
     --------
     >>> from etna.datasets import generate_periodic_df
     >>> from etna.datasets import TSDataset
     >>> from etna.models import CatBoostMultiSegmentModel
     >>> from etna.transforms import LagTransform
-    >>> classic_df = generate_periodic_df(
+    >>> df = generate_periodic_df(
     ...     periods=100,
     ...     start_time="2020-01-01",
     ...     n_segments=4,
     ...     period=7,
     ...     sigma=3
     ... )
-    >>> df = TSDataset.to_dataset(df=classic_df)
     >>> ts = TSDataset(df, freq="D")
     >>> horizon = 7
     >>> transforms = [
     ...     LagTransform(in_column="target", lags=[horizon, horizon+1, horizon+2])
     ... ]
     >>> ts.fit_transform(transforms=transforms)
     >>> future = ts.make_future(horizon, transforms=transforms)
```

### Comparing `etna-2.5.0/etna/models/deadline_ma.py` & `etna-2.6.0/etna/models/deadline_ma.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/decorators.py` & `etna-2.6.0/etna/models/decorators.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/holt_winters.py` & `etna-2.6.0/etna/models/holt_winters.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,26 @@
 
 import numpy as np
 import pandas as pd
 from scipy.special import inv_boxcox
 from statsmodels.tsa.holtwinters import ExponentialSmoothing
 from statsmodels.tsa.holtwinters.results import HoltWintersResultsWrapper
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.models.base import BaseAdapter
 from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import NonPredictionIntervalContextIgnorantModelMixin
 from etna.models.mixins import PerSegmentModelMixin
-from etna.models.utils import determine_freq
-from etna.models.utils import determine_num_steps
 from etna.models.utils import select_observations
 
+_DEFAULT_FREQ = object()
+
 
 class _HoltWintersAdapter(BaseAdapter):
     """
     Class for holding Holt-Winters' exponential smoothing model.
 
     Notes
     -----
@@ -193,17 +195,17 @@
         self.smoothing_seasonal = smoothing_seasonal
         self.damping_trend = damping_trend
         self.fit_kwargs = fit_kwargs
 
         self._model: Optional[ExponentialSmoothing] = None
         self._result: Optional[HoltWintersResultsWrapper] = None
 
-        self._first_train_timestamp: Optional[pd.Timestamp] = None
-        self._last_train_timestamp: Optional[pd.Timestamp] = None
-        self._train_freq: Optional[str] = None
+        self._first_train_timestamp: Union[pd.Timestamp, int, None] = None
+        self._last_train_timestamp: Union[pd.Timestamp, int, None] = None
+        self._train_freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
 
     def _check_not_used_columns(self, df: pd.DataFrame):
         columns = df.columns
         columns_not_used = set(columns).difference({"target", "timestamp"})
         if columns_not_used:
             warnings.warn(
                 message=f"This model doesn't work with exogenous features. "
@@ -223,17 +225,23 @@
         Returns
         -------
         :
             Fitted model
         """
         self._train_freq = determine_freq(timestamps=df["timestamp"])
         self._check_not_used_columns(df)
+        self._first_train_timestamp = df["timestamp"].min()
+        self._last_train_timestamp = df["timestamp"].max()
 
         targets = df["target"]
-        targets.index = df["timestamp"]
+        if pd.api.types.is_integer_dtype(df["timestamp"]):
+            # make index start with zero
+            targets.index = df["timestamp"] - self._first_train_timestamp
+        else:
+            targets.index = df["timestamp"]
 
         self._model = ExponentialSmoothing(
             endog=targets,
             trend=self.trend,
             damped_trend=self.damped_trend,
             seasonal=self.seasonal,
             seasonal_periods=self.seasonal_periods,
@@ -251,17 +259,14 @@
             smoothing_level=self.smoothing_level,
             smoothing_trend=self.smoothing_trend,
             smoothing_seasonal=self.smoothing_seasonal,
             damping_trend=self.damping_trend,
             **self.fit_kwargs,
         )
 
-        self._first_train_timestamp = targets.index.min()
-        self._last_train_timestamp = targets.index.max()
-
         return self
 
     def predict(self, df: pd.DataFrame) -> np.ndarray:
         """
         Compute predictions from a Holt-Winters' model.
 
         Parameters
@@ -273,15 +278,24 @@
         -------
         :
             Array with predictions
         """
         if self._result is None or self._model is None:
             raise ValueError("This model is not fitted! Fit the model before calling predict method!")
 
-        forecast = self._result.predict(start=df["timestamp"].min(), end=df["timestamp"].max())
+        start_timestamp = df["timestamp"].min()
+        end_timestamp = df["timestamp"].max()
+        start_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._train_freq
+        )
+        end_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._train_freq
+        )
+
+        forecast = self._result.predict(start=start_idx, end=end_idx)
         y_pred = forecast.values
         return y_pred
 
     def get_model(self) -> HoltWintersResultsWrapper:
         """Get :py:class:`statsmodels.tsa.holtwinters.results.HoltWintersResultsWrapper` model that was fitted inside etna class.
 
         Returns
@@ -325,15 +339,15 @@
         -------
         :
             dataframe with forecast components
         """
         model = self._model
         fit_result = self._result
 
-        if fit_result is None or model is None or self._train_freq is None:
+        if fit_result is None or model is None or self._train_freq is _DEFAULT_FREQ:
             raise ValueError("This model is not fitted!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
             raise NotImplementedError(
                 "This model can't make forecast decomposition on history data! "
                 "Use method predict for in-sample prediction decomposition."
             )
@@ -396,15 +410,15 @@
         -------
         :
             dataframe with prediction components
         """
         model = self._model
         fit_result = self._result
 
-        if fit_result is None or model is None or self._train_freq is None:
+        if fit_result is None or model is None or self._train_freq is _DEFAULT_FREQ:
             raise ValueError("This model is not fitted!")
 
         if df["timestamp"].min() < self._first_train_timestamp or df["timestamp"].max() > self._last_train_timestamp:
             raise NotImplementedError(
                 "This model can't make prediction decomposition on future out-of-sample data! "
                 "Use method forecast for future out-of-sample prediction decomposition."
             )
```

### Comparing `etna-2.5.0/etna/models/linear.py` & `etna-2.6.0/etna/models/linear.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/mixins.py` & `etna-2.6.0/etna/models/mixins.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/moving_average.py` & `etna-2.6.0/etna/models/moving_average.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/naive.py` & `etna-2.6.0/etna/models/naive.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/__init__.py` & `etna-2.6.0/etna/models/nn/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,8 +6,9 @@
     from etna.models.nn.deepstate.deepstate import DeepStateModel
     from etna.models.nn.mlp import MLPModel
     from etna.models.nn.nbeats import NBeatsGenericModel
     from etna.models.nn.nbeats import NBeatsInterpretableModel
     from etna.models.nn.patchts import PatchTSModel
     from etna.models.nn.rnn import RNNModel
     from etna.models.nn.tft import TFTModel
+    from etna.models.nn.tft_native import TFTNativeModel
     from etna.models.nn.utils import PytorchForecastingDatasetBuilder
```

### Comparing `etna-2.5.0/etna/models/nn/deepar.py` & `etna-2.6.0/etna/models/nn/deepar.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/deepar_native/deepar.py` & `etna-2.6.0/etna/models/nn/deepar_native/deepar.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,16 @@
         return loss, target, target_prediction
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterator[dict]:
         """Make samples from segment DataFrame."""
         segment = df["segment"].values[0]
         values_target = df["target"].values
         values_real = (
-            df.select_dtypes(include=[np.number])
+            df.drop(["segment", "timestamp"], axis=1)
+            .select_dtypes(include=[np.number])
             .assign(target_shifted=df["target"].shift(1))
             .drop(["target"], axis=1)
             .pipe(lambda x: x[["target_shifted"] + [i for i in x.columns if i != "target_shifted"]])
             .values
         )
 
         def _make(
```

### Comparing `etna-2.5.0/etna/models/nn/deepar_native/loss.py` & `etna-2.6.0/etna/models/nn/deepar_native/loss.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/deepstate/__init__.py` & `etna-2.6.0/etna/models/nn/deepstate/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/deepstate/deepstate.py` & `etna-2.6.0/etna/models/nn/deepstate/deepstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 class DeepStateBatch(TypedDict):
     """Batch specification for DeepStateModel."""
 
     encoder_real: Tensor  # (batch_size, seq_length, input_size)
     decoder_real: Tensor  # (batch_size, horizon, input_size)
     datetime_index: Tensor  # (batch_size, num_models , seq_length + horizon)
     encoder_target: Tensor  # (batch_size, seq_length, 1)
+    segment: Tensor  # (batch_size)
 
 
 class DeepStateNet(DeepBaseNet):
     """DeepState network."""
 
     def __init__(
         self,
```

### Comparing `etna-2.5.0/etna/models/nn/deepstate/linear_dynamic_system.py` & `etna-2.6.0/etna/models/nn/deepstate/linear_dynamic_system.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/deepstate/state_space_model.py` & `etna-2.6.0/etna/models/nn/deepstate/state_space_model.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/mlp.py` & `etna-2.6.0/etna/models/nn/mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
 
         output = self.mlp(decoder_real)
         loss = self.loss(output, decoder_target)
         return loss, decoder_target, output
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterable[dict]:
         """Make samples from segment DataFrame."""
-        values_real = (
-            df.select_dtypes(include=[np.number]).pipe(lambda x: x[[i for i in x.columns if i != "target"]]).values
-        )
+        values_real = df.drop(["target", "segment", "timestamp"], axis=1).select_dtypes(include=[np.number]).values
         values_target = df["target"].values
         segment = df["segment"].values[0]
 
         def _make(
             values_target: np.ndarray, values_real: np.ndarray, segment: str, start_idx: int, decoder_length: int
         ) -> Optional[dict]:
```

### Comparing `etna-2.5.0/etna/models/nn/nbeats/blocks.py` & `etna-2.6.0/etna/models/nn/nbeats/blocks.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/nbeats/metrics.py` & `etna-2.6.0/etna/models/nn/nbeats/metrics.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/nbeats/nbeats.py` & `etna-2.6.0/etna/models/nn/nbeats/nbeats.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/nbeats/nets.py` & `etna-2.6.0/etna/models/nn/nbeats/nets.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/nbeats/utils.py` & `etna-2.6.0/etna/models/nn/nbeats/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/nn/patchts.py` & `etna-2.6.0/etna/models/nn/patchts.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
         target_prediction = torch.unsqueeze(target_prediction, dim=2)
 
         loss = self.loss(target_prediction, decoder_target)
         return loss, decoder_target, target_prediction
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterator[dict]:
         """Make samples from segment DataFrame."""
-        values_real = df.select_dtypes(include=[np.number]).values
+        values_real = df.drop(["segment", "timestamp"], axis=1).select_dtypes(include=[np.number]).values
         values_target = df["target"].values
         segment = df["segment"].values[0]
 
         def _make(
             values_real: np.ndarray,
             values_target: np.ndarray,
             segment: str,
```

### Comparing `etna-2.5.0/etna/models/nn/rnn.py` & `etna-2.6.0/etna/models/nn/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,16 @@
 
         loss = self.loss(target_prediction, decoder_target)
         return loss, decoder_target, target_prediction
 
     def make_samples(self, df: pd.DataFrame, encoder_length: int, decoder_length: int) -> Iterator[dict]:
         """Make samples from segment DataFrame."""
         values_real = (
-            df.select_dtypes(include=[np.number])
+            df.drop(["segment", "timestamp"], axis=1)
+            .select_dtypes(include=[np.number])
             .assign(target_shifted=df["target"].shift(1))
             .drop(["target"], axis=1)
             .pipe(lambda x: x[["target_shifted"] + [i for i in x.columns if i != "target_shifted"]])
             .values
         )
         values_target = df["target"].values
         segment = df["segment"].values[0]
```

### Comparing `etna-2.5.0/etna/models/nn/tft.py` & `etna-2.6.0/etna/models/nn/tft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import warnings
 from typing import Any
 from typing import Dict
 from typing import Optional
 from typing import Sequence
 
 import pandas as pd
+from deprecated import deprecated
 
 from etna import SETTINGS
 from etna.datasets.tsdataset import TSDataset
 from etna.distributions import BaseDistribution
 from etna.distributions import FloatDistribution
 from etna.distributions import IntDistribution
 from etna.models.base import PredictionIntervalContextRequiredAbstractModel
@@ -23,14 +24,15 @@
     from pytorch_forecasting.metrics import MultiHorizonMetric
     from pytorch_forecasting.metrics import QuantileLoss
     from pytorch_forecasting.models import TemporalFusionTransformer
     from pytorch_lightning import LightningModule
     from pytorch_lightning import Trainer
 
 
+@deprecated(reason="TFTModel is deprecated. Use TFTNativeModel instead.", version="3.0")
 class TFTModel(
     _DeepCopyMixin, PytorchForecastingMixin, SavePytorchForecastingMixin, PredictionIntervalContextRequiredAbstractModel
 ):
     """Wrapper for :py:class:`pytorch_forecasting.models.temporal_fusion_transformer.TemporalFusionTransformer`.
 
     Note
     ----
```

### Comparing `etna-2.5.0/etna/models/nn/utils.py` & `etna-2.6.0/etna/models/nn/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 import pandas as pd
 from sklearn.preprocessing import RobustScaler
 from sklearn.preprocessing import StandardScaler
 
 from etna import SETTINGS
 from etna.core import BaseMixin
 from etna.datasets.tsdataset import TSDataset
+from etna.datasets.utils import determine_num_steps
+from etna.datasets.utils import timestamp_range
 from etna.loggers import tslogger
 from etna.models.base import log_decorator
-from etna.models.utils import determine_num_steps
 
 if SETTINGS.torch_required:
     import pytorch_lightning as pl
     from pytorch_forecasting.data import TimeSeriesDataSet
     from pytorch_forecasting.data.encoders import EncoderNormalizer
     from pytorch_forecasting.data.encoders import NaNLabelEncoder
     from pytorch_forecasting.data.encoders import TorchNormalizer
@@ -262,24 +263,24 @@
         self.model = self._from_dataset(pf_dataset_train)
         if self.trainer is not None and self.model is not None:
             self.trainer.fit(self.model, train_dataloader)
         else:
             raise ValueError("Trainer or model is None")
         return self
 
-    def _get_first_prediction_timestamp(self, ts: TSDataset, horizon: int) -> pd.Timestamp:
+    def _get_first_prediction_timestamp(self, ts: TSDataset, horizon: int) -> Union[pd.Timestamp, int]:
         return ts.index[-horizon]
 
     def _is_in_sample_prediction(self, ts: TSDataset, horizon: int) -> bool:
         first_prediction_timestamp = self._get_first_prediction_timestamp(ts=ts, horizon=horizon)
         return first_prediction_timestamp <= self._last_train_timestamp
 
     def _is_prediction_with_gap(self, ts: TSDataset, horizon: int) -> bool:
         first_prediction_timestamp = self._get_first_prediction_timestamp(ts=ts, horizon=horizon)
-        first_timestamp_after_train = pd.date_range(self._last_train_timestamp, periods=2, freq=self._freq)[-1]
+        first_timestamp_after_train = timestamp_range(start=self._last_train_timestamp, periods=2, freq=self._freq)[-1]
         return first_prediction_timestamp > first_timestamp_after_train
 
     def _make_target_prediction(self, ts: TSDataset, horizon: int) -> Tuple[TSDataset, DataLoader]:
         if self._is_in_sample_prediction(ts=ts, horizon=horizon):
             raise NotImplementedError(
                 "This model can't make forecast on history data! "
                 "In-sample forecast isn't supported by current implementation."
```

### Comparing `etna-2.5.0/etna/models/prophet.py` & `etna-2.6.0/etna/models/prophet.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Set
 from typing import Union
+from typing import cast
 
 import pandas as pd
 
 from etna import SETTINGS
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.distributions import FloatDistribution
@@ -46,14 +47,15 @@
         holidays_prior_scale: float = 10.0,
         changepoint_prior_scale: float = 0.05,
         mcmc_samples: int = 0,
         interval_width: float = 0.8,
         uncertainty_samples: Union[int, bool] = 1000,
         stan_backend: Optional[str] = None,
         additional_seasonality_params: Iterable[Dict[str, Union[str, float, int]]] = (),
+        timestamp_column: Optional[str] = None,
     ):
 
         self.growth = growth
         self.n_changepoints = n_changepoints
         self.changepoints = changepoints
         self.changepoint_range = changepoint_range
         self.yearly_seasonality = yearly_seasonality
@@ -65,14 +67,15 @@
         self.holidays_prior_scale = holidays_prior_scale
         self.changepoint_prior_scale = changepoint_prior_scale
         self.mcmc_samples = mcmc_samples
         self.interval_width = interval_width
         self.uncertainty_samples = uncertainty_samples
         self.stan_backend = stan_backend
         self.additional_seasonality_params = additional_seasonality_params
+        self.timestamp_column = timestamp_column
 
         self.model = self._create_model()
 
         self.regressor_columns: Optional[List[str]] = None
 
     def _create_model(self) -> "Prophet":
         model = Prophet(
@@ -127,16 +130,20 @@
         if regressors_with_nans:
             raise ValueError(
                 f"Regressors {regressors_with_nans} contain NaN values. "
                 "Try to lower horizon value, or drop these regressors."
             )
 
         if self.regressor_columns:
+            columns = deepcopy(self.regressor_columns)
+            if self.timestamp_column in columns:
+                columns.remove(self.timestamp_column)
+
             try:
-                result = df[self.regressor_columns].apply(pd.to_numeric)
+                result = df[columns].apply(pd.to_numeric)
             except ValueError as e:
                 raise ValueError(f"Only convertible to numeric features are allowed! Error: {str(e)}")
         else:
             result = None
 
         return result
 
@@ -152,16 +159,19 @@
             List of the columns with regressors
         """
         self.regressor_columns = regressors
         self._check_not_used_columns(df)
 
         prophet_df = self._prepare_prophet_df(df=df)
         for regressor in self.regressor_columns:
-            if regressor not in self.predefined_regressors_names:
-                self.model.add_regressor(regressor)
+            if regressor in self.predefined_regressors_names:
+                continue
+            if regressor == self.timestamp_column:
+                continue
+            self.model.add_regressor(regressor)
         self.model.fit(prophet_df)
         return self
 
     def predict(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float]) -> pd.DataFrame:
         """
         Compute predictions from a Prophet model.
 
@@ -189,28 +199,50 @@
                 y_pred[f"yhat_{quantile:.4g}"] = self.model.percentile(sim_values["yhat"], percentile, axis=1)
         rename_dict = {
             column: column.replace("yhat", "target") for column in y_pred.columns if column.startswith("yhat")
         }
         y_pred = y_pred.rename(rename_dict, axis=1)
         return y_pred
 
+    def _validate_timestamp(self, df: pd.DataFrame):
+        self.regressor_columns = cast(List[str], self.regressor_columns)
+
+        if self.timestamp_column is None:
+            if not pd.api.types.is_datetime64_dtype(df["timestamp"]):
+                raise ValueError("Invalid timestamp! Only datetime type is supported.")
+
+        else:
+            if self.timestamp_column not in df.columns:
+                raise ValueError("Invalid timestamp_column! It isn't present in a given dataset.")
+
+            if self.timestamp_column not in self.regressor_columns:
+                raise ValueError("Invalid timestamp_column! It should be a regressor.")
+
+            if not pd.api.types.is_datetime64_dtype(df[self.timestamp_column]):
+                raise ValueError("Invalid timestamp_column! Only datetime type is supported.")
+
     def _prepare_prophet_df(self, df: pd.DataFrame) -> pd.DataFrame:
         """Prepare dataframe for fit and predict."""
         if self.regressor_columns is None:
             raise ValueError("List of regressor is not set!")
 
+        self._validate_timestamp(df)
         df = df.reset_index()
 
         prophet_df = pd.DataFrame()
         prophet_df["y"] = df["target"]
-        prophet_df["ds"] = df["timestamp"]
+
+        if self.timestamp_column is None:
+            prophet_df["ds"] = df["timestamp"]
+        else:
+            prophet_df["ds"] = df[self.timestamp_column]
 
         regressors_data = self._select_regressors(df)
         if regressors_data is not None:
-            prophet_df[self.regressor_columns] = regressors_data[self.regressor_columns]
+            prophet_df[regressors_data.columns] = regressors_data
 
         return prophet_df
 
     @staticmethod
     def _filter_aggregated_components(components: Iterable[str]) -> Set[str]:
         """Filter out aggregated components."""
         # aggregation of corresponding model terms, e.g. sum
@@ -337,32 +369,31 @@
     if fitted. Corresponding components are obtained directly from the model.
 
     Examples
     --------
     >>> from etna.datasets import generate_periodic_df
     >>> from etna.datasets import TSDataset
     >>> from etna.models import ProphetModel
-    >>> classic_df = generate_periodic_df(
+    >>> df = generate_periodic_df(
     ...     periods=100,
     ...     start_time="2020-01-01",
     ...     n_segments=4,
     ...     period=7,
     ...     sigma=3
     ... )
-    >>> df = TSDataset.to_dataset(df=classic_df)
     >>> ts = TSDataset(df, freq="D")
     >>> future = ts.make_future(7)
     >>> model = ProphetModel(growth="flat")
     >>> model.fit(ts=ts)
     ProphetModel(growth = 'flat', changepoints = None, n_changepoints = 25,
     changepoint_range = 0.8, yearly_seasonality = 'auto', weekly_seasonality = 'auto',
     daily_seasonality = 'auto', holidays = None, seasonality_mode = 'additive',
     seasonality_prior_scale = 10.0, holidays_prior_scale = 10.0, changepoint_prior_scale = 0.05,
     mcmc_samples = 0, interval_width = 0.8, uncertainty_samples = 1000, stan_backend = None,
-    additional_seasonality_params = (), )
+    additional_seasonality_params = (), timestamp_column = None, )
     >>> forecast = model.forecast(future)
     >>> forecast
     segment    segment_0 segment_1 segment_2 segment_3
     feature       target    target    target    target
     timestamp
     2020-04-10      9.00      9.00      4.00      6.00
     2020-04-11      5.00      2.00      7.00      9.00
@@ -388,14 +419,15 @@
         holidays_prior_scale: float = 10.0,
         changepoint_prior_scale: float = 0.05,
         mcmc_samples: int = 0,
         interval_width: float = 0.8,
         uncertainty_samples: Union[int, bool] = 1000,
         stan_backend: Optional[str] = None,
         additional_seasonality_params: Iterable[Dict[str, Union[str, float, int]]] = (),
+        timestamp_column: Optional[str] = None,
     ):
         """
         Create instance of Prophet model.
 
         Parameters
         ----------
         growth:
@@ -463,14 +495,17 @@
         stan_backend:
             as defined in StanBackendEnum default: None - will try to
             iterate over all available backends and find the working one
         additional_seasonality_params: Iterable[Dict[str, Union[int, float, str]]]
             parameters that describe additional (not 'daily', 'weekly', 'yearly') seasonality that should be
             added to model; dict with required keys 'name', 'period', 'fourier_order' and optional ones 'prior_scale',
             'mode', 'condition_name' will be used for :py:meth:`prophet.Prophet.add_seasonality` method call.
+        timestamp_column:
+            Name of a column to be used as timestamp. If not given, index is used.
+            Column is expected to be regressor containing datetime values.
         """
         self.growth = growth
         self.n_changepoints = n_changepoints
         self.changepoints = changepoints
         self.changepoint_range = changepoint_range
         self.yearly_seasonality = yearly_seasonality
         self.weekly_seasonality = weekly_seasonality
@@ -481,14 +516,15 @@
         self.holidays_prior_scale = holidays_prior_scale
         self.changepoint_prior_scale = changepoint_prior_scale
         self.mcmc_samples = mcmc_samples
         self.interval_width = interval_width
         self.uncertainty_samples = uncertainty_samples
         self.stan_backend = stan_backend
         self.additional_seasonality_params = additional_seasonality_params
+        self.timestamp_column = timestamp_column
 
         super(ProphetModel, self).__init__(
             base_model=_ProphetAdapter(
                 growth=self.growth,
                 n_changepoints=self.n_changepoints,
                 changepoints=self.changepoints,
                 changepoint_range=self.changepoint_range,
@@ -501,14 +537,15 @@
                 holidays_prior_scale=self.holidays_prior_scale,
                 changepoint_prior_scale=self.changepoint_prior_scale,
                 mcmc_samples=self.mcmc_samples,
                 interval_width=self.interval_width,
                 uncertainty_samples=self.uncertainty_samples,
                 stan_backend=self.stan_backend,
                 additional_seasonality_params=self.additional_seasonality_params,
+                timestamp_column=self.timestamp_column,
             )
         )
 
     def params_to_tune(self) -> Dict[str, BaseDistribution]:
         """Get default grid for tuning hyperparameters.
 
         This grid tunes parameters: ``seasonality_mode``, ``seasonality_prior_scale``, ``changepoint_prior_scale``,
```

### Comparing `etna-2.5.0/etna/models/sarimax.py` & `etna-2.6.0/etna/models/sarimax.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,41 +11,43 @@
 import numpy as np
 import pandas as pd
 from statsmodels.tools.sm_exceptions import ValueWarning
 from statsmodels.tsa.statespace.sarimax import SARIMAX
 from statsmodels.tsa.statespace.sarimax import SARIMAXResultsWrapper
 from statsmodels.tsa.statespace.simulation_smoother import SimulationSmoother
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.distributions import IntDistribution
 from etna.libs.pmdarima_utils import seasonal_prediction_with_confidence
 from etna.models.base import BaseAdapter
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
-from etna.models.utils import determine_freq
-from etna.models.utils import determine_num_steps
 from etna.models.utils import select_observations
 
 warnings.filterwarnings(
     message="No frequency information was provided, so inferred frequency .* will be used",
     action="ignore",
     category=ValueWarning,
     module="statsmodels.tsa.base.tsa_model",
 )
 
+_DEFAULT_FREQ = object()
+
 
 class _SARIMAXBaseAdapter(BaseAdapter):
     """Base class for adapters based on :py:class:`statsmodels.tsa.statespace.sarimax.SARIMAX`."""
 
     def __init__(self):
         self.regressor_columns = None
         self._fit_results = None
-        self._freq = None
+        self._freq: Union[str, None] = _DEFAULT_FREQ  # type: ignore
         self._first_train_timestamp = None
         self._last_train_timestamp = None
 
     def fit(self, df: pd.DataFrame, regressors: List[str]) -> "_SARIMAXBaseAdapter":
         """
         Fits a SARIMAX model.
 
@@ -60,20 +62,21 @@
         -------
         :
             Fitted model
         """
         self.regressor_columns = regressors
         self._check_not_used_columns(df)
 
+        self._first_train_timestamp = df["timestamp"].min()
+        self._last_train_timestamp = df["timestamp"].max()
+
         exog_train = self._select_regressors(df)
         self._fit_results = self._get_fit_results(endog=df["target"], exog=exog_train)
 
         self._freq = determine_freq(timestamps=df["timestamp"])
-        self._first_train_timestamp = df["timestamp"].min()
-        self._last_train_timestamp = df["timestamp"].max()
 
         return self
 
     def _make_prediction(
         self, df: pd.DataFrame, prediction_interval: bool, quantiles: Sequence[float], dynamic: bool
     ) -> pd.DataFrame:
         """Make predictions taking into account ``dynamic`` parameter."""
@@ -82,19 +85,19 @@
 
         exog_future = self._select_regressors(df)
 
         start_timestamp = df["timestamp"].min()
         end_timestamp = df["timestamp"].max()
         # determine index of start_timestamp if counting from first timestamp of train
         start_idx = determine_num_steps(
-            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq
         )
         # determine index of end_timestamp if counting from first timestamp of train
         end_idx = determine_num_steps(
-            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq
         )
 
         if prediction_interval:
             forecast, _ = seasonal_prediction_with_confidence(
                 arima_res=self._fit_results, start=start_idx, end=end_idx, X=exog_future, alpha=0.05, dynamic=dynamic
             )
             y_pred = pd.DataFrame({"mean": forecast})
@@ -202,15 +205,20 @@
             )
 
         if self.regressor_columns:
             try:
                 result = df[self.regressor_columns].astype(float)
             except ValueError as e:
                 raise ValueError(f"Only convertible to float features are allowed! Error: {str(e)}")
-            result.index = df["timestamp"]
+
+            if pd.api.types.is_integer_dtype(df["timestamp"]):
+                # make index start with zero
+                result.index = df["timestamp"] - self._first_train_timestamp
+            else:
+                result.index = df["timestamp"]
         else:
             result = None
 
         return result
 
     def get_model(self) -> SARIMAXResultsWrapper:
         """Get :py:class:`statsmodels.tsa.statespace.sarimax.SARIMAXResultsWrapper` that is used inside etna class.
@@ -366,19 +374,19 @@
             raise NotImplementedError(
                 "This model can't make forecast decomposition on history data! "
                 "Use method predict for in-sample prediction decomposition."
             )
 
         # determine index of start_timestamp if counting from last timestamp of train
         start_idx = determine_num_steps(
-            start_timestamp=self._last_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._last_train_timestamp, end_timestamp=start_timestamp, freq=self._freq
         )
         # determine index of end_timestamp if counting from last timestamp of train
         end_idx = determine_num_steps(
-            start_timestamp=self._last_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._last_train_timestamp, end_timestamp=end_timestamp, freq=self._freq
         )
 
         if start_idx > 1:
             raise NotImplementedError(
                 "This model can't make forecast decomposition on out-of-sample data that goes after training data with a gap! "
                 "You can only forecast from the next point after the last one in the training dataset."
             )
```

### Comparing `etna-2.5.0/etna/models/seasonal_ma.py` & `etna-2.6.0/etna/models/seasonal_ma.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/sklearn.py` & `etna-2.6.0/etna/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/models/statsforecast.py` & `etna-2.6.0/etna/models/statsforecast.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 import numpy as np
 import pandas as pd
 from statsforecast.models import AutoARIMA
 from statsforecast.models import AutoCES
 from statsforecast.models import AutoETS
 from statsforecast.models import AutoTheta
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
 from etna.distributions import BaseDistribution
 from etna.distributions import IntDistribution
 from etna.libs.statsforecast import ARIMA
 from etna.models.base import BaseAdapter
 from etna.models.base import NonPredictionIntervalContextIgnorantAbstractModel
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import NonPredictionIntervalContextIgnorantModelMixin
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
-from etna.models.utils import determine_freq
-from etna.models.utils import determine_num_steps
 
 StatsForecastModel = Union[AutoCES, AutoARIMA, AutoTheta, AutoETS, ARIMA]
+_DEFAULT_FREQ = object()
 
 
 class _StatsForecastBaseAdapter(BaseAdapter):
     """Base class for adapters for models from statsforecast package."""
 
     def __init__(self, model: StatsForecastModel, support_prediction_intervals: bool):
         """
@@ -39,15 +40,15 @@
         ----------
         model:
             Model from statsforecast.
         support_prediction_intervals:
             Should model support prediction intervals.
         """
         self.regressor_columns: Optional[List[str]] = None
-        self._freq: Optional[str] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
         self._first_train_timestamp: Optional[pd.Timestamp] = None
         self._last_train_timestamp: Optional[pd.Timestamp] = None
         self._model = model
         self._support_prediction_intervals = support_prediction_intervals
 
     def _check_not_used_columns(self, df: pd.DataFrame):
         if self.regressor_columns is None:
@@ -136,32 +137,32 @@
             Levels of prediction distribution
 
         Returns
         -------
         :
             DataFrame with predictions
         """
-        if self._freq is None:
+        if self._freq is _DEFAULT_FREQ:
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
         start_timestamp = df["timestamp"].min()
         end_timestamp = df["timestamp"].max()
 
         if start_timestamp < self._last_train_timestamp:
             raise NotImplementedError(
                 "This model can't make forecast on history data! Use method predict for in-sample prediction."
             )
 
         # determine index of start_timestamp if counting from last timestamp of train
         start_idx = determine_num_steps(
-            start_timestamp=self._last_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._last_train_timestamp, end_timestamp=start_timestamp, freq=self._freq
         )
         # determine index of end_timestamp if counting from last timestamp of train
         end_idx = determine_num_steps(
-            start_timestamp=self._last_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._last_train_timestamp, end_timestamp=end_timestamp, freq=self._freq
         )
 
         if start_idx > 1:
             raise NotImplementedError(
                 "This model can't make forecast on out-of-sample data that goes after training data with a gap! "
                 "You can only forecast from the next point after the last one in the training dataset."
             )
@@ -209,15 +210,15 @@
             Levels of prediction distribution
 
         Returns
         -------
         :
             DataFrame with predictions
         """
-        if self._freq is None:
+        if self._freq is _DEFAULT_FREQ:
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
         start_timestamp = df["timestamp"].min()
         end_timestamp = df["timestamp"].max()
 
         if start_timestamp < self._first_train_timestamp:
             raise NotImplementedError(
@@ -228,19 +229,19 @@
             raise NotImplementedError(
                 "This model can't make predict on future out-of-sample data! "
                 "Use forecast method for this type of prediction."
             )
 
         # determine index of start_timestamp if counting from first timestamp of train
         start_idx = determine_num_steps(
-            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq
         )
         # determine index of end_timestamp if counting from first timestamp of train
         end_idx = determine_num_steps(
-            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq  # type: ignore
+            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq
         )
 
         if prediction_interval and self._support_prediction_intervals:
             levels = []
             for quantile in quantiles:
                 width = abs(1 / 2 - quantile) * 2
                 level = int(width * 100)
```

### Comparing `etna-2.5.0/etna/models/tbats.py` & `etna-2.6.0/etna/models/tbats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from typing import Iterable
 from typing import Optional
 from typing import Tuple
+from typing import Union
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 from tbats.abstract import ContextInterface
 from tbats.abstract import Estimator
 from tbats.bats import BATS
 from tbats.tbats import TBATS
 from tbats.tbats.Model import Model
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
+from etna.datasets.utils import timestamp_range
 from etna.models.base import BaseAdapter
 from etna.models.base import PredictionIntervalContextIgnorantAbstractModel
 from etna.models.mixins import PerSegmentModelMixin
 from etna.models.mixins import PredictionIntervalContextIgnorantModelMixin
-from etna.models.utils import determine_freq
-from etna.models.utils import determine_num_steps
 from etna.models.utils import select_observations
 
+_DEFAULT_FREQ = object()
+
 
 class _TBATSAdapter(BaseAdapter):
     def __init__(self, model: Estimator):
         self._model = model
         self._fitted_model: Optional[Model] = None
         self._first_train_timestamp = None
         self._last_train_timestamp = None
-        self._freq: Optional[str] = None
+        self._freq: Union[str, None] = _DEFAULT_FREQ  # type: ignore
 
     def _check_not_used_columns(self, df: pd.DataFrame):
         columns = df.columns
         columns_not_used = set(columns).difference({"target", "timestamp"})
         if columns_not_used:
             warn(
                 message=f"This model doesn't work with exogenous features. "
@@ -45,15 +49,15 @@
         self._fitted_model = self._model.fit(target)
         self._first_train_timestamp = df["timestamp"].min()
         self._last_train_timestamp = df["timestamp"].max()
 
         return self
 
     def forecast(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Iterable[float]) -> pd.DataFrame:
-        if self._fitted_model is None or self._freq is None:
+        if self._fitted_model is None or self._freq is _DEFAULT_FREQ:
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
         steps_to_forecast = self._get_steps_to_forecast(df=df)
         steps_to_skip = steps_to_forecast - df.shape[0]
 
         y_pred = pd.DataFrame()
         if prediction_interval:
@@ -72,19 +76,19 @@
 
         # skip non-relevant timestamps
         y_pred = y_pred.iloc[steps_to_skip:].reset_index(drop=True)
 
         return y_pred
 
     def predict(self, df: pd.DataFrame, prediction_interval: bool, quantiles: Iterable[float]) -> pd.DataFrame:
-        if self._fitted_model is None or self._freq is None:
+        if self._fitted_model is None or self._freq is _DEFAULT_FREQ or self._last_train_timestamp is None:
             raise ValueError("Model is not fitted! Fit the model before calling predict method!")
 
-        train_timestamp = pd.date_range(
-            start=str(self._first_train_timestamp), end=str(self._last_train_timestamp), freq=self._freq
+        train_timestamp = timestamp_range(
+            start=self._first_train_timestamp, end=self._last_train_timestamp, freq=self._freq
         )
 
         if not (set(df["timestamp"]) <= set(train_timestamp)):
             raise NotImplementedError(
                 "This model can't make predict on future out-of-sample data! "
                 "Use forecast method for this type of prediction."
             )
@@ -130,15 +134,15 @@
             features dataframe
 
         Returns
         -------
         :
             dataframe with forecast components
         """
-        if self._fitted_model is None or self._freq is None:
+        if self._fitted_model is None or self._freq is _DEFAULT_FREQ:
             raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
             raise NotImplementedError(
                 "This model can't make forecast decomposition on history data! "
                 "Use method predict for in-sample prediction decomposition."
             )
@@ -164,15 +168,15 @@
             features dataframe
 
         Returns
         -------
         :
             dataframe with prediction components
         """
-        if self._fitted_model is None or self._freq is None:
+        if self._fitted_model is None or self._freq is _DEFAULT_FREQ:
             raise ValueError("Model is not fitted! Fit the model before estimating forecast components!")
 
         if self._last_train_timestamp < df["timestamp"].max() or self._first_train_timestamp > df["timestamp"].min():
             raise NotImplementedError(
                 "This model can't make prediction decomposition on future out-of-sample data! "
                 "Use method forecast for future out-of-sample prediction decomposition."
             )
@@ -189,15 +193,15 @@
             end=self._last_train_timestamp,
             freq=self._freq,
         )
 
         return components
 
     def _get_steps_to_forecast(self, df: pd.DataFrame) -> int:
-        if self._freq is None:
+        if self._freq is _DEFAULT_FREQ:
             raise ValueError("Data frequency is not set!")
 
         if df["timestamp"].min() <= self._last_train_timestamp:
             raise NotImplementedError(
                 "This model can't make forecast on history data! Use method predict for in-sample prediction."
             )
```

### Comparing `etna-2.5.0/etna/pipeline/assembling_pipelines.py` & `etna-2.6.0/etna/pipeline/assembling_pipelines.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     >>> from etna.transforms import DateFlagsTransform, AddConstTransform, LagTransform
     >>> assemble_pipelines(models=LinearPerSegmentModel(), transforms=[LagTransform(in_column='target', lags=[1]), AddConstTransform(in_column='target', value=1)], horizons=[1,2,3])
     [Pipeline(model = LinearPerSegmentModel(fit_intercept = True, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), AddConstTransform(in_column = 'target', value = 1, inplace = True, out_column = None, )], horizon = 1, ),
     Pipeline(model = LinearPerSegmentModel(fit_intercept = True, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), AddConstTransform(in_column = 'target', value = 1, inplace = True, out_column = None, )], horizon = 2, ),
     Pipeline(model = LinearPerSegmentModel(fit_intercept = True, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), AddConstTransform(in_column = 'target', value = 1, inplace = True, out_column = None, )], horizon = 3, )]
     >>> assemble_pipelines(models=[LinearPerSegmentModel(), NaiveModel()], transforms=[LagTransform(in_column='target', lags=[1]), [AddConstTransform(in_column='target', value=1), DateFlagsTransform()]], horizons=[1,2])
     [Pipeline(model = LinearPerSegmentModel(fit_intercept = True, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), AddConstTransform(in_column = 'target', value = 1, inplace = True, out_column = None, )], horizon = 1, ),
-    Pipeline(model = NaiveModel(lag = 1, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), DateFlagsTransform(day_number_in_week = True, day_number_in_month = True, day_number_in_year = False, week_number_in_month = False, week_number_in_year = False, month_number_in_year = False, season_number = False, year_number = False, is_weekend = True, special_days_in_week = (), special_days_in_month = (), out_column = None, )], horizon = 2, )]
+    Pipeline(model = NaiveModel(lag = 1, ), transforms = [LagTransform(in_column = 'target', lags = [1], out_column = None, ), DateFlagsTransform(day_number_in_week = True, day_number_in_month = True, day_number_in_year = False, week_number_in_month = False, week_number_in_year = False, month_number_in_year = False, season_number = False, year_number = False, is_weekend = True, special_days_in_week = (), special_days_in_month = (), out_column = None, in_column = None, )], horizon = 2, )]
     """
     n_models = len(models) if isinstance(models, Sequence) else 1
     n_horizons = len(horizons) if isinstance(horizons, Sequence) else 1
     n_transforms = 1
 
     for transform_item in transforms:
         if isinstance(transform_item, Sequence):
```

### Comparing `etna-2.5.0/etna/pipeline/autoregressive_pipeline.py` & `etna-2.6.0/etna/pipeline/autoregressive_pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Sequence
 from typing import cast
 
 import pandas as pd
 from typing_extensions import get_args
 
 from etna.datasets import TSDataset
+from etna.datasets.utils import timestamp_range
 from etna.models.base import ContextIgnorantModelType
 from etna.models.base import ContextRequiredModelType
 from etna.models.base import ModelType
 from etna.pipeline.base import BasePipeline
 from etna.pipeline.mixins import ModelPipelineParamsToTuneMixin
 from etna.pipeline.mixins import ModelPipelinePredictMixin
 from etna.pipeline.mixins import SaveModelPipelineMixin
@@ -23,22 +24,21 @@
 
     Examples
     --------
     >>> from etna.datasets import generate_periodic_df
     >>> from etna.datasets import TSDataset
     >>> from etna.models import LinearPerSegmentModel
     >>> from etna.transforms import LagTransform
-    >>> classic_df = generate_periodic_df(
+    >>> df = generate_periodic_df(
     ...     periods=100,
     ...     start_time="2020-01-01",
     ...     n_segments=4,
     ...     period=7,
     ...     sigma=3
     ... )
-    >>> df = TSDataset.to_dataset(df=classic_df)
     >>> ts = TSDataset(df, freq="D")
     >>> horizon = 7
     >>> transforms = [
     ...     LagTransform(in_column="target", lags=list(range(1, horizon+1)))
     ... ]
     >>> model = LinearPerSegmentModel()
     >>> pipeline = AutoRegressivePipeline(model, horizon, transforms, step=1)
@@ -102,20 +102,21 @@
         if save_ts:
             self.ts = ts
 
         return self
 
     def _create_predictions_template(self, ts: TSDataset) -> pd.DataFrame:
         """Create dataframe to fill with forecasts."""
-        prediction_df = ts[:, :, "target"]
-        future_dates = pd.date_range(
-            start=prediction_df.index.max(), periods=self.horizon + 1, freq=ts.freq, closed="right"
-        )
-        prediction_df = prediction_df.reindex(prediction_df.index.append(future_dates))
-        prediction_df.index.name = "timestamp"
+        prediction_df = ts.to_pandas(features=["target"])
+        last_timestamp = prediction_df.index[-1]
+        to_add_index = timestamp_range(start=last_timestamp, periods=self.horizon + 1, freq=ts.freq)[1:]
+        new_index = prediction_df.index.append(to_add_index)
+        index_name = prediction_df.index.name
+        prediction_df = prediction_df.reindex(new_index)
+        prediction_df.index.name = index_name
         return prediction_df
 
     def _forecast(self, ts: TSDataset, return_components: bool) -> TSDataset:
         """Make predictions."""
         prediction_df = self._create_predictions_template(ts)
 
         target_components_dfs = []
@@ -168,25 +169,7 @@
         prediction_ts.raw_df = prediction_ts.raw_df.tail(self.horizon)
 
         if return_components:
             target_components_df = pd.concat(target_components_dfs)
             prediction_ts.add_target_components(target_components_df=target_components_df)
 
         return prediction_ts
-
-    def _predict(
-        self,
-        ts: TSDataset,
-        start_timestamp: pd.Timestamp,
-        end_timestamp: pd.Timestamp,
-        prediction_interval: bool,
-        quantiles: Sequence[float],
-        return_components: bool = False,
-    ) -> TSDataset:
-        return super()._predict(
-            ts=ts,
-            start_timestamp=start_timestamp,
-            end_timestamp=end_timestamp,
-            prediction_interval=prediction_interval,
-            quantiles=quantiles,
-            return_components=return_components,
-        )
```

### Comparing `etna-2.5.0/etna/pipeline/base.py` & `etna-2.6.0/etna/pipeline/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import math
+import reprlib
 import warnings
 from abc import abstractmethod
 from copy import deepcopy
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Set
 from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from joblib import Parallel
 from joblib import delayed
 from scipy.stats import norm
 from typing_extensions import TypedDict
 from typing_extensions import assert_never
 
 from etna.core import AbstractSaveable
 from etna.core import BaseMixin
 from etna.datasets import TSDataset
+from etna.datasets.utils import _check_timestamp_param
+from etna.datasets.utils import timestamp_range
 from etna.distributions import BaseDistribution
 from etna.loggers import tslogger
 from etna.metrics import Metric
 from etna.metrics import MetricAggregationMode
 from etna.metrics.functional_metrics import ArrayLike
 
-Timestamp = Union[str, pd.Timestamp]
-
 
 class CrossValidationMode(str, Enum):
     """Enum for different cross-validation modes."""
 
     expand = "expand"
     constant = "constant"
 
@@ -49,79 +51,170 @@
     """Container to hold the description of the fold mask.
 
     Fold masks are expected to be used for backtest strategy customization.
     """
 
     def __init__(
         self,
-        first_train_timestamp: Optional[Timestamp],
-        last_train_timestamp: Timestamp,
-        target_timestamps: List[Timestamp],
+        first_train_timestamp: Union[pd.Timestamp, int, str, None],
+        last_train_timestamp: Union[pd.Timestamp, int, str],
+        target_timestamps: List[Union[pd.Timestamp, int, str]],
     ):
         """Init FoldMask.
 
+        Values of ``target_timestamps`` are sorted in ascending order.
+
+        Notes
+        -----
+        String value is converted into :py:class`pd.Timestamps` using :py:func:`pandas.to_datetime`.
+
         Parameters
         ----------
         first_train_timestamp:
             First train timestamp, the first timestamp in the dataset if None is passed
         last_train_timestamp:
             Last train timestamp
         target_timestamps:
             List of target timestamps
+
+        Raises
+        ------
+        ValueError:
+            All timestamps should be one of two possible types: pd.Timestamp or int
+        ValueError:
+            Last train timestamp should be not sooner than first train timestamp
+        ValueError:
+            Target timestamps shouldn't be empty
+        ValueError:
+            Target timestamps shouldn't contain duplicates
+        ValueError:
+            Target timestamps should be strictly later then last train timestamp
         """
-        self.first_train_timestamp = pd.to_datetime(first_train_timestamp) if first_train_timestamp else None
-        self.last_train_timestamp = pd.to_datetime(last_train_timestamp)
-        self.target_timestamps = sorted([pd.to_datetime(timestamp) for timestamp in target_timestamps])
-
-        self._validate_last_train_timestamp()
-        self._validate_target_timestamps()
-
-    def _validate_last_train_timestamp(self):
-        """Check that last train timestamp is later then first train timestamp."""
-        if self.first_train_timestamp and self.last_train_timestamp < self.first_train_timestamp:
+        if isinstance(first_train_timestamp, str):
+            first_train_timestamp = pd.to_datetime(first_train_timestamp)
+
+        if isinstance(last_train_timestamp, str):
+            last_train_timestamp = pd.to_datetime(last_train_timestamp)
+
+        target_timestamps_processed = []
+        for timestamp in target_timestamps:
+            if isinstance(timestamp, str):
+                target_timestamps_processed.append(pd.to_datetime(timestamp))
+            else:
+                target_timestamps_processed.append(timestamp)
+
+        self._validate_parameters_same_type(
+            first_train_timestamp=first_train_timestamp,
+            last_train_timestamp=last_train_timestamp,
+            target_timestamps=target_timestamps_processed,
+        )
+
+        target_timestamps = sorted(target_timestamps_processed)
+
+        self._validate_first_last_train_timestamps_order(
+            first_train_timestamp=first_train_timestamp, last_train_timestamp=last_train_timestamp
+        )
+        self._validate_target_timestamps(last_train_timestamp=last_train_timestamp, target_timestamps=target_timestamps)
+
+        self.first_train_timestamp = first_train_timestamp
+        self.last_train_timestamp = last_train_timestamp
+        self.target_timestamps = target_timestamps
+
+    @staticmethod
+    def _validate_parameters_same_type(
+        first_train_timestamp: Union[pd.Timestamp, int, str, None],
+        last_train_timestamp: Union[pd.Timestamp, int],
+        target_timestamps: List[Union[pd.Timestamp, int]],
+    ):
+        """Check that first train timestamp, last train timestamp, target timestamps has the same type."""
+        if first_train_timestamp is not None:
+            values_to_check = [first_train_timestamp, last_train_timestamp, *target_timestamps]
+        else:
+            values_to_check = [last_train_timestamp, *target_timestamps]
+
+        types: Set[type] = set()
+        for value in values_to_check:
+            if isinstance(value, np.integer):
+                types.add(int)
+            else:
+                types.add(type(value))
+
+        if len(types) > 1:
+            raise ValueError("All timestamps should be one of two possible types: pd.Timestamp or int!")
+
+    @staticmethod
+    def _validate_first_last_train_timestamps_order(
+        first_train_timestamp: Union[pd.Timestamp, int, None], last_train_timestamp: Union[pd.Timestamp, int]
+    ):
+        """Check that last train timestamp is later than first train timestamp."""
+        if first_train_timestamp is not None and last_train_timestamp < first_train_timestamp:  # type: ignore
             raise ValueError("Last train timestamp should be not sooner than first train timestamp!")
 
-    def _validate_target_timestamps(self):
-        """Check that all target timestamps are later then last train timestamp."""
-        first_target_timestamp = self.target_timestamps[0]
-        if first_target_timestamp <= self.last_train_timestamp:
+    @staticmethod
+    def _validate_target_timestamps(
+        last_train_timestamp: Union[pd.Timestamp, int], target_timestamps: List[Union[pd.Timestamp, int]]
+    ):
+        """Check that all target timestamps aren't empty and later than last train timestamp."""
+        if len(target_timestamps) == 0:
+            raise ValueError("Target timestamps shouldn't be empty!")
+
+        if len(target_timestamps) != len(set(target_timestamps)):
+            raise ValueError("Target timestamps shouldn't contain duplicates!")
+
+        first_target_timestamp = target_timestamps[0]
+        if first_target_timestamp <= last_train_timestamp:  # type: ignore
             raise ValueError("Target timestamps should be strictly later then last train timestamp!")
 
     def validate_on_dataset(self, ts: TSDataset, horizon: int):
         """Validate fold mask on the dataset with specified horizon.
 
         Parameters
         ----------
         ts:
             Dataset to validate on
         horizon:
             Forecasting horizon
+
+        Raises
+        ------
+        ValueError:
+            First train timestamp isn't present in a given dataset
+        ValueError:
+            Last train timestamp isn't present in a given dataset
+        ValueError:
+            Some of target timestamps aren't present in a given dataset
+        ValueError:
+            First train timestamp should be later than minimal dataset timestamp
+        ValueError:
+            Last train timestamp should be not later than the ending of the shortest segment
+        ValueError:
+            Last target timestamp should be not later than horizon steps after last train timestamp
         """
-        dataset_timestamps = list(ts.index)
+        timestamps = ts.index.to_list()
+
+        if self.first_train_timestamp is not None and self.first_train_timestamp not in timestamps:
+            raise ValueError("First train timestamp isn't present in a given dataset!")
+
+        if self.last_train_timestamp not in timestamps:
+            raise ValueError("Last train timestamp isn't present in a given dataset!")
+
+        if not set(self.target_timestamps).issubset(set(timestamps)):
+            diff = set(self.target_timestamps).difference(set(timestamps))
+            raise ValueError(f"Some target timestamps aren't present in a given dataset: {reprlib.repr(diff)}")
+
         dataset_description = ts.describe()
 
-        min_first_timestamp = ts.index.min()
-        if self.first_train_timestamp and self.first_train_timestamp < min_first_timestamp:
-            raise ValueError(f"First train timestamp should be later than {min_first_timestamp}!")
-
-        last_timestamp = dataset_description["end_timestamp"].min()
-        if self.last_train_timestamp > last_timestamp:
-            raise ValueError(f"Last train timestamp should be not later than {last_timestamp}!")
-
-        dataset_first_target_timestamp = dataset_timestamps[dataset_timestamps.index(self.last_train_timestamp) + 1]
-        mask_first_target_timestamp = self.target_timestamps[0]
-        if mask_first_target_timestamp < dataset_first_target_timestamp:
-            raise ValueError(f"First target timestamp should be not sooner than {dataset_first_target_timestamp}!")
-
-        dataset_last_target_timestamp = dataset_timestamps[
-            dataset_timestamps.index(self.last_train_timestamp) + horizon
-        ]
+        dataset_min_last_timestamp = dataset_description["end_timestamp"].min()
+        if self.last_train_timestamp > dataset_min_last_timestamp:
+            raise ValueError(f"Last train timestamp should be not later than {dataset_min_last_timestamp}!")
+
+        dataset_horizon_border_timestamp = timestamps[timestamps.index(self.last_train_timestamp) + horizon]
         mask_last_target_timestamp = self.target_timestamps[-1]
-        if dataset_last_target_timestamp < mask_last_target_timestamp:
-            raise ValueError(f"Last target timestamp should be not later than {dataset_last_target_timestamp}!")
+        if dataset_horizon_border_timestamp < mask_last_target_timestamp:
+            raise ValueError(f"Last target timestamp should be not later than {dataset_horizon_border_timestamp}!")
 
 
 class AbstractPipeline(AbstractSaveable):
     """Interface for pipeline."""
 
     @abstractmethod
     def fit(self, ts: TSDataset, save_ts: bool = True) -> "AbstractPipeline":
@@ -174,25 +267,27 @@
         """
         pass
 
     @abstractmethod
     def predict(
         self,
         ts: TSDataset,
-        start_timestamp: Optional[pd.Timestamp] = None,
-        end_timestamp: Optional[pd.Timestamp] = None,
+        start_timestamp: Union[pd.Timestamp, int, str, None] = None,
+        end_timestamp: Union[pd.Timestamp, int, str, None] = None,
         prediction_interval: bool = False,
         quantiles: Sequence[float] = (0.025, 0.975),
         return_components: bool = False,
     ) -> TSDataset:
         """Make in-sample predictions on dataset in a given range.
 
         Currently, in situation when segments start with different timestamps
         we only guarantee to work with ``start_timestamp`` >= beginning of all segments.
 
+        Parameters ``start_timestamp`` and ``end_timestamp`` of type ``str`` are converted into ``pd.Timestamp``.
+
         Parameters
         ----------
         ts:
             Dataset to make predictions on.
         start_timestamp:
             First timestamp of prediction range to return, should be >= than first timestamp in ``ts``;
             expected that beginning of each segment <= ``start_timestamp``;
@@ -211,14 +306,16 @@
         -------
         :
             Dataset with predictions in ``[start_timestamp, end_timestamp]`` range.
 
         Raises
         ------
         ValueError:
+            Incorrect type of ``start_timestamp`` or ``end_timestamp`` is used according to ``ts.freq``
+        ValueError:
             Value of ``end_timestamp`` is less than ``start_timestamp``.
         ValueError:
             Value of ``start_timestamp`` goes before point where each segment started.
         ValueError:
             Value of ``end_timestamp`` goes after the last timestamp.
         """
 
@@ -458,61 +555,66 @@
                 ts=ts, predictions=predictions, quantiles=quantiles, n_folds=n_folds
             )
         return predictions
 
     @staticmethod
     def _make_predict_timestamps(
         ts: TSDataset,
-        start_timestamp: Optional[pd.Timestamp] = None,
-        end_timestamp: Optional[pd.Timestamp] = None,
-    ) -> Tuple[pd.Timestamp, pd.Timestamp]:
+        start_timestamp: Union[pd.Timestamp, int, str, None],
+        end_timestamp: Union[pd.Timestamp, int, str, None],
+    ) -> Union[Tuple[pd.Timestamp, pd.Timestamp], Tuple[int, int]]:
+        start_timestamp = _check_timestamp_param(param=start_timestamp, param_name="start_timestamp", freq=ts.freq)
+        end_timestamp = _check_timestamp_param(param=end_timestamp, param_name="end_timestamp", freq=ts.freq)
+
         min_timestamp = ts.describe()["start_timestamp"].max()
         max_timestamp = ts.index[-1]
 
         if start_timestamp is None:
             start_timestamp = min_timestamp
         if end_timestamp is None:
             end_timestamp = max_timestamp
 
         if start_timestamp < min_timestamp:
             raise ValueError("Value of start_timestamp is less than beginning of some segments!")
         if end_timestamp > max_timestamp:
             raise ValueError("Value of end_timestamp is more than ending of dataset!")
 
-        if start_timestamp > end_timestamp:
+        if start_timestamp > end_timestamp:  # type: ignore
             raise ValueError("Value of end_timestamp is less than start_timestamp!")
 
         return start_timestamp, end_timestamp
 
     @abstractmethod
     def _predict(
         self,
         ts: TSDataset,
-        start_timestamp: Optional[pd.Timestamp],
-        end_timestamp: Optional[pd.Timestamp],
+        start_timestamp: Union[pd.Timestamp, int],
+        end_timestamp: Union[pd.Timestamp, int],
         prediction_interval: bool,
         quantiles: Sequence[float],
         return_components: bool,
     ) -> TSDataset:
         pass
 
     def predict(
         self,
         ts: TSDataset,
-        start_timestamp: Optional[pd.Timestamp] = None,
-        end_timestamp: Optional[pd.Timestamp] = None,
+        start_timestamp: Union[pd.Timestamp, int, str, None] = None,
+        end_timestamp: Union[pd.Timestamp, int, str, None] = None,
         prediction_interval: bool = False,
         quantiles: Sequence[float] = (0.025, 0.975),
         return_components: bool = False,
     ) -> TSDataset:
         """Make in-sample predictions on dataset in a given range.
 
         Currently, in situation when segments start with different timestamps
         we only guarantee to work with ``start_timestamp`` >= beginning of all segments.
 
+        Parameters ``start_timestamp`` and ``end_timestamp`` of type ``str`` are converted into ``pd.Timestamp``.
+
         Parameters
         ----------
         ts:
             Dataset to make predictions on.
         start_timestamp:
             First timestamp of prediction range to return, should be >= than first timestamp in ``ts``;
             expected that beginning of each segment <= ``start_timestamp``;
@@ -530,14 +632,16 @@
         Returns
         -------
         :
             Dataset with predictions in ``[start_timestamp, end_timestamp]`` range.
 
         Raises
         ------
+        ValueError
+            Incorrect type of ``start_timestamp`` or ``end_timestamp`` is used according to ``ts.freq``
         ValueError:
             Value of ``end_timestamp`` is less than ``start_timestamp``.
         ValueError:
             Value of ``start_timestamp`` goes before point where each segment started.
         ValueError:
             Value of ``end_timestamp`` goes after the last timestamp.
         NotImplementedError:
@@ -628,19 +732,19 @@
             min_train_idx = min_timestamp_idx + (n_folds - offset) * stride * constant_history_length
             max_train_idx = max_timestamp_idx - stride * (offset - 1) - horizon - 1
             min_test_idx = max_train_idx + 1
             max_test_idx = max_train_idx + horizon
 
             min_train, max_train = dataset_timestamps[min_train_idx], dataset_timestamps[max_train_idx]
             min_test, max_test = dataset_timestamps[min_test_idx], dataset_timestamps[max_test_idx]
-
+            target_timestamps = timestamp_range(start=min_test, end=max_test, freq=ts.freq).tolist()
             mask = FoldMask(
                 first_train_timestamp=min_train,
                 last_train_timestamp=max_train,
-                target_timestamps=list(pd.date_range(start=min_test, end=max_test, freq=ts.freq)),
+                target_timestamps=target_timestamps,
             )
             masks.append(mask)
 
         return masks
 
     @staticmethod
     def _validate_backtest_metrics(metrics: List[Metric]):
```

### Comparing `etna-2.5.0/etna/pipeline/hierarchical_pipeline.py` & `etna-2.6.0/etna/pipeline/hierarchical_pipeline.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/pipeline/mixins.py` & `etna-2.6.0/etna/pipeline/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pathlib
 import tempfile
 import zipfile
 from copy import deepcopy
 from typing import Dict
 from typing import Optional
 from typing import Sequence
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from typing_extensions import Self
 from typing_extensions import get_args
 
 from etna.core import SaveMixin
@@ -23,57 +24,59 @@
 from etna.models import PredictionIntervalContextRequiredAbstractModel
 from etna.transforms import Transform
 
 
 class ModelPipelinePredictMixin:
     """Mixin for pipelines with model inside with implementation of ``_predict`` method."""
 
-    def _create_ts(self, ts: TSDataset, start_timestamp: pd.Timestamp, end_timestamp: pd.Timestamp) -> TSDataset:
+    def _create_ts(
+        self, ts: TSDataset, start_timestamp: Union[pd.Timestamp, int], end_timestamp: Union[pd.Timestamp, int]
+    ) -> TSDataset:
         """Create ``TSDataset`` to make predictions on."""
         self.model: ModelType
         self.transforms: Sequence[Transform]
 
         df = deepcopy(ts.raw_df)
         df_exog = deepcopy(ts.df_exog)
         freq = deepcopy(ts.freq)
         known_future = deepcopy(ts.known_future)
 
-        df_to_transform = df[:end_timestamp]
+        df_to_transform = df.loc[:end_timestamp]
 
         cur_ts = TSDataset(
             df=df_to_transform,
             df_exog=df_exog,
             freq=freq,
             known_future=known_future,
             hierarchical_structure=ts.hierarchical_structure,
         )
 
         cur_ts.transform(transforms=self.transforms)
 
         # correct start_timestamp taking into account context size
         timestamp_indices = pd.Series(np.arange(len(df.index)), index=df.index)
-        start_idx = timestamp_indices[start_timestamp]
+        start_idx = timestamp_indices.loc[start_timestamp]
         start_idx = max(0, start_idx - self.model.context_size)
         start_timestamp = timestamp_indices.index[start_idx]
 
-        cur_ts.df = cur_ts.df[start_timestamp:end_timestamp]
+        cur_ts.df = cur_ts.df.loc[start_timestamp:end_timestamp]
         return cur_ts
 
     def _determine_prediction_size(
-        self, ts: TSDataset, start_timestamp: pd.Timestamp, end_timestamp: pd.Timestamp
+        self, ts: TSDataset, start_timestamp: Union[pd.Timestamp, int], end_timestamp: Union[pd.Timestamp, int]
     ) -> int:
         timestamp_indices = pd.Series(np.arange(len(ts.index)), index=ts.index)
-        timestamps = timestamp_indices[start_timestamp:end_timestamp]
+        timestamps = timestamp_indices.loc[start_timestamp:end_timestamp]
         return len(timestamps)
 
     def _predict(
         self,
         ts: TSDataset,
-        start_timestamp: pd.Timestamp,
-        end_timestamp: pd.Timestamp,
+        start_timestamp: Union[pd.Timestamp, int],
+        end_timestamp: Union[pd.Timestamp, int],
         prediction_interval: bool,
         quantiles: Sequence[float],
         return_components: bool = False,
     ) -> TSDataset:
         predict_ts = self._create_ts(ts=ts, start_timestamp=start_timestamp, end_timestamp=end_timestamp)
         prediction_size = self._determine_prediction_size(
             ts=ts, start_timestamp=start_timestamp, end_timestamp=end_timestamp
```

### Comparing `etna-2.5.0/etna/pipeline/pipeline.py` & `etna-2.6.0/etna/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/reconciliation/base.py` & `etna-2.6.0/etna/reconciliation/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/reconciliation/bottom_up.py` & `etna-2.6.0/etna/reconciliation/bottom_up.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/reconciliation/top_down.py` & `etna-2.6.0/etna/reconciliation/top_down.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/settings.py` & `etna-2.6.0/etna/settings.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/__init__.py` & `etna-2.6.0/etna/transforms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from etna.transforms.encoders import OneHotEncoderTransform
 from etna.transforms.encoders import SegmentEncoderTransform
 from etna.transforms.feature_selection import FilterFeaturesTransform
 from etna.transforms.feature_selection import GaleShapleyFeatureSelectionTransform
 from etna.transforms.feature_selection import MRMRFeatureSelectionTransform
 from etna.transforms.feature_selection import TreeFeatureSelectionTransform
 from etna.transforms.math import AddConstTransform
+from etna.transforms.math import BinaryOperationTransform
+from etna.transforms.math import BinaryOperator
 from etna.transforms.math import BoxCoxTransform
 from etna.transforms.math import DifferencingTransform
 from etna.transforms.math import ExogShiftTransform
 from etna.transforms.math import LagTransform
 from etna.transforms.math import LambdaTransform
 from etna.transforms.math import LimitTransform
 from etna.transforms.math import LogTransform
```

### Comparing `etna-2.5.0/etna/transforms/base.py` & `etna-2.6.0/etna/transforms/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/__init__.py` & `etna-2.6.0/etna/transforms/decomposition/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/__init__.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/base.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         return series.values
 
     def _fit_per_interval_models(self, series: pd.Series):
         """Fit per-interval models with corresponding data from series."""
         if self.intervals is None or self.per_interval_models is None:
             raise ValueError("Something went wrong on fit! Check the parameters of the transform.")
         for interval in self.intervals:
-            tmp_series = series[interval[0] : interval[1]]
+            tmp_series = series.loc[interval[0] : interval[1]]
             features = self._get_features(series=tmp_series)
             targets = self._get_targets(series=tmp_series)
             self.per_interval_models[interval].fit(features=features, target=targets)
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentChangePointsTransform":
         """Fit transform.
         Get no-changepoints intervals with change_points_model and fit per_interval_model on the intervals.
@@ -109,15 +109,15 @@
 
     def _predict_per_interval_model(self, series: pd.Series) -> pd.Series:
         """Apply per-interval detrending to series."""
         if self.intervals is None or self.per_interval_models is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
         prediction_series = pd.Series(index=series.index, dtype=float)
         for interval in self.intervals:
-            tmp_series = series[interval[0] : interval[1]]
+            tmp_series = series.loc[interval[0] : interval[1]]
             if tmp_series.empty:
                 continue
             features = self._get_features(series=tmp_series)
             per_interval_prediction = self.per_interval_models[interval].predict(features=features)
             prediction_series[tmp_series.index] = per_interval_prediction
         return prediction_series
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/change_points_models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABC
 from abc import abstractmethod
 from typing import List
 from typing import Tuple
 from typing import Type
+from typing import Union
 
 import pandas as pd
 from sklearn.base import RegressorMixin
 
 from etna.core import BaseMixin
 
-TTimestampInterval = Tuple[pd.Timestamp, pd.Timestamp]
+TTimestampInterval = Tuple[Union[pd.Timestamp, int, None], Union[pd.Timestamp, int, None]]
 TDetrendModel = Type[RegressorMixin]
 
 
 class BaseChangePointsModelAdapter(BaseMixin, ABC):
     """BaseChangePointsModelAdapter is the base class for change point models adapters."""
 
     @abstractmethod
@@ -31,28 +32,27 @@
         -------
         change points:
             change point timestamps
         """
         pass
 
     @staticmethod
-    def _build_intervals(change_points: List[pd.Timestamp]) -> List[TTimestampInterval]:
+    def _build_intervals(change_points: List[Union[pd.Timestamp, int]]) -> List[TTimestampInterval]:
         """Create list of stable intervals from list of change points."""
-        change_points.extend([pd.Timestamp.min, pd.Timestamp.max])
-        change_points = sorted(change_points)
+        change_points = [None] + sorted(change_points) + [None]
         intervals = list(zip(change_points[:-1], change_points[1:]))
         return intervals
 
     def get_change_points_intervals(self, df: pd.DataFrame, in_column: str) -> List[TTimestampInterval]:
         """Find change point intervals in given dataframe and column.
 
         Parameters
         ----------
         df:
-            dataframe indexed with timestamp
+            dataframe indexed with timestamp (datetime or integer)
         in_column:
             name of column to get change points
 
         Returns
         -------
         :
             change points intervals
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/change_points_models/ruptures_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/detrend.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/trend.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 from typing import Dict
 from typing import Optional
 
-import numpy as np
 import pandas as pd
-from ruptures.detection import Binseg
+from ruptures import Binseg
 from sklearn.linear_model import LinearRegression
 
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.distributions import IntDistribution
-from etna.transforms.decomposition.change_points_based.base import ReversibleChangePointsTransform
-from etna.transforms.decomposition.change_points_based.base import _OneSegmentChangePointsTransform
+from etna.transforms.decomposition.change_points_based.base import IrreversibleChangePointsTransform
 from etna.transforms.decomposition.change_points_based.change_points_models import BaseChangePointsModelAdapter
-from etna.transforms.decomposition.change_points_based.change_points_models import RupturesChangePointsModel
+from etna.transforms.decomposition.change_points_based.change_points_models.ruptures_based import (
+    RupturesChangePointsModel,
+)
+from etna.transforms.decomposition.change_points_based.detrend import _OneSegmentChangePointsTrendTransform
 from etna.transforms.decomposition.change_points_based.per_interval_models import PerIntervalModel
 from etna.transforms.decomposition.change_points_based.per_interval_models import SklearnRegressionPerIntervalModel
 
 
-class _OneSegmentChangePointsTrendTransform(_OneSegmentChangePointsTransform):
-    """_OneSegmentChangePointsTransform subtracts multiple linear trend from series."""
+class _OneSegmentTrendTransform(_OneSegmentChangePointsTrendTransform):
+    """_OneSegmentTrendTransform adds trend as a feature."""
 
-    @staticmethod
-    def _get_features(series: pd.Series) -> np.ndarray:
-        """Convert ETNA timestamp-index to a list of timestamps to fit regression models."""
-        timestamps = series.index
-        timestamps = np.array([[ts.timestamp()] for ts in timestamps])
-        return timestamps
+    def __init__(
+        self,
+        in_column: str,
+        out_column: str,
+        change_points_model: BaseChangePointsModelAdapter,
+        per_interval_model: PerIntervalModel,
+    ):
+        """Init _OneSegmentTrendTransform.
+
+        Parameters
+        ----------
+        in_column:
+            name of column to apply transform to
+        out_column:
+            name of added column
+        change_points_model:
+            model to get trend change points
+        per_interval_model:
+            model to get trend from data
+        """
+        self.out_column = out_column
+        super().__init__(
+            in_column=in_column,
+            change_points_model=change_points_model,
+            per_interval_model=per_interval_model,
+        )
 
     def _apply_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
-        df.loc[:, self.in_column] -= transformed_series
+        df.loc[:, self.out_column] = transformed_series
         return df
 
     def _apply_inverse_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
-        for column_name in df.columns:
-            df.loc[:, column_name] += transformed_series
         return df
 
 
-class ChangePointsTrendTransform(ReversibleChangePointsTransform):
-    """Transform that makes a detrending of change-point intervals.
-
-    This class differs from :py:class:`~etna.transforms.decomposition.change_points_based.level.ChangePointsLevelTransform`
-    only by default values for ``change_points_model`` and ``per_interval_model``.
+class TrendTransform(IrreversibleChangePointsTransform):
+    """Transform that adds trend as a feature.
 
     Transform divides each segment into intervals using ``change_points_model``.
     Then a separate model is fitted on each interval using ``per_interval_model``.
-    Values predicted by the model are subtracted from each interval.
+    New column is created with values predicted by the model of each interval.
 
     Evaluated function can be linear, mean, median, etc. Look at the signature to find out which models can be used.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
@@ -62,40 +78,46 @@
     _default_per_interval_model = SklearnRegressionPerIntervalModel(model=LinearRegression())
 
     def __init__(
         self,
         in_column: str,
         change_points_model: Optional[BaseChangePointsModelAdapter] = None,
         per_interval_model: Optional[PerIntervalModel] = None,
+        out_column: Optional[str] = None,
     ):
-        """Init ChangePointsTrendTransform.
+        """Init TrendTransform.
 
         Parameters
         ----------
         in_column:
             name of column to apply transform to
         change_points_model:
             model to get trend change points,
             by default :py:class:`ruptures.detection.binseg.Binseg` in a wrapper with ``n_bkps=5`` is used
         per_interval_model:
             model to process intervals of segment,
             by default :py:class:`sklearn.linear_model.LinearRegression` in a wrapper is used
+        out_column:
+            name of added column.
+            If not given, use ``self.__repr__()``
         """
         self.in_column = in_column
+        self.out_column = out_column
 
         self.change_points_model = (
             change_points_model if change_points_model is not None else self._default_change_points_model
         )
         self.per_interval_model = (
             per_interval_model if per_interval_model is not None else self._default_per_interval_model
         )
 
         super().__init__(
-            transform=_OneSegmentChangePointsTrendTransform(
+            transform=_OneSegmentTrendTransform(
                 in_column=self.in_column,
+                out_column=self.out_column if self.out_column is not None else self.__repr__(),
                 change_points_model=self.change_points_model,
                 per_interval_model=self.per_interval_model,
             ),
             required_features=[in_column],
         )
 
     @property
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/level.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/level.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/__init__.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/sklearn_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/per_interval_models/statistics_based.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/segmentation.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/segmentation.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/decomposition/change_points_based/trend.py` & `etna-2.6.0/etna/transforms/decomposition/change_points_based/detrend.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,60 @@
 from typing import Dict
 from typing import Optional
 
+import numpy as np
 import pandas as pd
-from ruptures import Binseg
+from ruptures.detection import Binseg
 from sklearn.linear_model import LinearRegression
 
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.distributions import IntDistribution
-from etna.transforms.decomposition.change_points_based.base import IrreversibleChangePointsTransform
+from etna.transforms.decomposition.change_points_based.base import ReversibleChangePointsTransform
+from etna.transforms.decomposition.change_points_based.base import _OneSegmentChangePointsTransform
 from etna.transforms.decomposition.change_points_based.change_points_models import BaseChangePointsModelAdapter
-from etna.transforms.decomposition.change_points_based.change_points_models.ruptures_based import (
-    RupturesChangePointsModel,
-)
-from etna.transforms.decomposition.change_points_based.detrend import _OneSegmentChangePointsTrendTransform
+from etna.transforms.decomposition.change_points_based.change_points_models import RupturesChangePointsModel
 from etna.transforms.decomposition.change_points_based.per_interval_models import PerIntervalModel
 from etna.transforms.decomposition.change_points_based.per_interval_models import SklearnRegressionPerIntervalModel
 
 
-class _OneSegmentTrendTransform(_OneSegmentChangePointsTrendTransform):
-    """_OneSegmentTrendTransform adds trend as a feature."""
+class _OneSegmentChangePointsTrendTransform(_OneSegmentChangePointsTransform):
+    """_OneSegmentChangePointsTransform subtracts multiple linear trend from series."""
 
-    def __init__(
-        self,
-        in_column: str,
-        out_column: str,
-        change_points_model: BaseChangePointsModelAdapter,
-        per_interval_model: PerIntervalModel,
-    ):
-        """Init _OneSegmentTrendTransform.
+    @staticmethod
+    def _get_features(series: pd.Series) -> np.ndarray:
+        """Convert ETNA timestamp-index to a list of timestamps to fit regression models."""
+        timestamps = series.index.to_series()
+
+        if pd.api.types.is_integer_dtype(timestamps.dtype):
+            timestamps = timestamps.astype("float").to_numpy()
+        else:
+            timestamps = timestamps.apply(lambda ts: ts.timestamp()).to_numpy()
 
-        Parameters
-        ----------
-        in_column:
-            name of column to apply transform to
-        out_column:
-            name of added column
-        change_points_model:
-            model to get trend change points
-        per_interval_model:
-            model to get trend from data
-        """
-        self.out_column = out_column
-        super().__init__(
-            in_column=in_column,
-            change_points_model=change_points_model,
-            per_interval_model=per_interval_model,
-        )
+        return timestamps.reshape((-1, 1))
 
     def _apply_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
-        df.loc[:, self.out_column] = transformed_series
+        df.loc[:, self.in_column] -= transformed_series
         return df
 
     def _apply_inverse_transformation(self, df: pd.DataFrame, transformed_series: pd.Series) -> pd.DataFrame:
+        for column_name in df.columns:
+            df.loc[:, column_name] += transformed_series
         return df
 
 
-class TrendTransform(IrreversibleChangePointsTransform):
-    """Transform that adds trend as a feature.
+class ChangePointsTrendTransform(ReversibleChangePointsTransform):
+    """Transform that makes a detrending of change-point intervals.
+
+    This class differs from :py:class:`~etna.transforms.decomposition.change_points_based.level.ChangePointsLevelTransform`
+    only by default values for ``change_points_model`` and ``per_interval_model``.
 
     Transform divides each segment into intervals using ``change_points_model``.
     Then a separate model is fitted on each interval using ``per_interval_model``.
-    New column is created with values predicted by the model of each interval.
+    Values predicted by the model are subtracted from each interval.
 
     Evaluated function can be linear, mean, median, etc. Look at the signature to find out which models can be used.
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
@@ -78,46 +67,40 @@
     _default_per_interval_model = SklearnRegressionPerIntervalModel(model=LinearRegression())
 
     def __init__(
         self,
         in_column: str,
         change_points_model: Optional[BaseChangePointsModelAdapter] = None,
         per_interval_model: Optional[PerIntervalModel] = None,
-        out_column: Optional[str] = None,
     ):
-        """Init TrendTransform.
+        """Init ChangePointsTrendTransform.
 
         Parameters
         ----------
         in_column:
             name of column to apply transform to
         change_points_model:
             model to get trend change points,
             by default :py:class:`ruptures.detection.binseg.Binseg` in a wrapper with ``n_bkps=5`` is used
         per_interval_model:
             model to process intervals of segment,
             by default :py:class:`sklearn.linear_model.LinearRegression` in a wrapper is used
-        out_column:
-            name of added column.
-            If not given, use ``self.__repr__()``
         """
         self.in_column = in_column
-        self.out_column = out_column
 
         self.change_points_model = (
             change_points_model if change_points_model is not None else self._default_change_points_model
         )
         self.per_interval_model = (
             per_interval_model if per_interval_model is not None else self._default_per_interval_model
         )
 
         super().__init__(
-            transform=_OneSegmentTrendTransform(
+            transform=_OneSegmentChangePointsTrendTransform(
                 in_column=self.in_column,
-                out_column=self.out_column if self.out_column is not None else self.__repr__(),
                 change_points_model=self.change_points_model,
                 per_interval_model=self.per_interval_model,
             ),
             required_features=[in_column],
         )
 
     @property
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/deseasonal.py` & `etna-2.6.0/etna/transforms/decomposition/deseasonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 from typing import Literal
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 from statsmodels.tsa.seasonal import seasonal_decompose
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
-from etna.models.utils import determine_freq
-from etna.models.utils import determine_num_steps
 from etna.transforms.base import OneSegmentTransform
 from etna.transforms.base import ReversiblePerSegmentWrapper
 
+_DEFAULT_FREQ = object()
+
 
 class DeseasonalModel(str, Enum):
     """Enum for different types of deseasonality model."""
 
     additive = "additive"
     multiplicative = "multiplicative"
 
@@ -43,14 +45,15 @@
         model:
             'additive' (default) or 'multiplicative'
         """
         self.in_column = in_column
         self.period = period
         self.model = DeseasonalModel(model)
         self._seasonal: Optional[pd.Series] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
 
     def _roll_seasonal(self, x: pd.Series) -> np.ndarray:
         """
         Roll out seasonal component by x's time index.
 
         Parameters
         ----------
@@ -60,19 +63,24 @@
         Returns
         -------
         result:
             seasonal component
         """
         if self._seasonal is None:
             raise ValueError("Transform is not fitted! Fit the Transform before calling.")
-        freq = determine_freq(x.index)
         if self._seasonal.index[0] <= x.index[0]:
-            shift = -determine_num_steps(self._seasonal.index[0], x.index[0], freq) % self.period
+            shift = (
+                -determine_num_steps(start_timestamp=self._seasonal.index[0], end_timestamp=x.index[0], freq=self._freq)
+                % self.period
+            )
         else:
-            shift = determine_num_steps(x.index[0], self._seasonal.index[0], freq) % self.period
+            shift = (
+                determine_num_steps(start_timestamp=x.index[0], end_timestamp=self._seasonal.index[0], freq=self._freq)
+                % self.period
+            )
         return np.resize(np.roll(self._seasonal, shift=shift), x.shape[0])
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentDeseasonalityTransform":
         """
         Perform seasonal decomposition.
 
         Parameters
@@ -86,19 +94,21 @@
             instance after processing
 
         Raises
         ------
         ValueError:
             if input column contains NaNs in the middle of the series
         """
+        self._freq = determine_freq(df.index)
+
         df = df.loc[df[self.in_column].first_valid_index() : df[self.in_column].last_valid_index()]
         if df[self.in_column].isnull().values.any():
             raise ValueError("The input column contains NaNs in the middle of the series! Try to use the imputer.")
         self._seasonal = seasonal_decompose(
-            x=df[self.in_column], model=self.model, filt=None, two_sided=False, extrapolate_trend=0
+            x=df[self.in_column], model=self.model, period=self.period, filt=None, two_sided=False, extrapolate_trend=0
         ).seasonal[: self.period]
         return self
 
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Subtract seasonal component.
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/detrend.py` & `etna-2.6.0/etna/transforms/decomposition/detrend.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,22 @@
             [("polynomial", PolynomialFeatures(degree=self.poly_degree, include_bias=False)), ("regressor", regressor)]
         )
         # verification that this variable is fitted isn't needed because this class isn't used by the user
         self._x_median = None
 
     @staticmethod
     def _get_x(df) -> np.ndarray:
-        series_len = len(df)
         x = df.index.to_series()
-        if isinstance(type(x.dtype), pd.Timestamp):
-            raise ValueError("Your timestamp column has wrong format. Need np.datetime64 or datetime.datetime")
-        x = x.apply(lambda ts: ts.timestamp())
-        x = x.to_numpy().reshape(series_len, 1)
+
+        if pd.api.types.is_integer_dtype(x.dtype):
+            x = x.astype("float").to_numpy()
+        else:
+            x = x.apply(lambda ts: ts.timestamp()).to_numpy()
+
+        x = x.reshape(-1, 1)
         return x
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentLinearTrendBaseTransform":
         """
         Fit regression detrend_model with data from df.
 
         Parameters
```

### Comparing `etna-2.5.0/etna/transforms/decomposition/stl.py` & `etna-2.6.0/etna/transforms/decomposition/stl.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 import pandas as pd
 from statsmodels.tsa.arima.model import ARIMA
 from statsmodels.tsa.base.tsa_model import TimeSeriesModel
 from statsmodels.tsa.exponential_smoothing.ets import ETSModel
 from statsmodels.tsa.forecasting.stl import STLForecast
 from statsmodels.tsa.forecasting.stl import STLForecastResults
 
+from etna.datasets.utils import determine_freq
+from etna.datasets.utils import determine_num_steps
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.transforms.base import OneSegmentTransform
 from etna.transforms.base import ReversiblePerSegmentWrapper
 
+_DEFAULT_FREQ = object()
+
 
 class _OneSegmentSTLTransform(OneSegmentTransform):
     def __init__(
         self,
         in_column: str,
         period: int,
         model: Union[str, TimeSeriesModel] = "arima",
@@ -76,91 +80,115 @@
         else:
             raise ValueError("Model should be a string or TimeSeriesModel")
 
         self.robust = robust
         self.model_kwargs = model_kwargs
         self.stl_kwargs = stl_kwargs
         self.fit_results: Optional[STLForecastResults] = None
+        self._first_train_timestamp: Union[pd.Timestamp, int, None] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentSTLTransform":
         """
         Perform STL decomposition and fit trend model.
 
         Parameters
         ----------
         df:
             Features dataframe with time
 
         Returns
         -------
-        result: _OneSegmentSTLTransform
+        :
             instance after processing
         """
         df = df.loc[df[self.in_column].first_valid_index() : df[self.in_column].last_valid_index()]
         if df[self.in_column].isnull().values.any():
             raise ValueError("The input column contains NaNs in the middle of the series! Try to use the imputer.")
+
+        self._first_train_timestamp = df.index.min()
+        self._freq = determine_freq(df.index)
+
+        endog = df[self.in_column]
+        if pd.api.types.is_integer_dtype(df.index):
+            # make index start with zero
+            endog.index = endog.index - self._first_train_timestamp
+
         model = STLForecast(
-            df[self.in_column],
-            self.model,
+            endog=endog,
+            model=self.model,
             model_kwargs=self.model_kwargs,
             period=self.period,
             robust=self.robust,
             **self.stl_kwargs,
         )
         self.fit_results = model.fit()
         return self
 
+    def _get_season_trend(self, df: pd.DataFrame) -> pd.Series:
+        if self.fit_results is None:
+            raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
+
+        start_timestamp = df[self.in_column].first_valid_index()
+        end_timestamp = df[self.in_column].last_valid_index()
+
+        # if all values are NaNs
+        if start_timestamp is None:
+            return pd.Series([], dtype=float)
+
+        start_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=start_timestamp, freq=self._freq
+        )
+        end_idx = determine_num_steps(
+            start_timestamp=self._first_train_timestamp, end_timestamp=end_timestamp, freq=self._freq
+        )
+
+        prediction = self.fit_results.get_prediction(start=start_idx, end=end_idx).predicted_mean.values
+
+        index = df.index[df.index.get_loc(start_timestamp) : df.index.get_loc(end_timestamp) + 1]
+        season_trend = pd.Series(prediction, index=index)
+        return season_trend
+
     def transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Subtract trend and seasonal component.
 
         Parameters
         ----------
         df:
             Features dataframe with time
 
         Returns
         -------
-        result: pd.DataFrame
+        :
             Dataframe with extracted features
         """
         result = df
-        if self.fit_results is not None:
-            season_trend = self.fit_results.get_prediction(
-                start=df[self.in_column].first_valid_index(), end=df[self.in_column].last_valid_index()
-            ).predicted_mean
-        else:
-            raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
+        season_trend = self._get_season_trend(df=df)
         result[self.in_column] -= season_trend
         return result
 
     def inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Add trend and seasonal component.
 
         Parameters
         ----------
         df:
             Features dataframe with time
 
         Returns
         -------
-        result: pd.DataFrame
+        :
             Dataframe with extracted features
         """
         result = df
-        if self.fit_results is None:
-            raise ValueError("Transform is not fitted! Fit the Transform before calling inverse_transform method.")
-        season_trend = self.fit_results.get_prediction(
-            start=df[self.in_column].first_valid_index(), end=df[self.in_column].last_valid_index()
-        ).predicted_mean
-
+        season_trend = self._get_season_trend(df=df)
         for colum_name in df.columns:
             result.loc[:, colum_name] += season_trend
-
         return result
 
 
 class STLTransform(ReversiblePerSegmentWrapper):
     """Transform that uses :py:class:`statsmodels.tsa.seasonal.STL` to subtract season and trend from the data.
 
     Warning
```

### Comparing `etna-2.5.0/etna/transforms/encoders/categorical.py` & `etna-2.6.0/etna/transforms/encoders/categorical.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/encoders/mean_segment_encoder.py` & `etna-2.6.0/etna/transforms/encoders/mean_segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/encoders/segment_encoder.py` & `etna-2.6.0/etna/transforms/encoders/segment_encoder.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/feature_selection/base.py` & `etna-2.6.0/etna/transforms/feature_selection/base.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/feature_selection/feature_importance.py` & `etna-2.6.0/etna/transforms/feature_selection/feature_importance.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,21 +225,25 @@
 
         Returns
         -------
         result:
             instance after fitting
         """
         features = self._get_features_to_use(df)
-        ts = TSDataset(df=df, freq=pd.infer_freq(df.index))
-        relevance_table = self.relevance_table(ts[:, :, "target"], ts[:, :, features], **self.relevance_params)
+        df_target = df.loc[:, pd.IndexSlice[:, "target"]]
+        df_target = df_target.loc[df_target.first_valid_index() :]
+        df_features = df.loc[:, pd.IndexSlice[:, features]]
+        df_features = df_features.loc[df_features.first_valid_index() :]
+        relevance_table = self.relevance_table(df_target, df_features, **self.relevance_params)
+
         if not self.relevance_table.greater_is_better:
             relevance_table *= -1
         self.selected_features = mrmr(
             relevance_table=relevance_table,
-            regressors=ts[:, :, features],
+            regressors=df_features,
             top_k=self.top_k,
             fast_redundancy=self.fast_redundancy,
             relevance_aggregation_mode=self.relevance_aggregation_mode,
             redundancy_aggregation_mode=self.redundancy_aggregation_mode,
             atol=self.atol,
         )
         return self
```

### Comparing `etna-2.5.0/etna/transforms/feature_selection/filter.py` & `etna-2.6.0/etna/transforms/feature_selection/filter.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/feature_selection/gale_shapley.py` & `etna-2.6.0/etna/transforms/feature_selection/gale_shapley.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/__init__.py` & `etna-2.6.0/etna/transforms/math/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from etna.transforms.math.add_constant import AddConstTransform
 from etna.transforms.math.apply_lambda import LambdaTransform
+from etna.transforms.math.binary_operator import BinaryOperationTransform
+from etna.transforms.math.binary_operator import BinaryOperator
 from etna.transforms.math.differencing import DifferencingTransform
 from etna.transforms.math.lags import ExogShiftTransform
 from etna.transforms.math.lags import LagTransform
 from etna.transforms.math.limit import LimitTransform
 from etna.transforms.math.log import LogTransform
 from etna.transforms.math.power import BoxCoxTransform
 from etna.transforms.math.power import YeoJohnsonTransform
```

### Comparing `etna-2.5.0/etna/transforms/math/add_constant.py` & `etna-2.6.0/etna/transforms/math/add_constant.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/apply_lambda.py` & `etna-2.6.0/etna/transforms/math/apply_lambda.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/differencing.py` & `etna-2.6.0/etna/transforms/math/differencing.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 from typing import Union
 from typing import cast
 
 import numpy as np
 import pandas as pd
 
 from etna.datasets import TSDataset
+from etna.datasets.utils import timestamp_range
 from etna.distributions import BaseDistribution
 from etna.distributions import IntDistribution
 from etna.transforms.base import ReversibleTransform
 from etna.transforms.utils import check_new_segments
 
+_DEFAULT_FREQ = object()
+
 
 class _SingleDifferencingTransform(ReversibleTransform):
     """Calculate a time series differences of order 1.
 
     During ``fit`` this transform can work with NaNs at the beginning of the segment, but fails when meets NaN inside the segment.
     During ``transform`` and ``inverse_transform`` there is no special treatment of NaNs.
 
@@ -69,14 +72,15 @@
         self.inplace = inplace
         self.out_column = out_column
 
         self._train_timestamp: Optional[pd.DatetimeIndex] = None
         self._train_init_dict: Optional[Dict[str, pd.Series]] = None
         self._test_init_df: Optional[pd.DataFrame] = None
         self.in_column_regressor: Optional[bool] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
 
     def _get_column_name(self) -> str:
         if self.inplace:
             return self.in_column
         if self.out_column is None:
             return self.__repr__()
         else:
@@ -89,14 +93,15 @@
         if self.inplace:
             return []
         return [self._get_column_name()] if self.in_column_regressor else []
 
     def fit(self, ts: TSDataset) -> "_SingleDifferencingTransform":
         """Fit the transform."""
         self.in_column_regressor = self.in_column in ts.regressors
+        self._freq = ts.freq
         super().fit(ts)
         return self
 
     def _fit(self, df: pd.DataFrame) -> "_SingleDifferencingTransform":
         """Fit the transform.
 
         Parameters
@@ -190,20 +195,17 @@
 
     def _reconstruct_test(self, df: pd.DataFrame, columns_to_inverse: Set[str]) -> pd.DataFrame:
         """Reconstruct the test in ``inverse_transform``."""
         segments = sorted(set(df.columns.get_level_values("segment")))
         result_df = df.copy()
 
         # check that test is right after the train
-        expected_min_test_timestamp = pd.date_range(
-            start=self._test_init_df.index.max(),  # type: ignore
-            periods=2,
-            freq=pd.infer_freq(self._train_timestamp),
-            closed="right",
-        )[0]
+        expected_min_test_timestamp = timestamp_range(
+            start=self._test_init_df.index[-1], periods=2, freq=self._freq  # type: ignore
+        )[-1]
         if expected_min_test_timestamp != df.index.min():
             raise ValueError("Test should go after the train without gaps")
 
         # we can reconstruct the values by concatenating saved fit values before test values
         for column in columns_to_inverse:
             to_transform = df.loc[:, pd.IndexSlice[segments, column]].copy()
             init_df = self._test_init_df.copy()  # type: ignore
@@ -350,14 +352,15 @@
         # other transforms should make differences inplace
         for _ in range(self.order - 1):
             self._differencing_transforms.append(
                 _SingleDifferencingTransform(in_column=result_out_column, period=self.period, inplace=True)
             )
         self._fit_segments: Optional[List[str]] = None
         self.in_column_regressor: Optional[bool] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
 
     def _get_column_name(self) -> str:
         if self.inplace:
             return self.in_column
         if self.out_column is None:
             return self.__repr__()
         else:
@@ -370,14 +373,15 @@
         if self.inplace:
             return []
         return [self._get_column_name()] if self.in_column_regressor else []
 
     def fit(self, ts: TSDataset) -> "DifferencingTransform":
         """Fit the transform."""
         self.in_column_regressor = self.in_column in ts.regressors
+        self._freq = ts.freq
         super().fit(ts)
         return self
 
     def _fit(self, df: pd.DataFrame) -> "DifferencingTransform":
         """Fit the transform.
 
         Parameters
@@ -394,14 +398,17 @@
         ValueError:
             if NaNs are present inside the segment
         """
         # this is made because transforms of high order may need some columns created by transforms of lower order
         result_df = df
         for transform in self._differencing_transforms:
             result_df = transform._fit_transform(result_df)
+            transform._freq = self._freq
+            transform.in_column_regressor = self.in_column_regressor
+
         self._fit_segments = df.columns.get_level_values("segment").unique().tolist()
         return self
 
     def _check_is_fitted(self):
         if self._fit_segments is None:
             raise ValueError("Transform is not fitted!")
```

### Comparing `etna-2.5.0/etna/transforms/math/lags.py` & `etna-2.6.0/etna/transforms/math/lags.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,27 @@
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 import pandas as pd
 
 from etna.datasets import TSDataset
-from etna.models.utils import determine_num_steps
+from etna.datasets.utils import determine_num_steps
 from etna.transforms.base import IrreversibleTransform
 
+_DEFAULT_FREQ = object()
+
 
 class LagTransform(IrreversibleTransform):
-    """Generates series of lags from given dataframe."""
+    """Generates series of lags from given dataframe.
+
+    Notes
+    -----
+    Types of shifted variables could change due to applying :py:meth:`pandas.DataFrame.shift`.
+    """
 
     def __init__(self, in_column: str, lags: Union[List[int], int], out_column: Optional[str] = None):
         """Create instance of LagTransform.
 
         Parameters
         ----------
         in_column:
@@ -85,28 +92,34 @@
         """
         result = df
         segments = sorted(set(df.columns.get_level_values("segment")))
         all_transformed_features = []
         features = df.loc[:, pd.IndexSlice[:, self.in_column]]
         for lag in self.lags:
             column_name = self._get_column_name(lag)
+            # this could lead to type changes due to introduction of NaNs
             transformed_features = features.shift(lag)
             transformed_features.columns = pd.MultiIndex.from_product([segments, [column_name]])
             all_transformed_features.append(transformed_features)
         result = pd.concat([result] + all_transformed_features, axis=1)
         result = result.sort_index(axis=1)
         return result
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
         return [self._get_column_name(lag) for lag in self.lags]
 
 
 class ExogShiftTransform(IrreversibleTransform):
-    """Shifts exogenous variables from a given dataframe."""
+    """Shifts exogenous variables from a given dataframe.
+
+    Notes
+    -----
+    Types of shifted variables could change due to applying :py:meth:`pandas.DataFrame.shift`.
+    """
 
     def __init__(self, lag: Union[int, Literal["auto"]], horizon: Optional[int] = None):
         """Create instance of ExogShiftTransform.
 
         Parameters
         ----------
         lag:
@@ -122,18 +135,18 @@
         """
         super().__init__(required_features="all")
 
         self.lag: Optional[int] = None
         self.horizon: Optional[int] = None
         self._auto = False
 
-        self._freq: Optional[str] = None
+        self._freq: Optional[str] = _DEFAULT_FREQ  # type: ignore
         self._created_regressors: Optional[List[str]] = None
         self._exog_shifts: Optional[Dict[str, int]] = None
-        self._exog_last_date: Optional[Dict[str, pd.Timestamp]] = None
+        self._exog_last_timestamp: Union[Dict[str, pd.Timestamp], Dict[str, int], None] = None
         self._filter_out_columns = {"target"}
 
         if isinstance(lag, int):
             if lag <= 0:
                 raise ValueError(f"{self.__class__.__name__} works only with positive lags values, {lag} given")
             self.lag = lag
 
@@ -143,27 +156,29 @@
 
             if horizon < 1:
                 raise ValueError(f"{self.__class__.__name__} works only with positive horizon values, {horizon} given")
 
             self.horizon = horizon
             self._auto = True
 
-    def _save_exog_last_date(self, df_exog: Optional[pd.DataFrame] = None):
-        """Save last available date of each exogenous variable."""
-        self._exog_last_date = {}
+    def _save_exog_last_timestamp(self, df_exog: Optional[pd.DataFrame] = None):
+        """Save last available timestamp of each exogenous variable."""
+        exog_last_timestamp = {}
         if df_exog is not None:
             exog_names = set(df_exog.columns.get_level_values("feature"))
 
             for name in exog_names:
                 feature = df_exog.loc[:, pd.IndexSlice[:, name]]
 
                 na_mask = pd.isna(feature).any(axis=1)
-                last_date = feature.index[~na_mask].max()
+                last_timestamp = feature.index[~na_mask].max()
+
+                exog_last_timestamp[name] = last_timestamp
 
-                self._exog_last_date[name] = last_date
+        self._exog_last_timestamp = exog_last_timestamp
 
     def fit(self, ts: TSDataset) -> "ExogShiftTransform":
         """Fit the transform.
 
         Parameters
         ----------
         ts:
@@ -171,15 +186,15 @@
 
         Returns
         -------
         :
             The fitted transform instance.
         """
         self._freq = ts.freq
-        self._save_exog_last_date(df_exog=ts.df_exog)
+        self._save_exog_last_timestamp(df_exog=ts.df_exog)
 
         super().fit(ts=ts)
 
         return self
 
     def _fit(self, df: pd.DataFrame) -> "ExogShiftTransform":
         """Estimate shifts for exogenous variables.
@@ -207,34 +222,34 @@
                 self._created_regressors.append(f"{feature_name}_shift_{shift}")
 
         return self
 
     def _get_feature_names(self, df: pd.DataFrame) -> List[str]:
         """Return the names of exogenous variables."""
         feature_names = []
-        if self._exog_last_date is not None:
-            feature_names = list(self._exog_last_date.keys())
+        if self._exog_last_timestamp is not None:
+            feature_names = list(self._exog_last_timestamp.keys())
 
         df_columns = df.columns.get_level_values("feature")
         for name in feature_names:
             if name not in df_columns:
                 raise ValueError(f"Feature `{name}` is expected to be in the dataframe!")
 
         return feature_names
 
     def _estimate_shift(self, df: pd.DataFrame, feature_name: str) -> int:
         """Estimate shift value for exogenous variable."""
         if not self._auto:
             return self.lag  # type: ignore
 
-        if self._exog_last_date is None or self._freq is None:
+        if self._exog_last_timestamp is None:
             raise ValueError("Call `fit()` method before estimating exog shifts!")
 
         last_date = df.index.max()
-        last_feature_date = self._exog_last_date[feature_name]
+        last_feature_date = self._exog_last_timestamp[feature_name]
 
         if last_feature_date > last_date:
             delta = -determine_num_steps(start_timestamp=last_date, end_timestamp=last_feature_date, freq=self._freq)
 
         elif last_feature_date < last_date:
             delta = determine_num_steps(start_timestamp=last_feature_date, end_timestamp=last_date, freq=self._freq)
 
@@ -269,15 +284,16 @@
         features_to_remove = []
         for feature_name in feature_names:
             shift = self._exog_shifts[feature_name]
 
             feature = df.loc[:, pd.IndexSlice[:, feature_name]]
 
             if shift > 0:
-                shifted_feature = feature.shift(shift, freq=self._freq)
+                # this could lead to type changes due to introduction of NaNs
+                shifted_feature = feature.shift(shift)
 
                 column_name = f"{feature_name}_shift_{shift}"
                 shifted_feature.columns = pd.MultiIndex.from_product([segments, [column_name]])
 
                 shifted_features.append(shifted_feature)
                 features_to_remove.append(feature_name)
```

### Comparing `etna-2.5.0/etna/transforms/math/limit.py` & `etna-2.6.0/etna/transforms/math/limit.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/log.py` & `etna-2.6.0/etna/transforms/math/log.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/power.py` & `etna-2.6.0/etna/transforms/math/power.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/scalers.py` & `etna-2.6.0/etna/transforms/math/scalers.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/sklearn.py` & `etna-2.6.0/etna/transforms/math/sklearn.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/math/statistics.py` & `etna-2.6.0/etna/transforms/math/statistics.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/missing_values/imputation.py` & `etna-2.6.0/etna/transforms/missing_values/imputation.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/missing_values/resample.py` & `etna-2.6.0/etna/transforms/missing_values/resample.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,27 +40,35 @@
     def _get_folds(self, df: pd.DataFrame) -> List[int]:
         """
         Generate fold number for each timestamp of the dataframe.
 
         Here the ``in_column`` frequency gap is divided into the folds with the size of dataset frequency gap.
         """
         in_column_index = df[self.in_column].dropna().index
-        if len(in_column_index) <= 1 or (len(in_column_index) >= 3 and not pd.infer_freq(in_column_index)):
+
+        fail_datetime_timestamp = (
+            not pd.api.types.is_integer_dtype(in_column_index)
+            and len(in_column_index) >= 3
+            and not pd.infer_freq(in_column_index)
+        )
+        if len(in_column_index) <= 1 or fail_datetime_timestamp:
             raise ValueError(
-                "Can not infer in_column frequency!"
+                "Can not infer in_column frequency! "
                 "Check that in_column frequency is compatible with dataset frequency."
             )
+
         in_column_freq = in_column_index[1] - in_column_index[0]
         dataset_freq = df.index[1] - df.index[0]
+
         n_folds_per_gap = in_column_freq // dataset_freq
         n_periods = len(df) // n_folds_per_gap + 2
 
         in_column_start_index = in_column_index[0]
-        left_tie_len = len(df[:in_column_start_index]) - 1
-        right_tie_len = len(df[in_column_start_index:])
+        left_tie_len = len(df.loc[:in_column_start_index]) - 1
+        right_tie_len = len(df.loc[in_column_start_index:])
         folds_for_left_tie = list(range(n_folds_per_gap - left_tie_len, n_folds_per_gap))
         folds_for_right_tie = [fold for _ in range(n_periods) for fold in range(n_folds_per_gap)][:right_tie_len]
         return folds_for_left_tie + folds_for_right_tie
 
     def fit(self, df: pd.DataFrame) -> "_OneSegmentResampleWithDistributionTransform":
         """
         Obtain the resampling frequency and distribution from ``distribution_column``.
@@ -107,14 +115,23 @@
         """Inverse transform Dataframe."""
         return df
 
 
 class ResampleWithDistributionTransform(IrreversiblePerSegmentWrapper):
     """ResampleWithDistributionTransform resamples the given column using the distribution of the other column.
 
+    This transform expects ``in_column`` to have non-NaN values separated by the same number of timestamps to form a cycle.
+    The cycle starts with a non-NaN value and each position has a number from 0 to cycle size - 1.
+
+    During ``fit'', the fraction of each cycle position in a total sum of values is calculated according to ``distribution_column''.
+    During ``transform`` the NaNs within ``in_column`` are filled using the learned distribution.
+
+    The most common application of this transform is to fill NaNs in ``in_column`` that come from data with a different frequency.
+    For example, a dataset has an hourly frequency, but an exogenous variable has only a daily frequency.
+
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
 
     def __init__(
```

### Comparing `etna-2.5.0/etna/transforms/outliers/base.py` & `etna-2.6.0/etna/transforms/outliers/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 from abc import ABC
 from abc import abstractmethod
 from typing import Dict
 from typing import List
 from typing import Optional
+from typing import Union
 
 import numpy as np
 import pandas as pd
 from deprecated import deprecated
 
 from etna.datasets import TSDataset
 from etna.transforms.base import ReversibleTransform
 from etna.transforms.utils import check_new_segments
 
 
 class OutliersTransform(ReversibleTransform, ABC):
     """Finds outliers in specific columns of DataFrame and replaces it with NaNs."""
 
-    def __init__(self, in_column: str):
+    def __init__(self, in_column: str, ignore_flag_column: Optional[str] = None):
         """
         Create instance of OutliersTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
+        ignore_flag_column:
+            column name for skipping values from outlier check
         """
-        super().__init__(required_features=[in_column])
+        required_features = [in_column]
+        if ignore_flag_column:
+            required_features.append(ignore_flag_column)
+
+        super().__init__(required_features=required_features)
         self.in_column = in_column
+        self.ignore_flag_column = ignore_flag_column
 
         self.segment_outliers: Optional[Dict[str, pd.Series]] = None
 
         self._fit_segments: Optional[List[str]] = None
 
     @property
     @deprecated(
         reason="Attribute `outliers_timestamps` is deprecated and will be removed! Use `segment_outliers` instead.",
         version="3.0",
     )
-    def outliers_timestamps(self) -> Optional[Dict[str, List[pd.Timestamp]]]:
+    def outliers_timestamps(self) -> Union[Dict[str, List[pd.Timestamp]], Dict[str, List[int]], None]:
         """Backward compatibility property."""
         if self.segment_outliers is not None:
             return {segment: outliers.index.to_list() for segment, outliers in self.segment_outliers.items()}
         return None
 
     @property
     @deprecated(
         reason="Attribute `original_values` is deprecated and will be removed! Use `segment_outliers` instead.",
         version="3.0",
     )
-    def original_values(self) -> Optional[Dict[str, List[pd.Series]]]:
+    def original_values(self) -> Optional[Dict[str, pd.Series]]:
         """Backward compatibility property."""
         if self.segment_outliers is not None:
             return self.segment_outliers.copy()
         return None
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform.
@@ -60,32 +68,55 @@
         Returns
         -------
         :
             List with regressors created by the transform.
         """
         return []
 
+    def fit(self, ts: TSDataset) -> "OutliersTransform":
+        """Fit the transform.
+
+        Parameters
+        ----------
+        ts:
+            Dataset to fit the transform on.
+
+        Returns
+        -------
+        :
+            The fitted transform instance.
+        """
+        if self.ignore_flag_column is not None:
+            if self.ignore_flag_column not in ts.columns.get_level_values("feature"):
+                raise ValueError(f'Name ignore_flag_column="{self.ignore_flag_column}" not find.')
+            types_ignore_flag = ts[..., self.ignore_flag_column].isin([0, 1]).all(axis=0)
+            if not all(types_ignore_flag):
+                raise ValueError(
+                    f'Columns ignore_flag contain non binary value: columns: "{self.ignore_flag_column}" in segment: {types_ignore_flag[~types_ignore_flag].index.get_level_values("segment").tolist()}'
+                )
+
+        self.segment_outliers = self.detect_outliers(ts)
+        self._fit_segments = ts.segments
+        super().fit(ts=ts)
+        return self
+
     def _fit(self, df: pd.DataFrame) -> "OutliersTransform":
         """
         Find outliers using detection method.
 
         Parameters
         ----------
         df:
             dataframe with series to find outliers
 
         Returns
         -------
-        result: OutliersTransform
+        result:
             instance with saved outliers
         """
-        ts = TSDataset(df, freq=pd.infer_freq(df.index))
-        self.segment_outliers = self.detect_outliers(ts)
-        self._fit_segments = ts.segments
-
         return self
 
     def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Replace found outliers with NaNs.
 
         Parameters
@@ -112,16 +143,24 @@
         index_set = set(df.index.values)
 
         check_new_segments(transform_segments=segments, fit_segments=self._fit_segments)
         for segment in self.segment_outliers:
             if segment not in segments:
                 continue
             # to locate only present indices
-            segment_outliers_timestamps = list(index_set.intersection(self.segment_outliers[segment].index.values))
+            if self.ignore_flag_column:
+                available_points = set(df[df[segment, self.ignore_flag_column] == 0].index.values)
+            else:
+                available_points = index_set
+            segment_outliers_timestamps = list(
+                available_points.intersection(self.segment_outliers[segment].index.values)
+            )
+
             df.loc[segment_outliers_timestamps, pd.IndexSlice[segment, self.in_column]] = np.NaN
+
         return df
 
     def _inverse_transform(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Inverse transformation. Returns back deleted values.
 
         Parameters
```

### Comparing `etna-2.5.0/etna/transforms/outliers/point_outliers.py` & `etna-2.6.0/etna/transforms/outliers/point_outliers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Type
 from typing import Union
 
 import pandas as pd
 from typing_extensions import Literal
 
 from etna import SETTINGS
@@ -28,29 +29,37 @@
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
 
-    def __init__(self, in_column: str, window_size: int = 10, alpha: float = 3):
+    def __init__(
+        self,
+        in_column: str,
+        window_size: int = 10,
+        alpha: float = 3,
+        ignore_flag_column: Optional[str] = None,
+    ):
         """Create instance of MedianOutliersTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
         window_size:
             number of points in the window
         alpha:
             coefficient for determining the threshold
+        ignore_flag_column:
+            column name for skipping values from outlier check
         """
         self.window_size = window_size
         self.alpha = alpha
-        super().__init__(in_column=in_column)
+        super().__init__(in_column=in_column, ignore_flag_column=ignore_flag_column)
 
     def detect_outliers(self, ts: TSDataset) -> Dict[str, List[pd.Timestamp]]:
         """Call :py:func:`~etna.analysis.outliers.median_outliers.get_anomalies_median` function with self parameters.
 
         Parameters
         ----------
         ts:
@@ -93,14 +102,15 @@
     def __init__(
         self,
         in_column: str,
         window_size: int = 15,
         distance_coef: float = 3,
         n_neighbors: int = 3,
         distance_func: Union[Literal["absolute_difference"], Callable[[float, float], float]] = "absolute_difference",
+        ignore_flag_column: Optional[str] = None,
     ):
         """Create instance of DensityOutliersTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
@@ -109,20 +119,22 @@
         distance_coef:
             factor for standard deviation that forms distance threshold to determine points are close to each other
         n_neighbors:
             min number of close neighbors of point not to be outlier
         distance_func:
             distance function. If a string is specified, a corresponding vectorized implementation will be used.
             Custom callable will be used as a scalar function, which will result in worse performance.
+        ignore_flag_column:
+            column name for skipping values from outlier check
         """
         self.window_size = window_size
         self.distance_coef = distance_coef
         self.n_neighbors = n_neighbors
         self.distance_func = distance_func
-        super().__init__(in_column=in_column)
+        super().__init__(in_column=in_column, ignore_flag_column=ignore_flag_column)
 
     def detect_outliers(self, ts: TSDataset) -> Dict[str, List[pd.Timestamp]]:
         """Call :py:func:`~etna.analysis.outliers.density_outliers.get_anomalies_density` function with self parameters.
 
         Parameters
         ----------
         ts:
@@ -165,36 +177,38 @@
     """Transform that uses :py:func:`~etna.analysis.outliers.prediction_interval_outliers.get_anomalies_prediction_interval` to find anomalies in data."""
 
     def __init__(
         self,
         in_column: str,
         model: Union[Literal["prophet"], Literal["sarimax"], Type["ProphetModel"], Type["SARIMAXModel"]],
         interval_width: float = 0.95,
+        ignore_flag_column: Optional[str] = None,
         **model_kwargs,
     ):
         """Create instance of PredictionIntervalOutliersTransform.
 
         Parameters
         ----------
         in_column:
             name of processed column
         model:
             model for prediction interval estimation
         interval_width:
             width of the prediction interval
-
+        ignore_flag_column:
+            column name for skipping values from outlier check
         Notes
         -----
         For not "target" column only column data will be used for learning.
         """
         self.model = model
         self.interval_width = interval_width
         self.model_kwargs = model_kwargs
         self._model_type = self._get_model_type(model)
-        super().__init__(in_column=in_column)
+        super().__init__(in_column=in_column, ignore_flag_column=ignore_flag_column)
 
     @staticmethod
     def _get_model_type(
         model: Union[Literal["prophet"], Literal["sarimax"], Type["ProphetModel"], Type["SARIMAXModel"]]
     ) -> Union[Type["ProphetModel"], Type["SARIMAXModel"]]:
         if isinstance(model, str):
             if model == "prophet":
```

### Comparing `etna-2.5.0/etna/transforms/timestamp/date_flags.py` & `etna-2.6.0/etna/transforms/timestamp/date_flags.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from typing import List
 from typing import Optional
 from typing import Sequence
 
 import numpy as np
 import pandas as pd
 
+from etna.datasets import TSDataset
+from etna.datasets import duplicate_data
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.transforms.base import IrreversibleTransform
 
 
 class DateFlagsTransform(IrreversibleTransform):
     """DateFlagsTransform is a class that implements extraction of the main date-based features from datetime column.
@@ -43,14 +45,15 @@
         month_number_in_year: Optional[bool] = False,
         season_number: Optional[bool] = False,
         year_number: Optional[bool] = False,
         is_weekend: Optional[bool] = True,
         special_days_in_week: Sequence[int] = (),
         special_days_in_month: Sequence[int] = (),
         out_column: Optional[str] = None,
+        in_column: Optional[str] = None,
     ):
         """Create instance of DateFlags.
 
         Parameters
         ----------
         day_number_in_week:
             if True, add column with weekday info to feature dataframe in transform
@@ -80,14 +83,21 @@
             base for the name of created columns;
 
             * if set the final name is '{out_column}_{feature_name}';
 
             * if don't set, name will be ``transform.__repr__()``,
               repr will be made for transform that creates exactly this column
 
+        in_column:
+            name of column to work with; if not given, index is used, only datetime index is supported
+
+        Raises
+        ------
+        ValueError:
+            if all features aren't set in transform
         """
         if not any(
             [
                 day_number_in_week,
                 day_number_in_month,
                 day_number_in_year,
                 week_number_in_month,
@@ -102,29 +112,41 @@
         ):
             raise ValueError(
                 f"{type(self).__name__} feature does nothing with given init args configuration, "
                 f"at least one of day_number_in_week, day_number_in_month, day_number_in_year, week_number_in_month, "
                 f"week_number_in_year, month_number_in_year, season_number, year_number, is_weekend should be True or any of "
                 f"special_days_in_week, special_days_in_month should be not empty."
             )
-        super().__init__(required_features=["target"])
+
+        if in_column is None:
+            required_features = ["target"]
+        else:
+            required_features = [in_column]
+        super().__init__(required_features=required_features)
+
         self.day_number_in_week = day_number_in_week
         self.day_number_in_month = day_number_in_month
         self.day_number_in_year = day_number_in_year
         self.week_number_in_month = week_number_in_month
         self.week_number_in_year = week_number_in_year
         self.month_number_in_year = month_number_in_year
         self.season_number = season_number
         self.year_number = year_number
         self.is_weekend = is_weekend
 
         self.special_days_in_week = special_days_in_week
         self.special_days_in_month = special_days_in_month
 
         self.out_column = out_column
+        self.in_column = in_column
+
+        if self.in_column is None:
+            self.in_column_regressor: Optional[bool] = True
+        else:
+            self.in_column_regressor = None
 
         # create empty init parameters
         self._empty_parameters = dict(
             day_number_in_week=False,
             day_number_in_month=False,
             day_number_in_year=False,
             week_number_in_month=False,
@@ -144,14 +166,20 @@
             temp_transform = DateFlagsTransform(**init_parameters, out_column=self.out_column)  # type: ignore
             return temp_transform.__repr__()
         else:
             return f"{self.out_column}_{feature_name}"
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+
+        if not self.in_column_regressor:
+            return []
+
         features = [
             "day_number_in_week",
             "day_number_in_month",
             "day_number_in_year",
             "week_number_in_month",
             "week_number_in_year",
             "month_number_in_year",
@@ -162,98 +190,122 @@
             "special_days_in_month",
         ]
         output_columns = [
             self._get_column_name(feature_name=feature_name) for feature_name in features if getattr(self, feature_name)
         ]
         return output_columns
 
+    def fit(self, ts: TSDataset) -> "DateFlagsTransform":
+        """Fit the transform."""
+        if self.in_column is None:
+            self.in_column_regressor = True
+        else:
+            self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
     def _fit(self, df: pd.DataFrame) -> "DateFlagsTransform":
         """Fit model. In this case of DateFlags does nothing."""
         return self
 
-    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """Get required features from df.
-
-        Parameters
-        ----------
-        df:
-            dataframe for feature extraction, should contain 'timestamp' column
-
-        Returns
-        -------
-        :
-            dataframe with extracted features
-        """
-        features = pd.DataFrame(index=df.index)
-        timestamp_series = pd.Series(df.index)
+    def _compute_features(self, timestamps: pd.Series) -> pd.DataFrame:
+        timestamps_no_nans = timestamps.dropna()
+        features = pd.DataFrame(index=timestamps_no_nans.index)
 
         if self.day_number_in_week:
             features[self._get_column_name("day_number_in_week")] = self._get_day_number_in_week(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.day_number_in_month:
             features[self._get_column_name("day_number_in_month")] = self._get_day_number_in_month(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.day_number_in_year:
             features[self._get_column_name("day_number_in_year")] = self._get_day_number_in_year(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.week_number_in_month:
             features[self._get_column_name("week_number_in_month")] = self._get_week_number_in_month(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.week_number_in_year:
             features[self._get_column_name("week_number_in_year")] = self._get_week_number_in_year(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.month_number_in_year:
             features[self._get_column_name("month_number_in_year")] = self._get_month_number_in_year(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.season_number:
             features[self._get_column_name("season_number")] = self._get_season_number(
-                timestamp_series=timestamp_series
+                timestamp_series=timestamps_no_nans
             )
 
         if self.year_number:
-            features[self._get_column_name("year_number")] = self._get_year(timestamp_series=timestamp_series)
+            features[self._get_column_name("year_number")] = self._get_year(timestamp_series=timestamps_no_nans)
 
         if self.is_weekend:
-            features[self._get_column_name("is_weekend")] = self._get_weekends(timestamp_series=timestamp_series)
+            features[self._get_column_name("is_weekend")] = self._get_weekends(timestamp_series=timestamps_no_nans)
 
         if self.special_days_in_week:
             features[self._get_column_name("special_days_in_week")] = self._get_special_day_in_week(
-                special_days=self.special_days_in_week, timestamp_series=timestamp_series
+                special_days=self.special_days_in_week, timestamp_series=timestamps_no_nans
             )
 
         if self.special_days_in_month:
             features[self._get_column_name("special_days_in_month")] = self._get_special_day_in_month(
-                special_days=self.special_days_in_month, timestamp_series=timestamp_series
+                special_days=self.special_days_in_month, timestamp_series=timestamps_no_nans
             )
 
         for feature in features.columns:
             features[feature] = features[feature].astype("category")
 
-        dataframes = []
-        for seg in df.columns.get_level_values("segment").unique():
-            tmp = df[seg].join(features)
-            _idx = tmp.columns.to_frame()
-            _idx.insert(0, "segment", seg)
-            tmp.columns = pd.MultiIndex.from_frame(_idx)
-            dataframes.append(tmp)
+        # add NaNs in features
+        features = features.reindex(timestamps.index)
+
+        return features
+
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Get required features from df.
+
+        Parameters
+        ----------
+        df:
+            dataframe for feature extraction, should contain 'timestamp' column
+
+        Returns
+        -------
+        :
+            dataframe with extracted features
+        """
+        if self.in_column is None:
+            if pd.api.types.is_integer_dtype(df.index.dtype):
+                raise ValueError("Transform can't work with integer index, parameter in_column should be set!")
+
+            timestamps = pd.Series(df.index)
+            features = self._compute_features(timestamps=timestamps)
+            features.index = df.index
+
+            segments = df.columns.get_level_values("segment").unique().tolist()
+            result = duplicate_data(df=features.reset_index(), segments=segments)
+            result = pd.concat([df, result], axis=1).sort_index(axis=1)
+        else:
+            flat_df = TSDataset.to_flatten(df=df, features=[self.in_column])
+            features = self._compute_features(timestamps=flat_df[self.in_column])
+            features["timestamp"] = flat_df["timestamp"]
+            features["segment"] = flat_df["segment"]
+            wide_df = TSDataset.to_dataset(features)
+            result = pd.concat([df, wide_df], axis=1).sort_index(axis=1)
 
-        result = pd.concat(dataframes, axis=1).sort_index(axis=1)
-        result.columns.names = ["segment", "feature"]
         return result
 
     @staticmethod
     def _get_special_day_in_week(special_days: Sequence[int], timestamp_series: pd.Series) -> np.ndarray:
         """Return array with special days marked 1.
 
         Accepts a list of special days IN WEEK as input and returns array where these days are marked with 1
```

### Comparing `etna-2.5.0/etna/transforms/timestamp/event.py` & `etna-2.6.0/etna/transforms/timestamp/event.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/etna/transforms/timestamp/special_days.py` & `etna-2.6.0/etna/transforms/timestamp/special_days.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import pandas as pd
 
+from etna.datasets import TSDataset
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.transforms.base import IrreversiblePerSegmentWrapper
 from etna.transforms.base import OneSegmentTransform
 
 
 def calc_day_number_in_week(datetime_day: datetime.datetime) -> int:
@@ -27,24 +28,28 @@
 
     Notes
     -----
     You can read more about other anomalies detection methods in:
     `Time Series of Price Anomaly Detection <https://towardsdatascience.com/time-series-of-price-anomaly-detection-13586cd5ff46>`_
     """
 
-    def __init__(self, find_special_weekday: bool = True, find_special_month_day: bool = True):
+    def __init__(
+        self, find_special_weekday: bool = True, find_special_month_day: bool = True, in_column: Optional[str] = None
+    ):
         """
         Create instance of _OneSegmentSpecialDaysTransform.
 
         Parameters
         ----------
         find_special_weekday:
             flag, if True, find special weekdays in transform
         find_special_month_day:
             flag, if True, find special monthdays in transform
+        in_column:
+            name of column to work with; if not given, index is used, only datetime index is supported
 
         Raises
         ------
         ValueError:
             if all the modes are False
         """
         if not any([find_special_weekday, find_special_month_day]):
@@ -55,14 +60,16 @@
 
         self.find_special_weekday = find_special_weekday
         self.find_special_month_day = find_special_month_day
 
         self.anomaly_week_days: Optional[Tuple[int]] = None
         self.anomaly_month_days: Optional[Tuple[int]] = None
 
+        self.in_column = in_column
+
         self.res_type: Dict[str, Any]
         if self.find_special_weekday and find_special_month_day:
             self.res_type = {"df_sample": (0, 0), "columns": ["anomaly_weekdays", "anomaly_monthdays"]}
         elif self.find_special_weekday:
             self.res_type = {"df_sample": 0, "columns": ["anomaly_weekdays"]}
         elif self.find_special_month_day:
             self.res_type = {"df_sample": 0, "columns": ["anomaly_monthdays"]}
@@ -74,17 +81,25 @@
         Fit _OneSegmentSpecialDaysTransform with data from df.
 
         Parameters
         ----------
         df: pd.DataFrame
             value series with index column in timestamp format
         """
-        common_df = df[["target"]].reset_index()
+        if self.in_column is None:
+            if pd.api.types.is_integer_dtype(df.index.dtype):
+                raise ValueError("Transform can't work with integer index, parameter in_column should be set!")
+
+            common_df = df[["target"]].reset_index()
+        else:
+            common_df = df[[self.in_column, "target"]]
         common_df.columns = ["datetime", "value"]
 
+        common_df = common_df.dropna()
+
         if self.find_special_weekday:
             self.anomaly_week_days = self._find_anomaly_day_in_week(common_df)
 
         if self.find_special_month_day:
             self.anomaly_month_days = self._find_anomaly_day_in_month(common_df)
         return self
 
@@ -99,31 +114,42 @@
 
         Returns
         -------
         :
             pd.DataFrame with 'anomaly_weekday', 'anomaly_monthday' or both of them columns no-timestamp indexed that
             contains 1 at i-th position if i-th day is a special day
         """
-        common_df = df[["target"]].reset_index()
+        if self.in_column is None:
+            common_df = df[["target"]].reset_index()
+        else:
+            common_df = df[[self.in_column, "target"]].reset_index(drop=True)
         common_df.columns = ["datetime", "value"]
+        common_df_no_nans = common_df.dropna()
 
-        to_add = pd.DataFrame([self.res_type["df_sample"]] * len(df), columns=self.res_type["columns"])
+        to_add = pd.DataFrame(
+            [self.res_type["df_sample"]] * len(common_df_no_nans),
+            columns=self.res_type["columns"],
+            index=common_df_no_nans.index,
+        )
 
         if self.find_special_weekday:
             if self.anomaly_week_days is None:
                 raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
-            to_add["anomaly_weekdays"] += self._marked_special_week_day(common_df, self.anomaly_week_days)
+            to_add["anomaly_weekdays"] += self._marked_special_week_day(common_df_no_nans, self.anomaly_week_days)
             to_add["anomaly_weekdays"] = to_add["anomaly_weekdays"].astype("category")
 
         if self.find_special_month_day:
             if self.anomaly_month_days is None:
                 raise ValueError("Transform is not fitted! Fit the Transform before calling transform method.")
-            to_add["anomaly_monthdays"] += self._marked_special_month_day(common_df, self.anomaly_month_days)
+            to_add["anomaly_monthdays"] += self._marked_special_month_day(common_df_no_nans, self.anomaly_month_days)
             to_add["anomaly_monthdays"] = to_add["anomaly_monthdays"].astype("category")
 
+        # add NaNs in features
+        to_add = to_add.reindex(common_df.index)
+
         to_add.index = df.index
         to_return = pd.concat([df, to_add], axis=1)
         to_return.columns.names = df.columns.names
         return to_return
 
     @staticmethod
     def _find_anomaly_day_in_week(df: pd.DataFrame, agg_func=pd.core.groupby.SeriesGroupBy.mean) -> Tuple[int]:
@@ -181,39 +207,73 @@
 
     Warning
     -------
     This transform can suffer from look-ahead bias. For transforming data at some timestamp
     it uses information from the whole train part.
     """
 
-    def __init__(self, find_special_weekday: bool = True, find_special_month_day: bool = True):
+    def __init__(
+        self, find_special_weekday: bool = True, find_special_month_day: bool = True, in_column: Optional[str] = None
+    ):
         """
         Create instance of SpecialDaysTransform.
 
         Parameters
         ----------
         find_special_weekday:
             flag, if True, find special weekdays in transform
         find_special_month_day:
             flag, if True, find special monthdays in transform
+        in_column:
+            name of column to work with; if not given, index is used, only datetime index is supported
 
         Raises
         ------
         ValueError:
             if all the modes are False
         """
         self.find_special_weekday = find_special_weekday
         self.find_special_month_day = find_special_month_day
+        self.in_column = in_column
+
+        if self.in_column is None:
+            self.in_column_regressor: Optional[bool] = True
+        else:
+            self.in_column_regressor = None
+
+        if in_column is None:
+            required_features = ["target"]
+        else:
+            required_features = [in_column, "target"]
         super().__init__(
-            transform=_OneSegmentSpecialDaysTransform(self.find_special_weekday, self.find_special_month_day),
-            required_features=["target"],
+            transform=_OneSegmentSpecialDaysTransform(
+                find_special_weekday=self.find_special_weekday,
+                find_special_month_day=self.find_special_month_day,
+                in_column=self.in_column,
+            ),
+            required_features=required_features,
         )
 
+    def fit(self, ts: TSDataset) -> "SpecialDaysTransform":
+        """Fit the transform."""
+        if self.in_column is None:
+            self.in_column_regressor = True
+        else:
+            self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+
+        if not self.in_column_regressor:
+            return []
+
         output_columns = []
         if self.find_special_weekday:
             output_columns.append("anomaly_weekdays")
         if self.find_special_month_day:
             output_columns.append("anomaly_monthdays")
         return output_columns
```

### Comparing `etna-2.5.0/etna/transforms/timestamp/time_flags.py` & `etna-2.6.0/etna/transforms/timestamp/time_flags.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
+from etna.datasets import TSDataset
+from etna.datasets import duplicate_data
 from etna.distributions import BaseDistribution
 from etna.distributions import CategoricalDistribution
 from etna.transforms.base import IrreversibleTransform
 
 
 class TimeFlagsTransform(IrreversibleTransform):
     """TimeFlagsTransform is a class that implements extraction of the main time-based features from datetime column."""
@@ -19,14 +21,15 @@
         minute_in_hour_number: bool = True,
         fifteen_minutes_in_hour_number: bool = False,
         hour_number: bool = True,
         half_hour_number: bool = False,
         half_day_number: bool = False,
         one_third_day_number: bool = False,
         out_column: Optional[str] = None,
+        in_column: Optional[str] = None,
     ):
         """Initialise class attributes.
 
         Parameters
         ----------
         minute_in_hour_number:
             if True: add column with minute number to feature dataframe in transform
@@ -48,17 +51,21 @@
             base for the name of created columns;
 
             * if set the final name is '{out_column}_{feature_name}';
 
             * if don't set, name will be ``transform.__repr__()``,
               repr will be made for transform that creates exactly this column
 
+        in_column:
+            name of column to work with; if not given, index is used, only datetime index is supported
+
         Raises
         ------
-        ValueError: if feature has invalid initial params
+        ValueError:
+            if all features aren't set in transform
         """
         if not any(
             [
                 minute_in_hour_number,
                 fifteen_minutes_in_hour_number,
                 hour_number,
                 half_hour_number,
@@ -67,24 +74,36 @@
             ]
         ):
             raise ValueError(
                 f"{type(self).__name__} feature does nothing with given init args configuration, "
                 f"at least one of minute_in_hour_number, fifteen_minutes_in_hour_number, hour_number, "
                 f"half_hour_number, half_day_number, one_third_day_number should be True."
             )
-        super().__init__(required_features=["target"])
+
+        if in_column is None:
+            required_features = ["target"]
+        else:
+            required_features = [in_column]
+        super().__init__(required_features=required_features)
+
         self.date_column_name = None
         self.minute_in_hour_number: bool = minute_in_hour_number
         self.fifteen_minutes_in_hour_number: bool = fifteen_minutes_in_hour_number
         self.hour_number: bool = hour_number
         self.half_hour_number: bool = half_hour_number
         self.half_day_number: bool = half_day_number
         self.one_third_day_number: bool = one_third_day_number
 
         self.out_column = out_column
+        self.in_column = in_column
+
+        if self.in_column is None:
+            self.in_column_regressor: Optional[bool] = True
+        else:
+            self.in_column_regressor = None
 
         # create empty init parameters
         self._empty_parameters = dict(
             minute_in_hour_number=False,
             fifteen_minutes_in_hour_number=False,
             hour_number=False,
             half_hour_number=False,
@@ -99,87 +118,118 @@
             temp_transform = TimeFlagsTransform(**init_parameters, out_column=self.out_column)  # type: ignore
             return repr(temp_transform)
         else:
             return f"{self.out_column}_{feature_name}"
 
     def get_regressors_info(self) -> List[str]:
         """Return the list with regressors created by the transform."""
+        if self.in_column_regressor is None:
+            raise ValueError("Fit the transform to get the correct regressors info!")
+
+        if not self.in_column_regressor:
+            return []
+
         features = [
             "minute_in_hour_number",
             "fifteen_minutes_in_hour_number",
             "hour_number",
             "half_hour_number",
             "half_day_number",
             "one_third_day_number",
         ]
         output_columns = [
             self._get_column_name(feature_name=feature_name) for feature_name in features if getattr(self, feature_name)
         ]
         return output_columns
 
+    def fit(self, ts: TSDataset) -> "TimeFlagsTransform":
+        """Fit the transform."""
+        if self.in_column is None:
+            self.in_column_regressor = True
+        else:
+            self.in_column_regressor = self.in_column in ts.regressors
+        super().fit(ts)
+        return self
+
     def _fit(self, *args, **kwargs) -> "TimeFlagsTransform":
         """Fit datetime model."""
         return self
 
-    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transform method for features based on time.
-
-        Parameters
-        ----------
-        df:
-            Features dataframe with time
-
-        Returns
-        -------
-        result: pd.DataFrame
-            Dataframe with extracted features
-        """
-        features = pd.DataFrame(index=df.index)
-        timestamp_series = pd.Series(df.index)
+    def _compute_features(self, timestamps: pd.Series) -> pd.DataFrame:
+        timestamps_no_nans = timestamps.dropna()
+        features = pd.DataFrame(index=timestamps_no_nans.index)
 
         if self.minute_in_hour_number:
-            minute_in_hour_number = self._get_minute_number(timestamp_series=timestamp_series)
+            minute_in_hour_number = self._get_minute_number(timestamp_series=timestamps_no_nans)
             features[self._get_column_name("minute_in_hour_number")] = minute_in_hour_number
 
         if self.fifteen_minutes_in_hour_number:
             fifteen_minutes_in_hour_number = self._get_period_in_hour(
-                timestamp_series=timestamp_series, period_in_minutes=15
+                timestamp_series=timestamps_no_nans, period_in_minutes=15
             )
             features[self._get_column_name("fifteen_minutes_in_hour_number")] = fifteen_minutes_in_hour_number
 
         if self.hour_number:
-            hour_number = self._get_hour_number(timestamp_series=timestamp_series)
+            hour_number = self._get_hour_number(timestamp_series=timestamps_no_nans)
             features[self._get_column_name("hour_number")] = hour_number
 
         if self.half_hour_number:
-            half_hour_number = self._get_period_in_hour(timestamp_series=timestamp_series, period_in_minutes=30)
+            half_hour_number = self._get_period_in_hour(timestamp_series=timestamps_no_nans, period_in_minutes=30)
             features[self._get_column_name("half_hour_number")] = half_hour_number
 
         if self.half_day_number:
-            half_day_number = self._get_period_in_day(timestamp_series=timestamp_series, period_in_hours=12)
+            half_day_number = self._get_period_in_day(timestamp_series=timestamps_no_nans, period_in_hours=12)
             features[self._get_column_name("half_day_number")] = half_day_number
 
         if self.one_third_day_number:
-            one_third_day_number = self._get_period_in_day(timestamp_series=timestamp_series, period_in_hours=8)
+            one_third_day_number = self._get_period_in_day(timestamp_series=timestamps_no_nans, period_in_hours=8)
             features[self._get_column_name("one_third_day_number")] = one_third_day_number
 
         for feature in features.columns:
             features[feature] = features[feature].astype("category")
 
-        dataframes = []
-        for seg in df.columns.get_level_values("segment").unique():
-            tmp = df[seg].join(features)
-            _idx = tmp.columns.to_frame()
-            _idx.insert(0, "segment", seg)
-            tmp.columns = pd.MultiIndex.from_frame(_idx)
-            dataframes.append(tmp)
+        # add NaNs in features
+        features = features.reindex(timestamps.index)
+
+        return features
+
+    def _transform(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transform method for features based on time.
+
+        Parameters
+        ----------
+        df:
+            Features dataframe with time
+
+        Returns
+        -------
+        :
+            Dataframe with extracted features
+        """
+        if self.in_column is None:
+            if pd.api.types.is_integer_dtype(df.index.dtype):
+                raise ValueError("Transform can't work with integer index, parameter in_column should be set!")
+
+            timestamps = pd.Series(df.index)
+            features = self._compute_features(timestamps=timestamps)
+            features.index = df.index
+
+            segments = df.columns.get_level_values("segment").unique().tolist()
+            result = duplicate_data(df=features.reset_index(), segments=segments)
+            result = pd.concat([df, result], axis=1).sort_index(axis=1)
+
+        else:
+            flat_df = TSDataset.to_flatten(df=df, features=[self.in_column])
+            features = self._compute_features(timestamps=flat_df[self.in_column])
+            features["timestamp"] = flat_df["timestamp"]
+            features["segment"] = flat_df["segment"]
+            wide_df = TSDataset.to_dataset(features)
+            result = pd.concat([df, wide_df], axis=1).sort_index(axis=1)
 
-        result = pd.concat(dataframes, axis=1).sort_index(axis=1)
-        result.columns.names = ["segment", "feature"]
         return result
 
     @staticmethod
     def _get_minute_number(timestamp_series: pd.Series) -> np.ndarray:
         """Generate array with the minute number in the hour."""
         return timestamp_series.apply(lambda x: x.minute).values
```

### Comparing `etna-2.5.0/etna/transforms/utils.py` & `etna-2.6.0/etna/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `etna-2.5.0/pyproject.toml` & `etna-2.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "etna"
-version = "2.5.0"
+version = "2.6.0"
 repository = "https://github.com/etna-team/etna"
 readme = "README.md"
 description = "ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun."
 license = "Apache-2.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -126,15 +126,15 @@
 auto = ["optuna", "sqlalchemy"]
 classification = ["pyts", "tsfresh"]
 statsforecast = ["statsforecast"]
 # dev deps
 release = ["click", "semver"]
 docs = ["Sphinx", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython", "pydata-sphinx-theme", "sphinx-design", "jupyter"]
 tests = ["pytest-cov", "pytest", "pytest-shard"]
-jupyter = ["jupyter", "nbconvert", "black"]
+jupyter = ["jupyter", "nbconvert", "black", "ipywidgets"]
 style = ["black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools", "nbqa"]
 
 all = [
     "prophet",
     "torch", "pytorch-forecasting", "pytorch-lightning",
     "wandb",
     "optuna", "sqlalchemy",
@@ -148,15 +148,15 @@
     "wandb",
     "optuna", "sqlalchemy",
     "click", "semver",
     "Sphinx", "nbsphinx", "sphinx-mathjax-offline", "myst-parser", "GitPython", "pydata-sphinx-theme", "sphinx-design",
     "pytest-cov", "pytest", "pytest-shard",
     "black", "isort", "flake8", "pep8-naming", "flake8-docstrings", "mypy", "types-PyYAML", "codespell", "flake8-bugbear", "flake8-comprehensions", "types-setuptools", "nbqa",
     "click", "semver",
-    "jupyter", "nbconvert",
+    "jupyter", "nbconvert", "ipywidgets",
     "pyts", "tsfresh",
     "statsforecast"
 ]
 
 [tool.poetry.scripts]
 etna = "etna.commands.__main__:app"
 
@@ -198,15 +198,15 @@
     "error",
     "ignore: pkg_resources is deprecated as an API",
     "ignore: Deprecated call to `pkg_resources.declare_namespace",
     # etna warnings
     "ignore: TSDataset freq can't be inferred",
     "ignore: You probably set wrong freq. Discovered freq in you data",
     "ignore: Option `fast_redundancy=False` was added for backward compatibility and will be removed in etna 3.0.0.",
-    "ignore: Some regressors don't have enough values in segment",
+    "ignore: Some regressors don't have enough values",
     "ignore: Segments contains NaNs in the last timestamps",
     "ignore: Given top_k=.* is bigger than n_features=.*. Transform will not filter",
     "ignore: Given top_k=.* is less than n_segments=.*. Algo will filter data without Gale-Shapley run.",
     "ignore: This model doesn't work with exogenous features",
     "ignore: Some of external objects in input parameters could be not",
     # external warnings
     "ignore: Attribute 'logging_metrics' is an instance of `nn.Module` and is already",
@@ -241,15 +241,17 @@
     "ignore: Optimization did not converge :tbats.error.ModelWarning.ModelWarning",
     "ignore: The behavior of Timestamp.utcfromtimestamp is deprecated", # prophet
     "ignore: Starting from v1.9.0, `tensorboardX` has been removed as a dependency",
     "ignore: the `interpolation=` argument to percentile was renamed to `method=`", # pandas: old version uses deprecated numpy parameter
     "ignore: Trying to infer the `batch_size` from an ambiguous collection", # pytorch_forecasting
     "ignore: Implicitly cleaning up <TemporaryDirectory",
     "ignore: Call to deprecated class DeepARModel.",
-    "ignore: dropout option adds dropout after all but last recurrent layer"
+    "ignore: dropout option adds dropout after all but last recurrent layer",
+    "ignore: Call to deprecated class TFTModel."
+
 ]
 markers = [
     "smoke"
 ]
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `etna-2.5.0/PKG-INFO` & `etna-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etna
-Version: 2.5.0
+Version: 2.6.0
 Summary: ETNA is the first python open source framework of Tinkoff.ru AI Center. It is designed to make working with time series simple, productive, and fun.
 Home-page: https://github.com/etna-team/etna
 License: Apache-2.0
 Author: Andrey Alekseev
 Author-email: ilekseev@gmail.com
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,15 +48,15 @@
 Requires-Dist: flake8 (>=3.9.2,<4.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-bugbear (>=22.4.25,<23.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-comprehensions (>=3.9.0,<4.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: flake8-docstrings (>=1.6.0,<2.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: holidays (>=0.13,<1.0)
 Requires-Dist: hydra-slayer (>=0.2.0,<0.3.0)
 Requires-Dist: hydra_slayer
-Requires-Dist: ipywidgets (>=7.6.5,<8.0.0)
+Requires-Dist: ipywidgets (>=7.6.5,<8.0.0) ; extra == "jupyter" or extra == "all-dev"
 Requires-Dist: isort (>=5.8.0,<6.0.0) ; extra == "style" or extra == "all-dev"
 Requires-Dist: joblib
 Requires-Dist: jupyter ; extra == "docs" or extra == "jupyter" or extra == "all-dev"
 Requires-Dist: loguru (>=0.5.3,<0.6.0)
 Requires-Dist: matplotlib
 Requires-Dist: mypy (>=0.950,<2) ; extra == "style" or extra == "all-dev"
 Requires-Dist: myst-parser (>=1.0,<2.0) ; extra == "docs" or extra == "all-dev"
@@ -155,15 +155,14 @@
 import pandas as pd
 from etna.datasets import TSDataset
 
 # Read the data
 df = pd.read_csv("examples/data/example_dataset.csv")
 
 # Create a TSDataset
-df = TSDataset.to_dataset(df)
 ts = TSDataset(df, freq="D")
 
 # Choose a horizon
 HORIZON = 14
 
 # Make train/test split
 train_ts, test_ts = ts.train_test_split(test_size=HORIZON)
@@ -293,17 +292,18 @@
 | [Clustering](https://github.com/etna-team/etna/tree/master/examples/206-clustering.ipynb)                                   |                 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/206-clustering.ipynb) |
 | [Feature selection](https://github.com/etna-team/etna/blob/master/examples/207-feature_selection.ipynb)                     |          [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/207-feature_selection.ipynb) |
 | [Forecasting strategies](https://github.com/etna-team/etna/tree/master/examples/208-forecasting_strategies.ipynb)           |     [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/208-forecasting_strategies.ipynb) |
 | [Mechanics of forecasting](https://github.com/etna-team/etna/blob/master/examples/209-mechanics_of_forecasting.ipynb)       |   [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/209-mechanics_of_forecasting.ipynb) |
 | [Custom model and transform](https://github.com/etna-team/etna/tree/master/examples/301-custom_transform_and_model.ipynb)   | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/301-custom_transform_and_model.ipynb) |
 | [Inference: using saved pipeline on a new data](https://github.com/etna-team/etna/tree/master/examples/302-inference.ipynb) |                  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/302-inference.ipynb) |
 | [Hierarchical time series](https://github.com/etna-team/etna/blob/master/examples/303-hierarchical_pipeline.ipynb)          |      [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/303-hierarchical_pipeline.ipynb) |
-| [Forecast interpretation](https://github.com/etna-team/etna/tree/master/examples/304-forecasting_interpretation.ipynb)         |    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/304-forecasting_interpretation.ipynb) |
+| [Forecast interpretation](https://github.com/etna-team/etna/tree/master/examples/304-forecasting_interpretation.ipynb)      |    [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/304-forecasting_interpretation.ipynb) |
 | [Classification](https://github.com/etna-team/etna/blob/master/examples/305-classification.ipynb)                           |             [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/305-classification.ipynb) |
 | [Prediction intervals](https://github.com/etna-team/etna/tree/master/examples/306-prediction_intervals.ipynb)               |       [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/306-prediction_intervals.ipynb) |
+| [Working with misaligned data](https://github.com/etna-team/etna/tree/master/examples/307-working_with_misaligned_data.ipynb)       |       [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/etna-team/etna/master?filepath=examples/307-working_with_misaligned_data.ipynb) |
 
 ## Documentation
 
 ETNA documentation is available [here](https://docs.etna.ai/stable/).
 
 ## Community
```

