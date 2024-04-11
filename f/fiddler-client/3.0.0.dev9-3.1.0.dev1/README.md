# Comparing `tmp/fiddler-client-3.0.0.dev9.tar.gz` & `tmp/fiddler-client-3.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddler-client-3.0.0.dev9.tar", last modified: Tue Mar  5 11:53:54 2024, max compression
+gzip compressed data, was "fiddler-client-3.1.0.dev1.tar", last modified: Tue Apr  9 16:33:41 2024, max compression
```

## Comparing `fiddler-client-3.0.0.dev9.tar` & `fiddler-client-3.1.0.dev1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/
--rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/LICENSE.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    19978 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/PUBLIC.md
--rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/
--rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/VERSION
--rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/configs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5760 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/connection.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/constants/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      321 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/common.py
--rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/constants/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/decorators.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/entities/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11557 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8028 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6827 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4661 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4370 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16723 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5514 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3059 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20232 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/entities/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.292116 fiddler-client-3.0.0.dev9/fiddler/libs/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/http_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/libs/semver.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/packtools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/gem.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/keras_ig_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/project_attributions_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/packtools/template_model.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/schemas/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/base.py
--rw-r--r--   0 runner    (1001) runner    (1001)      923 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/custom_expression.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5382 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/custom_features.py
--rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/events.py
--rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/file.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/filter_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1361 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/model_task_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/organization.py
--rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/response.py
--rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/server_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/user.py
--rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/schemas/xai_params.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/tests/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/tests/apis/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_record.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_rule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7650 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_baseline.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8442 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4510 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_events.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_files.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4970 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_generate_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2453 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_mixin.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14652 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_artifact.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_deployment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_surrogate.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8038 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_segment.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_webhook.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28537 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_xai.py
--rw-r--r--   0 runner    (1001) runner    (1001)      857 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/conftest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_connection.py
--rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/test_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/tests/utils.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler/utils/
--rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/logger.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/model_generator.py
--rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/validations.py
--rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/utils/version.py
--rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/fiddler/version.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-03-05 11:53:54.000000 fiddler-client-3.0.0.dev9/fiddler_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-03-05 11:53:54.302116 fiddler-client-3.0.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-03-05 11:53:49.000000 fiddler-client-3.0.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/
+-rw-r--r--   0 runner    (1001) runner    (1001)      559 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       42 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    19978 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/PUBLIC.md
+-rw-r--r--   0 runner    (1001) runner    (1001)     2165 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/
+-rw-r--r--   0 runner    (1001) runner    (1001)       11 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/VERSION
+-rw-r--r--   0 runner    (1001) runner    (1001)     3757 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      217 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/configs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5677 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/connection.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/constants/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      400 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/common.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      126 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      114 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      233 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1706 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      278 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      214 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/constants/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1820 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/decorators.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/entities/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3564 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11569 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2106 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7907 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6568 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4399 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4291 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5220 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18503 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5520 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3769 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1074 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4631 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1243 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3798 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20250 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/entities/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2221 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/exceptions.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/libs/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6027 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/http_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      512 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15995 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/libs/semver.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.713794 fiddler-client-3.1.0.dev1/fiddler/packtools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4637 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/gem.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7941 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/keras_ig_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15799 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/project_attributions_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10467 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/packtools/template_model.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/schemas/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      668 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1222 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      189 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/base.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      933 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      844 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/custom_expression.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5382 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/custom_features.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      657 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      409 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      462 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/file.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1325 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/filter_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      354 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1378 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1128 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1914 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      642 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      691 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/model_task_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      281 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/organization.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      379 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1166 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      500 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/server_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      464 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      739 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      313 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/schemas/xai_params.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/tests/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/tests/apis/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3118 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_record.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11231 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_rule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7494 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_baseline.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8208 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4636 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5134 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_events.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4501 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_files.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5089 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_generate_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1891 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2453 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_mixin.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18346 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5635 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_artifact.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2441 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_deployment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4443 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_surrogate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6015 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7804 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_segment.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6440 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_webhook.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28590 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_xai.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      840 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/conftest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1865 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      783 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      312 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3333 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      335 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/tests/utils.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler/utils/
+-rw-r--r--   0 runner    (1001) runner    (1001)       53 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2908 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      669 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/logger.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2203 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/model_generator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      408 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/validations.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      531 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/utils/version.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      140 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/fiddler/version.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)    20672 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)     3321 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      137 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        8 2024-04-09 16:33:41.000000 fiddler-client-3.1.0.dev1/fiddler_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-09 16:33:41.733792 fiddler-client-3.1.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     1102 2024-04-09 16:33:36.000000 fiddler-client-3.1.0.dev1/setup.py
```

### Comparing `fiddler-client-3.0.0.dev9/LICENSE.txt` & `fiddler-client-3.1.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/PKG-INFO` & `fiddler-client-3.1.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.0.0.dev9
+Version: 3.1.0.dev1
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.0.0.dev9/PUBLIC.md` & `fiddler-client-3.1.0.dev1/PUBLIC.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/README.md` & `fiddler-client-3.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/__init__.py` & `fiddler-client-3.1.0.dev1/fiddler/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,38 @@
+from __future__ import annotations
+
 from fiddler.connection import Connection, ConnectionMixin, init  # noqa
 from fiddler.constants.alert_rule import (  # noqa
     AlertCondition,
     BinSize,
     CompareTo,
     Priority,
 )
-from fiddler.constants.baseline import BaselineType, WindowSize  # noqa
+from fiddler.constants.baseline import BaselineType, WindowBinSize  # noqa
 from fiddler.constants.dataset import EnvType  # noqa
 from fiddler.constants.job import JobStatus  # noqa
 from fiddler.constants.model import (  # noqa
     ArtifactStatus,
     CustomFeatureType,
     DataType,
     ModelInputType,
     ModelTask,
 )
 from fiddler.constants.model_deployment import ArtifactType, DeploymentType  # noqa
 from fiddler.constants.xai import ExplainMethod  # noqa
 from fiddler.entities.alert_record import AlertRecord  # noqa
 from fiddler.entities.alert_rule import AlertRule  # noqa
-from fiddler.entities.baseline import Baseline  # noqa
+from fiddler.entities.baseline import Baseline, BaselineCompact  # noqa
 from fiddler.entities.custom_expression import CustomMetric, Segment  # noqa
-from fiddler.entities.dataset import Dataset  # noqa
+from fiddler.entities.dataset import Dataset, DatasetCompact  # noqa
 from fiddler.entities.file import File  # noqa
 from fiddler.entities.job import Job  # noqa
-from fiddler.entities.model import Model  # noqa
+from fiddler.entities.model import Model, ModelCompact  # noqa
 from fiddler.entities.model_deployment import ModelDeployment  # noqa
-from fiddler.entities.project import Project  # noqa
+from fiddler.entities.project import Project, ProjectCompact  # noqa
 from fiddler.entities.webhook import Webhook  # noqa
 from fiddler.exceptions import (  # noqa
     ApiError,
     AsyncJobFailed,
     Conflict,
     ConnError,
     ConnTimeout,
@@ -58,19 +60,30 @@
     RowDataSource,
     SqlSliceQueryDataSource,
 )
 from fiddler.schemas.xai_params import XaiParams  # noqa
 from fiddler.utils.logger import set_logging  # noqa
 from fiddler.version import __version__  # noqa
 
