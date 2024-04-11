# Comparing `tmp/rasgotransforms-2.7.7.tar.gz` & `tmp/rasgotransforms-2.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rasgotransforms-2.7.7.tar", last modified: Wed Mar  8 15:08:22 2023, max compression
+gzip compressed data, was "dist/rasgotransforms-2.7.8.tar", last modified: Thu Apr 11 13:18:46 2024, max compression
```

## Comparing `rasgotransforms-2.7.7.tar` & `rasgotransforms-2.7.8.tar`

### file list

```diff
@@ -1,429 +1,435 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/macros/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/bigquery/aggregate_metrics.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/bigquery/pivot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/combine_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/distinct_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/expression_metrics.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/filter.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/period_over_period.sql
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/period_to_date.sql
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/prior.sql
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/rolling.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/secondary_calculation.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/macros/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/snowflake/aggregate_metrics.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/macros/snowflake/pivot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/render/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/render/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/render/infer_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/render/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/agg_dict.sql
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/boolean.sql
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/calculated_column_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column.sql
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_agg_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_or_expression.sql
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_or_expression_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/column_value_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/custom_option.sql
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/custom_option_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/date.sql
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/date_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/filter_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/int.sql
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/join_type.sql
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/number.sql
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/number_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/sort_dict.sql
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/sort_direction.sql
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/string.sql
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/string_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/table_list.sql
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/snippets/timestamp.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/bigquery/aggregate.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/snowflake/aggregate.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate_string/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate_string/aggregate_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate_string/aggregate_string.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/apply/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/apply/apply.sql
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/apply/apply.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bigquery/bin.sql
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bin.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bin.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/bigquery/cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cast/cast.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/clean/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/clean/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/clean/bigquery/clean.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/clean/clean.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/clean/clean.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/conditional_agg/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/conditional_agg/conditional_agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/conditional_agg/conditional_agg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/correlation/correlation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/correlation/correlation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cumulative_agg/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cumulative_agg/cumulative_agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/cumulative_agg/cumulative_agg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datarobot_score/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datarobot_score/datarobot_score.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datarobot_score/datarobot_score.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/bigquery/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/dateadd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/postgresql/dateadd.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/redshift/dateadd.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/snowflake/dateadd.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/bigquery/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/datediff.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/snowflake/datediff.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/bigquery/datepart.sql
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/datepart.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/datepart.sql
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/datepart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/postgresql/datepart.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/redshift/datepart.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/snowflake/datepart.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/bigquery/datespine.sql
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/datespine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/datespine.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/snowflake/datespine.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/bigquery/datespine_groups.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/datespine_groups.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/snowflake/datespine_groups.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/bigquery/datetrunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/datetrunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/datetrunc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/postgresql/datetrunc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/redshift/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/redshift/datetrunc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/snowflake/datetrunc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/bigquery/describe.sql
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/describe.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/describe/snowflake/describe.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/drop_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/drop_columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/drop_columns.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/dropna.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/dropna.sql
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/dropna.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/bigquery/encode_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/encode_values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/snowflake/encode_values.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/entropy/entropy.sql
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/entropy/entropy.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/extract_sequences.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/snowflake/extract_sequences.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/filter/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/filter/filter.sql
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/filter/filter.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/funnel/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/funnel/funnel.sql
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/funnel/funnel.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/bigquery/heatmap.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/heatmap.sql
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/heatmap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/histogram/histogram.sql
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/histogram/histogram.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/if_then.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/if_then.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/if_then.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/join/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/join/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/join/join.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/join/join.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/joins/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/joins/joins.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/joins/joins.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/bigquery/label_encode.sql
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/label_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/label_encode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/snowflake/label_encode.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/bigquery/lag.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/lag.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/lag.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lag/lag.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/latest/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/latest/latest.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/latest/latest.sql
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/latest/latest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/bigquery/lead.sql
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/lead.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/lead.sql
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/lead/lead.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/linear_regression/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/linear_regression/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/linear_regression/linear_regression.sql
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/linear_regression/linear_regression.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/market_basket/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/market_basket/market_basket.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/market_basket/market_basket.sql
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/market_basket/market_basket.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/bigquery/math.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/math.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/math.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/math/snowflake/math.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric/
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric/metric.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric/metric.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric_plot/
--rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric_plot/metric_plot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/metric_plot/metric_plot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/min_max_scaler.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/min_max_scaler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/moving_avg.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/moving_avg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/moving_avg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/new_columns/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/new_columns/new_columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/new_columns/new_columns.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/one_hot_encode/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/one_hot_encode/one_hot_encode.sql
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/one_hot_encode/one_hot_encode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/order/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/order/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/order/order.sql
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/order/order.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/bigquery/pivot_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/pivot_table.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/snowflake/pivot_table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/plot/
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/plot/plot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/plot/plot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/prefix/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/prefix/prefix.sql
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/prefix/prefix.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/profile_column/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/profile_column/profile_column.sql
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/profile_column/profile_column.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/bigquery/query.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/query.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/query/snowflake/query.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rank/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rank/rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rank/rank.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rank/rank.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/ratio_with_shrinkage.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_duplicates/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_duplicates/remove_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_duplicates/remove_duplicates.sql
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_duplicates/remove_duplicates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/remove_outliers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/remove_outliers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/remove_outliers.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/rename.sql
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/rename.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rename/snowflake/rename.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/bigquery/replace_missing.sql
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/replace_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/replace_missing.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/replace_missing.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/replace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/replace_string.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/replace_string.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/bigquery/reshape.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/reshape.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/snowflake/reshape.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rolling_agg/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rolling_agg/rolling_agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rolling_agg/rolling_agg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rsi/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rsi/rsi.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/rsi/rsi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample/sample.sql
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample/sample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample_class/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample_class/sample_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample_class/sample_class.sql
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sample_class/sample_class.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sankey/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sankey/sankey.sql
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sankey/sankey.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/scale_columns/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/scale_columns/scale_columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/scale_columns/scale_columns.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/select/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/select/select.sql
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/select/select.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/sliding_slope.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/sliding_slope.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/snowflake/sliding_slope.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/standard_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/standard_scaler.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/standard_scaler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/suffix/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/suffix/suffix.sql
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/suffix/suffix.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize/summarize.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize/summarize.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_flatlines/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/bigquery/summarize_islands.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/snowflake/summarize_islands.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/summarize_islands.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/target_encode/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/target_encode/target_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/target_encode/target_encode.sql
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/target_encode/target_encode.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/text_to_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/text_to_sql/text_to_sql.sql
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/text_to_sql/text_to_sql.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/bigquery/timeseries_agg.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/snowflake/timeseries_agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/timeseries_agg.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/timeseries_agg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/to_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/to_date.sql
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/to_date.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/train_test_split/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/train_test_split/train_test_split.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/train_test_split/train_test_split.sql
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/train_test_split/train_test_split.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/union/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/union/union.sql
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/union/union.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unions/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unions/unions.sql
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unions/unions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unpivot/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unpivot/unpivot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/unpivot/unpivot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/bigquery/uppercase_columns.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/snowflake/uppercase_columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/uppercase_columns/uppercase_columns.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/vlookup/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/vlookup/vlookup.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/transforms/vlookup/vlookup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/rasgotransforms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-08 15:08:21.000000 rasgotransforms-2.7.7/rasgotransforms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 15:08:22.000000 rasgotransforms-2.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-08 15:08:05.000000 rasgotransforms-2.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/macros/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/bigquery/aggregate_metrics.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/bigquery/pivot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/combine_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/distinct_values.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/expression_metrics.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/filter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/period_over_period.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/period_to_date.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/prior.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/rolling.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/secondary_calculation.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/macros/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/snowflake/aggregate_metrics.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/macros/snowflake/pivot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/render/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13976 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/render/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/render/infer_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/render/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/agg_dict.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/alias.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/boolean.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/calculated_column_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_agg_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_or_expression.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_or_expression_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/column_value_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/custom_option.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/custom_option_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/date.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/date_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/filter_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/int.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/join_type.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/number.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/number_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/sort_dict.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/sort_direction.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/string_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/table_list.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/snippets/timestamp.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/bigquery/aggregate.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/snowflake/aggregate.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate_string/aggregate_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate_string/aggregate_string.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/apply/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/apply/apply.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/apply/apply.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/bin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bigquery/bin.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bin.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bin.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/bigquery/cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cast/cast.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/clean/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/clean/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/clean/bigquery/clean.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/clean/clean.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/clean/clean.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/bigquery/comparison.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/comparison.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/comparison/snowflake/comparison.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/conditional_agg/
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/conditional_agg/conditional_agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/conditional_agg/conditional_agg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/correlation/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/correlation/correlation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/correlation/correlation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cumulative_agg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cumulative_agg/cumulative_agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/cumulative_agg/cumulative_agg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datarobot_score/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datarobot_score/datarobot_score.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datarobot_score/datarobot_score.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/bigquery/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/dateadd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/postgresql/dateadd.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/redshift/dateadd.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/snowflake/dateadd.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/bigquery/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/datediff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/datediff.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/snowflake/datediff.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/bigquery/datepart.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/datepart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/datepart.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/datepart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/postgresql/datepart.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/redshift/datepart.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/snowflake/datepart.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/bigquery/datespine.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/datespine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/datespine.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/snowflake/datespine.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/bigquery/datespine_groups.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/datespine_groups.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/snowflake/datespine_groups.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/bigquery/datetrunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/datetrunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/datetrunc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/postgresql/datetrunc.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/redshift/datetrunc.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/snowflake/datetrunc.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/bigquery/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/describe.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/describe/snowflake/describe.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/drop_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/drop_columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/drop_columns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/dropna.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/dropna.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/bigquery/encode_values.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/encode_values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/snowflake/encode_values.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/entropy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/entropy/entropy.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/entropy/entropy.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/extract_sequences.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/snowflake/extract_sequences.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/filter/filter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/filter/filter.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/funnel/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/funnel/funnel.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/funnel/funnel.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/bigquery/heatmap.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/heatmap.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/heatmap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/histogram/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/histogram/histogram.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/histogram/histogram.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/if_then.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/if_then.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/if_then.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/join/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/join/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/join/join.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/join/join.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/joins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/joins/joins.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/joins/joins.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/bigquery/label_encode.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/label_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/label_encode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/snowflake/label_encode.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/bigquery/lag.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/lag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/lag.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lag/lag.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/latest/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/latest/latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/latest/latest.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/latest/latest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/bigquery/lead.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/lead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/lead.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/lead/lead.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/linear_regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/linear_regression/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/linear_regression/linear_regression.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/linear_regression/linear_regression.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/market_basket/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/market_basket/market_basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/market_basket/market_basket.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/market_basket/market_basket.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/bigquery/math.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/math.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/math.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/math/snowflake/math.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric/metric.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric/metric.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric_plot/metric_plot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/metric_plot/metric_plot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/min_max_scaler.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/min_max_scaler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/moving_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/moving_avg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/moving_avg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/new_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/new_columns/new_columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/new_columns/new_columns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/one_hot_encode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/one_hot_encode/one_hot_encode.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/one_hot_encode/one_hot_encode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/order/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/order/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/order/order.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/order/order.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/bigquery/pivot_table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/pivot_table.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/snowflake/pivot_table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/plot/plot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/plot/plot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/prefix/prefix.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/prefix/prefix.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/profile_column/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/profile_column/profile_column.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/profile_column/profile_column.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/bigquery/query.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/query.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/query/snowflake/query.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rank/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rank/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rank/rank.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rank/rank.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/ratio_with_shrinkage.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_duplicates/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_duplicates/remove_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_duplicates/remove_duplicates.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_duplicates/remove_duplicates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/remove_outliers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/remove_outliers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/remove_outliers.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/rename.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rename/snowflake/rename.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/bigquery/replace_missing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/replace_missing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/replace_missing.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/replace_missing.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/replace_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/replace_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/replace_string.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/bigquery/reshape.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/reshape.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/snowflake/reshape.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rolling_agg/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rolling_agg/rolling_agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rolling_agg/rolling_agg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rsi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rsi/rsi.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/rsi/rsi.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample/sample.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample/sample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample_class/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample_class/sample_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample_class/sample_class.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sample_class/sample_class.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sankey/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sankey/sankey.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sankey/sankey.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/scale_columns/
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/scale_columns/scale_columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/scale_columns/scale_columns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/select/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/select/select.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/select/select.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/sliding_slope.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/sliding_slope.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/snowflake/sliding_slope.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/standard_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/standard_scaler.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/standard_scaler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/suffix/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/suffix/suffix.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/suffix/suffix.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize/
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize/summarize.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize/summarize.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_flatlines/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/bigquery/summarize_islands.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/snowflake/summarize_islands.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/summarize_islands.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/target_encode/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/target_encode/target_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/target_encode/target_encode.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/target_encode/target_encode.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/text_to_sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/text_to_sql/text_to_sql.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/text_to_sql/text_to_sql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/bigquery/timeseries_agg.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/snowflake/timeseries_agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/timeseries_agg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/timeseries_agg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/to_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/to_date.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/to_date.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/train_test_split/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/train_test_split/train_test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/train_test_split/train_test_split.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/train_test_split/train_test_split.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/union/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/union/union.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/union/union.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unions/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unions/unions.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unions/unions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unpivot/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unpivot/unpivot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/unpivot/unpivot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/bigquery/uppercase_columns.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/snowflake/uppercase_columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/uppercase_columns/uppercase_columns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/vlookup/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/vlookup/vlookup.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/transforms/vlookup/vlookup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/rasgotransforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/rasgotransforms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:18:46.000000 rasgotransforms-2.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-11 13:18:35.000000 rasgotransforms-2.7.8/setup.py
```

### Comparing `rasgotransforms-2.7.7/PKG-INFO` & `rasgotransforms-2.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasgotransforms
-Version: 2.7.7
+Version: 2.7.8
 Summary: Open-source SQL transform templates provided by RasgoML.
 Author: Rasgo Intelligence
 Author-email: patrick@rasgoml.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://docs.rasgoml.com/rasgo-docs/transforms/overview
 Project-URL: Source, https://github.com/rasgointelligence/RasgoTransforms
 Project-URL: Rasgo, https://www.rasgoml.com/
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 
 <p align="left">
   <img width="90%" href="https://rasgoml.com" target="_blank" src="https://gblobscdn.gitbook.com/assets%2F-MJDKltt3A57jhixTfmu%2F-MJZZeY9BhUCtGPyz6bm%2F-MJZiXHTjQnyVWs6YGPc%2Frasgo-logo-full-color-rgb%20(4).png?alt=media&token=64e56b18-4282-4140-836b-e19c8e2787dc" />
