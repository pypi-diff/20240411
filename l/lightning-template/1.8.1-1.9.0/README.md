# Comparing `tmp/lightning-template-1.8.1.tar.gz` & `tmp/lightning-template-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-template-1.8.1.tar", last modified: Fri Feb 23 05:11:00 2024, max compression
+gzip compressed data, was "lightning-template-1.9.0.tar", last modified: Fri Feb 23 12:22:28 2024, max compression
```

## Comparing `lightning-template-1.8.1.tar` & `lightning-template-1.9.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.633947 lightning-template-1.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.617947 lightning-template-1.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.621947 lightning-template-1.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.github/workflows/check_pre_commit_hooks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.github/workflows/pre_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-23 05:10:48.000000 lightning-template-1.8.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-23 05:10:48.000000 lightning-template-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-23 05:11:00.633947 lightning-template-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-23 05:10:48.000000 lightning-template-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.621947 lightning-template-1.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.621947 lightning-template-1.8.1/docs/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.621947 lightning-template-1.8.1/docs/configs/argument_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/configs/argument_parsers/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/configs/argument_parsers/json_file.md
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/configs/argument_parsers/yaml_with_merge.md
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/configs/config_file_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/configs/deep_update.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/docs/core/
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/core/dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/core/model.md
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/core/optimizer_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/core/trainer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/docs/get_started/
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/get_started/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/get_started/contribution.md
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/get_started/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/get_started/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/docs/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-02-23 05:10:48.000000 lightning-template-1.8.1/docs/tools/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11081 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/tools/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/model/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/model/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/tools/model/model_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.625947 lightning-template-1.8.1/lightning_template/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/custom_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/save_and_log_config_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/set_rich_traceback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/deep_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/json_file_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/instantiate_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/cli/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/loggers/
--rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/loop/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/loop/kfold.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/mixin/split_name_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.629947 lightning-template-1.8.1/lightning_template/utils/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/optim/configure_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/optim/warmup_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.633947 lightning-template-1.8.1/lightning_template/utils/progress/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/progress/rich_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.633947 lightning-template-1.8.1/lightning_template/utils/timer/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 05:10:48.000000 lightning-template-1.8.1/lightning_template/utils/timer/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.633947 lightning-template-1.8.1/lightning_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 05:11:00.000000 lightning-template-1.8.1/lightning_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-02-23 05:10:48.000000 lightning-template-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 05:11:00.633947 lightning-template-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 05:11:00.633947 lightning-template-1.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 05:10:48.000000 lightning-template-1.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-23 05:10:48.000000 lightning-template-1.8.1/tests/test_dummpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-23 05:10:48.000000 lightning-template-1.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.720864 lightning-template-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.700864 lightning-template-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.704864 lightning-template-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.github/workflows/check_pre_commit_hooks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.github/workflows/pre_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-23 12:22:11.000000 lightning-template-1.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-23 12:22:11.000000 lightning-template-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-23 12:22:28.720864 lightning-template-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-23 12:22:11.000000 lightning-template-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/configs/argument_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/configs/argument_parsers/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/configs/argument_parsers/json_file.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/configs/argument_parsers/yaml_with_merge.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/configs/config_file_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7464 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/configs/deep_update.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/core/dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/core/model.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/core/optimizer_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/core/trainer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/get_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/get_started/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/get_started/contribution.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/get_started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/get_started/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/docs/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-02-23 12:22:11.000000 lightning-template-1.9.0/docs/tools/cli.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.708864 lightning-template-1.9.0/lightning_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       53 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/tools/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/model/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/model/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/tools/model/model_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.712864 lightning-template-1.9.0/lightning_template/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/custom_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/save_and_log_config_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/set_rich_traceback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/deep_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/json_file_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4981 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/instantiate_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/cli/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/loggers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       56 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/loop/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/loop/kfold.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/mixin/split_name_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/optim/configure_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/optim/warmup_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/progress/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/progress/rich_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template/utils/timer/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-23 12:22:11.000000 lightning-template-1.9.0/lightning_template/utils/timer/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/lightning_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 12:22:28.000000 lightning-template-1.9.0/lightning_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-02-23 12:22:11.000000 lightning-template-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 12:22:28.720864 lightning-template-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:28.716864 lightning-template-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 12:22:11.000000 lightning-template-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-23 12:22:11.000000 lightning-template-1.9.0/tests/test_dummpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-23 12:22:11.000000 lightning-template-1.9.0/tox.ini
```

### Comparing `lightning-template-1.8.1/.github/workflows/check_pre_commit_hooks.yml` & `lightning-template-1.9.0/.github/workflows/check_pre_commit_hooks.yml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/.github/workflows/pre_release.yml` & `lightning-template-1.9.0/.github/workflows/pre_release.yml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/.github/workflows/release.yml` & `lightning-template-1.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/.github/workflows/test.yml` & `lightning-template-1.9.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/.pre-commit-config.yaml` & `lightning-template-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/.readthedocs.yaml` & `lightning-template-1.9.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/LICENSE` & `lightning-template-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/PKG-INFO` & `lightning-template-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.8.1
+Version: 1.9.0
 Summary: A template wrapper for pytorch-lightning.
 Author-email: shenmishajing <shenmishajing@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/shenmishajing/lightning_template
 Project-URL: Repository, https://github.com/shenmishajing/lightning_template
 Project-URL: Documentation, https://lightning-template.readthedocs.io
 Project-URL: Issues, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.8.1/README.md` & `lightning-template-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/Makefile` & `lightning-template-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/conf.py` & `lightning-template-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/configs/argument_parsers/json_file.md` & `lightning-template-1.9.0/docs/configs/argument_parsers/json_file.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/configs/argument_parsers/yaml_with_merge.md` & `lightning-template-1.9.0/docs/configs/argument_parsers/yaml_with_merge.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/configs/config_file_structure.md` & `lightning-template-1.9.0/docs/configs/config_file_structure.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/configs/deep_update.md` & `lightning-template-1.9.0/docs/configs/deep_update.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/core/dataset.md` & `lightning-template-1.9.0/docs/core/dataset.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/core/model.md` & `lightning-template-1.9.0/docs/core/model.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,29 @@
 
 A list of path of checkpoints, if you pass this argument, the checkpoints will be loaded from the path and be used to init the model sequentially.
 
 ### evaluator_cfg
 
 A dict to define your evaluators, which will be split for different split datasets. For more details, see the [Split attr set doc](dataset.md#split-attr-set) in the dataset doc. You can register all the evaluators as submodels of your model by setting the `evaluator_as_submodule` to `True`.
 
+### finetune_cfg
+
+A dict to define which parameters you want to finetune. The config would be like this:
+
+```yaml
+finetune_cfg:
+    finetune: True
+    params:
+        - model.layer1
+        - model.fc
+        ...
+```
+
+If the `finetune` is set to `True`, the parameters in the `params` list will be set to `requires_grad=True`, otherwise, the parameters in the `params` list will be set to `requires_grad=False`. You can omit the `finetune` key, when you want to set it `True`, and you can only set the `finetune_cfg` to the list of params you want to finetune. Also, you use a single str instead of a list of str as params, which means only one group of parameters match that str will be selected.
+
 ### loss_weights
 
 A dict for loss weights, if you use the `loss_step` method from the base LightningModule, the loss dict will multi the loss weight dict before calculating the total loss.
 
 ### predict_tasks
 
 See the [Predict loop doc](#predict-loop) for details.
```

### Comparing `lightning-template-1.8.1/docs/core/optimizer_config.md` & `lightning-template-1.9.0/docs/core/optimizer_config.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/get_started/changelog.md` & `lightning-template-1.9.0/docs/get_started/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## 1.9.0 (2024-02-23)
+
+### Feat
+
+- **finetune**: add finetune cfg feature
+
+### Fix
+
+- **parser_optim_config**: fix parser_optim_config str is sequence bug
+
 ## 1.8.1 (2024-02-23)
 
 ## 1.8.0 (2024-02-21)
 
 ### Feat
 
 - **SetRichTracebackHandlerCallback**: add SetRichTracebackHandlerCallback feature, remove useless doc strings
```

### Comparing `lightning-template-1.8.1/docs/get_started/contribution.md` & `lightning-template-1.9.0/docs/get_started/contribution.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/get_started/installation.md` & `lightning-template-1.9.0/docs/get_started/installation.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/get_started/usage.md` & `lightning-template-1.9.0/docs/get_started/usage.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/index.md` & `lightning-template-1.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/make.bat` & `lightning-template-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/docs/tools/cli.md` & `lightning-template-1.9.0/docs/tools/cli.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/datasets/base.py` & `lightning-template-1.9.0/lightning_template/datasets/base.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/models/base.py` & `lightning-template-1.9.0/lightning_template/models/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 
 import torch
 from lightning.pytorch import LightningModule as _LightningModule
 from lightning.pytorch.utilities.rank_zero import rank_zero_only
 
 from lightning_template.utils.cli import recursive_instantate_class
 from lightning_template.utils.mixin import SplitNameMixin
+from lightning_template.utils.optim.configure_optimizers import get_parameters
 
 
 class LightningModule(SplitNameMixin, _LightningModule):
     def __init__(
         self,
         model: Optional[torch.nn.Module] = None,
         ckpt_path: Optional[Union[str, List[str]]] = None,
+        finetune_cfg: Optional[Union[str, List[str], Mapping]] = None,
         evaluator_cfg: Mapping = None,
         evaluator_as_submodule: bool = True,
         loss_weights=None,
         predict_tasks: Optional[List[str]] = None,
         predict_path: str = "prediction",
         *args,
         **kwargs,
@@ -31,14 +33,23 @@
         self.ckpt_path = ckpt_path
         self.evaluators = {}
         self.loss_weights = loss_weights
 
         self.evaluator_cfg = self.get_split_config(evaluator_cfg)
         self.evaluate_as_submodule = evaluator_as_submodule
 
+        if finetune_cfg is not None:
+            if isinstance(finetune_cfg, str):
+                finetune_cfg = {finetune_cfg}
+            if isinstance(finetune_cfg, list):
+                finetune_cfg = set(finetune_cfg)
+            if isinstance(finetune_cfg, set):
+                finetune_cfg = {"finetune": True, "params": finetune_cfg}
+        self.finetune_cfg = finetune_cfg
+
         if predict_tasks is None:
             predict_tasks = []
         elif isinstance(predict_tasks, str):
             predict_tasks = [predict_tasks]
 
         for task in predict_tasks:
             assert hasattr(self, "predict_" + task), f"task {task} is not supported!"
@@ -46,22 +57,39 @@
         self.predict_tasks = predict_tasks
         self.predict_path = predict_path
 
         # leave for auto lr finder
         self.lr = None
         self.automatic_lr_schedule = True
         self.manual_step_scedulers = []
+        self.model_not_configured = True
 
         if ckpt_path is not None:
             for p in ckpt_path:
                 if os.path.exists(p):
                     checkpoint = torch.load(p, map_location="cpu")
                     self.on_load_checkpoint(checkpoint)
                     self.load_state_dict(checkpoint["state_dict"], strict=False)
 
+    def configure_model(self):
+        super().configure_model()
+
+        if self.model_not_configured:
+            if self.finetune_cfg:
+                params = get_parameters(
+                    self,
+                    self.finetune_cfg["params"],
+                    finetune_rest=not self.finetune_cfg["finetune"],
+                )
+                for param in params.values():
+                    for p in param:
+                        p.requires_grad = self.finetune_cfg["finetune"]
+
+            self.model_not_configured = False
+
     @staticmethod
     def recursive_parse_modules(module):
         modules = []
         if isinstance(module, torch.nn.Module):
             modules.append(module)
         elif isinstance(module, list):
             for m in module:
```

### Comparing `lightning-template-1.8.1/lightning_template/tools/model/batch_size_finder.py` & `lightning-template-1.9.0/lightning_template/tools/model/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/tools/model/model_statistics.py` & `lightning-template-1.9.0/lightning_template/tools/model/model_statistics.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/custom_repr.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/custom_repr.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/model_checkpoint.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/save_and_log_config_callback.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/save_and_log_config_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/set_rich_traceback_handler.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/set_rich_traceback_handler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py` & `lightning-template-1.9.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/deep_update.py` & `lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/deep_update.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/json_file_action.py` & `lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/json_file_action.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py` & `lightning-template-1.9.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/cli.py` & `lightning-template-1.9.0/lightning_template/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/instantiate_class.py` & `lightning-template-1.9.0/lightning_template/utils/cli/instantiate_class.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/cli/trainer.py` & `lightning-template-1.9.0/lightning_template/utils/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/loop/kfold.py` & `lightning-template-1.9.0/lightning_template/utils/loop/kfold.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/mixin/split_name_mixin.py` & `lightning-template-1.9.0/lightning_template/utils/mixin/split_name_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/optim/configure_optimizers.py` & `lightning-template-1.9.0/lightning_template/utils/optim/configure_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import copy
 from collections import defaultdict
 from itertools import chain
-from typing import List, Mapping, Sequence, Tuple, Union
+from typing import List, Mapping, Tuple, Union
 
 from lightning.pytorch import LightningModule
 from lightning.pytorch.cli import instantiate_class
 from lightning.pytorch.utilities.types import LRSchedulerType
 from torch.optim import Optimizer
 
 
 def parser_optim_config(optim_config):
     """Parse the optimizer config.
 
     Args:
         optim_config (dict): The optimizer and lr_scheduler config.
     """
     optim_config = copy.deepcopy(optim_config)
-    if not isinstance(optim_config, Sequence):
+    if not isinstance(optim_config, list):
         optim_config = [optim_config]
 
     all_required_parameters = set()
     for optim_idx, optim_cfg in enumerate(optim_config):
         # parse the optimizer config
         if "optimizer" not in optim_cfg:
             optim_config[optim_idx] = {"optimizer": optim_cfg}
@@ -28,27 +28,27 @@
 
         # parse the params of optimizers
         if "init_args" not in optim_cfg["optimizer"]:
             optim_cfg["optimizer"]["init_args"] = {}
         optimizer_init_args = optim_cfg["optimizer"]["init_args"]
         if "params" not in optimizer_init_args:
             optimizer_init_args["params"] = [{"params": None}]
-        if not isinstance(optimizer_init_args["params"], Sequence):
+        if not isinstance(optimizer_init_args["params"], list):
             optimizer_init_args["params"] = [optimizer_init_args["params"]]
 
         for param_idx in range(len(optimizer_init_args["params"])):
             cur_params = optimizer_init_args["params"][param_idx]
             if not isinstance(cur_params, Mapping):
-                if not isinstance(cur_params, List):
+                if not isinstance(cur_params, list):
                     cur_params = [cur_params]
                 optimizer_init_args["params"][param_idx] = {"params": cur_params}
                 cur_params = optimizer_init_args["params"][param_idx]
             elif "params" not in cur_params:
                 cur_params["params"] = [None]
-            elif not isinstance(cur_params["params"], List):
+            elif not isinstance(cur_params["params"], list):
                 cur_params["params"] = [cur_params["params"]]
 
             for p in cur_params["params"]:
                 assert p is None or isinstance(p, str), (
                     f"params must be None or str, but got {type(p)} in {param_idx}th"
                     f" parameter of {optim_idx}th optimizer"
                 )
@@ -59,37 +59,39 @@
         # parse the lr_scheduler config
         if "lr_scheduler" in optim_cfg:
             if "scheduler" not in optim_cfg["lr_scheduler"]:
                 optim_cfg["lr_scheduler"] = {"scheduler": optim_cfg["lr_scheduler"]}
     return optim_config, all_required_parameters
 
 
-def get_parameters(model, all_required_parameters):
+def get_parameters(
+    model, all_required_parameters: set, finetune_rest=False, return_rest=False
+):
     """Get all optimizer parameters.
 
     Args:
         model: a LightningModule.
         all_required_parameters: a set of required parameter names.
     """
     parameters = defaultdict(list)
-    set_rest = None in all_required_parameters
+    return_rest = return_rest or None in all_required_parameters
     all_required_parameters.discard(None)
     all_required_parameters = sorted(
         sorted(all_required_parameters), key=len, reverse=True
     )
     for name, p in model.named_parameters():
         for required_parameter in all_required_parameters:
             if required_parameter in name:
                 parameters[required_parameter].append(p)
                 break
         else:
-            if set_rest:
+            if return_rest:
                 parameters[None].append(p)
             else:
-                raise ValueError(f"parameter {name} is not in required_parameters")
+                p.requires_grad = finetune_rest
     return parameters
 
 
 def construct_lr_scheduler(lr_scheduler, optimizer):
     """Constructs the lr_scheduler.
 
     Args:
```

### Comparing `lightning-template-1.8.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py` & `lightning-template-1.9.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/optim/warmup_lr_scheduler.py` & `lightning-template-1.9.0/lightning_template/utils/optim/warmup_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/progress/rich_progress.py` & `lightning-template-1.9.0/lightning_template/utils/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template/utils/timer/timer.py` & `lightning-template-1.9.0/lightning_template/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template.egg-info/PKG-INFO` & `lightning-template-1.9.0/lightning_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.8.1
+Version: 1.9.0
 Summary: A template wrapper for pytorch-lightning.
 Author-email: shenmishajing <shenmishajing@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/shenmishajing/lightning_template
 Project-URL: Repository, https://github.com/shenmishajing/lightning_template
 Project-URL: Documentation, https://lightning-template.readthedocs.io
 Project-URL: Issues, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.8.1/lightning_template.egg-info/SOURCES.txt` & `lightning-template-1.9.0/lightning_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/lightning_template.egg-info/requires.txt` & `lightning-template-1.9.0/lightning_template.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightning-template-1.8.1/pyproject.toml` & `lightning-template-1.9.0/pyproject.toml`

 * *Files identical despite different names*