+# Global connection object
+conn: Connection | None = None
+
+
+def set_conn(conn_: Connection) -> None:
+    """Set global conn variable"""
+    global conn
+    conn = conn_
+
+
 __all__ = [
     '__version__',
     'Connection',
     'ConnectionMixin',
     'init',
+    'conn',
     # Constants
     'AlertCondition',
     'ArtifactStatus',
     'ArtifactType',
     'BaselineType',
     'BinSize',
     'CompareTo',
@@ -78,15 +91,15 @@
     'DeploymentType',
     'EnvType',
     'ExplainMethod',
     'JobStatus',
     'ModelInputType',
     'ModelTask',
     'Priority',
-    'WindowSize',
+    'WindowBinSize',
     # Schemas
     'CustomFeature',
     'DatasetDataSource',
     'DeploymentParams',
     'Enrichment',
     'EventIdDataSource',
     'ImageEmbedding',
@@ -99,21 +112,25 @@
     'TextEmbedding',
     'VectorFeature',
     'XaiParams',
     # Entities
     'AlertRecord',
     'AlertRule',
     'Baseline',
+    'BaselineCompact',
     'Dataset',
+    'DatasetCompact',
     'CustomMetric',
     'File',
     'Job',
     'Model',
+    'ModelCompact',
     'ModelDeployment',
     'Project',
+    'ProjectCompact',
     'Segment',
     'Webhook',
     # Exceptions
     'NotFound',
     'Conflict',
     'IncompatibleClient',
     'AsyncJobFailed',
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/connection.py` & `fiddler-client-3.1.0.dev1/fiddler/connection.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 from fiddler.schemas.server_info import ServerInfo, Version
 from fiddler.utils.logger import get_logger
 from fiddler.utils.version import match_semver
 from fiddler.version import __version__
 
 logger = get_logger(__name__)
 
-# Global connection object
-connection: Connection | None = None
-
 
 class Connection:
     def __init__(  # pylint: disable=too-many-arguments
         self,
         url: str,
         token: str,
         proxies: dict | None = None,
@@ -119,43 +116,45 @@
             return
 
         raise IncompatibleClient(server_version=str(self.server_version))
 
 
 class ConnectionMixin:
     @classmethod
-    def _connection(cls) -> Connection:
+    def _conn(cls) -> Connection:
         """Fiddler connection instance"""
-        assert connection is not None
-        return connection
+        from fiddler import conn
+
+        assert conn is not None
+        return conn
 
     @classmethod
     def _client(cls) -> RequestClient:
         """Request client instance"""
-        return cls._connection().client
+        return cls._conn().client
 
     @property
     def organization_name(self) -> str:
         """Organization name property"""
-        return self._connection().server_info.organization.name
+        return self._conn().server_info.organization.name
 
     @property
     def organization_id(self) -> UUID:
         """Organization id property"""
-        return self._connection().server_info.organization.id
+        return self._conn().server_info.organization.id
 
     @classmethod
     def get_organization_name(cls) -> str:
         """Organization name"""
-        return cls._connection().server_info.organization.name
+        return cls._conn().server_info.organization.name
 
     @classmethod
     def get_organization_id(cls) -> UUID:
         """Organization id"""
-        return cls._connection().server_info.organization.id
+        return cls._conn().server_info.organization.id
 
 
 def init(  # pylint: disable=too-many-arguments
     url: str,
     token: str,
     proxies: dict | None = None,
     timeout: int = DEFAULT_CONNECTION_TIMEOUT,
@@ -169,16 +168,19 @@
     :param token: Authorization token
     :param proxies: Dictionary mapping protocol to the URL of the proxy
     :param timeout: Seconds to wait for the server to send data before giving up
     :param verify: Controls whether we verify the server’s TLS certificate
     :param validate: Whether to validate the server/client version compatibility.
          Some functionalities might not work if this is turned off.
     """
-    global connection  # pylint: disable=global-statement
-    connection = Connection(
+    from fiddler import set_conn
+
+    conn = Connection(
         url=url,
         token=token,
         proxies=proxies,
         timeout=timeout,
         verify=verify,
         validate=validate,
     )
+
+    set_conn(conn_=conn)
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/constants/alert_rule.py` & `fiddler-client-3.1.0.dev1/fiddler/constants/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/constants/model.py` & `fiddler-client-3.1.0.dev1/fiddler/constants/model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/decorators.py` & `fiddler-client-3.1.0.dev1/fiddler/decorators.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/alert_record.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/alert_rule.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/alert_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 class AlertRule(
     BaseEntity, ModelCompactMixin, ProjectCompactMixin, BaselineCompactMixin
 ):
     def __init__(  # pylint: disable=too-many-arguments
         self,
         name: str,
-        model_id: UUID,
+        model_id: UUID | str,
         metric_id: str | UUID,
         priority: Priority | str,
         compare_to: CompareTo | str,
         condition: AlertCondition | str,
         bin_size: BinSize | str,
         critical_threshold: float,
         warning_threshold: float | None = None,
         columns: list[str] | None = None,
-        baseline_id: UUID | None = None,
+        baseline_id: UUID | str | None = None,
         compare_bin_delta: int | None = None,
     ) -> None:
         """Construct a alert rule instance."""
         self.name = name
         self.model_id = model_id
         self.metric_id = metric_id
         self.columns = columns
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/base.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/base.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/baseline.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/baseline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Iterator
 from uuid import UUID
 
+from fiddler.constants.baseline import WindowBinSize
 from fiddler.constants.dataset import EnvType
 from fiddler.decorators import handle_api_error
 from fiddler.entities.base import BaseEntity
 from fiddler.entities.dataset import DatasetCompactMixin
 from fiddler.entities.model import ModelCompactMixin
 from fiddler.entities.project import ProjectCompactMixin
 from fiddler.schemas.baseline import BaselineResp
@@ -18,33 +19,33 @@
 
 class Baseline(
     BaseEntity, ModelCompactMixin, ProjectCompactMixin, DatasetCompactMixin
 ):  # pylint: disable=too-many-instance-attributes
     def __init__(  # pylint: disable=too-many-arguments
         self,
         name: str,
-        model_id: UUID,
+        model_id: UUID | str,
         environment: EnvType,
         type_: str,
-        dataset_id: UUID | None = None,
+        dataset_id: UUID | str | None = None,
         start_time: int | None = None,
         end_time: int | None = None,
-        offset: int | None = None,
-        window_size: int | None = None,
+        offset_delta: int | None = None,
+        window_bin_size: WindowBinSize | str | None = None,
     ) -> None:
         """Construct a baseline instance."""
         self.name = name
         self.model_id = model_id
         self.type = type_
         self.environment = environment
         self.dataset_id = dataset_id
         self.start_time = start_time
         self.end_time = end_time
-        self.offset = offset
-        self.window_size = window_size
+        self.offset_delta = offset_delta
+        self.window_bin_size = window_bin_size
 
         self.id: UUID | None = None
         self.row_count: int | None = None
         self.project_id: UUID | None = None
         self.created_at: datetime | None = None
         self.updated_at: datetime | None = None
 
@@ -69,16 +70,16 @@
             name=resp_obj.name,
             model_id=resp_obj.model.id,
             environment=resp_obj.dataset.type,
             dataset_id=resp_obj.dataset.id,
             type_=resp_obj.type,
             start_time=resp_obj.start_time,
             end_time=resp_obj.end_time,
-            offset=resp_obj.offset,
-            window_size=resp_obj.window_size,
+            offset_delta=resp_obj.offset_delta,
+            window_bin_size=resp_obj.window_bin_size,
         )
 
         # Add remaining fields
         fields = [
             'id',
             'created_at',
             'updated_at',
@@ -105,16 +106,16 @@
         # Add remaining fields
         fields = [
             'id',
             'name',
             'type',
             'start_time',
             'end_time',
-            'offset',
-            'window_size',
+            'offset_delta',
+            'window_bin_size',
             'created_at',
             'updated_at',
             'row_count',
         ]
         for field in fields:
             setattr(self, field, getattr(resp_obj, field, None))
 
@@ -130,35 +131,31 @@
         :return: baseline instance
         """
         response = cls._client().get(url=cls._get_url(id_=id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
-    def from_name(cls, name: str, model_name: str, project_name: str) -> Baseline:
+    def from_name(cls, name: str, model_id: UUID | str) -> Baseline:
         """
-        Get the baseline instance using baseline name, model name and project name.
+        Get the baseline instance of a model from baseline name
 
         :param name: Baseline name
-        :param model_name: Name of the model associated with the baseline
-        :param project_name: Name of the project associated with the baseline
+        :param model_id: Model identifier
 
-        :return: Baseline instance for the provided params
+        :return: Baseline instance
         """
 
         _filter = QueryCondition(
             rules=[
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name),
                 QueryRule(
-                    field='project_name',
+                    field='model_id',
                     operator=OperatorType.EQUAL,
-                    value=project_name,
-                ),
-                QueryRule(
-                    field='model_name', operator=OperatorType.EQUAL, value=model_name
+                    value=model_id,
                 ),
             ]
         )
 
         response = cls._client().get(
             url=cls._get_url(),
             params={'filter': _filter.json()},
@@ -199,29 +196,29 @@
         url = f'/v3/models/{model_id}/baselines'
         for baseline in cls._paginate(url=url, params=params):
             yield cls._from_dict(data=baseline)
 
     @handle_api_error
     def create(self) -> Baseline:
         """Create a new baseline."""
-        payload = {
+        payload: dict[str, Any] = {
             'name': self.name,
             'model_id': self.model_id,
             'type': self.type,
             'env_type': self.environment,
             'env_id': self.dataset_id,
         }
         if self.start_time:
             payload['start_time'] = self.start_time
         if self.end_time:
             payload['end_time'] = self.end_time
-        if self.offset:
-            payload['offset'] = self.offset
-        if self.window_size:
-            payload['window_size'] = self.window_size
+        if self.offset_delta:
+            payload['offset_delta'] = self.offset_delta
+        if self.window_bin_size:
+            payload['window_bin_size'] = self.window_bin_size
 
         response = self._client().post(
             url=self._get_url(),
             data=payload,
         )
         self._refresh_from_response(response=response)
         return self
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/custom_expression.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/custom_expression.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from fiddler.utils.helpers import raise_not_found
 
 
 class CustomExpression(BaseEntity, ModelCompactMixin, ProjectCompactMixin):
     def __init__(
         self,
         name: str,
-        model_id: UUID,
+        model_id: UUID | str,
         definition: str,
         description: str | None = None,
     ) -> None:
         """Construct a custom expression instance."""
         self.name = name
         self.model_id = model_id
         self.definition = definition
@@ -108,37 +108,29 @@
         :return: CustomMetric instance
         """
         response = cls._client().get(url=cls._get_url(id_=id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
-    def from_name(
-        cls, name: str, model_name: str, project_name: str
-    ) -> CustomExpression:
+    def from_name(cls, name: str, model_id: UUID | str) -> CustomExpression:
         """
-        Get the custom metric instance using custom metric name, model name and project name.
+        Get the custom metric instance of a model from custom metric name
 
         :param name: Custom metric name
-        :param model_name: Name of the model associated with the custom metric
-        :param project_name: Name of the project associated with the custom metric
+        :param model_id: Model identifier
 
         :return: CustomMetric instance for the provided params
         """
 
         _filter = QueryCondition(
             rules=[
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name),
                 QueryRule(
-                    field='model_name', operator=OperatorType.EQUAL, value=model_name
-                ),
-                QueryRule(
-                    field='project_name',
-                    operator=OperatorType.EQUAL,
-                    value=project_name,
+                    field='model_id', operator=OperatorType.EQUAL, value=model_id
                 ),
             ]
         )
         params: dict[str, Any] = {
             'filter': _filter.json(),
         }
 
@@ -153,15 +145,15 @@
 
         return cls._from_dict(data=response.json()['data']['items'][0])
 
     @classmethod
     @handle_api_error
     def list(
         cls,
-        model_id: UUID,
+        model_id: UUID | str,
     ) -> Iterator[CustomExpression]:
         """Get a list of all custom metrics in the organization."""
 
         url = f'/v3/models/{model_id}/{cls._get_url_path()}'
 
         for item in cls._paginate(url=url):
             yield cls._from_dict(data=item)
@@ -191,15 +183,19 @@
         assert self.id is not None
 
         self._client().delete(url=self._get_url(id_=self.id))
 
 
 class CustomMetric(CustomExpression):
     def __init__(
-        self, name: str, model_id: UUID, definition: str, description: str | None = None
+        self,
+        name: str,
+        model_id: UUID | str,
+        definition: str,
+        description: str | None = None,
     ) -> None:
         """Construct a custom metric instance."""
         super().__init__(name, model_id, definition, description)
 
         # Deserialized response object
         self._resp: CustomMetricResp | None = None
 
@@ -210,15 +206,19 @@
     @staticmethod
     def _get_display_name() -> str:
         return 'Custom metric'
 
 
 class Segment(CustomExpression):
     def __init__(
-        self, name: str, model_id: UUID, definition: str, description: str | None = None
+        self,
+        name: str,
+        model_id: UUID | str,
+        definition: str,
+        description: str | None = None,
     ) -> None:
         """Construct a segment instance."""
         super().__init__(name, model_id, definition, description)
 
         # Deserialized response object
         self._resp: SegmentResp | None = None
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/dataset.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,34 +68,30 @@
         :return: dataset instance
         """
         response = cls._client().get(url=cls._get_url(id_=id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
-    def from_name(cls, name: str, model_name: str, project_name: str) -> Dataset:
+    def from_name(cls, name: str, model_id: UUID | str) -> Dataset:
         """
         Get the dataset instance using dataset name.
 
         :param name: Dataset name
-        :param model_name: Name of the model associated with the dataset
-        :param project_name: name of the project associated with the dataset
+        :param model_id: Model identifier
 
         :return: Dataset instance for the provided params
         """
         _filter = QueryCondition(
             rules=[
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name),
                 QueryRule(
-                    field='project_name',
+                    field='model_id',
                     operator=OperatorType.EQUAL,
-                    value=project_name,
-                ),
-                QueryRule(
-                    field='model_name', operator=OperatorType.EQUAL, value=model_name
+                    value=model_id,
                 ),
             ]
         )
 
         response = cls._client().get(
             url=cls._get_url(),
             params={'filter': _filter.json()},
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/events.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/events.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
+import tempfile
 from pathlib import Path
-from typing import Any, Iterator
+from typing import Any
 from uuid import UUID
 
 import pandas as pd
 from requests import Response
+from tqdm import tqdm
 
 from fiddler.configs import STREAM_EVENT_LIMIT
 from fiddler.connection import ConnectionMixin
 from fiddler.decorators import handle_api_error
 from fiddler.entities.file import File
 from fiddler.entities.job import Job
 from fiddler.schemas.dataset import EnvType
@@ -24,72 +26,67 @@
         """
         Event publishing methods
 
         :param model_id: Model identifier
         """
         self.model_id = model_id
 
-    def _get_stream_chunks(
-        self, source: pd.DataFrame | list[dict[str, Any]]
-    ) -> Iterator[list[dict[str, Any]]]:
-        """Chunk the source based on stream limit"""
-
-        for i in range(0, len(source), self.STREAM_LIMIT):
-            chunk = source[i : i + self.STREAM_LIMIT]
-
-            if isinstance(chunk, pd.DataFrame):
-                events = chunk.to_dict('records')
-            else:
-                events = chunk
-
-            yield events
-
     @handle_api_error
     def publish(
         self,
         source: list[dict[str, Any]] | str | Path | pd.DataFrame,
         environment: EnvType = EnvType.PRODUCTION,
         dataset_name: str | None = None,
         update: bool = False,
     ) -> list[UUID] | Job:
         """
         Publish Pre-production or Production data
 
         :param source: one of:
             Path or str path: path for data file.
-            list[dict]: list of event dicts (max 1000) EnvType.PRE_PRODUCTION is not supported
-            dataframe: events dataframe. EnvType.PRE_PRODUCTION not supported.
+            dataframe: events dataframe.
+            list[dict]: list of event dicts EnvType.PRE_PRODUCTION is not supported
         :param environment: Either EnvType.PRE_PRODUCTION or EnvType.PRODUCTION
         :param dataset_name: Name of the dataset. Not supported for EnvType.PRODUCTION
         :param update: flag indicating if the events are updates to previously published rows
 
-        :return: list[UUID] for list of dicts or dataframe source and Job object for file path source.
+        :return: list[UUID] for list of dicts source and Job object for file path or dataframe source.
         """
         if isinstance(source, (str, Path)):
             return self._publish_file(
                 source=source,
                 environment=environment,
                 dataset_name=dataset_name,
                 update=update,
             )
 
-        if isinstance(source, (list, pd.DataFrame)):
+        if isinstance(source, pd.DataFrame):
+            with tempfile.NamedTemporaryFile(suffix='.csv') as temp_file:
+                source.to_csv(temp_file.name, index=False)
+                return self._publish_file(
+                    source=temp_file.name,
+                    environment=environment,
+                    dataset_name=dataset_name,
+                    update=update,
+                )
+
+        elif isinstance(source, list):
             return self._publish_stream(source=source, update=update)
 
         raise ValueError(f'Unsupported source - {type(source)}')
 
     def _publish_stream(
         self,
-        source: list[dict[str, Any]] | pd.DataFrame,
+        source: list[dict[str, Any]],
         update: bool = False,
     ) -> list[UUID]:
         event_ids = []
-        for events in self._get_stream_chunks(source=source):
+        for i in tqdm(range(0, len(source), self.STREAM_LIMIT)):
             response = self._publish_call(
-                source=EventsSource(events=events),
+                source=EventsSource(events=source[i : i + self.STREAM_LIMIT]),
                 environment=EnvType.PRODUCTION,
                 dataset_name=None,
                 update=update,
             )
             event_ids.extend(response.json()['data']['event_ids'])
 
         return event_ids
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/file.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/file.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/job.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/model.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import builtins
+import copy
 import typing
 from dataclasses import dataclass
 from datetime import datetime
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Iterator
 from uuid import UUID
@@ -45,28 +46,30 @@
     ProjectCompactMixin,
     UpdatedByMixin,
     XaiMixin,
 ):  # pylint: disable=too-many-ancestors
     def __init__(  # pylint: disable=too-many-arguments
         self,
         name: str,
-        project_id: UUID,
+        project_id: UUID | str,
         schema: ModelSchema,
         spec: ModelSpec,
+        version: str | None = None,
         input_type: str = ModelInputType.TABULAR,
         task: str = ModelTask.NOT_SET,
         task_params: ModelTaskParams | None = None,
         description: str | None = None,
         event_id_col: str | None = None,
         event_ts_col: str | None = None,
         event_ts_format: str | None = None,
         xai_params: XaiParams | None = None,
     ) -> None:
         """Construct a model instance"""
         self.name = name
+        self.version = version
         self.project_id = project_id
         self.schema = schema
         self.input_type = input_type
         self.task = task
         self.description = description
         self.event_id_col = event_id_col
         self.event_ts_col = event_ts_col
@@ -97,14 +100,15 @@
 
         # Deserialize the response
         resp_obj = ModelResp(**data)
 
         # Initialize
         instance = cls(
             name=resp_obj.name,
+            version=resp_obj.version,
             schema=resp_obj.schema_,
             spec=resp_obj.spec,
             project_id=resp_obj.project.id,
             input_type=resp_obj.input_type,
             task=resp_obj.task,
             task_params=resp_obj.task_params,
             description=resp_obj.description,
@@ -137,14 +141,15 @@
         # Reset fields
         self.schema = resp_obj.schema_
         self.project_id = resp_obj.project.id
 
         fields = [
             'id',
             'name',
+            'version',
             'spec',
             'input_type',
             'task',
             'task_params',
             'description',
             'event_id_col',
             'event_ts_col',
@@ -184,98 +189,148 @@
     def get(cls, id_: UUID | str) -> Model:
         """Get the model instance using model id."""
         response = cls._client().get(url=cls._get_url(id_))
         return cls._from_response(response=response)
 
     @classmethod
     @handle_api_error
-    def from_name(cls, name: str, project_name: str) -> Model:
-        """Get the model instance using model name and project name."""
+    def from_name(
+        cls,
+        name: str,
+        project_id: UUID | str,
+        version: str | None = None,
+        latest: bool = False,
+    ) -> Model:
+        """
+        Get the model instance from model name within a project.
+
+        :param name: Model name
+        :param project_id: Project identifier
+        :param version: Version name
+        :param latest: Whether to fetch the latest version of the model or first version
+        :return: Model instance
+        """
         _filter = QueryCondition(
             rules=[
                 QueryRule(field='name', operator=OperatorType.EQUAL, value=name),
                 QueryRule(
-                    field='project_name',
+                    field='project_id',
                     operator=OperatorType.EQUAL,
-                    value=project_name,
+                    value=project_id,
                 ),
             ]
         )
 
+        if version:
+            _filter.add_rule(
+                QueryRule(field='version', operator=OperatorType.EQUAL, value=version)
+            )
+
+        ordering = '-created_at' if latest else 'created_at'
         response = cls._client().get(
-            url=cls._get_url(), params={'filter': _filter.json()}
+            url=cls._get_url(),
+            params={'filter': _filter.json(), 'limit': 1, 'ordering': ordering},
         )
 
         if response.json()['data']['total'] == 0:
             raise_not_found('Model not found for the given identifier')
 
         return cls.get(id_=response.json()['data']['items'][0]['id'])
 
     @handle_api_error
     def create(self) -> Model:
         """Create a new model."""
+        payload = {
+            'name': self.name,
+            'project_id': str(self.project_id),
+            'schema': self.schema.dict(),
+            'spec': self.spec.dict(),
+            'input_type': self.input_type,
+            'task': self.task,
+            'task_params': self.task_params.dict(),
+            'description': self.description,
+            'event_id_col': self.event_id_col,
+            'event_ts_col': self.event_ts_col,
+            'event_ts_format': self.event_ts_format,
+            'xai_params': self.xai_params.dict(),
+        }
+
+        if self.version:
+            payload['version'] = self.version
+
         response = self._client().post(
             url=self._get_url(),
-            data={
-                'name': self.name,
-                'project_id': str(self.project_id),
-                'schema': self.schema.dict(),
-                'spec': self.spec.dict(),
-                'input_type': self.input_type,
-                'task': self.task,
-                'task_params': self.task_params.dict(),
-                'description': self.description,
-                'event_id_col': self.event_id_col,
-                'event_ts_col': self.event_ts_col,
-                'event_ts_format': self.event_ts_format,
-                'xai_params': self.xai_params.dict(),
-            },
+            data=payload,
         )
         self._refresh_from_response(response=response)
         return self
 
     @handle_api_error
     def update(self) -> None:
         """Update an existing model."""
         body: dict[str, Any] = {
+            'version': self.version,
             'xai_params': self.xai_params.dict(),
             'description': self.description,
             'event_id_col': self.event_id_col,
             'event_ts_col': self.event_ts_col,
             'event_ts_format': self.event_ts_format,
         }
 
         response = self._client().patch(url=self._get_url(id_=self.id), data=body)
         self._refresh_from_response(response=response)
 
     @classmethod
     @handle_api_error
     def list(
-        cls,
-        project_id: UUID,
+        cls, project_id: UUID | str, name: str | None = None
     ) -> Iterator[ModelCompact]:
         """
         Get a list of all models with the given filters
 
         :param project_id: Project identifier
+        :param name: Model name, use this for listing all the versions of a model
         :return: ModelCompact iterator
         """
         _filter = QueryCondition(
             rules=[
                 QueryRule(
                     field='project_id', operator=OperatorType.EQUAL, value=project_id
                 ),
             ]
         )
 
+        if name:
+            _filter.add_rule(
+                QueryRule(field='name', operator=OperatorType.EQUAL, value=name)
+            )
+
         params = {'filter': _filter.json()}
 
         for model in cls._paginate(url=cls._get_url(), params=params):
             yield ModelCompact(id=model['id'], name=model['name'])
 
+    def duplicate(self, version: str | None = None) -> Model:
+        """
+        Duplicate the model instance with the given version name.
+
+        This call will not save the model on server. After making changes to the model
+        instance call .create() to add the model version to Fiddler Platform.
+
+        :param version: Version name for the new instance
+        :return: Model instance
+        """
+        self_copy = copy.deepcopy(self)
+        self_copy.id = None
+
+        if version:
+            self_copy.version = version
+
+        return self_copy
+
     @property
     def datasets(self) -> Iterator[Dataset]:
         """Fetch all the datasets of this model"""
         from fiddler.entities.dataset import (  # pylint: disable=import-outside-toplevel
             Dataset,
         )
 
@@ -304,16 +359,17 @@
 
     @classmethod
     @handle_api_error
     def from_data(  # pylint: disable=too-many-arguments, too-many-locals
         cls,
         source: pd.DataFrame | Path | str,
         name: str,
-        project_id: UUID,
+        project_id: UUID | str,
         spec: ModelSpec | None = None,
+        version: str | None = None,
         input_type: str = ModelInputType.TABULAR,
         task: str = ModelTask.NOT_SET,
         task_params: ModelTaskParams | None = None,
         description: str | None = None,
         event_id_col: str | None = None,
         event_ts_col: str | None = None,
         event_ts_format: str | None = None,
@@ -324,14 +380,15 @@
         """
         Build model instance from the given dataframe
 
         :param source: Dataframe or a file to generate model instance
         :param name: Model name
         :param project_id: Project identifier
         :param spec: ModelSpec instance
+        :param version: Model version name
         :param input_type: Model input task type
         :param task: Model task like Regression, Binary classification etc.
         :param task_params: Parameters based on the task type
         :param description: A note or description of the model
         :param event_id_col: Column name in which event id will be sent
         :param event_ts_col: Column name in which event timestamp will be sent
         :param event_ts_format: Format of values in `event_ts_col` column
@@ -344,14 +401,15 @@
         resp_obj = ModelGenerator(
             source=source,
             spec=spec,
         ).generate(max_cardinality=max_cardinality, sample_size=sample_size)
 
         return Model(
             name=name,
+            version=version,
             schema=resp_obj.schema_,
             spec=resp_obj.spec,
             project_id=project_id,
             input_type=input_type,
             task=task,
             task_params=task_params,
             description=description,
@@ -448,15 +506,15 @@
         :param output_dir: Path to download model artifact tar file
         """
 
         self._artifact.download(output_dir=output_dir)
 
     def add_surrogate(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
     ) -> Job:
         """
         Add a new surrogate model
 
         :param dataset_id: Dataset to be used for generating surrogate model
         :param deployment_params: Model deployment parameters
@@ -466,15 +524,15 @@
             dataset_id=dataset_id, deployment_params=deployment_params
         )
         return job
 
     @handle_api_error
     def update_surrogate(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
     ) -> Job:
         """
         Update an existing surrogate model
 
         :param dataset_id: Dataset to be used for generating surrogate model
         :param deployment_params: Model deployment parameters
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/model_artifact.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/model_artifact.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             job.id,
         )
 
         return job
 
     def _artifact_deploy(
         self,
-        file_id: UUID,
+        file_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
         update: bool = False,
     ) -> Job:
         """Artifact deploy base method."""
         http_method = self._get_http_method(update)
         payload = {
             'file_id': file_id,
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/model_deployment.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/model_deployment.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class ModelDeployment(
     BaseEntity, ProjectCompactMixin
 ):  # pylint: disable=too-many-instance-attributes
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        model_id: UUID,
+        model_id: UUID | str,
     ) -> None:
         """Construct a model deployment instance."""
         self.id: UUID | None = None  # pylint: disable=invalid-name
         self.model_id = model_id
         self.artifact_type: str | None = None
         self.deployment_type: str | None = None
         self.active: bool | None = None
@@ -106,15 +106,15 @@
 
         response = self._client().patch(
             url=self._get_url(model_id=self.model_id), data=payload
         )
         self._refresh_from_response(response=response)
 
     @classmethod
-    def of(cls, model_id: UUID) -> ModelDeployment:
+    def of(cls, model_id: UUID | str) -> ModelDeployment:
         """
         Get model deployment instance of the given model
 
         :param model_id: Model identifier
         :return: ModelDeployment instance
         """
         response = cls._client().get(url=cls._get_url(model_id=model_id))
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/organization.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/organization.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/project.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/surrogate.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/surrogate.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         :param model_id: Model identifier
         """
         self.model_id = model_id
 
     def _deploy(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
         update: bool = False,
     ) -> Job:
         """
         Deploy surrogate model to an existing model
 
         :param dataset_id: Dataset to be used for generating surrogate model
@@ -67,15 +67,15 @@
         )
 
         return Job.get(id_=job_compact.id)
 
     @handle_api_error
     def add(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
     ) -> Job:
         """
         Add a new surrogate.
 
         :param dataset_id: Dataset to be used for generating surrogate model
         :param deployment_params: Model deployment parameters
@@ -85,15 +85,15 @@
             dataset_id=dataset_id, deployment_params=deployment_params, update=False
         )
         return job
 
     @handle_api_error
     def update(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         deployment_params: DeploymentParams | None = None,
     ) -> Job:
         """
         Update an existing surrogate.
 
         :param dataset_id: Dataset to be used for generating surrogate model
         :param deployment_params: Model deployment parameters
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/user.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/user.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/webhook.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/entities/xai.py` & `fiddler-client-3.1.0.dev1/fiddler/entities/xai.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         return namedtuple('FeatureImportance', response.json()['data'])(
             **response.json()['data']
         )
 
     @handle_api_error
     def precompute_feature_impact(  # pylint: disable=too-many-arguments
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         num_samples: int | None = None,
         num_iterations: int | None = None,
         num_refs: int | None = None,
         ci_level: float | None = None,
         min_support: int | None = None,
         update: bool = False,
     ) -> Job:
@@ -440,15 +440,15 @@
             job_compact.id,
         )
         return Job.get(id_=job_compact.id)
 
     @handle_api_error
     def precompute_feature_importance(  # pylint: disable=too-many-arguments
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         num_samples: int | None = None,
         num_iterations: int | None = None,
         num_refs: int | None = None,
         ci_level: float | None = None,
         update: bool = False,
     ) -> Job:
         """Pre-compute feature importance for a model on a dataset.
@@ -524,15 +524,15 @@
         return namedtuple('FeatureImpact', response.json()['data'])(
             **response.json()['data']
         )
 
     @handle_api_error
     def precompute_predictions(
         self,
-        dataset_id: UUID,
+        dataset_id: UUID | str,
         chunk_size: int | None = None,
         update: bool = False,
     ) -> Job:
         """
         Pre-compute predictions for a model on a dataset
 
         :param dataset_id: The unique identifier of the dataset
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/exceptions.py` & `fiddler-client-3.1.0.dev1/fiddler/exceptions.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/libs/http_client.py` & `fiddler-client-3.1.0.dev1/fiddler/libs/http_client.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/libs/json_encoder.py` & `fiddler-client-3.1.0.dev1/fiddler/libs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/libs/semver.py` & `fiddler-client-3.1.0.dev1/fiddler/libs/semver.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/packtools/gem.py` & `fiddler-client-3.1.0.dev1/fiddler/packtools/gem.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/packtools/keras_ig_helpers.py` & `fiddler-client-3.1.0.dev1/fiddler/packtools/keras_ig_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/packtools/project_attributions_helpers.py` & `fiddler-client-3.1.0.dev1/fiddler/packtools/project_attributions_helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/packtools/template_model.py` & `fiddler-client-3.1.0.dev1/fiddler/packtools/template_model.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/alert_record.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/alert_rule.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/baseline.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     """Baseline response pydantic model."""
 
     id: UUID
     name: str
     type: str
     start_time: Optional[int]
     end_time: Optional[int]
-    offset: Optional[int]
-    window_size: Optional[int]
+    offset_delta: Optional[int]
+    window_bin_size: Optional[str]
     row_count: Optional[int]
 
     model: ModelCompactResp
     project: ProjectCompactResp
     organization: OrganizationCompactResp
     dataset: DatasetCompactResp = Field(alias='environment')
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/custom_expression.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/custom_expression.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/custom_features.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/custom_features.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/dataset.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/dataset.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/filter_query.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/filter_query.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/model.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     id: UUID
     name: str
 
 
 class ModelResp(BaseModel):
     id: UUID
     name: str
+    version: str
     input_type: str
     task: str
     task_params: ModelTaskParams
     schema_: ModelSchema = Field(alias='schema')
     spec: ModelSpec
     description: Optional[str]
     event_id_col: Optional[str]
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/model_deployment.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/model_schema.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/model_schema.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/model_spec.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/model_spec.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/model_task_params.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/model_task_params.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/response.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/response.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/schemas/xai.py` & `fiddler-client-3.1.0.dev1/fiddler/schemas/xai.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_record.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_record.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_alert_rule.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_alert_rule.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_baseline.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_baseline.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 API_RESPONSE_200 = {
     'data': {
         'id': BASELINE_ID,
         'name': BASELINE_NAME,
         'type': 'STATIC',
         'start_time': None,
         'end_time': None,
-        'offset': None,
-        'window_size': None,
+        'offset_delta': None,
+        'window_bin_size': None,
         'row_count': 20000,
         'model': {
             'id': MODEL_ID,
             'name': MODEL_NAME,
         },
         'project': {'id': PROJECT_ID, 'name': PROJECT_NAME},
         'organization': {
@@ -76,16 +76,16 @@
             API_RESPONSE_200['data'],
             {
                 'id': 'af05646f-0cef-4638-84c9-0d195df2575f',
                 'name': 'test_baseline_2',
                 'type': 'STATIC',
                 'start_time': None,
                 'end_time': None,
-                'offset': None,
-                'window_size': None,
+                'offset_delta': None,
+                'window_bin_size': None,
                 'row_count': 20000,
                 'model': {
                     'id': MODEL_ID,
                     'name': MODEL_NAME,
                 },
                 'project': {'id': PROJECT_ID, 'name': PROJECT_NAME},
                 'organization': {
@@ -156,51 +156,49 @@
     with pytest.raises(NotFound):
         Baseline.get(id_=BASELINE_ID)
 
 
 @responses.activate
 def test_baseline_from_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_baseline"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_baseline"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
 
     responses.get(
         url=f'{URL}/v3/baselines',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
     baseline = Baseline.from_name(
         name=BASELINE_NAME,
-        model_name=MODEL_NAME,
-        project_name=PROJECT_NAME,
+        model_id=MODEL_ID,
     )
     assert isinstance(baseline, Baseline)
 
 
 @responses.activate
 def test_baseline_from_name_not_found() -> None:
     resp = API_RESPONSE_FROM_NAME.copy()
     resp['data']['total'] = 0
     resp['data']['item_count'] = 0
     resp['data']['items'] = []
 
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_baseline"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "test_baseline"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
 
     responses.get(
         url=f'{URL}/v3/baselines',
         json=resp,
         match=[matchers.query_param_matcher(params)],
     )
     with pytest.raises(NotFound):
         Baseline.from_name(
             name=BASELINE_NAME,
-            model_name=MODEL_NAME,
-            project_name=PROJECT_NAME,
+            model_id=MODEL_ID,
         )
 
 
 @responses.activate
 def test_baseline_list_success() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}/baselines',
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_custom_metric.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_custom_metric.py`

 * *Files 7% similar despite different names*

```diff
@@ -183,46 +183,38 @@
     with pytest.raises(NotFound):
         CustomMetric.get(id_=CUSTOM_METRIC_ID)
 
 
 @responses.activate
 def test_from_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
 
     responses.get(
         url=f'{URL}/v3/custom-metrics',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
-    custom_metric = CustomMetric.from_name(
-        name=CUSTOM_METRIC_NAME,
-        model_name=MODEL_NAME,
-        project_name=PROJECT_NAME,
-    )
+    custom_metric = CustomMetric.from_name(name=CUSTOM_METRIC_NAME, model_id=MODEL_ID)
     assert isinstance(custom_metric, CustomMetric)
 
 
 @responses.activate
 def test_from_name_not_found() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "xyzabc"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
     responses.get(
         url=f'{URL}/v3/custom-metrics',
         json=EMPTY_LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     with pytest.raises(NotFound):
-        CustomMetric.from_name(
-            name=CUSTOM_METRIC_NAME,
-            model_name=MODEL_NAME,
-            project_name=PROJECT_NAME,
-        )
+        CustomMetric.from_name(name=CUSTOM_METRIC_NAME, model_id=MODEL_ID)
 
 
 @responses.activate
 def test_custom_metric_list_empty() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}/custom-metrics',
         json=EMPTY_LIST_API_RESPONSE,
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_dataset.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,49 +107,44 @@
     with pytest.raises(NotFound):
         Dataset.get(id_=DATASET_ID)
 
 
 @responses.activate
 def test_dataset_from_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "dataset3"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "dataset3"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
     responses.get(
         url=f'{URL}/v3/environments',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
-    dataset = Dataset.from_name(
-        name=DATASET_NAME,
-        model_name=MODEL_NAME,
-        project_name=PROJECT_NAME,
-    )
+    dataset = Dataset.from_name(name=DATASET_NAME, model_id=MODEL_ID)
     assert isinstance(dataset, Dataset)
 
 
 @responses.activate
 def test_dataset_from_name_not_found() -> None:
     resp = API_RESPONSE_FROM_NAME.copy()
     resp['data']['total'] = 0
     resp['data']['item_count'] = 0
     resp['data']['items'] = []
 
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "dataset3"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "dataset3"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
     responses.get(
         url=f'{URL}/v3/environments',
         json=resp,
         match=[matchers.query_param_matcher(params)],
     )
     with pytest.raises(NotFound):
         Dataset.from_name(
             name=DATASET_NAME,
-            model_name=MODEL_NAME,
-            project_name=PROJECT_NAME,
+            model_id=MODEL_ID,
         )
 
 
 @responses.activate
 def test_dataset_list_success() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}/environments',
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_events.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_events.py`

 * *Files 16% similar despite different names*

```diff
@@ -96,60 +96,82 @@
         source=FILE_PATH, environment=EnvType.PRODUCTION, dataset_name='dataset_2'
     )
 
     assert isinstance(publish_response, Job)
 
 
 @responses.activate
-def test_publish_stream() -> None:
+def test_publish_df() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}',
         json=MODEL_API_RESPONSE_200,
     )
     model = Model.get(id_=MODEL_ID)
 
     responses.post(
+        url=f'{URL}/v3/files/upload',
+        json=SINGLE_UPLOAD_200_RESPONSE,
+    )
+    responses.get(
+        url=f'{URL}/v3/jobs/{JOB_ID}',
+        json=PUBLISH_JOB_RESPONSE,
+    )
+
+    responses.post(
         url=f'{URL}/v3/events',
-        json=STREAM_PUBLISH_202_API_RESPONSE,
+        json=FILE_PUBLISH_202_API_RESPONSE,
     )
     publish_response = model.publish(
-        source=df,
-        environment=EnvType.PRODUCTION,
+        source=df, environment=EnvType.PRE_PRODUCTION, dataset_name='dataset_1'
     )
 
-    assert isinstance(publish_response, list)
-    assert len(publish_response) == df.shape[0]
+    assert isinstance(publish_response, Job)
+
+    FILE_PUBLISH_202_API_RESPONSE['data']['job']['name'] = 'Publish events'
 
     publish_response = model.publish(
-        source=df.to_dict('records'),
+        source=df,
         environment=EnvType.PRODUCTION,
     )
 
-    assert isinstance(publish_response, list)
-    assert len(publish_response) == df.shape[0]
+    assert isinstance(publish_response, Job)
+
+    FILE_PUBLISH_202_API_RESPONSE['data']['job']['name'] = 'Publish events'
 
 
 @responses.activate
-def test_publish_update() -> None:
+def test_publish_stream() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}',
         json=MODEL_API_RESPONSE_200,
     )
     model = Model.get(id_=MODEL_ID)
 
-    responses.patch(
+    responses.post(
         url=f'{URL}/v3/events',
         json=STREAM_PUBLISH_202_API_RESPONSE,
     )
+
     publish_response = model.publish(
-        source=df, environment=EnvType.PRODUCTION, update=True
+        source=df.to_dict('records'),
+        environment=EnvType.PRODUCTION,
     )
+
     assert isinstance(publish_response, list)
     assert len(publish_response) == df.shape[0]
 
+
+@responses.activate
+def test_publish_update() -> None:
+    responses.get(
+        url=f'{URL}/v3/models/{MODEL_ID}',
+        json=MODEL_API_RESPONSE_200,
+    )
+    model = Model.get(id_=MODEL_ID)
+
     responses.post(
         url=f'{URL}/v3/files/upload',
         json=SINGLE_UPLOAD_200_RESPONSE,
     )
     responses.get(
         url=f'{URL}/v3/jobs/{JOB_ID}',
         json=PUBLISH_JOB_RESPONSE,
@@ -163,7 +185,12 @@
         source=FILE_PATH,
         environment=EnvType.PRODUCTION,
         dataset_name='dataset_1',
         update=True,
     )
 
     assert isinstance(publish_response, Job)
+
+    publish_response = model.publish(
+        source=df, environment=EnvType.PRODUCTION, update=True
+    )
+    assert isinstance(publish_response, Job)
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_files.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_files.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_generate_model.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_generate_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,11 +178,16 @@
         responses.post(
             url=f'{URL}/v3/model-factory',
             json=API_RESPONSE_200,
         )
 
         DF.to_csv(temp_file.name, index=False)
 
+        version = 'v1.0'
         model = Model.from_data(
-            source=temp_file.name, name='model1', project_id=PROJECT_ID
+            source=temp_file.name,
+            name='model1',
+            version=version,
+            project_id=PROJECT_ID,
         )
         assert isinstance(model, Model)
+        assert model.version == version
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_job.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_job.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_mixin.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from fiddler.schemas.model_spec import ModelSpec
 from fiddler.tests.constants import (
     JOB_ID,
     JOB_NAME,
     MODEL_DEPLOYMENT_ID,
     MODEL_ID,
     MODEL_NAME,
+    MODEL_VERSION,
     ORG_ID,
     ORG_NAME,
     PROJECT_ID,
     PROJECT_NAME,
     URL,
     USER_EMAIL,
     USER_ID,
@@ -149,14 +150,15 @@
     'schema_version': 1,
     'targets': ['Churned'],
 }
 API_RESPONSE_200 = {
     'data': {
         'id': MODEL_ID,
         'name': MODEL_NAME,
+        'version': MODEL_VERSION,
         'project': {
             'id': PROJECT_ID,
             'name': PROJECT_NAME,
         },
         'organization': {
             'id': ORG_ID,
             'name': ORG_NAME,
@@ -304,14 +306,15 @@
         schema=ModelSchema(**MODEL_SCHEMA),
         spec=ModelSpec(**MODEL_SPEC),
     ).create()
 
     assert isinstance(model, Model)
     assert model.id == UUID(MODEL_ID)
     assert model.name == MODEL_NAME
+    assert model.version == MODEL_VERSION
 
 
 @responses.activate
 def test_add_model_conflict() -> None:
     responses.post(
         url=f'{URL}/v3/models', json=API_RESPONSE_409, status=HTTPStatus.CONFLICT
     )
@@ -346,75 +349,147 @@
     with pytest.raises(NotFound):
         Model.get(id_=MODEL_ID)
 
 
 @responses.activate
 def test_model_from_name_success() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'limit': 1,
+        'ordering': 'created_at',
     }
     responses.get(
         url=f'{URL}/v3/models',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}',
         json=API_RESPONSE_200,
     )
-    model = Model.from_name(name=MODEL_NAME, project_name=PROJECT_NAME)
+    model = Model.from_name(name=MODEL_NAME, project_id=PROJECT_ID)
+    assert isinstance(model, Model)
+
+
+@responses.activate
+def test_model_from_name_with_version_success() -> None:
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}, {"field": "version", "operator": "equal", "value": "v1"}]}',
+        'limit': 1,
+        'ordering': 'created_at',
+    }
+    responses.get(
+        url=f'{URL}/v3/models',
+        json=API_RESPONSE_FROM_NAME,
+        match=[matchers.query_param_matcher(params)],
+    )
+    responses.get(
+        url=f'{URL}/v3/models/{MODEL_ID}',
+        json=API_RESPONSE_200,
+    )
+    model = Model.from_name(
+        name=MODEL_NAME, version=MODEL_VERSION, project_id=PROJECT_ID
+    )
+    assert isinstance(model, Model)
+
+
+@responses.activate
+def test_model_from_name_latest_success() -> None:
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'limit': 1,
+        'ordering': '-created_at',
+    }
+    responses.get(
+        url=f'{URL}/v3/models',
+        json=API_RESPONSE_FROM_NAME,
+        match=[matchers.query_param_matcher(params)],
+    )
+    responses.get(
+        url=f'{URL}/v3/models/{MODEL_ID}',
+        json=API_RESPONSE_200,
+    )
+    model = Model.from_name(name=MODEL_NAME, project_id=PROJECT_ID, latest=True)
     assert isinstance(model, Model)
 
 
 @responses.activate
 def test_model_from_name_not_found() -> None:
     resp = API_RESPONSE_FROM_NAME.copy()
     resp['data']['total'] = 0
     resp['data']['item_count'] = 0
     resp['data']['items'] = []
 
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'limit': 1,
+        'ordering': 'created_at',
+    }
+    responses.get(
+        url=f'{URL}/v3/models',
+        json=resp,
+        match=[matchers.query_param_matcher(params)],
+    )
+
+    with pytest.raises(NotFound):
+        Model.from_name(name=MODEL_NAME, project_id=PROJECT_ID)
+
+
+@responses.activate
+def test_model_from_name_with_version_not_found() -> None:
+    resp = API_RESPONSE_FROM_NAME.copy()
+    resp['data']['total'] = 0
+    resp['data']['item_count'] = 0
+    resp['data']['items'] = []
+
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "bank_churn"}, {"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}, {"field": "version", "operator": "equal", "value": "v1"}]}',
+        'limit': 1,
+        'ordering': 'created_at',
     }
     responses.get(
         url=f'{URL}/v3/models',
         json=resp,
         match=[matchers.query_param_matcher(params)],
     )
 
     with pytest.raises(NotFound):
-        Model.from_name(name=MODEL_NAME, project_name=PROJECT_NAME)
+        Model.from_name(name=MODEL_NAME, version=MODEL_VERSION, project_id=PROJECT_ID)
 
 
 @responses.activate
 def test_model_list_success() -> None:
-    params = {'project_id': str(PROJECT_ID), 'limit': 50, 'offset': 0}
+    params = {
+        'filter': '{"condition": "AND", "rules": [{"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'limit': 50,
+        'offset': 0,
+    }
     responses.get(
         url=f'{URL}/v3/models',
         json=LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     models = Model.list(project_id=PROJECT_ID)
     for model in models:
         assert isinstance(model, ModelCompact)
 
 
 @responses.activate
-def test_model_list_success() -> None:
+def test_model_list_with_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}]}',
+        'filter': '{"condition": "AND", "rules": [{"field": "project_id", "operator": "equal", "value": "1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1"}, {"field": "name", "operator": "equal", "value": "bank_churn"}]}',
         'limit': 50,
         'offset': 0,
     }
     responses.get(
         url=f'{URL}/v3/models',
         json=LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
-    models = Model.list(project_id=PROJECT_ID)
+    models = Model.list(project_id=PROJECT_ID, name=MODEL_NAME)
     for model in models:
         assert isinstance(model, ModelCompact)
 
 
 @responses.activate
 def test_delete_model() -> None:
     responses.get(
@@ -467,14 +542,26 @@
         json=API_RESPONSE_200,
     )
     model.description = 'Test model update'
 
     model.update()
     assert model.description == 'Test model update'
 
+    # update version
+    new_version = 'v2'
+    mocker.patch.dict(API_RESPONSE_200['data'], {'version': new_version})
+
+    responses.patch(
+        url=f'{URL}/v3/models/{MODEL_ID}',
+        json=API_RESPONSE_200,
+    )
+    model.version = new_version
+    model.update()
+    assert model.version == new_version
+
 
 @responses.activate
 def test_update_model_not_found() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}',
         json=API_RESPONSE_200,
     )