```

### Comparing `rasgotransforms-2.7.7/rasgotransforms/dtypes.py` & `rasgotransforms-2.7.8/rasgotransforms/dtypes.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/bigquery/aggregate_metrics.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/bigquery/aggregate_metrics.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/bigquery/pivot.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/bigquery/pivot.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/combine_groups.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/combine_groups.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/distinct_values.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/distinct_values.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/expression_metrics.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/expression_metrics.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/filter.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/filter.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/period_over_period.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/period_over_period.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/period_to_date.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/period_to_date.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/rolling.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/rolling.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/secondary_calculation.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/secondary_calculation.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/snowflake/aggregate_metrics.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/snowflake/aggregate_metrics.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/macros/snowflake/pivot.sql` & `rasgotransforms-2.7.8/rasgotransforms/macros/snowflake/pivot.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/main.py` & `rasgotransforms-2.7.8/rasgotransforms/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 
 class DataWarehouse(Enum):
     """
     Supported Data Warehouses
     """
 
     BIGQUERY = "bigquery"
-    SNOWFLAKE = "snowflake"
-    POSTGRESQL = "postgresql"
+    DELTALAKE = "deltalake"
     MYSQL = "mysql"
+    POSTGRESQL = "postgresql"
     REDSHIFT = "redshift"
