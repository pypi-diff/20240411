# Comparing `tmp/sarus_data_spec_public-3.9.2.dev0.tar.gz` & `tmp/sarus_data_spec_public-4.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus_data_spec_public-3.9.2.dev0.tar", last modified: Fri Mar  8 09:25:44 2024, max compression
+gzip compressed data, was "sarus_data_spec_public-4.0.0.dev5.tar", last modified: Thu Apr 11 11:03:02 2024, max compression
```

## Comparing `sarus_data_spec_public-3.9.2.dev0.tar` & `sarus_data_spec_public-4.0.0.dev5.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.438304 sarus_data_spec_public-3.9.2.dev0/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      436 2024-03-08 09:25:44.438304 sarus_data_spec_public-3.9.2.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.401305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/
--rwxrwxrwx   0 root         (0) root         (0)      830 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.403305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7713 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/admin_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/array.py
--rw-rw-rw-   0 root         (0) root         (0)     7264 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2101 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/pandas_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/type.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/attribute.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/bounds.py
--rw-rw-rw-   0 root         (0) root         (0)     4160 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.404305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/public.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/state.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    21711 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.405305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4931 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    22981 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
--rw-rw-rw-   0 root         (0) root         (0)    11623 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.407305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17255 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py
--rw-rw-rw-   0 root         (0) root         (0)      815 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py
--rw-rw-rw-   0 root         (0) root         (0)     5717 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py
--rw-rw-rw-   0 root         (0) root         (0)    28914 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/signature.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5403 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     8849 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/deprecation.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/json_serialisation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.408305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7628 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/async_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32013 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/cache_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.409304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.409304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3892 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.410305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/remote/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/remote/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3302 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/remote/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.410305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7087 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.410305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.413304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23049 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py
--rw-rw-rw-   0 root         (0) root         (0)     3011 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py
--rw-rw-rw-   0 root         (0) root         (0)    10321 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)    21505 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.414305 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
--rw-rw-rw-   0 root         (0) root         (0)    31295 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
--rw-rw-rw-   0 root         (0) root         (0)    78772 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)    36882 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
--rw-rw-rw-   0 root         (0) root         (0)    34976 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.416304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/
--rw-rw-rw-   0 root         (0) root         (0)     4162 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26932 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
--rw-rw-rw-   0 root         (0) root         (0)    13453 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
--rw-rw-rw-   0 root         (0) root         (0)    14139 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py
--rw-rw-rw-   0 root         (0) root         (0)     6514 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.419304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20941 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
--rw-rw-rw-   0 root         (0) root         (0)    38069 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
--rw-rw-rw-   0 root         (0) root         (0)     1678 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
--rw-rw-rw-   0 root         (0) root         (0)     9874 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     3294 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12690 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8598 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4340 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
--rw-rw-rw-   0 root         (0) root         (0)     2884 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py
--rw-rw-rw-   0 root         (0) root         (0)    25448 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14158 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py
--rw-rw-rw-   0 root         (0) root         (0)    13012 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.422304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17181 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py
--rw-rw-rw-   0 root         (0) root         (0)    12231 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2898 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
--rw-rw-rw-   0 root         (0) root         (0)    12881 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py
--rw-rw-rw-   0 root         (0) root         (0)    11395 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py
--rw-rw-rw-   0 root         (0) root         (0)     8530 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.422304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3648 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py
--rw-rw-rw-   0 root         (0) root         (0)     9341 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py
--rw-rw-rw-   0 root         (0) root         (0)    11407 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py
--rw-rw-rw-   0 root         (0) root         (0)    13544 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
--rw-rw-rw-   0 root         (0) root         (0)    27871 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.423304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/privacy_params.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/random_seed.py
--rw-rw-rw-   0 root         (0) root         (0)     3320 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/routing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.424304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8822 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py
--rw-rw-rw-   0 root         (0) root         (0)    10539 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/marginals.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/multiplicity.py
--rw-rw-rw-   0 root         (0) root         (0)     3376 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/predicate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.436304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/
--rw-rw-rw-   0 root         (0) root         (0)     2045 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/attribute.proto
--rw-r--r--   0 root         (0) root         (0)     1507 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1840 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/bounds.proto
--rw-r--r--   0 root         (0) root         (0)     1712 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2160 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/constraint.proto
--rw-r--r--   0 root         (0) root         (0)     1964 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3236 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset.proto
--rw-r--r--   0 root         (0) root         (0)     3941 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9653 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/links.proto
--rw-r--r--   0 root         (0) root         (0)     2557 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/links_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4178 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/manager.proto
--rw-r--r--   0 root         (0) root         (0)     1417 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/manager_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/marginals.proto
--rw-r--r--   0 root         (0) root         (0)     1739 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2169 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/multiplicity.proto
--rw-r--r--   0 root         (0) root         (0)     1777 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2178 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/path.proto
--rw-r--r--   0 root         (0) root         (0)     1449 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/path_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate.proto
--rw-r--r--   0 root         (0) root         (0)     2416 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4839 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/proto_container.proto
--rw-r--r--   0 root         (0) root         (0)     1634 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1821 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      629 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation.proto
--rw-r--r--   0 root         (0) root         (0)     1545 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2606 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar.proto
--rw-r--r--   0 root         (0) root         (0)     3904 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9843 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      695 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/schema.proto
--rw-r--r--   0 root         (0) root         (0)     2606 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/schema_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/size.proto
--rw-r--r--   0 root         (0) root         (0)     1689 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/size_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2154 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3909 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics.proto
--rw-r--r--   0 root         (0) root         (0)    11222 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    32747 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      646 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status.proto
--rw-r--r--   0 root         (0) root         (0)     3258 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6181 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6908 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform.proto
--rw-r--r--   0 root         (0) root         (0)    16655 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform_pb2.py
--rw-r--r--   0 root         (0) root         (0)    48587 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type.proto
--rw-r--r--   0 root         (0) root         (0)     9784 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type_pb2.py
--rw-r--r--   0 root         (0) root         (0)    30590 2024-03-08 09:25:35.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      949 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3948 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/utilities.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    13749 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/scalar.py
--rw-rw-rw-   0 root         (0) root         (0)     4671 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1467 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/size.py
--rw-rw-rw-   0 root         (0) root         (0)    43603 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)    17261 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.437304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14527 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/local.py
--rw-rw-rw-   0 root         (0) root         (0)     5614 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     3084 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    39687 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/transform.py
--rw-rw-rw-   0 root         (0) root         (0)   117405 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/type.py
--rw-rw-rw-   0 root         (0) root         (0)    42425 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/typing.py
--rw-rw-rw-   0 root         (0) root         (0)     4998 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/variant_constraint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-08 09:25:44.438304 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/
--rw-r--r--   0 root         (0) root         (0)      436 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9090 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      125 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-08 09:25:44.000000 sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6927 2024-03-08 09:25:44.439304 sarus_data_spec_public-3.9.2.dev0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1191 2024-03-08 09:25:25.000000 sarus_data_spec_public-3.9.2.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.169659 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/
+-rwxrwxrwx   0 root         (0) root         (0)      947 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.171492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8407 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/admin_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/array.py
+-rw-rw-rw-   0 root         (0) root         (0)     7264 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2101 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/pandas_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6266 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1014 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/bounds.py
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.173325 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1331 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/public.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    21741 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.175158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4997 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22994 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py
+-rw-rw-rw-   0 root         (0) root         (0)    11623 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.176992 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17255 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py
+-rw-rw-rw-   0 root         (0) root         (0)      815 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5717 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/recursive_validator.py
+-rw-rw-rw-   0 root         (0) root         (0)    28906 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/signature.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/simple_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5355 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     8867 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/deprecation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/json_serialisation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.178825 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7629 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/async_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    31915 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6724 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/cache_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.178825 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.180658 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.181575 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.181575 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7120 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.182492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.186158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23081 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10321 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)    21505 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/optbinning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.187075 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py
+-rw-rw-rw-   0 root         (0) root         (0)    32015 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)    78764 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)    37535 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)    34976 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.188908 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/
+-rw-rw-rw-   0 root         (0) root         (0)     4162 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26932 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/explainer.py
+-rw-rw-rw-   0 root         (0) root         (0)    13453 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/maskers.py
+-rw-rw-rw-   0 root         (0) root         (0)    14139 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)     6514 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.193492 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20941 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38069 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py
+-rw-rw-rw-   0 root         (0) root         (0)     1678 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py
+-rw-rw-rw-   0 root         (0) root         (0)     9874 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12690 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4340 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2884 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py
+-rw-rw-rw-   0 root         (0) root         (0)    25448 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/std.py
+-rw-rw-rw-   0 root         (0) root         (0)     3011 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14158 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py
+-rw-rw-rw-   0 root         (0) root         (0)    13072 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.197158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17192 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py
+-rw-rw-rw-   0 root         (0) root         (0)     1625 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/error_estimation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py
+-rw-rw-rw-   0 root         (0) root         (0)    12256 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2922 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    12893 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py
+-rw-rw-rw-   0 root         (0) root         (0)    11420 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     8567 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.197158 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2462 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py
+-rw-rw-rw-   0 root         (0) root         (0)     9522 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py
+-rw-rw-rw-   0 root         (0) root         (0)    11403 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py
+-rw-rw-rw-   0 root         (0) root         (0)    13558 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/to_small_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    27871 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.198991 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/privacy_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/random_seed.py
+-rw-rw-rw-   0 root         (0) root         (0)     3320 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/routing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.198991 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8893 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/bigdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5703 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/queries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10279 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/marginals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/multiplicity.py
+-rw-rw-rw-   0 root         (0) root         (0)     3376 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/predicate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.215491 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute.proto
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds.proto
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint.proto
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset.proto
+-rw-r--r--   0 root         (0) root         (0)     3941 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9653 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links.proto
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager.proto
+-rw-r--r--   0 root         (0) root         (0)     1417 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals.proto
+-rw-r--r--   0 root         (0) root         (0)     1739 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity.proto
+-rw-r--r--   0 root         (0) root         (0)     1777 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2178 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path.proto
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate.proto
+-rw-r--r--   0 root         (0) root         (0)     2416 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4839 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container.proto
+-rw-r--r--   0 root         (0) root         (0)     1634 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation.proto
+-rw-r--r--   0 root         (0) root         (0)     1545 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar.proto
+-rw-r--r--   0 root         (0) root         (0)     3904 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9843 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      694 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema.proto
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size.proto
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics.proto
+-rw-r--r--   0 root         (0) root         (0)    11222 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    32747 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status.proto
+-rw-r--r--   0 root         (0) root         (0)     3258 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6181 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6970 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform.proto
+-rw-r--r--   0 root         (0) root         (0)    16759 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    48797 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type.proto
+-rw-r--r--   0 root         (0) root         (0)     9784 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    30590 2024-04-11 11:02:52.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3948 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/utilities.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    13753 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/scalar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1467 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/size.py
+-rw-rw-rw-   0 root         (0) root         (0)    43603 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)    17261 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.216408 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14527 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/local.py
+-rw-rw-rw-   0 root         (0) root         (0)     5606 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3084 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    40022 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/transform.py
+-rw-rw-rw-   0 root         (0) root         (0)   123297 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/type.py
+-rw-rw-rw-   0 root         (0) root         (0)    40869 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/variant_constraint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:03:02.217324 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      661 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9090 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 11:03:02.000000 sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     6927 2024-04-11 11:03:02.218241 sarus_data_spec_public-4.0.0.dev5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1191 2024-04-11 11:02:30.000000 sarus_data_spec_public-4.0.0.dev5/setup.py
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/__init__.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 from sarus_data_spec.context import push_global_context
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.status import Status
 from sarus_data_spec.transform import Transform
 from sarus_data_spec.variant_constraint import VariantConstraint
 
+__all__ = [
+    "Attribute",
+    "Dataset",
+    "Scalar",
+    "Status",
+    "Transform",
+    "VariantConstraint",
+]
+
 """A library to manage Sarus datasets"""
 # pylint: disable=unused-variable
 
-PACKAGE_NAME: Final[str] = 'sarus_data_spec'
-VERSION: Final[str] = '3.9.2.dev0'
+PACKAGE_NAME: Final[str] = "sarus_data_spec"
+VERSION: Final[str] = "4.0.0.dev5"
 
 try:
     import sarus_data_spec.context.worker as sw
 
     push_global_context(sw.WorkerContext())
 except ModuleNotFoundError as exception:
-    if exception.name == 'sarus_data_spec.context.worker':
+    if exception.name == "sarus_data_spec.context.worker":
         pass  # The worker context is absent from the public release
     else:
         raise exception
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/admin_utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/admin_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pyarrow as pa
 
 from sarus_data_spec.arrow.pandas_utils import (
     convert_pandas_metadata_to_admin_columns,
     pandas_index_columns,
     remove_pandas_index_columns,
 )
-from sarus_data_spec.constants import DATA, PUBLIC, USER_COLUMN, WEIGHTS
+from sarus_data_spec.constants import DATA, PU_COLUMN, PUBLIC, WEIGHTS
 import sarus_data_spec.typing as st
 
 
 async def async_to_arrow_extract_admin(
     dataset: st.Dataset, batch_size: int = 10000
 ) -> t.Optional[t.AsyncIterator[pa.RecordBatch]]:
     """This function return an async iterator record batches of the
@@ -20,15 +20,15 @@
     """
     schema = await dataset.async_schema()
     if not schema.has_admin_columns():
         return None
 
     # Extract admin data from DATA
     batches_async_it = await dataset.async_to_arrow(batch_size)
-    pe_field_names = [PUBLIC, USER_COLUMN, WEIGHTS]
+    pe_field_names = [PUBLIC, PU_COLUMN, WEIGHTS]
 
     async def extract_admin_columns(
         batches_async_it: t.AsyncIterator[pa.RecordBatch],
     ) -> t.AsyncIterator[t.Tuple[pa.RecordBatch, t.Optional[pa.RecordBatch]]]:
         async for batch in batches_async_it:
             field_names = list(batch.schema.names)
             index_cols = pandas_index_columns(batch.schema)
@@ -149,56 +149,75 @@
 
 
 def compute_admin_data(
     input_admin_data: pa.Table, result: st.DatasetCastable
 ) -> pa.Table:
     """Compute the output protected entity of an external transform."""
     # We guarantee that the data.index is a reliable way to trace how
-    # the rows were rearranged
+    # the rows were rearranged using PyArrow's  internal implementation
+    # See: https://arrow.apache.org/docs/python/pandas.html#handling-pandas-indexes
+
     if type(result) == pd.DataFrame:
         df = t.cast(pd.DataFrame, result)
         input_pe_df = input_admin_data.to_pandas()
-        return pa.Table.from_pandas(input_pe_df.loc[df.index])
+        output_admin_data = pa.Table.from_pandas(input_pe_df.loc[df.index])
     elif type(result) == pd.Series:
         sr = t.cast(pd.Series, result)
         input_pe_df = input_admin_data.to_pandas()
-        return pa.Table.from_pandas(input_pe_df.loc[sr.index])
+        output_admin_data = pa.Table.from_pandas(input_pe_df.loc[sr.index])
     elif type(result) == pd.core.groupby.DataFrameGroupBy:
         df_grouped_by = t.cast(pd.core.groupby.DataFrameGroupBy, result)
         combined_df = df_grouped_by.obj
         input_pe_df = input_admin_data.to_pandas()
-        return pa.Table.from_pandas(input_pe_df.loc[combined_df.index])
+        output_admin_data = pa.Table.from_pandas(
+            input_pe_df.loc[combined_df.index]
+        )
     elif type(result) == pd.core.groupby.SeriesGroupBy:
         series_grouped_by = t.cast(pd.core.groupby.SeriesGroupBy, result)
         combined_series = series_grouped_by.obj
         input_pe_df = input_admin_data.to_pandas()
-        return pa.Table.from_pandas(input_pe_df.loc[combined_series.index])
+        output_admin_data = pa.Table.from_pandas(
+            input_pe_df.loc[combined_series.index]
+        )
     else:
         raise TypeError(
             f"Cannot compute the admin data for type {type(result)}"
         )
 
+    columns_to_cast = set(input_admin_data.column_names) & set(
+        output_admin_data.column_names
+    )
+    for col in columns_to_cast:
+        field = input_admin_data.field(col)
+
+        if field != output_admin_data.field(col):
+            i = output_admin_data.schema.get_field_index(col)
+            column = output_admin_data.column(col).cast(field.type)
+            output_admin_data = output_admin_data.set_column(i, field, column)
+
+    return output_admin_data
+
 
 def validate_admin_data(
     admin_data: t.List[pa.Table],
 ) -> pa.Table:
     """Check that all admin data are equal."""
     # If we reach this part then there should be only one input admin data
     if len(admin_data) == 0:
         raise ValueError("The list of input admin data is empty.")
 
     pe = next(iter(admin_data), None)
     if pe is None:
         raise ValueError(
-            "The dataset was infered PEP but has no input admin data"
+            "The dataset was infered PUP but has no input admin data"
         )
 
     if not all([candidate.equals(pe) for candidate in admin_data]):
         raise ValueError(
-            "The dataset is PEP but has several differing input admin "
+            "The dataset is PUP but has several differing input admin "
             "data values"
         )
     return pe
 
 
 def create_admin_columns(table: pa.Table) -> pa.Table:
     """Isolate special columns to admin columns."""
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/conversion.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 async def async_arrow_batches_to_dataframegroupby(
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the group by object from the data."""
     arrow_batches = [batch async for batch in batches_async_iterator]
     tab = pa.Table.from_batches(arrow_batches)
 
-    groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, 'utf-8')
+    groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, "utf-8")
     if groupby_keys_bytes in tab.schema.metadata:
         keys_encoded = tab.schema.metadata[groupby_keys_bytes]
         keys = SarusJSONDecoder.decode_bytes(keys_encoded)
     else:
         raise ValueError(
             "Trying to convert to series Arrow batches "
             "without groupby keys already defined."
@@ -118,15 +118,15 @@
     batches_async_iterator: t.AsyncIterator[pa.RecordBatch],
 ) -> pd.Series:
     """Returns the group by object from the data."""
     arrow_batches = [batch async for batch in batches_async_iterator]
     tab = pa.Table.from_batches(arrow_batches)
     df = tab.to_pandas(split_blocks=False, self_destruct=True)
 
-    groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, 'utf-8')
+    groupby_keys_bytes = bytes(GROUPBY_KEYS_NAME, "utf-8")
     if groupby_keys_bytes in tab.schema.metadata:
         keys_encoded = tab.schema.metadata[groupby_keys_bytes]
         keys = SarusJSONDecoder.decode_bytes(keys_encoded)
     else:
         raise ValueError(
             "Trying to convert to series Arrow batches "
             "without groupby keys already defined."
@@ -137,15 +137,15 @@
 
     groupby_object = series.groupby(keys)
     return groupby_object
 
 
 def to_pyarrow_table(data: t.Any) -> pa.Table:
     """Convert the result of an external transform to a Pyarrow Table."""
-    if not type(data) in t.get_args(st.DatasetCastable):
+    if type(data) not in t.get_args(st.DatasetCastable):
         raise TypeError(f"Cannot convert {type(data)} to Arrow batches.")
 
     if isinstance(data, pd.DataFrame):
         df = t.cast(pd.DataFrame, data)
         return pa.Table.from_pandas(df)
     elif isinstance(data, pd.Series):
         sr = t.cast(pd.Series, data)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/pandas_utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/schema.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 pa.field(
                     name=field_name,
                     type=arrow_type.to_arrow(field_type),
                 )
                 for field_name, field_type in fields.items()
             ]
             arrow_fields.append(
-                pa.field(name='field_selected', type=pa.large_string())
+                pa.field(name="field_selected", type=pa.large_string())
             )
             self.schema = pa.schema(fields=arrow_fields)
 
         def Boolean(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             pass
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/arrow/type.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/arrow/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 FLOATBASE_TO_ARROW = {
     st.FloatBase.FLOAT64: pa.float64(),
     st.FloatBase.FLOAT32: pa.float32(),
     st.FloatBase.FLOAT16: pa.float16(),
 }
 
 DATETIMEBASE_TO_ARROW = {
-    st.DatetimeBase.INT64_NS: pa.timestamp('ns'),
-    st.DatetimeBase.INT64_MS: pa.timestamp('ms'),
+    st.DatetimeBase.INT64_NS: pa.timestamp("ns"),
+    st.DatetimeBase.INT64_MS: pa.timestamp("ms"),
     st.DatetimeBase.STRING: pa.large_string(),
 }
 
 DATEBASE_TO_ARROW = {
     st.DateBase.INT32: pa.date32(),
     st.DateBase.STRING: pa.large_string(),
 }
 
 TIMEBASE_TO_ARROW = {
-    st.TimeBase.INT64_US: pa.time64('us'),
-    st.TimeBase.INT32_MS: pa.time32('ms'),
+    st.TimeBase.INT64_US: pa.time64("us"),
+    st.TimeBase.INT32_MS: pa.time32("ms"),
     st.TimeBase.STRING: pa.large_string(),
 }
 
 
 def to_arrow(
     _type: st.Type,
     nullable: bool = True,
@@ -134,16 +134,16 @@
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             self.pa_type = pa.struct(
                 [
                     pa.field(
                         name=name,
                         type=to_arrow(field),
-                        nullable=field.protobuf().HasField('optional')
-                        or field.protobuf().HasField('unit'),
+                        nullable=field.protobuf().HasField("optional")
+                        or field.protobuf().HasField("unit"),
                     )
                     for name, field in fields.items()
                 ]
             )
 
         def Union(
             self,
@@ -158,15 +158,15 @@
                         type=to_arrow(field),
                         nullable=True,
                     )
                     for name, field in fields.items()
                 ]
                 + [
                     pa.field(
-                        name='field_selected',
+                        name="field_selected",
                         type=pa.large_string(),
                         nullable=False,
                     )
                 ]
             )
 
         def Optional(
@@ -301,28 +301,28 @@
         # timestamp or duration.
         if pa.types.is_timestamp(type):
             return sdt.Datetime(base=st.DatetimeBase.INT64_NS)
             # TODO: when we will support different bases for datetime
             # we need to remove the asserts in the Datetime builder and
             # the error rise in the check_visitor in user_settings
         if pa.types.is_time(type):
-            if type.unit in ['ns', 'us']:
+            if type.unit in ["ns", "us"]:
                 return sdt.Time(base=st.TimeBase.INT64_US)
             else:
                 return sdt.Time(base=st.TimeBase.INT32_MS)
 
         if pa.types.is_date(type):
             return sdt.Date()
         else:
             # It is a duration
-            if type.unit in ['s', 'ms', 'us']:
+            if type.unit in ["s", "ms", "us"]:
                 return sdt.Duration(unit=type.unit)
             else:
                 raise ValueError(
-                    'Duration type with nanosecond resolution not supported'
+                    "Duration type with nanosecond resolution not supported"
                 )
     if pa.types.is_null(type):
         return sdt.Unit()
     if pa.types.is_struct(type):
         struct_type = t.cast(pa.StructType, type)
         return sdt.Struct(
             {
@@ -333,15 +333,15 @@
             }
         )
     if pa.types.is_list(type):
         list_type = t.cast(pa.ListType, type)
         return sdt.List(
             type=type_from_arrow(list_type.value_type, nullable=False)
         )
-    raise NotImplementedError(f'Type {type} not implemented')
+    raise NotImplementedError(f"Type {type} not implemented")
 
 
 def type_from_arrow(
     arrow_type: pa.DataType,
     nullable: bool,
 ) -> st.Type:
     if nullable and not (pa.types.is_null(arrow_type)):
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/attribute.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/attribute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, Type
+from typing import Dict, Optional, Type
 
 from sarus_data_spec.base import Referring
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
 class Attribute(Referring[sp.Attribute]):
@@ -20,12 +20,16 @@
         return sp.Attribute
 
     def name(self) -> str:
         return self.protobuf().name
 
 
 def attach_properties(
-    dataspec: st.DataSpec, name: str = "", properties: Dict[str, str] = {}
+    dataspec: st.DataSpec,
+    name: str = "",
+    properties: Optional[Dict[str, str]] = None,
 ) -> Attribute:
+    if properties is None:
+        properties = {}
     return Attribute(
         sp.Attribute(object=dataspec.uuid(), properties=properties, name=name)
     )
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""A few base implementations of basic Protocols
-"""
+"""A few base implementations of basic Protocols"""
+
 from uuid import UUID
 import hashlib
 import logging
 import typing as t
 
 from sarus_data_spec.context.typing import Context, HasContext
 from sarus_data_spec.manager.typing import HasManager, Manager
@@ -11,15 +11,15 @@
 from sarus_data_spec.protobuf.utilities import copy, json, serialize, type_name
 from sarus_data_spec.storage.typing import HasStorage, Storage
 import sarus_data_spec.context as sc
 import sarus_data_spec.typing as st
 
 logger = logging.getLogger(__name__)
 
-P = t.TypeVar('P', bound=Protobuf, covariant=True)
+P = t.TypeVar("P", bound=Protobuf, covariant=True)
 
 
 class Base(st.HasProtobuf[P], st.Value, st.Frozen, HasContext):
     """An object with value semantics, properties, backed by a Protobuf, with
     a default implementation"""
 
     def __init__(self, protobuf: P) -> None:
@@ -72,15 +72,15 @@
     def _frozen(self) -> bool:
         return self._checksum() == self._frozen_checksum
 
     def context(self) -> Context:
         return self._context
 
 
-PU = t.TypeVar('PU', bound=ProtobufWithUUID, covariant=True)
+PU = t.TypeVar("PU", bound=ProtobufWithUUID, covariant=True)
 
 
 class Referrable(Base[PU], st.Referrable[PU], HasStorage, HasManager):
     def __init__(self, protobuf: PU, store: bool = True) -> None:
         super().__init__(protobuf)
         # Pay attention to the fact self._freeze() in super
         # will call the implementation bellow,
@@ -88,22 +88,22 @@
         if store:
             self.storage().store(self)
 
     def _freeze(self) -> None:
         """Referrable objects keep a uuid consistent with the checksum.
         The checksum is computed with empty uuid
         """
-        self._protobuf.uuid = ''
+        self._protobuf.uuid = ""
         self._frozen_checksum = self._checksum()
         self._protobuf.uuid = UUID(bytes=self._frozen_checksum).hex
 
     def _frozen(self) -> bool:
         """The checksum is computed with empty uuid."""
         uuid = self._protobuf.uuid
-        self._protobuf.uuid = ''
+        self._protobuf.uuid = ""
         result = (self._checksum() == self._frozen_checksum) and (
             uuid == UUID(bytes=self._frozen_checksum).hex
         )
         self._protobuf.uuid = uuid
         return result
 
     def uuid(self) -> str:
@@ -129,16 +129,16 @@
 
     def referred(self) -> t.Collection[st.Referrable]:
         result = set()
         for value in self._referred:
             referred = self.storage().referrable(value)
             if referred is None:
                 logger.info(
-                    f'{value} is not present '
-                    f'in the referrables table of the storage'
+                    f"{value} is not present "
+                    f"in the referrables table of the storage"
                 )
                 # raise ValueError(
                 #     f'{value} is not present '
                 #     f'in the referrables table of the storage'
                 # )
             else:
                 result.add(referred)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/bounds.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/bounds.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Builder
 def bounds(
     dataset: st.Dataset,
     statistics: t.Optional[st.Statistics] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Bounds:
-    name = f'{dataset.name()}_bounds'
+    name = f"{dataset.name()}_bounds"
 
     return Bounds(
         sp.Bounds(
             dataset=dataset.uuid(),
             name=name,
             statistics=statistics.protobuf()
             if statistics is not None
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/constants.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,141 +1,141 @@
 from enum import Enum
 
 from sarus_data_spec import typing as st
 
-DATA = 'sarus_data'
-USER_COLUMN = 'sarus_protected_entity'
-PEID_COLUMN = USER_COLUMN
-WEIGHTS = 'sarus_weights'
-PUBLIC = 'sarus_is_public'
+DATA = "sarus_data"
+PU_COLUMN = "sarus_privacy_unit"
+PID_COLUMN = PU_COLUMN
+WEIGHTS = "sarus_weights"
+PUBLIC = "sarus_is_public"
 
 # constants used in protection stored in each struct
-NON_EMPTY_PROTECTED_PATHS = 'non_zero_protected_values'
-STRUCT_KIND = 'merge_paths'
-TO_MERGE = 'fks_for_merging'
+NON_EMPTY_PRIVACY_UNIT_TRACKING_PATHS = "non_zero_protected_values"
+STRUCT_KIND = "merge_paths"
+TO_MERGE = "fks_for_merging"
 
 # protection constants for paths in types
-LIST_VALUES = 'sarus_list_values'
-ARRAY_VALUES = 'sarus_array_values'
-OPTIONAL_VALUE = 'sarus_optional_value'
-CONSTRAINED_VALUE = 'sarus_constrained_value'
+LIST_VALUES = "sarus_list_values"
+ARRAY_VALUES = "sarus_array_values"
+OPTIONAL_VALUE = "sarus_optional_value"
+CONSTRAINED_VALUE = "sarus_constrained_value"
 
 
 class StructKind(Enum):
-    HAS_PE = '0'
-    NO_PE = '1'
-    TO_MERGE = '2'
+    HAS_PU = "0"
+    NO_PU = "1"
+    TO_MERGE = "2"
 
 
 # constants for type properties
-TEXT_MIN_LENGTH = 'min_length'
-TEXT_MAX_LENGTH = 'max_length'
-TEXT_CHARSET = 'text_char_set'
-TEXT_EXACT_CHARSET = 'FullUserInput'
-TEXT_ALPHABET_NAME = 'text_alphabet_name'
-SQL_MAPPING = 'sql_mapping'
-FLOAT_DISTRIBUTION = 'distribution_model'
-FLOAT_DIST_PARAMS = 'parameters'
-MAX_MAX_MULT = 'max_max_multiplicity'
-MULTIPLICITY = 'multiplicity'
-RECOMPUTE_TYPE_RANGES = 'recompute_type_ranges'
+TEXT_MIN_LENGTH = "min_length"
+TEXT_MAX_LENGTH = "max_length"
+TEXT_CHARSET = "text_char_set"
+TEXT_EXACT_CHARSET = "FullUserInput"
+TEXT_ALPHABET_NAME = "text_alphabet_name"
+SQL_MAPPING = "sql_mapping"
+FLOAT_DISTRIBUTION = "distribution_model"
+FLOAT_DIST_PARAMS = "parameters"
+MAX_MAX_MULT = "max_max_multiplicity"
+MULTIPLICITY = "multiplicity"
+RECOMPUTE_TYPE_RANGES = "recompute_type_ranges"
 
 # constants for dataset properties
-DATASET_SLUGNAME = 'slugname'
+DATASET_SLUGNAME = "slugname"
 
 # constants for schema properties
-PRIMARY_KEYS = 'primary_keys'
-FOREIGN_KEYS = 'foreign_keys'
+PRIMARY_KEYS = "primary_keys"
+FOREIGN_KEYS = "foreign_keys"
 
 # names when transforming datetime type in struct
-DATETIME_YEAR = 'year'
-DATETIME_MONTH = 'month'
-DATETIME_DAY = 'day'
-DATETIME_HOUR = 'hour'
-DATETIME_MINUTES = 'minutes'
-DATETIME_SECONDS = 'seconds'
+DATETIME_YEAR = "year"
+DATETIME_MONTH = "month"
+DATETIME_DAY = "day"
+DATETIME_HOUR = "hour"
+DATETIME_MINUTES = "minutes"
+DATETIME_SECONDS = "seconds"
 
 
 # sql, to_sql status
 TO_SQL_TASK = "sql_preparation"
-SQL_TASK = 'sql'
+SQL_TASK = "sql"
 
 # Big Data Status
-BIG_DATA_TASK = 'big_data_dataset'
-BIG_DATA_THRESHOLD = 'threshold'
-IS_BIG_DATA = 'is_big_data'
-DATASET_N_LINES = 'dataset_n_lines'
-DATASET_N_BYTES = 'dataset_n_bytes'
+BIG_DATA_TASK = "big_data_dataset"
+BIG_DATA_THRESHOLD = "threshold"
+IS_BIG_DATA = "is_big_data"
+DATASET_N_LINES = "dataset_n_lines"
+DATASET_N_BYTES = "dataset_n_bytes"
 THRESHOLD_TYPE = "threshold_type"
 
 # Caching Status
-TO_PARQUET_TASK = 'to_parquet'
+TO_PARQUET_TASK = "to_parquet"
 CACHE = TO_PARQUET_TASK
-CACHE_PATH = 'path'
-COMPUTATION_QUEUED = 'computation_queued'
-TO_SQL_CACHING_TASK = 'to_sql_caching'
-SQL_CACHING_URI = 'sql_caching_uri'
-TABLE_MAPPING = 'table_mapping'
-EXTENDED_TABLE_MAPPING = 'extended_table_mapping'
+CACHE_PATH = "path"
+COMPUTATION_QUEUED = "computation_queued"
+TO_SQL_CACHING_TASK = "to_sql_caching"
+SQL_CACHING_URI = "sql_caching_uri"
+TABLE_MAPPING = "table_mapping"
+EXTENDED_TABLE_MAPPING = "extended_table_mapping"
 
 # Caching infos for scalar
-CACHE_TYPE = 'cache_type'
-CACHE_PROTO = 'cache_proto'
-SCALAR_TASK = 'scalar_value'
+CACHE_TYPE = "cache_type"
+CACHE_PROTO = "cache_proto"
+SCALAR_TASK = "scalar_value"
 
 
 class ScalarCaching(Enum):
-    PICKLE = 'pickle'
-    PROTO = 'protobuf'
-    TRAIN_STATE = 'train_state'
+    PICKLE = "pickle"
+    PROTO = "protobuf"
+    TRAIN_STATE = "train_state"
 
 
 # Attributes Status
-SCHEMA_TASK = 'schema'
-SIZE_TASK = 'size'
-MULTIPLICITY_TASK = 'multiplicity'
-BOUNDS_TASK = 'bounds'
-MARGINALS_TASK = 'marginals'
-ARROW_TASK = 'arrow'
-PROTECTION_TASK = 'protection_task'
-USER_SETTINGS_TASK = 'user_settings_task'
-PUBLIC_TASK = 'public_task'
-CACHE_SCALAR_TASK = 'cache_scalar'
-QB_TASK = 'query_builder'
-LINKS_TASK = 'links_statistics'
-SYNTHETIC_TASK = 'synthetic'
+SCHEMA_TASK = "schema"
+SIZE_TASK = "size"
+MULTIPLICITY_TASK = "multiplicity"
+BOUNDS_TASK = "bounds"
+MARGINALS_TASK = "marginals"
+ARROW_TASK = "arrow"
+PRIVACY_UNIT_TRACKING_TASK = "privacy_unit_tracking_task"
+USER_SETTINGS_TASK = "user_settings_task"
+PUBLIC_TASK = "public_task"
+CACHE_SCALAR_TASK = "cache_scalar"
+QB_TASK = "query_builder"
+LINKS_TASK = "links_statistics"
+SYNTHETIC_TASK = "synthetic"
 PROCESSING_INFO = "processing_info"
 
 
 # Privacy
-PEP_TOKEN = "pep_token"
+PUP_TOKEN = "pup_token"
 NO_TOKEN = "no_token"
 IS_PUBLIC = "is_public"
 IS_SYNTHETIC = "is_synthetic"
 PRIVACY_LIMIT = "privacy_limit"
 CONSTRAINT_KIND = "constraint_kind"
 BEST_ALTERNATIVE = "best_alternative"
 SALT = "salt"
 
 # QUERYBUILDER
-QUERIES = 'queries'
+QUERIES = "queries"
 
 # Attributes names
 PRIVATE_QUERY = "private_query"
 IS_REMOTE = "is_remote"
 VARIANT_UUID = "variant_uuid"
 RELATIONSHIP_SPEC = "relationship_spec"
-VALIDATED_TYPE = 'validated_type'
-IS_VALID = 'is_valid'
+VALIDATED_TYPE = "validated_type"
+IS_VALID = "is_valid"
 
 # SYNTHETIC DATA
 MODEL_PROPERTIES = "model_properties"
-SYNTHETIC_MODEL = 'sarus_synthetic_model'
-TRAIN_CORRELATIONS = 'train_correlations'
-USE_JAX_TEXT = 'use_jax_text'
+SYNTHETIC_MODEL = "sarus_synthetic_model"
+TRAIN_CORRELATIONS = "train_correlations"
+USE_JAX_TEXT = "use_jax_text"
 
 
 class SyntheticDataSettings:
     """Namespace for SD generation settings"""
 
     BATCH_SIZE = 64
     EPOCHS = 10
@@ -152,16 +152,16 @@
     "bigquery": st.SQLDialect.BIG_QUERY,
     "redshift": st.SQLDialect.REDSHIFT,
     "hive": st.SQLDialect.HIVE,
     "databricks": st.SQLDialect.DATABRICKS,
 }
 
 # Possible values
-POSSIBLE_VALUES_LENGTH = 'possible_values_length'
-POSSIBLE_VALUES = 'possible_values'
+POSSIBLE_VALUES_LENGTH = "possible_values_length"
+POSSIBLE_VALUES = "possible_values"
 
 # Model checkpoints
 TRAIN_STATE = "state"
 MODEL_NAME = "model_name"
 PROMPT = "prompt"
 
 # relationship spec
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/public.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/public.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/context/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/context/typing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataset.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     import tensorflow as tf
 except ModuleNotFoundError:
     pass  # Warning is displayed by typing.py
 
 try:
     from sqlalchemy.engine import make_url
 except ModuleNotFoundError:
-    warnings.warn('SqlAlchemy not found, sql operations not available')
+    warnings.warn("SqlAlchemy not found, sql operations not available")
 
 
 from sarus_data_spec.base import Referring
 from sarus_data_spec.constants import DATASET_SLUGNAME, PROMPT
 from sarus_data_spec.protobuf.utilities import to_base64
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.transform import Transform, external
@@ -74,68 +74,68 @@
         return self._protobuf.name
 
     def doc(self) -> str:
         return self._protobuf.doc
 
     def is_transformed(self) -> bool:
         """Is the dataset composed."""
-        return self._protobuf.spec.HasField('transformed')
+        return self._protobuf.spec.HasField("transformed")
 
     def is_file(self) -> bool:
         """Is the dataset composed."""
-        return self._protobuf.spec.HasField('file')
+        return self._protobuf.spec.HasField("file")
 
     def is_synthetic(self) -> bool:
         """Is the dataset synthetic."""
         return self.manager().dataspec_validator().is_synthetic(self)
 
     def has_admin_columns(self) -> bool:
         return self.schema().has_admin_columns()
 
     def is_protected(self) -> bool:
-        return self.schema().is_protected()
+        return self.schema().is_privacy_unit_tracking()
 
-    def is_pep(self) -> bool:
-        """Is the dataset PEP."""
-        return self.pep_token() is not None
-
-    def pep_token(self) -> Optional[str]:
-        """Returns the dataset PEP token."""
-        return self.manager().dataspec_validator().pep_token(self)
+    def is_pup(self) -> bool:
+        """Is the dataset PUP."""
+        return self.pup_token() is not None
+
+    def pup_token(self) -> Optional[str]:
+        """Returns the dataset PUP token."""
+        return self.manager().dataspec_validator().pup_token(self)
 
-    def rewritten_pep_token(self) -> Optional[str]:
-        """Returns the PEP token for the DP variant of this dataspec
+    def rewritten_pup_token(self) -> Optional[str]:
+        """Returns the PUP token for the DP variant of this dataspec
         during DP rewriting.
 
-        Currently, the implementation assumes a single DP/PEP variant per
+        Currently, the implementation assumes a single DP/PUP variant per
         dataspec, resulting in one possible value for
-        "rewritten_pep_token."
+        "rewritten_pup_token."
         Future changes could introduce multiple variants, necessitating
         the implementation of priority rules.
         """
-        return self.manager().dataspec_validator().rewritten_pep_token(self)
+        return self.manager().dataspec_validator().rewritten_pup_token(self)
 
     def is_dp(self) -> bool:
         """Is the dataspec the result of a DP transform"""
         return self.manager().dataspec_validator().is_dp(self)
 
     def is_public(self) -> bool:
         """Is the dataset public."""
         return self.manager().dataspec_validator().is_public(self)
 
     def is_dp_writable(self) -> bool:
         """Check if there exists a variant of this dataspec
         that utilizes the dp equivalent, and this variant is is_dp."""
         return self.manager().dataspec_validator().is_dp_writable(self)
 
-    def is_pep_writable(self) -> bool:
-        """Check if there exists a variant of this dataspec that is is_pep.
-        The dataspec is is_pep_writable if it has a non-None
-        rewritten_pep_token."""
-        return self.manager().dataspec_validator().is_pep_writable(self)
+    def is_pup_writable(self) -> bool:
+        """Check if there exists a variant of this dataspec that is is_pup.
+        The dataspec is is_pup_writable if it has a non-None
+        rewritten_pup_token."""
+        return self.manager().dataspec_validator().is_pup_writable(self)
 
     def is_publishable(self) -> bool:
         """Check if there exists a variant of this dataspec that is
         published."""
         return self.manager().dataspec_validator().is_publishable(self)
 
     def is_published(self) -> bool:
@@ -197,27 +197,27 @@
     def schema(self) -> st.Schema:
         return self.manager().schema(self)
 
     async def async_schema(self) -> st.Schema:
         return await self.manager().async_schema(self)
 
     def size(self) -> t.Optional[Size]:
-        return cast('Size', self.manager().size(self))
+        return cast("Size", self.manager().size(self))
 
     def multiplicity(self) -> t.Optional[Multiplicity]:
-        return cast('Multiplicity', self.manager().multiplicity(self))
+        return cast("Multiplicity", self.manager().multiplicity(self))
 
     def bounds(self) -> t.Optional[Bounds]:
-        return cast('Bounds', self.manager().bounds(self))
+        return cast("Bounds", self.manager().bounds(self))
 
     def marginals(self) -> t.Optional[Marginals]:
-        return cast('Marginals', self.manager().marginals(self))
+        return cast("Marginals", self.manager().marginals(self))
 
     def links(self) -> st.Links:
-        return cast('Links', self.manager().links(self))
+        return cast("Links", self.manager().links(self))
 
     def transform(self) -> st.Transform:
         return cast(
             st.Transform,
             self.storage().referrable(
                 self.protobuf().spec.transformed.transform
             ),
@@ -301,15 +301,15 @@
         with a random uuid so that even if they are submitted multiple times to
         an account, they are only accounted once (ask @cgastaud for more on
         accounting).
         """
         return self.manager().dataspec_validator().private_queries(self)
 
     def spec(self) -> str:
-        return cast(str, self._protobuf.spec.WhichOneof('spec'))
+        return cast(str, self._protobuf.spec.WhichOneof("spec"))
 
     def __iter__(self) -> Iterator[pa.RecordBatch]:
         return self.to_arrow(batch_size=1)
 
     def to_pandas(self) -> pd.DataFrame:
         return self.manager().to_pandas(self)
 
@@ -381,22 +381,22 @@
                             "Dataset",
                         )
                     else:
                         self.nodes[visited.uuid()] = (visited.name(), "Scalar")
 
                     if not visited.is_remote():
                         for argument in arguments:
-                            self.edges[
-                                (argument.uuid(), visited.uuid())
-                            ] = transform.name()
+                            self.edges[(argument.uuid(), visited.uuid())] = (
+                                transform.name()
+                            )
                             argument.accept(self)
                         for _, argument in named_arguments.items():
-                            self.edges[
-                                (argument.uuid(), visited.uuid())
-                            ] = transform.name()
+                            self.edges[(argument.uuid(), visited.uuid())] = (
+                                transform.name()
+                            )
                             argument.accept(self)
                     self.visited.add(visited)
 
             def other(self, visited: st.DataSpec) -> None:
                 if visited.prototype() == sp.Dataset:
                     self.nodes[visited.uuid()] = (
                         visited.name(),
@@ -406,23 +406,23 @@
                     self.nodes[visited.uuid()] = (visited.name(), "Scalar")
 
             def all(self, visited: st.DataSpec) -> None:
                 pass
 
         visitor = Dot()
         self.accept(visitor)
-        result = 'digraph {'
+        result = "digraph {"
         for uuid, (label, node_type) in visitor.nodes.items():
             shape = "polygon" if node_type == "Scalar" else "ellipse"
             result += (
                 f'\n"{uuid}" [label="{label} ({uuid[:2]})", shape={shape}];'
             )
         for (u1, u2), label in visitor.edges.items():
             result += f'\n"{u1}" -> "{u2}" [label="{label} ({uuid[:2]})"];'
-        result += '}'
+        result += "}"
         return result
 
     def primary_keys(self) -> List[st.Path]:
         return self.manager().primary_keys(self)
 
     def attribute(self, name: str) -> t.Optional[st.Attribute]:
         return self.manager().attribute(name=name, dataspec=self)
@@ -502,47 +502,47 @@
     attach_info_callback(output_dataspec)
     return output_dataspec
 
 
 def file(
     format: str,
     uri: str,
-    doc: str = 'A file dataset',
+    doc: str = "A file dataset",
     properties: Optional[Mapping[str, str]] = None,
 ) -> Dataset:
     return Dataset(
         sp.Dataset(
             name=basename(urlparse(uri).path),
             doc=doc,
             spec=sp.Dataset.Spec(file=sp.Dataset.File(format=format, uri=uri)),
             properties=properties,
         )
     )
 
 
 def csv_file(
     uri: str,
-    doc: str = 'A csv file dataset',
+    doc: str = "A csv file dataset",
     properties: Optional[Mapping[str, str]] = None,
 ) -> Dataset:
     return Dataset(
         sp.Dataset(
             name=basename(urlparse(uri).path),
             doc=doc,
-            spec=sp.Dataset.Spec(file=sp.Dataset.File(format='csv', uri=uri)),
+            spec=sp.Dataset.Spec(file=sp.Dataset.File(format="csv", uri=uri)),
             properties=properties,
         )
     )
 
 
 def files(
     name: str,
     format: str,
     uri_pattern: str,
-    doc: str = 'Dataset split into files',
+    doc: str = "Dataset split into files",
     properties: Optional[Mapping[str, str]] = None,
 ) -> Dataset:
     return Dataset(
         sp.Dataset(
             name=name,
             doc=doc,
             spec=sp.Dataset.Spec(
@@ -552,23 +552,23 @@
         )
     )
 
 
 def csv_files(
     name: str,
     uri_pattern: str,
-    doc: str = 'A csv file dataset',
+    doc: str = "A csv file dataset",
     properties: Optional[Mapping[str, str]] = None,
 ) -> Dataset:
     return Dataset(
         sp.Dataset(
             name=name,
             doc=doc,
             spec=sp.Dataset.Spec(
-                files=sp.Dataset.Files(format='csv', uri_pattern=uri_pattern)
+                files=sp.Dataset.Files(format="csv", uri_pattern=uri_pattern)
             ),
             properties=properties,
         )
     )
 
 
 def sql(
@@ -576,23 +576,23 @@
     tables: Optional[
         Collection[Tuple[str, str]]
     ] = None,  # pairs schema/table_name
     properties: Optional[Mapping[str, str]] = None,
 ) -> Dataset:
     parsed_uri = make_url(uri)
     if parsed_uri.database is None:
-        name = f'{parsed_uri.drivername}_db_dataset'
+        name = f"{parsed_uri.drivername}_db_dataset"
     else:
         name = parsed_uri.database
     if tables is None:
         tables = []
     return Dataset(
         sp.Dataset(
             name=name,
-            doc=f'Data from {uri}',
+            doc=f"Data from {uri}",
             spec=sp.Dataset.Spec(
                 sql=sp.Dataset.Sql(
                     uri=uri,
                     tables=[
                         sp.Dataset.Sql.Table(
                             schema=element[0], table=element[1]
                         )
@@ -608,31 +608,31 @@
 def mapped_sql(
     uri: str,
     mapping_sql: Mapping[st.Path, st.Path],
     schemas: Optional[Collection[str]] = None,
 ) -> Dataset:
     parsed_uri = make_url(uri)
     if parsed_uri.database is None:
-        name = f'{parsed_uri.drivername}_db_dataset'
+        name = f"{parsed_uri.drivername}_db_dataset"
     else:
         name = parsed_uri.database
 
     serialized_mapping = json.dumps(
         {
             to_base64(original_table.protobuf()): to_base64(
                 synthetic_table.protobuf()
             )
             for original_table, synthetic_table in mapping_sql.items()
         }
     )
-    properties = {'sql_mapping': serialized_mapping}
+    properties = {"sql_mapping": serialized_mapping}
     return Dataset(
         sp.Dataset(
             name=name,
-            doc=f'Data from {uri}',
+            doc=f"Data from {uri}",
             spec=sp.Dataset.Spec(
                 sql=sp.Dataset.Sql(
                     uri=uri,
                 )
             ),
             properties=properties,
         )
@@ -658,15 +658,15 @@
                 huggingface=sp.Dataset.Huggingface(name=name, split=split)
             ),
         )
     )
 
 
 if t.TYPE_CHECKING:
-    test_sql: st.Dataset = sql(uri='sqlite:///:memory:')
-    test_file: st.Dataset = file(format='', uri='')
-    test_csv_file: st.Dataset = csv_file(uri='')
-    test_files: st.Dataset = files(name='', uri_pattern='', format='')
-    test_csv_files: st.Dataset = csv_files(name='', uri_pattern='')
+    test_sql: st.Dataset = sql(uri="sqlite:///:memory:")
+    test_file: st.Dataset = file(format="", uri="")
+    test_csv_file: st.Dataset = csv_file(uri="")
+    test_files: st.Dataset = files(name="", uri_pattern="", format="")
+    test_csv_files: st.Dataset = csv_files(name="", uri_pattern="")
     test_transformed: st.DataSpec = transformed(
-        sdtr.protect(), sql(uri='sqlite:///:memory:')
+        sdtr.privacy_unit_tracking(), sql(uri="sqlite:///:memory:")
     )
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/base.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/graph_query_builder_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.manager.async_utils import sync
 from sarus_data_spec.manager.ops.processor import routing
 import sarus_data_spec.typing as st
 
 try:
-    from sarus_query_builder.builders.composed_builder import ComposedBuilder
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
+    from sarus_data_spec.sarus_query_builder.builders.composed_builder import (
+        ComposedBuilder,
+    )
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
 
     # Placeholder classes
     class ComposedBuilder:  # type: ignore
         pass
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/recursive_rewriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from sarus_data_spec.scalar import privacy_budget
 from sarus_data_spec.storage.typing import Storage
 from sarus_data_spec.variant_constraint import dp_constraint
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 try:
-    from sarus_query_builder.builders.composed_builder import ComposedBuilder
+    from sarus_data_spec.sarus_query_builder.builders.composed_builder import (
+        ComposedBuilder,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
     ComposedBuilder = Any  # type: ignore
     OptimizableQueryBuilder = Any
 
 logger = logging.getLogger(__name__)
@@ -42,17 +44,15 @@
 
 class RecursiveDataspecRewriter(BaseDataspecRewriter):
     def __init__(self, storage: Storage):
         self._storage = storage
         self._dataspec_validator = RecursiveDataspecValidator(storage=storage)
         self._rewriter_dict: Dict[
             Tuple[str, str], str
-        ] = (
-            {}
-        )  # help to rewrite, avoid rewriting multipletime the same dataspec
+        ] = {}  # help to rewrite, avoid rewriting multipletime the same dataspec
 
     def rewriter_dict(self) -> Dict[Tuple[str, str], str]:
         return self._rewriter_dict
 
     def rewrite_uuid(
         self,
         dataspec_uuid: str,
@@ -82,32 +82,32 @@
                 raise ValueError(
                     "A DP applicable dataspec should have a dp transform"
                 )
         else:
             transform_to_use = dataspec.transform()
         return transform_to_use
 
-    def get_transform_for_pep_rewriting(
+    def get_transform_for_pup_rewriting(
         self, dataspec: st.DataSpec
     ) -> st.Transform:
         """Returns the appropriate transform for rewriting
-        a dataspec in the context of PEP rewriting."""
+        a dataspec in the context of PUP rewriting."""
         if not dataspec.is_transformed():
             raise ValueError(
                 """A not transformed dataspec does not
                 have transform for rewriting"""
             )
 
-        if dataspec.is_pep_writable():
+        if dataspec.is_pup_writable():
             dataset = cast(st.Dataset, dataspec)
             _, StaticChecker = routing.get_op(dataspec)
-            transform_to_use = StaticChecker(dataset).pep_transform()
+            transform_to_use = StaticChecker(dataset).pup_transform()
             if transform_to_use is None:
                 raise ValueError(
-                    "A PEP applicable dataspec should have a pep transform"
+                    "A PUP applicable dataspec should have a pup transform"
                 )
         else:
             transform_to_use = dataspec.transform()
         return transform_to_use
 
     def variant(
         self,
@@ -150,15 +150,15 @@
                 public_context,
                 salt,
             )
             return mock_variant
 
         if privacy_limit is None:
             raise ValueError(
-                "Privacy limit must be defined for PEP or DP rewriting"
+                "Privacy limit must be defined for PUP or DP rewriting"
             )
 
         rewrite_uuid = self.rewrite_uuid(
             dataspec.uuid(), salt=salt, privacy_limit=privacy_limit
         )
 
         if target_kind == st.ConstraintKind.DP:
@@ -181,23 +181,23 @@
                 dataspec,
                 public_context=public_context,
                 graph_query_builder=graph_query_builder,
                 rewrite_uuid=rewrite_uuid,
             )
             return variant
 
-        elif target_kind == st.ConstraintKind.PEP:
-            if not dataspec.is_pep_writable():
+        elif target_kind == st.ConstraintKind.PUP:
+            if not dataspec.is_pup_writable():
                 return rewrite_synthetic(
                     self.dataspec_validator(), dataspec, public_context
                 )[0]
             graph_query_builder = build_and_fit_graph_builder(
                 dataspec, privacy_limit
             )
-            variant, _ = self.rewrite_pep(
+            variant, _ = self.rewrite_pup(
                 dataspec,
                 public_context=public_context,
                 graph_query_builder=graph_query_builder,
                 rewrite_uuid=rewrite_uuid,
             )
             return variant
         else:
@@ -239,15 +239,15 @@
         salt: Optional[int] = None,
         rewrite_uuid: Optional[str] = None,
     ) -> st.DataSpec:
         """
         Rewrites the dataspec 'arg' to the appropriate variant based on its
         properties.
 
-        Currently, the function assumes that there is only one DP/PEP variant
+        Currently, the function assumes that there is only one DP/PUP variant
         for any dataspec (excluding synthetic variants).
         This assumption may change in the future, and the function should be
         updated accordingly.
 
         Args:
             arg (st.DataSpec): The dataspec to be rewritten.
             public_context (Collection[str]): The public context for the
@@ -270,16 +270,16 @@
                 rewritten_arg = self.rewrite_dp(
                     arg,
                     public_context,
                     graph_query_builder=graph_query_builder,
                     salt=salt,
                     rewrite_uuid=rewrite_uuid,
                 )[0]
-            elif arg.is_pep_writable():
-                rewritten_arg = self.rewrite_pep(
+            elif arg.is_pup_writable():
+                rewritten_arg = self.rewrite_pup(
                     arg,
                     public_context,
                     graph_query_builder=graph_query_builder,
                     salt=salt,
                     rewrite_uuid=rewrite_uuid,
                 )[0]
             elif arg.is_public():
@@ -476,17 +476,17 @@
                     dataspec_type=sp.type_name(dataspec.prototype()),
                     dataspec_name=None,
                     **rewritten_kwargs,
                 ),
             )
         # cache result in rewriter
         if rewrite_uuid is not None:
-            self.rewriter_dict()[
-                (dataspec.uuid(), rewrite_uuid)
-            ] = dp_variant.uuid()
+            self.rewriter_dict()[(dataspec.uuid(), rewrite_uuid)] = (
+                dp_variant.uuid()
+            )
 
         # attach constraints
         dp_constraint(
             dataspec=dp_variant,
             required_context=list(public_context),
             privacy_limit=privacy_limit,
             salt=salt,
@@ -517,65 +517,65 @@
             variant=mock_variant,
             kind=st.ConstraintKind.MOCK,
         )
 
         assert dp_variant.is_published()
         return dp_variant, public_context
 
-    def rewrite_pep(
+    def rewrite_pup(
         self,
         dataspec: st.DataSpec,
         public_context: Collection[str],
         graph_query_builder: GraphBuilder,
         salt: Optional[int] = None,
         rewrite_uuid: Optional[str] = None,
     ) -> Tuple[st.DataSpec, Collection[str]]:
         """
-        Return an "is_pep_writable" dataspec into an pep variant.
+        Return an "is_pup_writable" dataspec into an pup variant.
 
         Args:
             dataspec (st.DataSpec): The dataspec to be rewritten.
             public_context (Collection[str]): Not used yet.
             graph_query_builder (GraphBuilder): The graph query builder of the
             dataspec we are rewriting
             salt (Optional[int]): A salt value for the rewriting, if required.
             Default is None.
             rewrite_uuid (Optional[str]): A UUID string for tracking the
             rewrite process. Default is None.
 
         Returns:
             Tuple[st.DataSpec, Collection[str]]: A tuple containing the
-            "is_pep" dataspec and an updated collection of public
+            "is_pup" dataspec and an updated collection of public
             context information.
 
         Note:
-            The dataspec provided must be "is_pep_writable" for the
+            The dataspec provided must be "is_pup_writable" for the
             rewriting to proceed. Ensure that the dataspec
             meets this criterion before invoking this function.
         """
-        if not dataspec.is_pep_writable():
+        if not dataspec.is_pup_writable():
             raise ValueError(
-                "Try to rewrite in pep a non pep appicable dataspec"
+                "Try to rewrite in pup a non pup appicable dataspec"
             )
 
-        if dataspec.is_pep():
+        if dataspec.is_pup():
             return dataspec, public_context
 
         # find already computed variant during the rewriting
         existing_variant = self.find_variant_from_rewriter(
             dataspec.uuid(), rewrite_uuid
         )
         if existing_variant is not None:
             return existing_variant, public_context
 
         if graph_query_builder is not None:
             privacy_limit = extract_privacy_limit(graph_query_builder)
 
         # find already computed variant from constraint
-        kind = st.ConstraintKind.PEP
+        kind = st.ConstraintKind.PUP
         existing_variant = find_dataspec_from_constraint(
             dataspec_validator=self.dataspec_validator(),
             dataspec=dataspec,
             kind=kind,
             public_context=public_context,
             privacy_limit=privacy_limit,
         )
@@ -587,51 +587,51 @@
             dataspec=dataspec,
             public_context=public_context,
             graph_query_builder=graph_query_builder,
             rewrite_uuid=rewrite_uuid,
         )
 
         # create dataspec
-        transform_to_use = self.get_transform_for_pep_rewriting(
+        transform_to_use = self.get_transform_for_pup_rewriting(
             dataspec=dataspec
         )
-        pep_variant = cast(
+        pup_variant = cast(
             st.DataSpec,
             transformed(
                 transform_to_use,
                 *rewritten_args,
                 dataspec_type=sp.type_name(dataspec.prototype()),
                 dataspec_name=None,
                 **rewritten_kwargs,
             ),
         )
 
         # cache result in rewriter
         if rewrite_uuid is not None:
-            self.rewriter_dict()[
-                (dataspec.uuid(), rewrite_uuid)
-            ] = pep_variant.uuid()
+            self.rewriter_dict()[(dataspec.uuid(), rewrite_uuid)] = (
+                pup_variant.uuid()
+            )
 
         # We also attach the dataspec's synthetic/mock variant
         # to be the DP dataspec's synthetic variant. This is to
         # avoid to have DP computations in the MOCK.
         syn_variant = dataspec.variant(st.ConstraintKind.SYNTHETIC)
         if syn_variant is None:
             raise ValueError("Could not find a synthetic variant.")
         attach_variant(
-            original=pep_variant,
+            original=pup_variant,
             variant=syn_variant,
             kind=st.ConstraintKind.SYNTHETIC,
         )
 
         mock_variant = dataspec.variant(st.ConstraintKind.MOCK)
         if mock_variant is None:
             raise ValueError("Could not find a mock variant.")
         attach_variant(
-            original=pep_variant,
+            original=pup_variant,
             variant=mock_variant,
             kind=st.ConstraintKind.MOCK,
         )
 
-        # assert pep_variant.pep_token() is not None
-        assert pep_variant.is_pep()
-        return pep_variant, public_context
+        # assert pup_variant.pup_token() is not None
+        assert pup_variant.is_pup()
+        return pup_variant, public_context
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/simple_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,29 @@
             public_context,
             salt,
         )
         return mock_variant
 
     if privacy_limit is None:
         raise ValueError(
-            "Privacy limit must be defined for PEP or DP rewriting"
+            "Privacy limit must be defined for PUP or DP rewriting"
         )
 
     if kind == st.ConstraintKind.DP:
         variant, _ = rewrite_dp(
             dataspec_validator,
             dataspec,
             public_context=public_context,
             privacy_limit=privacy_limit,
             salt=salt,
         )
         return variant
 
-    elif kind == st.ConstraintKind.PEP:
-        raise NotImplementedError("PEP rewriting")
+    elif kind == st.ConstraintKind.PUP:
+        raise NotImplementedError("PUP rewriting")
 
     else:
         raise ValueError(
             f"Privacy policy {kind} rewriting not implemented yet"
         )
 
 
@@ -150,17 +150,17 @@
         attach_variant(dataspec, syn_variant, kind=st.ConstraintKind.SYNTHETIC)
         return syn_variant, public_context
 
     elif dataspec.is_public():
         return dataspec, public_context
     else:
         raise TypeError(
-            'Non public source Datasets cannot'
-            'be rewritten to Synthetic, a synthetic variant'
-            'should have been created downstream in the graph.'
+            "Non public source Datasets cannot"
+            "be rewritten to Synthetic, a synthetic variant"
+            "should have been created downstream in the graph."
         )
 
 
 def rewrite_mock(
     dataspec_validator: DataspecValidator,
     dataspec: st.DataSpec,
     public_context: Collection[str],
@@ -194,17 +194,17 @@
                 privacy_limit=None,
             ):
                 return variant, public_context
 
     if not dataspec.is_transformed():
         if not dataspec.is_public():
             raise ValueError(
-                'Cannot rewrite the MOCK of a non public source DataSpec. '
-                'A MOCK should be set manually downstream in the '
-                'computation graph.'
+                "Cannot rewrite the MOCK of a non public source DataSpec. "
+                "A MOCK should be set manually downstream in the "
+                "computation graph."
             )
         else:
             return dataspec, public_context
 
     # The DataSpec is the result of an internal transform
     transform = dataspec.transform()
     args, kwargs = dataspec.parents()
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,23 @@
 from sarus_data_spec.storage.typing import Storage
 import sarus_data_spec.typing as st
 
 logger = logging.getLogger(__name__)
 
 
 class DataspecRewriter(Protocol):
-    def storage(self) -> Storage:
-        ...
+    def storage(self) -> Storage: ...
 
-    def dataspec_validator(self) -> DataspecValidator:
-        ...
+    def dataspec_validator(self) -> DataspecValidator: ...
 
     def variant(
         self,
         dataspec: st.DataSpec,
         kind: st.ConstraintKind,
         public_context: Collection[str],
         privacy_limit: Optional[st.PrivacyLimit],
         salt: Optional[int] = None,
-    ) -> Optional[st.DataSpec]:
-        ...
+    ) -> Optional[st.DataSpec]: ...
 
     def variants(self, dataspec: st.DataSpec) -> Collection[st.DataSpec]:
         """Return all variants attached to a Dataspec."""
         ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_rewriter/utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_rewriter/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 import json
 import logging
 
 from sarus_data_spec.attribute import attach_properties
 from sarus_data_spec.constants import (
     IS_VALID,
     NO_TOKEN,
-    PEP_TOKEN,
     PRIVATE_QUERY,
     PUBLIC,
+    PUP_TOKEN,
 )
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.manager.async_utils import sync
 from sarus_data_spec.manager.ops.processor import routing
 from sarus_data_spec.manager.ops.processor.external.external_op import (
     external_implementation,
 )
 from sarus_data_spec.protobuf.utilities import dejson
 from sarus_data_spec.protobuf.utilities import json as proto_to_json
 from sarus_data_spec.storage.typing import Storage
 from sarus_data_spec.transform import handle_big_data
 from sarus_data_spec.variant_constraint import (
-    pep_constraint,
     public_constraint,
+    pup_constraint,
     syn_constraint,
 )
 import sarus_data_spec.dataspec_validator.simple_rules as verification_rules
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 try:
@@ -236,70 +236,70 @@
             is_public = False
 
         # save variant constraint
         public_constraint(dataspec, is_public)
 
         return is_public
 
-    def pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
-        """Return a token if the dataspec is PEP, otherwise return None.
+    def pup_token(self, dataspec: st.DataSpec) -> Optional[str]:
+        """Return a token if the dataspec is PUP, otherwise return None.
 
-        DataSpec.pep_token() returns a PEP token if the dataset is PEP and None
-        otherwise. The PEP token is stored in the properties of the
+        DataSpec.pup_token() returns a PUP token if the dataset is PUP and None
+        otherwise. The PUP token is stored in the properties of the
         VariantConstraint. It is a hash initialized with a value when the
         Dataset is protected.
 
         If a transform does not preserve the PEID then the token is set to None
         If a transform preserves the PEID assignment but changes the rows (e.g.
         sample, shuffle, filter,...) then the token's value is changed If a
         transform does not change the rows (e.g. selecting a column, adding a
         scalar,...) then the token is passed without change
 
-        A Dataspec is PEP if its PEP token is not None. Two PEP Dataspecs are
+        A Dataspec is PUP if its PUP token is not None. Two PUP Dataspecs are
         aligned (i.e. they have the same number of rows and all their rows have
         the same PEID) if their tokens are equal.
         """
         if dataspec.prototype() == sp.Scalar:
             return None
 
         dataset = cast(st.Dataset, dataspec)
 
         # TODO fetch real context and budget
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
-        kind = st.ConstraintKind.PEP
+        kind = st.ConstraintKind.PUP
 
         for constraint in self.verified_constraints(dataspec):
             check_constraint = self.verifies(
                 constraint, kind, public_context, privacy_limit
             )
             if check_constraint is not None:
                 if check_constraint:
-                    return constraint.properties()[PEP_TOKEN]
+                    return constraint.properties()[PUP_TOKEN]
                 else:
                     return None
 
-        # Compute the PEP token
+        # Compute the PUP token
         if not dataset.is_transformed():
             return None
 
         transform = dataset.transform()
         _, StaticChecker = routing.get_dataset_op(transform)
-        pep_token = StaticChecker(dataset).pep_token(public_context)
-        if pep_token is None:
-            pep_token = NO_TOKEN
+        pup_token = StaticChecker(dataset).pup_token(public_context)
+        if pup_token is None:
+            pup_token = NO_TOKEN
 
-        pep_constraint(
+        pup_constraint(
             dataspec=dataset,
-            token=pep_token,
+            token=pup_token,
             required_context=[],
             privacy_limit=privacy_limit,
         )
 
-        return None if pep_token == NO_TOKEN else pep_token
+        return None if pup_token == NO_TOKEN else pup_token
 
     def private_queries(self, dataspec: st.DataSpec) -> List[st.PrivateQuery]:
         """Return the list of PrivateQueries used in a Dataspec's transform.
 
         It represents the privacy loss associated with the current computation.
 
         It can be used by Sarus when a user (Access object) reads a DP dataspec
@@ -419,24 +419,24 @@
             properties={IS_VALID: str(is_valid)},
         )
         return is_valid
 
     def is_dp_writable(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
-    def is_pep_writable(self, dataspec: st.DataSpec) -> bool:
+    def is_pup_writable(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
     def is_publishable(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
     def is_published(self, dataspec: st.DataSpec) -> bool:
         raise NotImplementedError
 
-    def rewritten_pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
+    def rewritten_pup_token(self, dataspec: st.DataSpec) -> Optional[str]:
         raise NotImplementedError
 
     def is_big_data_computable(self, dataspec: st.DataSpec) -> bool:
         """
         Check if the dataspec can be computed if the source is bigdata.
         Certain transformations are designed to handle big data datasets,
         meaning that the transformation can be converted into an SQL
@@ -455,18 +455,18 @@
 
         source_ds = sources.pop()
         if not manager.is_big_data(source_ds):
             return True
 
         # TODO: to remove when it actually works without this
         if dataspec.is_transformed() and dataspec.transform().name() in [
-            'budget_assignment',
-            'attributes_budget',
-            'Protect',
-            'automatic_budget',
+            "budget_assignment",
+            "attributes_budget",
+            "Protect",
+            "automatic_budget",
         ]:
             return True
 
         parents = dataspec.parents_list()
         if not handle_big_data(dataspec.transform()):
             if any(
                 [
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/parameter_kind.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/parameter_kind.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         ]
     )
 
 
 class ParameterKind(Enum):
     DATASET = auto()
     SCALAR = auto()
-    PEP = auto()
+    PUP = auto()
     PUBLIC = auto()
     STATIC = auto()
     TRANSFORM = auto()
 
     def __and__(
         self, other: t.Union[AcceptanceCondition, ParameterKind]
     ) -> AcceptanceCondition:
@@ -125,11 +125,11 @@
 
 # Aliases
 ParameterCondition = t.Union[AcceptanceCondition, ParameterKind]
 
 DATASET = ParameterKind.DATASET
 SCALAR = ParameterKind.SCALAR
 STATIC = ParameterKind.STATIC
-PEP = ParameterKind.PEP
-PEP_DATASET = ParameterKind.DATASET & ParameterKind.PEP
+PUP = ParameterKind.PUP
+PUP_DATASET = ParameterKind.DATASET & ParameterKind.PUP
 DATASPEC = ParameterKind.SCALAR | ParameterKind.DATASET
 TRANSFORM = ParameterKind.TRANSFORM
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/privacy_limit.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/privacy_limit.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/recursive_validator.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/recursive_validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 from __future__ import annotations
 
 from typing import Collection, List, Optional, cast
 import logging
 
-from sarus_data_spec.constants import NO_TOKEN, PEP_TOKEN
+from sarus_data_spec.constants import NO_TOKEN, PUP_TOKEN
 from sarus_data_spec.dataspec_rewriter.utils import graph_private_queries
 from sarus_data_spec.dataspec_validator.base import BaseDataspecValidator
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 from sarus_data_spec.manager.ops.processor import routing
 from sarus_data_spec.storage.typing import Storage
-from sarus_data_spec.variant_constraint import pep_for_rewriting_constraint
+from sarus_data_spec.variant_constraint import pup_for_rewriting_constraint
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 logger = logging.getLogger(__name__)
 
 
 class RecursiveDataspecValidator(BaseDataspecValidator):
     def __init__(self, storage: Storage):
         self._storage = storage
 
     # Local property
     def is_dp_able(self, dataspec: st.DataSpec) -> bool:
         """Checks if the dataspec has a transform that either has a DP
         equivalent, allowing the rewritten dataspec to be considered DP
-        if the input rewritten PEP token is not None."""
+        if the input rewritten PUP token is not None."""
         if not dataspec.is_transformed():
             return False
 
         if dataspec.is_dp():
             return True
 
         _, StaticChecker = routing.get_op(dataspec)
         return StaticChecker(dataspec).is_dp_able()
 
-    def is_pep_able(self, dataspec: st.DataSpec) -> bool:
-        """Checks if the dataspec has a transform that either has a PEP
+    def is_pup_able(self, dataspec: st.DataSpec) -> bool:
+        """Checks if the dataspec has a transform that either has a PUP
         equivalent or does not require one, allowing the rewritten dataspec to
-        be considered 'PEP' if the input rewritten PEP token is not None."""
-        if dataspec.is_pep():
+        be considered 'PUP' if the input rewritten PUP token is not None."""
+        if dataspec.is_pup():
             return True
 
         _, StaticChecker = routing.get_op(dataspec)
-        return StaticChecker(dataspec).is_pep_able()
+        return StaticChecker(dataspec).is_pup_able()
 
     def is_dp_writable(self, dataspec: st.DataSpec) -> bool:
         if not self.is_dp_able(dataspec):
             return False
 
         if dataspec.is_dp():
             return True
 
         _, StaticChecker = routing.get_op(dataspec)
         return StaticChecker(dataspec).is_dp_writable([])
 
-    def is_pep_writable(self, dataspec: st.DataSpec) -> bool:
-        if not self.is_pep_able(dataspec):
+    def is_pup_writable(self, dataspec: st.DataSpec) -> bool:
+        if not self.is_pup_able(dataspec):
             return False
 
-        return self.rewritten_pep_token(dataspec) is not None
+        return self.rewritten_pup_token(dataspec) is not None
 
     def is_publishable(self, dataspec: st.DataSpec) -> bool:
         if not dataspec.is_transformed():
             return False
 
         if self.is_dp_writable(dataspec):
             return True
@@ -88,62 +88,62 @@
             return True
 
         parents = dataspec.parents_list()
         return all(
             [self.is_published(dataspec_parent) for dataspec_parent in parents]
         )
 
-    def rewritten_pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
-        """Returns the PEP token for the DP variant of this dataspec
+    def rewritten_pup_token(self, dataspec: st.DataSpec) -> Optional[str]:
+        """Returns the PUP token for the DP variant of this dataspec
         during DP rewriting.
 
-        Currently, the implementation assumes a single DP/PEP variant per
+        Currently, the implementation assumes a single DP/PUP variant per
         dataspec, resulting in one possible value for
-        "rewritten_pep_token."
+        "rewritten_pup_token."
         Future changes could introduce multiple variants, necessitating
         the implementation of priority rules.
         """
         if dataspec.prototype() == sp.Scalar:
             return None
 
         dataset = cast(st.Dataset, dataspec)
 
         # TODO fetch real context and budget
         public_context: Collection[str] = []
         privacy_limit = DeltaEpsilonLimit({0.0: 0.0})
-        kind = st.ConstraintKind.PEP_FOR_REWRITING
+        kind = st.ConstraintKind.PUP_FOR_REWRITING
 
         for constraint in self.verified_constraints(dataspec):
             check_constraint = self.verifies(
                 constraint, kind, public_context, privacy_limit
             )
             if check_constraint is not None:
                 if check_constraint:
-                    return constraint.properties()[PEP_TOKEN]
+                    return constraint.properties()[PUP_TOKEN]
                 else:
                     return None
 
-        # Compute the PEP token
+        # Compute the PUP token
         if not dataset.is_transformed():
             return None
 
         transform = dataset.transform()
         _, StaticChecker = routing.get_dataset_op(transform)
-        pep_token = StaticChecker(dataset).rewritten_pep_token(public_context)
-        if pep_token is None:
-            pep_token = NO_TOKEN
+        pup_token = StaticChecker(dataset).rewritten_pup_token(public_context)
+        if pup_token is None:
+            pup_token = NO_TOKEN
 
-        pep_for_rewriting_constraint(
+        pup_for_rewriting_constraint(
             dataspec=dataset,
-            token=pep_token,
+            token=pup_token,
             required_context=[],
             privacy_limit=privacy_limit,
         )
 
-        return None if pep_token == NO_TOKEN else pep_token
+        return None if pup_token == NO_TOKEN else pup_token
 
     def graph_private_queries(
         self, dataspec: st.DataSpec
     ) -> List[st.PrivateQuery]:
         """Return the list of PrivateQueries used in a Dataspec's transform.
 
         This method collect all the private queries of the  computation graph.
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/signature.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/signature.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sarus_data_spec.arrow.admin_utils import (
     async_admin_data,
     validate_admin_data,
 )
 from sarus_data_spec.dataspec_validator.parameter_kind import (
     DATASET,
     DATASPEC,
-    PEP_DATASET,
+    PUP_DATASET,
     SCALAR,
     STATIC,
     TRANSFORM,
     ParameterCondition,
     is_accepted,
 )
 from sarus_data_spec.manager.ops.processor.external.utils import (
@@ -347,44 +347,44 @@
 
     def parameter_kind(self) -> ParameterCondition:
         """Return the value type associated with the Parameter."""
         if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
             if dataspec.prototype() == sp.Dataset:
                 dataset = t.cast(st.Dataset, dataspec)
-                if dataset.is_pep():
-                    return PEP_DATASET
+                if dataset.is_pup():
+                    return PUP_DATASET
                 else:
                     return DATASET
             else:
                 return SCALAR
         elif isinstance(self.static_value(), st.Transform):
             return TRANSFORM
         else:
             return STATIC
 
-    def pep_token(self) -> t.Optional[str]:
+    def pup_token(self) -> t.Optional[str]:
         if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
-            return dataspec.pep_token()
+            return dataspec.pup_token()
         else:
             return None
 
-    def rewritten_pep_token(self) -> t.Optional[str]:
+    def rewritten_pup_token(self) -> t.Optional[str]:
         if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
-            return dataspec.rewritten_pep_token()
+            return dataspec.rewritten_pup_token()
         else:
             return None
 
-    def is_pep(self) -> bool:
-        return self.pep_token() is not None
+    def is_pup(self) -> bool:
+        return self.pup_token() is not None
 
-    def is_pep_for_rewriting(self) -> bool:
-        return self.rewritten_pep_token() is not None
+    def is_pup_for_rewriting(self) -> bool:
+        return self.rewritten_pup_token() is not None
 
     def is_public(self) -> bool:
         if isinstance(self.static_value(), st.DataSpec):
             dataspec = t.cast(st.DataSpec, self.static_value())
             return dataspec.is_public()
         else:
             return True
@@ -430,16 +430,15 @@
             value = self.static_value()
             if not self.parameter.predicate(value):
                 raise ValueError(
                     f"Got invalid value `{value}` for "
                     f"parameter `{self.name()}`"
                 )
 
-    async def dynamic_validation(self) -> None:
-        ...
+    async def dynamic_validation(self) -> None: ...
 
     async def collect(self) -> t.Any:
         """Evaluate the argument before calling the data function."""
         if isinstance(self.static_value(), st.DataSpec):
             ds = t.cast(st.DataSpec, self.static_value())
             if ds.prototype() == sp.Dataset:
                 dataset = t.cast(st.Dataset, self.static_value())
@@ -507,23 +506,23 @@
                     value=value,
                     positional_only=self.positional_only,
                 )
 
         return arg_callable
 
     async def admin_data(self) -> t.Optional[pa.Table]:
-        if not self.is_pep():
+        if not self.is_pup():
             return None
 
         dataset = t.cast(st.Dataset, self.static_value())
         admin_data = await async_admin_data(dataset)
         if admin_data is None:
             raise ValueError(
                 f"The dataset {dataset.uuid()} was"
-                " inferred PEP but has no admin data."
+                " inferred PUP but has no admin data."
             )
         return admin_data
 
 
 class SarusBoundSignature:
     """A BoundSignature is a list of BoundArguments."""
 
@@ -641,71 +640,71 @@
             arg.name(): await arg.collect()
             for arg in self.arguments
             if not arg.positional_only
         }
 
         return positional_values, keyword_values
 
-    def pep_token(self) -> t.Optional[str]:
-        """Compute the PEP token of the inputs.
+    def pup_token(self) -> t.Optional[str]:
+        """Compute the PUP token of the inputs.
 
-        A PEP token exists if:
-          - all input dataspecs are PEP or PUBLIC
-          - there must be at least one input PEP dataspec
-          - if there are more that one input PEP dataspecs, all PEP inputs must
+        A PUP token exists if:
+          - all input dataspecs are PUP or PUBLIC
+          - there must be at least one input PUP dataspec
+          - if there are more that one input PUP dataspecs, all PUP inputs must
             have the same token
         """
 
         if not all(
             [
-                arg.is_public() or arg.is_pep() or arg.is_published()
+                arg.is_public() or arg.is_pup() or arg.is_published()
                 for arg in self.arguments
             ]
         ):
             return None
 
-        pep_args = [arg for arg in self.arguments if arg.is_pep()]
-        if len(pep_args) == 0:
+        pup_args = [arg for arg in self.arguments if arg.is_pup()]
+        if len(pup_args) == 0:
             return None
 
-        tokens = [arg.pep_token() for arg in pep_args]
+        tokens = [arg.pup_token() for arg in pup_args]
         unique_tokens = set(tokens)
         if len(unique_tokens) != 1:
             return None
         else:
             return unique_tokens.pop()
 
-    def rewritten_pep_token(self) -> t.Optional[str]:
+    def rewritten_pup_token(self) -> t.Optional[str]:
         if not all(
             [
                 arg.is_public()
-                or arg.is_pep_for_rewriting()
+                or arg.is_pup_for_rewriting()
                 or arg.is_publishable()
                 for arg in self.arguments
             ]
         ):
             return None
 
-        pep_args = [
-            arg for arg in self.arguments if arg.is_pep_for_rewriting()
+        pup_args = [
+            arg for arg in self.arguments if arg.is_pup_for_rewriting()
         ]
-        if len(pep_args) == 0:
+        if len(pup_args) == 0:
             return None
 
-        tokens = [arg.rewritten_pep_token() for arg in pep_args]
+        tokens = [arg.rewritten_pup_token() for arg in pup_args]
         unique_tokens = set(tokens)
         if len(unique_tokens) != 1:
             return None
         else:
             return unique_tokens.pop()
 
     async def admin_data(self) -> pa.Table:
         """Return the admin data of the inputs."""
         admin_data = [
-            await arg.admin_data() for arg in self.arguments if arg.is_pep()
+            await arg.admin_data() for arg in self.arguments if arg.is_pup()
         ]
         if len(admin_data) == 0:
             raise ValueError(
                 "The list of input admin data is empty "
                 f"among arguments {self.arguments}"
             )
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/simple_rules.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/simple_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Collection, List, Optional, Tuple, cast
 import logging
 
 from sarus_data_spec.constants import (
     IS_PUBLIC,
     IS_SYNTHETIC,
     NO_TOKEN,
-    PEP_TOKEN,
+    PUP_TOKEN,
     SALT,
 )
 import sarus_data_spec.typing as st
 
 ArgStruct = Tuple[List[int], List[str]]
 logger = logging.getLogger(__name__)
 
@@ -32,18 +32,18 @@
 
     elif kind == st.ConstraintKind.DP:
         return verifies_dp(
             variant_constraint=variant_constraint,
             privacy_limit=privacy_limit,
             salt=salt,
         )
-    elif kind == st.ConstraintKind.PEP:
-        return verifies_pep(variant_constraint=variant_constraint)
-    else:  # kind == st.ConstraintKind.PEP_FOR_REWRITING:
-        return verifies_pep_for_rewriting(
+    elif kind == st.ConstraintKind.PUP:
+        return verifies_pup(variant_constraint=variant_constraint)
+    else:  # kind == st.ConstraintKind.PUP_FOR_REWRITING:
+        return verifies_pup_for_rewriting(
             variant_constraint=variant_constraint
         )
 
 
 def verifies_public(
     variant_constraint: st.VariantConstraint,
 ) -> Optional[bool]:
@@ -73,35 +73,35 @@
     kind = variant_constraint.constraint_kind()
     if kind == st.ConstraintKind.MOCK:
         return True
     else:
         return None
 
 
-def verifies_pep(
+def verifies_pup(
     variant_constraint: st.VariantConstraint,
 ) -> Optional[bool]:
-    """If we attached a PEP constraint to a dataspec then it is PEP.
+    """If we attached a PUP constraint to a dataspec then it is PUP.
 
     NB: for now we don't check the context nor the privacy limit
     """
     kind = variant_constraint.constraint_kind()
-    if kind == st.ConstraintKind.PEP:
-        stored_token = variant_constraint.properties()[PEP_TOKEN]
+    if kind == st.ConstraintKind.PUP:
+        stored_token = variant_constraint.properties()[PUP_TOKEN]
         return False if stored_token == NO_TOKEN else True
     else:
         return None
 
 
-def verifies_pep_for_rewriting(
+def verifies_pup_for_rewriting(
     variant_constraint: st.VariantConstraint,
 ) -> Optional[bool]:
     kind = variant_constraint.constraint_kind()
-    if kind == st.ConstraintKind.PEP_FOR_REWRITING:
-        stored_token = variant_constraint.properties()[PEP_TOKEN]
+    if kind == st.ConstraintKind.PUP_FOR_REWRITING:
+        stored_token = variant_constraint.properties()[PUP_TOKEN]
         return False if stored_token == NO_TOKEN else True
     else:
         return None
 
 
 def verifies_dp(
     variant_constraint: st.VariantConstraint,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/dataspec_validator/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/dataspec_validator/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,24 +13,23 @@
 class DataspecPrivacyPolicy(Enum):
     WHITE_LISTED = "Whitelisted"
     DP = "Differentially-private evaluation"
     SYNTHETIC = "Evaluated from synthetic data only"
     PUBLIC = "Public"
 
 
-class PEPKind(Enum):
-    NOT_PEP = 0
-    PEP = 1
+class PUPKind(Enum):
+    NOT_PUP = 0
+    PUP = 1
     TOKEN_PRESERVING = 2
     ROW = 3
 
 
 class DataspecValidator(Protocol):
-    def storage(self) -> Storage:
-        ...
+    def storage(self) -> Storage: ...
 
     def verifies(
         self,
         variant_constraint: st.VariantConstraint,
         kind: st.ConstraintKind,
         public_context: Collection[str],
         privacy_limit: Optional[st.PrivacyLimit],
@@ -57,29 +56,29 @@
         """Return the list of VariantConstraints attached to a DataSpec.
 
         A VariantConstraint attached to a DataSpec means that the DataSpec
         verifies the constraint.
         """
         ...
 
-    def pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
-        """Return a token if the dataspec is PEP, otherwise return None.
+    def pup_token(self, dataspec: st.DataSpec) -> Optional[str]:
+        """Return a token if the dataspec is PUP, otherwise return None.
 
-        DataSpec.pep_token() returns a PEP token if the dataset is PEP and None
-        otherwise. The PEP token is stored in the properties of the
+        DataSpec.pup_token() returns a PUP token if the dataset is PUP and None
+        otherwise. The PUP token is stored in the properties of the
         VariantConstraint. It is a hash initialized with a value when the
         Dataset is protected.
 
         If a transform does not preserve the PEID then the token is set to None
         If a transform preserves the PEID assignment but changes the rows (e.g.
         sample, shuffle, filter,...) then the token's value is changed If a
         transform does not change the rows (e.g. selecting a column, adding a
         scalar,...) then the token is passed without change
 
-        A Dataspec is PEP if its PEP token is not None. Two PEP Dataspecs are
+        A Dataspec is PUP if its PUP token is not None. Two PUP Dataspecs are
         aligned (i.e. they have the same number of rows and all their rows have
         the same PEID) if their tokens are equal.
         """
         ...
 
     def is_public(self, dataspec: st.DataSpec) -> bool:
         """Return True if the dataspec is public.
@@ -121,33 +120,28 @@
         It can be used by Sarus when a user (Access object) reads a DP dataspec
         to update its accountant. Note that Private Query objects are generated
         with a random uuid so that even if they are submitted multiple times to
         an account, they are only accounted once (ask @cgastaud for more on
         accounting)."""
         ...
 
-    def is_dp_writable(self, dataspec: st.DataSpec) -> bool:
-        ...
+    def is_dp_writable(self, dataspec: st.DataSpec) -> bool: ...
 
-    def is_pep_writable(self, dataspec: st.DataSpec) -> bool:
-        ...
+    def is_pup_writable(self, dataspec: st.DataSpec) -> bool: ...
 
-    def is_publishable(self, dataspec: st.DataSpec) -> bool:
-        ...
+    def is_publishable(self, dataspec: st.DataSpec) -> bool: ...
 
-    def is_published(self, dataspec: st.DataSpec) -> bool:
-        ...
+    def is_published(self, dataspec: st.DataSpec) -> bool: ...
 
-    def rewritten_pep_token(self, dataspec: st.DataSpec) -> Optional[str]:
-        """Returns the PEP token for the DP variant of this dataspec
+    def rewritten_pup_token(self, dataspec: st.DataSpec) -> Optional[str]:
+        """Returns the PUP token for the DP variant of this dataspec
         during DP rewriting.
 
-        Currently, the implementation assumes a single DP/PEP variant per
+        Currently, the implementation assumes a single DP/PUP variant per
         dataspec, resulting in one possible value for
-        "rewritten_pep_token."
+        "rewritten_pup_token."
         Future changes could introduce multiple variants, necessitating
         the implementation of priority rules.
         """
         ...
 
-    def is_big_data_computable(self, dataspec: st.DataSpec) -> bool:
-        ...
+    def is_big_data_computable(self, dataspec: st.DataSpec) -> bool: ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/deprecation.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/deprecation.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,30 +125,31 @@
             "removed_in": "\n   This will be removed in {}.".format(removed_in)
             if removed_in
             else "",
             "details": " %s" % details if details else "",
         }
 
         deprecation_note = (
-            ".. deprecated::{deprecated_in}"
-            "{removed_in}{details}".format(**parts)
+            ".. deprecated::{deprecated_in}" "{removed_in}{details}".format(
+                **parts
+            )
         )
 
         # default location for insertion of deprecation note
         loc = 1
 
         # split docstring at first occurrence of newline
         string_list = existing_docstring.split("\n", 1)
 
         if len(string_list) > 1:
             # With a multi-line docstring, when we modify
             # existing_docstring to add our deprecation_note,
             # if we're not careful we'll interfere with the
             # indentation levels of the contents below the
-            # first line, or as PEP 257 calls it, the summary
+            # first line, or as PUP 257 calls it, the summary
             # line. Since the summary line can start on the
             # same line as the """, dedenting the whole thing
             # won't help. Split the summary and contents up,
             # dedent the contents independently, then join
             # summary, dedent'ed contents, and our
             # deprecation_note.
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/factory.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self) -> None:
         self.type_name_create: MutableMapping[str, Builder] = {}
 
     def register(self, name: str, create: Builder) -> None:
         self.type_name_create[name] = create
 
-    M = TypeVar('M', bound=Protobuf)
+    M = TypeVar("M", bound=Protobuf)
 
     def create(self, message: M, store: bool = True) -> st.HasProtobuf[M]:
         """Instantiate a wrapping class from a protobuf message.
 
         Factory functions (builders) may optionally take a `store` parameter.
         We check dynamically if the registered builder accepts the `store`
         parameter and pass it the `store` parameter accordingly.
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/json_serialisation.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/json_serialisation.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,203 +7,203 @@
 import numpy as np
 import pandas as pd
 
 
 class SarusJSONEncoder(json.JSONEncoder):
     def default(self, obj: Any) -> Any:
         if isinstance(obj, np.ndarray):
-            return {'_type': 'numpy.ndarray', 'data': obj.tolist()}
+            return {"_type": "numpy.ndarray", "data": obj.tolist()}
         elif isinstance(obj, pd.DataFrame):
             return {
-                '_type': 'pandas.DataFrame',
-                'data': obj.to_json(date_format='iso'),
+                "_type": "pandas.DataFrame",
+                "data": obj.to_json(date_format="iso"),
             }
         elif isinstance(obj, pd.Series):
             return {
-                '_type': 'pandas.Series',
-                'data': obj.to_json(date_format='iso'),
+                "_type": "pandas.Series",
+                "data": obj.to_json(date_format="iso"),
             }
         elif isinstance(obj, pd.Timestamp):
-            return {'_type': 'pandas.Timestamp', 'data': obj.isoformat()}
+            return {"_type": "pandas.Timestamp", "data": obj.isoformat()}
         elif isinstance(obj, datetime):
-            return {'_type': 'datetime', 'data': obj.isoformat()}
+            return {"_type": "datetime", "data": obj.isoformat()}
         elif isinstance(obj, timedelta):
-            return {'_type': 'timedelta', 'data': obj.total_seconds()}
+            return {"_type": "timedelta", "data": obj.total_seconds()}
         elif isinstance(obj, timezone):
             utcoffset_result = obj.utcoffset(None)
             if utcoffset_result is not None:
                 return {
-                    '_type': 'timezone',
-                    'data': utcoffset_result.total_seconds(),
+                    "_type": "timezone",
+                    "data": utcoffset_result.total_seconds(),
                 }
             else:
                 raise ValueError("Invalid timezone object")
         elif isinstance(obj, time):
-            return {'_type': 'time', 'data': obj.isoformat()}
+            return {"_type": "time", "data": obj.isoformat()}
         elif isinstance(obj, date):
-            return {'_type': 'date', 'data': obj.isoformat()}
+            return {"_type": "date", "data": obj.isoformat()}
         elif isinstance(obj, np.generic):
             if np.issubdtype(obj, np.complexfloating):
                 complex_obj = obj.astype(np.complex128)
                 return {
-                    '_type': 'numpy.complex',
-                    'data': {
+                    "_type": "numpy.complex",
+                    "data": {
                         '"real"': complex_obj.real,
                         '"imag"': complex_obj.imag,
                     },
                 }
             else:
-                return {'_type': 'numpy.generic', 'data': obj.item()}
+                return {"_type": "numpy.generic", "data": obj.item()}
         elif isinstance(obj, pd.MultiIndex):
             return {
-                '_type': 'pandas.MultiIndex',
-                'data': obj.tolist(),
-                'names': obj.names,
-                'levels': [level.tolist() for level in obj.levels],
-                'codes': list(obj.codes),
+                "_type": "pandas.MultiIndex",
+                "data": obj.tolist(),
+                "names": obj.names,
+                "levels": [level.tolist() for level in obj.levels],
+                "codes": list(obj.codes),
             }
         elif isinstance(obj, pd.Index):
             return {
-                '_type': 'pandas.Index',
-                'class': type(obj).__name__,
-                'data': obj.tolist(),
-                'dtype': str(obj.dtype),
+                "_type": "pandas.Index",
+                "class": type(obj).__name__,
+                "data": obj.tolist(),
+                "dtype": str(obj.dtype),
             }
         elif isinstance(obj, pd.Period):
             return {
-                '_type': 'pandas.Period',
-                'data': str(obj),
-                'freq': obj.freqstr,
+                "_type": "pandas.Period",
+                "data": str(obj),
+                "freq": obj.freqstr,
             }
         elif isinstance(obj, pd.Timedelta):
-            return {'_type': 'pandas.Timedelta', 'data': obj.value}
+            return {"_type": "pandas.Timedelta", "data": obj.value}
         elif isinstance(obj, pd.Interval):
-            return {'_type': 'pandas.Interval', 'data': (obj.left, obj.right)}
+            return {"_type": "pandas.Interval", "data": (obj.left, obj.right)}
         elif isinstance(obj, pd.Categorical):
             return {
-                '_type': 'pandas.Categorical',
-                'data': obj.tolist(),
-                'categories': obj.categories.tolist(),
-                'ordered': obj.ordered,
+                "_type": "pandas.Categorical",
+                "data": obj.tolist(),
+                "categories": obj.categories.tolist(),
+                "ordered": obj.ordered,
             }
         elif isinstance(obj, type):
             return {
-                '_type': 'class',
-                'data': {'"name"': obj.__name__, '"module"': obj.__module__},
+                "_type": "class",
+                "data": {'"name"': obj.__name__, '"module"': obj.__module__},
             }
         elif isinstance(obj, pd.api.extensions.ExtensionDtype):
-            return {'_type': 'dtype', 'data': str(obj)}
+            return {"_type": "dtype", "data": str(obj)}
         elif isinstance(obj, slice):
-            return {'_type': 'slice', 'data': (obj.start, obj.stop, obj.step)}
+            return {"_type": "slice", "data": (obj.start, obj.stop, obj.step)}
         elif isinstance(obj, range):
             return {
-                '_type': 'range',
-                'data': {
+                "_type": "range",
+                "data": {
                     '"start"': obj.start,
                     '"stop"': obj.stop,
                     '"step"': obj.step,
                 },
             }
         return super().default(obj)
 
     def encode_obj(self, obj: Any) -> Any:
         if isinstance(obj, tuple):
             return {
-                '_type': 'tuple',
-                'data': [self.encode_obj(v) for v in obj],
+                "_type": "tuple",
+                "data": [self.encode_obj(v) for v in obj],
             }
         elif isinstance(obj, list):
             return [self.encode_obj(v) for v in obj]
         elif isinstance(obj, dict):
             return {self.encode(k): self.encode_obj(v) for k, v in obj.items()}
         return obj
 
     def encode(self, obj: Any) -> str:
         obj_transformed = self.encode_obj(obj)
         return super().encode(obj_transformed)
 
     @classmethod
     def encode_bytes(cls, obj: Any) -> bytes:
         encoder = cls()
-        return (encoder.encode(obj)).encode('utf-8')
+        return (encoder.encode(obj)).encode("utf-8")
 
 
 class SarusJSONDecoder(json.JSONDecoder):
     def decode(self, s: str, *args: Any, **kwargs: Any) -> Any:
         obj = super().decode(s, *args, **kwargs)
         return self.decode_obj(obj)
 
     def decode_obj(self, obj: Any) -> Any:
         if isinstance(obj, dict):
-            if '_type' in obj:
-                data = self.decode_obj(obj['data'])
-                if obj['_type'] == 'tuple':
+            if "_type" in obj:
+                data = self.decode_obj(obj["data"])
+                if obj["_type"] == "tuple":
                     return tuple(self.decode_obj(v) for v in data)
-                elif obj['_type'] == 'numpy.ndarray':
+                elif obj["_type"] == "numpy.ndarray":
                     return np.array(data)
-                elif obj['_type'] == 'pandas.DataFrame':
+                elif obj["_type"] == "pandas.DataFrame":
                     return pd.read_json(data, convert_dates=True)
-                elif obj['_type'] == 'pandas.Series':
-                    return pd.read_json(data, typ='series', convert_dates=True)
-                elif obj['_type'] == 'pandas.Timestamp':
+                elif obj["_type"] == "pandas.Series":
+                    return pd.read_json(data, typ="series", convert_dates=True)
+                elif obj["_type"] == "pandas.Timestamp":
                     return pd.Timestamp(data)
-                elif obj['_type'] == 'datetime':
+                elif obj["_type"] == "datetime":
                     return parse(data)
-                elif obj['_type'] == 'timedelta':
+                elif obj["_type"] == "timedelta":
                     return timedelta(seconds=data)
-                elif obj['_type'] == 'timezone':
+                elif obj["_type"] == "timezone":
                     return timezone(timedelta(seconds=data))
-                elif obj['_type'] == 'time':
+                elif obj["_type"] == "time":
                     return parse(data).time()
-                elif obj['_type'] == 'date':
+                elif obj["_type"] == "date":
                     return parse(data).date()
-                elif obj['_type'] == 'numpy.generic':
+                elif obj["_type"] == "numpy.generic":
                     return np.array(data).item()
-                elif obj['_type'] == 'numpy.complex':
-                    return np.complex128(complex(data['real'], data['imag']))
-                elif obj['_type'] == 'pandas.Index':
-                    cls = getattr(pd, obj['class'])
-                    return cls(data, dtype=obj['dtype'])
-                elif obj['_type'] == 'pandas.MultiIndex':
+                elif obj["_type"] == "numpy.complex":
+                    return np.complex128(complex(data["real"], data["imag"]))
+                elif obj["_type"] == "pandas.Index":
+                    cls = getattr(pd, obj["class"])
+                    return cls(data, dtype=obj["dtype"])
+                elif obj["_type"] == "pandas.MultiIndex":
                     return pd.MultiIndex(
-                        levels=[pd.Index(level) for level in obj['levels']],
-                        codes=self.decode_obj(obj['codes']),
-                        names=obj['names'],
+                        levels=[pd.Index(level) for level in obj["levels"]],
+                        codes=self.decode_obj(obj["codes"]),
+                        names=obj["names"],
                     )
-                elif obj['_type'] == 'pandas.Period':
-                    return pd.Period(data, freq=obj['freq'])
-                elif obj['_type'] == 'pandas.Timedelta':
+                elif obj["_type"] == "pandas.Period":
+                    return pd.Period(data, freq=obj["freq"])
+                elif obj["_type"] == "pandas.Timedelta":
                     return pd.to_timedelta(data)
-                elif obj['_type'] == 'pandas.Interval':
+                elif obj["_type"] == "pandas.Interval":
                     return pd.Interval(*data)
-                elif obj['_type'] == 'pandas.Categorical':
+                elif obj["_type"] == "pandas.Categorical":
                     return pd.Categorical(
                         data,
-                        categories=obj['categories'],
-                        ordered=obj['ordered'],
+                        categories=obj["categories"],
+                        ordered=obj["ordered"],
                     )
-                elif obj['_type'] == 'class':
-                    if data['module'] in ['builtins', 'numpy', 'pandas']:
+                elif obj["_type"] == "class":
+                    if data["module"] in ["builtins", "numpy", "pandas"]:
                         cls = getattr(
-                            sys.modules[data['module']], data['name']
+                            sys.modules[data["module"]], data["name"]
                         )
                         if isinstance(cls, type):
                             return cls
                         else:
                             raise ValueError("Decoded object is not a type")
                     else:
                         raise ValueError("Invalid module name")
-                elif obj['_type'] == 'dtype':
+                elif obj["_type"] == "dtype":
                     return pd.api.types.pandas_dtype(data)
-                elif obj['_type'] == 'slice':
+                elif obj["_type"] == "slice":
                     return slice(*data)
-                elif obj['_type'] == 'range':
-                    return range(data['start'], data['stop'], data['step'])
+                elif obj["_type"] == "range":
+                    return range(data["start"], data["stop"], data["step"])
             return {self.decode(k): self.decode_obj(v) for k, v in obj.items()}
         elif isinstance(obj, list):
             return [self.decode_obj(v) for v in obj]
         return obj
 
     @classmethod
     def decode_bytes(cls, b: bytes, *args: Any, **kwargs: Any) -> Any:
         decoder = cls()
-        return decoder.decode(b.decode('utf-8'), *args, **kwargs)
+        return decoder.decode(b.decode("utf-8"), *args, **kwargs)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/async_utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/async_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             queue.task_done()
             break
         queue.task_done()
         yield x
 
 
 def to_recordbatch(
-    output: t.Mapping[str, pa.Table]
+    output: t.Mapping[str, pa.Table],
 ) -> t.AsyncIterator[pa.RecordBatch]:
     """This function is inspired from arrow_recordbatch in
     sarus_data_spec/manager/ops/source/sql/arrow.py
     In order to create a recordbatch from different pyarrow tables, a struct is
     created where the corresponding other missing tables
     have been added as None"""
     struct_arrays = {
@@ -152,15 +152,15 @@
         ]
         fields = [
             pa.field(name=name, type=arr.type)
             for name, arr in zip(names, arrays_list)
         ]
         fields.append(
             pa.field(
-                name='field_selected', type=pa.large_string(), nullable=False
+                name="field_selected", type=pa.large_string(), nullable=False
             )
         )
         arrays_list.append(
             pa.array([current_table] * len(arr_array), type=pa.large_string())
         )
         batches.append(
             pa.RecordBatch.from_arrays(
@@ -191,31 +191,31 @@
     if isinstance(query, str):
         # we preserve the schema name of the parent
         queries = {parent_schema_name: query}
     else:
         if len(query) == 1:
             # we override the schema name
             queries = {
-                key if isinstance(key, str) else '.'.join(key): value
+                key if isinstance(key, str) else ".".join(key): value
                 for key, value in query.items()
             }
         else:
             # we override if prefix is the same otherwise we preserve
             prefixes = [
-                key.split('.')[0] if isinstance(key, str) else key[0]
+                key.split(".")[0] if isinstance(key, str) else key[0]
                 for key in list(query.keys())
             ]
             if len(prefixes) == len(set(prefixes)):
                 # all prefixes are the same, we preserve parents schema
                 queries = {
-                    f'{parent_schema_name}.{key}'
+                    f"{parent_schema_name}.{key}"
                     if isinstance(key, str)
-                    else '.'.join([parent_schema_name, *key]): value
+                    else ".".join([parent_schema_name, *key]): value
                     for key, value in query.items()
                 }
             else:
                 # we override parents schema
                 queries = {
-                    key if isinstance(key, str) else '.'.join(key): value
+                    key if isinstance(key, str) else ".".join(key): value
                     for key, value in query.items()
                 }
     return queries
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def __init__(
         self, storage: storage_typing.Storage, protobuf: sp.Manager
     ) -> None:
         self._protobuf: sp.Manager = copy(protobuf)
         self._freeze()
         self._storage = storage
         self.storage().store(self)
-        self._parquet_dir = os.path.expanduser('/tmp/sarus_dataset/')
+        self._parquet_dir = os.path.expanduser("/tmp/sarus_dataset/")
         os.makedirs(self.parquet_dir(), exist_ok=True)
         self._dataspec_rewriter = RecursiveDataspecRewriter(storage=storage)
         self._dataspec_validator = RecursiveDataspecValidator(storage=storage)
 
         # To define in subclasses
         self.to_arrow_computation: Computation[t.AsyncIterator[pa.RecordBatch]]
         self.to_parquet_computation: Computation[str]
@@ -131,21 +131,21 @@
     def _checksum(self) -> bytes:
         """Compute an md5 checksum"""
         md5 = hashlib.md5(usedforsecurity=False)
         md5.update(sp.serialize(self._protobuf))
         return md5.digest()
 
     def _freeze(self) -> None:
-        self._protobuf.uuid = ''
+        self._protobuf.uuid = ""
         self._frozen_checksum = self._checksum()
         self._protobuf.uuid = UUID(bytes=self._frozen_checksum).hex
 
     def _frozen(self) -> bool:
         uuid = self._protobuf.uuid
-        self._protobuf.uuid = ''
+        self._protobuf.uuid = ""
         result = (self._checksum() == self._frozen_checksum) and (
             uuid == UUID(bytes=self._frozen_checksum).hex
         )
         self._protobuf.uuid = uuid
         return result
 
     def uuid(self) -> str:
@@ -179,15 +179,15 @@
 
         if len(filtered_attributes) == 0:
             return None
 
         if len(filtered_attributes) == 1:
             return t.cast(st.Attribute, filtered_attributes[0])
 
-        raise ValueError('There are two attributes with the same name')
+        raise ValueError("There are two attributes with the same name")
 
     def attributes(
         self, name: str, dataspec: st.DataSpec
     ) -> t.List[st.Attribute]:
         attributes = t.cast(
             t.Set[st.Attribute],
             self.storage().referring(
@@ -205,27 +205,27 @@
         """Infer the transform output type : minimal type inference."""
 
         def attach_nothing(ds: st.DataSpec) -> None:
             return
 
         # Some internal transforms return a Scalar
         if transform.spec() in [
-            'protected_paths',
-            'automatic_user_settings',
-            'public_paths',
-            'automatic_budget',
-            'attribute_budget',
-            'sd_budget',
-            'sampling_ratios',
-            'derive_seed',
-            'relationship_spec',
-            'validated_user_type',
-            'error_estimation',
-            'fit_model',
-            'fit_model_dp',
+            "privacy_unit_tracking_paths",
+            "automatic_user_settings",
+            "public_paths",
+            "automatic_budget",
+            "attribute_budget",
+            "sd_budget",
+            "sampling_ratios",
+            "derive_seed",
+            "relationship_spec",
+            "validated_user_type",
+            "error_estimation",
+            "fit_model",
+            "fit_model_dp",
         ]:
             return sp.type_name(sp.Scalar), attach_nothing
 
         # Other internal transforms return a Dataset
         if not transform.is_external():
             return sp.type_name(sp.Dataset), attach_nothing
 
@@ -251,21 +251,21 @@
         status = self.status(dataset, task_name=BIG_DATA_TASK)
 
         if status is not None:
             # check if big_data_present
             big_data_task = status.task(BIG_DATA_TASK)
             # if yes:return answer
             if (big_data_task is not None) and (
-                big_data_task.stage() == 'ready'
+                big_data_task.stage() == "ready"
             ):
                 return big_data_task.properties()[IS_BIG_DATA] == str(True)
 
         if dataset.is_source():
             raise NotImplementedError(
-                'Found source dataset without any big data status'
+                "Found source dataset without any big data status"
             )
         else:
             if dataset.transform().is_external():
                 return False
             parents, named_parents = dataset.parents()
             parents_list = [
                 parent for parent in parents if isinstance(parent, st.DataSpec)
@@ -281,15 +281,15 @@
                 if element.type_name() == sp.type_name(sp.Dataset)
             ]
             for element in parents_dict.values():
                 if element.type_name() == sp.type_name(sp.Dataset):
                     ds_args.append(element)
             if len(ds_args) > 1:
                 raise NotImplementedError(
-                    'transforms with many dataspecs not supported yet'
+                    "transforms with many dataspecs not supported yet"
                 )
             if len(ds_args) == 0:
                 return False
             is_parent_big_data = self.is_big_data(ds_args[0])
 
             if not is_parent_big_data:
                 # write status it is not big data
@@ -321,17 +321,15 @@
                 # is put with the wrong manager
                 if status is None:
                     status = stt.last_status(
                         dataspec=ds_args[0], task=BIG_DATA_TASK
                     )
                 assert status
                 big_data_threshold = int(
-                    status.task(BIG_DATA_TASK).properties()[  # type:ignore
-                        BIG_DATA_THRESHOLD
-                    ]
+                    status.task(BIG_DATA_TASK).properties()[BIG_DATA_THRESHOLD]  # type:ignore
                 )
                 # write status
                 stt.ready(
                     dataset,
                     task=BIG_DATA_TASK,
                     properties={
                         IS_BIG_DATA: str(is_big_data),
@@ -792,46 +790,38 @@
     status = parent_dataset.manager().status(
         parent_dataset, task_name=BIG_DATA_TASK
     )
     if status is None:
         status = stt.last_status(parent_dataset, task=BIG_DATA_TASK)
     assert status
     big_data_threshold = int(
-        status.task(BIG_DATA_TASK).properties()[  # type:ignore
-            BIG_DATA_THRESHOLD
-        ]
+        status.task(BIG_DATA_TASK).properties()[BIG_DATA_THRESHOLD]  # type:ignore
     )
-    threshold_kind = status.task(BIG_DATA_TASK).properties()[  # type:ignore
-        THRESHOLD_TYPE
-    ]
+    threshold_kind = status.task(BIG_DATA_TASK).properties()[THRESHOLD_TYPE]  # type:ignore
 
-    parent_n_lines_str = status.task(
-        BIG_DATA_TASK
-    ).properties()[  # type:ignore
+    parent_n_lines_str = status.task(BIG_DATA_TASK).properties()[  # type:ignore
         DATASET_N_LINES
     ]
-    if parent_n_lines_str == '':
+    if parent_n_lines_str == "":
         parent_n_lines = 0
     else:
         parent_n_lines = int(parent_n_lines_str)
 
-    parent_bytes_str = status.task(BIG_DATA_TASK).properties()[  # type:ignore
-        DATASET_N_BYTES
-    ]
-    if parent_bytes_str == '':
+    parent_bytes_str = status.task(BIG_DATA_TASK).properties()[DATASET_N_BYTES]  # type:ignore
+    if parent_bytes_str == "":
         parent_bytes = 0
     else:
         parent_bytes = int(parent_bytes_str)
 
     transform_name = transform.name()
-    if transform_name in ('Sample', 'DifferentiatedSample'):
-        transform_type = transform.protobuf().spec.WhichOneof('spec')
+    if transform_name in ("Sample", "DifferentiatedSample"):
+        transform_type = transform.protobuf().spec.WhichOneof("spec")
         assert transform_type
         if getattr(transform.protobuf().spec, transform_type).HasField(
-            'fraction'
+            "fraction"
         ):
             fraction = getattr(
                 transform.protobuf().spec, transform_type
             ).fraction
             new_bytes = int(fraction * parent_bytes)
             n_lines = int(fraction * parent_n_lines)
 
@@ -849,20 +839,20 @@
             if threshold_kind == DATASET_N_BYTES:
                 big_data_threshold = int(1e5)
 
         threshold_kind = DATASET_N_LINES
 
         return n_lines > big_data_threshold, n_lines, new_bytes, threshold_kind
 
-    elif transform_name == 'filter':
+    elif transform_name == "filter":
         # TODO: we need to save the real sizes of a dataspec in the statuses
         # so that we can check what happens here
         return True, parent_n_lines, parent_bytes, threshold_kind
 
-    elif transform_name == 'Synthetic data':
+    elif transform_name == "Synthetic data":
         # here we should leverage the sampling ratio just to get the size,
         # in any case, synthetic data is never big data
 
         threshold_kind = DATASET_N_LINES
         synthetic_size = parent_dataset.size()
         assert synthetic_size is not None
 
@@ -880,17 +870,17 @@
         # TODO https://gitlab.com/sarus-tech/sarus-data-spec/-/issues/207
         return True, parent_n_lines, parent_bytes, threshold_kind
     # just for test
     elif transform_name == "ToSmallData":
         return (False, -1, -1, threshold_kind)
     else:
         # other transforms do not affect size
-        if transform_name == 'user_settings':
+        if transform_name == "user_settings":
             warnings.warn(
-                'user_settings transform considered to' 'not affect size'
+                "user_settings transform considered to" "not affect size"
             )
         return True, parent_n_lines, parent_bytes, threshold_kind
 
 
 async def write_tf_batch(
     filename: str,
     batch: pa.RecordBatch,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/cache_utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/cache_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     """
     if isinstance(result, (pd.DataFrame, pd.Series)):
         return result.copy()
     return result
 
 
 def lru_caching(
-    category: str = 'default', use_first_arg: bool = True
+    category: str = "default", use_first_arg: bool = True
 ) -> t.Callable:
     """
     Decorator that provides caching functionality for functions, with support
     for
     both asynchronous and synchronous functions.
 
     Args:
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class BaseComputation(Computation[T]):
     """General class that implements some
     methods of the protocol shared by all task
     computations"""
 
-    task_name = ''
+    task_name = ""
 
     def __init__(self, computing_manager: Base):
         self._computing_manager = computing_manager
 
     def computing_manager(self) -> Base:
         return self._computing_manager
 
@@ -62,26 +62,26 @@
         except stt.DataSpecErrorStatus as exception:
             stt.error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(exception.relaunch),
+                    "relaunch": str(exception.relaunch),
                 },
             )
             raise
         except Exception:
             stt.error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(False),
+                    "relaunch": str(False),
                 },
             )
             raise stt.DataSpecErrorStatus((False, traceback.format_exc()))
 
     async def result_from_stage_properties(
         self,
         dataspec: st.DataSpec,
@@ -173,15 +173,15 @@
             stage = status.task(self.task_name)
             assert stage
             if stage.processing() and PROCESSING_INFO in stage.properties():
                 max_info_length = 100
                 print(max_info_length * " ", end="\r")  # clear line
                 print(stage[PROCESSING_INFO][:max_info_length], end="\r")
             if stage.stage() == current_stage:
-                logger.info(f'POLLING {self.task_name} {dataspec.uuid()}')
+                logger.info(f"POLLING {self.task_name} {dataspec.uuid()}")
                 await asyncio.sleep(delay)
                 total_wait += delay
                 delay = min(2 * delay, max_delay, timeout - total_wait)
             else:
                 break
         assert stage
         return stage
@@ -229,25 +229,25 @@
         except stt.DataSpecErrorStatus as exception:
             stt.error(
                 dataspec=self.dataspec,
                 manager=self.computation.computing_manager(),
                 task=self.computation.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(exception.relaunch),
+                    "relaunch": str(exception.relaunch),
                 },
             )
             raise
         except Exception:
             stt.error(
                 dataspec=self.dataspec,
                 manager=self.computation.computing_manager(),
                 task=self.computation.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(False),
+                    "relaunch": str(False),
                 },
             )
             raise stt.DataSpecErrorStatus((False, traceback.format_exc()))
 
         else:
             return batch
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,27 @@
         """If processing, wait for the task to be ready.
         Such a case can happen if another manager has taken the computation
         of the task. After a given timeout, an error is raised.
         """
 
         stage = await self.wait_for_computation(
             dataspec=dataspec,
-            current_stage='processing',
+            current_stage="processing",
             timeout=self.computing_manager().computation_timeout(dataspec),
             max_delay=self.computing_manager().computation_max_delay(dataspec),
         )
         if stage.processing():
             stt.error(
                 dataspec=dataspec,
                 manager=dataspec.manager(),
                 task=self.task_name,
                 properties={
                     "message": "TimeOutError:Processing time out for task"
                     f" {self.task_name} on dataspec {dataspec}",
-                    'relaunch': str(True),
+                    "relaunch": str(True),
                 },
             )
             raise stt.DataSpecErrorStatus(
                 (
                     True,
                     "TimeOutError:Processing time out for task"
                     f" {self.task_name} on dataspec {dataspec}",
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/local/schema.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/local/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,63 +17,63 @@
 class SchemaComputation(LocalComputation[st.Schema]):
     """Class responsible to compute schemas"""
 
     task_name = SCHEMA_TASK
 
     async def prepare(self, dataspec: st.DataSpec) -> None:
         try:
-            logger.info(f'STARTED SCHEMA {dataspec.uuid()}')
+            logger.info(f"STARTED SCHEMA {dataspec.uuid()}")
             start = time.perf_counter()
             schema = await self.computing_manager().async_schema_op(
                 dataset=t.cast(Dataset, dataspec)
             )
 
         except DataSpecErrorStatus as exception:
             error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(exception.relaunch),
+                    "relaunch": str(exception.relaunch),
                 },
             )
             raise
         except Exception:
             error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": traceback.format_exc(),
-                    'relaunch': str(False),
+                    "relaunch": str(False),
                 },
             )
             raise DataSpecErrorStatus((False, traceback.format_exc()))
         else:
             end = time.perf_counter()
             logger.info(
-                f'FINISHED SCHEMA {dataspec.uuid()} ({end-start:.2f}s)'
+                f"FINISHED SCHEMA {dataspec.uuid()} ({end-start:.2f}s)"
             )
             ready(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
-                properties={'uuid': schema.uuid()},
+                properties={"uuid": schema.uuid()},
             )
 
     async def result_from_stage_properties(
         self,
         dataspec: st.DataSpec,
         properties: t.Mapping[str, str],
         **kwargs: t.Any,
     ) -> st.Schema:
         return t.cast(
             Schema,
-            dataspec.storage().referrable(properties['uuid']),
+            dataspec.storage().referrable(properties["uuid"]),
         )
 
     @lru_caching("computation", use_first_arg=True)
     async def task_result(
         self, dataspec: st.DataSpec, **kwargs: t.Any
     ) -> st.Schema:
         return await super().task_result(dataspec, **kwargs)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/computations/remote/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/computations/remote/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,30 +23,30 @@
     async def pending(self, dataspec: st.DataSpec) -> st.Status:
         """If the status of a task is pending, delegation has been
         already done, so the manager just waits for the task to
         be completed"""
 
         stage = await self.wait_for_computation(
             dataspec=dataspec,
-            current_stage='pending',
+            current_stage="pending",
             timeout=self.computing_manager().computation_timeout(dataspec),
             max_delay=self.computing_manager().computation_max_delay(dataspec),
         )
 
         if stage.pending():
             stt.error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": (
                         "TimeOutError: Pending time out for task"
                         f" {self.task_name} on dataspec {dataspec}"
                     ),
-                    'relaunch': str(True),
+                    "relaunch": str(True),
                 },
             )
             raise stt.DataSpecErrorStatus(
                 (
                     True,
                     "Pending time out for task"
                     f" {self.task_name} on dataspec {dataspec}",
@@ -59,30 +59,30 @@
         """If processing, wait for the task to be ready.
         Such a case can happen if another manager has taken the computation
         of the task. After a given timeout, an error is raised.
         """
 
         stage = await self.wait_for_computation(
             dataspec=dataspec,
-            current_stage='processing',
+            current_stage="processing",
             timeout=self.computing_manager().computation_timeout(dataspec),
             max_delay=self.computing_manager().computation_max_delay(dataspec),
         )
         if stage.processing() or stage.pending():
             # TODO push error status to worker ?
             stt.error(
                 dataspec=dataspec,
                 manager=self.computing_manager(),
                 task=self.task_name,
                 properties={
                     "message": (
                         "TimeOutError: Processing time out for task"
                         f" {self.task_name} on dataspec {dataspec}"
                     ),
-                    'relaunch': str(True),
+                    "relaunch": str(True),
                 },
             )
             raise stt.DataSpecErrorStatus(
                 (
                     True,
                     "Processing time out for task"
                     f" {self.task_name} on dataspec {dataspec}",
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/base.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import pyarrow as pa
 
 from sarus_data_spec.manager.async_utils import decoupled_async_iter
 import sarus_data_spec.dataspec_validator.typing as sdvt
 import sarus_data_spec.typing as st
 
 try:
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
 
 
 class DataspecStaticChecker:
     def __init__(self, dataspec: st.DataSpec):
@@ -22,42 +24,42 @@
 
     def is_dp_writable(self, public_context: t.Collection[str]) -> bool:
         """Statically check if a DP transform is applicable in this position.
 
         This verification is common to all dataspecs and is true if:
             - the dataspec is transformed and its transform has an equivalent
             DP transform
-            - the DP transform's required PEP arguments are PEP and aligned
-            (i.e. same PEP token)
+            - the DP transform's required PUP arguments are PUP and aligned
+            (i.e. same PUP token)
             - other dataspecs arguments are public
         """
         return False
 
     def is_dp(self) -> bool:
         """Checks if the transform is DP and compatible with the arguments."""
         return False
 
     def is_dp_able(self) -> bool:
         """Checks if the dataspec has a transform that either has a DP
         equivalent, allowing the rewritten dataspec to be considered DP
-        if the input rewritten PEP token is not None."""
+        if the input rewritten PUP token is not None."""
         return False
 
-    def is_pep_able(self) -> bool:
-        """Checks if the dataspec has a transform that either has a PEP
+    def is_pup_able(self) -> bool:
+        """Checks if the dataspec has a transform that either has a PUP
         equivalent or does not require one, allowing the rewritten dataspec to
-        be considered 'PEP' if the input rewritten PEP token is not None."""
+        be considered 'PUP' if the input rewritten PUP token is not None."""
         return False
 
     def dp_transform(self) -> t.Optional[st.Transform]:
         """Return the dataspec's DP equivalent transform if existing."""
         return None
 
-    def pep_transform(self) -> t.Optional[st.Transform]:
-        """Return the dataspec's PEP equivalent transform if existing."""
+    def pup_transform(self) -> t.Optional[st.Transform]:
+        """Return the dataspec's PUP equivalent transform if existing."""
         return None
 
     def dp_equivalent(self) -> t.Optional[st.Transform]:
         """Return the dataspec's DP equivalent transform if existing."""
         raise NotImplementedError
 
     async def private_queries(self) -> t.List[st.PrivateQuery]:
@@ -76,24 +78,24 @@
         super().__init__(dataset)
         self.dataset = dataset
 
     async def schema(self) -> st.Schema:
         """Computes the schema of the dataspec"""
         raise NotImplementedError
 
-    def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        """Return a token if the output is PEP."""
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        """Return a token if the output is PUP."""
         raise NotImplementedError
 
-    def rewritten_pep_token(
+    def rewritten_pup_token(
         self, public_context: t.Collection[str]
     ) -> t.Optional[str]:
         raise NotImplementedError
 
-    def pep_kind(self) -> sdvt.PEPKind:
+    def pup_kind(self) -> sdvt.PUPKind:
         raise NotImplementedError
 
 
 class DatasetImplementation:
     def __init__(self, dataset: st.Dataset):
         self.dataset = dataset
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/__init__.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,32 +62,32 @@
     return ops_mapping
 
 
 def replace_none(x: Optional[str]) -> str:
     return x if x else ""
 
 
-_INITIALIZED = globals().get('_INITIALIZED', False)
+_INITIALIZED = globals().get("_INITIALIZED", False)
 
 if not _INITIALIZED:
     ROUTING = {
         module_name: ops_mapping(module_name) for module_name in MODULES
     }
 
-    # These are lists of PEP and DP transforms. They are mappings {OP_ID:
+    # These are lists of PUP and DP transforms. They are mappings {OP_ID:
     # DOCSTRING}. The docstrings are displayed in the documentation to explain
-    # under which condition the op is PEP or DP.
+    # under which condition the op is PUP or DP.
 
     ALL_OPS: List[ExternalOpImplementation] = sum(
         [valid_ops(module_name) for module_name in MODULES], []
     )
-    PEP_TRANSFORMS = {
-        op.transform_id(): replace_none(op.pep_kind.__doc__)
+    PUP_TRANSFORMS = {
+        op.transform_id(): replace_none(op.pup_kind.__doc__)
         for op in ALL_OPS
-        if op.pep_kind.__doc__ != ExternalOpImplementation.pep_kind.__doc__
+        if op.pup_kind.__doc__ != ExternalOpImplementation.pup_kind.__doc__
     }
 
     DP_TRANSFORMS = {
         op.transform_id(): replace_none(
             cast(ExternalOpImplementation, op.dp_equivalent()).is_dp.__doc__
         )
         for op in ALL_OPS
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/external_op.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/external_op.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sarus_data_spec.constants import MAX_MAX_MULT, MULTIPLICITY
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusSignature,
     SarusSignatureValue,
 )
-from sarus_data_spec.dataspec_validator.typing import PEPKind
+from sarus_data_spec.dataspec_validator.typing import PUPKind
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.manager.ops.base import (
     DatasetImplementation,
     DatasetStaticChecker,
     DataspecStaticChecker,
     ScalarImplementation,
 )
@@ -36,20 +36,22 @@
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 from .typing import NO_TRANSFORM_ID
 from .utils import static_arguments
 
 try:
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
 
-DEFAULT_MAX_MAX_MULT = '1000.0'
+DEFAULT_MAX_MAX_MULT = "1000.0"
 
 
 class ExternalScalarStaticChecker(DataspecStaticChecker):
     async def private_queries(self) -> t.List[st.PrivateQuery]:
         """Return the PrivateQueries summarizing DP characteristics."""
         implementation = external_implementation(self.dataspec.transform())
         bound_signature = implementation.signature().bind_dataspec(
@@ -64,15 +66,15 @@
             self.dataspec
         )
         return implementation.is_dp(bound_signature)
 
     def is_dp_able(self) -> bool:
         """Checks if the dataspec has a transform that either has a DP
         equivalent, allowing the rewritten dataspec to be considered DP
-        if the input rewritten PEP token is not None."""
+        if the input rewritten PUP token is not None."""
         if self.is_dp():
             return True
 
         transform = self.dataspec.transform()
         implementation = external_implementation(transform)
         dp_implementation = implementation.dp_equivalent()
         if dp_implementation is None:
@@ -85,30 +87,30 @@
 
     def is_dp_writable(self, public_context: t.Collection[str]) -> bool:
         """Statically check if a DP transform is applicable in this position.
 
         This verification is common to all dataspecs and is true if:
             - the dataspec is transformed and its transform has an equivalent
             DP transform
-            - the DP transform's required PEP arguments are PEP and aligned
-            (i.e. same PEP token)
+            - the DP transform's required PUP arguments are PUP and aligned
+            (i.e. same PUP token)
             - other dataspecs arguments are public
         """
         transform = self.dataspec.transform()
         implementation = external_implementation(transform)
         dp_implementation = implementation.dp_equivalent()
         if dp_implementation is None:
             return False
         bound_signature = implementation.signature().bind_dataspec(
             self.dataspec
         )
         if not dp_implementation.is_dp(bound_signature):
             return False
 
-        return bound_signature.rewritten_pep_token() is not None
+        return bound_signature.rewritten_pup_token() is not None
 
     def dp_transform(self) -> t.Optional[st.Transform]:
         """Return the dataspec's DP equivalent transform if existing."""
         transform = self.dataspec.transform()
         op_implementation = external_implementation(transform)
         py_args, py_kwargs, ds_args_pos, ds_types = static_arguments(transform)
 
@@ -127,21 +129,21 @@
             dp_transform_id,
             py_args=py_args,
             py_kwargs=py_kwargs,
             ds_args_pos=ds_args_pos,
             ds_types=ds_types,
         )
 
-    def pep_transform(self) -> t.Optional[st.Transform]:
+    def pup_transform(self) -> t.Optional[st.Transform]:
         transform = self.dataspec.transform()
-        pep_implementation = pep_external_implementation(self.dataspec)
-        if pep_implementation is None:
+        pup_implementation = pup_external_implementation(self.dataspec)
+        if pup_implementation is None:
             return None
         py_args, py_kwargs, ds_args_pos, ds_types = static_arguments(transform)
-        dp_transform_id = pep_implementation.transform_id()
+        dp_transform_id = pup_implementation.transform_id()
         assert dp_transform_id is not None
         return external(
             dp_transform_id,
             py_args=py_args,
             py_kwargs=py_kwargs,
             ds_args_pos=ds_args_pos,
             ds_types=ds_types,
@@ -170,79 +172,79 @@
 class ExternalDatasetStaticChecker(
     ExternalScalarStaticChecker, DatasetStaticChecker
 ):
     def __init__(self, dataset: st.Dataset):
         super().__init__(dataset)
         self.dataset = dataset
 
-    def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        """Return the dataspec's PEP token."""
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        """Return the dataspec's PUP token."""
         transform = self.dataspec.transform()
         implementation = external_implementation(transform)
         bound_signature = implementation.signature().bind_dataspec(
             self.dataspec
         )
 
-        input_token = bound_signature.pep_token()
+        input_token = bound_signature.pup_token()
         if input_token is None:
             return None
 
-        pep_kind = implementation.pep_kind(bound_signature)
-        if pep_kind == PEPKind.NOT_PEP:
+        pup_kind = implementation.pup_kind(bound_signature)
+        if pup_kind == PUPKind.NOT_PUP:
             return None
-        elif pep_kind == PEPKind.TOKEN_PRESERVING:
+        elif pup_kind == PUPKind.TOKEN_PRESERVING:
             return input_token
-        else:  # PEP or ROW
+        else:  # PUP or ROW
             h = hashlib.md5(usedforsecurity=False)
             h.update(input_token.encode("ascii"))
             h.update(transform.protobuf().SerializeToString())
             new_token = h.hexdigest()
             return new_token
 
-    def rewritten_pep_token(
+    def rewritten_pup_token(
         self, public_context: t.Collection[str]
     ) -> t.Optional[str]:
         transform = self.dataspec.transform()
-        implementation = pep_external_implementation(self.dataspec)
+        implementation = pup_external_implementation(self.dataspec)
         if implementation is None:
             return None
         bound_signature = implementation.signature().bind_dataspec(
             self.dataspec
         )
 
-        input_token = bound_signature.rewritten_pep_token()
+        input_token = bound_signature.rewritten_pup_token()
         if input_token is None:
             return None
 
-        pep_kind = implementation.pep_kind(bound_signature)
-        if pep_kind == PEPKind.NOT_PEP:
+        pup_kind = implementation.pup_kind(bound_signature)
+        if pup_kind == PUPKind.NOT_PUP:
             return None
-        elif pep_kind == PEPKind.TOKEN_PRESERVING:
+        elif pup_kind == PUPKind.TOKEN_PRESERVING:
             return input_token
-        else:  # PEP or ROW
+        else:  # PUP or ROW
             h = hashlib.md5(usedforsecurity=False)
             h.update(input_token.encode("ascii"))
             h.update(transform.protobuf().SerializeToString())
             new_token = h.hexdigest()
             return new_token
 
-    def is_pep_able(self) -> bool:
-        """Checks if the dataspec has a transform that either has a PEP
+    def is_pup_able(self) -> bool:
+        """Checks if the dataspec has a transform that either has a PUP
         equivalent or does not require one, allowing the rewritten dataspec to
-        be considered 'PEP' if the input rewritten PEP token is not None."""
-        implementation = pep_external_implementation(self.dataspec)
+        be considered 'PUP' if the input rewritten PUP token is not None."""
+        implementation = pup_external_implementation(self.dataspec)
         if implementation is None:
             return False
         # probably not needed
         bound_signature = implementation.signature().bind_dataspec(
             self.dataspec
         )
 
-        pep_kind = implementation.pep_kind(bound_signature)
-        return not pep_kind == PEPKind.NOT_PEP
+        pup_kind = implementation.pup_kind(bound_signature)
+        return not pup_kind == PUPKind.NOT_PUP
 
     async def schema(self) -> st.Schema:
         """Computes the schema of the dataspec.
 
         The schema is computed by computing the synthetic data value and
         converting the Pyarrow schema to a Sarus schema.q
         """
@@ -257,54 +259,54 @@
 
         schema_type = type_from_arrow_schema(schema)
         # retrieve max_mul from parent
         parents_args, parents_kwargs = self.dataset.parents()
         parents_args.extend(parents_kwargs.values())
         parents_args = [el for el in parents_args if isinstance(el, Dataset)]
         if len(parents_args) > 1 or len(parents_args) == 0:
-            max_mult = ''  # we cannot infer max_mult in this case
+            max_mult = ""  # we cannot infer max_mult in this case
             max_max_mult = DEFAULT_MAX_MAX_MULT
         else:
             parent_ds = t.cast(st.Dataset, parents_args[0])
             parent_schema = await self.dataset.manager().async_schema(
                 parent_ds
             )
             max_mult = await retrieve_max_mult_info_from_parent(
                 parent_ds=parent_ds, parent_schema=parent_schema
             )
             max_max_mult = parent_schema.properties().get(
                 MAX_MAX_MULT, DEFAULT_MAX_MAX_MULT
             )
         properties = {}
-        if self.dataset.is_pep():
-            # If the dataset is PEP then the schema of the real data should
+        if self.dataset.is_pup():
+            # If the dataset is PUP then the schema of the real data should
             # have protection but the synthetic data might not have it. We
             # need to add it manually.
             schema_type = sdt.protected_type(schema_type)
             # now take care of multiplicity
             implementation = external_implementation(self.dataset.transform())
             bound_signature = implementation.signature().bind_dataspec(
                 self.dataset
             )
-            pep_kind = implementation.pep_kind(bound_signature)
-            if pep_kind == PEPKind.TOKEN_PRESERVING:
-                if max_mult != '':
+            pup_kind = implementation.pup_kind(bound_signature)
+            if pup_kind == PUPKind.TOKEN_PRESERVING:
+                if max_mult != "":
                     properties[MULTIPLICITY] = max_mult
                     properties[MAX_MAX_MULT] = max_mult
                 else:
                     properties[MAX_MAX_MULT] = max_max_mult
 
             else:
                 # in this case, rows are not preserved,
                 # so the max multiplicity might change,
                 # we take as bound the older one, this is
                 # an approximation and may cause bias
                 # if the dataset rows increase
                 properties = {
-                    MAX_MAX_MULT: max_mult if max_mult != '' else max_max_mult
+                    MAX_MAX_MULT: max_mult if max_mult != "" else max_max_mult
                 }
         else:
             properties = {}
         return schema_builder(
             self.dataset, schema_type=schema_type, properties=properties
         )
 
@@ -316,19 +318,19 @@
         transform = self.dataset.transform()
         implementation = external_implementation(transform)
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
         bound_signature.static_validation()
 
-        if self.dataset.is_pep():
+        if self.dataset.is_pup():
             result = await implementation.compute(bound_signature)
             if (
                 isinstance(result, pd.Series)
-                and implementation.pep_kind(bound_signature) == PEPKind.ROW
+                and implementation.pup_kind(bound_signature) == PUPKind.ROW
             ):
                 # Reformat the series as a dataframe with a single row
                 result = result.to_frame().transpose()
 
             ds_result = t.cast(st.DatasetCastable, result)
             admin_data = await bound_signature.admin_data()
             output_admin_data = compute_admin_data(admin_data, ds_result)
@@ -343,38 +345,37 @@
         return async_iter(table.to_batches(max_chunksize=batch_size))
 
     async def size(self) -> st.Size:
         implementation = external_implementation(self.dataset.transform())
         bound_signature = implementation.signature().bind_dataspec(
             self.dataset
         )
-        pep_kind = implementation.pep_kind(bound_signature)
-        if pep_kind == PEPKind.TOKEN_PRESERVING:
-
+        pup_kind = implementation.pup_kind(bound_signature)
+        if pup_kind == PUPKind.TOKEN_PRESERVING:
             parents_args, parents_kwargs = self.dataset.parents()
             parents_args.extend(parents_kwargs.values())
             parents_args = [
                 el for el in parents_args if isinstance(el, Dataset)
             ]
             assert len(parents_args) == 1
             parent_ds = t.cast(st.Dataset, parents_args[0])
             sizes = await self.dataset.manager().async_size(parent_ds)
             return size_builder(
                 dataset=self.dataset, statistics=sizes.statistics()
             )
-        elif pep_kind == PEPKind.PEP:
+        elif pup_kind == PUPKind.PUP:
             syn_variant = self.dataset.variant(
                 kind=st.ConstraintKind.SYNTHETIC
             )
             assert syn_variant is not None
             syn_variant = t.cast(Dataset, syn_variant)
             import warnings
 
             warnings.warn(
-                'Using hack to compute sizes of dataset with synthetic variant'
+                "Using hack to compute sizes of dataset with synthetic variant"
             )
             size = len(
                 await syn_variant.manager().async_to_pandas(syn_variant)
             )
             return size_builder(
                 dataset=self.dataset,
                 statistics=sds.Struct(fields={}, multiplicity=1.0, size=size),
@@ -414,27 +415,27 @@
     )
     bound_signature.static_validation()
     data = await implementation.compute(bound_signature)
     return data
 
 
 class ExternalOpImplementation:
-    """External PEP op implementation class.
+    """External PUP op implementation class.
 
     This class wraps together several elements of an external op
     implementation:
         - `call` is the function that computes the output value from the
           input(s) value(s).
     """
 
     _transform_id: str = NO_TRANSFORM_ID
     _dp_equivalent_id: t.Optional[str] = None
     _non_dp_equivalent_id: t.Optional[str] = None
-    _pep_equivalent_id: t.Optional[str] = None
-    _non_pep_equivalent_id: t.Optional[str] = None
+    _pup_equivalent_id: t.Optional[str] = None
+    _non_pup_equivalent_id: t.Optional[str] = None
     _signature: t.Optional[SarusSignature] = None
 
     def transform_id(self) -> str:
         return self._transform_id
 
     def dp_equivalent_id(self) -> t.Optional[str]:
         return self._dp_equivalent_id
@@ -444,19 +445,19 @@
 
     def dp_equivalent(self) -> t.Optional[ExternalOpImplementation]:
         if not self._dp_equivalent_id:
             return None
 
         return external_implementation_from_id(self._dp_equivalent_id)
 
-    def pep_equivalent(self) -> t.Optional[ExternalOpImplementation]:
-        if not self._pep_equivalent_id:
+    def pup_equivalent(self) -> t.Optional[ExternalOpImplementation]:
+        if not self._pup_equivalent_id:
             return None
 
-        return external_implementation_from_id(self._pep_equivalent_id)
+        return external_implementation_from_id(self._pup_equivalent_id)
 
     def signature(self) -> SarusSignature:
         if self._signature is not None:
             return self._signature
 
         if self._non_dp_equivalent_id is None:
             raise ValueError(
@@ -479,24 +480,24 @@
     def call(self, signature_value: SarusSignatureValue) -> t.Any:
         raise NotImplementedError
 
     async def call_dp(self, bound_signature: SarusBoundSignature) -> t.Any:
         """DP ops `call` need to be async to compute schema, tasks, etc"""
         raise NotImplementedError
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        """Return the PEP properties of the transform.
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        """Return the PUP properties of the transform.
 
         It takes the transform arguments as input because it can depend on some
-        transform parameters. For instance, it is not PEP if we are aggregating
-        the rows (axis=0) and it is PEP if we are aggregating the columns
+        transform parameters. For instance, it is not PUP if we are aggregating
+        the rows (axis=0) and it is PUP if we are aggregating the columns
         (axis=1).
         """
         # Default implementation
-        return PEPKind.NOT_PEP
+        return PUPKind.NOT_PUP
 
     def is_dp(self, bound_signature: SarusBoundSignature) -> bool:
         """Return True if the DP transform is compatible with the arguments.
 
         It takes the transform arguments as input because it can depend on some
         transform parameters. For instance, if we are aggregating the rows
         (axis=0), then there might be an equivalent DP transform but if we are
@@ -554,33 +555,33 @@
     The mapping is done by the config file.
     """
     assert transform and transform.is_external()
     id = transform_id(transform)
     return external_implementation_from_id(id)
 
 
-def pep_external_implementation(
+def pup_external_implementation(
     dataspec: st.DataSpec,
 ) -> t.Optional[ExternalOpImplementation]:
     transform = dataspec.transform()
     implementation = external_implementation(transform)
     bound_signature = implementation.signature().bind_dataspec(dataspec)
-    pep_kind = implementation.pep_kind(bound_signature)
-    if not pep_kind == PEPKind.NOT_PEP:
+    pup_kind = implementation.pup_kind(bound_signature)
+    if not pup_kind == PUPKind.NOT_PUP:
         return implementation
     else:
-        pep_implementation = implementation.pep_equivalent()
-        if pep_implementation is None:
+        pup_implementation = implementation.pup_equivalent()
+        if pup_implementation is None:
             return None
         else:
-            pep_kind = pep_implementation.pep_kind(bound_signature)
-            if pep_kind == PEPKind.NOT_PEP:
+            pup_kind = pup_implementation.pup_kind(bound_signature)
+            if pup_kind == PUPKind.NOT_PUP:
                 return None
             else:
-                return pep_implementation
+                return pup_implementation
 
 
 def external_implementation_from_id(id: str) -> ExternalOpImplementation:
     # Imported here to avoid circular imports
     from . import ROUTING
 
     library, op_name = id.split(".")
@@ -593,21 +594,21 @@
 async def retrieve_max_mult_info_from_parent(
     parent_ds: st.Dataset, parent_schema: st.Schema
 ) -> str:
     """If the dataset is transformed by an external the max_mult
     lies in the schema while for standard transforms we can derive
      the multiplicity from the parent directly"""
     if not parent_ds.is_transformed():
-        return ''
+        return ""
     if parent_ds.transform().is_external():
-        max_mult = parent_schema.properties().get(MULTIPLICITY, '')
+        max_mult = parent_schema.properties().get(MULTIPLICITY, "")
     else:
         try:
             max_mult = str(
                 (await parent_ds.manager().async_multiplicity(parent_ds))
                 .statistics()
                 .multiplicity()
             )
         except Exception:
             # this is for the mock, not very nice
-            max_mult = ''
+            max_mult = ""
     return max_mult
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/imblearn.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/imblearn.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 try:
     from imblearn import over_sampling, pipeline, under_sampling
 except ModuleNotFoundError:
     pass  # error message in typing.py
 
 SamplingStrategy = Literal[
-    'majority', 'not minority', 'not majority', 'all', 'auto'
+    "majority", "not minority", "not majority", "all", "auto"
 ]
 
 
 # ------ CONSTRUCTORS ------
 class imb_pipeline(ExternalOpImplementation):
     _transform_id = "imblearn.IMB_PIPELINE"
     _signature = SarusSignature(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/numpy.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/numpy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/optbinning.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/optbinning.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,22 +579,22 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         df = this.build(**kwargs)
         # small edit of the result to convert it in arrow
-        if kwargs['add_totals']:
+        if kwargs["add_totals"]:
             df["WoE"]["Totals"] = 0.0
-            df['WoE'] = df['WoE'].astype(float)
+            df["WoE"] = df["WoE"].astype(float)
             df_reset = df.reset_index()
-            df_reset['index'] = df_reset['index'].astype(
+            df_reset["index"] = df_reset["index"].astype(
                 str
             )  # Replace str with the desired type
-            df_reset = df_reset.set_index('index')
+            df_reset = df_reset.set_index("index")
         return df_reset
 
 
 class scorecard(ExternalOpImplementation):
     _transform_id = "optbinning.SCORECARD"
     _signature = SarusSignature(
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     List,
     Literal,
     Optional,
     Union,
 )
 
 from pandas._libs.tslibs import BaseOffset
-from pandas.core.window.indexers import BaseIndexer
+from pandas.api.indexers import BaseIndexer
 import pandas as pd
 import pandas._typing as pdt
 
 from sarus_data_spec.dataspec_validator.parameter_kind import DATASPEC
 from sarus_data_spec.dataspec_validator.signature import (
     SarusParameter,
     SarusSignature,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/groupby_dp.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,60 +20,82 @@
     pd.core.groupby.DataFrameGroupBy,
     pd.core.groupby.SeriesGroupBy,
 ]
 
 logger = logging.getLogger(__name__)
 
 try:
-    from sarus_statistics.ops.bounds.op import BoundOp
-    from sarus_statistics.ops.histograms.op import GroupByCountOp
-    from sarus_statistics.ops.max_multiplicity.op import MaxMultiplicityOp
-    from sarus_statistics.ops.mean.op import GroupByMeanOp
-    from sarus_statistics.ops.median.op import GroupbyMedianOp
-    from sarus_statistics.ops.std.op import GroupByStdOp
-    from sarus_statistics.ops.sum.op import GroupBySumOp
-    from sarus_statistics.ops.tau_thresholding.op import TauThresholdingOp
-except ModuleNotFoundError as e_groupby_dp:
-    if "sarus_statistics" not in str(e_groupby_dp):
-        raise
+    from sarus_data_spec.sarus_statistics.ops.bounds.op import BoundOp
+    from sarus_data_spec.sarus_statistics.ops.histograms.op import (
+        GroupByCountOp,
+    )
+    from sarus_data_spec.sarus_statistics.ops.max_multiplicity.op import (
+        MaxMultiplicityOp,
+    )
+    from sarus_data_spec.sarus_statistics.ops.mean.op import GroupByMeanOp
+    from sarus_data_spec.sarus_statistics.ops.median.op import GroupbyMedianOp
+    from sarus_data_spec.sarus_statistics.ops.std.op import GroupByStdOp
+    from sarus_data_spec.sarus_statistics.ops.sum.op import GroupBySumOp
+    from sarus_data_spec.sarus_statistics.ops.tau_thresholding.op import (
+        TauThresholdingOp,
+    )
+except ModuleNotFoundError:
+    pass
+    # TODO properly: from sarus_data_spec.sarus_statistics.ops.bounds.op
+    # imports sarus_differential_privacy
+    # if "sarus_data_spec.sarus_statistics" not in str(e_pandas_dp):
+    #     raise
 
 try:
     from sarus_differential_privacy.query import ComposedPrivateQuery
-except ModuleNotFoundError as e_groupby_dp:
-    if "sarus_differential_privacy" not in str(e_groupby_dp):
+except ModuleNotFoundError as e_pandas_dp:
+    if "sarus_differential_privacy" not in str(e_pandas_dp):
         raise
 
 try:
-    from sarus_query_builder.builders.bounds_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.bounds_builder import (
         simple_bounds_builder,
     )
-    from sarus_query_builder.builders.composed_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.composed_builder import (
         simple_composed_builder,
     )
-    from sarus_query_builder.builders.max_multiplicity_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.max_multiplicity_builder import (  # noqa : E501
         simple_max_multiplicity_builder,
     )
-    from sarus_query_builder.builders.mean_builder import mean_builder
-    from sarus_query_builder.builders.median_builder import median_builder
-    from sarus_query_builder.builders.standard_mechanisms_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.mean_builder import (
+        mean_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.median_builder import (
+        median_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.standard_mechanisms_builder import (  # noqa : E501
         laplace_builder,
     )
-    from sarus_query_builder.builders.std_builder import std_builder
-    from sarus_query_builder.builders.sum_builder import sum_builder
-    from sarus_query_builder.builders.tau_thresholding_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.std_builder import (
+        std_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.sum_builder import (
+        sum_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.tau_thresholding_builder import (  # noqa : E501
         tau_threshold_builder_delta,
     )
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
-    from sarus_query_builder.protobuf.query_pb2 import GenericTask, Query
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
+    from sarus_data_spec.sarus_query_builder.protobuf.query_pb2 import (
+        GenericTask,
+        Query,
+    )
 except ModuleNotFoundError as e_groupby_dp:
     if "sarus" not in str(e_groupby_dp):
         raise
     OptimizableQueryBuilder = t.Any  # type: ignore
 
-NUMERIC_TYPES = ('integer', 'float', 'boolean')
+NUMERIC_TYPES = ("integer", "float", "boolean")
 
 DEFAULT_DELTA = 0.01
 
 
 def has_budget(signature: SarusBoundSignature) -> bool:
     """Retrieve (epsilon, delta) from signature"""
     return "budget" in signature
@@ -189,25 +211,25 @@
         # keys_values = [key for key,_ in dataframegroupby_synth]
 
         # keys values from tau thresholding
         # work with only one index name for the group by
         keys_name = dataframegroupby.keys
         dataset_above_tau_threshold = TauThresholdingOp(
             parent_ds,
-            tau_thresholding_task.parameters['epsilon_tau_thresholding'],
-            tau_thresholding_task.parameters['delta_tau_thresholding'],
+            tau_thresholding_task.parameters["epsilon_tau_thresholding"],
+            tau_thresholding_task.parameters["delta_tau_thresholding"],
         ).value(keys_name, max_mul, random_generator)
         keys_values = list(dataset_above_tau_threshold.index)
 
         dataframes_with_counts = {}
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             count_parameters = shape_task[index]
             dataframes_with_counts[column_name] = GroupByCountOp(
                 parent_ds,
-                count_parameters.parameters['noise'],
+                count_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator, keys_values)
 
         if len(dataframes_with_counts.keys()) == 1:
             return list(dataframes_with_counts.values())[0]
         else:
             for col_name, df in dataframes_with_counts.items():
                 df.columns = [col_name]
@@ -318,47 +340,48 @@
         else:
             max_mul = 1
 
         keys_name = dataframegroupby.keys
 
         dataset_above_tau_threshold = TauThresholdingOp(
             parent_ds,
-            tau_thresholding_task.parameters['epsilon_tau_thresholding'],
-            tau_thresholding_task.parameters['delta_tau_thresholding'],
+            tau_thresholding_task.parameters["epsilon_tau_thresholding"],
+            tau_thresholding_task.parameters["delta_tau_thresholding"],
         ).value(keys_name, max_mul, random_generator)
         keys_values = list(dataset_above_tau_threshold.index)
 
         dataframes_with_dp_means = {}
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             subtasks = [unwrap(task) for task in mean_tasks[index].subtasks]
 
-            bounds_parameters, mean_parameters = t.cast(
-                GenericTask, subtasks[0]
-            ), t.cast(GenericTask, subtasks[1])
+            bounds_parameters, mean_parameters = (
+                t.cast(GenericTask, subtasks[0]),
+                t.cast(GenericTask, subtasks[1]),
+            )
             column_type = (
                 parent_ds.schema()
                 .data_type()
                 .children()[column_name]
                 .protobuf()
             )
-            if column_type.WhichOneof('type') == 'optional':
+            if column_type.WhichOneof("type") == "optional":
                 dataframes_with_dp_means[column_name] = dataframegroupby.apply(
                     lambda x: np.nan
                 ).to_frame(name="Mean")
                 continue
-            if column_type.WhichOneof('type') not in NUMERIC_TYPES:
+            if column_type.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             mean_op = GroupByMeanOp(
                 parent_ds,
-                mean_parameters.parameters['noise'],
+                mean_parameters.parameters["noise"],
             )
             dataframes_with_dp_means[column_name] = mean_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
         if len(dataframes_with_dp_means.keys()) == 1:
             return list(dataframes_with_dp_means.values())[0]
@@ -472,48 +495,49 @@
         else:
             max_mul = 1
 
         keys_name = dataframegroupby.keys
 
         dataset_above_tau_threshold = TauThresholdingOp(
             parent_ds,
-            tau_thresholding_task.parameters['epsilon_tau_thresholding'],
-            tau_thresholding_task.parameters['delta_tau_thresholding'],
+            tau_thresholding_task.parameters["epsilon_tau_thresholding"],
+            tau_thresholding_task.parameters["delta_tau_thresholding"],
         ).value(keys_name, max_mul, random_generator)
         keys_values = list(dataset_above_tau_threshold.index)
 
         dataframes_with_dp_median = {}
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             subtasks = [unwrap(task) for task in median_tasks[index].subtasks]
-            bounds_parameters, median_parameters = t.cast(
-                GenericTask, subtasks[0]
-            ), t.cast(GenericTask, subtasks[1])
+            bounds_parameters, median_parameters = (
+                t.cast(GenericTask, subtasks[0]),
+                t.cast(GenericTask, subtasks[1]),
+            )
             column_type = (
                 parent_ds.schema()
                 .data_type()
                 .children()[column_name]
                 .protobuf()
             )
-            if column_type.WhichOneof('type') == 'optional':
-                dataframes_with_dp_median[
-                    column_name
-                ] = dataframegroupby.apply(lambda x: np.nan).to_frame(
-                    name="Median"
+            if column_type.WhichOneof("type") == "optional":
+                dataframes_with_dp_median[column_name] = (
+                    dataframegroupby.apply(
+                        lambda x: np.nan
+                    ).to_frame(name="Median")
                 )
                 continue
-            if column_type.WhichOneof('type') not in NUMERIC_TYPES:
+            if column_type.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             median_op = GroupbyMedianOp(
                 parent_ds,
-                median_parameters.parameters['noise'],
+                median_parameters.parameters["noise"],
             )
             dataframes_with_dp_median[column_name] = median_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
         if len(dataframes_with_dp_median.keys()) == 1:
             return list(dataframes_with_dp_median.values())[0]
@@ -626,48 +650,49 @@
             ).value(random_generator)
         else:
             max_mul = 1
 
         keys_name = dataframegroupby.keys
         dataset_above_tau_threshold = TauThresholdingOp(
             parent_ds,
-            tau_thresholding_task.parameters['epsilon_tau_thresholding'],
-            tau_thresholding_task.parameters['delta_tau_thresholding'],
+            tau_thresholding_task.parameters["epsilon_tau_thresholding"],
+            tau_thresholding_task.parameters["delta_tau_thresholding"],
         ).value(keys_name, max_mul, random_generator)
         keys_values = list(dataset_above_tau_threshold.index)
 
         dataframes_with_dp_std = {}
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             subtasks = [unwrap(task) for task in std_tasks[index].subtasks]
-            bounds_parameters, std_parameters = t.cast(
-                GenericTask, subtasks[0]
-            ), t.cast(GenericTask, subtasks[1])
+            bounds_parameters, std_parameters = (
+                t.cast(GenericTask, subtasks[0]),
+                t.cast(GenericTask, subtasks[1]),
+            )
             column_type = (
                 parent_ds.schema()
                 .data_type()
                 .children()[column_name]
                 .protobuf()
             )
-            if column_type.WhichOneof('type') == 'optional':
+            if column_type.WhichOneof("type") == "optional":
                 dataframes_with_dp_std[column_name] = dataframegroupby.apply(
                     lambda x: np.nan
                 ).to_frame(name="Std")
                 continue
-            if column_type.WhichOneof('type') not in NUMERIC_TYPES:
+            if column_type.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             std_op = GroupByStdOp(
                 parent_ds,
-                std_parameters.parameters['noise_mean'],
-                std_parameters.parameters['noise_square'],
-                std_parameters.parameters['noise_count'],
+                std_parameters.parameters["noise_mean"],
+                std_parameters.parameters["noise_square"],
+                std_parameters.parameters["noise_count"],
             )
             dataframes_with_dp_std[column_name] = std_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
         if len(dataframes_with_dp_std.keys()) == 1:
             return list(dataframes_with_dp_std.values())[0]
@@ -781,46 +806,47 @@
             ).value(random_generator)
         else:
             max_mul = 1
 
         keys_name = dataframegroupby.keys
         dataset_above_tau_threshold = TauThresholdingOp(
             parent_ds,
-            tau_thresholding_task.parameters['epsilon_tau_thresholding'],
-            tau_thresholding_task.parameters['delta_tau_thresholding'],
+            tau_thresholding_task.parameters["epsilon_tau_thresholding"],
+            tau_thresholding_task.parameters["delta_tau_thresholding"],
         ).value(keys_name, max_mul, random_generator)
         keys_values = list(dataset_above_tau_threshold.index)
 
         dataframes_with_dp_sum = {}
         for index, column_name in enumerate(dataframegroupby.nth(0).columns):
             subtasks = [unwrap(task) for task in sum_tasks[index].subtasks]
-            bounds_parameters, sum_parameters = t.cast(
-                GenericTask, subtasks[0]
-            ), t.cast(GenericTask, subtasks[1])
+            bounds_parameters, sum_parameters = (
+                t.cast(GenericTask, subtasks[0]),
+                t.cast(GenericTask, subtasks[1]),
+            )
             column_type = (
                 parent_ds.schema()
                 .data_type()
                 .children()[column_name]
                 .protobuf()
             )
-            if column_type.WhichOneof('type') == 'optional':
+            if column_type.WhichOneof("type") == "optional":
                 dataframes_with_dp_sum[column_name] = dataframegroupby.apply(
                     lambda x: np.nan
                 ).to_frame(name="Sum")
                 continue
-            if column_type.WhichOneof('type') not in NUMERIC_TYPES:
+            if column_type.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             sum_op = GroupBySumOp(
                 parent_ds,
-                sum_parameters.parameters['noise'],
+                sum_parameters.parameters["noise"],
             )
             dataframes_with_dp_sum[column_name] = sum_op.value(
                 column_name, max_mul, bounds, random_generator, keys_values
             )
 
         if len(dataframes_with_dp_sum.keys()) == 1:
             return list(dataframes_with_dp_sum.values())[0]
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Type,
     Union,
 )
 import typing as t
 
 from pandas._libs import lib
 from pandas._libs.tslibs import BaseOffset
-from pandas.core.window.indexers import BaseIndexer
+from pandas.api.indexers import BaseIndexer
 import numpy as np
 import pandas as pd
 import pandas._typing as pdt
 
 from sarus_data_spec.dataspec_validator.parameter_kind import (
     DATASPEC,
     STATIC,
@@ -30,15 +30,15 @@
 )
 from sarus_data_spec.dataspec_validator.signature import (
     SarusBoundSignature,
     SarusParameter,
     SarusSignature,
     SarusSignatureValue,
 )
-from sarus_data_spec.dataspec_validator.typing import PEPKind
+from sarus_data_spec.dataspec_validator.typing import PUPKind
 import sarus_data_spec.typing as st
 
 from ..external_op import ExternalOpImplementation
 
 # Defined in pandas version > 1.3.5
 IgnoreRaise = t.Literal["ignore", "raise"]
 ValueKeyFunc = Optional[
@@ -159,34 +159,34 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
         (this, key) = signature.collect_args()
         return this.loc[key]
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """Token preserving if the key is a tuple or a slice that
         selects all the rows (e.g. loc[:, "col"], loc[:]).
-        PEP in the other cases.
+        PUP in the other cases.
         """
         key_arg = bound_signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, tuple) and len(key_value) == 2:
                 row_key, _ = key_value
                 if row_key == slice(None, None, None):
-                    return PEPKind.TOKEN_PRESERVING
+                    return PUPKind.TOKEN_PRESERVING
             elif isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
-                    return PEPKind.TOKEN_PRESERVING
+                    return PUPKind.TOKEN_PRESERVING
             elif isinstance(key_value, (int, str)):
                 # a scalar selects a single row
-                return PEPKind.ROW
+                return PUPKind.ROW
 
-        return PEPKind.PEP
+        return PUPKind.PUP
 
 
 class pd_set_loc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_LOC"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -225,30 +225,30 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
         (this, key) = signature.collect_args()
         return this.iloc[key]
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """Token preserving the alignment if the key is a slice that
         selects all the rows (e.g. iloc[:]).
-        PEP in the other cases.
+        PUP in the other cases.
         """
         key_arg = bound_signature["key"]
         if STATIC.isin(key_arg.parameter_kind()):
             key_value = key_arg.static_value()
             if isinstance(key_value, slice):
                 if key_value == slice(None, None, None):
-                    return PEPKind.TOKEN_PRESERVING
+                    return PUPKind.TOKEN_PRESERVING
             elif isinstance(key_value, (int, str)):
                 # a scalar selects a single row
-                return PEPKind.ROW
+                return PUPKind.ROW
 
-        return PEPKind.PEP
+        return PUPKind.PUP
 
 
 class pd_set_iloc(ExternalOpImplementation):
     _transform_id = "pandas.PD_SET_ILOC"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -288,16 +288,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         return this.head(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.PEP
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.PUP
 
 
 class pd_astype(ExternalOpImplementation):
     _transform_id = "pandas.PD_ASTYPE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -320,16 +320,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> pd.DataFrame:
         (this, kwargs) = signature.collect_kwargs_method()
         return this.astype(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_getitem(ExternalOpImplementation):
     _transform_id = "pandas.PD_GETITEM"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -342,35 +342,35 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, key) = signature.collect_args()
         return this[key]
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        """PEP in any case. Token preserving if the key is a string or a list
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        """PUP in any case. Token preserving if the key is a string or a list
         of strings."""
         if isinstance(bound_signature["key"].static_value(), st.DataSpec):
             key_type = bound_signature["key"].python_type()
             return (
-                PEPKind.TOKEN_PRESERVING
+                PUPKind.TOKEN_PRESERVING
                 if key_type in [str(str)]
-                else PEPKind.PEP
+                else PUPKind.PUP
             )
         else:
             key_value = bound_signature["key"].static_value()
             if isinstance(key_value, list):
                 # can select columns or rows depending on the type of the list
                 # values
                 all_strings = all([isinstance(x, str) for x in key_value])
-                return PEPKind.TOKEN_PRESERVING if all_strings else PEPKind.PEP
+                return PUPKind.TOKEN_PRESERVING if all_strings else PUPKind.PUP
             return (
-                PEPKind.TOKEN_PRESERVING
+                PUPKind.TOKEN_PRESERVING
                 if isinstance(key_value, str)
-                else PEPKind.PEP
+                else PUPKind.PUP
             )
 
 
 class pd_sum(ExternalOpImplementation):
     _transform_id = "pandas.PD_SUM"
     _dp_equivalent_id = "pandas.PD_SUM_DP"
     _signature = SarusSignature(
@@ -408,21 +408,21 @@
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.sum(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`axis=1`"""
         if bound_signature["this"].python_type() == str(pd.Series):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
 
         axis = bound_signature["axis"].static_value()
-        return PEPKind.TOKEN_PRESERVING if axis == 1 else PEPKind.NOT_PEP
+        return PUPKind.TOKEN_PRESERVING if axis == 1 else PUPKind.NOT_PUP
 
 
 class pd_mean(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEAN"
     _dp_equivalent_id = "pandas.PD_MEAN_DP"
     _signature = SarusSignature(
         SarusParameter(
@@ -454,21 +454,21 @@
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.mean(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`axis=1`"""
         if bound_signature["this"].python_type() == str(pd.Series):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
 
         axis = bound_signature["axis"].static_value()
-        return PEPKind.TOKEN_PRESERVING if axis == 1 else PEPKind.NOT_PEP
+        return PUPKind.TOKEN_PRESERVING if axis == 1 else PUPKind.NOT_PUP
 
 
 class pd_std(ExternalOpImplementation):
     _transform_id = "pandas.PD_STD"
     _dp_equivalent_id = "pandas.PD_STD_DP"
     _signature = SarusSignature(
         SarusParameter(
@@ -505,18 +505,18 @@
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.std(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`axis=1`"""
         axis = bound_signature["axis"].static_value()
-        return PEPKind.TOKEN_PRESERVING if axis == 1 else PEPKind.NOT_PEP
+        return PUPKind.TOKEN_PRESERVING if axis == 1 else PUPKind.NOT_PUP
 
 
 class pd_median(ExternalOpImplementation):
     _transform_id = "pandas.PD_MEDIAN"
     _dp_equivalent_id = "pandas.PD_MEDIAN_DP"
     _signature = SarusSignature(
         SarusParameter(
@@ -548,21 +548,21 @@
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["numeric_only"]
         return this.median(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`axis=1`"""
         if bound_signature["this"].python_type() == str(pd.Series):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
 
         axis = bound_signature["axis"].static_value()
-        return PEPKind.TOKEN_PRESERVING if axis == 1 else PEPKind.NOT_PEP
+        return PUPKind.TOKEN_PRESERVING if axis == 1 else PUPKind.NOT_PUP
 
 
 class pd_abs(ExternalOpImplementation):
     _transform_id = "pandas.PD_ABS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -571,16 +571,16 @@
         )
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this = signature["this"].value
         return this.abs()
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_drop(ExternalOpImplementation):
     _transform_id = "pandas.PD_DROP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -629,20 +629,20 @@
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.drop(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         axis = bound_signature["axis"].static_value()
-        if axis in [0, 'columns']:
-            return PEPKind.PEP
+        if axis in [0, "columns"]:
+            return PUPKind.PUP
         else:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
 
 
 class pd_dropna(ExternalOpImplementation):
     _transform_id = "pandas.PD_DROPNA"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -681,20 +681,20 @@
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["subset"]
             del kwargs["thresh"]
         return this.dropna(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         axis = bound_signature["axis"].static_value()
-        if axis in [0, 'columns']:
-            return PEPKind.PEP
+        if axis in [0, "columns"]:
+            return PUPKind.PUP
         else:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
 
 
 class pd_fillna(ExternalOpImplementation):
     _transform_id = "pandas.PD_FILLNA"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -736,21 +736,21 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.fillna(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`method` is `None`"""
         method = bound_signature["method"].static_value()
         if method is None:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
         else:
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
 
 
 class pd_isin(ExternalOpImplementation):
     _transform_id = "pandas.PD_ISIN"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -763,16 +763,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.isin(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_isnull(ExternalOpImplementation):
     _transform_id = "pandas.PD_ISNULL"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -781,16 +781,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, _ = signature.collect_kwargs_method()
         return this.isnull()
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_mask(ExternalOpImplementation):
     _transform_id = "pandas.PD_MASK"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -813,37 +813,37 @@
             annotation=bool,
             default=False,
             predicate=lambda x: x is False,
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[
-                Union[int, Literal['index', 'columns', 'rows']]
+                Union[int, Literal["index", "columns", "rows"]]
             ],
             default=None,
         ),
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.mask(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`cond` and `other` are not callable"""
         cond = bound_signature["cond"].static_value()
         other = bound_signature["other"].static_value()
         if callable(cond) or callable(other):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
         else:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
 
 
 class pd_notnull(ExternalOpImplementation):
     _transform_id = "pandas.PD_NOTNULL"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -852,16 +852,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, _ = signature.collect_kwargs_method()
         return this.notnull()
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_rename(ExternalOpImplementation):
     _transform_id = "pandas.PD_RENAME"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -885,53 +885,53 @@
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
         SarusParameter(
-            name='copy',
+            name="copy",
             annotation=Optional[bool],
             default=None,
         ),
         SarusParameter(
             name="inplace",
             annotation=bool,
             default=False,
             predicate=lambda x: x is False,
         ),
         SarusParameter(
-            name='level',
+            name="level",
             default=None,
             annotation=Hashable,
         ),
         SarusParameter(
             name="errors",
-            annotation=Literal['ignore', 'raise'],
-            default='ignore',
+            annotation=Literal["ignore", "raise"],
+            default="ignore",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["mapper"]
             del kwargs["columns"]
             del kwargs["axis"]
         return this.rename(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`mapper`, `index` and `columns` are not callable"""
         mapper = bound_signature["mapper"].static_value()
         index = bound_signature["index"].static_value()
         columns = bound_signature["columns"].static_value()
         if callable(mapper) or callable(index) or callable(columns):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
         else:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
 
 
 class pd_replace(ExternalOpImplementation):
     _transform_id = "pandas.PD_REPLACE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -961,31 +961,31 @@
         SarusParameter(
             name="regex",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
             name="method",
-            annotation=Literal['pad', 'ffill', 'bfill'],
+            annotation=Literal["pad", "ffill", "bfill"],
             default=lib.no_default,
         ),
         name=_transform_id,
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.replace(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         """`value` is not `None`"""
         value = bound_signature["value"].static_value()
         if value is None:
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
         else:
-            return PEPKind.TOKEN_PRESERVING
+            return PUPKind.TOKEN_PRESERVING
 
 
 class pd_round(ExternalOpImplementation):
     _transform_id = "pandas.PD_ROUND"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -999,16 +999,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.round(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_select_dtypes(ExternalOpImplementation):
     _transform_id = "pandas.PD_SELECT_DTYPES"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1027,16 +1027,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, kwargs) = signature.collect_kwargs_method()
         return this.select_dtypes(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.PEP
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.PUP
 
 
 class pd_add(ExternalOpImplementation):
     _transform_id = "pandas.PD_ADD"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1051,39 +1051,39 @@
             name="fill_value",
             annotation=Optional[Union[float, int]],
             default=None,
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[
-                Union[int, Literal['index', 'columns', 'rows']]
+                Union[int, Literal["index", "columns", "rows"]]
             ],
-            default='columns',
+            default="columns",
         ),
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.add(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 # for test only to remove
 class pd_add_test(ExternalOpImplementation):
     _transform_id = "pandas.PD_ADD_TEST"
-    _pep_equivalent_id = "pandas.PD_ADD_TEST_PEP"
+    _pup_equivalent_id = "pandas.PD_ADD_TEST_PUP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
         SarusParameter(
@@ -1094,39 +1094,39 @@
             name="fill_value",
             annotation=Optional[Union[float, int]],
             default=None,
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[
-                Union[int, Literal['index', 'columns', 'rows']]
+                Union[int, Literal["index", "columns", "rows"]]
             ],
-            default='columns',
+            default="columns",
         ),
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.add(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.NOT_PEP
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.NOT_PUP
 
 
 # for test only to remove
-class pd_add_test_pep(ExternalOpImplementation):
-    _transform_id = "pandas.PD_ADD_TEST_PEP"
-    _non_pep_equivalent_id = "pandas.PD_ADD_TEST"
+class pd_add_test_pup(ExternalOpImplementation):
+    _transform_id = "pandas.PD_ADD_TEST_PUP"
+    _non_pup_equivalent_id = "pandas.PD_ADD_TEST"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
             annotation=Union[pd.Series, pd.DataFrame],
             condition=DATASPEC,
         ),
         SarusParameter(
@@ -1137,33 +1137,33 @@
             name="fill_value",
             annotation=Optional[Union[float, int]],
             default=None,
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[
-                Union[int, Literal['index', 'columns', 'rows']]
+                Union[int, Literal["index", "columns", "rows"]]
             ],
-            default='columns',
+            default="columns",
         ),
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.add(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_sub(ExternalOpImplementation):
     _transform_id = "pandas.PD_SUB"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1178,33 +1178,33 @@
             name="fill_value",
             annotation=Optional[Union[float, int]],
             default=None,
         ),
         SarusParameter(
             name="axis",
             annotation=Optional[
-                Union[int, Literal['index', 'columns', 'rows']]
+                Union[int, Literal["index", "columns", "rows"]]
             ],
-            default='columns',
+            default="columns",
         ),
         SarusParameter(
             name="level",
             annotation=Optional[Union[int, str]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
         return this.sub(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_reset_index(ExternalOpImplementation):
     _transform_id = "pandas.PD_RESET_INDEX"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1394,15 +1394,15 @@
         SarusParameter(
             name="percentiles",
             annotation=Optional[Sequence[float]],
             default=None,
         ),
         SarusParameter(
             name="include",
-            annotation=Optional[Union[Literal['all'], List[pdt.Dtype]]],
+            annotation=Optional[Union[Literal["all"], List[pdt.Dtype]]],
             default=None,
         ),
         SarusParameter(
             name="exclude",
             annotation=Optional[List[pdt.Dtype]],
             default=None,
         ),
@@ -1689,21 +1689,21 @@
         this, kwargs = signature.collect_kwargs_method()
         if signature["this"].python_type() == str(pd.Series):
             del kwargs["axis"]
             del kwargs["result_type"]
             del kwargs["raw"]
         return this.apply(**kwargs)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
         axis_arg = bound_signature["axis"]
         if STATIC.isin(axis_arg.parameter_kind()):
             axis_value = axis_arg.static_value()
             if axis_value == 1:
-                return PEPKind.TOKEN_PRESERVING
-        return super().pep_kind(bound_signature)
+                return PUPKind.TOKEN_PRESERVING
+        return super().pup_kind(bound_signature)
 
 
 class pd_applymap(ExternalOpImplementation):
     _transform_id = "pandas.PD_APPLYMAP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1723,16 +1723,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.applymap(**kwargs)
 
-    def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_map(ExternalOpImplementation):
     _transform_id = "pandas.PD_MAP"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -1752,16 +1752,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.map(**kwargs)
 
-    def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_skew(ExternalOpImplementation):
     _transform_id = "pandas.PD_SKEW"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -2324,20 +2324,20 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, kwargs = signature.collect_kwargs_method()
         return this.groupby(**kwargs)
 
-    def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
+    def pup_kind(self, signature: SarusBoundSignature) -> PUPKind:
         by = signature["axis"].static_value()
         if callable(by):
-            return PEPKind.NOT_PEP
+            return PUPKind.NOT_PUP
         else:
-            return PEPKind.PEP
+            return PUPKind.PUP
 
 
 class pd_merge(ExternalOpImplementation):
     _transform_id = "pandas.PD_MERGE"
     _signature = SarusSignature(
         SarusParameter(
             name="left",
@@ -2560,16 +2560,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this, other) = signature.collect_args()
         return this == other
 
-    def pep_kind(self, signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pd_concat(ExternalOpImplementation):
     _transform_id = "pandas.PD_CONCAT"
     _signature = SarusSignature(
         SarusParameter(
             name="objs",
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas/pandas_dp.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,65 +15,86 @@
     ExternalOpImplementation,
     retrieve_max_mult_info_from_parent,
 )
 
 logger = logging.getLogger(__name__)
 
 try:
-    from sarus_statistics.ops.bounds.op import BoundOp
-    from sarus_statistics.ops.corr.op import CorrOp
-    from sarus_statistics.ops.histograms.op import CountOp, HistogramOp
-    from sarus_statistics.ops.max_multiplicity.op import MaxMultiplicityOp
-    from sarus_statistics.ops.mean.op import MeanOp
-    from sarus_statistics.ops.median.op import MedianOp
-    from sarus_statistics.ops.std.op import StdOp
-    from sarus_statistics.ops.sum.op import SumOp
-    from sarus_statistics.protobuf.multiplicity_pb2 import (
+    from sarus_data_spec.sarus_statistics.ops.bounds.op import BoundOp
+    from sarus_data_spec.sarus_statistics.ops.corr.op import CorrOp
+    from sarus_data_spec.sarus_statistics.ops.histograms.op import (
+        CountOp,
+        HistogramOp,
+    )
+    from sarus_data_spec.sarus_statistics.ops.max_multiplicity.op import (
+        MaxMultiplicityOp,
+    )
+    from sarus_data_spec.sarus_statistics.ops.mean.op import MeanOp
+    from sarus_data_spec.sarus_statistics.ops.median.op import MedianOp
+    from sarus_data_spec.sarus_statistics.ops.std.op import StdOp
+    from sarus_data_spec.sarus_statistics.ops.sum.op import SumOp
+    from sarus_data_spec.sarus_statistics.protobuf.multiplicity_pb2 import (
         MultiplicityParameters,
     )
-except ModuleNotFoundError as e_pandas_dp:
-    if "sarus_statistics" not in str(e_pandas_dp):
-        raise
+except ModuleNotFoundError:
+    pass
+    # TODO properly: from sarus_data_spec.sarus_statistics.ops.bounds.op
+    # imports sarus_differential_privacy
+    # if "sarus_data_spec.sarus_statistics" not in str(e_pandas_dp):
+    #     raise
 
 try:
     from sarus_differential_privacy.query import ComposedPrivateQuery
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus_differential_privacy" not in str(e_pandas_dp):
         raise
 
 try:
-    from sarus_query_builder.builders.bounds_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.bounds_builder import (
         simple_bounds_builder,
     )
-    from sarus_query_builder.builders.composed_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.composed_builder import (
         ComposedBuilder,
         simple_composed_builder,
     )
-    from sarus_query_builder.builders.corr_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.corr_builder import (
         corr_builder as simple_corr_builder,
     )
-    from sarus_query_builder.builders.max_multiplicity_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.max_multiplicity_builder import (  # noqa : E501
         simple_max_multiplicity_builder,
     )
-    from sarus_query_builder.builders.mean_builder import mean_builder
-    from sarus_query_builder.builders.median_builder import median_builder
-    from sarus_query_builder.builders.standard_mechanisms_builder import (
+    from sarus_data_spec.sarus_query_builder.builders.mean_builder import (
+        mean_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.median_builder import (
+        median_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.standard_mechanisms_builder import (  # noqa : E501
         laplace_builder,
     )
-    from sarus_query_builder.builders.std_builder import std_builder
-    from sarus_query_builder.builders.sum_builder import sum_builder
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
-    from sarus_query_builder.protobuf.query_pb2 import GenericTask, Query
+    from sarus_data_spec.sarus_query_builder.builders.std_builder import (
+        std_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.builders.sum_builder import (
+        sum_builder,
+    )
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
+    from sarus_data_spec.sarus_query_builder.protobuf.query_pb2 import (
+        GenericTask,
+        Query,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
     OptimizableQueryBuilder = t.Any  # type: ignore
 
 
-NUMERIC_TYPES = ('integer', 'float', 'boolean')
+NUMERIC_TYPES = ("integer", "float", "boolean")
 
 
 class pd_shape_dp(ExternalOpImplementation):
     _transform_id = "pandas.PD_SHAPE_DP"
     _non_dp_equivalent_id = "pandas.PD_SHAPE"
 
     def is_dp(self, signature: SarusBoundSignature) -> bool:
@@ -121,15 +142,16 @@
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
-            - `pe`: the protected entity used by `sarus_statistics` primitives
+            - `pe`: the protected entity used by
+            `sarus_data_spec.sarus_statistics`primitives
         """
         # Evaluate arguments
         parent_ds = signature.static_kwargs()["this"]
         (dataframe, budget, seed) = await signature.collect_args()
 
         # Get QB task parametrization
         _, tasks = await self.private_queries_and_task(signature)
@@ -143,15 +165,15 @@
         random_generator = np.random.default_rng(abs(seed))
         max_mul, shape_task = retrieve_or_compute_max_mult(
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
         assert len(shape_task) == 1
         n_rows = CountOp(
             parent_ds,
-            noise=shape_task[0].parameters['noise'],
+            noise=shape_task[0].parameters["noise"],
         ).value(None, max_mul, random_generator)
 
         dp_shape = (n_rows, *shape[1:])
         return dp_shape
 
 
 class pd_sum_dp(ExternalOpImplementation):
@@ -233,39 +255,40 @@
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
         sum_dp_dict = {}
         schema_fields = parent_schema.data_type().children()
         for tasks_column, (column_name, column_type) in zip(
             unwrapped_other_tasks, (schema_fields.items())
         ):
-            bounds_parameters, sum_parameters = t.cast(
-                GenericTask, unwrap(tasks_column.subtasks[0])
-            ), t.cast(GenericTask, unwrap(tasks_column.subtasks[0]))
+            bounds_parameters, sum_parameters = (
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+            )
             type_pb = column_type.protobuf()
-            if type_pb.WhichOneof('type') == 'optional':
+            if type_pb.WhichOneof("type") == "optional":
                 if not skipna:
                     sum_dp_dict[column_name] = np.nan
                     continue
                 type_pb = type_pb.optional.type
-            if type_pb.WhichOneof('type') not in NUMERIC_TYPES:
+            if type_pb.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             # TODO parent_ds doesn't have a size
             # if parent_ds.size().children()[column_name].size()
             #  < min_count:
             #     sum_dp_dict[column_name] = np.nan
             #     continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             sum_op = SumOp(
                 parent_ds,
-                sum_parameters.parameters['noise'],
+                sum_parameters.parameters["noise"],
             )
             sum_dp_dict[column_name] = sum_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
         if signature["this"].python_type() == str(pd.DataFrame):
             sum_dp = pd.Series(sum_dp_dict)
@@ -353,33 +376,34 @@
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
         mean_dp_dict = {}
         schema_fields = parent_schema.data_type().children()
         for tasks_column, (column_name, column_type) in zip(
             unwrapped_other_tasks, (schema_fields.items())
         ):
-            bounds_parameters, mean_parameters = t.cast(
-                GenericTask, unwrap(tasks_column.subtasks[0])
-            ), t.cast(GenericTask, unwrap(tasks_column.subtasks[1]))
+            bounds_parameters, mean_parameters = (
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[1])),
+            )
 
             type_pb = column_type.protobuf()
-            if type_pb.WhichOneof('type') == 'optional':
+            if type_pb.WhichOneof("type") == "optional":
                 if not skipna:
                     mean_dp_dict[column_name] = np.nan
                     continue
                 type_pb = type_pb.optional.type
-            if type_pb.WhichOneof('type') not in NUMERIC_TYPES:
+            if type_pb.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             mean_op = MeanOp(
                 parent_ds,
-                mean_parameters.parameters['noise'],
+                mean_parameters.parameters["noise"],
             )
             mean_dp_dict[column_name] = mean_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
         if signature["this"].python_type() == str(pd.DataFrame):
             mean_dp = pd.Series(mean_dp_dict)
@@ -467,34 +491,35 @@
         )
 
         median_dp_dict = {}
         schema_fields = parent_schema.data_type().children()
         for tasks_column, (column_name, column_type) in zip(
             unwrapped_other_tasks, (schema_fields.items())
         ):
-            bounds_parameters, median_parameters = t.cast(
-                GenericTask, unwrap(tasks_column.subtasks[0])
-            ), t.cast(GenericTask, unwrap(tasks_column.subtasks[1]))
+            bounds_parameters, median_parameters = (
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[1])),
+            )
             type_pb = column_type.protobuf()
-            if type_pb.WhichOneof('type') == 'optional':
+            if type_pb.WhichOneof("type") == "optional":
                 if not skipna:
                     median_dp_dict[column_name] = np.nan
                     continue
                 type_pb = type_pb.optional.type
 
-            if type_pb.WhichOneof('type') not in NUMERIC_TYPES:
+            if type_pb.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             median_op = MedianOp(
                 parent_ds,
-                median_parameters.parameters['noise'],
+                median_parameters.parameters["noise"],
             )
             median_dp_dict[column_name] = median_op.value(
                 column_name, max_mul, bounds, random_generator
             )
         if signature["this"].python_type() == str(pd.DataFrame):
             median_dp = pd.Series(median_dp_dict)
         else:
@@ -582,35 +607,36 @@
         )
 
         std_dp_dict = {}
         schema_fields = parent_schema.data_type().children()
         for tasks_column, (column_name, column_type) in zip(
             unwrapped_other_tasks, (schema_fields.items())
         ):
-            bounds_parameters, std_parameters = t.cast(
-                GenericTask, unwrap(tasks_column.subtasks[0])
-            ), t.cast(GenericTask, unwrap(tasks_column.subtasks[0]))
+            bounds_parameters, std_parameters = (
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+                t.cast(GenericTask, unwrap(tasks_column.subtasks[0])),
+            )
             type_pb = column_type.protobuf()
-            if type_pb.HasField('optional'):
+            if type_pb.HasField("optional"):
                 if not skipna:
                     std_dp_dict[column_name] = np.nan
                     continue
                 type_pb = type_pb.optional.type
-            if type_pb.WhichOneof('type') not in NUMERIC_TYPES:
+            if type_pb.WhichOneof("type") not in NUMERIC_TYPES:
                 continue
 
             bounds = BoundOp(
                 parent_ds,
-                bounds_parameters.parameters['noise'],
+                bounds_parameters.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
             std_op = StdOp(
                 parent_ds,
-                std_parameters.parameters['noise_mean'],
-                std_parameters.parameters['noise_square'],
-                std_parameters.parameters['noise_count'],
+                std_parameters.parameters["noise_mean"],
+                std_parameters.parameters["noise_square"],
+                std_parameters.parameters["noise_count"],
             )
             std_dp_dict[column_name] = std_op.value(
                 column_name, max_mul, bounds, random_generator
             )
 
         if signature["this"].python_type() == str(pd.DataFrame):
             std_dp = pd.Series(std_dp_dict)
@@ -683,20 +709,20 @@
         random_generator = np.random.default_rng(abs(seed_value))
         max_mul, unwrapped_other_tasks = retrieve_or_compute_max_mult(
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
         count_dp_dict = {}
 
         schema_fields = parent_schema.data_type().children()
-        for count_parameter, (column_name, column_type) in zip(
-            unwrapped_other_tasks, (schema_fields.items())
+        for count_parameter, column_name in zip(
+            unwrapped_other_tasks, (schema_fields.keys())
         ):
             count_dp_dict[column_name] = CountOp(
                 parent_ds,
-                count_parameter.parameters['noise'],
+                count_parameter.parameters["noise"],
             ).value(column_name, max_mul, random_generator)
 
         if signature["this"].python_type() == str(pd.DataFrame):
             count_dp = pd.Series(count_dp_dict)
         else:
             count_dp = list(count_dp_dict.values()).pop()
         return count_dp
@@ -751,15 +777,16 @@
         """Implementation of DP shape.
 
         A DP implementation receives additional arguments compared to a
         standard external implementation:
             - `budget`: a list of sp.Scalar.PrivacyParams.Point
                 object containing each an epsilon and a delta values
             - `seed`: an integer used to parametrize random number generators
-            - `pe`: the protected entity used by `sarus_statistics` primitives
+            - `pe`: the protected entity used by
+            `sarus_data_spec.sarus_statistics` primitives
         """
         parent_ds: st.Dataset = signature["this"].static_value()
         budget_value = await signature["budget"].collect()
         seed_value = await signature["seed"].collect()
         sort = await signature["sort"].collect()
         ascending = await signature["ascending"].collect()
         normalize = await signature["normalize"].collect()
@@ -775,31 +802,29 @@
         )
         max_mul, unwrapped_other_tasks = retrieve_or_compute_max_mult(
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
 
         count_dp_dict = {}
         schema_fields = parent_schema.data_type().children()
-        for count_parameters, (column_name, column_type) in zip(
-            unwrapped_other_tasks, (schema_fields.items())
+        for count_parameters, column_name in zip(
+            unwrapped_other_tasks, (schema_fields.keys())
         ):
             histogram = t.cast(
                 t.Dict[str, float],
                 HistogramOp(
                     parent_ds,
-                    noise=count_parameters.parameters['noise'],
+                    noise=count_parameters.parameters["noise"],
                     sort=sort,
                     ascending=ascending,
                     normalize=normalize,
                     dropna=dropna,
                 ).value(column_name, max_mul, random_generator),
             )
-            count_dp_dict[column_name] = {
-                key: round(count) for key, count in histogram.items()
-            }
+            count_dp_dict[column_name] = histogram
 
         # for now only on series
         count_dp = pd.Series(list(count_dp_dict.values())[0])
         return count_dp
 
 
 class pd_corr_dp(ExternalOpImplementation):
@@ -814,15 +839,15 @@
         `min_periods = 1`
         """
         method = signature["method"].static_value()
         min_periods = signature["min_periods"].static_value()
         is_dataframe = bool(
             signature["this"].python_type() == str(pd.DataFrame)
         )
-        return is_dataframe and (min_periods == 1) and (method == 'pearson')
+        return is_dataframe and (min_periods == 1) and (method == "pearson")
 
     async def query_builder(
         self, signature: SarusBoundSignature
     ) -> OptimizableQueryBuilder:
         parent_ds = signature["this"].static_value()
         parent_schema = await parent_ds.manager().async_schema(parent_ds)
         max_max_mult = ceil(
@@ -871,16 +896,16 @@
         )
         max_mul, unwrapped_other_tasks = retrieve_or_compute_max_mult(
             max_mult, tasks, parent_ds, random_generator, epsilon
         )
         assert len(unwrapped_other_tasks) == 1
         corr_dp = CorrOp(
             parent_ds,
-            unwrapped_other_tasks[0].parameters['epsilon'],
-            unwrapped_other_tasks[0].parameters['dims'],
+            unwrapped_other_tasks[0].parameters["epsilon"],
+            unwrapped_other_tasks[0].parameters["dims"],
         ).value(max_mul, random_generator=random_generator)
 
         return corr_dp
 
 
 async def get_budget(signature: SarusBoundSignature) -> t.Tuple[float, float]:
     """Retrieve (epsilon, delta) from signature"""
@@ -900,15 +925,15 @@
 
 
 def builder_from_multiplicity(
     builder: OptimizableQueryBuilder, max_mult: str, max_max_mult: int
 ) -> OptimizableQueryBuilder:
     """Adds a builder from multiplicity if the max_mult is empty"""
 
-    if max_mult != '':
+    if max_mult != "":
         # in this case no need to recompute it
         return builder
     max_mult_builder = simple_max_multiplicity_builder(
         builder.dataset,
         Query(
             max_multiplicity=Query.MaxMultiplicity(
                 max_max_multiplicity=max_max_mult
@@ -933,15 +958,15 @@
     parent_ds: st.Dataset,
     random_generator: np.random.Generator,
     epsilon: float,
 ) -> t.Tuple[int, t.List[st.Task]]:
     """Either retrieves the max_mult if it is not an empty string or computes it
     using the tasks"""
 
-    if max_mult == '':
+    if max_mult == "":
         # there is no pre-computed max_multiplicity so we need
         # to recompute it
         unwrapped = [unwrap(subtask) for subtask in tasks.subtasks]
         max_mult_task, unwrapped_other_tasks = (
             t.cast(MultiplicityParameters, unwrapped[0]),
             t.cast(t.List[GenericTask], unwrapped[1:]),
         )
@@ -950,15 +975,15 @@
             epsilon,  # parameter for quantiles
             max_mult_task.compute.noise_user_count,
             max_mult_task.compute.noise_multiplicity,
             max_mult_task.compute.max_max_multiplicity,
         ).value(random_generator)
     else:
         max_mul = float(max_mult)
-        if hasattr(tasks, 'subtasks'):
+        if hasattr(tasks, "subtasks"):
             unwrapped_other_tasks = t.cast(
                 t.List[GenericTask],
                 [unwrap(subtask) for subtask in tasks.subtasks],
             )  # for type compatibility mainly
         else:
             unwrapped_other_tasks = [tasks]
     return ceil(max_mul), unwrapped_other_tasks
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/pandas_profiling.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,87 +23,87 @@
 Settings = Any
 
 
 class pd_profile_report(ExternalOpImplementation):
     _transform_id = "pandas_profiling.PD_PROFILE_REPORT"
     _signature = SarusSignature(
         SarusParameter(
-            name='df',
+            name="df",
             annotation=Optional[pd.DataFrame],
             default=None,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
-            name='minimal',
+            name="minimal",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='tsmode',
+            name="tsmode",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='sortby',
+            name="sortby",
             annotation=Optional[str],
             default=None,
         ),
         SarusParameter(
-            name='sensitive',
+            name="sensitive",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='explorative',
+            name="explorative",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='dark_mode',
+            name="dark_mode",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='orange_mode',
+            name="orange_mode",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
-            name='sample',
+            name="sample",
             annotation=Optional[dict],
             default=None,
         ),
         SarusParameter(
-            name='config_file',
+            name="config_file",
             annotation=Optional[Union[Path, str]],
             default=None,
             predicate=lambda x: x is None,
         ),
         SarusParameter(
-            name='lazy',
+            name="lazy",
             annotation=bool,
             default=True,
         ),
         SarusParameter(
-            name='typeset',
+            name="typeset",
             annotation=Optional[VisionsTypeset],
             default=None,
         ),
         SarusParameter(
-            name='summarizer',
+            name="summarizer",
             annotation=Optional[BaseSummarizer],
             default=None,
         ),
         SarusParameter(
-            name='config',
+            name="config",
             annotation=Optional[Settings],
             default=None,
         ),
         SarusParameter(
-            name='type_schema',
+            name="type_schema",
             annotation=Optional[dict],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/scipy.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/scipy.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/Explanation.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/explainer.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/explainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,21 +263,21 @@
             name="data",
             annotation=Optional[Union[ndarray, DataFrame]],
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="model_output",
             annotation=str,
-            default='raw',
+            default="raw",
             condition=STATIC,
         ),
         SarusParameter(
             name="feature_perturbation",
             annotation=str,
-            default='interventional',
+            default="interventional",
             condition=STATIC,
         ),
         SarusParameter(
             name="feature_names",
             annotation=Optional[List[str]],
             default=None,
             condition=STATIC,
@@ -310,20 +310,20 @@
             name="data",
             annotation=Optional[Union[np.ndarray, pd.DataFrame]],
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="model_output",
             annotation=str,
-            default='raw',
+            default="raw",
         ),
         SarusParameter(
             name="feature_perturbation",
             annotation=str,
-            default='interventional',
+            default="interventional",
         ),
         SarusParameter(
             name="feature_names",
             annotation=Optional[List[str]],
             default=None,
         ),
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/maskers.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/maskers.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             name="max_samples",
             annotation=int,
             default=100,
         ),
         SarusParameter(
             name="clustering",
             annotation=str,
-            default='correlation',
+            default="correlation",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return shap.maskers.Partition(**kwargs)
 
@@ -146,15 +146,15 @@
             name="data",
             annotation=Union[np.ndarray, pd.DataFrame, Dict[str, np.ndarray]],
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="method",
             annotation=str,
-            default='linear',
+            default="linear",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return shap.maskers.Impute(**kwargs)
 
@@ -283,20 +283,20 @@
             name="mask_token",
             annotation=Optional[Union[str, int, None]],
             default=None,
         ),
         SarusParameter(
             name="collapse_mask_token",
             annotation=Optional[Union[bool, str]],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="output_type",
             annotation=Optional[str],
-            default='string',
+            default="string",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return shap.maskers.Text(**kwargs)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/plots.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     import shap
 
     explanation_abs = Explanation.abs
 except ModuleNotFoundError:
     OpChain = Any
     explanation_abs = Any
     Explanation = Any
-    warnings.warn('Shap not available')
+    warnings.warn("Shap not available")
 
 
 class shap_plots_bar(ExternalOpImplementation):
     _transform_id = "shap.SHAP_PLOTS_BAR"
     _signature = SarusSignature(
         SarusParameter(
             name="shap_values",
@@ -61,15 +61,15 @@
             name="merge_cohorts",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
             name="show_data",
             annotation=str,
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="show",
             annotation=bool,
             default=True,
         ),
     )
@@ -153,15 +153,15 @@
             name="color",
             annotation=Optional[OpChain],
             default=None,
         ),
         SarusParameter(
             name="axis_color",
             annotation=Optional[str],
-            default='#333333',
+            default="#333333",
         ),
         SarusParameter(
             name="alpha",
             annotation=Optional[float],
             default=1,
         ),
         SarusParameter(
@@ -173,15 +173,15 @@
             name="log_scale",
             annotation=Optional[bool],
             default=False,
         ),
         SarusParameter(
             name="color_bar_label",
             annotation=Optional[str],
-            default='Feature value',
+            default="Feature value",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         if kwargs["order"] is None:
             kwargs["order"] = shap.Explanation.abs.mean(0)
@@ -273,15 +273,15 @@
             name="color",
             annotation=Optional[Any],
             default=None,
         ),
         SarusParameter(
             name="axis_color",
             annotation=str,
-            default='#333333',
+            default="#333333",
         ),
         SarusParameter(
             name="title",
             annotation=Optional[str],
             default=None,
         ),
         SarusParameter(
@@ -303,15 +303,15 @@
             name="color_bar",
             annotation=bool,
             default=True,
         ),
         SarusParameter(
             name="plot_size",
             annotation=Union[str, float, Tuple[float, float]],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="layered_violin_max_num_bins",
             annotation=int,
             default=20,
         ),
         SarusParameter(
@@ -323,15 +323,15 @@
             name="class_inds",
             annotation=Optional[List[int]],
             default=None,
         ),
         SarusParameter(
             name="color_bar_label",
             annotation=str,
-            default='Feature value',
+            default="Feature value",
         ),
         SarusParameter(
             name="cmap",
             annotation=Any,  # Adjust accordingly
             default=None,
         ),
         SarusParameter(
@@ -379,25 +379,25 @@
             annotation=Optional[Union[ndarray, DataFrame]],
             default=None,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="interaction_index",
             annotation=Union[str, int],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="color",
             annotation=str,
-            default='#1E88E5',
+            default="#1E88E5",
         ),
         SarusParameter(
             name="axis_color",
             annotation=str,
-            default='#333333',
+            default="#333333",
         ),
         SarusParameter(
             name="cmap",
             annotation=Optional[str],
             default=None,
         ),
         SarusParameter(
@@ -476,20 +476,20 @@
             name="out_names",
             annotation=Optional[str],
             default=None,
         ),
         SarusParameter(
             name="link",
             annotation=str,
-            default='identity',
+            default="identity",
         ),
         SarusParameter(
             name="plot_cmap",
             annotation=str,
-            default='RdBu',
+            default="RdBu",
         ),
         SarusParameter(
             name="matplotlib",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/shap/utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/shap/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             name="X",
             annotation=Any,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="metric",
             annotation=str,
-            default='sqeuclidean',
+            default="sqeuclidean",
         ),
         SarusParameter(
             name="anchor_first",
             annotation=bool,
             default=False,
         ),
     )
@@ -85,15 +85,15 @@
             name="X",
             annotation=Any,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="metric",
             annotation=str,
-            default='correlation',
+            default="correlation",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return shap.utils.partition_tree(**kwargs)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,25 +65,25 @@
             name="min_samples",
             annotation=int,
             default=5,
         ),
         SarusParameter(
             name="metric",
             annotation=Union[str, Callable],
-            default='euclidean',
+            default="euclidean",
         ),
         SarusParameter(
             name="metric_params",
             annotation=Optional[dict],
             default=None,
         ),
         SarusParameter(
             name="algorithm",
-            annotation=Literal['auto', 'ball_tree', 'kd_tree', 'brute'],
-            default='auto',
+            annotation=Literal["auto", "ball_tree", "kd_tree", "brute"],
+            default="auto",
         ),
         SarusParameter(
             name="leaf_size",
             annotation=int,
             default=30,
         ),
         SarusParameter(
@@ -352,56 +352,56 @@
             annotation=float,
             default=np.inf,
         ),
         SarusParameter(
             name="metric",
             annotation=Union[
                 Literal[
-                    'cityblock',
-                    'cosine',
-                    'euclidean',
-                    'l1',
-                    'l2',
-                    'manhattan',
-                    'braycurtis',
-                    'canberra',
-                    'chebyshev',
-                    'correlation',
-                    'dice',
-                    'hamming',
-                    'jaccard',
-                    'kulsinski',
-                    'mahalanobis',
-                    'minkowski',
-                    'rogerstanimoto',
-                    'russellrao',
-                    'seuclidean',
-                    'sokalmichener',
-                    'sokalsneath',
-                    'sqeuclidean',
-                    'yule',
+                    "cityblock",
+                    "cosine",
+                    "euclidean",
+                    "l1",
+                    "l2",
+                    "manhattan",
+                    "braycurtis",
+                    "canberra",
+                    "chebyshev",
+                    "correlation",
+                    "dice",
+                    "hamming",
+                    "jaccard",
+                    "kulsinski",
+                    "mahalanobis",
+                    "minkowski",
+                    "rogerstanimoto",
+                    "russellrao",
+                    "seuclidean",
+                    "sokalmichener",
+                    "sokalsneath",
+                    "sqeuclidean",
+                    "yule",
                 ],
                 Callable,
             ],
-            default='minkowski',
+            default="minkowski",
         ),
         SarusParameter(
             name="p",
             annotation=float,
             default=2,
         ),
         SarusParameter(
             name="metric_params",
             annotation=Optional[dict],
             default=None,
         ),
         SarusParameter(
             name="cluster_method",
             annotation=Literal["xi", "dbscan"],
-            default='xi',
+            default="xi",
         ),
         SarusParameter(
             name="eps",
             annotation=Optional[float],
             default=None,
         ),
         SarusParameter(
@@ -417,16 +417,16 @@
         SarusParameter(
             name="min_cluster_size",
             annotation=Optional[Union[float, int]],
             default=None,
         ),
         SarusParameter(
             name="algorithm",
-            annotation=Literal['auto', 'ball_tree', 'kd_tree', 'brute'],
-            default='auto',
+            annotation=Literal["auto", "ball_tree", "kd_tree", "brute"],
+            default="auto",
         ),
         SarusParameter(
             name="leaf_size",
             annotation=int,
             default=30,
         ),
         SarusParameter(
@@ -502,15 +502,15 @@
         SarusParameter(
             name="eigen_tol",
             annotation=Union[float, Literal["auto"]],
             default="auto",
         ),
         SarusParameter(
             name="assign_labels",
-            annotation=Literal['kmeans', 'discretize', 'cluster_qr'],
+            annotation=Literal["kmeans", "discretize", "cluster_qr"],
             default="kmeans",
         ),
         SarusParameter(
             name="degree",
             annotation=int,
             default=3,
         ),
@@ -548,46 +548,46 @@
         SarusParameter(
             name="n_clusters",
             annotation=Union[int, Tuple[int, int]],
             default=3,
         ),
         SarusParameter(
             name="method",
-            annotation=Literal['bistochastic', 'scale', 'log'],
-            default='bistochastic',
+            annotation=Literal["bistochastic", "scale", "log"],
+            default="bistochastic",
         ),
         SarusParameter(
             name="n_components",
             annotation=int,
             default=6,
         ),
         SarusParameter(
             name="n_best",
             annotation=int,
             default=3,
         ),
         SarusParameter(
             name="svd_method",
-            annotation=Literal['randomized', 'arpack'],
-            default='randomized',
+            annotation=Literal["randomized", "arpack"],
+            default="randomized",
         ),
         SarusParameter(
             name="n_svd_vecs",
             annotation=Optional[int],
             default=None,
         ),
         SarusParameter(
             name="mini_batch",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
             name="init",
-            annotation=Union[Literal['k-means++', 'random'], np.ndarray],
-            default='k-means++',
+            annotation=Union[Literal["k-means++", "random"], np.ndarray],
+            default="k-means++",
         ),
         SarusParameter(
             name="n_init",
             annotation=int,
             default=10,
         ),
         SarusParameter(
@@ -673,15 +673,15 @@
         SarusParameter(
             name="preference",
             annotation=Optional[Union[ArrayLike, float]],
             default=None,
         ),
         SarusParameter(
             name="affinity",
-            annotation=Literal['euclidean', 'precomputed'],
+            annotation=Literal["euclidean", "precomputed"],
             default="euclidean",
         ),
         SarusParameter(
             name="verbose",
             annotation=bool,
             default=False,
         ),
@@ -703,16 +703,16 @@
         SarusParameter(
             name="n_clusters",
             annotation=Optional[int],
             default=2,
         ),
         SarusParameter(
             name="affinity",
-            annotation=Union[Literal['euclidean', 'precomputed'], Callable],
-            default='euclidean',
+            annotation=Union[Literal["euclidean", "precomputed"], Callable],
+            default="euclidean",
         ),
         SarusParameter(
             name="metric",
             annotation=Optional[
                 Union[
                     Literal[
                         "euclidean",
@@ -737,20 +737,20 @@
             name="connectivity",
             annotation=Optional[Union[ArrayLike, Callable]],
             default=None,
         ),
         SarusParameter(
             name="compute_full_tree",
             annotation=Union[Literal["auto"], bool],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="linkage",
-            annotation=Literal['ward', 'complete', 'average', 'single'],
-            default='ward',
+            annotation=Literal["ward", "complete", "average", "single"],
+            default="ward",
         ),
         SarusParameter(
             name="distance_threshold",
             annotation=Optional[float],
             default=None,
         ),
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/decomposition.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,36 +32,36 @@
         SarusParameter(
             name="whiten",
             annotation=bool,
             default=False,
         ),
         SarusParameter(
             name="svd_solver",
-            annotation=Literal['auto', 'full', 'arpack', 'randomized'],
-            default='auto',
+            annotation=Literal["auto", "full", "arpack", "randomized"],
+            default="auto",
         ),
         SarusParameter(
             name="tol",
             annotation=float,
             default=0.0,
         ),
         SarusParameter(
             name="iterated_power",
             annotation=Union[int, Literal["auto"]],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="n_oversamples",
             annotation=int,
             default=10,
         ),
         SarusParameter(
             name="power_iteration_normalizer",
-            annotation=Literal['auto', 'QR', 'LU', 'none'],
-            default='auto',
+            annotation=Literal["auto", "QR", "LU", "none"],
+            default="auto",
         ),
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
     )
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         SarusParameter(
             name="learning_rate",
             annotation=float,
             default=1.0,
         ),
         SarusParameter(
             name="loss",
-            annotation=Literal['linear', 'square', 'exponential'],
+            annotation=Literal["linear", "square", "exponential"],
             default="linear",
         ),
         SarusParameter(
             name="random_state",
             annotation=Optional[Union[int, np.random.RandomState]],
             default=None,
         ),
@@ -1013,17 +1013,17 @@
                 int, BaseCrossValidator, Iterable, Literal["prefit"]
             ],
             default=None,
         ),
         SarusParameter(
             name="stack_method",
             annotation=Literal[
-                'auto', 'predict_proba', 'decision_function', 'predict'
+                "auto", "predict_proba", "decision_function", "predict"
             ],
-            default='auto',
+            default="auto",
         ),
         SarusParameter(
             name="n_jobs",
             annotation=int,
             default=None,
             predicate=lambda x: x is None,
         ),
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/inspection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/lib.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,17 @@
             name="y_score",
             annotation=npt.ArrayLike,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="average",
             annotation=Optional[
-                Literal['micro', 'samples', 'weighted', 'macro']
+                Literal["micro", "samples", "weighted", "macro"]
             ],
-            default='macro',
+            default="macro",
         ),
         SarusParameter(
             name="pos_label",
             annotation=Union[int, str],
             default=1,
         ),
         SarusParameter(
@@ -157,15 +157,15 @@
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
         SarusParameter(
             name="normalize",
-            annotation=Optional[Literal['true', 'pred', 'all']],
+            annotation=Optional[Literal["true", "pred", "all"]],
             default=None,
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return metrics.confusion_matrix(**kwargs)
@@ -193,17 +193,17 @@
             name="pos_label",
             annotation=Union[int, str],
             default=1,
         ),
         SarusParameter(
             name="average",
             annotation=Optional[
-                Literal['micro', 'macro', 'samples', 'weighted', 'binary']
+                Literal["micro", "macro", "samples", "weighted", "binary"]
             ],
-            default='binary',
+            default="binary",
         ),
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
         SarusParameter(
@@ -270,27 +270,27 @@
             name="pos_label",
             annotation=Union[int, str],
             default=1,
         ),
         SarusParameter(
             name="average",
             annotation=Optional[
-                Literal['micro', 'macro', 'samples', 'weighted', 'binary']
+                Literal["micro", "macro", "samples", "weighted", "binary"]
             ],
-            default='binary',
+            default="binary",
         ),
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
         SarusParameter(
             name="zero_division",
-            annotation=Literal['warn', 0, 1],
-            default='warn',
+            annotation=Literal["warn", 0, 1],
+            default="warn",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return metrics.precision_score(**kwargs)
 
@@ -317,27 +317,27 @@
             name="pos_label",
             annotation=Union[str, int],
             default=1,
         ),
         SarusParameter(
             name="average",
             annotation=Optional[
-                Literal['micro', 'macro', 'samples', 'weighted', 'binary']
+                Literal["micro", "macro", "samples", "weighted", "binary"]
             ],
-            default='binary',
+            default="binary",
         ),
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
         SarusParameter(
             name="zero_division",
-            annotation=Literal['warn', 0, 1],
-            default='warn',
+            annotation=Literal["warn", 0, 1],
+            default="warn",
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         kwargs = signature.collect_kwargs()
         return metrics.recall_score(**kwargs)
 
@@ -354,17 +354,17 @@
             name="y_score",
             annotation=npt.ArrayLike,
             condition=DATASPEC | STATIC,
         ),
         SarusParameter(
             name="average",
             annotation=Optional[
-                Literal['micro', 'macro', 'samples', 'weighted']
+                Literal["micro", "macro", "samples", "weighted"]
             ],
-            default='macro',
+            default="macro",
         ),
         SarusParameter(
             name="sample_weight",
             annotation=Optional[npt.ArrayLike],
             default=None,
         ),
         SarusParameter(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/sklearn/svm.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,27 @@
             name="C",
             annotation=float,
             default=1.0,
         ),
         SarusParameter(
             name="kernel",
             annotation=Union[
-                Literal['linear', 'poly', 'rbf', 'sigmoid', 'precomputed'],
+                Literal["linear", "poly", "rbf", "sigmoid", "precomputed"],
                 callable,
             ],
             default="rbf",
         ),
         SarusParameter(
             name="degree",
             annotation=int,
             default=3,
         ),
         SarusParameter(
             name="gamma",
-            annotation=Union[Literal['scale', 'auto'], float],
+            annotation=Union[Literal["scale", "auto"], float],
             default="scale",
         ),
         SarusParameter(
             name="coef0",
             annotation=float,
             default=0.0,
         ),
@@ -80,15 +80,15 @@
         SarusParameter(
             name="max_iter",
             annotation=int,
             default=-1,
         ),
         SarusParameter(
             name="decision_function_shape",
-            annotation=Literal['ovo', 'ovr'],
+            annotation=Literal["ovo", "ovr"],
             default="ovr",
         ),
         SarusParameter(
             name="break_ties",
             annotation=bool,
             default=False,
         ),
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/skopt.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/skopt.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/std.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/std.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     SarusBoundSignature,
     SarusParameter,
     SarusParameterArray,
     SarusParameterMapping,
     SarusSignature,
     SarusSignatureValue,
 )
-from sarus_data_spec.dataspec_validator.typing import PEPKind
+from sarus_data_spec.dataspec_validator.typing import PUPKind
 
 from .external_op import ExternalOpImplementation
 
 
 class add(ExternalOpImplementation):
     _transform_id = "std.ADD"
     _signature = SarusSignature(
@@ -26,16 +26,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this + other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class sub(ExternalOpImplementation):
     _transform_id = "std.SUB"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -48,16 +48,16 @@
         name="substract",
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this - other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class rsub(ExternalOpImplementation):
     _transform_id = "std.RSUB"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -69,16 +69,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return other - this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class mul(ExternalOpImplementation):
     _transform_id = "std.MUL"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -91,16 +91,16 @@
         name="multiply",
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this * other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class div(ExternalOpImplementation):
     _transform_id = "std.DIV"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -112,16 +112,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this / other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class rdiv(ExternalOpImplementation):
     _transform_id = "std.RDIV"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -133,16 +133,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return other / this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class invert(ExternalOpImplementation):
     _transform_id = "std.INVERT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -150,16 +150,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this,) = signature.collect_args()
         return ~this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class length(ExternalOpImplementation):
     _transform_id = "std.LEN"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -186,16 +186,16 @@
         name=_transform_id,
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, key = signature.collect_args()
         return this[key]
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.PEP
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.PUP
 
 
 class setitem(ExternalOpImplementation):
     _transform_id = "std.SETITEM"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -213,20 +213,20 @@
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, key, value = signature.collect_args()
         this[key] = value
         return this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        token_value = bound_signature['value'].pep_token()
-        token_previous = bound_signature['this'].pep_token()
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        token_value = bound_signature["value"].pup_token()
+        token_previous = bound_signature["this"].pup_token()
         if token_value == token_previous:
-            return PEPKind.TOKEN_PRESERVING
-        return PEPKind.NOT_PEP
+            return PUPKind.TOKEN_PRESERVING
+        return PUPKind.NOT_PUP
 
 
 class greater_than(ExternalOpImplementation):
     _transform_id = "std.GT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -238,16 +238,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this > other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class greater_equal(ExternalOpImplementation):
     _transform_id = "std.GE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -259,16 +259,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this >= other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class lower_than(ExternalOpImplementation):
     _transform_id = "std.LT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -280,16 +280,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this < other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class lower_equal(ExternalOpImplementation):
     _transform_id = "std.LE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -301,16 +301,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this <= other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class not_equal(ExternalOpImplementation):
     _transform_id = "std.NE"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -322,16 +322,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this != other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class equal(ExternalOpImplementation):
     _transform_id = "std.EQ"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -343,16 +343,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this == other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class neg(ExternalOpImplementation):
     _transform_id = "std.NEG"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -360,16 +360,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this,) = signature.collect_args()
         return -this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class pos(ExternalOpImplementation):
     _transform_id = "std.POS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -377,16 +377,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this,) = signature.collect_args()
         return +this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class _abs(ExternalOpImplementation):
     _transform_id = "std.ABS"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -394,16 +394,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this,) = signature.collect_args()
         return abs(this)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class _round(ExternalOpImplementation):
     _transform_id = "std.ROUND"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -411,16 +411,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         (this,) = signature.collect_args()
         return round(this)
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class modulo(ExternalOpImplementation):
     _transform_id = "std.MOD"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -432,16 +432,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this % other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class rmodulo(ExternalOpImplementation):
     _transform_id = "std.RMOD"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -453,16 +453,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return other % this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class _or(ExternalOpImplementation):
     _transform_id = "std.OR"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -474,16 +474,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this | other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class ror(ExternalOpImplementation):
     _transform_id = "std.ROR"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -495,16 +495,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return other | this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class _and(ExternalOpImplementation):
     _transform_id = "std.AND"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -516,16 +516,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return this & other
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class rand(ExternalOpImplementation):
     _transform_id = "std.RAND"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
@@ -537,16 +537,16 @@
         ),
     )
 
     def call(self, signature: SarusSignatureValue) -> Any:
         this, other = signature.collect_args()
         return other & this
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        return PEPKind.TOKEN_PRESERVING
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        return PUPKind.TOKEN_PRESERVING
 
 
 class _int(ExternalOpImplementation):
     _transform_id = "std.INT"
     _signature = SarusSignature(
         SarusParameter(
             name="this",
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 from __future__ import annotations
 
 import typing as t
 
 from sarus_data_spec.dataspec_validator.signature import SarusBoundSignature
-from sarus_data_spec.dataspec_validator.typing import PEPKind
+from sarus_data_spec.dataspec_validator.typing import PUPKind
 import sarus_data_spec.typing as st
 
 NO_TRANSFORM_ID = "no_transform_id"
 
 try:
-    from sarus_query_builder.core.core import OptimizableQueryBuilder
+    from sarus_data_spec.sarus_query_builder.core.core import (
+        OptimizableQueryBuilder,
+    )
 except ModuleNotFoundError as e_pandas_dp:
     if "sarus" not in str(e_pandas_dp):
         raise
 
 
 @t.runtime_checkable
 class ExternalOpImplementation(t.Protocol):
     """External Op implementation class.
 
-    The `allowed_pep_args` is a list of combinations of arguments' names which
-    are managed by the Op. The result of the Op will be PEP only if the set of
-    PEP arguments passed to the Op are in this list.
+    The `allowed_pup_args` is a list of combinations of arguments' names which
+    are managed by the Op. The result of the Op will be PUP only if the set of
+    PUP arguments passed to the Op are in this list.
 
     For instance, if we have an op that takes 3 arguments `a`, `b` and `c` and
-    the `allowed_pep_args` are [{'a'}, {'b'}, {'a','b'}] then the following
-    combinations will yield a PEP output:
-        - `a` is a PEP dataspec, `b` and `c` are either not dataspecs or public
+    the `allowed_pup_args` are [{'a'}, {'b'}, {'a','b'}] then the following
+    combinations will yield a PUP output:
+        - `a` is a PUP dataspec, `b` and `c` are either not dataspecs or public
           dataspecs
-        - `b` is a PEP dataspec, `a` and `c` are either not dataspecs or public
+        - `b` is a PUP dataspec, `a` and `c` are either not dataspecs or public
           dataspecs
-        - `a` and `b` are PEP dataspecs, `c` is either not a dataspec or a
+        - `a` and `b` are PUP dataspecs, `c` is either not a dataspec or a
           public dataspec
     """
 
-    def transform_id(self) -> str:
-        ...
+    def transform_id(self) -> str: ...
 
-    def dp_equivalent_id(self) -> t.Optional[str]:
-        ...
+    def dp_equivalent_id(self) -> t.Optional[str]: ...
 
-    def dp_equivalent(self) -> t.Optional[ExternalOpImplementation]:
-        ...
+    def dp_equivalent(self) -> t.Optional[ExternalOpImplementation]: ...
 
     async def call(self, bound_signature: SarusBoundSignature) -> t.Any:
         """Compute the external op output value.
 
         DP implementation take additional arguments:
             - `seed` an integer used to parametrize rangom number generators
             - `budget` the privacy budget that can be spend in the op
             - `pe` the protected entity information of each row
         """
 
-    def pep_kind(self, bound_signature: SarusBoundSignature) -> PEPKind:
-        """Return the PEP properties of the transform.
+    def pup_kind(self, bound_signature: SarusBoundSignature) -> PUPKind:
+        """Return the PUP properties of the transform.
 
         It takes the transform arguments as input because it can depend on some
-        transform parameters. For instance, it is not PEP if we are aggregating
-        the rows (axis=0) and it is PEP if we are aggregating the columns
+        transform parameters. For instance, it is not PUP if we are aggregating
+        the rows (axis=0) and it is PUP if we are aggregating the columns
         (axis=1).
         """
 
     def is_dp(self, bound_signature: SarusBoundSignature) -> bool:
         """Return True if the DP transform is compatible with the arguments.
 
         It takes the transform arguments as input because it can depend on some
@@ -73,9 +72,8 @@
     async def private_queries(
         self, signature: SarusBoundSignature
     ) -> t.List[st.PrivateQuery]:
         """Return the PrivateQueries summarizing DP characteristics."""
 
     async def query_builder(
         self, signature: SarusBoundSignature
-    ) -> OptimizableQueryBuilder:
-        ...
+    ) -> OptimizableQueryBuilder: ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/external/xgboost.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/external/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/routing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,17 +102,17 @@
     logger.info("Transforms: SelectSQL not available.")
 from sarus_data_spec.manager.ops.processor.standard.shuffle import (
     Shuffle,
     ShuffleStaticChecker,
 )
 
 try:
-    from sarus_data_spec.manager.ops.processor.standard.protection_utils.protected_paths import (  # noqa: E501
-        ProtectedPaths,
-        ProtectedPathsStaticChecker,
+    from sarus_data_spec.manager.ops.processor.standard.protection_utils.privacy_unit_tracking_paths import (  # noqa: E501
+        PrivacyUnitTrackingPaths,
+        PrivacyUnitTrackingStaticChecker,
         PublicPaths,
         PublicPathStaticChecker,
     )
     from sarus_data_spec.manager.ops.processor.standard.protection_utils.protection import (  # noqa: E501
         ProtectedDataset,
         ProtectedDatasetStaticChecker,
     )
@@ -219,84 +219,84 @@
 
 
 def get_dataset_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[DatasetImplementation], t.Type[DatasetStaticChecker]]:
     if transform.is_external():
         return ExternalDatasetOp, ExternalDatasetStaticChecker
-    elif transform.spec() == 'sample':
+    elif transform.spec() == "sample":
         return Sample, SampleStaticChecker
-    elif transform.spec() == 'differentiated_sample':
+    elif transform.spec() == "differentiated_sample":
         return DifferentiatedSample, DifferentiatedSampleStaticChecker
-    elif transform.spec() == 'to_small_data':
+    elif transform.spec() == "to_small_data":
         return ToSmallData, ToSmallDataStaticChecker
-    elif transform.spec() == 'protect_dataset':
+    elif transform.spec() == "privacy_unit_tracking":
         return ProtectedDataset, ProtectedDatasetStaticChecker
-    elif transform.spec() == 'user_settings':
+    elif transform.spec() == "user_settings":
         return UserSettingsDataset, UserSettingsStaticChecker
-    elif transform.spec() == 'filter':
+    elif transform.spec() == "filter":
         return Filter, FilterStaticChecker
-    elif transform.spec() == 'project':
+    elif transform.spec() == "project":
         return Project, ProjectStaticChecker
-    elif transform.spec() == 'shuffle':
+    elif transform.spec() == "shuffle":
         return Shuffle, ShuffleStaticChecker
-    elif transform.spec() == 'synthetic':
+    elif transform.spec() == "synthetic":
         return Synthetic, SyntheticStaticChecker
-    elif transform.spec() == 'get_item':
+    elif transform.spec() == "get_item":
         return GetItem, GetItemStaticChecker
-    elif transform.spec() == 'assign_budget':
+    elif transform.spec() == "assign_budget":
         return AssignBudget, AssignBudgetStaticChecker
-    elif transform.spec() == 'group_by_pe':
+    elif transform.spec() == "group_by_pe":
         return GroupByPE, GroupByPEStaticChecker
-    elif transform.name() == 'Transcode':
+    elif transform.name() == "Transcode":
         return Transcode, TranscodeStaticChecker
-    elif transform.spec() == 'select_sql':
+    elif transform.spec() == "select_sql":
         return SelectSQL, SelectSQLStaticChecker
-    elif transform.spec() == 'dp_select_sql':
+    elif transform.spec() == "dp_select_sql":
         return DPSelectSQL, DPSelectSQLStaticChecker
-    elif transform.spec() == 'extract':
+    elif transform.spec() == "extract":
         return Extract, ExtractStaticChecker
-    elif transform.spec() == 'generate_from_model':
+    elif transform.spec() == "generate_from_model":
         return GenerateFromModel, GenerateFromModelStaticChecker
     else:
         raise NotImplementedError(transform.spec())
 
 
 def get_scalar_op(
     transform: st.Transform,
 ) -> t.Tuple[t.Type[ScalarImplementation], t.Type[DataspecStaticChecker]]:
     if transform.is_external():
         return ExternalScalarOp, ExternalScalarStaticChecker
-    elif transform.name() == 'automatic_protected_paths':
+    elif transform.name() == "automatic_privacy_unit_tracking_paths":
         # here we assume this transform is called
         # on a single dataset
-        return ProtectedPaths, ProtectedPathsStaticChecker
-    elif transform.name() == 'automatic_public_paths':
+        return PrivacyUnitTrackingPaths, PrivacyUnitTrackingStaticChecker
+    elif transform.name() == "automatic_public_paths":
         # here we assume this transform is called
         # on a single dataset
         return PublicPaths, PublicPathStaticChecker
-    elif transform.name() == 'automatic_user_settings':
+    elif transform.name() == "automatic_user_settings":
         return AutomaticUserSettings, AutomaticUserSettingsStaticChecker
-    elif transform.name() == 'automatic_budget':
+    elif transform.name() == "automatic_budget":
         return AutomaticBudget, AutomaticBudgetStaticChecker
-    elif transform.name() == 'attributes_budget':
+    elif transform.name() == "attributes_budget":
         return AttributesBudget, AttributesBudgetStaticChecker
-    elif transform.name() == 'sd_budget':
+    elif transform.name() == "sd_budget":
         return SDBudget, SDBudgetStaticChecker
-    elif transform.name() == 'derive_seed':
+    elif transform.name() == "derive_seed":
         return DeriveSeed, DeriveSeedStaticChecker
-    elif transform.name() == 'relationship_spec':
+    elif transform.name() == "relationship_spec":
         return RelationshipSpecOp, RelationshipSpecOpStaticChecker
-    elif transform.name() == 'validated_user_type':
+    elif transform.name() == "validated_user_type":
         return ValidatedUserTypeOp, ValidatedUserTypeOpStaticChecker
-    elif transform.spec() == 'error_estimation':
+    elif transform.spec() == "error_estimation":
         return ErrorEstimation, ErrorEstimationStaticChecker
-    elif transform.name() == 'fit_model':
+    elif transform.name() == "fit_model":
         return FitModel, FitModelStaticChecker
-    elif transform.name() == 'fit_model_dp':
+    elif transform.name() == "fit_model_dp":
         return FitModelDP, FitModelDPStaticChecker
     else:
         raise NotImplementedError(f"scalar_transformed for {transform}")
 
 
 def get_op(
     dataspec: st.DataSpec,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/differentiated_sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,29 @@
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 try:
     import sqlalchemy as sa
 except ModuleNotFoundError:
-    warnings.warn('sqlalchemy not installed. No sampling on bigdata')
+    warnings.warn("sqlalchemy not installed. No sampling on bigdata")
 
 try:
     from sarus_data_spec.manager.ops.processor.standard.sampling.differentiated_sampling_sizes import (  # noqa: E501
         differentiated_sampling_sizes,
     )
     from sarus_data_spec.manager.ops.processor.standard.sampling.size_utils import (  # noqa: E501
         differentiated_sampled_size,
         sampled_size,
     )
 except ModuleNotFoundError as exception:
     # for the public repo
     if (
         exception.name
-        == 'sarus_data_spec.manager.ops.processor.standard.sampling'  # noqa: E501
+        == "sarus_data_spec.manager.ops.processor.standard.sampling"  # noqa: E501
     ):
         pass
     else:
         raise exception
 
 try:
     from sarus_data_spec.manager.ops.sql_utils.bigdata import (
@@ -55,24 +55,24 @@
         sqlalchemy_query_to_string,
     )
     from sarus_data_spec.manager.ops.sql_utils.queries import nest_queries
     from sarus_data_spec.manager.ops.sql_utils.schema_translations import (
         async_sa_metadata_from_dataset,
     )
 except ModuleNotFoundError:
-    warnings.warn('sql utils not installed.')
+    warnings.warn("sql utils not installed.")
 
 
 class DifferentiatedSampleStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.type(),
-            protected_paths=parent_schema.protobuf().protected,
+            privacy_unit_tracking_paths=parent_schema.protobuf().privacy_unit,
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class DifferentiatedSample(StandardDatasetImplementation):
     """Computes schema and arrow
@@ -215,15 +215,14 @@
             ).to_batches(max_chunksize=1000),
             batch_size=batch_size,
         )
 
     async def sql_implementation(
         self,
     ) -> t.Optional[t.Dict[t.Tuple[str, ...], str]]:
-
         schema = await self.parent_schema()
         previous_size = await self.parent_size()
         size_dict = await differentiated_sampling_sizes(self.dataset)
         assert previous_size
         previous_stats = previous_size.statistics()
         sqlalchemy_metadata = await async_sa_metadata_from_dataset(
             self.dataset
@@ -239,15 +238,15 @@
                 straight_path(full_tablename)
             )
             sa_table = sqlalchemy_metadata.tables[sa_table_name]
             sample_size = size_dict[table_path]
             if (
                 self.dataset.transform()
                 .protobuf()
-                .spec.differentiated_sample.HasField('fraction')
+                .spec.differentiated_sample.HasField("fraction")
             ):
                 fraction = (
                     self.dataset.transform()
                     .protobuf()
                     .spec.differentiated_sample.fraction
                 )
                 sample_query = sa.select(sa_table).where(
@@ -285,33 +284,31 @@
     stat: st.Statistics,
     selected_indices: pa.Array,
     new_size_dict: t.Dict[st.Path, int],
     random_gen: np.random.Generator,
     curr_path: t.List[str],
 ) -> pa.Array:
     class IndicesSampler(st.StatisticsVisitor):
-
         indices: pa.Array = selected_indices
         batch_array: pa.Array = array
 
         def Union(
             self,
             fields: t.Mapping[str, st.Statistics],
             size: int,
             multiplicity: float,
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
-
             new_indices = []
             for field, field_stat in fields.items():
                 index_element = self.batch_array.type.get_field_index(field)
                 filter_idex = pa.array(
                     np.equal(
-                        self.batch_array.field('field_selected'),
+                        self.batch_array.field("field_selected"),
                         np.array(field),
                     )
                 )
                 updated_indices = sample_indices_from_array(
                     self.batch_array.filter(filter_idex).flatten()[
                         index_element
                     ],
@@ -328,15 +325,14 @@
             self,
             fields: t.Mapping[str, st.Statistics],
             size: int,
             multiplicity: float,
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
-
             # sample indices to size and sample ratio
             new_size = new_size_dict[straight_path(curr_path.copy())]
             self.indices = pa.array(
                 random_gen.choice(
                     self.indices,
                     replace=False,
                     size=min(new_size, size, len(array)),
@@ -377,15 +373,15 @@
         def Enum(
             self,
             size: int,
             multiplicity: float,
             probabilities: t.Optional[t.List[float]] = None,
             names: t.Optional[t.List[str]] = None,
             values: t.Optional[t.List[float]] = None,
-            name: str = 'Enum',
+            name: str = "Enum",
         ) -> None:
             raise NotImplementedError
 
         def Float(
             self,
             size: int,
             multiplicity: float,
@@ -398,15 +394,15 @@
 
         def Text(
             self,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            example: str = '',
+            example: str = "",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Bytes(self, size: int, multiplicity: float) -> None:
             raise NotImplementedError
@@ -419,28 +415,28 @@
         def List(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            name: str = 'List',
+            name: str = "List",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Array(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_values: t.Optional[t.List[float]] = None,
             max_values: t.Optional[t.List[float]] = None,
-            name: str = 'Array',
+            name: str = "Array",
             probabilities: t.Optional[t.List[t.List[float]]] = None,
             values: t.Optional[t.List[t.List[float]]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Datetime(
             self,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/error_estimation.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/error_estimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
     StandardScalarImplementation,
     StandardScalarStaticChecker,
 )
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
-class ErrorEstimationStaticChecker(StandardScalarStaticChecker):
-    ...
+class ErrorEstimationStaticChecker(StandardScalarStaticChecker): ...
 
 
 class ErrorEstimation(StandardScalarImplementation):
     """Computes the budget via standard rule
     depending on the number of columns of the
     parent dataspec"""
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/extract.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/extract.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class ExtractStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.type(),
-            protected_paths=None,
+            privacy_unit_tracking_paths=None,
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Extract(StandardDatasetImplementation):
     """Computes schema and arrow
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/filter.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 class FilterStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         new_type = sdt.Type(
             self.dataset.transform().protobuf().spec.filter.filter
         )
         new_type = update_fks(
-            curr_type=new_type, original_type=new_type  # type:ignore
+            curr_type=new_type,
+            original_type=new_type,  # type:ignore
         )
         old_properties = parent_schema.properties()
 
         if PRIMARY_KEYS in old_properties.keys():
             new_pks = filter_primary_keys(
                 old_properties[PRIMARY_KEYS],
                 new_type,
@@ -50,15 +51,15 @@
         previous_fields = parent_schema.type().children()
         if DATA in previous_fields.keys():
             previous_fields[DATA] = new_type.data_type()
             new_type = sdt.Struct(fields=previous_fields)
         return schema(
             self.dataset,
             schema_type=new_type,
-            protected_paths=None,
+            privacy_unit_tracking_paths=None,
             properties=old_properties,
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Filter(StandardDatasetImplementation):
     """Computes schema and arrow
@@ -198,15 +199,15 @@
                 )
                 for fieldname, fieldtype in children_type.items()
             }
             self.result = sds.Union(
                 fields=new_fields,
                 size=size,
                 multiplicity=multiplicity,
-                name=name if name is not None else 'Union',
+                name=name if name is not None else "Union",
                 properties=self.result.properties(),
             )
 
         def Optional(
             self, statistics: st.Statistics, size: int, multiplicity: float
         ) -> None:
             self.result = sds.Optional(
@@ -252,15 +253,15 @@
         def Enum(
             self,
             size: int,
             multiplicity: float,
             probabilities: t.Optional[t.List[float]] = None,
             names: t.Optional[t.List[str]] = None,
             values: t.Optional[t.List[float]] = None,
-            name: str = 'Enum',
+            name: str = "Enum",
         ) -> None:
             pass
 
         def Float(
             self,
             size: int,
             multiplicity: float,
@@ -273,15 +274,15 @@
 
         def Text(
             self,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            example: str = '',
+            example: str = "",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             pass
 
         def Bytes(self, size: int, multiplicity: float) -> None:
             pass
@@ -289,28 +290,28 @@
         def List(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            name: str = 'List',
+            name: str = "List",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Array(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_values: t.Optional[t.List[float]] = None,
             max_values: t.Optional[t.List[float]] = None,
-            name: str = 'Array',
+            name: str = "Array",
             probabilities: t.Optional[t.List[t.List[float]]] = None,
             values: t.Optional[t.List[t.List[float]]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Datetime(
             self,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/generate_from_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing as t
 import warnings
 
 try:
     from sarus_llm.torch_interface.sample import TextSampler
     from sarus_llm.torch_interface.typing import ModelProvider
 except (ModuleNotFoundError, ValueError, RuntimeError):
-    warnings.warn('Sarus LLM not available')
+    warnings.warn("Sarus LLM not available")
 
 import pyarrow as pa
 
 from sarus_data_spec.constants import PUBLIC
 from sarus_data_spec.dataset import Dataset
 from sarus_data_spec.manager.ops.processor.standard.standard_op import (  # noqa: E501
     StandardDatasetImplementation,
@@ -46,15 +46,17 @@
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         _, kwargs = self.dataset.parents()
         pretrained_model = kwargs["model"]
         prompts = kwargs["prompts"]
         transform = self.dataset.transform()
 
-        assert pretrained_model.prototype() == sp.Scalar, "pretrained model should be a Scalar"  # type: ignore # noqa: E501
+        assert (
+            pretrained_model.prototype() == sp.Scalar  # type: ignore # noqa: E501
+        ), "pretrained model should be a Scalar"
         pretrained_ds = t.cast(st.Scalar, pretrained_model)
         model_provider = t.cast(
             ModelProvider, await pretrained_ds.async_value()
         )
 
         assert prompts.prototype() == sp.Dataset, "prompts should be a Dataset"
         prompts_ds = t.cast(st.Dataset, prompts)
@@ -66,16 +68,16 @@
             temperature=specs.temperature,
             max_new_tokens=specs.max_new_tokens,
         )
 
         async def async_iterator() -> t.AsyncIterator[pa.RecordBatch]:
             async for batch in await prompts_ds.async_to_arrow(batch_size):
                 text_samples = pa.array(
-                    sampler.generate(prompts=batch.to_pydict()['prompt'])
+                    sampler.generate(prompts=batch.to_pydict()["prompt"])
                 )
                 yield pa.RecordBatch.from_struct_array(
                     pa.StructArray.from_arrays(
-                        arrays=[text_samples], names=['text']
+                        arrays=[text_samples], names=["text"]
                     )
                 )
 
         return async_iterator()
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/get_item.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/get_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 try:
     import sqlalchemy as sa
 except ModuleNotFoundError:
-    warnings.warn('sqlalchemy not installed. No sampling on bigdata')
+    warnings.warn("sqlalchemy not installed. No sampling on bigdata")
 
 try:
     from sarus_data_spec.manager.ops.sql_utils.bigdata import (
         path_to_quoted_string,
         sqlalchemy_query_to_string,
     )
     from sarus_data_spec.manager.ops.sql_utils.schema_translations import (
         async_sa_metadata_from_dataset,
     )
 except ModuleNotFoundError:
-    warnings.warn('sql utils not installed.')
+    warnings.warn("sql utils not installed.")
 
 
 class GetItemStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         path = Path(self.dataset.transform().protobuf().spec.get_item.path)
         sub_types = parent_schema.data_type().sub_types(path)
@@ -60,15 +60,15 @@
             properties = {}
         if DATA in previous_fields.keys():
             previous_fields[DATA] = new_type
             new_type = sdt.Struct(fields=previous_fields)
         return schema(
             self.dataset,
             schema_type=new_type,
-            protected_paths=None,
+            privacy_unit_tracking_paths=None,
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
             properties=properties,
         )
 
 
 class GetItem(StandardDatasetImplementation):
     """Computes schema and arrow
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/project.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,45 +24,46 @@
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.statistics as sds
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 
 class ProjectStaticChecker(StandardDatasetStaticChecker):
-    def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        """This transform doesn't change the PEP alignment."""
-        return self.parent().pep_token()
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        """This transform doesn't change the PUP alignment."""
+        return self.parent().pup_token()
 
-    def rewritten_pep_token(
+    def rewritten_pup_token(
         self, public_context: t.Collection[str]
     ) -> t.Optional[str]:
-        """This transform doesn't change the PEP alignment."""
-        return self.parent().rewritten_pep_token()
+        """This transform doesn't change the PUP alignment."""
+        return self.parent().rewritten_pup_token()
 
     async def schema(self) -> st.Schema:
         new_type = sdt.Type(
             self.dataset.transform().protobuf().spec.project.projection
         )
         parent_schema = await self.parent_schema()
         new_type = update_fks(
-            curr_type=new_type, original_type=new_type  # type:ignore
+            curr_type=new_type,
+            original_type=new_type,  # type:ignore
         )
         old_properties = parent_schema.properties()
 
         if PRIMARY_KEYS in old_properties.keys():
             new_pks = filter_primary_keys(
                 old_properties[PRIMARY_KEYS],
                 new_type,
             )
             old_properties[PRIMARY_KEYS] = new_pks  # type:ignore
 
         return schema(
             self.dataset,
             schema_type=new_type,
-            protected_paths=None,
+            privacy_unit_tracking_paths=None,
             properties=old_properties,
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Project(StandardDatasetImplementation):
     """Computes schema and arrow
@@ -177,15 +178,15 @@
                 )
                 for fieldname, fieldstats in self.result.children().items()
             }
             self.result = sds.Union(
                 fields=new_fields,
                 size=size,
                 multiplicity=multiplicity,
-                name=name if name is not None else 'Union',
+                name=name if name is not None else "Union",
                 properties=self.result.properties(),
             )
 
         def Optional(
             self, statistics: st.Statistics, size: int, multiplicity: float
         ) -> None:
             self.result = sds.Optional(
@@ -231,15 +232,15 @@
         def Enum(
             self,
             size: int,
             multiplicity: float,
             probabilities: t.Optional[t.List[float]] = None,
             names: t.Optional[t.List[str]] = None,
             values: t.Optional[t.List[float]] = None,
-            name: str = 'Enum',
+            name: str = "Enum",
         ) -> None:
             pass
 
         def Float(
             self,
             size: int,
             multiplicity: float,
@@ -252,15 +253,15 @@
 
         def Text(
             self,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            example: str = '',
+            example: str = "",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             pass
 
         def Bytes(self, size: int, multiplicity: float) -> None:
             pass
@@ -268,28 +269,28 @@
         def List(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_value: int,
             max_value: int,
-            name: str = 'List',
+            name: str = "List",
             probabilities: t.Optional[t.List[float]] = None,
             values: t.Optional[t.List[int]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Array(
             self,
             statistics: st.Statistics,
             size: int,
             multiplicity: float,
             min_values: t.Optional[t.List[float]] = None,
             max_values: t.Optional[t.List[float]] = None,
-            name: str = 'Array',
+            name: str = "Array",
             probabilities: t.Optional[t.List[t.List[float]]] = None,
             values: t.Optional[t.List[t.List[float]]] = None,
         ) -> None:
             raise NotImplementedError
 
         def Datetime(
             self,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sample.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,45 +20,47 @@
 from sarus_data_spec.schema import schema
 from sarus_data_spec.size import size as size_builder
 import sarus_data_spec.typing as st
 
 try:
     import sqlalchemy as sa
 except ModuleNotFoundError:
-    warnings.warn('sqlalchemy not installed. No sampling on bigdata')
+    warnings.warn("sqlalchemy not installed. No sampling on bigdata")
 
 try:
-    from sarus_statistics.tasks.size.sample_visitor import sampled_size
+    from sarus_data_spec.sarus_statistics.tasks.size.sample_visitor import (
+        sampled_size,
+    )
 except ModuleNotFoundError as exception:
     # for the public repo
-    if 'sarus_statistics' in str(exception.name):
+    if "sarus_data_spec.sarus_statistics" in str(exception.name):
         pass
     else:
         raise exception
 
 try:
     from sarus_data_spec.manager.ops.sql_utils.bigdata import (
         path_to_quoted_string,
         sqlalchemy_query_to_string,
     )
     from sarus_data_spec.manager.ops.sql_utils.queries import nest_queries
     from sarus_data_spec.manager.ops.sql_utils.schema_translations import (
         async_sa_metadata_from_dataset,
     )
 except ModuleNotFoundError:
-    warnings.warn('sql utils not installed.')
+    warnings.warn("sql utils not installed.")
 
 
 class SampleStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.type(),
-            protected_paths=parent_schema.protobuf().protected,
+            privacy_unit_tracking_paths=parent_schema.protobuf().privacy_unit,
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Sample(StandardDatasetImplementation):
     """Computes schema and arrow
@@ -126,22 +128,19 @@
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         return await sample_arrow_to_arrow(self, batch_size)
 
     async def sql_implementation(
         self,
     ) -> t.Optional[t.Dict[t.Tuple[str, ...], str]]:
-
         schema = await self.dataset.async_schema()
         parent_ds = t.cast(Dataset, self.parent())
         sample_spec = getattr(
             self.dataset.transform().protobuf().spec,
-            self.dataset.transform()
-            .protobuf()
-            .spec.WhichOneof('spec'),  # type: ignore[arg-type]
+            self.dataset.transform().protobuf().spec.WhichOneof("spec"),  # type: ignore[arg-type]
         )
 
         previous_size = await parent_ds.manager().async_size(parent_ds)
         assert previous_size
         previous_stats = previous_size.statistics()
 
         sqlalchemy_metadata = await async_sa_metadata_from_dataset(
@@ -154,15 +153,15 @@
             full_tablename = (
                 curr_path[1:] if curr_path[0] == DATA else curr_path
             )
             sa_table_name = path_to_quoted_string(
                 straight_path(full_tablename)
             )
             sa_table = sqlalchemy_metadata.tables[sa_table_name]
-            if sample_spec.HasField('fraction'):
+            if sample_spec.HasField("fraction"):
                 fraction = sample_spec.fraction
                 sample_query = sa.select(sa_table).where(
                     sa.func.random() < fraction
                 )
             else:
                 sample_query = (
                     sa.select(sa_table)
@@ -199,35 +198,35 @@
 
 def new_sampling_ratio(
     dataset: st.Dataset, statistics: st.Statistics
 ) -> float:
     """From a transformed dataset which last transform is sample or
     differentiated_sample, get sampling ratio"""
     spec = dataset.transform().protobuf().spec
-    transform_type = spec.WhichOneof('spec')
+    transform_type = spec.WhichOneof("spec")
     assert transform_type
     sampling_spec = getattr(spec, transform_type)
-    if sampling_spec.HasField('fraction'):
+    if sampling_spec.HasField("fraction"):
         return t.cast(float, sampling_spec.fraction)
     return t.cast(float, sampling_spec.size / statistics.size())
 
 
 async def sample_arrow_to_arrow(
     op: StandardDatasetImplementation, batch_size: int
 ) -> t.AsyncIterator[pa.RecordBatch]:
     spec = op.dataset.transform().protobuf().spec
-    transform_type = spec.WhichOneof('spec')
+    transform_type = spec.WhichOneof("spec")
     assert transform_type
     sampling_spec = getattr(spec, transform_type)
     seed = Scalar(sampling_spec.seed).value()
     generator = np.random.default_rng(seed)
     parent_batches = [batch async for batch in await op.parent_to_arrow()]
     parent_table = pa.Table.from_batches(parent_batches)
 
-    if sampling_spec.HasField('fraction'):
+    if sampling_spec.HasField("fraction"):
         new_size = int(sampling_spec.fraction * parent_table.num_rows)
     else:
         new_size = sampling_spec.size
 
     parent_size = await op.parent_size()
     if new_size >= parent_size.statistics().size():
         return await op.parent_to_arrow(batch_size)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/sampling/differentiated_sampling_sizes.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ) -> Dict[st.Path, int]:
     """Get the sampling rates for each table"""
     parent_ds = cast(Dataset, dataset.parents()[0][0])
     parent_size = await parent_ds.manager().async_size(parent_ds)
     assert parent_size
 
     transform = dataset.transform().protobuf().spec.differentiated_sample
-    if transform.HasField('fraction'):
+    if transform.HasField("fraction"):
         sampled_size = parent_size.statistics().size() * transform.fraction
     else:
         sampled_size = transform.size
 
     return await differentiated_sampling_sizes_bisection(
         parent_ds, int(sampled_size)
     )
@@ -83,15 +83,14 @@
         **public_table_path_sizes,
     }
 
 
 def sync_bisection(
     size_stat: st.Statistics, table_paths: List[st.Path], sampled_size: int
 ) -> Dict[st.Path, int]:
-
     table_path_sizes = {
         table_path: size_stat.nodes_statistics(table_path)[0].size()
         for table_path in table_paths
     }
 
     def new_size(max_table_size: float) -> int:
         return int(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/shuffle.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/shuffle.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class ShuffleStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.type(),
-            protected_paths=None,
+            privacy_unit_tracking_paths=None,
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Shuffle(StandardDatasetImplementation):
     """Computes schema and arrow
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/standard_op.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/standard_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,68 +9,69 @@
 from sarus_data_spec.manager.ops.base import (
     DatasetImplementation,
     DatasetStaticChecker,
     DataspecStaticChecker,
     ScalarImplementation,
     _ensure_batch_correct,
 )
+from sarus_data_spec.typing import Path
 
 try:
     from sarus_data_spec.manager.ops.sql_utils.table_mapping import (
         name_encoder,
         table_mapping,
     )
 except ModuleNotFoundError:
-    warnings.warn('table_mapping not found. Cannot send sql queries.')
+    warnings.warn("table_mapping not found. Cannot send sql queries.")
 try:
     from sarus_data_spec.manager.ops.sql_utils.queries import (
         rename_and_compose_queries,
     )
 except ModuleNotFoundError:
-    warnings.warn('Queries composition not available.')
+    warnings.warn("Queries composition not available.")
 from sarus_data_spec.scalar import Scalar
 import sarus_data_spec.typing as st
 
 logger = logging.getLogger(__name__)
 
 
 class StandardDatasetStaticChecker(DatasetStaticChecker):
-    def parent(self, kind: str = 'dataset') -> t.Union[st.Dataset, st.Scalar]:
+    def parent(self, kind: str = "dataset") -> t.Union[st.Dataset, st.Scalar]:
         return parent(self.dataset, kind=kind)
 
     async def parent_schema(self) -> st.Schema:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_schema(parent)
 
     async def parent_marginals(self) -> st.Marginals:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_marginals(parent)
 
-    def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        """By default we implement that the transform inherits the PEP status
-        but changes the PEP token."""
-        parent_token = self.parent().pep_token()
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        """By default we implement that the transform inherits the PUP status
+        but changes the PUP token."""
+        parent_token = self.parent().pup_token()
         if parent_token is None:
             return None
 
         transform = self.dataset.transform()
         h = hashlib.md5(usedforsecurity=False)
         h.update(parent_token.encode("ascii"))
         h.update(transform.protobuf().SerializeToString())
 
         return h.hexdigest()
 
-    def rewritten_pep_token(
+    def rewritten_pup_token(
         self, public_context: t.Collection[str]
     ) -> t.Optional[str]:
-        """By default we implement that the transform inherits the PEP status
-        but changes the PEP token."""
-        parent_token = self.parent().rewritten_pep_token()
+        """By default we implement that the transform inherits the PUP status
+        but changes the PUP token."""
+        parent_token = self.parent().rewritten_pup_token()
         if parent_token is None:
             return None
 
         transform = self.dataset.transform()
         h = hashlib.md5(usedforsecurity=False)
         h.update(parent_token.encode("ascii"))
         h.update(transform.protobuf().SerializeToString())
@@ -82,54 +83,54 @@
     """Object that executes first routing among ops between
     transformed/source and processor
     """
 
     def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
         return parents(self.dataset)
 
-    def parent(self, kind: str = 'dataset') -> t.Union[st.Dataset, st.Scalar]:
+    def parent(self, kind: str = "dataset") -> t.Union[st.Dataset, st.Scalar]:
         return parent(self.dataset, kind=kind)
 
     async def parent_to_arrow(
         self, batch_size: int = 10000
     ) -> t.AsyncIterator[pa.RecordBatch]:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         parent_iterator = await parent.manager().async_to_arrow(
             parent, batch_size=batch_size
         )
         return await self.decoupled_async_iter(parent_iterator)
 
     async def parent_schema(self) -> st.Schema:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_schema(parent)
 
     async def parent_value(self) -> t.Any:
-        parent = self.parent(kind='scalar')
+        parent = self.parent(kind="scalar")
         assert isinstance(parent, Scalar)
         return await parent.manager().async_value(parent)
 
     async def parent_size(self) -> st.Size:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_size(parent)
 
     async def parent_multiplicity(self) -> st.Multiplicity:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_multiplicity(parent)
 
     async def parent_bounds(self) -> st.Bounds:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_bounds(parent)
 
     async def parent_marginals(self) -> st.Marginals:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_marginals(parent)
 
     async def ensure_batch_correct(
         self,
         async_iterator: t.AsyncIterator[pa.RecordBatch],
         func_to_apply: t.Callable,
@@ -167,21 +168,24 @@
         parent_schema = await self.parent_schema()
         if (
             queries_transform is None
             and current_schema.name() == parent_schema.name()
         ):
             parent_query = query
         else:
-            table_map = {}
+            table_map: dict[Path, tuple[str, ...]] = {}
             if queries_transform is not None:
-                table_map = table_mapping(
-                    tables=current_schema.tables(),
-                    sarus_schema_name=current_schema.name(),
-                    encoded_name_length=10,
-                    encoder_prefix_name=self.dataset.uuid(),
+                table_map = t.cast(
+                    dict[Path, tuple[str, ...]],
+                    table_mapping(
+                        tables=current_schema.tables(),
+                        sarus_schema_name=current_schema.name(),
+                        encoded_name_length=10,
+                        encoder_prefix_name=self.dataset.uuid(),
+                    ),
                 )
             updated_queries_transform = (
                 {
                     name_encoder(
                         names=(self.dataset.uuid(), *tab_name),
                         length=10,
                     ): query_str
@@ -194,63 +198,62 @@
             parent_query = rename_and_compose_queries(
                 query_or_dict=query,
                 curr_path=[],
                 queries_transform=updated_queries_transform,
                 table_map=table_map,
             )
 
-        parent_ds = t.cast(st.Dataset, self.parent(kind='dataset'))
+        parent_ds = t.cast(st.Dataset, self.parent(kind="dataset"))
         logger.info(
             f"query {parent_query} sent to the "
             f"parent dataset {parent_ds.uuid()}"
         )
         return await parent_ds.manager().async_sql(
             dataset=parent_ds,
             query=parent_query,
             dialect=dialect,
             batch_size=batch_size,
             result_type=result_type,
         )
 
 
-class StandardScalarStaticChecker(DataspecStaticChecker):
-    ...
+class StandardScalarStaticChecker(DataspecStaticChecker): ...
 
 
 class StandardScalarImplementation(ScalarImplementation):
-    def parent(self, kind: str = 'dataset') -> st.DataSpec:
+    def parent(self, kind: str = "dataset") -> st.DataSpec:
         return parent(self.scalar, kind=kind)
 
     def parents(self) -> t.List[t.Union[st.DataSpec, st.Transform]]:
         return parents(self.scalar)
 
     async def parent_to_arrow(
         self, batch_size: int = 10000
     ) -> t.AsyncIterator[pa.RecordBatch]:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         parent_iterator = await parent.manager().async_to_arrow(
             parent, batch_size=batch_size
         )
         return await self.decoupled_async_iter(parent_iterator)
 
     async def parent_schema(self) -> st.Schema:
-        parent = self.parent(kind='dataset')
+        parent = self.parent(kind="dataset")
         assert isinstance(parent, Dataset)
         return await parent.manager().async_schema(parent)
 
     async def parent_value(self) -> t.Any:
-        parent = self.parent(kind='scalar')
+        parent = self.parent(kind="scalar")
         assert isinstance(parent, Scalar)
         return await parent.manager().async_value(parent)
 
 
 def parent(dataspec: st.DataSpec, kind: str) -> t.Union[st.Dataset, st.Scalar]:
     pars = parents(dataspec)
-    if kind == 'dataset':
+    if kind == "dataset":
         parent: t.Union[t.List[Scalar], t.List[Dataset]] = [
             element for element in pars if isinstance(element, Dataset)
         ]
     else:
         parent = [element for element in pars if isinstance(element, Scalar)]
     assert len(parent) == 1
     return parent[0]
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/synthetic.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/synthetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 [
                     pa.field(name, type=arr.type)
                     for arr, name in zip(arrs[:-1], names)
                 ]
             )
             schema = schema.append(
                 pa.field(
-                    'field_selected', type=pa.large_string(), nullable=False
+                    "field_selected", type=pa.large_string(), nullable=False
                 )
             )
             self.result = pa.Table.from_arrays(
                 arrays=arrow_data.flatten(), schema=schema
             )
 
         def Null(
@@ -247,56 +247,56 @@
     """Async generator from the synthetic data iterator."""
     for batch in iterator:
         yield batch
     return
 
 
 class SyntheticStaticChecker(StandardDatasetStaticChecker):
-    def pep_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
-        # TODO add pep token when the synthetic data is actually protected
+    def pup_token(self, public_context: t.Collection[str]) -> t.Optional[str]:
+        # TODO add pup token when the synthetic data is actually protected
         return None
 
-    def rewritten_pep_token(
+    def rewritten_pup_token(
         self, public_context: t.Collection[str]
     ) -> t.Optional[str]:
-        # TODO add pep token when the synthetic data is actually protected
+        # TODO add pup token when the synthetic data is actually protected
         return None
 
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.data_type(),
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class Synthetic(StandardDatasetImplementation):
-    """Create a Synthetic op class for is_pep."""
+    """Create a Synthetic op class for is_pup."""
 
     async def to_arrow(
         self, batch_size: int
     ) -> t.AsyncIterator[pa.RecordBatch]:
         dataset = self.dataset
         parents, parents_dict = dataset.parents()
 
         # Forcing the marginals to be computed first
         parent = t.cast(Dataset, parents[0])
         _ = await parent.manager().async_marginals(parent)
 
         # Budget
-        budget_param = parents_dict['sd_budget']
+        budget_param = parents_dict["sd_budget"]
         budget = t.cast(
             t.Tuple[float, float],
             await dataset.manager().async_value(t.cast(Scalar, budget_param)),
         )
 
         # Model
-        model_properties = t.cast(Scalar, parents_dict['synthetic_model'])
+        model_properties = t.cast(Scalar, parents_dict["synthetic_model"])
         train_correlations = t.cast(
             bool, await dataset.manager().async_value(model_properties)
         )
 
         attribute = model_properties.attributes(name=SYNTHETIC_MODEL)
         use_jax_text = len(attribute) > 0 and (
             attribute[0]
@@ -345,16 +345,15 @@
         return bounds_builder(self.dataset, parent_bounds.statistics())
 
     async def marginals(self) -> st.Marginals:
         parent_marginals = await self.parent_marginals()
         return marginals_builder(self.dataset, parent_marginals.statistics())
 
 
-class SyntheticModelStaticChecker(StandardScalarStaticChecker):
-    ...
+class SyntheticModelStaticChecker(StandardScalarStaticChecker): ...
 
 
 class SyntheticModel(StandardScalarImplementation):
     """Computes the synthetic model to use"""
 
     async def value(self) -> t.Any:
         attribute = self.scalar.attribute(name=SYNTHETIC_MODEL)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/to_small_data.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/to_small_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,38 +17,38 @@
 from sarus_data_spec.scalar import Scalar
 from sarus_data_spec.schema import schema
 import sarus_data_spec.typing as st
 
 try:
     import sqlalchemy as sa
 except ModuleNotFoundError:
-    warnings.warn('sqlalchemy not installed. No sampling on bigdata')
+    warnings.warn("sqlalchemy not installed. No sampling on bigdata")
 
 try:
     from sarus_data_spec.manager.ops.sql_utils.bigdata import (
         path_to_quoted_string,
         sqlalchemy_query_to_string,
     )
     from sarus_data_spec.manager.ops.sql_utils.queries import nest_queries
     from sarus_data_spec.manager.ops.sql_utils.schema_translations import (
         async_sa_metadata_from_dataset,
     )
 except ModuleNotFoundError:
-    warnings.warn('sql utils not installed.')
+    warnings.warn("sql utils not installed.")
 
 logger = logging.getLogger(__name__)
 
 
 class ToSmallDataStaticChecker(StandardDatasetStaticChecker):
     async def schema(self) -> st.Schema:
         parent_schema = await self.parent_schema()
         return schema(
             self.dataset,
             schema_type=parent_schema.type(),
-            protected_paths=parent_schema.protobuf().protected,
+            privacy_unit_tracking_paths=parent_schema.protobuf().privacy_unit,
             properties=parent_schema.properties(),
             name=self.dataset.properties().get(DATASET_SLUGNAME, None),
         )
 
 
 class ToSmallData(StandardDatasetImplementation):
     async def size(self) -> st.Size:
@@ -127,15 +127,14 @@
             ).to_batches(max_chunksize=1000),
             batch_size=batch_size,
         )
 
     async def sql_implementation(
         self,
     ) -> t.Optional[t.Dict[t.Tuple[str, ...], str]]:
-
         schema = await self.parent_schema()
         to_small_data_proto = (
             self.dataset.transform().protobuf().spec.to_small_data
         )
         random_sampling = to_small_data_proto.random_sampling
         size_dict = await to_small_data_sizes(self.dataset)
         sqlalchemy_metadata = await async_sa_metadata_from_dataset(
@@ -209,15 +208,15 @@
             new_indices = []
             for item_name, item_type in fields.items():
                 index_element = self.batch_array.type.get_field_index(
                     item_name
                 )
                 filter_idex = pa.array(
                     np.equal(
-                        self.batch_array.field('field_selected'),
+                        self.batch_array.field("field_selected"),
                         np.array(item_name),
                     )
                 )
                 updated_indices = limit_indices_from_array(
                     self.batch_array.filter(filter_idex).flatten()[
                         index_element
                     ],
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/processor/standard/visitor_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,30 @@
         batch_array: pa.Array = array
         filter_indices: pa.Array
 
         def Null(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             self.filter_indices = pa.array(
-                np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                np.ones(len(self.batch_array.to_pylist())).astype("bool")
             )
 
         def Unit(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             self.filter_indices = pa.array(
-                np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                np.ones(len(self.batch_array.to_pylist())).astype("bool")
             )
 
         def Boolean(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Integer(
@@ -62,15 +62,15 @@
             max: int,
             base: st.IntegerBase,
             possible_values: t.Iterable[int],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Float(
@@ -79,15 +79,15 @@
             max: float,
             base: st.FloatBase,
             possible_values: t.Iterable[float],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Datetime(
@@ -97,15 +97,15 @@
             max: str,
             base: st.DatetimeBase,
             possible_values: t.Iterable[str],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Date(
@@ -115,15 +115,15 @@
             max: str,
             base: st.DateBase,
             possible_values: t.Iterable[str],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Time(
@@ -133,15 +133,15 @@
             max: str,
             base: st.TimeBase,
             possible_values: t.Iterable[str],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Duration(
@@ -150,15 +150,15 @@
             min: int,
             max: int,
             possible_values: t.Iterable[int],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Id(
@@ -166,15 +166,15 @@
             unique: bool,
             reference: t.Optional[st.Path] = None,
             base: t.Optional[st.IdBase] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Enum(
@@ -182,42 +182,42 @@
             name: str,
             name_values: t.Sequence[t.Tuple[str, int]],
             ordered: bool,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Text(
             self,
             encoding: str,
             possible_values: t.Iterable[str],
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Bytes(
             self, properties: t.Optional[t.Mapping[str, str]] = None
         ) -> None:
             if is_optional:
                 self.filter_indices = pa.array(
-                    np.ones(len(self.batch_array.to_pylist())).astype('bool')
+                    np.ones(len(self.batch_array.to_pylist())).astype("bool")
                 )
             else:
                 self.filter_indices = pa.compute.invert(
                     self.batch_array.is_null(nan_is_null=True)
                 )
 
         def Struct(
@@ -282,15 +282,15 @@
             self,
             fields: t.Mapping[str, st.Type],
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             # build filter array for this level
             initial_field_selected = self.batch_array.field(
-                'field_selected'
+                "field_selected"
             ).to_numpy(zero_copy_only=False)
 
             indices = [
                 initial_field_selected == field_name
                 for field_name in fields.keys()
             ]
             index = np.logical_or.reduce(indices)
@@ -332,20 +332,20 @@
             ]
             struct_fields = [
                 pa.field(name=field_name, type=arr.type)
                 for arr, field_name in zip(selected_arrays, fields_name)
             ]
             struct_fields.append(
                 pa.field(
-                    name='field_selected',
+                    name="field_selected",
                     type=pa.large_string(),
                     nullable=False,
                 )
             )
-            selected_arrays.append(self.batch_array.field('field_selected'))
+            selected_arrays.append(self.batch_array.field("field_selected"))
             self.batch_array = pa.StructArray.from_arrays(
                 selected_arrays,
                 fields=struct_fields,
             )
 
         def Array(
             self,
@@ -444,15 +444,15 @@
             arrays = [
                 select_columns(
                     field_type,
                     self.batch_array.flatten()[
                         self.batch_array.type.get_field_index(field_name)
                     ].filter(
                         pa.array(
-                            self.batch_array.field('field_selected').to_numpy(
+                            self.batch_array.field("field_selected").to_numpy(
                                 zero_copy_only=False
                             )
                             == field_name
                         )
                     ),
                 )
                 for field_name, field_type in fields.items()
@@ -469,15 +469,15 @@
                             pa.array(
                                 sum(sizes[i + 1 :]) * [None], type=array.type
                             ),
                         ]
                     )
                 )
 
-            structs.append(self.batch_array.field('field_selected'))
+            structs.append(self.batch_array.field("field_selected"))
             pa_fields = [
                 field.with_type(array.type)
                 for field, array in zip(self.batch_array.type, structs)
             ]
             self.batch_array = pa.StructArray.from_arrays(
                 structs,
                 fields=pa_fields,
@@ -667,15 +667,15 @@
             for fieldname, fieldtype in fields.items():
                 new_fields[fieldname] = update_fks(
                     curr_type=fieldtype, original_type=original_type
                 )
 
             self.result = sdt.Struct(
                 fields=new_fields,
-                name=name if name is not None else 'Struct',
+                name=name if name is not None else "Struct",
                 properties=properties,
             )
             # otherwise struct is empty and it is a terminal node
 
         def Union(
             self,
             fields: t.Mapping[str, st.Type],
@@ -686,55 +686,55 @@
             for fieldname, fieldtype in fields.items():
                 new_fields[fieldname] = update_fks(
                     curr_type=fieldtype, original_type=original_type
                 )
 
             self.result = sdt.Union(
                 fields=new_fields,
-                name=name if name is not None else 'Union',
+                name=name if name is not None else "Union",
                 properties=properties,
             )
 
         def Optional(
             self,
             type: st.Type,
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             self.result = sdt.Optional(
                 type=update_fks(curr_type=type, original_type=original_type),
-                name=name if name is not None else 'Optional',
+                name=name if name is not None else "Optional",
                 properties=properties,
             )
 
         def List(
             self,
             type: st.Type,
             max_size: int,
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             self.result = sdt.List(
                 type=update_fks(curr_type=type, original_type=original_type),
                 max_size=max_size,
-                name=name if name is not None else 'Optional',
+                name=name if name is not None else "Optional",
                 properties=properties,
             )
 
         def Array(
             self,
             type: st.Type,
             shape: t.Tuple[int, ...],
             name: t.Optional[str] = None,
             properties: t.Optional[t.Mapping[str, str]] = None,
         ) -> None:
             self.result = sdt.Array(
                 type=update_fks(curr_type=type, original_type=original_type),
                 shape=shape,
-                name=name if name is not None else 'Optional',
+                name=name if name is not None else "Optional",
                 properties=properties,
             )
 
         def Id(
             self,
             unique: bool,
             reference: t.Optional[st.Path] = None,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/source/routing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/source/routing.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,29 +73,29 @@
     if dataset.is_file():
         file_format = dataset.protobuf().spec.file.format
         if file_format == "csv":
             return csv_to_arrow(dataset, batch_size=batch_size)
         else:
             raise NotImplementedError(f"File format {file_format}")
 
-    elif dataset.protobuf().spec.HasField('sql'):
+    elif dataset.protobuf().spec.HasField("sql"):
         return await SourceSQL(dataset=dataset).to_arrow(batch_size=batch_size)
-    elif dataset.protobuf().spec.HasField('huggingface'):
+    elif dataset.protobuf().spec.HasField("huggingface"):
         return await Huggingface(dataset=dataset).to_arrow(
             batch_size=batch_size
         )
     else:
-        source_type = dataset.protobuf().spec.WhichOneof('spec')
+        source_type = dataset.protobuf().spec.WhichOneof("spec")
         raise NotImplementedError(f"Source {source_type}")
 
 
 async def source_dataset_schema(dataset: st.Dataset) -> st.Schema:
-    if dataset.protobuf().spec.HasField('sql'):
+    if dataset.protobuf().spec.HasField("sql"):
         return await SourceSQL(dataset=dataset).schema()
-    elif dataset.protobuf().spec.HasField('huggingface'):
+    elif dataset.protobuf().spec.HasField("huggingface"):
         return await HuggingfaceStaticChecker(dataset=dataset).schema()
     elif dataset.is_file():
         file_format = dataset.protobuf().spec.file.format
         if file_format == "csv":
             return await csv_schema(dataset)
         else:
             raise NotImplementedError(f"File format {file_format}")
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/bigdata.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/bigdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # pylint: disable=too-many-return-statements
 from __future__ import annotations
 
 from itertools import zip_longest
 import typing as t
 import warnings
 
-from scipy.stats import binom
+try:
+    from scipy.stats import binom
+except ModuleNotFoundError:
+    warnings.warn("scipy not installed")
 
 from sarus_data_spec.path import straight_path
 import sarus_data_spec.typing as st
 
 try:
     from sarus_sql.ast_transform.utils import split_quote
     import sqlalchemy as sa
 except ModuleNotFoundError:
-    warnings.warn('sqlalchemy not installed')
+    warnings.warn("sqlalchemy not installed")
 
 T = t.TypeVar("T")
 
 
 def access_table_or_col(
     metadata_or_table: t.Any, key: str, create_cte: bool = True
 ) -> t.Any:
@@ -45,29 +48,29 @@
     """
     if isinstance(metadata_or_table, (sa.sql.Selectable, sa.Table)):
         if create_cte:
             return sa.select(
                 # label('') tells SQLAlchemy to handle the alias for such col
                 # without it will generate an alias with the same name as col
                 # with it will assign a non-ambigous and allowed alias
-                getattr(metadata_or_table.exported_columns, key).label(''),
+                getattr(metadata_or_table.exported_columns, key).label(""),
             ).cte()
         if isinstance(metadata_or_table, sa.sql.Selectable):
-            return metadata_or_table.exported_columns._index[0]
+            return metadata_or_table.exported_columns[0]
         return getattr(metadata_or_table.c, key)
 
     if isinstance(metadata_or_table, sa.MetaData):
         result: t.Dict[str, t.Any] = {}
         for child_key, child_value in metadata_or_table.tables.items():
-            first_key, *rest = split_quote(child_key, '')
+            first_key, *rest = split_quote(child_key, "")
             if rest:
                 if first_key not in result:
-                    result[first_key] = {'.'.join(rest): child_value}
+                    result[first_key] = {".".join(rest): child_value}
                 else:
-                    result[first_key]['.'.join(rest)] = child_value
+                    result[first_key][".".join(rest)] = child_value
             else:
                 result[first_key] = child_value
         return result[key]
     else:
         # it is a dict on the form
         return metadata_or_table[key]
 
@@ -145,15 +148,15 @@
 
             if path_str in str2path:
                 path = str2path[path_str]
             else:
                 splitted_path = (
                     [path_str]
                     if not path_str
-                    else list(split_quote(path_str, ''))
+                    else list(split_quote(path_str, ""))
                 )
                 path = straight_path(splitted_path)
                 str2path[path_str] = path
 
             if path not in result_dict:
                 if result_length == 1:
                     result_dict[path] = {operation: result[0]}
@@ -190,15 +193,15 @@
     (my_schema, my.table) -> "my_schema"."my.table"
 
     where (my_schema, my.table) is the tuple representation of the st.Path
 
     Used to create sql queries and table objects manipulated by sqlachemy
     metadata.
     """
-    return '.'.join(f'"{path}"' for path in path.to_strings_list()[0])
+    return ".".join(f'"{path}"' for path in path.to_strings_list()[0])
 
 
 def sqlalchemy_query_to_string(sa_query: sa.sql.ClauseElement) -> str:
     """Compiles the sqlalchemy query into a string"""
     return str(sa_query.compile(compile_kwargs={"literal_binds": True}))
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/ops/sql_utils/queries.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/ops/sql_utils/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from sarus_sql import ast_utils, rename_tables, translator
 except ModuleNotFoundError:
     logger = logging.getLogger(__name__)
     logger.info("sarus_sql not available.")
 
-from sarus_data_spec.path import Path
+from sarus_data_spec.typing import Path
 import sarus_data_spec.type as sdt
 import sarus_data_spec.typing as st
 
 
 def rename_and_compose_queries(
     query_or_dict: t.Union[str, t.Dict[str, t.Any]],
     curr_path: t.List[str],
@@ -21,34 +21,36 @@
 ) -> t.Union[str, t.Dict[str, t.Any]]:
     """Composition is done by first updating the table names
     in the leaves of queries_or_dict and then composing with
     all the queries in queries_transform
     """
     if isinstance(query_or_dict, str):
         # type ignore because issue of typing in sarus_sql
-        updated_query = rename_tables.rename_tables(query_or_dict, table_map)  # type: ignore # noqa : E501
+        updated_query: str = rename_tables.rename_tables(
+            query_or_dict, table_map
+        )  # noqa : E501
         if queries_transform is not None:
             updated_query = ast_utils.compose_query(
                 queries_transform, updated_query
             )
         return updated_query
     else:
-        new_queries = {}
+        new_queries: dict[str, t.Any] = {}
         for name, sub_queries_or_dict in query_or_dict.items():
             new_queries[name] = rename_and_compose_queries(
                 query_or_dict=sub_queries_or_dict,
                 curr_path=[*curr_path, name],
                 queries_transform=queries_transform,
                 table_map=table_map,
             )
         return new_queries
 
 
 def flatten_queries_dict(
-    queries: t.Dict[str, t.Any]
+    queries: t.Dict[str, t.Any],
 ) -> t.Dict[t.Tuple[str, ...], str]:
     """Transform nested dict in linear dict where each
     key is the tuple of the nesting path"""
 
     final_dict: t.Dict[t.Tuple[str, ...], str] = {}
 
     def update_dict(
@@ -109,15 +111,15 @@
                 destination_dialect,
             )
         )
     return new_query
 
 
 def nest_queries(
-    queries: t.Dict[t.Tuple[str, ...], str]
+    queries: t.Dict[t.Tuple[str, ...], str],
 ) -> t.Dict[str, t.Any]:
     """It transform the dict of queries according to the tuple keys:
     if queries = {
             ('a','b'):'q',
             ('a','c'):'q'
     }
     the results woulf be: {a: {b: 'q', c: 'q'}
@@ -143,15 +145,15 @@
     for name, subdict in intermediate.items():
         final[name] = nest_queries(subdict)
 
     return final
 
 
 def nested_dict_of_types(
-    types: t.Dict[t.Tuple[str, ...], st.Type]
+    types: t.Dict[t.Tuple[str, ...], st.Type],
 ) -> t.Dict[str, t.Any]:
     """Similar to nest_queries but values are sarus types instead of strings"""
     intermediate: t.Dict[str, t.Dict[t.Tuple[str, ...], t.Any]] = defaultdict(
         dict
     )
     final: t.Dict[str, t.Any] = {}
     for type_path, type in types.items():
@@ -163,15 +165,15 @@
     for name, subdict in intermediate.items():
         final[name] = nested_dict_of_types(subdict)
 
     return final
 
 
 def nested_unions_from_nested_dict_of_types(
-    nested_types: t.Dict[str, t.Any]
+    nested_types: t.Dict[str, t.Any],
 ) -> t.Dict[str, st.Type]:
     """create unions out of nested_types"""
     fields: t.Dict[str, st.Type] = {}
     for path_string, type_or_dict in nested_types.items():
         if isinstance(type_or_dict, dict):
             fields[path_string] = sdt.Union(
                 nested_unions_from_nested_dict_of_types(type_or_dict)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/manager/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/manager/typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,186 +121,154 @@
         """Synchronous parquet caching"""
         ...
 
     async def async_to_parquet(self, dataset: st.Dataset) -> None:
         """Asynchronous parquet caching"""
         ...
 
-    def parquet_dir(self) -> str:
-        ...
+    def parquet_dir(self) -> str: ...
 
-    def marginals(self, dataset: st.Dataset) -> st.Marginals:
-        ...
+    def marginals(self, dataset: st.Dataset) -> st.Marginals: ...
 
-    async def async_marginals(self, dataset: st.Dataset) -> st.Marginals:
-        ...
+    async def async_marginals(self, dataset: st.Dataset) -> st.Marginals: ...
 
-    def bounds(self, dataset: st.Dataset) -> st.Bounds:
-        ...
+    def bounds(self, dataset: st.Dataset) -> st.Bounds: ...
 
-    async def async_bounds(self, dataset: st.Dataset) -> st.Bounds:
-        ...
+    async def async_bounds(self, dataset: st.Dataset) -> st.Bounds: ...
 
-    def size(self, dataset: st.Dataset) -> st.Size:
-        ...
+    def size(self, dataset: st.Dataset) -> st.Size: ...
 
-    async def async_size(self, dataset: st.Dataset) -> st.Size:
-        ...
+    async def async_size(self, dataset: st.Dataset) -> st.Size: ...
 
-    def multiplicity(self, dataset: st.Dataset) -> st.Multiplicity:
-        ...
+    def multiplicity(self, dataset: st.Dataset) -> st.Multiplicity: ...
 
-    async def async_multiplicity(self, dataset: st.Dataset) -> st.Multiplicity:
-        ...
+    async def async_multiplicity(
+        self, dataset: st.Dataset
+    ) -> st.Multiplicity: ...
 
-    def to_pandas(self, dataset: st.Dataset) -> pd.DataFrame:
-        ...
+    def to_pandas(self, dataset: st.Dataset) -> pd.DataFrame: ...
 
-    async def async_to_pandas(self, dataset: st.Dataset) -> pd.DataFrame:
-        ...
+    async def async_to_pandas(self, dataset: st.Dataset) -> pd.DataFrame: ...
 
     async def async_to(
         self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
     ) -> st.DatasetCastable:
         """Casts a Dataset to a Python type passed as argument."""
         ...
 
     def to(
         self, dataset: st.Dataset, kind: t.Type, drop_admin: bool = True
-    ) -> st.DatasetCastable:
-        ...
+    ) -> st.DatasetCastable: ...
 
-    def to_tensorflow(self, dataset: st.Dataset) -> tf.data.Dataset:
-        ...
+    def to_tensorflow(self, dataset: st.Dataset) -> tf.data.Dataset: ...
 
     async def async_to_tensorflow(
         self, dataset: st.Dataset
-    ) -> tf.data.Dataset:
-        ...
+    ) -> tf.data.Dataset: ...
 
-    def to_sql(self, dataset: st.Dataset) -> None:
-        ...
+    def to_sql(self, dataset: st.Dataset) -> None: ...
 
-    async def async_to_sql(self, dataset: st.Dataset) -> None:
-        ...
+    async def async_to_sql(self, dataset: st.Dataset) -> None: ...
 
     def status(
         self, dataspec: st.DataSpec, task_name: t.Optional[str] = None
-    ) -> t.Optional[st.Status]:
-        ...
+    ) -> t.Optional[st.Status]: ...
 
-    def dataspec_rewriter(self) -> sdrt.DataspecRewriter:
-        ...
+    def dataspec_rewriter(self) -> sdrt.DataspecRewriter: ...
 
-    def dataspec_validator(self) -> sdvt.DataspecValidator:
-        ...
+    def dataspec_validator(self) -> sdvt.DataspecValidator: ...
 
     def is_remote(self, dataspec: st.DataSpec) -> bool:
         """Is the dataspec a remotely defined dataset."""
         ...
 
     def infer_output_type(
         self,
         transform: st.Transform,
         *arguments: t.Union[st.DataSpec, st.Transform],
         **named_arguments: t.Union[st.DataSpec, st.Transform],
-    ) -> Tuple[str, Callable[[st.DataSpec], None]]:
-        ...
+    ) -> Tuple[str, Callable[[st.DataSpec], None]]: ...
 
-    def foreign_keys(self, dataset: st.Dataset) -> Dict[st.Path, st.Path]:
-        ...
+    def foreign_keys(self, dataset: st.Dataset) -> Dict[st.Path, st.Path]: ...
 
     async def async_foreign_keys(
         self, dataset: st.Dataset
-    ) -> Dict[st.Path, st.Path]:
-        ...
+    ) -> Dict[st.Path, st.Path]: ...
 
-    async def async_primary_keys(self, dataset: st.Dataset) -> List[st.Path]:
-        ...
+    async def async_primary_keys(
+        self, dataset: st.Dataset
+    ) -> List[st.Path]: ...
 
-    def primary_keys(self, dataset: st.Dataset) -> List[st.Path]:
-        ...
+    def primary_keys(self, dataset: st.Dataset) -> List[st.Path]: ...
 
     def sql(
         self,
         dataset: st.Dataset,
         query: t.Union[str, t.Dict[str, t.Any]],
         dialect: Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
-    ) -> Iterator[pa.RecordBatch]:
-        ...
+    ) -> Iterator[pa.RecordBatch]: ...
 
     async def async_sql(
         self,
         dataset: st.Dataset,
         query: t.Union[str, t.Dict[str, t.Any]],
         dialect: Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
         result_type: t.Optional[st.Type] = None,
-    ) -> AsyncIterator[pa.RecordBatch]:
-        ...
+    ) -> AsyncIterator[pa.RecordBatch]: ...
 
     async def execute_sql_query(
         self,
         dataset: st.Dataset,
         caching_properties: t.Mapping[str, str],
         query: t.Union[str, t.Dict[str, t.Any]],
         dialect: t.Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
         result_type: t.Optional[st.Type] = None,
-    ) -> t.AsyncIterator[pa.RecordBatch]:
-        ...
+    ) -> t.AsyncIterator[pa.RecordBatch]: ...
 
     async def async_sql_op(
         self,
         dataset: st.Dataset,
         query: t.Union[str, t.Dict[str, t.Any]],
         dialect: t.Optional[st.SQLDialect] = None,
         batch_size: int = 10000,
         result_type: t.Optional[st.Type] = None,
-    ) -> t.AsyncIterator[pa.RecordBatch]:
-        ...
+    ) -> t.AsyncIterator[pa.RecordBatch]: ...
 
-    def is_big_data(self, dataset: st.DataSpec) -> bool:
-        ...
+    def is_big_data(self, dataset: st.DataSpec) -> bool: ...
 
-    def caches(self) -> t.Any:
-        ...
+    def caches(self) -> t.Any: ...
 
     def is_cached(self, dataspec: st.DataSpec) -> bool:
         """Returns whether a dataspec should be cached
         or not"""
         ...
 
     def is_pushed_to_sql(self, dataspec: st.DataSpec) -> bool:
         """Returns whether a dataspec should be pushed to sql
         or not"""
         ...
 
     def attribute(
         self, name: str, dataspec: st.DataSpec
-    ) -> t.Optional[st.Attribute]:
-        ...
+    ) -> t.Optional[st.Attribute]: ...
 
     def attributes(
         self, name: str, dataspec: st.DataSpec
-    ) -> t.List[st.Attribute]:
-        ...
+    ) -> t.List[st.Attribute]: ...
 
-    def links(self, dataset: st.Dataset) -> st.Links:
-        ...
+    def links(self, dataset: st.Dataset) -> st.Links: ...
 
-    async def async_links(self, dataset: st.Dataset) -> st.Links:
-        ...
+    async def async_links(self, dataset: st.Dataset) -> st.Links: ...
 
-    def sql_pushing_schema_prefix(self, dataset: st.Dataset) -> str:
-        ...
+    def sql_pushing_schema_prefix(self, dataset: st.Dataset) -> str: ...
 
-    def engine(self, uri: str) -> sa_engine:
-        ...
+    def engine(self, uri: str) -> sa_engine: ...
 
     def mock_value(
         self,
         transform: st.Transform,
         *arguments: st.DataSpec,
         **named_arguments: st.DataSpec,
     ) -> t.Any:
@@ -336,15 +304,15 @@
     and that updates statuses during the process
     - result: a method that allows to get the value of the computation
     either by reading the cache/storage or via the ops.
 
     Furthermore, a computation has a method to monitor task completion.
     """
 
-    task_name: str = ''
+    task_name: str = ""
 
     def launch_task(self, dataspec: st.DataSpec) -> t.Optional[t.Awaitable]:
         """This methods launches a task in the background
         but returns immediately without waiting for the
         result. It updates the statuses during its process."""
         ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/marginals.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/marginals.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Builder
 def marginals(
     dataset: st.Dataset,
     statistics: t.Optional[st.Statistics] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Marginals:
-    name = f'{dataset.name()}_marginals'
+    name = f"{dataset.name()}_marginals"
 
     return Marginals(
         sp.Marginals(
             dataset=dataset.uuid(),
             name=name,
             statistics=statistics.protobuf()
             if statistics is not None
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/multiplicity.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/multiplicity.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Builder
 def multiplicity(
     dataset: st.Dataset,
     statistics: t.Optional[st.Statistics] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Multiplicity:
-    name = f'{dataset.name()}_multiplicities'
+    name = f"{dataset.name()}_multiplicities"
 
     return Multiplicity(
         sp.Multiplicity(
             dataset=dataset.uuid(),
             name=name,
             statistics=statistics.protobuf()
             if statistics is not None
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/path.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/path.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                 if available_sub_path.label() == sub_path.label():
                     final_sub_paths.extend(available_sub_path.select(sub_path))
 
         return final_sub_paths
 
     def is_empty(self) -> bool:
         assert not self.has_sub_paths()
-        return self.label() == ''
+        return self.label() == ""
 
     def has_sub_paths(self) -> bool:
         return len(self._protobuf.paths) > 0
 
     def to_strings_list(self) -> t.List[t.List[str]]:
         paths = []
         proto = self._protobuf
@@ -53,15 +53,15 @@
                 )
             paths.extend(out)
         return paths
 
     def to_dict(self) -> t.Dict[str, str]:
         list_paths = self.to_strings_list()
         return {
-            '.'.join(path[1:-1]): path[-1] for path in list_paths
+            ".".join(path[1:-1]): path[-1] for path in list_paths
         }  # always start with DATA
 
 
 def paths(path_list: t.List[t.List[str]]) -> t.List[Path]:
     out = defaultdict(list)
     for path in path_list:
         try:
@@ -77,27 +77,27 @@
                 paths=[path.protobuf() for path in paths(path_list)],
             )
         )
         for element, path_list in dict(out).items()
     ]
 
 
-def path(label: str = '', paths: t.Optional[t.List[st.Path]] = None) -> Path:
+def path(label: str = "", paths: t.Optional[t.List[st.Path]] = None) -> Path:
     """Builds a Path out of a label and a set of sub-paths"""
     if paths is None:
         paths = []
     return Path(
         sp.Path(label=label, paths=[element.protobuf() for element in paths])
     )
 
 
 def straight_path(nodes: t.List[str]) -> Path:
     """Returns linear path between elements in the list"""
     if len(nodes) == 0:
-        raise ValueError('At least one node must be provided')
+        raise ValueError("At least one node must be provided")
     curr_sub_path: t.List[st.Path] = []
     for el in reversed(nodes):
         update = path(label=el, paths=curr_sub_path)
         curr_sub_path = [update]
     return update
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/predicate.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/predicate.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,53 +13,53 @@
     def prototype(self) -> Type[sp.Predicate]:
         """Return the type of the underlying protobuf."""
         return sp.Predicate
 
     # A bunch of operators
     def __or__(self, predicate: st.Predicate) -> Predicate:
         """Union operator"""
-        if self._protobuf.HasField('union'):
+        if self._protobuf.HasField("union"):
             result = Predicate(self._protobuf)
-            if predicate.protobuf().HasField('union'):
+            if predicate.protobuf().HasField("union"):
                 result._protobuf.union.predicates.extend(
                     predicate.protobuf().union.predicates
                 )
             else:
                 result._protobuf.union.predicates.append(predicate.protobuf())
             return result
         else:
-            if predicate.protobuf().HasField('union'):
+            if predicate.protobuf().HasField("union"):
                 result = Predicate(predicate.protobuf())
                 result._protobuf.union.predicates.insert(0, self._protobuf)
                 return result
             else:
                 return union(self, predicate)
 
     def __and__(self, predicate: st.Predicate) -> Predicate:
         """Inter operator"""
-        if self._protobuf.HasField('inter'):
+        if self._protobuf.HasField("inter"):
             result = Predicate(self._protobuf)
-            if predicate.protobuf().HasField('inter'):
+            if predicate.protobuf().HasField("inter"):
                 result._protobuf.inter.predicates.extend(
                     predicate.protobuf().inter.predicates
                 )
             else:
                 result._protobuf.inter.predicates.append(predicate.protobuf())
             return result
         else:
-            if predicate.protobuf().HasField('inter'):
+            if predicate.protobuf().HasField("inter"):
                 result = Predicate(predicate.protobuf())
                 result._protobuf.inter.predicates.insert(0, self._protobuf)
                 return result
             else:
                 return inter(self, predicate)
 
     def __invert__(self) -> Predicate:
         """Complement"""
-        if self._protobuf.HasField('comp'):
+        if self._protobuf.HasField("comp"):
             return Predicate(self._protobuf.comp.predicate)
         else:
             return comp(self)
 
 
 def inter(*predicates: st.Predicate) -> Predicate:
     return Predicate(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/attribute_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/attribute_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/bounds_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/bounds_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/bounds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/constraint_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)sarus_data_spec/protobuf/constraint.proto\x12\x0fsarus_data_spec\"\x82\x02\n\x11VariantConstraint\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61taspec\x18\x02 \x01(\t\x12\x38\n\x0f\x63onstraint_kind\x18\x03 \x01(\x0e\x32\x1f.sarus_data_spec.ConstraintKind\x12\x18\n\x10required_context\x18\x04 \x03(\t\x12\x46\n\nproperties\x18\x05 \x03(\x0b\x32\x32.sarus_data_spec.VariantConstraint.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01*]\n\x0e\x43onstraintKind\x12\r\n\tSYNTHETIC\x10\x00\x12\x06\n\x02\x44P\x10\x01\x12\n\n\x06PUBLIC\x10\x02\x12\x07\n\x03PEP\x10\x03\x12\x08\n\x04MOCK\x10\x04\x12\x15\n\x11PEP_FOR_REWRITING\x10\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)sarus_data_spec/protobuf/constraint.proto\x12\x0fsarus_data_spec\"\x82\x02\n\x11VariantConstraint\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61taspec\x18\x02 \x01(\t\x12\x38\n\x0f\x63onstraint_kind\x18\x03 \x01(\x0e\x32\x1f.sarus_data_spec.ConstraintKind\x12\x18\n\x10required_context\x18\x04 \x03(\t\x12\x46\n\nproperties\x18\x05 \x03(\x0b\x32\x32.sarus_data_spec.VariantConstraint.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01*]\n\x0e\x43onstraintKind\x12\r\n\tSYNTHETIC\x10\x00\x12\x06\n\x02\x44P\x10\x01\x12\n\n\x06PUBLIC\x10\x02\x12\x07\n\x03PUP\x10\x03\x12\x08\n\x04MOCK\x10\x04\x12\x15\n\x11PUP_FOR_REWRITING\x10\x05\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sarus_data_spec.protobuf.constraint_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _VARIANTCONSTRAINT_PROPERTIESENTRY._options = None
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/constraint_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/constraint_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
     ValueType = typing.NewType('ValueType', builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 class _ConstraintKindEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ConstraintKind.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
     SYNTHETIC: ConstraintKind.ValueType = ...  # 0
     DP: ConstraintKind.ValueType = ...  # 1
     PUBLIC: ConstraintKind.ValueType = ...  # 2
-    PEP: ConstraintKind.ValueType = ...  # 3
+    PUP: ConstraintKind.ValueType = ...  # 3
     MOCK: ConstraintKind.ValueType = ...  # 4
-    PEP_FOR_REWRITING: ConstraintKind.ValueType = ...  # 5
+    PUP_FOR_REWRITING: ConstraintKind.ValueType = ...  # 5
 class ConstraintKind(_ConstraintKind, metaclass=_ConstraintKindEnumTypeWrapper):
     pass
 
 SYNTHETIC: ConstraintKind.ValueType = ...  # 0
 DP: ConstraintKind.ValueType = ...  # 1
 PUBLIC: ConstraintKind.ValueType = ...  # 2
-PEP: ConstraintKind.ValueType = ...  # 3
+PUP: ConstraintKind.ValueType = ...  # 3
 MOCK: ConstraintKind.ValueType = ...  # 4
-PEP_FOR_REWRITING: ConstraintKind.ValueType = ...  # 5
+PUP_FOR_REWRITING: ConstraintKind.ValueType = ...  # 5
 global___ConstraintKind = ConstraintKind
 
 
 class VariantConstraint(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/dataset_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/links_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/links_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/manager_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/manager_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/marginals_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/marginals_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/marginals_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/multiplicity_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/multiplicity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/path_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/path_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/path_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/predicate_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/predicate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/proto_container_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/proto_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/relation_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/relation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/scalar_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/scalar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/schema_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 _sym_db = _symbol_database.Default()
 
 
 from sarus_data_spec.protobuf import type_pb2 as sarus__data__spec_dot_protobuf_dot_type__pb2
 from sarus_data_spec.protobuf import path_pb2 as sarus__data__spec_dot_protobuf_dot_path__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%sarus_data_spec/protobuf/schema.proto\x12\x0fsarus_data_spec\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\"\xd0\x03\n\x06Schema\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12#\n\x04type\x18\x04 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12(\n\tprotected\x18\x05 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12;\n\nproperties\x18\x06 \x03(\x0b\x32\'.sarus_data_spec.Schema.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd9\x01\n\nHypothesis\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12#\n\x04type\x18\x04 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\x46\n\nproperties\x18\x05 \x03(\x0b\x32\x32.sarus_data_spec.Schema.Hypothesis.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%sarus_data_spec/protobuf/schema.proto\x12\x0fsarus_data_spec\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\"\xd3\x03\n\x06Schema\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12#\n\x04type\x18\x04 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12+\n\x0cprivacy_unit\x18\x05 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12;\n\nproperties\x18\x06 \x03(\x0b\x32\'.sarus_data_spec.Schema.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xd9\x01\n\nHypothesis\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0f\n\x07\x64\x61taset\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12#\n\x04type\x18\x04 \x01(\x0b\x32\x15.sarus_data_spec.Type\x12\x46\n\nproperties\x18\x05 \x03(\x0b\x32\x32.sarus_data_spec.Schema.Hypothesis.PropertiesEntry\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sarus_data_spec.protobuf.schema_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _SCHEMA_PROPERTIESENTRY._options = None
   _SCHEMA_PROPERTIESENTRY._serialized_options = b'8\001'
   _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._options = None
   _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._serialized_options = b'8\001'
   _SCHEMA._serialized_start=133
-  _SCHEMA._serialized_end=597
-  _SCHEMA_PROPERTIESENTRY._serialized_start=328
-  _SCHEMA_PROPERTIESENTRY._serialized_end=377
-  _SCHEMA_HYPOTHESIS._serialized_start=380
-  _SCHEMA_HYPOTHESIS._serialized_end=597
-  _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._serialized_start=328
-  _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._serialized_end=377
+  _SCHEMA._serialized_end=600
+  _SCHEMA_PROPERTIESENTRY._serialized_start=331
+  _SCHEMA_PROPERTIESENTRY._serialized_end=380
+  _SCHEMA_HYPOTHESIS._serialized_start=383
+  _SCHEMA_HYPOTHESIS._serialized_end=600
+  _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._serialized_start=331
+  _SCHEMA_HYPOTHESIS_PROPERTIESENTRY._serialized_end=380
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/schema_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/schema_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -72,38 +72,38 @@
         def HasField(self, field_name: typing_extensions.Literal["type",b"type"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","type",b"type","uuid",b"uuid"]) -> None: ...
 
     UUID_FIELD_NUMBER: builtins.int
     DATASET_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
-    PROTECTED_FIELD_NUMBER: builtins.int
+    PRIVACY_UNIT_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     uuid: typing.Text = ...
     """Schema definition attribute"""
 
     dataset: typing.Text = ...
     """uuid"""
 
     name: typing.Text = ...
     @property
     def type(self) -> sarus_data_spec.protobuf.type_pb2.Type: ...
     @property
-    def protected(self) -> sarus_data_spec.protobuf.path_pb2.Path:
-        """Protected entity (may be empty for non-Sarus datasets)"""
+    def privacy_unit(self) -> sarus_data_spec.protobuf.path_pb2.Path:
+        """Privacy Unit (may be empty for non-Sarus datasets)"""
         pass
     @property
     def properties(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]:
         """Other properties"""
         pass
     def __init__(self,
         *,
         uuid : typing.Text = ...,
         dataset : typing.Text = ...,
         name : typing.Text = ...,
         type : typing.Optional[sarus_data_spec.protobuf.type_pb2.Type] = ...,
-        protected : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
+        privacy_unit : typing.Optional[sarus_data_spec.protobuf.path_pb2.Path] = ...,
         properties : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["protected",b"protected","type",b"type"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","properties",b"properties","protected",b"protected","type",b"type","uuid",b"uuid"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["privacy_unit",b"privacy_unit","type",b"type"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["dataset",b"dataset","name",b"name","privacy_unit",b"privacy_unit","properties",b"properties","type",b"type","uuid",b"uuid"]) -> None: ...
 global___Schema = Schema
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/size_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/size_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/size_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/statistics_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/statistics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/status_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform.proto`

 * *Files 7% similar despite different names*

```diff
@@ -22,21 +22,21 @@
       Project project = 4;
       Filter filter = 5;
       Shuffle shuffle = 6;
       Join join = 7;
       Cast cast = 8;
       Sample sample = 9;
       UserSettings user_settings = 10;
-      Protect protect_dataset = 11;
+      PrivacyUnitTracking privacy_unit_tracking = 11;
       External external = 12; // np transforms, pd transforms,...
       Synthetic synthetic = 13;
       Transcode transcode = 14;
       InverseTranscode inverse_transcode = 15;
       GetItem get_item = 16;
-      ProtectedPaths protected_paths = 17;
+      PrivacyUnitTrackingPaths privacy_unit_tracking_paths = 17;
       AutomaticUserSettings automatic_user_settings = 18;
       PublicPaths public_paths = 19;
       AssignBudget assign_budget = 20;
       AutomaticBudget automatic_budget = 21;
       AttributesBudget attribute_budget = 22;
       SDBudget sd_budget = 23;
       DeriveSeed derive_seed = 24;
@@ -197,15 +197,15 @@
   message UserSettings {
   }
 
   message AutomaticUserSettings {
     int64 max_categories = 1;
   }
 
-  message Protect {
+  message PrivacyUnitTracking {
   }
 
   message Transcode {
   }
 
   message InverseTranscode {
   }
@@ -213,15 +213,15 @@
     oneof proportion {
       double fraction = 1;
       int64 size = 2;
     }
     sarus_data_spec.Scalar seed = 3;
   }
 
-  message ProtectedPaths {
+  message PrivacyUnitTrackingPaths {
   }
 
   message PublicPaths {
   }
 
   message GetItem {
     sarus_data_spec.Path path = 1;
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,143 +12,143 @@
 
 
 from sarus_data_spec.protobuf import type_pb2 as sarus__data__spec_dot_protobuf_dot_type__pb2
 from sarus_data_spec.protobuf import path_pb2 as sarus__data__spec_dot_protobuf_dot_path__pb2
 from sarus_data_spec.protobuf import scalar_pb2 as sarus__data__spec_dot_protobuf_dot_scalar__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\x93)\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xea\r\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12-\n\x0fprotect_dataset\x18\x0b \x01(\x0b\x32\x12.Transform.ProtectH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12\x34\n\x0fprotected_paths\x18\x11 \x01(\x0b\x32\x19.Transform.ProtectedPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\t\n\x07Protect\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x10\n\x0eProtectedPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(sarus_data_spec/protobuf/transform.proto\x1a#sarus_data_spec/protobuf/type.proto\x1a#sarus_data_spec/protobuf/path.proto\x1a%sarus_data_spec/protobuf/scalar.proto\"\xd1)\n\tTransform\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0b\n\x03\x64oc\x18\x03 \x01(\t\x12\x1d\n\x04spec\x18\x04 \x01(\x0b\x32\x0f.Transform.Spec\x12.\n\nproperties\x18\x05 \x03(\x0b\x32\x1a.Transform.PropertiesEntry\x12\x12\n\ninversible\x18\x06 \x01(\x08\x12\x19\n\x11schema_preserving\x18\x07 \x01(\x08\x1a\x31\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x92\x0e\n\x04Spec\x12\'\n\x08identity\x18\x01 \x01(\x0b\x32\x13.Transform.IdentityH\x00\x12\'\n\x08variable\x18\x02 \x01(\x0b\x32\x13.Transform.VariableH\x00\x12\'\n\x08\x63omposed\x18\x03 \x01(\x0b\x32\x13.Transform.ComposedH\x00\x12%\n\x07project\x18\x04 \x01(\x0b\x32\x12.Transform.ProjectH\x00\x12#\n\x06\x66ilter\x18\x05 \x01(\x0b\x32\x11.Transform.FilterH\x00\x12%\n\x07shuffle\x18\x06 \x01(\x0b\x32\x12.Transform.ShuffleH\x00\x12\x1f\n\x04join\x18\x07 \x01(\x0b\x32\x0f.Transform.JoinH\x00\x12\x1f\n\x04\x63\x61st\x18\x08 \x01(\x0b\x32\x0f.Transform.CastH\x00\x12#\n\x06sample\x18\t \x01(\x0b\x32\x11.Transform.SampleH\x00\x12\x30\n\ruser_settings\x18\n \x01(\x0b\x32\x17.Transform.UserSettingsH\x00\x12?\n\x15privacy_unit_tracking\x18\x0b \x01(\x0b\x32\x1e.Transform.PrivacyUnitTrackingH\x00\x12\'\n\x08\x65xternal\x18\x0c \x01(\x0b\x32\x13.Transform.ExternalH\x00\x12)\n\tsynthetic\x18\r \x01(\x0b\x32\x14.Transform.SyntheticH\x00\x12)\n\ttranscode\x18\x0e \x01(\x0b\x32\x14.Transform.TranscodeH\x00\x12\x38\n\x11inverse_transcode\x18\x0f \x01(\x0b\x32\x1b.Transform.InverseTranscodeH\x00\x12&\n\x08get_item\x18\x10 \x01(\x0b\x32\x12.Transform.GetItemH\x00\x12J\n\x1bprivacy_unit_tracking_paths\x18\x11 \x01(\x0b\x32#.Transform.PrivacyUnitTrackingPathsH\x00\x12\x43\n\x17\x61utomatic_user_settings\x18\x12 \x01(\x0b\x32 .Transform.AutomaticUserSettingsH\x00\x12.\n\x0cpublic_paths\x18\x13 \x01(\x0b\x32\x16.Transform.PublicPathsH\x00\x12\x30\n\rassign_budget\x18\x14 \x01(\x0b\x32\x17.Transform.AssignBudgetH\x00\x12\x36\n\x10\x61utomatic_budget\x18\x15 \x01(\x0b\x32\x1a.Transform.AutomaticBudgetH\x00\x12\x37\n\x10\x61ttribute_budget\x18\x16 \x01(\x0b\x32\x1b.Transform.AttributesBudgetH\x00\x12(\n\tsd_budget\x18\x17 \x01(\x0b\x32\x13.Transform.SDBudgetH\x00\x12,\n\x0b\x64\x65rive_seed\x18\x18 \x01(\x0b\x32\x15.Transform.DeriveSeedH\x00\x12+\n\x0bgroup_by_pe\x18\x19 \x01(\x0b\x32\x14.Transform.GroupByPEH\x00\x12\x34\n\x0fsampling_ratios\x18\x1a \x01(\x0b\x32\x19.Transform.SamplingRatiosH\x00\x12*\n\nselect_sql\x18\x1b \x01(\x0b\x32\x14.Transform.SelectSqlH\x00\x12%\n\x07\x65xtract\x18\x1c \x01(\x0b\x32\x12.Transform.ExtractH\x00\x12\x38\n\x11relationship_spec\x18\x1d \x01(\x0b\x32\x1b.Transform.RelationshipSpecH\x00\x12@\n\x15\x64ifferentiated_sample\x18\x1e \x01(\x0b\x32\x1f.Transform.DifferentiatedSampleH\x00\x12;\n\x13validated_user_type\x18\x1f \x01(\x0b\x32\x1c.Transform.ValidatedUserTypeH\x00\x12/\n\rdp_select_sql\x18  \x01(\x0b\x32\x16.Transform.DPSelectSqlH\x00\x12\x36\n\x10\x65rror_estimation\x18! \x01(\x0b\x32\x1a.Transform.ErrorEstimationH\x00\x12(\n\tfit_model\x18\" \x01(\x0b\x32\x13.Transform.FitModelH\x00\x12-\n\x0c\x66it_model_dp\x18# \x01(\x0b\x32\x15.Transform.FitModelDPH\x00\x12;\n\x13generate_from_model\x18$ \x01(\x0b\x32\x1c.Transform.GenerateFromModelH\x00\x12/\n\rto_small_data\x18% \x01(\x0b\x32\x16.Transform.ToSmallDataH\x00\x42\x06\n\x04spec\x1a\xf6\x07\n\x08\x45xternal\x12\x11\n\targuments\x18\x01 \x01(\x0c\x12\x17\n\x0fnamed_arguments\x18\x02 \x01(\x0c\x12\x37\n\rop_identifier\x18\x03 \x01(\x0b\x32 .Transform.External.OpIdentifier\x1a\xd7\x04\n\x0cOpIdentifier\x12&\n\x03std\x18\x01 \x01(\x0b\x32\x17.Transform.External.StdH\x00\x12,\n\x06pandas\x18\x02 \x01(\x0b\x32\x1a.Transform.External.PandasH\x00\x12*\n\x05numpy\x18\x03 \x01(\x0b\x32\x19.Transform.External.NumpyH\x00\x12\x34\n\ntensorflow\x18\x04 \x01(\x0b\x32\x1e.Transform.External.TensorflowH\x00\x12.\n\x07sklearn\x18\x05 \x01(\x0b\x32\x1b.Transform.External.SklearnH\x00\x12?\n\x10pandas_profiling\x18\x06 \x01(\x0b\x32#.Transform.External.PandasProfilingH\x00\x12.\n\x07xgboost\x18\x07 \x01(\x0b\x32\x1b.Transform.External.XGBoostH\x00\x12*\n\x05skopt\x18\x08 \x01(\x0b\x32\x19.Transform.External.SkoptH\x00\x12\x30\n\x08imblearn\x18\t \x01(\x0b\x32\x1c.Transform.External.ImblearnH\x00\x12(\n\x04shap\x18\n \x01(\x0b\x32\x18.Transform.External.ShapH\x00\x12*\n\x05scipy\x18\x0b \x01(\x0b\x32\x19.Transform.External.ScipyH\x00\x12\x34\n\noptbinning\x18\x0c \x01(\x0b\x32\x1e.Transform.External.OptBinningH\x00\x42\x04\n\x02op\x1a\x13\n\x03Std\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x16\n\x06Pandas\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Numpy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nTensorflow\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07Sklearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1f\n\x0fPandasProfiling\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x17\n\x07XGBoost\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Skopt\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x18\n\x08Imblearn\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x14\n\x04Shap\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x15\n\x05Scipy\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\x1a\n\nOptBinning\x12\x0c\n\x04name\x18\x01 \x01(\t\x1a\n\n\x08Identity\x1a*\n\x08Variable\x12\x10\n\x08position\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x1a\xa9\x01\n\x08\x43omposed\x12\x11\n\ttransform\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x03(\t\x12@\n\x0fnamed_arguments\x18\x03 \x03(\x0b\x32\'.Transform.Composed.NamedArgumentsEntry\x1a\x35\n\x13NamedArgumentsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x34\n\x07Project\x12)\n\nprojection\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a/\n\x06\x46ilter\x12%\n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\t\n\x07Shuffle\x1a)\n\x04Join\x12!\n\x02on\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a+\n\x04\x43\x61st\x12#\n\x04type\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Type\x1a\x61\n\x06Sample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1av\n\x0fSchemaInference\x12:\n\x0b\x63\x61st_policy\x18\x01 \x01(\x0e\x32%.Transform.SchemaInference.CastPolicy\"\'\n\nCastPolicy\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bMOST_LIKELY\x10\x01\x1a\x16\n\x07GroupBy\x12\x0b\n\x03key\x18\x01 \x01(\t\x1a[\n\x0bToSmallData\x12\x0c\n\x04size\x18\x01 \x01(\x05\x12\x17\n\x0frandom_sampling\x18\x02 \x01(\x08\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.Scalar\x1a\x0b\n\tSynthetic\x1a\x0e\n\x0cUserSettings\x1a/\n\x15\x41utomaticUserSettings\x12\x16\n\x0emax_categories\x18\x01 \x01(\x03\x1a\x15\n\x13PrivacyUnitTracking\x1a\x0b\n\tTranscode\x1a\x12\n\x10InverseTranscode\x1ao\n\x14\x44ifferentiatedSample\x12\x12\n\x08\x66raction\x18\x01 \x01(\x01H\x00\x12\x0e\n\x04size\x18\x02 \x01(\x03H\x00\x12%\n\x04seed\x18\x03 \x01(\x0b\x32\x17.sarus_data_spec.ScalarB\x0c\n\nproportion\x1a\x1a\n\x18PrivacyUnitTrackingPaths\x1a\r\n\x0bPublicPaths\x1a.\n\x07GetItem\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x1a\x0e\n\x0c\x41ssignBudget\x1a\x11\n\x0f\x41utomaticBudget\x1a\x12\n\x10\x41ttributesBudget\x1a\n\n\x08SDBudget\x1a$\n\nDeriveSeed\x12\x16\n\x0erandom_integer\x18\x01 \x01(\x03\x1a\x0b\n\tGroupByPE\x1a\x10\n\x0eSamplingRatios\x1a\x12\n\x10RelationshipSpec\x1a\x88\x01\n\tSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a\x8a\x01\n\x0b\x44PSelectSql\x12\x0f\n\x05query\x18\x01 \x01(\tH\x00\x12\x34\n\x0f\x61liased_queries\x18\x02 \x01(\x0b\x32\x19.Transform.AliasedQueriesH\x00\x12*\n\x0bsql_dialect\x18\x03 \x01(\x0e\x32\x15.Transform.SQLDialectB\x08\n\x06select\x1a@\n\x0e\x41liasedQueries\x12.\n\raliased_query\x18\x01 \x03(\x0b\x32\x17.Transform.AliasedQuery\x1a\x42\n\x0c\x41liasedQuery\x12#\n\x04path\x18\x01 \x01(\x0b\x32\x15.sarus_data_spec.Path\x12\r\n\x05query\x18\x02 \x01(\t\x1a\x17\n\x07\x45xtract\x12\x0c\n\x04size\x18\x01 \x01(\x05\x1a\x13\n\x11ValidatedUserType\x1a\x11\n\x0f\x45rrorEstimation\x1aV\n\x08\x46itModel\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x02 \x01(\x05\x12&\n\ttext_kind\x18\x03 \x01(\x0b\x32\x13.Transform.TextKind\x1aN\n\x08TextKind\x12\x14\n\ntext_field\x18\x01 \x01(\tH\x00\x12\x1f\n\x04\x63hat\x18\x02 \x01(\x0b\x32\x0f.Transform.ChatH\x00\x42\x0b\n\ttext_kind\x1a\x34\n\x04\x43hat\x12\x16\n\x0equestion_field\x18\x01 \x01(\t\x12\x14\n\x0c\x61nswer_field\x18\x02 \x01(\t\x1an\n\nFitModelDP\x12\x12\n\nbatch_size\x18\x01 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x03 \x01(\x05\x12\x14\n\x0cl2_norm_clip\x18\x04 \x01(\x01\x12&\n\ttext_kind\x18\x05 \x01(\x0b\x32\x13.Transform.TextKind\x1a@\n\x11GenerateFromModel\x12\x16\n\x0emax_new_tokens\x18\x01 \x01(\x05\x12\x13\n\x0btemperature\x18\x02 \x01(\x01\"\x80\x01\n\nSQLDialect\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08POSTGRES\x10\x01\x12\x0e\n\nSQL_SERVER\x10\x02\x12\n\n\x06MY_SQL\x10\x03\x12\x0b\n\x07SQLLITE\x10\x04\x12\n\n\x06ORACLE\x10\x05\x12\r\n\tBIG_QUERY\x10\x06\x12\x0c\n\x08REDSHIFT\x10\x07\x12\x08\n\x04HIVE\x10\x08\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sarus_data_spec.protobuf.transform_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _TRANSFORM_PROPERTIESENTRY._options = None
   _TRANSFORM_PROPERTIESENTRY._serialized_options = b'8\001'
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._options = None
   _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_options = b'8\001'
   _TRANSFORM._serialized_start=158
-  _TRANSFORM._serialized_end=5425
+  _TRANSFORM._serialized_end=5487
   _TRANSFORM_PROPERTIESENTRY._serialized_start=338
   _TRANSFORM_PROPERTIESENTRY._serialized_end=387
   _TRANSFORM_SPEC._serialized_start=390
-  _TRANSFORM_SPEC._serialized_end=2160
-  _TRANSFORM_EXTERNAL._serialized_start=2163
-  _TRANSFORM_EXTERNAL._serialized_end=3177
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2277
-  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=2876
-  _TRANSFORM_EXTERNAL_STD._serialized_start=2878
-  _TRANSFORM_EXTERNAL_STD._serialized_end=2897
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=2899
-  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=2921
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=2923
-  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=2944
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=2946
-  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=2972
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=2974
-  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=2997
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=2999
-  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3030
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3032
-  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3055
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3057
-  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3078
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3080
-  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3104
-  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3106
-  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3126
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3128
-  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3149
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3151
-  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3177
-  _TRANSFORM_IDENTITY._serialized_start=3179
-  _TRANSFORM_IDENTITY._serialized_end=3189
-  _TRANSFORM_VARIABLE._serialized_start=3191
-  _TRANSFORM_VARIABLE._serialized_end=3233
-  _TRANSFORM_COMPOSED._serialized_start=3236
-  _TRANSFORM_COMPOSED._serialized_end=3405
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3352
-  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3405
-  _TRANSFORM_PROJECT._serialized_start=3407
-  _TRANSFORM_PROJECT._serialized_end=3459
-  _TRANSFORM_FILTER._serialized_start=3461
-  _TRANSFORM_FILTER._serialized_end=3508
-  _TRANSFORM_SHUFFLE._serialized_start=3510
-  _TRANSFORM_SHUFFLE._serialized_end=3519
-  _TRANSFORM_JOIN._serialized_start=3521
-  _TRANSFORM_JOIN._serialized_end=3562
-  _TRANSFORM_CAST._serialized_start=3564
-  _TRANSFORM_CAST._serialized_end=3607
-  _TRANSFORM_SAMPLE._serialized_start=3609
-  _TRANSFORM_SAMPLE._serialized_end=3706
-  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3708
-  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3826
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3787
-  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3826
-  _TRANSFORM_GROUPBY._serialized_start=3828
-  _TRANSFORM_GROUPBY._serialized_end=3850
-  _TRANSFORM_TOSMALLDATA._serialized_start=3852
-  _TRANSFORM_TOSMALLDATA._serialized_end=3943
-  _TRANSFORM_SYNTHETIC._serialized_start=3945
-  _TRANSFORM_SYNTHETIC._serialized_end=3956
-  _TRANSFORM_USERSETTINGS._serialized_start=3958
-  _TRANSFORM_USERSETTINGS._serialized_end=3972
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=3974
-  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4021
-  _TRANSFORM_PROTECT._serialized_start=4023
-  _TRANSFORM_PROTECT._serialized_end=4032
-  _TRANSFORM_TRANSCODE._serialized_start=4034
-  _TRANSFORM_TRANSCODE._serialized_end=4045
-  _TRANSFORM_INVERSETRANSCODE._serialized_start=4047
-  _TRANSFORM_INVERSETRANSCODE._serialized_end=4065
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4067
-  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4178
-  _TRANSFORM_PROTECTEDPATHS._serialized_start=4180
-  _TRANSFORM_PROTECTEDPATHS._serialized_end=4196
-  _TRANSFORM_PUBLICPATHS._serialized_start=4198
-  _TRANSFORM_PUBLICPATHS._serialized_end=4211
-  _TRANSFORM_GETITEM._serialized_start=4213
-  _TRANSFORM_GETITEM._serialized_end=4259
-  _TRANSFORM_ASSIGNBUDGET._serialized_start=4261
-  _TRANSFORM_ASSIGNBUDGET._serialized_end=4275
-  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4277
-  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4294
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4296
-  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4314
-  _TRANSFORM_SDBUDGET._serialized_start=4316
-  _TRANSFORM_SDBUDGET._serialized_end=4326
-  _TRANSFORM_DERIVESEED._serialized_start=4328
-  _TRANSFORM_DERIVESEED._serialized_end=4364
-  _TRANSFORM_GROUPBYPE._serialized_start=4366
-  _TRANSFORM_GROUPBYPE._serialized_end=4377
-  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4379
-  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4395
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4397
-  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4415
-  _TRANSFORM_SELECTSQL._serialized_start=4418
-  _TRANSFORM_SELECTSQL._serialized_end=4554
-  _TRANSFORM_DPSELECTSQL._serialized_start=4557
-  _TRANSFORM_DPSELECTSQL._serialized_end=4695
-  _TRANSFORM_ALIASEDQUERIES._serialized_start=4697
-  _TRANSFORM_ALIASEDQUERIES._serialized_end=4761
-  _TRANSFORM_ALIASEDQUERY._serialized_start=4763
-  _TRANSFORM_ALIASEDQUERY._serialized_end=4829
-  _TRANSFORM_EXTRACT._serialized_start=4831
-  _TRANSFORM_EXTRACT._serialized_end=4854
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=4856
-  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=4875
-  _TRANSFORM_ERRORESTIMATION._serialized_start=4877
-  _TRANSFORM_ERRORESTIMATION._serialized_end=4894
-  _TRANSFORM_FITMODEL._serialized_start=4896
-  _TRANSFORM_FITMODEL._serialized_end=4982
-  _TRANSFORM_TEXTKIND._serialized_start=4984
-  _TRANSFORM_TEXTKIND._serialized_end=5062
-  _TRANSFORM_CHAT._serialized_start=5064
-  _TRANSFORM_CHAT._serialized_end=5116
-  _TRANSFORM_FITMODELDP._serialized_start=5118
-  _TRANSFORM_FITMODELDP._serialized_end=5228
-  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5230
-  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5294
-  _TRANSFORM_SQLDIALECT._serialized_start=5297
-  _TRANSFORM_SQLDIALECT._serialized_end=5425
+  _TRANSFORM_SPEC._serialized_end=2200
+  _TRANSFORM_EXTERNAL._serialized_start=2203
+  _TRANSFORM_EXTERNAL._serialized_end=3217
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_start=2317
+  _TRANSFORM_EXTERNAL_OPIDENTIFIER._serialized_end=2916
+  _TRANSFORM_EXTERNAL_STD._serialized_start=2918
+  _TRANSFORM_EXTERNAL_STD._serialized_end=2937
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_start=2939
+  _TRANSFORM_EXTERNAL_PANDAS._serialized_end=2961
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_start=2963
+  _TRANSFORM_EXTERNAL_NUMPY._serialized_end=2984
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_start=2986
+  _TRANSFORM_EXTERNAL_TENSORFLOW._serialized_end=3012
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_start=3014
+  _TRANSFORM_EXTERNAL_SKLEARN._serialized_end=3037
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_start=3039
+  _TRANSFORM_EXTERNAL_PANDASPROFILING._serialized_end=3070
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_start=3072
+  _TRANSFORM_EXTERNAL_XGBOOST._serialized_end=3095
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_start=3097
+  _TRANSFORM_EXTERNAL_SKOPT._serialized_end=3118
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_start=3120
+  _TRANSFORM_EXTERNAL_IMBLEARN._serialized_end=3144
+  _TRANSFORM_EXTERNAL_SHAP._serialized_start=3146
+  _TRANSFORM_EXTERNAL_SHAP._serialized_end=3166
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_start=3168
+  _TRANSFORM_EXTERNAL_SCIPY._serialized_end=3189
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_start=3191
+  _TRANSFORM_EXTERNAL_OPTBINNING._serialized_end=3217
+  _TRANSFORM_IDENTITY._serialized_start=3219
+  _TRANSFORM_IDENTITY._serialized_end=3229
+  _TRANSFORM_VARIABLE._serialized_start=3231
+  _TRANSFORM_VARIABLE._serialized_end=3273
+  _TRANSFORM_COMPOSED._serialized_start=3276
+  _TRANSFORM_COMPOSED._serialized_end=3445
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_start=3392
+  _TRANSFORM_COMPOSED_NAMEDARGUMENTSENTRY._serialized_end=3445
+  _TRANSFORM_PROJECT._serialized_start=3447
+  _TRANSFORM_PROJECT._serialized_end=3499
+  _TRANSFORM_FILTER._serialized_start=3501
+  _TRANSFORM_FILTER._serialized_end=3548
+  _TRANSFORM_SHUFFLE._serialized_start=3550
+  _TRANSFORM_SHUFFLE._serialized_end=3559
+  _TRANSFORM_JOIN._serialized_start=3561
+  _TRANSFORM_JOIN._serialized_end=3602
+  _TRANSFORM_CAST._serialized_start=3604
+  _TRANSFORM_CAST._serialized_end=3647
+  _TRANSFORM_SAMPLE._serialized_start=3649
+  _TRANSFORM_SAMPLE._serialized_end=3746
+  _TRANSFORM_SCHEMAINFERENCE._serialized_start=3748
+  _TRANSFORM_SCHEMAINFERENCE._serialized_end=3866
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_start=3827
+  _TRANSFORM_SCHEMAINFERENCE_CASTPOLICY._serialized_end=3866
+  _TRANSFORM_GROUPBY._serialized_start=3868
+  _TRANSFORM_GROUPBY._serialized_end=3890
+  _TRANSFORM_TOSMALLDATA._serialized_start=3892
+  _TRANSFORM_TOSMALLDATA._serialized_end=3983
+  _TRANSFORM_SYNTHETIC._serialized_start=3985
+  _TRANSFORM_SYNTHETIC._serialized_end=3996
+  _TRANSFORM_USERSETTINGS._serialized_start=3998
+  _TRANSFORM_USERSETTINGS._serialized_end=4012
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_start=4014
+  _TRANSFORM_AUTOMATICUSERSETTINGS._serialized_end=4061
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_start=4063
+  _TRANSFORM_PRIVACYUNITTRACKING._serialized_end=4084
+  _TRANSFORM_TRANSCODE._serialized_start=4086
+  _TRANSFORM_TRANSCODE._serialized_end=4097
+  _TRANSFORM_INVERSETRANSCODE._serialized_start=4099
+  _TRANSFORM_INVERSETRANSCODE._serialized_end=4117
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_start=4119
+  _TRANSFORM_DIFFERENTIATEDSAMPLE._serialized_end=4230
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_start=4232
+  _TRANSFORM_PRIVACYUNITTRACKINGPATHS._serialized_end=4258
+  _TRANSFORM_PUBLICPATHS._serialized_start=4260
+  _TRANSFORM_PUBLICPATHS._serialized_end=4273
+  _TRANSFORM_GETITEM._serialized_start=4275
+  _TRANSFORM_GETITEM._serialized_end=4321
+  _TRANSFORM_ASSIGNBUDGET._serialized_start=4323
+  _TRANSFORM_ASSIGNBUDGET._serialized_end=4337
+  _TRANSFORM_AUTOMATICBUDGET._serialized_start=4339
+  _TRANSFORM_AUTOMATICBUDGET._serialized_end=4356
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_start=4358
+  _TRANSFORM_ATTRIBUTESBUDGET._serialized_end=4376
+  _TRANSFORM_SDBUDGET._serialized_start=4378
+  _TRANSFORM_SDBUDGET._serialized_end=4388
+  _TRANSFORM_DERIVESEED._serialized_start=4390
+  _TRANSFORM_DERIVESEED._serialized_end=4426
+  _TRANSFORM_GROUPBYPE._serialized_start=4428
+  _TRANSFORM_GROUPBYPE._serialized_end=4439
+  _TRANSFORM_SAMPLINGRATIOS._serialized_start=4441
+  _TRANSFORM_SAMPLINGRATIOS._serialized_end=4457
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_start=4459
+  _TRANSFORM_RELATIONSHIPSPEC._serialized_end=4477
+  _TRANSFORM_SELECTSQL._serialized_start=4480
+  _TRANSFORM_SELECTSQL._serialized_end=4616
+  _TRANSFORM_DPSELECTSQL._serialized_start=4619
+  _TRANSFORM_DPSELECTSQL._serialized_end=4757
+  _TRANSFORM_ALIASEDQUERIES._serialized_start=4759
+  _TRANSFORM_ALIASEDQUERIES._serialized_end=4823
+  _TRANSFORM_ALIASEDQUERY._serialized_start=4825
+  _TRANSFORM_ALIASEDQUERY._serialized_end=4891
+  _TRANSFORM_EXTRACT._serialized_start=4893
+  _TRANSFORM_EXTRACT._serialized_end=4916
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_start=4918
+  _TRANSFORM_VALIDATEDUSERTYPE._serialized_end=4937
+  _TRANSFORM_ERRORESTIMATION._serialized_start=4939
+  _TRANSFORM_ERRORESTIMATION._serialized_end=4956
+  _TRANSFORM_FITMODEL._serialized_start=4958
+  _TRANSFORM_FITMODEL._serialized_end=5044
+  _TRANSFORM_TEXTKIND._serialized_start=5046
+  _TRANSFORM_TEXTKIND._serialized_end=5124
+  _TRANSFORM_CHAT._serialized_start=5126
+  _TRANSFORM_CHAT._serialized_end=5178
+  _TRANSFORM_FITMODELDP._serialized_start=5180
+  _TRANSFORM_FITMODELDP._serialized_end=5290
+  _TRANSFORM_GENERATEFROMMODEL._serialized_start=5292
+  _TRANSFORM_GENERATEFROMMODEL._serialized_end=5356
+  _TRANSFORM_SQLDIALECT._serialized_start=5359
+  _TRANSFORM_SQLDIALECT._serialized_end=5487
 # @@protoc_insertion_point(module_scope)
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/transform_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/transform_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -66,21 +66,21 @@
         PROJECT_FIELD_NUMBER: builtins.int
         FILTER_FIELD_NUMBER: builtins.int
         SHUFFLE_FIELD_NUMBER: builtins.int
         JOIN_FIELD_NUMBER: builtins.int
         CAST_FIELD_NUMBER: builtins.int
         SAMPLE_FIELD_NUMBER: builtins.int
         USER_SETTINGS_FIELD_NUMBER: builtins.int
-        PROTECT_DATASET_FIELD_NUMBER: builtins.int
+        PRIVACY_UNIT_TRACKING_FIELD_NUMBER: builtins.int
         EXTERNAL_FIELD_NUMBER: builtins.int
         SYNTHETIC_FIELD_NUMBER: builtins.int
         TRANSCODE_FIELD_NUMBER: builtins.int
         INVERSE_TRANSCODE_FIELD_NUMBER: builtins.int
         GET_ITEM_FIELD_NUMBER: builtins.int
-        PROTECTED_PATHS_FIELD_NUMBER: builtins.int
+        PRIVACY_UNIT_TRACKING_PATHS_FIELD_NUMBER: builtins.int
         AUTOMATIC_USER_SETTINGS_FIELD_NUMBER: builtins.int
         PUBLIC_PATHS_FIELD_NUMBER: builtins.int
         ASSIGN_BUDGET_FIELD_NUMBER: builtins.int
         AUTOMATIC_BUDGET_FIELD_NUMBER: builtins.int
         ATTRIBUTE_BUDGET_FIELD_NUMBER: builtins.int
         SD_BUDGET_FIELD_NUMBER: builtins.int
         DERIVE_SEED_FIELD_NUMBER: builtins.int
@@ -114,29 +114,29 @@
         @property
         def cast(self) -> global___Transform.Cast: ...
         @property
         def sample(self) -> global___Transform.Sample: ...
         @property
         def user_settings(self) -> global___Transform.UserSettings: ...
         @property
-        def protect_dataset(self) -> global___Transform.Protect: ...
+        def privacy_unit_tracking(self) -> global___Transform.PrivacyUnitTracking: ...
         @property
         def external(self) -> global___Transform.External:
             """np transforms, pd transforms,..."""
             pass
         @property
         def synthetic(self) -> global___Transform.Synthetic: ...
         @property
         def transcode(self) -> global___Transform.Transcode: ...
         @property
         def inverse_transcode(self) -> global___Transform.InverseTranscode: ...
         @property
         def get_item(self) -> global___Transform.GetItem: ...
         @property
-        def protected_paths(self) -> global___Transform.ProtectedPaths: ...
+        def privacy_unit_tracking_paths(self) -> global___Transform.PrivacyUnitTrackingPaths: ...
         @property
         def automatic_user_settings(self) -> global___Transform.AutomaticUserSettings: ...
         @property
         def public_paths(self) -> global___Transform.PublicPaths: ...
         @property
         def assign_budget(self) -> global___Transform.AssignBudget: ...
         @property
@@ -183,21 +183,21 @@
             project : typing.Optional[global___Transform.Project] = ...,
             filter : typing.Optional[global___Transform.Filter] = ...,
             shuffle : typing.Optional[global___Transform.Shuffle] = ...,
             join : typing.Optional[global___Transform.Join] = ...,
             cast : typing.Optional[global___Transform.Cast] = ...,
             sample : typing.Optional[global___Transform.Sample] = ...,
             user_settings : typing.Optional[global___Transform.UserSettings] = ...,
-            protect_dataset : typing.Optional[global___Transform.Protect] = ...,
+            privacy_unit_tracking : typing.Optional[global___Transform.PrivacyUnitTracking] = ...,
             external : typing.Optional[global___Transform.External] = ...,
             synthetic : typing.Optional[global___Transform.Synthetic] = ...,
             transcode : typing.Optional[global___Transform.Transcode] = ...,
             inverse_transcode : typing.Optional[global___Transform.InverseTranscode] = ...,
             get_item : typing.Optional[global___Transform.GetItem] = ...,
-            protected_paths : typing.Optional[global___Transform.ProtectedPaths] = ...,
+            privacy_unit_tracking_paths : typing.Optional[global___Transform.PrivacyUnitTrackingPaths] = ...,
             automatic_user_settings : typing.Optional[global___Transform.AutomaticUserSettings] = ...,
             public_paths : typing.Optional[global___Transform.PublicPaths] = ...,
             assign_budget : typing.Optional[global___Transform.AssignBudget] = ...,
             automatic_budget : typing.Optional[global___Transform.AutomaticBudget] = ...,
             attribute_budget : typing.Optional[global___Transform.AttributesBudget] = ...,
             sd_budget : typing.Optional[global___Transform.SDBudget] = ...,
             derive_seed : typing.Optional[global___Transform.DeriveSeed] = ...,
@@ -211,17 +211,17 @@
             dp_select_sql : typing.Optional[global___Transform.DPSelectSql] = ...,
             error_estimation : typing.Optional[global___Transform.ErrorEstimation] = ...,
             fit_model : typing.Optional[global___Transform.FitModel] = ...,
             fit_model_dp : typing.Optional[global___Transform.FitModelDP] = ...,
             generate_from_model : typing.Optional[global___Transform.GenerateFromModel] = ...,
             to_small_data : typing.Optional[global___Transform.ToSmallData] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","project",b"project","protect_dataset",b"protect_dataset","protected_paths",b"protected_paths","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","project",b"project","protect_dataset",b"protect_dataset","protected_paths",b"protected_paths","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","protect_dataset","external","synthetic","transcode","inverse_transcode","get_item","protected_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data"]]: ...
+        def HasField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["assign_budget",b"assign_budget","attribute_budget",b"attribute_budget","automatic_budget",b"automatic_budget","automatic_user_settings",b"automatic_user_settings","cast",b"cast","composed",b"composed","derive_seed",b"derive_seed","differentiated_sample",b"differentiated_sample","dp_select_sql",b"dp_select_sql","error_estimation",b"error_estimation","external",b"external","extract",b"extract","filter",b"filter","fit_model",b"fit_model","fit_model_dp",b"fit_model_dp","generate_from_model",b"generate_from_model","get_item",b"get_item","group_by_pe",b"group_by_pe","identity",b"identity","inverse_transcode",b"inverse_transcode","join",b"join","privacy_unit_tracking",b"privacy_unit_tracking","privacy_unit_tracking_paths",b"privacy_unit_tracking_paths","project",b"project","public_paths",b"public_paths","relationship_spec",b"relationship_spec","sample",b"sample","sampling_ratios",b"sampling_ratios","sd_budget",b"sd_budget","select_sql",b"select_sql","shuffle",b"shuffle","spec",b"spec","synthetic",b"synthetic","to_small_data",b"to_small_data","transcode",b"transcode","user_settings",b"user_settings","validated_user_type",b"validated_user_type","variable",b"variable"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["spec",b"spec"]) -> typing.Optional[typing_extensions.Literal["identity","variable","composed","project","filter","shuffle","join","cast","sample","user_settings","privacy_unit_tracking","external","synthetic","transcode","inverse_transcode","get_item","privacy_unit_tracking_paths","automatic_user_settings","public_paths","assign_budget","automatic_budget","attribute_budget","sd_budget","derive_seed","group_by_pe","sampling_ratios","select_sql","extract","relationship_spec","differentiated_sample","validated_user_type","dp_select_sql","error_estimation","fit_model","fit_model_dp","generate_from_model","to_small_data"]]: ...
 
     class External(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         class OpIdentifier(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
             STD_FIELD_NUMBER: builtins.int
             PANDAS_FIELD_NUMBER: builtins.int
@@ -614,15 +614,15 @@
         max_categories: builtins.int = ...
         def __init__(self,
             *,
             max_categories : builtins.int = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["max_categories",b"max_categories"]) -> None: ...
 
-    class Protect(google.protobuf.message.Message):
+    class PrivacyUnitTracking(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class Transcode(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
@@ -648,15 +648,15 @@
             size : builtins.int = ...,
             seed : typing.Optional[sarus_data_spec.protobuf.scalar_pb2.Scalar] = ...,
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["fraction",b"fraction","proportion",b"proportion","seed",b"seed","size",b"size"]) -> None: ...
         def WhichOneof(self, oneof_group: typing_extensions.Literal["proportion",b"proportion"]) -> typing.Optional[typing_extensions.Literal["fraction","size"]]: ...
 
-    class ProtectedPaths(google.protobuf.message.Message):
+    class PrivacyUnitTrackingPaths(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
             ) -> None: ...
 
     class PublicPaths(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         def __init__(self,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type.proto` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type.proto`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type_pb2.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/type_pb2.pyi` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/typing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-"""Protocols describing common object behaviors
-"""
+"""Protocols describing common object behaviors"""
+
 from typing import (
     ByteString,
     MutableMapping,
     Protocol,
     TypeVar,
     Union,
     runtime_checkable,
 )
 
 from google.protobuf.descriptor import Descriptor
 
-M = TypeVar('M')
+M = TypeVar("M")
 
 
 @runtime_checkable
 class Protobuf(Protocol):
     """A protobuf message.
     Only the used methods are defined in this protocol.
     We assume all protobuf messages have properties
     """
 
     DESCRIPTOR: Descriptor
 
-    def CopyFrom(self: M, other_msg: M) -> None:
-        ...
+    def CopyFrom(self: M, other_msg: M) -> None: ...
 
-    def SerializeToString(self: M, deterministic: bool) -> bytes:
-        ...
+    def SerializeToString(self: M, deterministic: bool) -> bytes: ...
 
-    def FromString(self: M, s: Union[ByteString, bytes]) -> M:
-        ...
+    def FromString(self: M, s: Union[ByteString, bytes]) -> M: ...
 
     @property
-    def properties(self) -> MutableMapping:
-        ...
+    def properties(self) -> MutableMapping: ...
 
 
 @runtime_checkable
 class ProtobufWithUUID(Protobuf, Protocol):
     uuid: str
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/protobuf/utilities.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/protobuf/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def unwrap(wrapped_message: AnyProto) -> Protobuf:
     """Unwrap an Any to a Message"""
     result = message(wrapped_message.TypeName())  # type: ignore
     wrapped_message.Unpack(result)
     return result
 
 
-M = TypeVar('M', bound=Protobuf)
+M = TypeVar("M", bound=Protobuf)
 
 
 def copy(value: M) -> M:
     result = message(value.DESCRIPTOR.full_name)
     result.CopyFrom(value)
     return cast(M, result)
 
@@ -78,20 +78,20 @@
 
 def json_serialize(message: Protobuf) -> bytes:
     return MessageToJson(
         wrap(message),
         including_default_value_fields=True,
         preserving_proto_field_name=True,
         sort_keys=True,
-    ).encode('utf8')
+    ).encode("utf8")
 
 
 def json_deserialize(bytes: bytes) -> Protobuf:
     wrapped_message: AnyProto = AnyProto()
-    Parse(bytes.decode('utf8'), wrapped_message)
+    Parse(bytes.decode("utf8"), wrapped_message)
     return unwrap(wrapped_message)
 
 
 def dict_serialize(message: Protobuf) -> Dict[str, Any]:
     return MessageToDict(
         wrap(message),
         including_default_value_fields=True,
@@ -117,15 +117,15 @@
 def dejson(string: str) -> Protobuf:
     wrapped_message: AnyProto = AnyProto()
     Parse(string, wrapped_message)
     return unwrap(wrapped_message)
 
 
 def to_base64(message: Protobuf) -> str:
-    return base64.b64encode(serialize(message)).decode('ASCII')
+    return base64.b64encode(serialize(message)).decode("ASCII")
 
 
 def from_base64(string: str, message: Optional[M] = None) -> M:
     return cast(M, unwrap(AnyProto().FromString(base64.b64decode(string))))
 
 
 def serialize_protos_list(protos: List[M]) -> str:
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/scalar.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/scalar.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def name(self) -> str:
         return self._protobuf.name
 
     def doc(self) -> str:
         return self._protobuf.doc
 
     def spec(self) -> str:
-        return str(self._protobuf.spec.WhichOneof('spec'))
+        return str(self._protobuf.spec.WhichOneof("spec"))
 
     def is_transformed(self) -> bool:
         """Is the scalar composed."""
         return self._protobuf.spec.HasField("transformed")
 
     def is_remote(self) -> bool:
         """Is the dataspec a remotely defined dataset."""
@@ -66,17 +66,17 @@
             self._protobuf.spec.model.WhichOneof("type") == "pretrained_model"
         )
 
     def is_fitted_model(self) -> bool:
         if not self.is_transformed():
             return False
         transform = self.transform()
-        return transform.protobuf().spec.WhichOneof('spec') in [
-            'fit_model',
-            'fit_model_dp',
+        return transform.protobuf().spec.WhichOneof("spec") in [
+            "fit_model",
+            "fit_model_dp",
         ]
 
     def is_privacy_params(self) -> bool:
         """Is the scalar privacy parameters."""
         return self._protobuf.spec.HasField("privacy_params")
 
     def is_random_seed(self) -> bool:
@@ -89,23 +89,23 @@
                 return True
         return False
 
     def is_synthetic_model(self) -> bool:
         """Is the scalar composed."""
         return self._protobuf.spec.HasField("synthetic_model")
 
-    def is_pep(self) -> bool:
-        """Is the scalar PEP."""
+    def is_pup(self) -> bool:
+        """Is the scalar PUP."""
         return False
 
-    def pep_token(self) -> Optional[str]:
-        """Returns the scalar PEP token."""
+    def pup_token(self) -> Optional[str]:
+        """Returns the scalar PUP token."""
         return None
 
-    def rewritten_pep_token(self) -> Optional[str]:
+    def rewritten_pup_token(self) -> Optional[str]:
         return None
 
     def is_synthetic(self) -> bool:
         """Is the scalar synthetic."""
         return self.manager().dataspec_validator().is_synthetic(self)
 
     def is_dp(self) -> bool:
@@ -117,16 +117,16 @@
         return self.manager().dataspec_validator().is_public(self)
 
     def is_dp_writable(self) -> bool:
         """Check if it exists a variant of this dataspec
         that utilizes the dp equivalent, and this variant is is_dp."""
         return self.manager().dataspec_validator().is_dp_writable(self)
 
-    def is_pep_writable(self) -> bool:
-        """Check if it exists a variant of this dataspec that is is_pep."""
+    def is_pup_writable(self) -> bool:
+        """Check if it exists a variant of this dataspec that is is_pup."""
         return False
 
     def is_publishable(self) -> bool:
         """Check if it exists a variant of this dataspec that is published"""
         return self.manager().dataspec_validator().is_publishable(self)
 
     def is_published(self) -> bool:
@@ -295,22 +295,22 @@
                             "Dataset",
                         )
                     else:
                         self.nodes[visited.uuid()] = (visited.name(), "Scalar")
 
                     if not visited.is_remote():
                         for argument in arguments:
-                            self.edges[
-                                (argument.uuid(), visited.uuid())
-                            ] = transform.name()
+                            self.edges[(argument.uuid(), visited.uuid())] = (
+                                transform.name()
+                            )
                             argument.accept(self)
                         for _, argument in named_arguments.items():
-                            self.edges[
-                                (argument.uuid(), visited.uuid())
-                            ] = transform.name()
+                            self.edges[(argument.uuid(), visited.uuid())] = (
+                                transform.name()
+                            )
                             argument.accept(self)
                     self.visited.add(visited)
 
             def other(self, visited: st.DataSpec) -> None:
                 if visited.prototype() == sp.Dataset:
                     self.nodes[visited.uuid()] = (
                         visited.name(),
@@ -320,37 +320,37 @@
                     self.nodes[visited.uuid()] = (visited.name(), "Scalar")
 
             def all(self, visited: st.DataSpec) -> None:
                 pass
 
         visitor = Dot()
         self.accept(visitor)
-        result = 'digraph {'
+        result = "digraph {"
         for uuid, (label, node_type) in visitor.nodes.items():
             shape = "polygon" if node_type == "Scalar" else "ellipse"
             result += (
                 f'\n"{uuid}" [label="{label} ({uuid[:2]})", shape={shape}];'
             )
         for (u1, u2), label in visitor.edges.items():
             result += f'\n"{u1}" -> "{u2}" [label="{label} ({uuid[:2]})"];'
-        result += '}'
+        result += "}"
         return result
 
     def attribute(self, name: str) -> Optional[st.Attribute]:
         return self.manager().attribute(name=name, dataspec=self)
 
     def attributes(self, name: str) -> List[st.Attribute]:
         return self.manager().attributes(name=name, dataspec=self)
 
 
 def privacy_budget(privacy_limit: st.PrivacyLimit) -> Scalar:
     delta_epsilon_dict = privacy_limit.delta_epsilon_dict()
     return Scalar(
         sp.Scalar(
-            name='privacy_budget',
+            name="privacy_budget",
             spec=sp.Scalar.Spec(
                 privacy_params=sp.Scalar.PrivacyParameters(
                     points=[
                         sp.Scalar.PrivacyParameters.Point(
                             epsilon=epsilon, delta=delta
                         )
                         for delta, epsilon in delta_epsilon_dict.items()
@@ -360,26 +360,26 @@
         )
     )
 
 
 def random_seed(value: int) -> Scalar:
     return Scalar(
         sp.Scalar(
-            name='seed',
+            name="seed",
             spec=sp.Scalar.Spec(random_seed=sp.Scalar.RandomSeed(value=value)),
         )
     )
 
 
 def pretrained_model(
-    foundation_model_name: str, peft_initialisation_uri: str = ''
+    foundation_model_name: str, peft_initialisation_uri: str = ""
 ) -> Scalar:
     return Scalar(
         sp.Scalar(
-            name='Pretrained Model',
+            name="Pretrained Model",
             spec=sp.Scalar.Spec(
                 model=sp.Scalar.Model(
                     pretrained_model=sp.Scalar.Model.PretrainedModel(
                         foundation_model_name=foundation_model_name,
                         peft_initialisation_uri=peft_initialisation_uri,
                     )
                 ),
@@ -387,17 +387,17 @@
         )
     )
 
 
 def synthetic_model() -> Scalar:
     return Scalar(
         sp.Scalar(
-            name='synthetic_model',
+            name="synthetic_model",
             spec=sp.Scalar.Spec(synthetic_model=sp.Scalar.SyntheticModel()),
-            properties={'creation_time': str(datetime.datetime.now())},
+            properties={"creation_time": str(datetime.datetime.now())},
         )
     )
 
 
 class Visitor:
     """A visitor class for Scalar"""
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/schema.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,26 +41,26 @@
 
     def type(self) -> Type:
         """Returns the first type level of the schema"""
         return self._type
 
     def data_type(self) -> Type:
         """Returns the first type level containing the data,
-        hence skips the protected_entity struct if there is one"""
+        hence skips the privacy_unit struct if there is one"""
         return self.type().data_type()
 
     def has_admin_columns(self) -> bool:
         return self.type().has_admin_columns()
 
-    def is_protected(self) -> bool:
-        return self.type().has_protection()
+    def is_privacy_unit_tracking(self) -> bool:
+        return self.type().has_privacy_unit_tracking()
 
-    def protected_path(self) -> Path:
-        """Returns the path to the protected entities"""
-        return Path(self.protobuf().protected)
+    def privacy_unit_tracking_paths(self) -> Path:
+        """Returns the path to the privacy unit"""
+        return Path(self.protobuf().privacy_unit)
 
     # TODO: Add to_parquet, to_tensorflow, to_sql... here?
     # The Schema has a manager, it would provide the implementation
 
     def tables(self) -> t.List[st.Path]:
         struct_paths = self.data_type().structs()
         if struct_paths is None:  # there is no struct
@@ -90,22 +90,22 @@
 
 
 # Builder
 def schema(
     dataset: st.Dataset,
     fields: t.Optional[t.Mapping[str, st.Type]] = None,
     schema_type: t.Optional[st.Type] = None,
-    protected_paths: t.Optional[sp.Path] = None,
+    privacy_unit_tracking_paths: t.Optional[sp.Path] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
     name: t.Optional[str] = None,
 ) -> Schema:
     """A builder to ease the construction of a schema"""
     if name is None:
         name = dataset.properties().get(
-            DATASET_SLUGNAME, f'{dataset.name()}_schema'
+            DATASET_SLUGNAME, f"{dataset.name()}_schema"
         )
     assert name is not None
 
     if fields is not None:
         return Schema(
             sp.Schema(
                 dataset=dataset.uuid(),
@@ -116,35 +116,35 @@
                             sp.Type.Struct.Field(
                                 name=name, type=type.protobuf()
                             )
                             for name, type in fields.items()
                         ]
                     )
                 ),
-                protected=protected_paths,
+                privacy_unit=privacy_unit_tracking_paths,
                 properties=properties,
             )
         )
     if schema_type is not None:
         return Schema(
             sp.Schema(
                 dataset=dataset.uuid(),
                 name=name,
                 type=schema_type.protobuf(),
-                protected=protected_paths,
+                privacy_unit=privacy_unit_tracking_paths,
                 properties=properties,
             )
         )
     # If none of fields or type is defined, set type to Null
     return Schema(
         sp.Schema(
             dataset=dataset.uuid(),
             name=name,
-            type=sp.Type(name='Null', null=sp.Type.Null()),
-            protected=protected_paths,
+            type=sp.Type(name="Null", null=sp.Type.Null()),
+            privacy_unit=privacy_unit_tracking_paths,
             properties=properties,
         )
     )
 
 
 if t.TYPE_CHECKING:
-    test_schema: st.Schema = schema(sd.sql(uri='sqlite:///:memory:'))
+    test_schema: st.Schema = schema(sd.sql(uri="sqlite:///:memory:"))
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/size.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/size.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # Builder
 def size(
     dataset: st.Dataset,
     statistics: t.Optional[st.Statistics] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Size:
-    name = f'{dataset.name()}_sizes'
+    name = f"{dataset.name()}_sizes"
 
     return Size(
         sp.Size(
             dataset=dataset.uuid(),
             name=name,
             statistics=statistics.protobuf()
             if statistics is not None
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/statistics.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,45 +21,45 @@
         """Return the statistics name"""
         return self.protobuf().name
 
     def distribution(self) -> st.Distribution:
         return Distribution(
             getattr(
                 self.protobuf(),
-                t.cast(str, self.protobuf().WhichOneof('statistics')),
+                t.cast(str, self.protobuf().WhichOneof("statistics")),
             ).distribution
         )
 
     def size(self) -> int:
         return t.cast(
             int,
             getattr(
                 self.protobuf(),
-                t.cast(str, self.protobuf().WhichOneof('statistics')),
+                t.cast(str, self.protobuf().WhichOneof("statistics")),
             ).size,
         )
 
     def multiplicity(self) -> float:
         return t.cast(
             float,
             getattr(
                 self.protobuf(),
-                t.cast(str, self.protobuf().WhichOneof('statistics')),
+                t.cast(str, self.protobuf().WhichOneof("statistics")),
             ).multiplicity,
         )
 
     def accept(self, visitor: st.StatisticsVisitor) -> None:
         dispatch: t.Callable[[], None] = {
-            'null': lambda: visitor.Null(
+            "null": lambda: visitor.Null(
                 self._protobuf.null.size, self._protobuf.null.multiplicity
             ),
-            'unit': lambda: visitor.Unit(
+            "unit": lambda: visitor.Unit(
                 self._protobuf.unit.size, self._protobuf.unit.multiplicity
             ),
-            'boolean': lambda: visitor.Boolean(
+            "boolean": lambda: visitor.Boolean(
                 size=self._protobuf.boolean.size,
                 multiplicity=self._protobuf.boolean.multiplicity,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.boolean.distribution.boolean.points  # noqa: E501
                 ],
                 names=[
@@ -67,32 +67,32 @@
                     for element in self._protobuf.boolean.distribution.boolean.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.boolean.distribution.boolean.points  # noqa: E501
                 ],
             ),
-            'integer': lambda: visitor.Integer(
+            "integer": lambda: visitor.Integer(
                 size=self._protobuf.integer.size,
                 multiplicity=self._protobuf.integer.multiplicity,
                 min_value=self._protobuf.integer.distribution.integer.min,
                 max_value=self._protobuf.integer.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.integer.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.integer.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'id': lambda: visitor.Id(
+            "id": lambda: visitor.Id(
                 self._protobuf.id.size, self._protobuf.id.multiplicity
             ),
-            'enum': lambda: visitor.Enum(
+            "enum": lambda: visitor.Enum(
                 size=self._protobuf.enum.size,
                 multiplicity=self._protobuf.enum.multiplicity,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.enum.distribution.enum.points  # noqa: E501
                 ],
                 names=[
@@ -100,87 +100,87 @@
                     for element in self._protobuf.enum.distribution.enum.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.enum.distribution.enum.points  # noqa: E501
                 ],
             ),
-            'float': lambda: visitor.Float(
+            "float": lambda: visitor.Float(
                 size=self._protobuf.float.size,
                 multiplicity=self._protobuf.float.multiplicity,
                 min_value=self._protobuf.float.distribution.double.min,
                 max_value=self._protobuf.float.distribution.double.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.float.distribution.double.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.float.distribution.double.points  # noqa: E501
                 ],
             ),
-            'text': lambda: visitor.Text(
+            "text": lambda: visitor.Text(
                 size=self._protobuf.text.size,
                 multiplicity=self._protobuf.text.multiplicity,
                 min_value=self._protobuf.text.distribution.integer.min,
                 max_value=self._protobuf.text.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.text.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.text.distribution.integer.points  # noqa: E501
                 ],
                 example=self._protobuf.text.example,
             ),
-            'bytes': lambda: visitor.Bytes(
+            "bytes": lambda: visitor.Bytes(
                 self._protobuf.bytes.size, self._protobuf.bytes.multiplicity
             ),
-            'struct': lambda: visitor.Struct(
+            "struct": lambda: visitor.Struct(
                 {
                     field.name: Statistics(field.statistics)
                     for field in self._protobuf.struct.fields
                 },
                 self._protobuf.struct.size,
                 name=self._protobuf.name,
                 multiplicity=self._protobuf.struct.multiplicity,
                 properties=self._protobuf.properties,
             ),
-            'union': lambda: visitor.Union(
+            "union": lambda: visitor.Union(
                 {
                     field.name: Statistics(field.statistics)
                     for field in self._protobuf.union.fields
                 },
                 size=self._protobuf.union.size,
                 name=self._protobuf.name,
                 multiplicity=self._protobuf.union.multiplicity,
                 properties=self._protobuf.properties,
             ),
-            'optional': lambda: visitor.Optional(
+            "optional": lambda: visitor.Optional(
                 Statistics(self._protobuf.optional.statistics),
                 size=self._protobuf.optional.size,
                 multiplicity=self._protobuf.optional.multiplicity,
             ),
-            'list': lambda: visitor.List(
+            "list": lambda: visitor.List(
                 statistics=Statistics(self._protobuf.list.statistics),
                 size=self._protobuf.list.size,
                 multiplicity=self._protobuf.list.multiplicity,
                 min_value=self._protobuf.list.distribution.integer.min,
                 max_value=self._protobuf.list.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.list.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.list.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'array': lambda: visitor.Array(
+            "array": lambda: visitor.Array(
                 statistics=Statistics(self._protobuf.array.statistics),
                 size=self._protobuf.array.size,
                 multiplicity=self._protobuf.array.multiplicity,
                 min_values=[
                     distribution.double.min
                     for distribution in self._protobuf.array.distributions
                 ],
@@ -196,77 +196,77 @@
                     for distribution in self._protobuf.array.distributions
                 ],
                 values=[
                     [element.value for element in distribution.double.points]
                     for distribution in self._protobuf.array.distributions
                 ],
             ),
-            'datetime': lambda: visitor.Datetime(
+            "datetime": lambda: visitor.Datetime(
                 size=self._protobuf.datetime.size,
                 multiplicity=self._protobuf.datetime.multiplicity,
                 min_value=self._protobuf.datetime.distribution.integer.min,
                 max_value=self._protobuf.datetime.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.datetime.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.datetime.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'date': lambda: visitor.Date(
+            "date": lambda: visitor.Date(
                 size=self._protobuf.date.size,
                 multiplicity=self._protobuf.date.multiplicity,
                 min_value=self._protobuf.date.distribution.integer.min,
                 max_value=self._protobuf.date.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.date.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.date.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'time': lambda: visitor.Time(
+            "time": lambda: visitor.Time(
                 size=self._protobuf.time.size,
                 multiplicity=self._protobuf.time.multiplicity,
                 min_value=self._protobuf.time.distribution.integer.min,
                 max_value=self._protobuf.time.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.time.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.time.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'duration': lambda: visitor.Duration(
+            "duration": lambda: visitor.Duration(
                 size=self._protobuf.duration.size,
                 multiplicity=self._protobuf.duration.multiplicity,
                 min_value=self._protobuf.duration.distribution.integer.min,
                 max_value=self._protobuf.duration.distribution.integer.max,
                 probabilities=[
                     element.probability
                     for element in self._protobuf.duration.distribution.integer.points  # noqa: E501
                 ],
                 values=[
                     element.value
                     for element in self._protobuf.duration.distribution.integer.points  # noqa: E501
                 ],
             ),
-            'constrained': lambda: visitor.Constrained(
+            "constrained": lambda: visitor.Constrained(
                 Statistics(self._protobuf.constrained.statistics),
                 self._protobuf.constrained.size,
                 self._protobuf.constrained.multiplicity,
             ),
             None: lambda: None,
-        }[self._protobuf.WhichOneof('statistics')]
+        }[self._protobuf.WhichOneof("statistics")]
         dispatch()
 
     def nodes_statistics(self, path: st.Path) -> t.List[st.Statistics]:
         """Returns the List of each statistics corresponding at the leaves of
         path"""
 
         class Select(st.StatisticsVisitor):
@@ -322,15 +322,15 @@
             def List(
                 self,
                 statistics: st.Statistics,
                 size: int,
                 multiplicity: float,
                 min_value: int,
                 max_value: int,
-                name: str = 'List',
+                name: str = "List",
                 probabilities: t.Optional[t.List[float]] = None,
                 values: t.Optional[t.List[int]] = None,
             ) -> None:
                 result = []
                 if len(path.sub_paths()) == 1:
                     result.extend(
                         statistics.nodes_statistics(path.sub_paths()[0])
@@ -340,15 +340,15 @@
             def Array(
                 self,
                 statistics: st.Statistics,
                 size: int,
                 multiplicity: float,
                 min_values: t.Optional[t.List[float]] = None,
                 max_values: t.Optional[t.List[float]] = None,
-                name: str = 'Array',
+                name: str = "Array",
                 probabilities: t.Optional[t.List[t.List[float]]] = None,
                 values: t.Optional[t.List[t.List[float]]] = None,
             ) -> None:
                 result = []
                 if len(path.sub_paths()) == 1:
                     result.extend(
                         statistics.nodes_statistics(path.sub_paths()[0])
@@ -448,15 +448,15 @@
             def Enum(
                 self,
                 size: int,
                 multiplicity: float,
                 probabilities: t.Optional[t.List[float]] = None,
                 names: t.Optional[t.List[str]] = None,
                 values: t.Optional[t.List[float]] = None,
-                name: str = 'Enum',
+                name: str = "Enum",
             ) -> None:
                 pass
 
             def Float(
                 self,
                 size: int,
                 multiplicity: float,
@@ -469,15 +469,15 @@
 
             def Text(
                 self,
                 size: int,
                 multiplicity: float,
                 min_value: int,
                 max_value: int,
-                example: str = '',
+                example: str = "",
                 probabilities: t.Optional[t.List[float]] = None,
                 values: t.Optional[t.List[int]] = None,
             ) -> None:
                 pass
 
         visitor = Select(statistics=self)
         self.accept(visitor)
@@ -525,28 +525,28 @@
             def List(
                 self,
                 statistics: st.Statistics,
                 size: int,
                 multiplicity: float,
                 min_value: int,
                 max_value: int,
-                name: str = 'List',
+                name: str = "List",
                 probabilities: t.Optional[t.List[float]] = None,
                 values: t.Optional[t.List[int]] = None,
             ) -> None:
                 self.result = {LIST_VALUES: statistics}
 
             def Array(
                 self,
                 statistics: st.Statistics,
                 size: int,
                 multiplicity: float,
                 min_values: t.Optional[t.List[float]] = None,
                 max_values: t.Optional[t.List[float]] = None,
-                name: str = 'Array',
+                name: str = "Array",
                 probabilities: t.Optional[t.List[t.List[float]]] = None,
                 values: t.Optional[t.List[t.List[float]]] = None,
             ) -> None:
                 self.result = {ARRAY_VALUES: statistics}
 
             def Bytes(self, size: int, multiplicity: float) -> None:
                 pass
@@ -628,15 +628,15 @@
             def Enum(
                 self,
                 size: int,
                 multiplicity: float,
                 probabilities: t.Optional[t.List[float]] = None,
                 names: t.Optional[t.List[str]] = None,
                 values: t.Optional[t.List[float]] = None,
-                name: str = 'Enum',
+                name: str = "Enum",
             ) -> None:
                 pass
 
             def Float(
                 self,
                 size: int,
                 multiplicity: float,
@@ -649,15 +649,15 @@
 
             def Text(
                 self,
                 size: int,
                 multiplicity: float,
                 min_value: int,
                 max_value: int,
-                example: str = '',
+                example: str = "",
                 probabilities: t.Optional[t.List[float]] = None,
                 values: t.Optional[t.List[int]] = None,
             ) -> None:
                 pass
 
             def Constrained(
                 self, statistics: st.Statistics, size: int, multiplicity: float
@@ -677,53 +677,53 @@
         return sp.Distribution
 
     def values(self) -> t.Union[t.List[float], t.List[int]]:
         return [
             element.value
             for element in getattr(
                 self.protobuf(),
-                t.cast(str, self.protobuf().WhichOneof('distribution')),
+                t.cast(str, self.protobuf().WhichOneof("distribution")),
             ).points
         ]
 
     def probabilities(self) -> t.List[float]:
         return [
             element.probability
             for element in getattr(
                 self.protobuf(),
-                t.cast(str, self.protobuf().WhichOneof('distribution')),
+                t.cast(str, self.protobuf().WhichOneof("distribution")),
             ).points
         ]
 
     def names(self) -> t.Union[t.List[bool], t.List[str]]:
-        distrib_type = t.cast(str, self.protobuf().WhichOneof('distribution'))
-        if distrib_type in ['integer', 'double']:
+        distrib_type = t.cast(str, self.protobuf().WhichOneof("distribution"))
+        if distrib_type in ["integer", "double"]:
             raise TypeError(
-                f'{distrib_type} distribution has no attribute names'
+                f"{distrib_type} distribution has no attribute names"
             )
         return [
             element.name
             for element in getattr(self.protobuf(), distrib_type).points
         ]
 
     def min_value(self) -> t.Union[int, float]:
-        distrib_type = t.cast(str, self.protobuf().WhichOneof('distribution'))
-        if distrib_type in ['enum', 'boolean']:
-            raise TypeError(f'{distrib_type} distribution has no min')
+        distrib_type = t.cast(str, self.protobuf().WhichOneof("distribution"))
+        if distrib_type in ["enum", "boolean"]:
+            raise TypeError(f"{distrib_type} distribution has no min")
         # mypy thinks the return should be Any
-        if distrib_type == 'float':
+        if distrib_type == "float":
             return t.cast(float, getattr(self.protobuf(), distrib_type).min)
         return t.cast(int, getattr(self.protobuf(), distrib_type).min)
 
     def max_value(self) -> t.Union[int, float]:
-        distrib_type = t.cast(str, self.protobuf().WhichOneof('distribution'))
-        if distrib_type in ['enum', 'boolean']:
-            raise TypeError(f'{distrib_type} distribution has no max')
+        distrib_type = t.cast(str, self.protobuf().WhichOneof("distribution"))
+        if distrib_type in ["enum", "boolean"]:
+            raise TypeError(f"{distrib_type} distribution has no max")
         # mypy thinks the return should be Any
-        if distrib_type == 'float':
+        if distrib_type == "float":
             return t.cast(float, getattr(self.protobuf(), distrib_type).max)
         return t.cast(int, getattr(self.protobuf(), distrib_type).max)
 
 
 # A few builders
 
 
@@ -842,53 +842,53 @@
     )
 
 
 # Statistics
 def Null(size: int, multiplicity: float) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Null',
+            name="Null",
             null=sp.Statistics.Null(size=size, multiplicity=multiplicity),
         )
     )
 
 
 def Unit(
     size: int,
     multiplicity: float,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Unit',
+            name="Unit",
             unit=sp.Statistics.Unit(size=size, multiplicity=multiplicity),
             properties=properties,
         )
     )
 
 
 def Id(size: int, multiplicity: float) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Id',
+            name="Id",
             id=sp.Statistics.Id(size=size, multiplicity=multiplicity),
         )
     )
 
 
 def Boolean(
     size: int,
     multiplicity: float,
     probabilities: t.Optional[t.List[float]] = None,
     names: t.Optional[t.List[bool]] = None,
     values: t.Optional[t.List[int]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Boolean',
+            name="Boolean",
             boolean=sp.Statistics.Boolean(
                 distribution=Boolean_Distribution(
                     probabilities=probabilities, names=names, values=values
                 ).protobuf(),
                 size=size,
                 multiplicity=multiplicity,
             ),
@@ -903,15 +903,15 @@
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Integer',
+            name="Integer",
             integer=sp.Statistics.Integer(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -925,15 +925,15 @@
 
 def Enum(
     size: int,
     multiplicity: float,
     probabilities: t.Optional[t.List[float]] = None,
     names: t.Optional[t.List[str]] = None,
     values: t.Optional[t.List[float]] = None,
-    name: str = 'Enum',
+    name: str = "Enum",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
             name=name,
             enum=sp.Statistics.Enum(
                 distribution=Enum_Distribution(
@@ -954,15 +954,15 @@
     max_value: t.Optional[float] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[float]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Float',
+            name="Float",
             float=sp.Statistics.Float(
                 distribution=Double_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -973,24 +973,24 @@
         )
     )
 
 
 def Text(
     size: int,
     multiplicity: float,
-    example: str = '',
+    example: str = "",
     min_value: t.Optional[int] = None,
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Text',
+            name="Text",
             text=sp.Statistics.Text(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -1002,30 +1002,30 @@
         )
     )
 
 
 def Bytes(size: int, multiplicity: float) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Bytes',
+            name="Bytes",
             bytes=sp.Statistics.Bytes(size=size, multiplicity=multiplicity),
         )
     )
 
 
 def Struct(
     fields: t.Mapping[str, st.Statistics],
     size: int,
     multiplicity: float,
     name: t.Optional[str] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Struct' if name is None else name,
+            name="Struct" if name is None else name,
             struct=sp.Statistics.Struct(
                 fields=[
                     sp.Statistics.Struct.Field(
                         name=name, statistics=statistics.protobuf()
                     )
                     for name, statistics in fields.items()
                 ],
@@ -1037,15 +1037,15 @@
     )
 
 
 def Union(
     fields: t.Mapping[str, st.Statistics],
     size: int,
     multiplicity: float,
-    name: str = 'Union',
+    name: str = "Union",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
             name=name,
             union=sp.Statistics.Union(
                 fields=[
@@ -1062,15 +1062,15 @@
     )
 
 
 def Optional(
     statistics: st.Statistics,
     size: int,
     multiplicity: float,
-    name: str = 'Optional',
+    name: str = "Optional",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
             name=name,
             optional=sp.Statistics.Optional(
                 statistics=statistics.protobuf(),
@@ -1082,15 +1082,15 @@
     )
 
 
 def List(
     statistics: st.Statistics,
     size: int,
     multiplicity: float,
-    name: str = 'List',
+    name: str = "List",
     min_value: t.Optional[int] = None,
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
@@ -1112,15 +1112,15 @@
     )
 
 
 def Array(
     statistics: st.Statistics,
     size: int,
     multiplicity: float,
-    name: str = 'Array',
+    name: str = "Array",
     min_values: t.Optional[t.List[float]] = None,
     max_values: t.Optional[t.List[float]] = None,
     probabilities: t.Optional[t.List[t.List[float]]] = None,
     values: t.Optional[t.List[t.List[float]]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     if min_values is None:
@@ -1171,15 +1171,15 @@
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Datetime',
+            name="Datetime",
             datetime=sp.Statistics.Datetime(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -1198,15 +1198,15 @@
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Date',
+            name="Date",
             date=sp.Statistics.Date(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -1225,15 +1225,15 @@
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Time',
+            name="Time",
             time=sp.Statistics.Time(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -1252,15 +1252,15 @@
     max_value: t.Optional[int] = None,
     probabilities: t.Optional[t.List[float]] = None,
     values: t.Optional[t.List[int]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Duration',
+            name="Duration",
             duration=sp.Statistics.Duration(
                 distribution=Integer_Distribution(
                     min_value=min_value,
                     max_value=max_value,
                     probabilities=probabilities,
                     values=values,
                 ).protobuf(),
@@ -1276,15 +1276,15 @@
     statistics: st.Statistics,
     size: int,
     multiplicity: float,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Statistics:
     return Statistics(
         sp.Statistics(
-            name='Constrained',
+            name="Constrained",
             constrained=sp.Statistics.Constrained(
                 statistics=statistics.protobuf(),
                 size=size,
                 multiplicity=multiplicity,
             ),
             properties=properties,
         )
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/status.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,21 +82,20 @@
         is processing the task).
         If the task does not exist, nothing is created"""
         # We copy the content of the current status
 
         def clear_update(
             status: st.Referring[ProtobufWithUUIDAndDatetime],
         ) -> t.Tuple[st.Referring[ProtobufWithUUIDAndDatetime], bool]:
-
             status = t.cast(Status, status)
             proto = status.protobuf()
             # We update its timestamp and properties
             proto.datetime = datetime.now().isoformat()
             stage = proto.task_stages.pop(task)
-            if stage.WhichOneof('stage') is None:
+            if stage.WhichOneof("stage") is None:
                 return status, False
 
             # we can create a new empty status only
             # if the current stage is static ie ready
             # (for example when removing cache) or
             # error (relaunch after timeout)
             else:
@@ -129,57 +128,57 @@
         """this is true if all tasks have status at least pending
         (i.e. pending, processing or ready) and at least one is pending"""
         has_one = False
         all_better = True
         task_stages = self.protobuf().task_stages
         if task_stages is not None:
             for task in task_stages:
-                has_one = has_one or task_stages[task].HasField('pending')
+                has_one = has_one or task_stages[task].HasField("pending")
                 all_better = all_better and not (
-                    task_stages[task].HasField('error')
+                    task_stages[task].HasField("error")
                 )
         return has_one and all_better
 
     def processing(
         self,
     ) -> bool:
         """this is true if all tasks have status at least processing
         (i.e. processing or ready) and at least one is processing"""
         has_one = False
         all_better = True
         task_stages = self.protobuf().task_stages
         if task_stages is not None:
             for task in task_stages:
-                has_one = has_one or task_stages[task].HasField('processing')
+                has_one = has_one or task_stages[task].HasField("processing")
                 all_better = all_better and not (
-                    task_stages[task].HasField('error')
-                    or task_stages[task].HasField('pending')
+                    task_stages[task].HasField("error")
+                    or task_stages[task].HasField("pending")
                 )
         return has_one and all_better
 
     def ready(
         self,
     ) -> bool:  # TODO this should be true if all tasks have status ready
         """this is true if all tasks have status ready"""
         all_ready = True
         task_stages = self.protobuf().task_stages
         if task_stages is not None:
             for task in task_stages:
-                all_ready = all_ready and task_stages[task].HasField('ready')
+                all_ready = all_ready and task_stages[task].HasField("ready")
         return all_ready
 
     def error(
         self,
     ) -> bool:  # TODO this should be true if any task have status error
         """this is true if any tasks have status error"""
         has_error = False
         task_stages = self.protobuf().task_stages
         if task_stages is not None:
             for task in task_stages:
-                has_error = has_error or task_stages[task].HasField('error')
+                has_error = has_error or task_stages[task].HasField("error")
         return has_error
 
     def dataset(self) -> Dataset:
         dataspec = self.dataspec()
         assert isinstance(dataspec, Dataset)
         return dataspec
 
@@ -207,27 +206,27 @@
     for error and ready that can be reset to None.
     When the stage is None, it means that the task is not present"""
 
     if existing_stage is None:
         return True  # all transitions allowed if no task exists
 
     allowed_transitions = {
-        'pending': ['processing', 'ready', 'error'],
-        'processing': ['ready', 'error'],
-        'ready': ['error', None],
-        'error': [None, 'ready'],
-        None: ['pending', 'processing', 'ready', 'error']
+        "pending": ["processing", "ready", "error"],
+        "processing": ["ready", "error"],
+        "ready": ["error", None],
+        "error": [None, "ready"],
+        None: ["pending", "processing", "ready", "error"],
         # the transition error to ready can occur
         # if a long task is processed, meanwhile another worker sets an error
         # because it timeouts after waiting, then the first worker finishes
     }
     if new_stage is not None:
         if (
-            new_stage.WhichOneof('stage')  # type:ignore
-            in allowed_transitions[existing_stage.WhichOneof('stage')]
+            new_stage.WhichOneof("stage")  # type:ignore
+            in allowed_transitions[existing_stage.WhichOneof("stage")]
         ):
             return True
         else:
             logger.warning(
                 f"Trying to update a status with stage "
                 f"{new_stage.WhichOneof('stage')} for the task {task_name} "
                 f"while the existing stage "
@@ -235,15 +234,15 @@
                 f"therefore the update will be ignored"
             )
         return False
 
     else:
         if (
             new_stage  # type: ignore
-            in allowed_transitions[existing_stage.WhichOneof('stage')]
+            in allowed_transitions[existing_stage.WhichOneof("stage")]
         ):
             return True
 
         else:
             logger.warning(
                 f"Trying to update a status with stage "
                 f"{new_stage} for the task {task_name} "
@@ -324,35 +323,35 @@
 
 
 class Stage(Base[sp.Status.Stage]):
     """A simple wrapper type to simplify protobuf usage"""
 
     def accept(self, visitor: st.StageVisitor) -> None:
         dispatch: Callable[[], None] = {
-            'pending': visitor.pending,
-            'processing': visitor.processing,
-            'ready': visitor.ready,
-            'error': visitor.error,
-        }[cast(str, self.protobuf().WhichOneof('stage'))]
+            "pending": visitor.pending,
+            "processing": visitor.processing,
+            "ready": visitor.ready,
+            "error": visitor.error,
+        }[cast(str, self.protobuf().WhichOneof("stage"))]
         dispatch()
 
     def stage(self) -> str:
-        return cast(str, self.protobuf().WhichOneof('stage'))
+        return cast(str, self.protobuf().WhichOneof("stage"))
 
     def ready(self) -> bool:
-        return self.stage() == 'ready'
+        return self.stage() == "ready"
 
     def pending(self) -> bool:
-        return self.stage() == 'pending'
+        return self.stage() == "pending"
 
     def processing(self) -> bool:
-        return self.stage() == 'processing'
+        return self.stage() == "processing"
 
     def error(self) -> bool:
-        return self.stage() == 'error'
+        return self.stage() == "error"
 
 
 # Builders for stages
 def pending_stage(properties: Optional[Mapping[str, str]] = None) -> Stage:
     return Stage(
         sp.Status.Stage(
             pending=sp.Status.Stage.Pending(), properties=properties
@@ -468,16 +467,16 @@
         # Protobuf implementation of the merge
         # does not work as expected on maps...
     if task_stages is not None:
         for task in task_stages:
             stage = task_stages[task].protobuf()
             if (
                 task in proto.task_stages
-                and proto.task_stages[task].WhichOneof('stage')
-                == task_stages[task].protobuf().WhichOneof('stage')
+                and proto.task_stages[task].WhichOneof("stage")
+                == task_stages[task].protobuf().WhichOneof("stage")
                 and not stage.properties == proto.task_stages[task].properties
             ):
                 proto.task_stages[task].properties.update(stage.properties)
             else:
                 if transition_allowed(
                     existing_stage=proto.task_stages.get(task, None),
                     new_stage=stage,
@@ -492,15 +491,15 @@
 
 def status_error_policy(stage: st.Stage) -> bool:
     """This methods returns whether a given error message
     should be reset to None or not. Currently, the quick
     shortcut is to check whether the error message starts
     with a TimeoutError, in this case, we want to retry"""
     assert stage.error()
-    return stage.properties().get('relaunch', 'False') == str(True)
+    return stage.properties().get("relaunch", "False") == str(True)
 
 
 def error_aggregation(errors: t.List[Exception]) -> Exception:
     """Takes as input a list of exceptions, the first error
     that is not a DataSpecErrorStatus or that has not a relaunch.
     If they are all DataSpecErrorStatuses with relaunch, returns
     the first"""
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/local.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from sarus_data_spec.protobuf.typing import (
     ProtobufWithUUID,
     ProtobufWithUUIDAndDatetime,
 )
 from sarus_data_spec.storage.utils import sort_dataspecs
 from sarus_data_spec.typing import DataSpec, Referrable, Referring
 
-SEP: Final[str] = ','
+SEP: Final[str] = ","
 
 
 def referrable_collection_string(
     values: Collection[Referrable[ProtobufWithUUID]],
 ) -> str:
     return SEP.join(sorted(value.uuid() for value in values))
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,15 @@
     def create_referring_with_datetime(
         self,
         value: Referring[ProtobufWithUUIDAndDatetime],
         update: Callable[
             [Referring[ProtobufWithUUIDAndDatetime]],
             Tuple[Referring[ProtobufWithUUIDAndDatetime], bool],
         ],
-    ) -> Tuple[Referring[ProtobufWithUUIDAndDatetime], bool]:
-        ...
+    ) -> Tuple[Referring[ProtobufWithUUIDAndDatetime], bool]: ...
 
     def type_name(
         self, type_name: str
     ) -> Collection[Referrable[ProtobufWithUUID]]:
         """List all values from a given type_name."""
         ...
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/storage/utils.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/storage/utils.py`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/transform.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,22 @@
         return self._protobuf.name
 
     def doc(self) -> str:
         return self._protobuf.doc
 
     def is_composed(self) -> bool:
         """Is the transform composed."""
-        return self._protobuf.spec.HasField('composed')
+        return self._protobuf.spec.HasField("composed")
 
     def is_variable(self) -> bool:
         """Is the transform a variable."""
-        return self._protobuf.spec.HasField('variable')
+        return self._protobuf.spec.HasField("variable")
 
     def spec(self) -> str:
-        return t.cast(str, self._protobuf.spec.WhichOneof('spec'))
+        return t.cast(str, self._protobuf.spec.WhichOneof("spec"))
 
     def is_external(self) -> bool:
         """Is the transform an external operation."""
         return self._protobuf.spec.HasField("external")
 
     def infer_output_type(
         self,
@@ -77,15 +77,15 @@
             ) -> None:
                 self.visited.add(transform)
                 if transform not in self.visited:
                     transform.accept(self)
                 for arg in arguments:
                     if arg not in self.visited:
                         arg.accept(self)
-                for name, arg in named_arguments.items():
+                for arg in named_arguments.values():
                     if arg not in self.visited:
                         arg.accept(self)
 
             def other(self, visited: st.Transform) -> None:
                 raise ValueError(
                     "A composed transform can only have Variables "
                     "or Composed ancestors."
@@ -360,20 +360,20 @@
                 raise NotImplementedError
 
             def all(self, visited: st.Transform) -> None:
                 pass
 
         visitor = Dot()
         self.accept(visitor)
-        result = 'digraph {'
+        result = "digraph {"
         for uuid, label in visitor.nodes.items():
             result += f'\n"{uuid}" [label="{label} ({uuid[:2]})"];'
         for u1, u2 in visitor.edges:
             result += f'\n"{u1}" -> "{u2}";'
-        result += '}'
+        result += "}"
         return result
 
     def transform_to_apply(self) -> st.Transform:
         """Return the transform of a composed transform."""
         assert self.is_composed()
         uuid = self.protobuf().spec.composed.transform
         return t.cast(st.Transform, self.storage().referrable(uuid))
@@ -405,26 +405,26 @@
         return self.manager().composed_callable(self)
 
 
 # Builders
 def identity() -> Transform:
     return Transform(
         sp.Transform(
-            name='Identity',
+            name="Identity",
             spec=sp.Transform.Spec(identity=sp.Transform.Identity()),
             inversible=True,
             schema_preserving=True,
         )
     )
 
 
 def variable(name: str, position: int = 0) -> Transform:
     return Transform(
         sp.Transform(
-            name='Variable',
+            name="Variable",
             spec=sp.Transform.Spec(
                 variable=sp.Transform.Variable(
                     name=name,
                     position=position,
                 )
             ),
             inversible=True,
@@ -439,15 +439,15 @@
     **named_arguments: st.Transform,
 ) -> st.Transform:
     if transform.is_composed():
         # We want to compose simple transforms only
         return transform.compose(*arguments, **named_arguments)
     return Transform(
         sp.Transform(
-            name='Composed',
+            name="Composed",
             spec=sp.Transform.Spec(
                 composed=sp.Transform.Composed(
                     transform=transform.uuid(),
                     arguments=(a.uuid() for a in arguments),
                     named_arguments={
                         n: a.uuid() for n, a in named_arguments.items()
                     },
@@ -505,32 +505,40 @@
         library = str(spec.external.op_identifier.WhichOneof("op"))
         op_name = getattr(spec.external.op_identifier, library).name
         return f"{library}.{op_name}"
 
 
 def external(
     id: str,
-    py_args: t.Dict[int, t.Any] = {},
-    py_kwargs: t.Dict[str, t.Any] = {},
-    ds_args_pos: t.List[int] = [],
-    ds_types: t.Dict[t.Union[int, str], str] = {},
+    py_args: t.Optional[t.Dict[int, t.Any]] = None,
+    py_kwargs: t.Optional[t.Dict[str, t.Any]] = None,
+    ds_args_pos: t.Optional[t.List[int]] = None,
+    ds_types: t.Optional[t.Dict[t.Union[int, str], str]] = None,
 ) -> Transform:
     """Create an external library transform.
 
     Args:
         id (str): id in the form library.name (e.g. sklearn.PD_MEAN)
         py_args (Dict[int, Any]):
             the Python objects passed as arguments to the transform.
         py_kwargs (Dict[int, Any]):
             the Python objects passed as keyword arguments to the transform.
         ds_args_pos (List[int]):
             the positions of Dataspecs passed in args.
         ds_types (Dict[int | str, str]):
             the types of the Dataspecs passed as arguments.
     """
+    if py_args is None:
+        py_args = {}
+    if py_kwargs is None:
+        py_kwargs = {}
+    if ds_args_pos is None:
+        ds_args_pos = []
+    if ds_types is None:
+        ds_types = {}
     external = sp.Transform.External(
         arguments=SarusJSONEncoder.encode_bytes([]),
         named_arguments=SarusJSONEncoder.encode_bytes(
             {
                 "py_args": py_args,
                 "py_kwargs": py_kwargs,
                 "ds_args_pos": ds_args_pos,
@@ -549,63 +557,63 @@
         )
     )
 
 
 def project(projection: st.Type) -> Transform:
     return Transform(
         sp.Transform(
-            name='Project',
+            name="Project",
             spec=sp.Transform.Spec(
                 project=sp.Transform.Project(projection=projection.protobuf())
             ),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
 def filter(filter: st.Type) -> Transform:
     return Transform(
         sp.Transform(
-            name='Filter',
+            name="Filter",
             spec=sp.Transform.Spec(
                 filter=sp.Transform.Filter(filter=filter.protobuf())
             ),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
 def shuffle() -> Transform:
     return Transform(
         sp.Transform(
-            name='Shuffle',
+            name="Shuffle",
             spec=sp.Transform.Spec(shuffle=sp.Transform.Shuffle()),
             inversible=False,
             schema_preserving=True,
         )
     )
 
 
 def join(on: st.Type) -> Transform:
     return Transform(
         sp.Transform(
-            name='Join',
+            name="Join",
             spec=sp.Transform.Spec(join=sp.Transform.Join(on=on.protobuf())),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
 def cast(type: st.Type) -> Transform:
     return Transform(
         sp.Transform(
-            name='Cast',
+            name="Cast",
             spec=sp.Transform.Spec(
                 cast=sp.Transform.Cast(type=type.protobuf())
             ),
             inversible=False,
             schema_preserving=False,
         )
     )
@@ -613,15 +621,15 @@
 
 def sample(fraction_size: t.Union[float, int], seed: st.Scalar) -> Transform:
     """Transform to sample from a dataspec
     - the dataset that needs to be protected as the first arg
     - a kwarg seed"""
     return Transform(
         sp.Transform(
-            name='Sample',
+            name="Sample",
             spec=sp.Transform.Spec(
                 sample=sp.Transform.Sample(
                     size=fraction_size,
                     seed=seed.protobuf(),
                 )
                 if isinstance(fraction_size, int)
                 else sp.Transform.Sample(
@@ -638,37 +646,37 @@
     """Transform to create a dataspec from
     a protected one with a new schema. It should
     be called on:
     - the dataset that needs to be protected as the first arg
     - a kwarg user_type: scalar output of automatic_user_setttings"""
     return Transform(
         sp.Transform(
-            name='User Settings',
+            name="User Settings",
             spec=sp.Transform.Spec(user_settings=sp.Transform.UserSettings()),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
 def automatic_user_settings(max_categories: int = 200) -> Transform:
     """Transform to be called on a protected dataset
     we want to change the schema. It creates a scalar
     whose value explicits the new type of the schema"""
     return Transform(
         sp.Transform(
-            name='automatic_user_settings',
+            name="automatic_user_settings",
             spec=sp.Transform.Spec(
                 automatic_user_settings=sp.Transform.AutomaticUserSettings(
                     max_categories=max_categories
                 )
             ),
             inversible=False,
             schema_preserving=False,
-            properties={'creation_time': str(datetime.datetime.now())},
+            properties={"creation_time": str(datetime.datetime.now())},
         )
     )
 
 
 def synthetic() -> Transform:
     """Synthetic transform. This transform should be
     called on a dataset with the additional following kwargs:
@@ -682,88 +690,90 @@
             ),
             inversible=False,
             schema_preserving=True,
         )
     )
 
 
-def protect() -> Transform:
-    """Transform used for protection should be called on:
-    - the dataset that needs to be protected as the first arg
-    - a kwarg protected_paths: scalar specifying the paths
-     to the entities to protect
+def privacy_unit_tracking() -> Transform:
+    """Transform used for PUT should be called on:
+    - the dataset that needs to be PUT as the first arg
+    - a kwarg privacy_unit_tracking_paths: scalar specifying the paths
+     to the entities to PUT
     - a kwarg public_paths: scalar specifying the paths to
     the public tables"""
     return Transform(
         sp.Transform(
-            name='Protect',
-            spec=sp.Transform.Spec(protect_dataset=sp.Transform.Protect()),
+            name="Protect",
+            spec=sp.Transform.Spec(
+                privacy_unit_tracking=sp.Transform.PrivacyUnitTracking()
+            ),
             inversible=True,
             schema_preserving=False,
         )
     )
 
 
 def transcode(model_properties: t.Dict[str, t.Any]) -> st.Transform:
     return Transform(
         sp.Transform(
-            name='Transcode',
+            name="Transcode",
             spec=sp.Transform.Spec(transcode=sp.Transform.Transcode()),
             inversible=True,
             schema_preserving=False,
             properties={MODEL_PROPERTIES: json.dumps(model_properties)},
         )
     )
 
 
 def inverse_transcode() -> st.Transform:
     return Transform(
         sp.Transform(
-            name='Inverse Transcoding for synthetic data',
+            name="Inverse Transcoding for synthetic data",
             spec=sp.Transform.Spec(
                 inverse_transcode=sp.Transform.InverseTranscode()
             ),
             inversible=True,
             schema_preserving=False,
         )
     )
 
 
-def automatic_protected_paths() -> st.Transform:
+def automatic_privacy_unit_tracking_paths() -> st.Transform:
     """Transform that should be called on the dataset
     that needs to be protected, it creates a scalar whose
     value will explicit the paths to protect"""
     return Transform(
         sp.Transform(
-            name='automatic_protected_paths',
+            name="automatic_privacy_unit_tracking_paths",
             spec=sp.Transform.Spec(
-                protected_paths=sp.Transform.ProtectedPaths()
+                privacy_unit_tracking_paths=sp.Transform.PrivacyUnitTrackingPaths()  # noqa: E501
             ),
-            properties={'creation_time': str(datetime.datetime.now())},
+            properties={"creation_time": str(datetime.datetime.now())},
         )
     )
 
 
 def automatic_public_paths() -> st.Transform:
     """Transform that should be called on the dataset
     that needs to be protected, it creates a scalar whose
     value will explicit the paths to public entities"""
     return Transform(
         sp.Transform(
-            name='automatic_public_paths',
+            name="automatic_public_paths",
             spec=sp.Transform.Spec(public_paths=sp.Transform.PublicPaths()),
-            properties={'creation_time': str(datetime.datetime.now())},
+            properties={"creation_time": str(datetime.datetime.now())},
         )
     )
 
 
 def get_item(path: st.Path) -> st.Transform:
     return Transform(
         sp.Transform(
-            name='get_item',
+            name="get_item",
             spec=sp.Transform.Spec(
                 get_item=sp.Transform.GetItem(path=path.protobuf())
             ),
             inversible=False,
             schema_preserving=False,
         )
     )
@@ -772,30 +782,30 @@
 def assign_budget() -> st.Transform:
     """Transform to assign a given privacy budget to a dataset.
     It is used to specify the budget to compute the attributes
     size, bounds, marginals"""
 
     return Transform(
         sp.Transform(
-            name='budget_assignment',
+            name="budget_assignment",
             spec=sp.Transform.Spec(assign_budget=sp.Transform.AssignBudget()),
         )
     )
 
 
 def automatic_budget() -> st.Transform:
     """Transform to create a scalar specifying a budget
     automatically from the dataset it is called on.
     The rule to fix the budget is set in the corresponding
     op.
     """
 
     return Transform(
         sp.Transform(
-            name='automatic_budget',
+            name="automatic_budget",
             spec=sp.Transform.Spec(
                 automatic_budget=sp.Transform.AutomaticBudget()
             ),
         )
     )
 
 
@@ -803,15 +813,15 @@
     """Transform to create a scalar specifying an
      epsilon,delta budget for the DP attributes of a
     dataset. It is called on a scalar specifying a
     global budget for attributes+sd."""
 
     return Transform(
         sp.Transform(
-            name='attributes_budget',
+            name="attributes_budget",
             spec=sp.Transform.Spec(
                 attribute_budget=sp.Transform.AttributesBudget()
             ),
         )
     )
 
 
@@ -819,51 +829,51 @@
     """Transform to create a scalar specifying an
      epsilon,delta budget for a synthetic dataset.
     It should be called on another scalar that specifies
     a global budget (SD+DP attributes)"""
 
     return Transform(
         sp.Transform(
-            name='sd_budget',
+            name="sd_budget",
             spec=sp.Transform.Spec(sd_budget=sp.Transform.SDBudget()),
         )
     )
 
 
 def derive_seed(random_int: int) -> st.Transform:
     """Transform to derive a seed from a master seed"""
     return Transform(
         sp.Transform(
-            name='derive_seed',
+            name="derive_seed",
             spec=sp.Transform.Spec(
                 derive_seed=sp.Transform.DeriveSeed(random_integer=random_int)
             ),
         )
     )
 
 
 def group_by_pe() -> st.Transform:
     """Transform that allows to group fields
     by protected entity value. This implies that
     the dataset on which the transform is
-    applied should be PEP"""
+    applied should be PUP"""
     return Transform(
         sp.Transform(
-            name='group_by',
+            name="group_by",
             spec=sp.Transform.Spec(group_by_pe=sp.Transform.GroupByPE()),
         )
     )
 
 
 def differentiated_sample(  # type: ignore[no-untyped-def]
     fraction_size: t.Union[float, int], seed=st.Scalar
 ) -> Transform:
     return Transform(
         sp.Transform(
-            name='DifferentiatedSample',
+            name="DifferentiatedSample",
             spec=sp.Transform.Spec(
                 differentiated_sample=sp.Transform.DifferentiatedSample(
                     size=fraction_size, seed=seed.protobuf()
                 )
                 if isinstance(fraction_size, int)
                 else sp.Transform.DifferentiatedSample(
                     fraction=fraction_size, seed=seed.protobuf()
@@ -874,15 +884,15 @@
 
 
 def to_small_data(
     size: int, random_sampling: bool, seed: st.Scalar
 ) -> Transform:
     return Transform(
         sp.Transform(
-            name='ToSmallData',
+            name="ToSmallData",
             spec=sp.Transform.Spec(
                 to_small_data=sp.Transform.ToSmallData(
                     size=size,
                     random_sampling=random_sampling,
                     seed=seed.protobuf(),
                 )
             ),
@@ -893,24 +903,24 @@
 
 
 def handle_big_data_from_name(code_name: str) -> bool:
     """
     Check if the transform with name codename can handle bigdata in SQL.
     """
     if code_name in [
-        'assign_budget',
-        'differentiated_sample',
-        'dp_select_sql',
-        'select_sql',
-        'extract',
-        'sample',
-        'protect_dataset',
-        'user_settings',
-        'automatic_user_settings',
-        'ToSmallData',
+        "assign_budget",
+        "differentiated_sample",
+        "dp_select_sql",
+        "select_sql",
+        "extract",
+        "sample",
+        "privacy_unit_tracking",
+        "user_settings",
+        "automatic_user_settings",
+        "ToSmallData",
     ]:
         return True
     return False
 
 
 def handle_big_data(transform: st.Transform) -> bool:
     """
@@ -931,17 +941,15 @@
 
     if manager.is_big_data(dataspec) and (
         code_name is None or not handle_big_data_from_name(code_name)
     ):
         status = manager.status(dataspec, task_name=BIG_DATA_TASK)
         assert status
         big_data_threshold = int(
-            status.task(BIG_DATA_TASK).properties()[  # type:ignore
-                BIG_DATA_THRESHOLD
-            ]
+            status.task(BIG_DATA_TASK).properties()[BIG_DATA_THRESHOLD]  # type:ignore
         )
         seed = global_context().generate_seed()
         small_dataspec = t.cast(
             st.DataSpec,
             to_small_data(
                 size=big_data_threshold,
                 random_sampling=random_sampling,
@@ -998,15 +1006,15 @@
                 ),
             ),
             sql_dialect=sql_dialect,
         )
 
     return Transform(
         sp.Transform(
-            name='select_sql',
+            name="select_sql",
             spec=sp.Transform.Spec(select_sql=select_sql),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
@@ -1054,15 +1062,15 @@
                 ),
             ),
             sql_dialect=sql_dialect,
         )
 
     return Transform(
         sp.Transform(
-            name='dp_select_sql',
+            name="dp_select_sql",
             spec=sp.Transform.Spec(dp_select_sql=proto),
             inversible=False,
             schema_preserving=False,
         )
     )
 
 
@@ -1073,75 +1081,74 @@
     extract some rows from according to the size parameter and a kwargs
     random_seed, a scalar that is a seed. For now, seed and size are
     ignored and iterating on the extract transformed dataset will be as
     iterating over the parent dataset.
     """
     return Transform(
         sp.Transform(
-            name='extract',
+            name="extract",
             spec=sp.Transform.Spec(extract=sp.Transform.Extract(size=size)),
             inversible=False,
             schema_preserving=True,
         )
     )
 
 
 def relationship_spec() -> st.Transform:
     """Transform that allows to redefine the primary and foreign keys
     of a dataset."""
     return Transform(
         sp.Transform(
-            name='relationship_spec',
+            name="relationship_spec",
             spec=sp.Transform.Spec(
                 relationship_spec=sp.Transform.RelationshipSpec()
             ),
         )
     )
 
 
 def validated_user_type() -> st.Transform:
     """Transform that allows to set whether the user has validated
     the schema or if some types have to be changed"""
     return Transform(
         sp.Transform(
-            name='validated_user_type',
+            name="validated_user_type",
             spec=sp.Transform.Spec(
                 validated_user_type=sp.Transform.ValidatedUserType()
             ),
         )
     )
 
 
 def error_estimation() -> st.Transform:
     """Transform that computes 95th percentile from true value"""
     return Transform(
         sp.Transform(
-            name='error_estimation',
+            name="error_estimation",
             spec=sp.Transform.Spec(
                 error_estimation=sp.Transform.ErrorEstimation()
             ),
         )
     )
 
 
 def fit_model(
     batch_size: int,
     epochs: int = 1,
     text_field: t.Optional[str] = None,
     question_field: t.Optional[str] = None,
     answer_field: t.Optional[str] = None,
 ) -> st.Transform:
-
     is_text_field = text_field is not None
     is_chat = question_field is not None and answer_field is not None
 
     if is_chat and is_text_field:
         raise ValueError(
-            'Wrong arguments: you must either fill text_field or '
-            'both answer_field and question_field'
+            "Wrong arguments: you must either fill text_field or "
+            "both answer_field and question_field"
         )
     if is_chat:
         question_field = t.cast(str, question_field)
         answer_field = t.cast(str, answer_field)
         return Transform(
             sp.Transform(
                 name="fit_model",
@@ -1171,36 +1178,34 @@
                         text_kind=sp.Transform.TextKind(text_field=text_field),
                     ),
                 ),
             )
         )
 
     raise ValueError(
-        'Wrong arguments: you must either fill text_field '
-        'or both answer_field and question_field'
+        "Wrong arguments: you must either fill text_field "
+        "or both answer_field and question_field"
     )
 
 
 def fit_model_dp(
     batch_size: int,
     epochs: int = 1,
     l2_norm_clip: float = 1e-2,
     text_field: t.Optional[str] = None,
     question_field: t.Optional[str] = None,
     answer_field: t.Optional[str] = None,
 ) -> st.Transform:
-
     is_text_field = text_field is not None
     is_chat = question_field is not None and answer_field is not None
 
     if is_chat and is_text_field:
-
         raise ValueError(
-            'Wrong arguments: you must either fill text_field'
-            ' or both answer_field and question_field'
+            "Wrong arguments: you must either fill text_field"
+            " or both answer_field and question_field"
         )
     if is_chat:
         question_field = t.cast(str, question_field)
         answer_field = t.cast(str, answer_field)
         return Transform(
             sp.Transform(
                 name="fit_model_dp",
@@ -1231,16 +1236,16 @@
                         epochs=epochs,
                         text_kind=sp.Transform.TextKind(text_field=text_field),
                     ),
                 ),
             )
         )
     raise ValueError(
-        'Wrong arguments: you must either fill text_field '
-        'or both answer_field and question_field'
+        "Wrong arguments: you must either fill text_field "
+        "or both answer_field and question_field"
     )
 
 
 def generate_from_model(
     max_new_tokens: int = 20, temperature: float = 1.0
 ) -> st.Transform:
     return Transform(
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/type.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,43 +10,43 @@
 
 from sarus_data_spec.base import Base
 from sarus_data_spec.constants import (
     ARRAY_VALUES,
     DATA,
     LIST_VALUES,
     OPTIONAL_VALUE,
+    PU_COLUMN,
     PUBLIC,
     TEXT_CHARSET,
     TEXT_MAX_LENGTH,
-    USER_COLUMN,
     WEIGHTS,
 )
 from sarus_data_spec.path import Path
 from sarus_data_spec.path import path as path_builder
 from sarus_data_spec.predicate import Predicate
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 try:
     import tensorflow as tf
 except ModuleNotFoundError:
     pass
 
-VisitedType = t.TypeVar('VisitedType')
+VisitedType = t.TypeVar("VisitedType")
 
 DURATION_UNITS_TO_RANGE = {
-    'us': (
+    "us": (
         int(np.iinfo(np.int64).min / 1e3),
         int(np.iinfo(np.int64).max / 1e3),
     ),
-    'ms': (
+    "ms": (
         int(np.iinfo(np.int64).min / 1e6),
         int(np.iinfo(np.int64).max / 1e6),
     ),
-    's': (
+    "s": (
         int(np.iinfo(np.int64).min / 1e9),
         int(np.iinfo(np.int64).max / 1e9),
     ),
 }
 
 BASE_ID_TO_PROTO = {
     st.IdBase.INT64.value: sp.Type.Id.INT64,
@@ -96,34 +96,34 @@
         """Return the type of the underlying protobuf."""
         return sp.Type
 
     def name(self) -> str:
         """Returns the name of the underlying protobuf."""
         return self.protobuf().name
 
-    def has_protection(self) -> bool:
+    def has_privacy_unit_tracking(self) -> bool:
         """Return True if the Type has protection information."""
         protection_fields = {
             PUBLIC,
-            USER_COLUMN,
+            PU_COLUMN,
             WEIGHTS,
         }
 
         if self.has_admin_columns():
             type = self.protobuf()
             field_names = {element.name for element in type.struct.fields}
             # there may be additional administrative columns
             return protection_fields.issubset(field_names)
         else:
             return False
 
     def has_admin_columns(self) -> bool:
         """Return True if the Type has administrative columns."""
         type = self.protobuf()
-        if type.HasField('struct'):
+        if type.HasField("struct"):
             field_names = {element.name for element in type.struct.fields}
             # there may be additional administrative columns
             return DATA in field_names
         else:
             return False
 
     def data_type(self) -> Type:
@@ -144,344 +144,344 @@
             return Type(data_type)
         else:
             return self
 
     # A Visitor acceptor
     def accept(self, visitor: st.TypeVisitor) -> None:
         dispatch: t.Callable[[], None] = {
-            'null': lambda: visitor.Null(properties=self._protobuf.properties),
-            'unit': lambda: visitor.Unit(properties=self._protobuf.properties),
-            'boolean': lambda: visitor.Boolean(
+            "null": lambda: visitor.Null(properties=self._protobuf.properties),
+            "unit": lambda: visitor.Unit(properties=self._protobuf.properties),
+            "boolean": lambda: visitor.Boolean(
                 properties=self._protobuf.properties
             ),
-            'integer': lambda: visitor.Integer(
+            "integer": lambda: visitor.Integer(
                 min=self._protobuf.integer.min,
                 max=self._protobuf.integer.max,
                 base=st.IntegerBase(self._protobuf.integer.base),
                 possible_values=self._protobuf.integer.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'id': lambda: visitor.Id(
+            "id": lambda: visitor.Id(
                 base=st.IdBase(self._protobuf.id.base),
                 unique=self._protobuf.id.unique,
                 reference=Path(self._protobuf.id.reference)
                 if self._protobuf.id.reference != sp.Path()
                 else None,
                 properties=self._protobuf.properties,
             ),
-            'enum': lambda: visitor.Enum(
+            "enum": lambda: visitor.Enum(
                 self._protobuf.name,
                 [
                     (name_value.name, name_value.value)
                     for name_value in self._protobuf.enum.name_values
                 ],
                 self._protobuf.enum.ordered,
                 properties=self._protobuf.properties,
             ),
-            'float': lambda: visitor.Float(
+            "float": lambda: visitor.Float(
                 min=self._protobuf.float.min,
                 max=self._protobuf.float.max,
                 base=st.FloatBase(self._protobuf.float.base),
                 possible_values=self._protobuf.float.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'text': lambda: visitor.Text(
+            "text": lambda: visitor.Text(
                 self._protobuf.text.encoding,
                 possible_values=self._protobuf.text.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'bytes': lambda: visitor.Bytes(
+            "bytes": lambda: visitor.Bytes(
                 properties=self._protobuf.properties
             ),
-            'struct': lambda: visitor.Struct(
+            "struct": lambda: visitor.Struct(
                 {
                     field.name: Type(field.type)
                     for field in self._protobuf.struct.fields
                 },
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'union': lambda: visitor.Union(
+            "union": lambda: visitor.Union(
                 {
                     field.name: Type(field.type)
                     for field in self._protobuf.union.fields
                 },
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'optional': lambda: visitor.Optional(
+            "optional": lambda: visitor.Optional(
                 Type(self._protobuf.optional.type),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'list': lambda: visitor.List(
+            "list": lambda: visitor.List(
                 Type(self._protobuf.list.type),
                 max_size=self._protobuf.list.max_size,
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'array': lambda: visitor.Array(
+            "array": lambda: visitor.Array(
                 Type(self._protobuf.array.type),
                 tuple(self._protobuf.array.shape),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'datetime': lambda: visitor.Datetime(
+            "datetime": lambda: visitor.Datetime(
                 self._protobuf.datetime.format,
                 self._protobuf.datetime.min,
                 self._protobuf.datetime.max,
                 st.DatetimeBase(self._protobuf.datetime.base),
                 possible_values=self._protobuf.datetime.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'date': lambda: visitor.Date(
+            "date": lambda: visitor.Date(
                 self._protobuf.date.format,
                 self._protobuf.date.min,
                 self._protobuf.date.max,
                 st.DateBase(self._protobuf.date.base),
                 possible_values=self._protobuf.date.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'time': lambda: visitor.Time(
+            "time": lambda: visitor.Time(
                 self._protobuf.time.format,
                 self._protobuf.time.min,
                 self._protobuf.time.max,
                 st.TimeBase(self._protobuf.time.base),
                 possible_values=self._protobuf.time.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'duration': lambda: visitor.Duration(
+            "duration": lambda: visitor.Duration(
                 self._protobuf.duration.unit,
                 self._protobuf.duration.min,
                 self._protobuf.duration.max,
                 possible_values=self._protobuf.duration.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'constrained': lambda: visitor.Constrained(
+            "constrained": lambda: visitor.Constrained(
                 Type(self._protobuf.constrained.type),
                 Predicate(self._protobuf.constrained.constraint),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'hypothesis': lambda: visitor.Hypothesis(
+            "hypothesis": lambda: visitor.Hypothesis(
                 *[
                     (Type(scored.type), scored.score)
                     for scored in self._protobuf.hypothesis.types
                 ],
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
             None: lambda: None,
-        }[self._protobuf.WhichOneof('type')]
+        }[self._protobuf.WhichOneof("type")]
         dispatch()
 
     # A NewVisitor acceptor
     def accept_(self, visitor: st.TypeVisitor_[VisitedType]) -> VisitedType:
         dispatch: t.Callable[[], VisitedType] = {
-            'null': lambda: visitor.Null(properties=self._protobuf.properties),
-            'unit': lambda: visitor.Unit(properties=self._protobuf.properties),
-            'boolean': lambda: visitor.Boolean(
+            "null": lambda: visitor.Null(properties=self._protobuf.properties),
+            "unit": lambda: visitor.Unit(properties=self._protobuf.properties),
+            "boolean": lambda: visitor.Boolean(
                 properties=self._protobuf.properties
             ),
-            'integer': lambda: visitor.Integer(
+            "integer": lambda: visitor.Integer(
                 min=self._protobuf.integer.min,
                 max=self._protobuf.integer.max,
                 base=st.IntegerBase(self._protobuf.integer.base),
                 possible_values=self._protobuf.integer.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'id': lambda: visitor.Id(
+            "id": lambda: visitor.Id(
                 base=st.IdBase(self._protobuf.id.base),
                 unique=self._protobuf.id.unique,
                 reference=Path(self._protobuf.id.reference)
                 if self._protobuf.id.reference != sp.Path()
                 else None,
                 properties=self._protobuf.properties,
             ),
-            'enum': lambda: visitor.Enum(
+            "enum": lambda: visitor.Enum(
                 self._protobuf.name,
                 [
                     (name_value.name, name_value.value)
                     for name_value in self._protobuf.enum.name_values
                 ],
                 self._protobuf.enum.ordered,
                 properties=self._protobuf.properties,
             ),
-            'float': lambda: visitor.Float(
+            "float": lambda: visitor.Float(
                 min=self._protobuf.float.min,
                 max=self._protobuf.float.max,
                 base=st.FloatBase(self._protobuf.float.base),
                 possible_values=self._protobuf.float.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'text': lambda: visitor.Text(
+            "text": lambda: visitor.Text(
                 self._protobuf.text.encoding,
                 possible_values=self._protobuf.text.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'bytes': lambda: visitor.Bytes(
+            "bytes": lambda: visitor.Bytes(
                 properties=self._protobuf.properties
             ),
-            'struct': lambda: visitor.Struct(
+            "struct": lambda: visitor.Struct(
                 {
                     field.name: Type(field.type).accept_(visitor)
                     for field in self._protobuf.struct.fields
                 },
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'union': lambda: visitor.Union(
+            "union": lambda: visitor.Union(
                 {
                     field.name: Type(field.type).accept_(visitor)
                     for field in self._protobuf.union.fields
                 },
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'optional': lambda: visitor.Optional(
+            "optional": lambda: visitor.Optional(
                 Type(self._protobuf.optional.type).accept_(visitor),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'list': lambda: visitor.List(
+            "list": lambda: visitor.List(
                 Type(self._protobuf.list.type).accept_(visitor),
                 max_size=self._protobuf.list.max_size,
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'array': lambda: visitor.Array(
+            "array": lambda: visitor.Array(
                 Type(self._protobuf.array.type).accept_(visitor),
                 tuple(self._protobuf.array.shape),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'datetime': lambda: visitor.Datetime(
+            "datetime": lambda: visitor.Datetime(
                 self._protobuf.datetime.format,
                 self._protobuf.datetime.min,
                 self._protobuf.datetime.max,
                 st.DatetimeBase(self._protobuf.datetime.base),
                 possible_values=self._protobuf.datetime.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'date': lambda: visitor.Date(
+            "date": lambda: visitor.Date(
                 self._protobuf.date.format,
                 self._protobuf.date.min,
                 self._protobuf.date.max,
                 st.DateBase(self._protobuf.date.base),
                 possible_values=self._protobuf.date.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'time': lambda: visitor.Time(
+            "time": lambda: visitor.Time(
                 self._protobuf.time.format,
                 self._protobuf.time.min,
                 self._protobuf.time.max,
                 st.TimeBase(self._protobuf.time.base),
                 possible_values=self._protobuf.time.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'duration': lambda: visitor.Duration(
+            "duration": lambda: visitor.Duration(
                 self._protobuf.duration.unit,
                 self._protobuf.duration.min,
                 self._protobuf.duration.max,
                 possible_values=self._protobuf.duration.possible_values,
                 properties=self._protobuf.properties,
             ),
-            'constrained': lambda: visitor.Constrained(
+            "constrained": lambda: visitor.Constrained(
                 Type(self._protobuf.constrained.type).accept_(visitor),
                 Predicate(self._protobuf.constrained.constraint),
-                None if self._protobuf.name == '' else self._protobuf.name,
+                None if self._protobuf.name == "" else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
-            'hypothesis': lambda: visitor.Hypothesis(
+            "hypothesis": lambda: visitor.Hypothesis(
                 *[
                     (Type(scored.type).accept_(visitor), scored.score)
                     for scored in self._protobuf.hypothesis.types
                 ],
                 name=None
-                if self._protobuf.name == ''
+                if self._protobuf.name == ""
                 else self._protobuf.name,
                 properties=self._protobuf.properties,
             ),
             None: lambda: visitor.default(),
-        }[self._protobuf.WhichOneof('type')]
+        }[self._protobuf.WhichOneof("type")]
         return dispatch()
 
     def latex(self) -> str:
         """return a latex representation of the type"""
 
         class Latex(TypeVisitor_[str]):
             def default(self) -> str:
-                return r''
+                return r""
 
             def Null(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'\emptyset'
+                return r"\emptyset"
 
             def Unit(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'\mathbb{1}'
+                return r"\mathbb{1}"
 
             def Boolean(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'\left\{0,1\right}'
+                return r"\left\{0,1\right}"
 
             def Integer(
                 self,
                 min: int,
                 max: int,
                 base: st.IntegerBase,
                 possible_values: t.Iterable[int],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if (
                     min <= np.iinfo(np.int32).min
                     or max >= np.iinfo(np.int32).max
                 ):
-                    return r'\mathbb{N}'
+                    return r"\mathbb{N}"
                 else:
-                    return r'\left[' + str(min) + r'..' + str(max) + r'\right]'
+                    return r"\left[" + str(min) + r".." + str(max) + r"\right]"
 
             def Enum(
                 self,
                 name: str,
                 name_values: t.Sequence[t.Tuple[str, int]],
                 ordered: bool,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                result = ''
+                result = ""
                 if len(name_values) > 3:
-                    result += r'\left\{'
+                    result += r"\left\{"
                     for name, _ in name_values[:2]:
-                        result += r'\text{' + name + r'}, '
-                    result += r',\ldots, '
+                        result += r"\text{" + name + r"}, "
+                    result += r",\ldots, "
                     for name, _ in name_values[-1:]:
-                        result += r'\text{' + name + r'}, '
-                    result = result[:-2] + r'\right\}'
+                        result += r"\text{" + name + r"}, "
+                    result = result[:-2] + r"\right\}"
                 elif len(name_values) > 0:
-                    result = r'\left\{'
+                    result = r"\left\{"
                     for name, _ in name_values:
-                        result += r'\text{' + name + r'}, '
-                    result = result[:-2] + r'\right\}'
+                        result += r"\text{" + name + r"}, "
+                    result = result[:-2] + r"\right\}"
                 else:
                     result = self.Unit()
                 return result
 
             def Float(
                 self,
                 min: float,
@@ -490,228 +490,228 @@
                 possible_values: t.Iterable[float],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if (
                     min <= np.finfo(np.float32).min
                     or max >= np.finfo(np.float32).max
                 ):
-                    return r'\mathbb{R}'
+                    return r"\mathbb{R}"
                 else:
-                    return r'\left[' + str(min) + r', ' + str(max) + r'\right]'
+                    return r"\left[" + str(min) + r", " + str(max) + r"\right]"
 
             def Text(
                 self,
                 encoding: str,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'\text{Text}'
+                return r"\text{Text}"
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'\text{Bytes}'
+                return r"\text{Bytes}"
 
             def Struct(
                 self,
                 fields: t.Mapping[str, str],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if len(fields) > 0:
                     if name is None:
-                        result = r'\left\{'
+                        result = r"\left\{"
                     else:
-                        result = r'\text{' + name + r'}: \left\{'
+                        result = r"\text{" + name + r"}: \left\{"
                     for type_name, type_ in fields.items():
                         result = (
                             result
-                            + r'\text{'
+                            + r"\text{"
                             + type_name
-                            + r'}:'
+                            + r"}:"
                             + type_
-                            + r', '
+                            + r", "
                         )
-                    result = result[:-2] + r'\right\}'
+                    result = result[:-2] + r"\right\}"
                     return result
                 else:
                     return self.Unit()
 
             def Union(
                 self,
                 fields: t.Mapping[str, str],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 result = ""
                 if len(fields) > 0:
                     for type_ in fields.values():
-                        result = result + type_ + r' | '
+                        result = result + type_ + r" | "
                     result = result[:-2]
-                    result = r'\left(' + result + r'\right)'
+                    result = r"\left(" + result + r"\right)"
                 else:
                     result = self.Null()
                 return result
 
             def Optional(
                 self,
                 type_: str,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return type_ + r'?'
+                return type_ + r"?"
 
             def List(
                 self,
                 type_: str,
                 max_size: int,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if max_size < 100:
-                    return type_ + r'^{' + str(max_size) + r'}'
+                    return type_ + r"^{" + str(max_size) + r"}"
                 else:
-                    return type_ + r'^*'
+                    return type_ + r"^*"
 
             def Array(
                 self,
                 type_: str,
                 shape: t.Tuple[int, ...],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 return (
                     type_
-                    + r'^{'
-                    + r'\times '.join([str(i) for i in shape])
-                    + r'}'
+                    + r"^{"
+                    + r"\times ".join([str(i) for i in shape])
+                    + r"}"
                 )
 
             def Datetime(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.DatetimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'\text{Datetime}'
+                return r"\text{Datetime}"
 
             def Date(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.DateBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'\text{Date}'
+                return r"\text{Date}"
 
             def Time(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.TimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'\text{Time}'
+                return r"\text{Time}"
 
             def Duration(
                 self,
                 unit: str,
                 min: int,
                 max: int,
                 possible_values: t.Iterable[int],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'\text{Duration}'
+                return r"\text{Duration}"
 
             def Hypothesis(
                 self,
                 *types: t.Tuple[str, float],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 result = ""
                 if len(types) > 0:
                     for type_, score in types:
-                        result = result + type_ + f',{score}|'
+                        result = result + type_ + f",{score}|"
                     result = result[:-2]
-                    result = r'\langle' + result + r'\rangle'
+                    result = r"\langle" + result + r"\rangle"
                 else:
                     result = self.Null()
                 return result
 
         visitor = Latex()
         return self.accept_(visitor)
 
     def compact(self: st.Type) -> str:
         """return a compact representation of the type"""
 
         class Compact(TypeVisitor_[str]):
             def default(self) -> str:
-                return r''
+                return r""
 
             def Null(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'∅'
+                return r"∅"
 
             def Unit(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'𝟙'
+                return r"𝟙"
 
             def Boolean(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'𝔹'
+                return r"𝔹"
 
             def Integer(
                 self,
                 min: int,
                 max: int,
                 base: st.IntegerBase,
                 possible_values: t.Iterable[int],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if (
                     min <= np.iinfo(np.int32).min
                     or max >= np.iinfo(np.int32).max
                 ):
-                    return r'ℕ'
+                    return r"ℕ"
                 else:
-                    return r'[' + str(min) + r'..' + str(max) + r']'
+                    return r"[" + str(min) + r".." + str(max) + r"]"
 
             def Enum(
                 self,
                 name: str,
                 name_values: t.Sequence[t.Tuple[str, int]],
                 ordered: bool,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                result = r''
+                result = r""
                 if len(name_values) > 3:
-                    result = r'{'
+                    result = r"{"
                     for name, _ in name_values[:2]:
                         result += name
-                    result += r',..., '
+                    result += r",..., "
                     for name, _ in name_values[-1:]:
-                        result += name + r', '
-                    result = result[:-2] + r'}'
+                        result += name + r", "
+                    result = result[:-2] + r"}"
                     return result
                 elif len(name_values) > 0:
-                    result = r'{'
+                    result = r"{"
                     for name, _ in name_values:
-                        result += name + r', '
-                    result = result[:-2] + r'}'
+                        result += name + r", "
+                    result = result[:-2] + r"}"
                 else:
                     result = self.Unit()
                 return result
 
             def Float(
                 self,
                 min: float,
@@ -720,146 +720,146 @@
                 possible_values: t.Iterable[float],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if (
                     min <= np.finfo(np.float32).min
                     or max >= np.finfo(np.float32).max
                 ):
-                    return r'ℝ'
+                    return r"ℝ"
                 else:
-                    return r'[' + str(min) + r', ' + str(max) + r']'
+                    return r"[" + str(min) + r", " + str(max) + r"]"
 
             def Text(
                 self,
                 encoding: str,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'𝒯'
+                return r"𝒯"
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> str:
-                return r'ℬ'
+                return r"ℬ"
 
             def Struct(
                 self,
                 fields: t.Mapping[str, str],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if len(fields) > 0:
                     if name is None:
-                        result = '{'
+                        result = "{"
                     else:
-                        result = name + r': {'
+                        result = name + r": {"
                     for type_name, type_ in fields.items():
-                        result = result + type_name + r': ' + type_ + r', '
-                    result = result[:-2] + r'}'
+                        result = result + type_name + r": " + type_ + r", "
+                    result = result[:-2] + r"}"
                     return result
                 else:
                     return self.Unit()
 
             def Union(
                 self,
                 fields: t.Mapping[str, str],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if len(fields) > 0:
-                    result = ''
+                    result = ""
                     for compact in fields.values():
-                        result = result + compact + r' | '
-                    result = r'(' + result[:-2] + r')'
+                        result = result + compact + r" | "
+                    result = r"(" + result[:-2] + r")"
                     return result
                 else:
                     return self.Null()
 
             def Optional(
                 self,
                 type_: str,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return type_ + r'?'
+                return type_ + r"?"
 
             def List(
                 self,
                 type_: str,
                 max_size: int,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return type_ + r'*'
+                return type_ + r"*"
 
             def Array(
                 self,
                 type_: str,
                 shape: t.Tuple[int, ...],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 return (
-                    type_ + r'**(' + r'x'.join([str(i) for i in shape]) + r')'
+                    type_ + r"**(" + r"x".join([str(i) for i in shape]) + r")"
                 )
 
             def Datetime(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.DatetimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'𝒟𝓉'
+                return r"𝒟𝓉"
 
             def Date(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.DateBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'𝒟𝒶'
+                return r"𝒟𝒶"
 
             def Time(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.TimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'𝒯𝓂'
+                return r"𝒯𝓂"
 
             def Duration(
                 self,
                 unit: str,
                 min: int,
                 max: int,
                 possible_values: t.Iterable[int],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
-                return r'𝒟𝓊'
+                return r"𝒟𝓊"
 
             def Hypothesis(
                 self,
                 *types: t.Tuple[str, float],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> str:
                 if len(types) > 0:
-                    result = r'<'
+                    result = r"<"
                     for type_, score in types:
-                        result = result + type_ + f',{score}|'
-                    result = result[:-1] + r'>'
+                        result = result + type_ + f",{score}|"
+                    result = result[:-1] + r">"
                     return result
                 else:
                     return self.Null()
 
         visitor = Compact()
         return self.accept_(visitor)
 
@@ -980,15 +980,15 @@
                 proto = item.protobuf()
                 new_fields = {}
                 for path in proto.paths:
                     # here struct each path must have a label
                     new_fields[path.label] = fields[path.label].get(Path(path))
                 self.result = Struct(
                     fields=new_fields if len(new_fields) > 0 else fields,
-                    name=name if name is not None else 'Struct',
+                    name=name if name is not None else "Struct",
                     properties=self.properties,
                 )
 
             def Union(
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
@@ -996,15 +996,15 @@
             ) -> None:
                 proto = item.protobuf()
                 new_fields = {}
                 for path in proto.paths:
                     new_fields[path.label] = fields[path.label].get(Path(path))
                 self.result = Union(
                     fields=new_fields if len(new_fields) > 0 else fields,
-                    name=name if name is not None else 'Union',
+                    name=name if name is not None else "Union",
                     properties=self.properties,
                 )
 
             def Optional(
                 self,
                 type: st.Type,
                 name: t.Optional[str] = None,
@@ -1234,15 +1234,15 @@
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 paths = []
                 for type_name, curr_type in fields.items():
-                    if curr_type.protobuf().WhichOneof('type') == 'struct':
+                    if curr_type.protobuf().WhichOneof("type") == "struct":
                         paths.append(Path(sp.Path(label=type_name)))
                     else:
                         sub_paths = curr_type.structs()
                         if sub_paths is not None:
                             paths.extend(
                                 [
                                     Path(
@@ -1259,15 +1259,15 @@
 
             def Optional(
                 self,
                 type: st.Type,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-                if type.protobuf().WhichOneof('type') == 'struct':
+                if type.protobuf().WhichOneof("type") == "struct":
                     self.result = [Path(sp.Path(label=OPTIONAL_VALUE))]
                 else:
                     sub_paths = type.structs()
                     if sub_paths is not None:
                         self.result = [
                             Path(
                                 sp.Path(
@@ -1283,15 +1283,15 @@
             def List(
                 self,
                 type: st.Type,
                 max_size: int,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-                if type.protobuf().WhichOneof('type') == 'struct':
+                if type.protobuf().WhichOneof("type") == "struct":
                     self.result = [Path(sp.Path(label=LIST_VALUES))]
                 else:
                     sub_paths = type.structs()
                     if sub_paths is not None:
                         self.result = [
                             Path(
                                 sp.Path(
@@ -1307,15 +1307,15 @@
             def Array(
                 self,
                 type: st.Type,
                 shape: t.Tuple[int, ...],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-                if type.protobuf().WhichOneof('type') == 'struct':
+                if type.protobuf().WhichOneof("type") == "struct":
                     self.result = [Path(sp.Path(label=ARRAY_VALUES))]
                 else:
                     sub_paths = type.structs()
                     if sub_paths is not None:
                         self.result = [
                             Path(
                                 sp.Path(
@@ -1500,17 +1500,17 @@
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 # TODO: we should clarify for Ids, user_input
                 # and so on, to be consistent
                 if base == st.IdBase.STRING:
                     self.Text(
                         encoding="",
-                        possible_values=['1'],
+                        possible_values=["1"],
                         properties={
-                            TEXT_CHARSET: "[\"1\"]",
+                            TEXT_CHARSET: '["1"]',
                             TEXT_MAX_LENGTH: "1",
                         },
                     )
                 elif base in (
                     st.IdBase.INT8,
                     st.IdBase.INT16,
                     st.IdBase.INT32,
@@ -1581,35 +1581,35 @@
             ) -> None:
                 try:
                     char_set = json.loads(self.properties[TEXT_CHARSET])
                 except json.JSONDecodeError:
                     self.result = pa.array([""], pa.large_string())
                 else:
                     max_length = int(self.properties[TEXT_MAX_LENGTH])
-                    ex = ''.join(char_set)
+                    ex = "".join(char_set)
                     if len(ex) > max_length:
                         ex = ex[:max_length]
                     self.result = pa.array([ex], pa.large_string())
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
                 self.result = pa.array(
-                    [bytes('1', 'utf-8')], pa.binary(length=1)
+                    [bytes("1", "utf-8")], pa.binary(length=1)
                 )
 
             def Struct(
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 assert properties is not None
-                if properties['kind'] == 'text':
-                    max_size = fields['input_ids'].protobuf().list.max_size
+                if properties["kind"] == "text":
+                    max_size = fields["input_ids"].protobuf().list.max_size
                     if max_size == np.iinfo(np.int64).max:
                         # there is no convention given
                         # on the max size so we take 1
                         pos_ids = pa.ListArray.from_arrays(
                             offsets=[0, 1],
                             values=pa.concat_arrays([pa.array([0])]),
                         )
@@ -1637,46 +1637,45 @@
                             values=pa.array([0] * max_size),
                         )
 
                     self.result = pa.StructArray.from_arrays(
                         arrays=[input_ids, attention_mask, pos_ids],
                         fields=[
                             pa.field(
-                                name='input_ids',
+                                name="input_ids",
                                 type=input_ids.type,
                                 nullable=False,
                             ),
                             pa.field(
-                                name='attention_mask',
+                                name="attention_mask",
                                 type=attention_mask.type,
                                 nullable=False,
                             ),
                             pa.field(
-                                name='position_ids',
+                                name="position_ids",
                                 type=pos_ids.type,
                                 nullable=False,
                             ),
                         ],
                     )
 
                 else:
-
                     arrays = [
                         field_type.example() for field_type in fields.values()
                     ]
 
                     self.result = pa.StructArray.from_arrays(
                         arrays=arrays,
                         fields=[
                             pa.field(
                                 name=field_name,
                                 nullable=field_type.protobuf().HasField(
-                                    'optional'
+                                    "optional"
                                 )
-                                or field_type.protobuf().HasField('unit'),
+                                or field_type.protobuf().HasField("unit"),
                                 type=array.type,
                             )
                             for (field_name, field_type), array in zip(
                                 fields.items(), arrays
                             )
                         ],
                     )
@@ -1694,15 +1693,15 @@
                     early_arr = pa.nulls(j, type=middle_arr.type)
                     late_arr = pa.nulls(n_fields - j - 1, type=middle_arr.type)
                     arrays.append(
                         pa.concat_arrays([early_arr, middle_arr, late_arr])
                     )
                 names = list(fields.keys())
                 arrays.append(pa.array(names, pa.large_string()))
-                names.append('field_selected')
+                names.append("field_selected")
                 self.result = pa.StructArray.from_arrays(
                     arrays=arrays,
                     names=names,
                 )
 
             def Optional(
                 self,
@@ -1740,15 +1739,15 @@
                 min: str,
                 max: str,
                 base: st.DatetimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 self.result = pa.array(
-                    pd.to_datetime([max], format=format), pa.timestamp('ns')
+                    pd.to_datetime([max], format=format), pa.timestamp("ns")
                 )
 
         visitor = Example(properties=self.properties())
         self.accept(visitor)
         return visitor.result
 
     def numpy_example(self) -> np.ndarray:
@@ -1787,15 +1786,15 @@
                 reference: t.Optional[st.Path] = None,
                 base: t.Optional[st.IdBase] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 # TODO: we should clarify for Ids, user_input
                 # and so on, to be consistent
                 if base == st.IdBase.STRING:
-                    self.result = tf.constant(['1'], tf.string)
+                    self.result = tf.constant(["1"], tf.string)
                 elif base == st.IdBase.INT64:
                     self.result = tf.constant([1], tf.int64)
                 else:
                     raise NotImplementedError
 
             def Integer(
                 self,
@@ -1834,23 +1833,23 @@
             ) -> None:
                 try:
                     char_set = json.loads(self.properties[TEXT_CHARSET])
                 except json.JSONDecodeError:
                     self.result = tf.constant([""], tf.string)
                 else:
                     max_length = int(self.properties[TEXT_MAX_LENGTH])
-                    ex = ''.join(char_set)
+                    ex = "".join(char_set)
                     if len(ex) > max_length:
                         ex = ex[:max_length]
                     self.result = tf.constant([ex], tf.string)
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
-                self.result = tf.constant(['1'], tf.string)
+                self.result = tf.constant(["1"], tf.string)
 
             def Struct(
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
@@ -1873,16 +1872,16 @@
             def Optional(
                 self,
                 type: st.Type,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 self.result = {
-                    'input_mask': tf.constant([1], dtype=tf.int64),
-                    'values': type.tensorflow_example(),
+                    "input_mask": tf.constant([1], dtype=tf.int64),
+                    "values": type.tensorflow_example(),
                 }
 
             def Datetime(
                 self,
                 format: str,
                 min: str,
                 max: str,
@@ -1926,15 +1925,15 @@
                 reference: t.Optional[st.Path] = None,
                 base: t.Optional[st.IdBase] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 # TODO: we should clarify for Ids, user_input
                 # and so on, to be consistent
                 if base == st.IdBase.STRING:
-                    self.result = pa.array(['1'], pa.large_string())
+                    self.result = pa.array(["1"], pa.large_string())
                 elif base == st.IdBase.INT64:
                     self.result = pa.array([1], pa.int64())
                 else:
                     raise NotImplementedError
 
             def Integer(
                 self,
@@ -1973,24 +1972,24 @@
             ) -> None:
                 try:
                     char_set = json.loads(self.properties[TEXT_CHARSET])
                 except json.JSONDecodeError:
                     self.result = pa.array([""], pa.large_string())
                 else:
                     max_length = int(self.properties[TEXT_MAX_LENGTH])
-                    ex = ''.join(char_set)
+                    ex = "".join(char_set)
                     if len(ex) > max_length:
                         ex = ex[:max_length]
                     self.result = pa.array([ex], pa.large_string())
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
                 self.result = pa.array(
-                    [bytes('1', 'utf-8')], pa.binary(length=1)
+                    [bytes("1", "utf-8")], pa.binary(length=1)
                 )
 
             def Struct(
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
@@ -2015,15 +2014,15 @@
                     early_arr = pa.nulls(j, type=middle_arr.type)
                     late_arr = pa.nulls(n_fields - j - 1, type=middle_arr.type)
                     arrays.append(
                         pa.concat_arrays([early_arr, middle_arr, late_arr])
                     )
                 names = list(fields.keys())
                 arrays.append(pa.array(names, pa.large_string()))
-                names.append('field_selected')
+                names.append("field_selected")
                 self.result = pa.StructArray.from_arrays(
                     arrays=arrays,
                     names=names,
                 )
 
             def Optional(
                 self,
@@ -2039,15 +2038,15 @@
                 min: str,
                 max: str,
                 base: st.DatetimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 self.result = pa.array(
-                    pd.to_datetime([max], format=format), pa.timestamp('ns')
+                    pd.to_datetime([max], format=format), pa.timestamp("ns")
                 )
 
         visitor = Default(properties=self.properties())
         self.accept(visitor)
         return visitor.result
 
     def numpy_default(self) -> np.ndarray:
@@ -2093,24 +2092,24 @@
                 base: t.Optional[st.IdBase] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 # TODO: we should clarify for Ids, user_input
                 # and so on, to be consistent
                 if is_optional:
                     if base == st.IdBase.STRING:
-                        self.result = tf.constant([''], dtype=tf.string)
+                        self.result = tf.constant([""], dtype=tf.string)
                     elif base == st.IdBase.INT64:
                         self.result = tf.constant(
                             [np.iinfo(np.int64).max], pa.large_string()
                         )
                     else:
                         raise NotImplementedError
                 else:
                     if base == st.IdBase.STRING:
-                        self.result = tf.constant(['1'], tf.string)
+                        self.result = tf.constant(["1"], tf.string)
                     elif base == st.IdBase.INT64:
                         self.result = tf.constant([1], tf.int64)
                     else:
                         raise NotImplementedError
 
             def Integer(
                 self,
@@ -2133,15 +2132,15 @@
                 self,
                 name: str,
                 name_values: t.Sequence[t.Tuple[str, int]],
                 ordered: bool,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 if is_optional:
-                    self.result = tf.constant([''], dtype=tf.string)
+                    self.result = tf.constant([""], dtype=tf.string)
                 else:
                     self.result = tf.constant([name_values[0][0]], tf.string)
 
             def Float(
                 self,
                 min: float,
                 max: float,
@@ -2159,34 +2158,34 @@
             def Text(
                 self,
                 encoding: str,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 if is_optional:
-                    self.result = tf.constant([''], dtype=tf.string)
+                    self.result = tf.constant([""], dtype=tf.string)
                 else:
                     try:
                         char_set = json.loads(self.properties[TEXT_CHARSET])
                     except json.JSONDecodeError:
                         self.result = tf.constant([""], tf.string)
                     else:
                         max_length = int(self.properties[TEXT_MAX_LENGTH])
-                        ex = ''.join(char_set)
+                        ex = "".join(char_set)
                         if len(ex) > max_length:
                             ex = ex[:max_length]
                         self.result = tf.constant([ex], tf.string)
 
             def Bytes(
                 self, properties: t.Optional[t.Mapping[str, str]] = None
             ) -> None:
                 if is_optional:
-                    self.result = tf.constant([''], dtype=tf.string)
+                    self.result = tf.constant([""], dtype=tf.string)
                 else:
-                    self.result = tf.constant(['1'], tf.string)
+                    self.result = tf.constant(["1"], tf.string)
 
             def Struct(
                 self,
                 fields: t.Mapping[str, st.Type],
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
@@ -2213,29 +2212,29 @@
             def Optional(
                 self,
                 type: st.Type,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 self.result = {
-                    'input_mask': tf.constant([0], dtype=tf.int64),
-                    'values': type.tensorflow_default(is_optional=True),
+                    "input_mask": tf.constant([0], dtype=tf.int64),
+                    "values": type.tensorflow_default(is_optional=True),
                 }
 
             def Datetime(
                 self,
                 format: str,
                 min: str,
                 max: str,
                 base: st.DatetimeBase,
                 possible_values: t.Iterable[str],
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
                 if is_optional:
-                    self.result = tf.constant([''], dtype=tf.string)
+                    self.result = tf.constant([""], dtype=tf.string)
                 else:
                     self.result = tf.constant([min], dtype=tf.string)
 
         visitor = ToTensorflow(properties=self.properties())
         self.accept(visitor)
         return visitor.result
 
@@ -2291,15 +2290,14 @@
 
             def Optional(
                 self,
                 type: st.Type,
                 name: t.Optional[str] = None,
                 properties: t.Optional[t.Mapping[str, str]] = None,
             ) -> None:
-
                 sub_paths = type.path_leaves()
                 if len(sub_paths) > 0:
                     self.result.extend(
                         [
                             path_builder(label=OPTIONAL_VALUE, paths=[el])
                             for el in sub_paths
                         ]
@@ -2664,46 +2662,46 @@
 
 
 # A few builders
 def Null(
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
-        sp.Type(name='Null', null=sp.Type.Null(), properties=properties)
+        sp.Type(name="Null", null=sp.Type.Null(), properties=properties)
     )
 
 
 def Unit(properties: t.Optional[t.Mapping[str, str]] = None) -> Type:
     return Type(
-        sp.Type(name='Unit', unit=sp.Type.Unit(), properties=properties)
+        sp.Type(name="Unit", unit=sp.Type.Unit(), properties=properties)
     )
 
 
 def Id(
     unique: bool,
     base: t.Optional[st.IdBase] = None,
     reference: t.Optional[st.Path] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     if base is None:
         base = st.IdBase.STRING
     if reference is None:
         return Type(
             sp.Type(
-                name='Id',
+                name="Id",
                 id=sp.Type.Id(
                     base=BASE_ID_TO_PROTO[base.value],
                     unique=unique,
                 ),
                 properties=properties,
             )
         )
     return Type(
         sp.Type(
-            name='Id',
+            name="Id",
             id=sp.Type.Id(
                 base=BASE_ID_TO_PROTO[base.value],
                 unique=unique,
                 reference=reference.protobuf(),
             ),
             properties=properties,
         )
@@ -2711,15 +2709,15 @@
 
 
 def Boolean(
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
-            name='Boolean', boolean=sp.Type.Boolean(), properties=properties
+            name="Boolean", boolean=sp.Type.Boolean(), properties=properties
         )
     )
 
 
 def Integer(
     min: t.Optional[int] = None,
     max: t.Optional[int] = None,
@@ -2745,15 +2743,15 @@
             max = np.iinfo(np.int32).max
         elif base == st.IntegerBase.INT16:
             max = np.iinfo(np.int16).max
         else:
             max = np.iinfo(np.int8).max
     return Type(
         sp.Type(
-            name='Integer',
+            name="Integer",
             integer=sp.Type.Integer(
                 base=BASE_INT_TO_PROTO[base.value],
                 min=min,
                 max=max,
                 possible_values=possible_values,
             ),
             properties=properties,
@@ -2824,49 +2822,49 @@
             max = np.finfo(np.float64).max  # type:ignore
         elif base == st.FloatBase.FLOAT32:
             max = np.finfo(np.float32).max  # type:ignore
         else:
             max = np.finfo(np.float16).max  # type:ignore
     return Type(
         sp.Type(
-            name='Float64',
+            name="Float64",
             float=sp.Type.Float(
                 base=BASE_FLOAT_TO_PROTO[base.value],
                 min=min,  # type:ignore
                 max=max,  # type:ignore
                 possible_values=possible_values,
             ),
             properties=properties,
         )
     )
 
 
 def Text(
-    encoding: str = 'UTF-8',
+    encoding: str = "UTF-8",
     possible_values: t.Optional[t.Iterable[str]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
-            name=f'Text {encoding}',
+            name=f"Text {encoding}",
             text=sp.Type.Text(
-                encoding='UTF-8', possible_values=possible_values
+                encoding="UTF-8", possible_values=possible_values
             ),
             properties=properties,
         )
     )
 
 
 def Bytes() -> Type:
-    return Type(sp.Type(name='Bytes', bytes=sp.Type.Bytes()))
+    return Type(sp.Type(name="Bytes", bytes=sp.Type.Bytes()))
 
 
 def Struct(
     fields: t.Mapping[str, st.Type],
-    name: str = 'Struct',
+    name: str = "Struct",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             struct=sp.Type.Struct(
                 fields=[
@@ -2877,15 +2875,15 @@
             properties=properties,
         )
     )
 
 
 def Union(
     fields: t.Mapping[str, st.Type],
-    name: str = 'Union',
+    name: str = "Union",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             union=sp.Type.Union(
                 fields=[
@@ -2898,45 +2896,45 @@
             properties=properties,
         )
     )
 
 
 def Optional(
     type: st.Type,
-    name: str = 'Optional',
+    name: str = "Optional",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             optional=sp.Type.Optional(type=type.protobuf()),
             properties=properties,
         )
     )
 
 
 def List(
     type: st.Type,
     max_size: int = np.iinfo(np.int64).max,
-    name: str = 'List',
+    name: str = "List",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             list=sp.Type.List(type=type.protobuf(), max_size=max_size),
             properties=properties,
         )
     )
 
 
 def Array(
     type: st.Type,
     shape: t.Sequence[int],
-    name: str = 'Array',
+    name: str = "Array",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             array=sp.Type.Array(type=type.protobuf(), shape=shape),
             properties=properties,
@@ -2949,15 +2947,15 @@
     min: t.Optional[str] = None,
     max: t.Optional[str] = None,
     base: t.Optional[st.DatetimeBase] = None,
     possible_values: t.Optional[t.Iterable[str]] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     if format is None:
-        format = '%Y-%m-%dT%H:%M:%S'
+        format = "%Y-%m-%dT%H:%M:%S"
     if base is None:
         base = st.DatetimeBase.INT64_NS
     assert base == st.DatetimeBase.INT64_NS
     bounds = []
     iint64 = np.iinfo(np.int64)
     for i, bound in enumerate((min, max)):
         if bound is None:  # the bound is assumed to be sound otherwise
@@ -2970,15 +2968,15 @@
             # max = max.astype("datetime64[us]")
             # ```
             # More generally, the date format can only store a bound lower
             # than that bound, which is fine with the max but not for the
             # min, as it truncates some time units.
             if i == 0:
                 int_bound = iint64.min + 1  # iint64.min maps to 'NaT'
-                aliasing = np.timedelta64(0, 'ns')
+                aliasing = np.timedelta64(0, "ns")
                 # This looks for the lowest offset for the format:
                 # see:
                 # https://numpy.org/doc/stable/reference/arrays.datetime.html#datetime-and-timedelta-arithmetic
                 for unit, np_unit in [
                     ("%Y", "Y"),
                     ("%m", "M"),
                     ("%d", "D"),
@@ -2995,28 +2993,28 @@
                         aliasing = np.timedelta64(1, np_unit)
                         aliasing = as_unit + aliasing - as_unit
                         aliasing = aliasing.astype("timedelta64[ns]")
                     else:
                         aliasing = np.timedelta64(1, np_unit)
             elif i == 1:
                 int_bound = iint64.max
-                aliasing = np.timedelta64(0, 'ns')
+                aliasing = np.timedelta64(0, "ns")
             bound = str(
                 (np.datetime64(int_bound, "ns") + aliasing).astype(
                     "datetime64[us]"
                 )
             )
             bound = datetime.datetime.strptime(
-                bound, '%Y-%m-%dT%H:%M:%S.%f'
+                bound, "%Y-%m-%dT%H:%M:%S.%f"
             ).strftime(format)
         bounds.append(bound)
 
     return Type(
         sp.Type(
-            name='Datetime',
+            name="Datetime",
             datetime=sp.Type.Datetime(
                 format=format,
                 min=bounds[0],
                 max=bounds[1],
                 base=BASE_DATETIME_TO_PROTO[base.value],
                 possible_values=possible_values,
             ),
@@ -3045,31 +3043,31 @@
     Default ranges are defined by datetime.date lowest and highest year:
     0001-01-01 and 9999-12-31. Note that if the SQL database has a date outside
     of this range the table reflection would fail since also sql alchemy is
     using datetime.date as an underlying python type.
     """
 
     if format is None:
-        format = '%Y-%m-%d'
+        format = "%Y-%m-%d"
 
     if base is None:
         base = st.DateBase.INT32
 
     if min is None:
         min = datetime.datetime.strptime(
-            str(datetime.date(datetime.MINYEAR, 1, 1)), '%Y-%m-%d'
+            str(datetime.date(datetime.MINYEAR, 1, 1)), "%Y-%m-%d"
         ).strftime(format)
     if max is None:
         max = datetime.datetime.strptime(
-            str(datetime.date(datetime.MAXYEAR, 12, 31)), '%Y-%m-%d'
+            str(datetime.date(datetime.MAXYEAR, 12, 31)), "%Y-%m-%d"
         ).strftime(format)
 
     return Type(
         sp.Type(
-            name='Date',
+            name="Date",
             date=sp.Type.Date(
                 format=format,
                 min=min,
                 max=max,
                 base=BASE_DATE_TO_PROTO[base.value],
                 possible_values=possible_values,
             ),
@@ -3086,20 +3084,20 @@
     base: t.Optional[st.TimeBase] = None,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     """Very similar to Datetime. The difference here is that the
     range is simpler.
     """
     if format is None:
-        format = '%H:%M:%S.%f'
+        format = "%H:%M:%S.%f"
     if base is None:
         base = st.TimeBase.INT64_US
     if base == st.TimeBase.INT64_NS:
         raise NotImplementedError(
-            'time with nanoseconds resolution not supported'
+            "time with nanoseconds resolution not supported"
         )
     if min is None:
         min = datetime.time.min.strftime(
             format.replace("%f", "{__subseconds__}").format(
                 __subseconds__=(
                     "000000" if base == st.TimeBase.INT64_US else "000"
                 )
@@ -3112,15 +3110,15 @@
                     "999999" if base == st.TimeBase.INT64_US else "999"
                 )
             )
         )
 
     return Type(
         sp.Type(
-            name='Time',
+            name="Time",
             time=sp.Type.Time(
                 format=format,
                 min=min,
                 max=max,
                 base=BASE_TIME_TO_PROTO[base.value],
                 possible_values=possible_values,
             ),
@@ -3146,31 +3144,31 @@
     and it would cause problems when pushing to sql (also SQL duration
     types have up to 'us' resolution).
 
     It raises an error if the unit provided is not among:
     ('us','ms', 's'). Default value 'us'
     """
     if unit is None:
-        unit = 'us'
+        unit = "us"
 
     default_bounds = DURATION_UNITS_TO_RANGE.get(unit)
     if default_bounds is None:
         raise ValueError(
-            f'Duration unit {unit} not recongnized'
-            f'Only values in {DURATION_UNITS_TO_RANGE.keys()} are allowed'
+            f"Duration unit {unit} not recongnized"
+            f"Only values in {DURATION_UNITS_TO_RANGE.keys()} are allowed"
         )
 
     bounds = [
         default_bounds[0] if min is None else min,
         default_bounds[1] if max is None else max,
     ]
 
     return Type(
         sp.Type(
-            name='Duration',
+            name="Duration",
             duration=sp.Type.Duration(
                 unit=unit,
                 min=bounds[0],
                 max=bounds[1],
                 possible_values=possible_values,
             ),
             properties=properties,
@@ -3181,26 +3179,26 @@
 def Constrained(
     type: st.Type,
     constraint: Predicate,
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
-            name='Constrained',
+            name="Constrained",
             constrained=sp.Type.Constrained(
                 type=type.protobuf(), constraint=constraint._protobuf
             ),
             properties=properties,
         )
     )
 
 
 def Hypothesis(
     *types: t.Tuple[st.Type, float],
-    name: str = 'Hypothesis',
+    name: str = "Hypothesis",
     properties: t.Optional[t.Mapping[str, str]] = None,
 ) -> Type:
     return Type(
         sp.Type(
             name=name,
             hypothesis=sp.Type.Hypothesis(
                 types=(
@@ -3352,18 +3350,18 @@
     return visitor.project_type
 
 
 def protected_type(input_type: st.Type) -> st.Type:
     """Convert a data Type to a protected Type."""
     protection_fields = {
         PUBLIC: Boolean(),
-        USER_COLUMN: Optional(type=Id(base=st.IdBase.STRING, unique=False)),
+        PU_COLUMN: Optional(type=Id(base=st.IdBase.STRING, unique=False)),
         WEIGHTS: Float(min=0.0, max=np.finfo(np.float64).max),  # type: ignore
     }
-    if input_type.has_protection():
+    if input_type.has_privacy_unit_tracking():
         # Already protected
         return input_type
     elif input_type.has_admin_columns():
         # Add protection to existing admin columns
         fields = {
             **input_type.children(),
             **protection_fields,
@@ -3374,9 +3372,207 @@
         fields = {
             DATA: input_type,
             **protection_fields,
         }
         return Struct(fields=fields)
 
 
+def to_numeric_string(
+    sds_type: st.Type,
+) -> t.Literal["int64", "int32", "int16", "int8", "float32", "float64"]:
+    class ToNumericString(st.TypeVisitor):
+        """Visitor that converts sarus type to a string"""
+
+        str_type: t.Literal[
+            "int64", "int32", "int16", "int8", "float32", "float64"
+        ]
+
+        def Integer(
+            self,
+            min: int,
+            max: int,
+            base: st.IntegerBase,
+            possible_values: t.Iterable[int],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            if base == st.IntegerBase.INT32:
+                self.str_type = "int32"
+            elif base == st.IntegerBase.INT64:
+                self.str_type = "int64"
+            elif base == st.IntegerBase.INT8:
+                self.str_type = "int8"
+            elif base == st.IntegerBase.INT16:
+                self.str_type = "int16"
+            else:
+                raise NotImplementedError
+
+        def Float(
+            self,
+            min: float,
+            max: float,
+            base: st.FloatBase,
+            possible_values: t.Iterable[float],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            if base == st.FloatBase.FLOAT32:
+                self.str_type = "float32"
+            elif base == st.FloatBase.FLOAT64:
+                self.str_type = "float64"
+
+            else:
+                raise NotImplementedError
+
+        def Union(
+            self,
+            fields: t.Mapping[str, st.Type],
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Struct(
+            self,
+            fields: t.Mapping[str, st.Type],
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Optional(
+            self,
+            type: st.Type,
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Array(
+            self,
+            type: st.Type,
+            shape: t.Tuple[int, ...],
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def List(
+            self,
+            type: st.Type,
+            max_size: int,
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Boolean(
+            self, properties: t.Optional[t.Mapping[str, str]] = None
+        ) -> None:
+            raise NotImplementedError
+
+        def Bytes(
+            self, properties: t.Optional[t.Mapping[str, str]] = None
+        ) -> None:
+            raise NotImplementedError
+
+        def Unit(
+            self, properties: t.Optional[t.Mapping[str, str]] = None
+        ) -> None:
+            raise NotImplementedError
+
+        def Constrained(
+            self,
+            type: st.Type,
+            constraint: st.Predicate,
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Date(
+            self,
+            format: str,
+            min: str,
+            max: str,
+            base: st.DateBase,
+            possible_values: t.Iterable[str],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Time(
+            self,
+            format: str,
+            min: str,
+            max: str,
+            base: st.TimeBase,
+            possible_values: t.Iterable[str],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Datetime(
+            self,
+            format: str,
+            min: str,
+            max: str,
+            base: st.DatetimeBase,
+            possible_values: t.Iterable[str],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Duration(
+            self,
+            unit: str,
+            min: int,
+            max: int,
+            possible_values: t.Iterable[int],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Enum(
+            self,
+            name: str,
+            name_values: t.Sequence[t.Tuple[str, int]],
+            ordered: bool,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Text(
+            self,
+            encoding: str,
+            possible_values: t.Iterable[str],
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Hypothesis(
+            self,
+            *types: t.Tuple[st.Type, float],
+            name: t.Optional[str] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Id(
+            self,
+            unique: bool,
+            reference: t.Optional[st.Path] = None,
+            base: t.Optional[st.IdBase] = None,
+            properties: t.Optional[t.Mapping[str, str]] = None,
+        ) -> None:
+            raise NotImplementedError
+
+        def Null(
+            self, properties: t.Optional[t.Mapping[str, str]] = None
+        ) -> None:
+            raise NotImplementedError
+
+    visitor = ToNumericString()
+    sds_type.accept(visitor)
+    return visitor.str_type
+
+
 if t.TYPE_CHECKING:
     test_type: st.Type = Type(sp.Type())
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/typing.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Protocols describing common object behaviors.
-"""
+"""Protocols describing common object behaviors."""
+
 from __future__ import annotations
 
 from abc import abstractmethod
 from enum import Enum, IntEnum
 import datetime as dt
 import logging
 import typing as t
@@ -19,43 +19,36 @@
 import sarus_data_spec.storage.typing as storage_typing
 
 logger = logging.getLogger(__name__)
 
 try:
     import tensorflow as tf
 except ModuleNotFoundError:
-    logger.warning('tensorflow not found, tensorflow datasets not available')
+    logger.warning("tensorflow not found, tensorflow datasets not available")
 
 try:
     import sklearn  # noqa: F401
 except ModuleNotFoundError:
-    logger.warning('sklearn not found, sklearn models not available')
+    logger.warning("sklearn not found, sklearn models not available")
 
 try:
     from sarus_differential_privacy.query import (
         PrivateQuery as RealPrivateQuery,
     )
 
     PrivateQuery = RealPrivateQuery
 except ImportError:
     PrivateQuery = t.Any  # type: ignore
     warnings.warn(
         "`sarus_differential_privacy` not installed. "
         "DP primitives not available."
     )
 
-try:
-    from sarus_query_builder.core.typing import Task as RealTask
-
-    Task = RealTask
-except ImportError:
-    Task = t.Any  # type: ignore
-    warnings.warn(
-        "`sarus_query_builder` not installed. DP methods not available."
-    )
+# this is really bad but in QB actually it is not defined!
+Task = t.Any
 
 try:
     import transformers  # noqa: F401
 except ImportError:
     warnings.warn("`transformers` not installed. LLM not available.")
 
 
@@ -73,15 +66,15 @@
     pd.Series,
     t.Iterator[pa.RecordBatch],
     pd.core.groupby.DataFrameGroupBy,
     pd.core.groupby.SeriesGroupBy,
 ]
 
 
-P = t.TypeVar('P', bound=Protobuf, covariant=True)
+P = t.TypeVar("P", bound=Protobuf, covariant=True)
 
 
 @t.runtime_checkable
 class HasProtobuf(t.Protocol[P]):
     """An object backed by a protocol buffer message."""
 
     def protobuf(self) -> P:
@@ -105,28 +98,23 @@
         ...
 
 
 @t.runtime_checkable
 class Value(t.Protocol):
     """An object with value semantics."""
 
-    def __bytes__(self) -> bytes:
-        ...
+    def __bytes__(self) -> bytes: ...
 
-    def __repr__(self) -> str:
-        ...
+    def __repr__(self) -> str: ...
 
-    def __str__(self) -> str:
-        ...
+    def __str__(self) -> str: ...
 
-    def __eq__(self, value: object) -> bool:
-        ...
+    def __eq__(self, value: object) -> bool: ...
 
-    def __hash__(self) -> int:
-        ...
+    def __hash__(self) -> int: ...
 
 
 @t.runtime_checkable
 class Frozen(t.Protocol):
     """An immutable object."""
 
     def _freeze(self) -> None:
@@ -134,15 +122,15 @@
         ...
 
     def _frozen(self) -> bool:
         """Check if the frozen object was left unchanged"""
         ...
 
 
-PU = t.TypeVar('PU', bound=ProtobufWithUUID, covariant=True)
+PU = t.TypeVar("PU", bound=ProtobufWithUUID, covariant=True)
 
 
 @t.runtime_checkable
 class Referrable(HasProtobuf[PU], Frozen, t.Protocol[PU]):
     """Can be referred to by uuid."""
 
     def uuid(self) -> str:
@@ -151,19 +139,17 @@
 
     def referring(
         self, type_name: t.Optional[str] = None
     ) -> t.Collection[Referring[ProtobufWithUUID]]:
         """Referring objects pointing to this one."""
         ...
 
-    def storage(self) -> storage_typing.Storage:
-        ...
+    def storage(self) -> storage_typing.Storage: ...
 
-    def manager(self) -> manager_typing.Manager:
-        ...
+    def manager(self) -> manager_typing.Manager: ...
 
 
 @t.runtime_checkable
 class Referring(Referrable[PU], Frozen, t.Protocol[PU]):
     """Is referring to other Referrables"""
 
     _referred: t.MutableSet[str] = set()
@@ -173,15 +159,15 @@
         ...
 
     def referred_uuid(self) -> t.Collection[str]:
         """Uuid of object referred by this object"""
         ...
 
 
-FM = t.TypeVar('FM', bound=Protobuf)
+FM = t.TypeVar("FM", bound=Protobuf)
 
 
 @t.runtime_checkable
 class Factory(t.Protocol):
     """Can produce objects from protobuf messages"""
 
     def register(self, name: str, type: t.Type[HasProtobuf[Protobuf]]) -> None:
@@ -190,138 +176,122 @@
 
     def create(self, message: FM, store: bool) -> HasProtobuf[FM]:
         """Returns a wrapped protobuf"""
         ...
 
 
 class VariantConstraint(Referrable[sp.VariantConstraint], t.Protocol):
-    def constraint_kind(self) -> ConstraintKind:
-        ...
+    def constraint_kind(self) -> ConstraintKind: ...
 
-    def required_context(self) -> t.List[str]:
-        ...
+    def required_context(self) -> t.List[str]: ...
 
-    def privacy_limit(self) -> t.Optional[PrivacyLimit]:
-        ...
+    def privacy_limit(self) -> t.Optional[PrivacyLimit]: ...
 
-    def accept(self, visitor: TransformVisitor) -> None:
-        ...
+    def accept(self, visitor: TransformVisitor) -> None: ...
 
 
 # Type alias
-DS = t.TypeVar('DS', bound=t.Union[sp.Scalar, sp.Dataset])
+DS = t.TypeVar("DS", bound=t.Union[sp.Scalar, sp.Dataset])
 
 
 class Attribute(Referring[sp.Attribute], t.Protocol):
-    def prototype(self) -> t.Type[sp.Attribute]:
-        ...
+    def prototype(self) -> t.Type[sp.Attribute]: ...
 
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
 
 @t.runtime_checkable
 class DataSpec(Referring[DS], t.Protocol):
     def parents(
         self,
     ) -> t.Tuple[
         t.List[t.Union[DataSpec[DS], Transform]],
         t.Dict[str, t.Union[DataSpec[DS], Transform]],
-    ]:
-        ...
+    ]: ...
 
     def parents_list(
         self,
-    ) -> t.List[DataSpec[DS]]:
-        ...
+    ) -> t.List[DataSpec[DS]]: ...
 
     def variant(
         self,
         kind: ConstraintKind,
         public_context: t.Collection[str] = (),
         privacy_limit: t.Optional[PrivacyLimit] = None,
         salt: t.Optional[int] = None,
-    ) -> t.Optional[DataSpec[DS]]:
-        ...
+    ) -> t.Optional[DataSpec[DS]]: ...
 
-    def variants(self) -> t.Collection[DataSpec]:
-        ...
+    def variants(self) -> t.Collection[DataSpec]: ...
 
     def private_queries(self) -> t.List[PrivateQuery]:
         """Return the list of PrivateQueries used in a Dataspec's transform.
 
         It represents the privacy loss associated with the current computation.
 
         It can be used by Sarus when a user (Access object) reads a DP dataspec
         to update its accountant. Note that Private Query objects are generated
         with a random uuid so that even if they are submitted multiple times to
         an account, they are only accounted once (ask @cgastaud for more on
         accounting)."""
         ...
 
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
-    def doc(self) -> str:
-        ...
+    def doc(self) -> str: ...
 
-    def is_pep(self) -> bool:
-        ...
+    def is_pup(self) -> bool: ...
 
-    def pep_token(self) -> t.Optional[str]:
-        """Returns a PEP token if the dataset is PEP and None otherwise.
+    def pup_token(self) -> t.Optional[str]:
+        """Returns a PUP token if the dataset is PUP and None otherwise.
 
-        The PEP token is stored in the properties of the VariantConstraint. It
+        The PUP token is stored in the properties of the VariantConstraint. It
         is a hash initialized with a value when the Dataset is protected.
 
         If a transform does not preserve the PEID then the token is set to None
         If a transform preserves the PEID assignment but changes the rows (e.g.
         sample, shuffle, filter,...) then the token's value is changed If a
         transform does not change the rows (e.g. selecting a column, adding a
         scalar,...) then the token is passed without change
 
-        A Dataspec is PEP if its PEP token is not None. Two PEP Dataspecs are
+        A Dataspec is PUP if its PUP token is not None. Two PUP Dataspecs are
         aligned (i.e. they have the same number of rows and all their rows have
         the same PEID) if their tokens are equal.
         """
         ...
 
-    def rewritten_pep_token(self) -> t.Optional[str]:
-        """Returns the PEP token for the DP variant of this dataspec
+    def rewritten_pup_token(self) -> t.Optional[str]:
+        """Returns the PUP token for the DP variant of this dataspec
         during DP rewriting.
 
-        Currently, the implementation assumes a single DP/PEP variant per
+        Currently, the implementation assumes a single DP/PUP variant per
         dataspec, resulting in one possible value for
-        "rewritten_pep_token."
+        "rewritten_pup_token."
         Future changes could introduce multiple variants, necessitating
         the implementation of priority rules.
         """
         ...
 
-    def is_public(self) -> bool:
-        ...
+    def is_public(self) -> bool: ...
 
     def is_synthetic(self) -> bool:
         """Is the dataspec synthetic."""
         ...
 
     def is_dp(self) -> bool:
         """Is the dataspec the result of a DP transform."""
         ...
 
     def is_dp_writable(self) -> bool:
         """Check if it exists a variant of this dataspec
         that utilizes the dp equivalent, and this variant is is_dp."""
         ...
 
-    def is_pep_writable(self) -> bool:
-        ...
+    def is_pup_writable(self) -> bool: ...
 
-    def is_publishable(self) -> bool:
-        ...
+    def is_publishable(self) -> bool: ...
 
     def is_published(self) -> bool:
         """Check if the dataspec is the result of a DP transform or another
         published dataspec.
         There is at least one parent that is DP.
         Such a dataspec has at least one private query in its computation
         graph."""
@@ -339,108 +309,85 @@
         """Check if the dataspec can be computed if it is big data."""
         ...
 
     def is_remote(self) -> bool:
         """Is the dataspec a remotely defined dataset."""
         ...
 
-    def sources(self, type_name: t.Optional[str]) -> t.Set[DataSpec]:
-        ...
+    def sources(self, type_name: t.Optional[str]) -> t.Set[DataSpec]: ...
 
-    def transform(self) -> Transform:
-        ...
+    def transform(self) -> Transform: ...
 
     def status(
         self, task_names: t.Optional[t.List[str]]
-    ) -> t.Optional[Status]:
-        ...
+    ) -> t.Optional[Status]: ...
 
-    def accept(self, visitor: Visitor) -> None:
-        ...
+    def accept(self, visitor: Visitor) -> None: ...
 
     def attribute(self, name: str) -> t.Optional[Attribute]:
         """Return the attribute with the given name or None if not found."""
         ...
 
     def attributes(self, name: str) -> t.List[Attribute]:
         """Return all the attributes with the given name."""
         ...
 
 
 class Dataset(DataSpec[sp.Dataset], t.Protocol):
-    def prototype(self) -> t.Type[sp.Dataset]:
-        ...
+    def prototype(self) -> t.Type[sp.Dataset]: ...
 
-    def is_synthetic(self) -> bool:
-        ...
+    def is_synthetic(self) -> bool: ...
 
-    def has_admin_columns(self) -> bool:
-        ...
+    def has_admin_columns(self) -> bool: ...
 
-    def is_protected(self) -> bool:
-        ...
+    def is_protected(self) -> bool: ...
 
-    def is_file(self) -> bool:
-        ...
+    def is_file(self) -> bool: ...
 
-    def schema(self) -> Schema:
-        ...
+    def schema(self) -> Schema: ...
 
-    async def async_schema(self) -> Schema:
-        ...
+    async def async_schema(self) -> Schema: ...
 
-    def size(self) -> t.Optional[Size]:
-        ...
+    def size(self) -> t.Optional[Size]: ...
 
-    def multiplicity(self) -> t.Optional[Multiplicity]:
-        ...
+    def multiplicity(self) -> t.Optional[Multiplicity]: ...
 
-    def bounds(self) -> t.Optional[Bounds]:
-        ...
+    def bounds(self) -> t.Optional[Bounds]: ...
 
-    def marginals(self) -> t.Optional[Marginals]:
-        ...
+    def marginals(self) -> t.Optional[Marginals]: ...
 
-    def to_arrow(self, batch_size: int = 10000) -> t.Iterator[pa.RecordBatch]:
-        ...
+    def to_arrow(
+        self, batch_size: int = 10000
+    ) -> t.Iterator[pa.RecordBatch]: ...
 
     async def async_to_arrow(
         self, batch_size: int = 10000
-    ) -> t.AsyncIterator[pa.RecordBatch]:
-        ...
+    ) -> t.AsyncIterator[pa.RecordBatch]: ...
 
-    def to_sql(self) -> None:
-        ...
+    def to_sql(self) -> None: ...
 
-    def spec(self) -> str:
-        ...
+    def spec(self) -> str: ...
 
-    def __iter__(self) -> t.Iterator[pa.RecordBatch]:
-        ...
+    def __iter__(self) -> t.Iterator[pa.RecordBatch]: ...
 
-    def to_pandas(self) -> pd.DataFrame:
-        ...
+    def to_pandas(self) -> pd.DataFrame: ...
 
-    async def async_to_pandas(self) -> pd.DataFrame:
-        ...
+    async def async_to_pandas(self) -> pd.DataFrame: ...
 
-    def to_tensorflow(self) -> tf.data.Dataset:
-        ...
+    def to_tensorflow(self) -> tf.data.Dataset: ...
 
-    async def async_to_tensorflow(self) -> tf.data.Dataset:
-        ...
+    async def async_to_tensorflow(self) -> tf.data.Dataset: ...
 
     async def async_to(
         self, kind: t.Type, drop_admin: bool = True
     ) -> DatasetCastable:
         """Casts a Dataset to a Python type passed as argument."""
         ...
 
-    def to(self, kind: t.Type, drop_admin: bool = True) -> DatasetCastable:
-        ...
+    def to(self, kind: t.Type, drop_admin: bool = True) -> DatasetCastable: ...
 
     def dot(self) -> str:
         """return a graphviz representation of the dataset"""
         ...
 
     def sql(
         self,
@@ -467,251 +414,202 @@
 
 
 class Scalar(DataSpec[sp.Scalar], t.Protocol):
     def prototype(self) -> t.Type[sp.Scalar]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def is_pretrained_model(self) -> bool:
-        ...
+    def is_pretrained_model(self) -> bool: ...
 
     def is_privacy_params(self) -> bool:
         """Is the scalar privacy parameters."""
 
     def is_random_seed(self) -> bool:
         """Is the scalar a random seed."""
 
     def is_synthetic_model(self) -> bool:
         """is the scalar a synthetic model"""
 
-    def value(self) -> DataSpecValue:
-        ...
+    def value(self) -> DataSpecValue: ...
 
-    async def async_value(self) -> DataSpecValue:
-        ...
+    async def async_value(self) -> DataSpecValue: ...
 
-    def spec(self) -> str:
-        ...
+    def spec(self) -> str: ...
 
 
 class Visitor(t.Protocol):
     """A visitor class for Dataset"""
 
-    def all(self, visited: DataSpec) -> None:
-        ...
+    def all(self, visited: DataSpec) -> None: ...
 
     def transformed(
         self,
         visited: DataSpec,
         transform: Transform,
         *arguments: DataSpec,
         **named_arguments: DataSpec,
-    ) -> None:
-        ...
+    ) -> None: ...
 
-    def other(self, visited: DataSpec) -> None:
-        ...
+    def other(self, visited: DataSpec) -> None: ...
 
 
 class Bounds(Referring[sp.Bounds], t.Protocol):
     """A python abstract class to describe bounds"""
 
     def prototype(self) -> t.Type[sp.Bounds]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def statistics(self) -> Statistics:
-        ...
+    def statistics(self) -> Statistics: ...
 
 
 class Marginals(Referring[sp.Marginals], t.Protocol):
     """A python abstract class to describe marginals"""
 
     def prototype(self) -> t.Type[sp.Marginals]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def statistics(self) -> Statistics:
-        ...
+    def statistics(self) -> Statistics: ...
 
 
 class Size(Referring[sp.Size], t.Protocol):
     """A python abstract class to describe size"""
 
     def prototype(self) -> t.Type[sp.Size]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def statistics(self) -> Statistics:
-        ...
+    def statistics(self) -> Statistics: ...
 
 
 class Multiplicity(Referring[sp.Multiplicity], t.Protocol):
     """A python abstract class to describe size"""
 
     def prototype(self) -> t.Type[sp.Multiplicity]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def statistics(self) -> Statistics:
-        ...
+    def statistics(self) -> Statistics: ...
 
 
 class Schema(Referring[sp.Schema], t.Protocol):
     """A python abstract class to describe schemas"""
 
     def prototype(self) -> t.Type[sp.Schema]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def to_arrow(self) -> pa.Schema:
-        ...
+    def to_arrow(self) -> pa.Schema: ...
 
-    def type(self) -> Type:
-        ...
+    def type(self) -> Type: ...
 
-    def has_admin_columns(self) -> bool:
-        ...
+    def has_admin_columns(self) -> bool: ...
 
-    def is_protected(self) -> bool:
-        ...
+    def is_privacy_unit_tracking(self) -> bool: ...
 
-    def tables(self) -> t.List[Path]:
-        ...
+    def tables(self) -> t.List[Path]: ...
 
-    def protected_path(self) -> Path:
-        ...
+    def privacy_unit_tracking_paths(self) -> Path: ...
 
-    def data_type(self) -> Type:
-        ...
+    def data_type(self) -> Type: ...
 
-    def private_tables(self) -> t.List[Path]:
-        ...
+    def private_tables(self) -> t.List[Path]: ...
 
-    def public_tables(self) -> t.List[Path]:
-        ...
+    def public_tables(self) -> t.List[Path]: ...
 
 
 class Status(Referring[sp.Status], t.Protocol):
     """A python abstract class to describe status"""
 
     def prototype(self) -> t.Type[sp.Status]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataspec(self) -> DataSpec:
-        ...
+    def dataspec(self) -> DataSpec: ...
 
-    def datetime(self) -> dt.datetime:
-        ...
+    def datetime(self) -> dt.datetime: ...
 
     def update(
         self,
         task_stages: t.Optional[t.Mapping[str, Stage]],
         properties: t.Optional[t.Mapping[str, str]],
-    ) -> t.Tuple[Status, bool]:
-        ...
+    ) -> t.Tuple[Status, bool]: ...
 
-    def task(self, task: str) -> t.Optional[Stage]:
-        ...
+    def task(self, task: str) -> t.Optional[Stage]: ...
 
-    def pending(self) -> bool:
-        ...
+    def pending(self) -> bool: ...
 
-    def processing(self) -> bool:
-        ...
+    def processing(self) -> bool: ...
 
-    def ready(self) -> bool:
-        ...
+    def ready(self) -> bool: ...
 
-    def error(self) -> bool:
-        ...
+    def error(self) -> bool: ...
 
     def owner(
         self,
-    ) -> (
-        manager_typing.Manager
-    ):  # TODO: Maybe find a better name, but this was shadowing the actual manager of this object.  # noqa: E501
+    ) -> manager_typing.Manager:  # TODO: Maybe find a better name, but this was shadowing the actual manager of this object.  # noqa: E501
         ...
 
     def clear_task(self, task: str) -> t.Tuple[Status, bool]:
         """Creates a new status removing the task specified.
         If the task does not exist, nothing is created"""
 
 
 class Stage(HasProtobuf[sp.Status.Stage], t.Protocol):
-    def accept(self, visitor: StageVisitor) -> None:
-        ...
+    def accept(self, visitor: StageVisitor) -> None: ...
 
-    def stage(self) -> str:
-        ...
+    def stage(self) -> str: ...
 
-    def ready(self) -> bool:
-        ...
+    def ready(self) -> bool: ...
 
-    def processing(self) -> bool:
-        ...
+    def processing(self) -> bool: ...
 
-    def pending(self) -> bool:
-        ...
+    def pending(self) -> bool: ...
 
-    def error(self) -> bool:
-        ...
+    def error(self) -> bool: ...
 
 
 class StageVisitor(t.Protocol):
     """A visitor class for Status/Stage"""
 
-    def pending(self) -> None:
-        ...
+    def pending(self) -> None: ...
 
-    def processing(self) -> None:
-        ...
+    def processing(self) -> None: ...
 
-    def ready(self) -> None:
-        ...
+    def ready(self) -> None: ...
 
-    def error(self) -> None:
-        ...
+    def error(self) -> None: ...
 
 
 @t.runtime_checkable
 class Transform(Referrable[sp.Transform], t.Protocol):
     """A python abstract class to describe transforms"""
 
     def prototype(self) -> t.Type[sp.Transform]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
-    def doc(self) -> str:
-        ...
+    def doc(self) -> str: ...
 
-    def spec(self) -> str:
-        ...
+    def spec(self) -> str: ...
 
     def is_composed(self) -> bool:
         """Is the transform composed."""
         ...
 
     def is_variable(self) -> bool:
         """Is the transform a variable."""
@@ -740,44 +638,39 @@
         """Return all the variables from a composed transform"""
         ...
 
     def compose(
         self,
         *compose_arguments: Transform,
         **compose_named_arguments: Transform,
-    ) -> Transform:
-        ...
+    ) -> Transform: ...
 
     def apply(
         self,
         *apply_arguments: DataSpec,
         **apply_named_arguments: DataSpec,
-    ) -> DataSpec:
-        ...
+    ) -> DataSpec: ...
 
     def abstract(
         self,
         *arguments: str,
         **named_arguments: str,
-    ) -> Transform:
-        ...
+    ) -> Transform: ...
 
     def __call__(
         self,
         *arguments: t.Union[Transform, DataSpec, int, str],
         **named_arguments: t.Union[Transform, DataSpec, int, str],
     ) -> t.Union[Transform, DataSpec]:
         """Applies the transform to another element"""
         ...
 
-    def __mul__(self, argument: Transform) -> Transform:
-        ...
+    def __mul__(self, argument: Transform) -> Transform: ...
 
-    def accept(self, visitor: TransformVisitor) -> None:
-        ...
+    def accept(self, visitor: TransformVisitor) -> None: ...
 
     def transform_to_apply(self) -> Transform:
         """Return the transform of a composed transform."""
 
     def composed_parents(
         self,
     ) -> t.Tuple[t.List[Transform], t.Dict[str, Transform]]:
@@ -789,51 +682,46 @@
         The function takes an undefined number of named arguments.
         """
 
 
 class TransformVisitor(t.Protocol):
     """A visitor class for Transform"""
 
-    def all(self, visited: Transform) -> None:
-        ...
+    def all(self, visited: Transform) -> None: ...
 
     def composed(
         self,
         visited: Transform,
         transform: Transform,
         *arguments: Transform,
         **named_arguments: Transform,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     def variable(
         self,
         visited: Transform,
         name: str,
         position: int,
-    ) -> None:
-        ...
+    ) -> None: ...
 
-    def other(self, visited: Transform) -> None:
-        ...
+    def other(self, visited: Transform) -> None: ...
 
 
 class Path(HasProtobuf[sp.Path], Frozen, Value, t.Protocol):
     """
     A python class to describe Paths
     A Path is essentially a tree of paths
     Each Path in the tree is a sequence of Labels
     """
 
     def prototype(self) -> t.Type[sp.Path]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def label(self) -> str:
-        ...
+    def label(self) -> str: ...
 
     def sub_paths(self) -> t.List[Path]:
         """Select within self the suffix paths that have
         select_path as their prefixes
         """
         ...
 
@@ -841,22 +729,19 @@
         """Tells if the path is empty (no label and no subpath)"""
         ...
 
     def has_sub_paths(self) -> bool:
         """Tells if the path has sub-paths"""
         ...
 
-    def select(self, select_path: Path) -> t.List[Path]:
-        ...
+    def select(self, select_path: Path) -> t.List[Path]: ...
 
-    def to_strings_list(self) -> t.List[t.List[str]]:
-        ...
+    def to_strings_list(self) -> t.List[t.List[str]]: ...
 
-    def to_dict(self) -> t.Dict[str, str]:
-        ...
+    def to_dict(self) -> t.Dict[str, str]: ...
 
 
 class Type(HasProtobuf[sp.Type], Frozen, Value, t.Protocol):
     def prototype(self) -> t.Type[sp.Type]:
         """Return the type of the underlying protobuf."""
         ...
 
@@ -867,15 +752,15 @@
     def data_type(self) -> Type:
         """Returns the first type level containing the data,
         hence skips the protected_entity struct if there is one"""
 
     def has_admin_columns(self) -> bool:
         """Return True if the Type has administrative columns."""
 
-    def has_protection(self) -> bool:
+    def has_privacy_unit_tracking(self) -> bool:
         """Return True if the Type has protection information."""
 
     def structs(self: Type) -> t.Optional[t.List[Path]]:
         """Returns the path to the first level structs encountered in the
         type.
         For example, Union[Struct1,Union[Struct2[Struct3]] will return only a
         path that brings to Struct1 and Struct2.
@@ -891,20 +776,18 @@
         ...
 
     def children(self) -> t.Dict[str, Type]:
         """Returns the children contained in the type tree structure"""
         ...
 
     # A Visitor acceptor
-    def accept(self, visitor: TypeVisitor) -> None:
-        ...
+    def accept(self, visitor: TypeVisitor) -> None: ...
 
     # A new Visitor acceptor
-    def accept_(self, visitor: TypeVisitor_[VisitedType]) -> VisitedType:
-        ...
+    def accept_(self, visitor: TypeVisitor_[VisitedType]) -> VisitedType: ...
 
     def sub_types(self: Type, item: Path) -> t.List[Type]:
         """Returns the terminal nodes contained in the path"""
         ...
 
     def default(self: Type) -> pa.Array:
         """Returns an example of arrow array matching the type.
@@ -988,19 +871,19 @@
     FLOAT64 = 0
     FLOAT32 = 1
     FLOAT16 = 2
 
 
 class ConstraintKind(Enum):
     SYNTHETIC = sp.ConstraintKind.SYNTHETIC
-    PEP = sp.ConstraintKind.PEP
+    PUP = sp.ConstraintKind.PUP
     DP = sp.ConstraintKind.DP
     PUBLIC = sp.ConstraintKind.PUBLIC
     MOCK = sp.ConstraintKind.MOCK
-    PEP_FOR_REWRITING = sp.ConstraintKind.PEP_FOR_REWRITING
+    PUP_FOR_REWRITING = sp.ConstraintKind.PUP_FOR_REWRITING
 
 
 class SQLDialect(Enum):
     """SQL Dialects"""
 
     POSTGRES = 1
     SQL_SERVER = 2
@@ -1023,375 +906,339 @@
     PARETO = "Pareto"
 
 
 class TypeVisitor(t.Protocol):
     """A visitor class for Type"""
 
     @abstractmethod
-    def Null(self, properties: t.Optional[t.Mapping[str, str]] = None) -> None:
-        ...
+    def Null(
+        self, properties: t.Optional[t.Mapping[str, str]] = None
+    ) -> None: ...
 
     @abstractmethod
-    def Unit(self, properties: t.Optional[t.Mapping[str, str]] = None) -> None:
-        ...
+    def Unit(
+        self, properties: t.Optional[t.Mapping[str, str]] = None
+    ) -> None: ...
 
     @abstractmethod
     def Boolean(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Id(
         self,
         unique: bool,
         reference: t.Optional[Path] = None,
         base: t.Optional[IdBase] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Integer(
         self,
         min: int,
         max: int,
         base: IntegerBase,
         possible_values: t.Iterable[int],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Enum(
         self,
         name: str,
         name_values: t.Sequence[t.Tuple[str, int]],
         ordered: bool,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Float(
         self,
         min: float,
         max: float,
         base: FloatBase,
         possible_values: t.Iterable[float],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Text(
         self,
         encoding: str,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Bytes(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Struct(
         self,
         fields: t.Mapping[str, Type],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Union(
         self,
         fields: t.Mapping[str, Type],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Optional(
         self,
         type: Type,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def List(
         self,
         type: Type,
         max_size: int,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Array(
         self,
         type: Type,
         shape: t.Tuple[int, ...],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Datetime(
         self,
         format: str,
         min: str,
         max: str,
         base: DatetimeBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Time(
         self,
         format: str,
         min: str,
         max: str,
         base: TimeBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Date(
         self,
         format: str,
         min: str,
         max: str,
         base: DateBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Duration(
         self,
         unit: str,
         min: int,
         max: int,
         possible_values: t.Iterable[int],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Constrained(
         self,
         type: Type,
         constraint: Predicate,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Hypothesis(
         self,
         *types: t.Tuple[Type, float],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
-VisitedType = t.TypeVar('VisitedType')
+VisitedType = t.TypeVar("VisitedType")
 
 
 class TypeVisitor_(t.Protocol, t.Generic[VisitedType]):
     """A visitor class for Type"""
 
     def default(self) -> VisitedType:
         """This is the minimal implementation to provide"""
         ...
 
     def Null(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Unit(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Boolean(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Id(
         self,
         unique: bool,
         reference: t.Optional[Path] = None,
         base: t.Optional[IdBase] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Integer(
         self,
         min: int,
         max: int,
         base: IntegerBase,
         possible_values: t.Iterable[int],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Enum(
         self,
         name: str,
         name_values: t.Sequence[t.Tuple[str, int]],
         ordered: bool,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Float(
         self,
         min: float,
         max: float,
         base: FloatBase,
         possible_values: t.Iterable[float],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Text(
         self,
         encoding: str,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Bytes(
         self, properties: t.Optional[t.Mapping[str, str]] = None
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Struct(
         self,
         fields: t.Mapping[str, VisitedType],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Union(
         self,
         fields: t.Mapping[str, VisitedType],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Optional(
         self,
         type_: VisitedType,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def List(
         self,
         type_: VisitedType,
         max_size: int,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Array(
         self,
         type_: VisitedType,
         shape: t.Tuple[int, ...],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Datetime(
         self,
         format: str,
         min: str,
         max: str,
         base: DatetimeBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Time(
         self,
         format: str,
         min: str,
         max: str,
         base: TimeBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Date(
         self,
         format: str,
         min: str,
         max: str,
         base: DateBase,
         possible_values: t.Iterable[str],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Duration(
         self,
         unit: str,
         min: int,
         max: int,
         possible_values: t.Iterable[int],
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Constrained(
         self,
         type_: VisitedType,
         constraint: Predicate,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
     def Hypothesis(
         self,
         *types: t.Tuple[VisitedType, float],
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> VisitedType:
-        ...
+    ) -> VisitedType: ...
 
 
 class Predicate(HasProtobuf[sp.Predicate], Frozen, Value, t.Protocol):
     """A python class to describe types"""
 
     def prototype(self) -> t.Type[sp.Predicate]:
         """Return the type of the underlying protobuf."""
@@ -1410,28 +1257,23 @@
 class Statistics(HasProtobuf[sp.Statistics], Frozen, Value, t.Protocol):
     """A python class to describe statistics"""
 
     def prototype(self) -> t.Type[sp.Statistics]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def name(self) -> str:
-        ...
+    def name(self) -> str: ...
 
-    def distribution(self) -> Distribution:
-        ...
+    def distribution(self) -> Distribution: ...
 
-    def size(self) -> int:
-        ...
+    def size(self) -> int: ...
 
-    def multiplicity(self) -> float:
-        ...
+    def multiplicity(self) -> float: ...
 
-    def accept(self, visitor: StatisticsVisitor) -> None:
-        ...
+    def accept(self, visitor: StatisticsVisitor) -> None: ...
 
     def nodes_statistics(self, path: Path) -> t.List[Statistics]:
         """Returns the List of each statistics corresponding at the leaves
         of path"""
         ...
 
     def children(self) -> t.Dict[str, Statistics]:
@@ -1442,217 +1284,193 @@
 class Distribution(HasProtobuf[sp.Distribution], Frozen, Value, t.Protocol):
     """A python class to describe distributions"""
 
     def prototype(self) -> t.Type[sp.Distribution]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def values(self) -> t.Union[t.List[float], t.List[int]]:
-        ...
+    def values(self) -> t.Union[t.List[float], t.List[int]]: ...
 
-    def probabilities(self) -> t.List[float]:
-        ...
+    def probabilities(self) -> t.List[float]: ...
 
-    def names(self) -> t.Union[t.List[bool], t.List[str]]:
-        ...
+    def names(self) -> t.Union[t.List[bool], t.List[str]]: ...
 
-    def min_value(self) -> t.Union[int, float]:
-        ...
+    def min_value(self) -> t.Union[int, float]: ...
 
-    def max_value(self) -> t.Union[int, float]:
-        ...
+    def max_value(self) -> t.Union[int, float]: ...
 
 
 class StatisticsVisitor(t.Protocol):
     """A visitor class for Statistics"""
 
     @abstractmethod
-    def Null(self, size: int, multiplicity: float) -> None:
-        ...
+    def Null(self, size: int, multiplicity: float) -> None: ...
 
     @abstractmethod
-    def Unit(self, size: int, multiplicity: float) -> None:
-        ...
+    def Unit(self, size: int, multiplicity: float) -> None: ...
 
     def Boolean(
         self,
         size: int,
         multiplicity: float,
         probabilities: t.Optional[t.List[float]] = None,
         names: t.Optional[t.List[bool]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
-    def Id(self, size: int, multiplicity: float) -> None:
-        ...
+    def Id(self, size: int, multiplicity: float) -> None: ...
 
     @abstractmethod
     def Integer(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Enum(
         self,
         size: int,
         multiplicity: float,
         probabilities: t.Optional[t.List[float]] = None,
         names: t.Optional[t.List[str]] = None,
         values: t.Optional[t.List[float]] = None,
-        name: str = 'Enum',
-    ) -> None:
-        ...
+        name: str = "Enum",
+    ) -> None: ...
 
     @abstractmethod
     def Float(
         self,
         size: int,
         multiplicity: float,
         min_value: float,
         max_value: float,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[float]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Text(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
-        example: str = '',
+        example: str = "",
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
-    def Bytes(self, size: int, multiplicity: float) -> None:
-        ...
+    def Bytes(self, size: int, multiplicity: float) -> None: ...
 
     @abstractmethod
     def Struct(
         self,
         fields: t.Mapping[str, Statistics],
         size: int,
         multiplicity: float,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Union(
         self,
         fields: t.Mapping[str, Statistics],
         size: int,
         multiplicity: float,
         name: t.Optional[str] = None,
         properties: t.Optional[t.Mapping[str, str]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Optional(
         self, statistics: Statistics, size: int, multiplicity: float
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def List(
         self,
         statistics: Statistics,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
-        name: str = 'List',
+        name: str = "List",
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Array(
         self,
         statistics: Statistics,
         size: int,
         multiplicity: float,
         min_values: t.Optional[t.List[float]] = None,
         max_values: t.Optional[t.List[float]] = None,
-        name: str = 'Array',
+        name: str = "Array",
         probabilities: t.Optional[t.List[t.List[float]]] = None,
         values: t.Optional[t.List[t.List[float]]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Datetime(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Date(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Time(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Duration(
         self,
         size: int,
         multiplicity: float,
         min_value: int,
         max_value: int,
         probabilities: t.Optional[t.List[float]] = None,
         values: t.Optional[t.List[int]] = None,
-    ) -> None:
-        ...
+    ) -> None: ...
 
     @abstractmethod
     def Constrained(
         self, statistics: Statistics, size: int, multiplicity: float
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 class InferredDistribution(t.Protocol):
     """A python class to to infer user input distribution
 
     Attributes:
         nparams: number of parameters
@@ -1687,30 +1505,28 @@
             if alphabet is [1,2,3] U [10] = [1,2,3,10] has complexity=2
     """
 
     charset: t.List[int]
     complexity: int
 
 
-T = t.TypeVar('T', covariant=True)
+T = t.TypeVar("T", covariant=True)
 
 
 class Links(Referring[sp.Links], t.Protocol):
     """A python abstract class to describe all
     the links statistics in a dataset"""
 
     def prototype(self) -> t.Type[sp.Links]:
         """Return the type of the underlying protobuf."""
         ...
 
-    def dataset(self) -> Dataset:
-        ...
+    def dataset(self) -> Dataset: ...
 
-    def links_statistics(self) -> t.List[LinkStatistics]:
-        ...
+    def links_statistics(self) -> t.List[LinkStatistics]: ...
 
 
 class LinkStatistics(HasProtobuf[sp.Links.LinkStat], t.Protocol):
     """A python class to describe the statistics of a link
     for a foreign key"""
 
     def prototype(self) -> t.Type[sp.Links.LinkStat]:
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec/variant_constraint.py` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec/variant_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import List, Optional, Type, cast
 import json
 
 from sarus_data_spec.base import Referring
 from sarus_data_spec.constants import (
     IS_PUBLIC,
     IS_SYNTHETIC,
-    PEP_TOKEN,
     PRIVACY_LIMIT,
+    PUP_TOKEN,
     SALT,
 )
 from sarus_data_spec.dataspec_validator.privacy_limit import DeltaEpsilonLimit
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 
 
@@ -86,49 +86,49 @@
             constraint_kind=sp.ConstraintKind.DP,
             required_context=required_context,
             properties=properties,
         )
     )
 
 
-def pep_constraint(
+def pup_constraint(
     dataspec: st.DataSpec,
     token: str,
     required_context: List[str],
     privacy_limit: st.PrivacyLimit,
 ) -> VariantConstraint:
-    """Create a variant constraint specifying a dataspec is PEP."""
+    """Create a variant constraint specifying a dataspec is PUP."""
     return VariantConstraint(
         sp.VariantConstraint(
             dataspec=dataspec.uuid(),
-            constraint_kind=sp.ConstraintKind.PEP,
+            constraint_kind=sp.ConstraintKind.PUP,
             required_context=required_context,
             properties={
                 PRIVACY_LIMIT: json.dumps(privacy_limit.delta_epsilon_dict()),
-                PEP_TOKEN: token,
+                PUP_TOKEN: token,
             },
         )
     )
 
 
-def pep_for_rewriting_constraint(
+def pup_for_rewriting_constraint(
     dataspec: st.DataSpec,
     token: str,
     required_context: List[str],
     privacy_limit: st.PrivacyLimit,
 ) -> VariantConstraint:
-    """Create a variant constraint specifying a dataspec is PEP."""
+    """Create a variant constraint specifying a dataspec is PUP."""
     return VariantConstraint(
         sp.VariantConstraint(
             dataspec=dataspec.uuid(),
-            constraint_kind=sp.ConstraintKind.PEP_FOR_REWRITING,
+            constraint_kind=sp.ConstraintKind.PUP_FOR_REWRITING,
             required_context=required_context,
             properties={
                 PRIVACY_LIMIT: json.dumps(privacy_limit.delta_epsilon_dict()),
-                PEP_TOKEN: token,
+                PUP_TOKEN: token,
             },
         )
     )
 
 
 def syn_constraint(
     dataspec: st.DataSpec,
```

### Comparing `sarus_data_spec_public-3.9.2.dev0/sarus_data_spec_public.egg-info/SOURCES.txt` & `sarus_data_spec_public-4.0.0.dev5/sarus_data_spec_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/setup.cfg` & `sarus_data_spec_public-4.0.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `sarus_data_spec_public-3.9.2.dev0/setup.py` & `sarus_data_spec_public-4.0.0.dev5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
     def run(self):
         generate_proto_code()
         build_py.run(self)
 
 
 if __name__ == "__main__":
-    setup(version="3.9.2.dev0")
+    setup(version="4.0.0.dev5")
```