@@ -552,7 +639,29 @@
     # Delete method - success
     del schema['CreditScoreNew']
     assert schema.columns[0] != 'CreditScoreNew'
 
     # Delete method - KeyError
     with pytest.raises(KeyError):
         del schema['foo']
+
+
+@responses.activate
+def test_model_duplicate() -> None:
+    responses.get(
+        url=f'{URL}/v3/models/{MODEL_ID}',
+        json=API_RESPONSE_200,
+    )
+    model = Model.get(id_=MODEL_ID)
+
+    assert model.id == UUID(MODEL_ID)
+
+    # Without version parameter
+    model_copy = model.duplicate()
+    assert model_copy.id is None
+    assert model_copy.version == model.version
+
+    # With version parameter
+    new_version = 'v2'
+    model_copy = model.duplicate(version=new_version)
+    assert model_copy.id is None
+    assert model_copy.version == new_version
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_artifact.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_artifact.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_deployment.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_deployment.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_model_surrogate.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_model_surrogate.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_project.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_project.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_segment.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_segment.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,46 +183,38 @@
     with pytest.raises(NotFound):
         Segment.get(id_=SEGMENT_ID)
 
 
 @responses.activate
 def test_segment_from_name() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "age < 50"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "age < 50"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
 
     responses.get(
         url=f'{URL}/v3/segments',
         json=API_RESPONSE_FROM_NAME,
         match=[matchers.query_param_matcher(params)],
     )