+    SNOWFLAKE = "snowflake"
 
 
 class TransformTemplate:
     """
     Reference to a Rasgo transform template
     """
```

### Comparing `rasgotransforms-2.7.7/rasgotransforms/render/environment.py` & `rasgotransforms-2.7.8/rasgotransforms/render/environment.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/render/infer_columns.py` & `rasgotransforms-2.7.8/rasgotransforms/render/infer_columns.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/render/transforms.py` & `rasgotransforms-2.7.8/rasgotransforms/render/transforms.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/snippets/agg_dict.sql` & `rasgotransforms-2.7.8/rasgotransforms/snippets/agg_dict.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.py` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/aggregate.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/aggregate.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/bigquery/aggregate.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/bigquery/aggregate.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate/snowflake/aggregate.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate/snowflake/aggregate.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/aggregate_string/aggregate_string.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/aggregate_string/aggregate_string.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/apply/apply.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/apply/apply.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bigquery/bin.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bigquery/bin.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/bin/bin.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/bin/bin.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/cast/bigquery/cast.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/cast/bigquery/cast.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/cast/cast.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/cast/cast.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/cast/cast.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/cast/cast.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/clean/bigquery/clean.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/clean/bigquery/clean.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/clean/clean.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/clean/clean.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/clean/clean.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/clean/clean.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/conditional_agg/conditional_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/conditional_agg/conditional_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/conditional_agg/conditional_agg.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/conditional_agg/conditional_agg.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/correlation/correlation.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/correlation/correlation.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/cumulative_agg/cumulative_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/cumulative_agg/cumulative_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/cumulative_agg/cumulative_agg.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/cumulative_agg/cumulative_agg.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datarobot_score/datarobot_score.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datarobot_score/datarobot_score.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datarobot_score/datarobot_score.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datarobot_score/datarobot_score.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/dateadd.py` & `rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/dateadd.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/dateadd/dateadd.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/dateadd/dateadd.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datediff/datediff.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datediff/datediff.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/bigquery/datepart.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/bigquery/datepart.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datepart/datepart.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datepart/datepart.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/bigquery/datespine.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/bigquery/datespine.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/datespine.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/datespine.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine/snowflake/datespine.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine/snowflake/datespine.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/bigquery/datespine_groups.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/bigquery/datespine_groups.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/datespine_groups.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/datespine_groups.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datespine_groups/snowflake/datespine_groups.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datespine_groups/snowflake/datespine_groups.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/datetrunc/datetrunc.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/datetrunc/datetrunc.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/describe/bigquery/describe.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/describe/bigquery/describe.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/describe/snowflake/describe.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/describe/snowflake/describe.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/drop_columns.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/drop_columns.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/drop_columns/drop_columns.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/drop_columns/drop_columns.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/dropna.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/dropna.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/dropna/dropna.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/dropna/dropna.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/bigquery/encode_values.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/bigquery/encode_values.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/encode_values.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/encode_values.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/encode_values/snowflake/encode_values.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/encode_values/snowflake/encode_values.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/entropy/entropy.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/entropy/entropy.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/entropy/entropy.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/entropy/entropy.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/extract_sequences.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/extract_sequences.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/extract_sequences/snowflake/extract_sequences.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/extract_sequences/snowflake/extract_sequences.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/filter/filter.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/filter/filter.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/funnel/funnel.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/funnel/funnel.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/bigquery/heatmap.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/bigquery/heatmap.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/heatmap.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/heatmap.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/heatmap/heatmap.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/heatmap/heatmap.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/histogram/histogram.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/histogram/histogram.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/histogram/histogram.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/histogram/histogram.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/if_then.py` & `rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/if_then.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/if_then/if_then.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/if_then/if_then.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/join/join.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/join/join.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/join/join.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/join/join.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/joins/joins.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/joins/joins.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/joins/joins.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/joins/joins.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/label_encode/label_encode.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/label_encode/label_encode.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lag/bigquery/lag.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lag/bigquery/lag.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lag/lag.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lag/lag.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lag/lag.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lag/lag.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/latest/latest.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/latest/latest.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/latest/latest.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/latest/latest.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lead/bigquery/lead.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lead/bigquery/lead.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lead/lead.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lead/lead.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/lead/lead.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/lead/lead.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/linear_regression/linear_regression.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/linear_regression/linear_regression.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/market_basket/market_basket.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/market_basket/market_basket.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/math/math.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/math/math.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/metric/metric.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/metric/metric.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/metric/metric.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/metric/metric.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/metric_plot/metric_plot.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/metric_plot/metric_plot.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/metric_plot/metric_plot.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/metric_plot/metric_plot.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/min_max_scaler.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/min_max_scaler.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/min_max_scaler/min_max_scaler.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/min_max_scaler/min_max_scaler.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/moving_avg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/moving_avg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/moving_avg/moving_avg.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/moving_avg/moving_avg.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/new_columns/new_columns.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/new_columns/new_columns.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/one_hot_encode/one_hot_encode.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/one_hot_encode/one_hot_encode.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/one_hot_encode/one_hot_encode.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/one_hot_encode/one_hot_encode.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/bigquery/pivot_table.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/bigquery/pivot_table.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/pivot_table.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/pivot_table.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/pivot_table/snowflake/pivot_table.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/pivot_table/snowflake/pivot_table.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/plot/plot.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/plot/plot.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/plot/plot.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/plot/plot.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/query/bigquery/query.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/query/bigquery/query.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/query/query.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/query/query.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/query/snowflake/query.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/query/snowflake/query.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rank/rank.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rank/rank.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rank/rank.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rank/rank.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/ratio_with_shrinkage.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/ratio_with_shrinkage.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/ratio_with_shrinkage/snowflake/ratio_with_shrinkage.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/remove_duplicates/remove_duplicates.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/remove_duplicates/remove_duplicates.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/remove_outliers.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/remove_outliers.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/remove_outliers/remove_outliers.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/remove_outliers/remove_outliers.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/bigquery/replace_missing.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/bigquery/replace_missing.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/replace_missing.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/replace_missing.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/replace_missing/replace_missing.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/replace_missing/replace_missing.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/replace_string.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/replace_string.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/replace_string/replace_string.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/replace_string/replace_string.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/bigquery/reshape.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/bigquery/reshape.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/reshape.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/reshape.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/reshape/snowflake/reshape.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/reshape/snowflake/reshape.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rolling_agg/rolling_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rolling_agg/rolling_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rolling_agg/rolling_agg.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rolling_agg/rolling_agg.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rsi/rsi.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rsi/rsi.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/rsi/rsi.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/rsi/rsi.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sample/sample.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sample/sample.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sample/sample.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sample/sample.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sankey/sankey.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sankey/sankey.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/scale_columns/scale_columns.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/scale_columns/scale_columns.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/scale_columns/scale_columns.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/scale_columns/scale_columns.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/sliding_slope.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/sliding_slope.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/sliding_slope.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/sliding_slope.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/sliding_slope/snowflake/sliding_slope.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/sliding_slope/snowflake/sliding_slope.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/standard_scaler.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/standard_scaler.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/standard_scaler/standard_scaler.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/standard_scaler/standard_scaler.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize/summarize.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize/summarize.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize/summarize.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize/summarize.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_flatlines/summarize_flatlines.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/bigquery/summarize_islands.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/bigquery/summarize_islands.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/snowflake/summarize_islands.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/snowflake/summarize_islands.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/summarize_islands/summarize_islands.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/summarize_islands/summarize_islands.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/target_encode/target_encode.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/target_encode/target_encode.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/text_to_sql/text_to_sql.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/text_to_sql/text_to_sql.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/bigquery/timeseries_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/bigquery/timeseries_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/snowflake/timeseries_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/snowflake/timeseries_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/timeseries_agg.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/timeseries_agg.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/timeseries_agg/timeseries_agg.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/timeseries_agg/timeseries_agg.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/to_date.py` & `rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/to_date.py`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/to_date/to_date.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/to_date/to_date.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/train_test_split/train_test_split.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/train_test_split/train_test_split.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/union/union.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/union/union.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/union/union.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/union/union.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/unions/unions.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/unions/unions.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/unions/unions.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/unions/unions.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/unpivot/unpivot.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/unpivot/unpivot.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/vlookup/vlookup.sql` & `rasgotransforms-2.7.8/rasgotransforms/transforms/vlookup/vlookup.sql`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms/transforms/vlookup/vlookup.yaml` & `rasgotransforms-2.7.8/rasgotransforms/transforms/vlookup/vlookup.yaml`

 * *Files identical despite different names*