-    segment = Segment.from_name(
-        name=SEGMENT_NAME,
-        model_name=MODEL_NAME,
-        project_name=PROJECT_NAME,
-    )
+    segment = Segment.from_name(name=SEGMENT_NAME, model_id=MODEL_ID)
     assert isinstance(segment, Segment)
 
 
 @responses.activate
 def test_segment_from_name_not_found() -> None:
     params = {
-        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "age < 50"}, {"field": "model_name", "operator": "equal", "value": "bank_churn"}, {"field": "project_name", "operator": "equal", "value": "bank_churn"}]}'
+        'filter': '{"condition": "AND", "rules": [{"field": "name", "operator": "equal", "value": "age < 50"}, {"field": "model_id", "operator": "equal", "value": "4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2"}]}'
     }
     responses.get(
         url=f'{URL}/v3/segments',
         json=EMPTY_LIST_API_RESPONSE,
         match=[matchers.query_param_matcher(params)],
     )
     with pytest.raises(NotFound):
-        Segment.from_name(
-            name=SEGMENT_NAME,
-            model_name=MODEL_NAME,
-            project_name=PROJECT_NAME,
-        )
+        Segment.from_name(name=SEGMENT_NAME, model_id=MODEL_ID)
 
 
 @responses.activate
 def test_segment_list_empty() -> None:
     responses.get(
         url=f'{URL}/v3/models/{MODEL_ID}/segments',
         json=EMPTY_LIST_API_RESPONSE,
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_webhook.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_webhook.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/apis/test_xai.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/apis/test_xai.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from fiddler.tests.constants import (
     BASE_TEST_DIR,
     DATASET_ID,
     DATASET_NAME,
     JOB_ID,
     MODEL_ID,
     MODEL_NAME,
+    MODEL_VERSION,
     ORG_ID,
     ORG_NAME,
     OUTPUT_DIR,
     PROJECT_ID,
     PROJECT_NAME,
     URL,
     USER_EMAIL,
@@ -66,14 +67,15 @@
     'schema_version': 1,
     'targets': ['Churned'],
 }
 MODEL_API_RESPONSE_200 = {
     'data': {
         'id': MODEL_ID,
         'name': MODEL_NAME,
+        'version': MODEL_VERSION,
         'project': {
             'id': PROJECT_ID,
             'name': PROJECT_NAME,
         },
         'organization': {
             'id': ORG_ID,
             'name': ORG_NAME,
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/conftest.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,9 +22,9 @@
             'organization': {
                 'id': ORG_ID,
                 'name': ORG_NAME,
             },
         }
     )
     session_mocker.patch.object(conn, '_get_server_info', return_value=server_info)
-    session_mocker.patch('fiddler.connection.connection', conn)
+    session_mocker.patch('fiddler.conn', conn)
     yield conn
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/constants.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ORG_ID = '5531bfd9-2ca2-4a7b-bb5a-136c8da09ca0'
 ORG_NAME = 'fiddler_dev'
 SERVER_VERSION = '23.7.0'
 PROJECT_NAME = 'bank_churn'
 PROJECT_ID = '1531bfd9-2ca2-4a7b-bb5a-136c8da09ca1'
 MODEL_NAME = 'bank_churn'
 MODEL_ID = '4531bfd9-2ca2-4a7b-bb5a-136c8da09ca2'
+MODEL_VERSION = 'v1'
 USER_ID = '5531bfd9-2ca2-4a7b-bb5a-136c8da09ca3'
 USER_NAME = 'foo'
 USER_EMAIL = 'foo@fiddler.ai'
 JOB_ID = '9df70575-7ced-42fd-bb50-a0e4351d2c9d'
 JOB_NAME = f'Deleting model {MODEL_NAME}'
 DATASET_ID = 'ba6ec4e4-7188-44c5-ba84-c2cb22b4bb00'
 DATASET_NAME = 'dataset3'
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/test_connection.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/test_json_encoder.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/tests/test_utils.py` & `fiddler-client-3.1.0.dev1/fiddler/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/utils/helpers.py` & `fiddler-client-3.1.0.dev1/fiddler/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/utils/logger.py` & `fiddler-client-3.1.0.dev1/fiddler/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/utils/model_generator.py` & `fiddler-client-3.1.0.dev1/fiddler/utils/model_generator.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler/utils/version.py` & `fiddler-client-3.1.0.dev1/fiddler/utils/version.py`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/fiddler_client.egg-info/PKG-INFO` & `fiddler-client-3.1.0.dev1/fiddler_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddler-client
-Version: 3.0.0.dev9
+Version: 3.1.0.dev1
 Summary: Python client for Fiddler Platform
 Home-page: https://fiddler.ai
 Author: Fiddler Labs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8.0
```

### Comparing `fiddler-client-3.0.0.dev9/fiddler_client.egg-info/SOURCES.txt` & `fiddler-client-3.1.0.dev1/fiddler_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fiddler-client-3.0.0.dev9/setup.py` & `fiddler-client-3.1.0.dev1/setup.py`

 * *Files identical despite different names*