### Comparing `rasgotransforms-2.7.7/rasgotransforms.egg-info/PKG-INFO` & `rasgotransforms-2.7.8/rasgotransforms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasgotransforms
-Version: 2.7.7
+Version: 2.7.8
 Summary: Open-source SQL transform templates provided by RasgoML.
 Author: Rasgo Intelligence
 Author-email: patrick@rasgoml.com
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Project-URL: Documentation, https://docs.rasgoml.com/rasgo-docs/transforms/overview
 Project-URL: Source, https://github.com/rasgointelligence/RasgoTransforms
 Project-URL: Rasgo, https://www.rasgoml.com/
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Code Generators
 Description-Content-Type: text/markdown
 
 <p align="left">
   <img width="90%" href="https://rasgoml.com" target="_blank" src="https://gblobscdn.gitbook.com/assets%2F-MJDKltt3A57jhixTfmu%2F-MJZZeY9BhUCtGPyz6bm%2F-MJZiXHTjQnyVWs6YGPc%2Frasgo-logo-full-color-rgb%20(4).png?alt=media&token=64e56b18-4282-4140-836b-e19c8e2787dc" />
```

### Comparing `rasgotransforms-2.7.7/rasgotransforms.egg-info/SOURCES.txt` & `rasgotransforms-2.7.8/rasgotransforms.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 rasgotransforms/transforms/cast/cast.py
 rasgotransforms/transforms/cast/cast.sql
 rasgotransforms/transforms/cast/cast.yaml
 rasgotransforms/transforms/cast/bigquery/cast.sql
 rasgotransforms/transforms/clean/clean.sql
 rasgotransforms/transforms/clean/clean.yaml
 rasgotransforms/transforms/clean/bigquery/clean.sql
+rasgotransforms/transforms/comparison/comparison.yaml
+rasgotransforms/transforms/comparison/bigquery/comparison.sql
+rasgotransforms/transforms/comparison/snowflake/comparison.sql
 rasgotransforms/transforms/conditional_agg/conditional_agg.sql
 rasgotransforms/transforms/conditional_agg/conditional_agg.yaml
 rasgotransforms/transforms/correlation/correlation.sql
 rasgotransforms/transforms/correlation/correlation.yaml
 rasgotransforms/transforms/cumulative_agg/cumulative_agg.sql
 rasgotransforms/transforms/cumulative_agg/cumulative_agg.yaml
 rasgotransforms/transforms/datarobot_score/datarobot_score.sql
```

### Comparing `rasgotransforms-2.7.7/setup.py` & `rasgotransforms-2.7.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,14 @@
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Database',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Code Generators',
     ],
     zip_safe=False,
 )
```

