# Comparing `tmp/trl-0.8.1.tar.gz` & `tmp/trl-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trl-0.8.1.tar", last modified: Wed Mar 20 10:14:40 2024, max compression
+gzip compressed data, was "trl-0.8.2.tar", last modified: Thu Apr 11 13:39:44 2024, max compression
```

## Comparing `trl-0.8.1.tar` & `trl-0.8.2.tar`

### file list

```diff
@@ -1,106 +1,116 @@
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.184010 trl-0.8.1/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2507 2024-03-18 13:19:22.000000 trl-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.8.1/LICENSE
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      110 2024-03-18 13:19:22.000000 trl-0.8.1/MANIFEST.in
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10215 2024-03-20 10:14:40.184010 trl-0.8.1/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9100 2024-03-19 15:56:20.000000 trl-0.8.1/README.md
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.164008 trl-0.8.1/examples/
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.176009 trl-0.8.1/examples/datasets/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4229 2024-03-18 13:19:22.000000 trl-0.8.1/examples/datasets/anthropic_hh.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4139 2024-03-18 13:19:22.000000 trl-0.8.1/examples/datasets/tldr_preference.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1559 2024-03-18 13:19:22.000000 trl-0.8.1/examples/datasets/tokenize_ds.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1380 2024-02-15 03:39:06.000000 trl-0.8.1/examples/hello_world.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.164008 trl-0.8.1/examples/scripts/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6500 2024-03-11 16:24:14.000000 trl-0.8.1/examples/scripts/ddpo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5361 2024-03-18 13:19:22.000000 trl-0.8.1/examples/scripts/dpo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4996 2024-03-04 01:30:55.000000 trl-0.8.1/examples/scripts/kto.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7646 2024-02-15 03:39:06.000000 trl-0.8.1/examples/scripts/ppo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5261 2024-02-15 03:39:06.000000 trl-0.8.1/examples/scripts/ppo_multi_adapter.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4596 2024-03-11 16:24:14.000000 trl-0.8.1/examples/scripts/reward_modeling.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4730 2024-03-18 13:19:22.000000 trl-0.8.1/examples/scripts/sft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      509 2024-03-12 11:43:24.000000 trl-0.8.1/pyproject.toml
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       73 2024-03-20 10:14:40.184010 trl-0.8.1/setup.cfg
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4547 2024-03-20 10:13:56.000000 trl-0.8.1/setup.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.172009 trl-0.8.1/tests/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.8.1/tests/__init__.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.172009 trl-0.8.1/tests/slow/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-01-19 10:49:50.000000 trl-0.8.1/tests/slow/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7757 2024-02-02 13:30:59.000000 trl-0.8.1/tests/slow/test_dpo_slow.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14741 2024-02-02 13:30:59.000000 trl-0.8.1/tests/slow/test_sft_slow.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1082 2024-01-19 10:49:50.000000 trl-0.8.1/tests/slow/testing_constants.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3158 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1718 2024-03-19 15:56:20.000000 trl-0.8.1/tests/test_cli.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1545 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_core.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5505 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_data_collator_completion_only.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6894 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_dataset_formatting.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4168 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_ddpo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    22515 2024-03-04 01:30:55.000000 trl-0.8.1/tests/test_dpo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.8.1/tests/test_e2e.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11127 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_environments.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4597 2024-03-18 13:19:22.000000 trl-0.8.1/tests/test_iterative_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12028 2024-03-18 13:19:22.000000 trl-0.8.1/tests/test_kto_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    22746 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_modeling_value_head.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5560 2024-03-18 13:19:22.000000 trl-0.8.1/tests/test_no_peft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9122 2024-02-02 13:30:59.000000 trl-0.8.1/tests/test_peft_models.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    47392 2024-03-18 13:19:22.000000 trl-0.8.1/tests/test_ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    13529 2024-02-16 07:52:28.000000 trl-0.8.1/tests/test_reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    36508 2024-03-04 01:30:55.000000 trl-0.8.1/tests/test_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.8.1/tests/testing_constants.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3067 2024-01-19 10:49:50.000000 trl-0.8.1/tests/testing_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.172009 trl-0.8.1/trl/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3699 2024-03-20 10:13:56.000000 trl-0.8.1/trl/__init__.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.176009 trl-0.8.1/trl/commands/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1207 2024-03-18 13:19:22.000000 trl-0.8.1/trl/commands/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2367 2024-03-19 15:56:20.000000 trl-0.8.1/trl/commands/cli.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12964 2024-03-19 15:56:20.000000 trl-0.8.1/trl/commands/cli_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.176009 trl-0.8.1/trl/commands/scripts/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12612 2024-03-20 10:12:57.000000 trl-0.8.1/trl/commands/scripts/chat.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.180009 trl-0.8.1/trl/commands/scripts/config/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      487 2024-03-19 15:56:20.000000 trl-0.8.1/trl/commands/scripts/config/default_chat_config.yaml
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6500 2024-03-11 16:24:14.000000 trl-0.8.1/trl/commands/scripts/ddpo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5361 2024-03-18 13:19:22.000000 trl-0.8.1/trl/commands/scripts/dpo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4996 2024-03-04 01:30:55.000000 trl-0.8.1/trl/commands/scripts/kto.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7646 2024-02-15 03:39:06.000000 trl-0.8.1/trl/commands/scripts/ppo.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5261 2024-02-15 03:39:06.000000 trl-0.8.1/trl/commands/scripts/ppo_multi_adapter.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4596 2024-03-11 16:24:14.000000 trl-0.8.1/trl/commands/scripts/reward_modeling.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4730 2024-03-18 13:19:22.000000 trl-0.8.1/trl/commands/scripts/sft.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12148 2024-03-11 16:24:14.000000 trl-0.8.1/trl/core.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.180009 trl-0.8.1/trl/environment/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      390 2024-03-18 13:19:22.000000 trl-0.8.1/trl/environment/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    17569 2024-02-15 03:39:06.000000 trl-0.8.1/trl/environment/base_environment.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.180009 trl-0.8.1/trl/extras/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      971 2024-03-18 13:19:22.000000 trl-0.8.1/trl/extras/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5182 2024-02-15 03:39:06.000000 trl-0.8.1/trl/extras/best_of_n_sampler.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3646 2024-01-15 13:42:04.000000 trl-0.8.1/trl/extras/dataset_formatting.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6005 2024-03-18 13:19:22.000000 trl-0.8.1/trl/import_utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.180009 trl-0.8.1/trl/models/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2177 2024-03-18 13:19:22.000000 trl-0.8.1/trl/models/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    28788 2024-02-15 03:39:06.000000 trl-0.8.1/trl/models/modeling_base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    27695 2024-02-15 03:58:35.000000 trl-0.8.1/trl/models/modeling_sd_base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18552 2024-02-15 03:39:06.000000 trl-0.8.1/trl/models/modeling_value_head.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5874 2024-02-15 03:58:35.000000 trl-0.8.1/trl/models/sd_utils.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3535 2024-03-18 13:19:22.000000 trl-0.8.1/trl/models/utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.184010 trl-0.8.1/trl/trainer/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3043 2024-03-18 13:19:22.000000 trl-0.8.1/trl/trainer/__init__.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.8.1/trl/trainer/base.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4891 2024-02-15 03:39:06.000000 trl-0.8.1/trl/trainer/ddpo_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    26796 2024-02-15 03:39:06.000000 trl-0.8.1/trl/trainer/ddpo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    62508 2024-03-19 09:59:20.000000 trl-0.8.1/trl/trainer/dpo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    16699 2024-02-02 13:30:59.000000 trl-0.8.1/trl/trainer/iterative_sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4782 2024-02-22 08:57:14.000000 trl-0.8.1/trl/trainer/kto_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    59606 2024-03-18 13:19:22.000000 trl-0.8.1/trl/trainer/kto_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3189 2024-03-12 15:24:54.000000 trl-0.8.1/trl/trainer/model_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8202 2024-01-30 06:49:36.000000 trl-0.8.1/trl/trainer/ppo_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    62832 2024-02-15 04:30:52.000000 trl-0.8.1/trl/trainer/ppo_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1623 2024-01-30 06:49:36.000000 trl-0.8.1/trl/trainer/reward_config.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    13957 2024-02-22 08:57:14.000000 trl-0.8.1/trl/trainer/reward_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    26584 2024-03-18 13:19:22.000000 trl-0.8.1/trl/trainer/sft_trainer.py
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    34989 2024-03-18 13:19:22.000000 trl-0.8.1/trl/trainer/utils.py
-drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-03-20 10:14:40.176009 trl-0.8.1/trl.egg-info/
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10215 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/PKG-INFO
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2644 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/SOURCES.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/dependency_links.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       46 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/entry_points.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.8.1/trl.egg-info/not-zip-safe
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      519 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/requires.txt
--rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2024-03-20 10:14:40.000000 trl-0.8.1/trl.egg-info/top_level.txt
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.908942 trl-0.8.2/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2507 2024-03-18 13:19:22.000000 trl-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11357 2023-05-03 09:18:40.000000 trl-0.8.2/LICENSE
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      110 2024-03-18 13:19:22.000000 trl-0.8.2/MANIFEST.in
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10388 2024-04-11 13:39:44.908942 trl-0.8.2/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9273 2024-04-08 14:24:56.000000 trl-0.8.2/README.md
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.896942 trl-0.8.2/examples/
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/examples/datasets/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4229 2024-03-18 13:19:22.000000 trl-0.8.2/examples/datasets/anthropic_hh.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4139 2024-03-18 13:19:22.000000 trl-0.8.2/examples/datasets/tldr_preference.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1559 2024-03-18 13:19:22.000000 trl-0.8.2/examples/datasets/tokenize_ds.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1380 2024-02-15 03:39:06.000000 trl-0.8.2/examples/hello_world.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.896942 trl-0.8.2/examples/scripts/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6500 2024-03-11 16:24:14.000000 trl-0.8.2/examples/scripts/ddpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6054 2024-04-08 14:24:56.000000 trl-0.8.2/examples/scripts/dpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3729 2024-04-08 14:24:56.000000 trl-0.8.2/examples/scripts/kto.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7646 2024-02-15 03:39:06.000000 trl-0.8.2/examples/scripts/ppo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5261 2024-02-15 03:39:06.000000 trl-0.8.2/examples/scripts/ppo_multi_adapter.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4596 2024-03-11 16:24:14.000000 trl-0.8.2/examples/scripts/reward_modeling.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4730 2024-03-18 13:19:22.000000 trl-0.8.2/examples/scripts/sft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      509 2024-03-12 11:43:24.000000 trl-0.8.2/pyproject.toml
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       73 2024-04-11 13:39:44.908942 trl-0.8.2/setup.cfg
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4547 2024-04-11 13:36:19.000000 trl-0.8.2/setup.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/tests/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2023-05-03 09:18:40.000000 trl-0.8.2/tests/__init__.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/tests/slow/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-01-19 10:49:50.000000 trl-0.8.2/tests/slow/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7757 2024-02-02 13:30:59.000000 trl-0.8.2/tests/slow/test_dpo_slow.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14741 2024-02-02 13:30:59.000000 trl-0.8.2/tests/slow/test_sft_slow.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1082 2024-01-19 10:49:50.000000 trl-0.8.2/tests/slow/testing_constants.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3158 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1723 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_cli.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1545 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_core.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6283 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_cpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5505 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_data_collator_completion_only.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6894 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_dataset_formatting.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4168 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_ddpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    22515 2024-03-04 01:30:55.000000 trl-0.8.2/tests/test_dpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      152 2023-06-21 08:50:41.000000 trl-0.8.2/tests/test_e2e.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    11127 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_environments.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4597 2024-03-18 13:19:22.000000 trl-0.8.2/tests/test_iterative_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14983 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_kto_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    22746 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_modeling_value_head.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5560 2024-03-18 13:19:22.000000 trl-0.8.2/tests/test_no_peft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6119 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_orpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     9122 2024-02-02 13:30:59.000000 trl-0.8.2/tests/test_peft_models.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    47392 2024-03-18 13:19:22.000000 trl-0.8.2/tests/test_ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    13419 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1640 2024-04-08 14:24:56.000000 trl-0.8.2/tests/test_rich_progress_callback.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    43099 2024-04-11 13:36:02.000000 trl-0.8.2/tests/test_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      799 2023-05-03 09:18:40.000000 trl-0.8.2/tests/testing_constants.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3342 2024-04-11 13:36:02.000000 trl-0.8.2/tests/testing_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/trl/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3921 2024-04-11 13:36:25.000000 trl-0.8.2/trl/__init__.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/trl/commands/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1207 2024-03-18 13:19:22.000000 trl-0.8.2/trl/commands/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2367 2024-03-19 15:56:20.000000 trl-0.8.2/trl/commands/cli.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12965 2024-04-08 14:24:56.000000 trl-0.8.2/trl/commands/cli_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.904942 trl-0.8.2/trl/commands/scripts/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12612 2024-03-20 10:12:57.000000 trl-0.8.2/trl/commands/scripts/chat.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.904942 trl-0.8.2/trl/commands/scripts/config/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      487 2024-03-19 15:56:20.000000 trl-0.8.2/trl/commands/scripts/config/default_chat_config.yaml
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4003 2024-04-08 14:24:56.000000 trl-0.8.2/trl/commands/scripts/cpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6500 2024-03-11 16:24:14.000000 trl-0.8.2/trl/commands/scripts/ddpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6054 2024-04-08 14:24:56.000000 trl-0.8.2/trl/commands/scripts/dpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3729 2024-04-08 14:24:56.000000 trl-0.8.2/trl/commands/scripts/kto.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4057 2024-04-08 14:24:56.000000 trl-0.8.2/trl/commands/scripts/orpo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7646 2024-02-15 03:39:06.000000 trl-0.8.2/trl/commands/scripts/ppo.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5261 2024-02-15 03:39:06.000000 trl-0.8.2/trl/commands/scripts/ppo_multi_adapter.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4596 2024-03-11 16:24:14.000000 trl-0.8.2/trl/commands/scripts/reward_modeling.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4730 2024-03-18 13:19:22.000000 trl-0.8.2/trl/commands/scripts/sft.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     7371 2024-04-11 13:36:02.000000 trl-0.8.2/trl/commands/scripts/vsft_llava.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    12148 2024-03-11 16:24:14.000000 trl-0.8.2/trl/core.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.904942 trl-0.8.2/trl/environment/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      390 2024-03-18 13:19:22.000000 trl-0.8.2/trl/environment/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    17569 2024-02-15 03:39:06.000000 trl-0.8.2/trl/environment/base_environment.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.904942 trl-0.8.2/trl/extras/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      971 2024-03-18 13:19:22.000000 trl-0.8.2/trl/extras/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5182 2024-02-15 03:39:06.000000 trl-0.8.2/trl/extras/best_of_n_sampler.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3646 2024-01-15 13:42:04.000000 trl-0.8.2/trl/extras/dataset_formatting.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6079 2024-04-11 13:36:02.000000 trl-0.8.2/trl/import_utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.904942 trl-0.8.2/trl/models/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2208 2024-04-08 14:24:56.000000 trl-0.8.2/trl/models/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    28788 2024-02-15 03:39:06.000000 trl-0.8.2/trl/models/modeling_base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    27695 2024-02-15 03:58:35.000000 trl-0.8.2/trl/models/modeling_sd_base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    18933 2024-04-08 14:24:56.000000 trl-0.8.2/trl/models/modeling_value_head.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     5874 2024-02-15 03:58:35.000000 trl-0.8.2/trl/models/sd_utils.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     6026 2024-04-08 14:24:56.000000 trl-0.8.2/trl/models/utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.908942 trl-0.8.2/trl/trainer/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3343 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/__init__.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1772 2023-05-03 09:18:40.000000 trl-0.8.2/trl/trainer/base.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3875 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/cpo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    44118 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/cpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4891 2024-02-15 03:39:06.000000 trl-0.8.2/trl/trainer/ddpo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    26796 2024-02-15 03:39:06.000000 trl-0.8.2/trl/trainer/ddpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    62510 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/dpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    16699 2024-02-02 13:30:59.000000 trl-0.8.2/trl/trainer/iterative_sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     4970 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/kto_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    63623 2024-04-11 13:28:54.000000 trl-0.8.2/trl/trainer/kto_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3297 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/model_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     3500 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/orpo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    45703 2024-04-11 13:28:54.000000 trl-0.8.2/trl/trainer/orpo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     8202 2024-01-30 06:49:36.000000 trl-0.8.2/trl/trainer/ppo_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    63097 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/ppo_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     1623 2024-01-30 06:49:36.000000 trl-0.8.2/trl/trainer/reward_config.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    14097 2024-04-11 13:28:54.000000 trl-0.8.2/trl/trainer/reward_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    27414 2024-04-11 13:36:02.000000 trl-0.8.2/trl/trainer/sft_trainer.py
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    35309 2024-04-08 14:24:56.000000 trl-0.8.2/trl/trainer/utils.py
+drwxr-xr-x   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        0 2024-04-11 13:39:44.900942 trl-0.8.2/trl.egg-info/
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)    10388 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/PKG-INFO
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)     2934 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/SOURCES.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/dependency_links.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       46 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/entry_points.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)        1 2023-05-17 08:26:30.000000 trl-0.8.2/trl.egg-info/not-zip-safe
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)      519 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/requires.txt
+-rw-r--r--   0 younes_huggingface_co (441877810) younes_huggingface_co (441877810)       10 2024-04-11 13:39:44.000000 trl-0.8.2/trl.egg-info/top_level.txt
```

### Comparing `trl-0.8.1/CONTRIBUTING.md` & `trl-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/LICENSE` & `trl-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/PKG-INFO` & `trl-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.1
+Version: 0.8.2
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -59,15 +59,15 @@
 ## Highlights
 
 - **`Efficient and scalable`**: 
     - [`accelerate`](https://github.com/huggingface/accelerate) is the backbone of `trl` which allows to scale model training from a single GPU to a large scale multi-node cluster with methods such as DDP and DeepSpeed.
     - [`PEFT`](https://github.com/huggingface/peft) is fully integrated and allows to train even the largest models on modest hardware with quantisation and methods such as LoRA or QLoRA.
     - [`unsloth`](https://github.com/unslothai/unsloth) is also integrated and allows to significantly speed up training with dedicated kernels.
 - **`CLI`**: With the [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with LLMs without writing any code using a single command and a flexible config system.
-- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer).
+- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.ORPOTrainer).
 - **`AutoModels`**: The [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForCausalLMWithValueHead) & [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value head to the model which allows to train them with RL algorithms such as PPO.
 - **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT sentiment classifier, full RLHF using adapters only, train GPT-j to be less toxic, [StackLlama example](https://huggingface.co/blog/stackllama), etc. following the [examples](https://github.com/huggingface/trl/tree/main/examples).
 
 ## Installation
 
 ### Python package
 Install the library with `pip`:
@@ -96,32 +96,32 @@
 ```bash
 trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --output_dir opt-sft-imdb
 ```
 
 **DPO:**
 
 ```bash
-trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-processed --output_dir opt-sft-hh-rlhf 
+trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --output_dir opt-sft-hh-rlhf 
 ```
 
 **Chat:**
 
 ```bash
 trl chat --model_name_or_path Qwen/Qwen1.5-0.5B-Chat
 ```
 
 Read more about CLI in the [relevant documentation section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more details.
 
 ## How to use
 
-For more flexibility and control over the training you can use the dedicated trainer classes to fine-tune the model in Python.
+For more flexibility and control over the training, you can use the dedicated trainer classes to fine-tune the model in Python.
 
 ### `SFTTrainer`
 
-This is a basic example on how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
+This is a basic example of how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
 
 ```python
 # imports
 from datasets import load_dataset
 from trl import SFTTrainer
 
 # get dataset
@@ -137,15 +137,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `RewardTrainer`
 
-This is a basic example on how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+This is a basic example of how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 from trl import RewardTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -163,15 +163,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `PPOTrainer`
 
-This is a basic example on how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
+This is a basic example of how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
 
 ```python
 # imports
 import torch
 from transformers import AutoTokenizer
 from trl import PPOTrainer, PPOConfig, AutoModelForCausalLMWithValueHead, create_reference_model
 from trl.core import respond_to_batch
@@ -202,15 +202,15 @@
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### `DPOTrainer`
 
-`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from trl import DPOTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -242,15 +242,15 @@
 
 ## References
 
 ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper **"Fine-Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper](https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-human-preferences)].
 
 ### Direct Preference Optimization
-DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
+DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
 
 
 ## Citation
 
 ```bibtex
 @misc{vonwerra2022trl,
   author = {Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert and Shengyi Huang},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.1 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.2 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
@@ -35,16 +35,18 @@
 significantly speed up training with dedicated kernels. - **`CLI`**: With the
 [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with
 LLMs without writing any code using a single command and a flexible config
 system. - **`Trainers`**: The Trainer classes are an abstraction to apply many
 fine-tuning methods with ease such as the [`SFTTrainer`](https://
 huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/
 docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/
-docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/
-trainer#trl.PPOTrainer). - **`AutoModels`**: The
+docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.ORPOTrainer). - **`AutoModels`**: The
 [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForCausalLMWithValueHead) &
 [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value
 head to the model which allows to train them with RL algorithms such as PPO. -
 **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT
 sentiment classifier, full RLHF using adapters only, train GPT-j to be less
@@ -57,37 +59,37 @@
 want to use the examples you can clone the repository with the following
 command: ```bash git clone https://github.com/huggingface/trl.git ``` ##
 Command Line Interface (CLI) You can use TRL Command Line Interface (CLI) to
 quickly get started with Supervised Fine-tuning (SFT), Direct Preference
 Optimization (DPO) and test your aligned model with the chat CLI: **SFT:**
 ```bash trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --
 output_dir opt-sft-imdb ``` **DPO:** ```bash trl dpo --model_name_or_path
-facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-
-processed --output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --
-model_name_or_path Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the
-[relevant documentation section](https://huggingface.co/docs/trl/main/en/clis)
-or use `--help` for more details. ## How to use For more flexibility and
-control over the training you can use the dedicated trainer classes to fine-
-tune the model in Python. ### `SFTTrainer` This is a basic example on how to
-use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper
-around the `transformers` Trainer to easily fine-tune language models or
-adapters on a custom dataset. ```python # imports from datasets import
-load_dataset from trl import SFTTrainer # get dataset dataset = load_dataset
-("imdb", split="train") # get trainer trainer = SFTTrainer( "facebook/opt-
-350m", train_dataset=dataset, dataset_text_field="text", max_seq_length=512, )
-# train trainer.train() ``` ### `RewardTrainer` This is a basic example on how
-to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper
-around the `transformers` Trainer to easily fine-tune reward models or adapters
-on a custom preference dataset. ```python # imports from transformers import
+facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --
+output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --model_name_or_path
+Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the [relevant documentation
+section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more
+details. ## How to use For more flexibility and control over the training, you
+can use the dedicated trainer classes to fine-tune the model in Python. ###
+`SFTTrainer` This is a basic example of how to use the `SFTTrainer` from the
+library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer
+to easily fine-tune language models or adapters on a custom dataset. ```python
+# imports from datasets import load_dataset from trl import SFTTrainer # get
+dataset dataset = load_dataset("imdb", split="train") # get trainer trainer =
+SFTTrainer( "facebook/opt-350m", train_dataset=dataset,
+dataset_text_field="text", max_seq_length=512, ) # train trainer.train() ```
+### `RewardTrainer` This is a basic example of how to use the `RewardTrainer`
+from the library. The `RewardTrainer` is a wrapper around the `transformers`
+Trainer to easily fine-tune reward models or adapters on a custom preference
+dataset. ```python # imports from transformers import
 AutoModelForSequenceClassification, AutoTokenizer from trl import RewardTrainer
 # load model and dataset - dataset needs to be in a specific format model =
 AutoModelForSequenceClassification.from_pretrained("gpt2", num_labels=1)
 tokenizer = AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer =
 RewardTrainer( model=model, tokenizer=tokenizer, train_dataset=dataset, ) #
-train trainer.train() ``` ### `PPOTrainer` This is a basic example on how to
+train trainer.train() ``` ### `PPOTrainer` This is a basic example of how to
 use the `PPOTrainer` from the library. Based on a query the language model
 creates a response which is then evaluated. The evaluation could be a human in
 the loop or another model's output. ```python # imports import torch from
 transformers import AutoTokenizer from trl import PPOTrainer, PPOConfig,
 AutoModelForCausalLMWithValueHead, create_reference_model from trl.core import
 respond_to_batch # get models model =
 AutoModelForCausalLMWithValueHead.from_pretrained('gpt2') model_ref =
@@ -99,15 +101,15 @@
 (model, query_tensor) # create a ppo trainer ppo_trainer = PPOTrainer
 (ppo_config, model, model_ref, tokenizer) # define a reward for response #
 (this could be any reward such as human feedback or output from another model)
 reward = [torch.tensor(1.0)] # train model for one step with ppo train_stats =
 ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward) ``` ###
 `DPOTrainer` `DPOTrainer` is a trainer that uses [Direct Preference
 Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic
-example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
+example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
 wrapper around the `transformers` Trainer to easily fine-tune reward models or
 adapters on a custom preference dataset. ```python # imports from transformers
 import AutoModelForCausalLM, AutoTokenizer from trl import DPOTrainer # load
 model and dataset - dataset needs to be in a specific format model =
 AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer = DPOTrainer
 ( model=model, tokenizer=tokenizer, train_dataset=dataset, ) # train
@@ -117,14 +119,15 @@
 dev install: ```bash git clone https://github.com/huggingface/trl.git cd trl/
 make dev ``` ## References ### Proximal Policy Optimisation The PPO
 implementation largely follows the structure introduced in the paper **"Fine-
 Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper]
 (https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-
 human-preferences)]. ### Direct Preference Optimization DPO is based on the
 original implementation of **"Direct Preference Optimization: Your Language
-Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code]
-(https://github.com/eric-mitchell/direct-preference-optimization)] ## Citation
-```bibtex @misc{vonwerra2022trl, author = {Leandro von Werra and Younes Belkada
-and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert
-and Shengyi Huang}, title = {TRL: Transformer Reinforcement Learning}, year =
-{2020}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/huggingface/trl}} } ```
+Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://
+arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-
+preference-optimization)] ## Citation ```bibtex @misc{vonwerra2022trl, author =
+{Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching
+and Tristan Thrush and Nathan Lambert and Shengyi Huang}, title = {TRL:
+Transformer Reinforcement Learning}, year = {2020}, publisher = {GitHub},
+journal = {GitHub repository}, howpublished = {\url{https://github.com/
+huggingface/trl}} } ```
```

### Comparing `trl-0.8.1/README.md` & `trl-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ## Highlights
 
 - **`Efficient and scalable`**: 
     - [`accelerate`](https://github.com/huggingface/accelerate) is the backbone of `trl` which allows to scale model training from a single GPU to a large scale multi-node cluster with methods such as DDP and DeepSpeed.
     - [`PEFT`](https://github.com/huggingface/peft) is fully integrated and allows to train even the largest models on modest hardware with quantisation and methods such as LoRA or QLoRA.
     - [`unsloth`](https://github.com/unslothai/unsloth) is also integrated and allows to significantly speed up training with dedicated kernels.
 - **`CLI`**: With the [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with LLMs without writing any code using a single command and a flexible config system.
-- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer).
+- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.ORPOTrainer).
 - **`AutoModels`**: The [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForCausalLMWithValueHead) & [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value head to the model which allows to train them with RL algorithms such as PPO.
 - **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT sentiment classifier, full RLHF using adapters only, train GPT-j to be less toxic, [StackLlama example](https://huggingface.co/blog/stackllama), etc. following the [examples](https://github.com/huggingface/trl/tree/main/examples).
 
 ## Installation
 
 ### Python package
 Install the library with `pip`:
@@ -65,32 +65,32 @@
 ```bash
 trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --output_dir opt-sft-imdb
 ```
 
 **DPO:**
 
 ```bash
-trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-processed --output_dir opt-sft-hh-rlhf 
+trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --output_dir opt-sft-hh-rlhf 
 ```
 
 **Chat:**
 
 ```bash
 trl chat --model_name_or_path Qwen/Qwen1.5-0.5B-Chat
 ```
 
 Read more about CLI in the [relevant documentation section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more details.
 
 ## How to use
 
-For more flexibility and control over the training you can use the dedicated trainer classes to fine-tune the model in Python.
+For more flexibility and control over the training, you can use the dedicated trainer classes to fine-tune the model in Python.
 
 ### `SFTTrainer`
 
-This is a basic example on how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
+This is a basic example of how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
 
 ```python
 # imports
 from datasets import load_dataset
 from trl import SFTTrainer
 
 # get dataset
@@ -106,15 +106,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `RewardTrainer`
 
-This is a basic example on how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+This is a basic example of how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 from trl import RewardTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -132,15 +132,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `PPOTrainer`
 
-This is a basic example on how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
+This is a basic example of how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
 
 ```python
 # imports
 import torch
 from transformers import AutoTokenizer
 from trl import PPOTrainer, PPOConfig, AutoModelForCausalLMWithValueHead, create_reference_model
 from trl.core import respond_to_batch
@@ -171,15 +171,15 @@
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### `DPOTrainer`
 
-`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from trl import DPOTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -211,15 +211,15 @@
 
 ## References
 
 ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper **"Fine-Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper](https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-human-preferences)].
 
 ### Direct Preference Optimization
-DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
+DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
 
 
 ## Citation
 
 ```bibtex
 @misc{vonwerra2022trl,
   author = {Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert and Shengyi Huang},
```

#### html2text {}

```diff
@@ -19,16 +19,18 @@
 significantly speed up training with dedicated kernels. - **`CLI`**: With the
 [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with
 LLMs without writing any code using a single command and a flexible config
 system. - **`Trainers`**: The Trainer classes are an abstraction to apply many
 fine-tuning methods with ease such as the [`SFTTrainer`](https://
 huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/
 docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/
-docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/
-trainer#trl.PPOTrainer). - **`AutoModels`**: The
+docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.ORPOTrainer). - **`AutoModels`**: The
 [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForCausalLMWithValueHead) &
 [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value
 head to the model which allows to train them with RL algorithms such as PPO. -
 **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT
 sentiment classifier, full RLHF using adapters only, train GPT-j to be less
@@ -41,37 +43,37 @@
 want to use the examples you can clone the repository with the following
 command: ```bash git clone https://github.com/huggingface/trl.git ``` ##
 Command Line Interface (CLI) You can use TRL Command Line Interface (CLI) to
 quickly get started with Supervised Fine-tuning (SFT), Direct Preference
 Optimization (DPO) and test your aligned model with the chat CLI: **SFT:**
 ```bash trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --
 output_dir opt-sft-imdb ``` **DPO:** ```bash trl dpo --model_name_or_path
-facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-
-processed --output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --
-model_name_or_path Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the
-[relevant documentation section](https://huggingface.co/docs/trl/main/en/clis)
-or use `--help` for more details. ## How to use For more flexibility and
-control over the training you can use the dedicated trainer classes to fine-
-tune the model in Python. ### `SFTTrainer` This is a basic example on how to
-use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper
-around the `transformers` Trainer to easily fine-tune language models or
-adapters on a custom dataset. ```python # imports from datasets import
-load_dataset from trl import SFTTrainer # get dataset dataset = load_dataset
-("imdb", split="train") # get trainer trainer = SFTTrainer( "facebook/opt-
-350m", train_dataset=dataset, dataset_text_field="text", max_seq_length=512, )
-# train trainer.train() ``` ### `RewardTrainer` This is a basic example on how
-to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper
-around the `transformers` Trainer to easily fine-tune reward models or adapters
-on a custom preference dataset. ```python # imports from transformers import
+facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --
+output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --model_name_or_path
+Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the [relevant documentation
+section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more
+details. ## How to use For more flexibility and control over the training, you
+can use the dedicated trainer classes to fine-tune the model in Python. ###
+`SFTTrainer` This is a basic example of how to use the `SFTTrainer` from the
+library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer
+to easily fine-tune language models or adapters on a custom dataset. ```python
+# imports from datasets import load_dataset from trl import SFTTrainer # get
+dataset dataset = load_dataset("imdb", split="train") # get trainer trainer =
+SFTTrainer( "facebook/opt-350m", train_dataset=dataset,
+dataset_text_field="text", max_seq_length=512, ) # train trainer.train() ```
+### `RewardTrainer` This is a basic example of how to use the `RewardTrainer`
+from the library. The `RewardTrainer` is a wrapper around the `transformers`
+Trainer to easily fine-tune reward models or adapters on a custom preference
+dataset. ```python # imports from transformers import
 AutoModelForSequenceClassification, AutoTokenizer from trl import RewardTrainer
 # load model and dataset - dataset needs to be in a specific format model =
 AutoModelForSequenceClassification.from_pretrained("gpt2", num_labels=1)
 tokenizer = AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer =
 RewardTrainer( model=model, tokenizer=tokenizer, train_dataset=dataset, ) #
-train trainer.train() ``` ### `PPOTrainer` This is a basic example on how to
+train trainer.train() ``` ### `PPOTrainer` This is a basic example of how to
 use the `PPOTrainer` from the library. Based on a query the language model
 creates a response which is then evaluated. The evaluation could be a human in
 the loop or another model's output. ```python # imports import torch from
 transformers import AutoTokenizer from trl import PPOTrainer, PPOConfig,
 AutoModelForCausalLMWithValueHead, create_reference_model from trl.core import
 respond_to_batch # get models model =
 AutoModelForCausalLMWithValueHead.from_pretrained('gpt2') model_ref =
@@ -83,15 +85,15 @@
 (model, query_tensor) # create a ppo trainer ppo_trainer = PPOTrainer
 (ppo_config, model, model_ref, tokenizer) # define a reward for response #
 (this could be any reward such as human feedback or output from another model)
 reward = [torch.tensor(1.0)] # train model for one step with ppo train_stats =
 ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward) ``` ###
 `DPOTrainer` `DPOTrainer` is a trainer that uses [Direct Preference
 Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic
-example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
+example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
 wrapper around the `transformers` Trainer to easily fine-tune reward models or
 adapters on a custom preference dataset. ```python # imports from transformers
 import AutoModelForCausalLM, AutoTokenizer from trl import DPOTrainer # load
 model and dataset - dataset needs to be in a specific format model =
 AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer = DPOTrainer
 ( model=model, tokenizer=tokenizer, train_dataset=dataset, ) # train
@@ -101,14 +103,15 @@
 dev install: ```bash git clone https://github.com/huggingface/trl.git cd trl/
 make dev ``` ## References ### Proximal Policy Optimisation The PPO
 implementation largely follows the structure introduced in the paper **"Fine-
 Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper]
 (https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-
 human-preferences)]. ### Direct Preference Optimization DPO is based on the
 original implementation of **"Direct Preference Optimization: Your Language
-Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code]
-(https://github.com/eric-mitchell/direct-preference-optimization)] ## Citation
-```bibtex @misc{vonwerra2022trl, author = {Leandro von Werra and Younes Belkada
-and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert
-and Shengyi Huang}, title = {TRL: Transformer Reinforcement Learning}, year =
-{2020}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/huggingface/trl}} } ```
+Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://
+arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-
+preference-optimization)] ## Citation ```bibtex @misc{vonwerra2022trl, author =
+{Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching
+and Tristan Thrush and Nathan Lambert and Shengyi Huang}, title = {TRL:
+Transformer Reinforcement Learning}, year = {2020}, publisher = {GitHub},
+journal = {GitHub repository}, howpublished = {\url{https://github.com/
+huggingface/trl}} } ```
```

### Comparing `trl-0.8.1/examples/datasets/anthropic_hh.py` & `trl-0.8.2/examples/datasets/anthropic_hh.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/datasets/tldr_preference.py` & `trl-0.8.2/examples/datasets/tldr_preference.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/datasets/tokenize_ds.py` & `trl-0.8.2/examples/datasets/tokenize_ds.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/hello_world.py` & `trl-0.8.2/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/scripts/ddpo.py` & `trl-0.8.2/examples/scripts/ddpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/scripts/dpo.py` & `trl-0.8.2/examples/scripts/dpo.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 # regular:
 python examples/scripts/dpo.py \
+    --dataset_name=trl-internal-testing/hh-rlhf-trl-style \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
-    --max_steps 1000 \
     --learning_rate 1e-3 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
     --output_dir="dpo_anthropic_hh" \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns
 
 # peft:
 python examples/scripts/dpo.py \
+    --dataset_name=trl-internal-testing/hh-rlhf-trl-style \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
-    --max_steps 1000 \
     --learning_rate 1e-3 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
     --output_dir="dpo_anthropic_hh" \
     --optim rmsprop \
     --warmup_steps 150 \
@@ -46,14 +46,15 @@
     --logging_first_step \
     --no_remove_unused_columns \
     --use_peft \
     --lora_r=16 \
     --lora_alpha=16
 """
 import logging
+import multiprocessing
 import os
 from contextlib import nullcontext
 
 TRL_USE_RICH = os.environ.get("TRL_USE_RICH", False)
 
 from trl.commands.cli_utils import DpoScriptArguments, init_zero_verbose, TrlParser
 
@@ -114,14 +115,16 @@
     if peft_config is None:
         model_ref = AutoModelForCausalLM.from_pretrained(model_config.model_name_or_path, **model_kwargs)
     else:
         model_ref = None
     tokenizer = AutoTokenizer.from_pretrained(model_config.model_name_or_path)
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
+    if tokenizer.chat_template is None:
+        tokenizer.chat_template = "{% for message in messages %}{{message['role'] + ': ' + message['content'] + '\n\n'}}{% endfor %}{{ eos_token }}"
     if args.ignore_bias_buffers:
         # torch distributed hack
         model._ddp_params_and_buffers_to_ignore = [
             name for name, buffer in model.named_buffers() if buffer.dtype == torch.bool
         ]
 
     ################
@@ -133,16 +136,31 @@
         if not TRL_USE_RICH
         else console.status(f"[bold green]Training completed! Saving the model to {training_args.output_dir}")
     )
 
     ################
     # Dataset
     ################
-    train_dataset = load_dataset(args.dataset_name, split="train")
-    eval_dataset = load_dataset(args.dataset_name, split="test")
+    ds = load_dataset(args.dataset_name)
+    if args.sanity_check:
+        for key in ds:
+            ds[key] = ds[key].select(range(50))
+
+    def process(row):
+        row["chosen"] = tokenizer.apply_chat_template(row["chosen"], tokenize=False)
+        row["rejected"] = tokenizer.apply_chat_template(row["rejected"], tokenize=False)
+        return row
+
+    ds = ds.map(
+        process,
+        num_proc=multiprocessing.cpu_count(),
+        load_from_cache_file=False,
+    )
+    train_dataset = ds["train"]
+    eval_dataset = ds["test"]
 
     ################
     # Training
     ################
     with init_context:
         trainer = DPOTrainer(
             model,
```

### Comparing `trl-0.8.1/examples/scripts/kto.py` & `trl-0.8.2/trl/commands/scripts/cpo.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,146 +7,115 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """
-Run the KTO training script with the following command with some example arguments.
-In general, the optimal configuration for KTO will be similar to that of DPO:
+Run the CPO training script with the following command with some example arguments.
+In general, the optimal configuration for CPO will be similar to that of DPO:
 
 # regular:
-python examples/scripts/kto.py \
+python examples/scripts/cpo.py \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
     --max_steps 1000 \
-    --learning_rate 1e-3 \
+    --learning_rate 8e-6 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
-    --output_dir="kto_anthropic_hh" \
+    --output_dir="gpt2-aligned-cpo" \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns
 
 # peft:
-python examples/scripts/kto.py \
+python examples/scripts/cpo.py \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
     --max_steps 1000 \
-    --learning_rate 1e-3 \
+    --learning_rate 8e-5 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
-    --output_dir="kto_anthropic_hh" \
+    --output_dir="gpt2-lora-aligned-cpo" \
     --optim rmsprop \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns \
     --use_peft \
     --lora_r=16 \
     --lora_alpha=16
 """
 
+import multiprocessing
 from dataclasses import dataclass, field
-from typing import Optional
 
-from datasets import Dataset, load_dataset
+from datasets import load_dataset
 from transformers import AutoModelForCausalLM, AutoTokenizer, HfArgumentParser
 
-from trl import KTOConfig, KTOTrainer, ModelConfig, get_peft_config
+from trl import CPOConfig, CPOTrainer, ModelConfig, get_peft_config
 
 
-# Define and parse arguments.
 @dataclass
 class ScriptArguments:
-    """
-    The arguments for the KTO training script.
-    """
-
-    # debugging
-    sanity_check: Optional[bool] = field(default=True, metadata={"help": "only train on 1000 samples"})
-
-
-def extract_anthropic_prompt(prompt_and_response):
-    """Extract the anthropic prompt from a prompt and response pair."""
-    search_term = "\n\nAssistant:"
-    search_term_idx = prompt_and_response.rfind(search_term)
-
-    if search_term_idx == -1:
-        raise ValueError(f"Prompt and response does not contain '{search_term}'")
-
-    return prompt_and_response[: search_term_idx + len(search_term)]
-
-
-def get_hh(split: str, sanity_check: bool = False, silent: bool = False, cache_dir: str = None) -> Dataset:
-    """Load the Anthropic Helpful-Harmless dataset from Hugging Face and convert it to the necessary format.
-
-    The dataset is converted to a dictionary with the following structure:
-    {
-        'prompt': List[str],
-        'completion': List[str],
-        'label': List[bool],
-    }
-
-    Prompts should be structured as follows:
-      \n\nHuman: <prompt>\n\nAssistant:
-    Multiple turns are allowed, but the prompt should always start with \n\nHuman: and end with \n\nAssistant:.
-    """
-    dataset = load_dataset("Anthropic/hh-rlhf", split=split, cache_dir=cache_dir)
-    if sanity_check:
-        dataset = dataset.select(range(min(len(dataset), 1000)))
-
-    flat_data = {
-        "prompt": [],
-        "completion": [],
-        "label": [],
-    }
-    for sample in dataset:
-        prompt = extract_anthropic_prompt(sample["chosen"])
-        flat_data["prompt"].append(prompt)
-        flat_data["completion"].append(sample["chosen"][len(prompt) :])
-        flat_data["label"].append(True)
-        flat_data["prompt"].append(prompt)
-        flat_data["completion"].append(sample["rejected"][len(prompt) :])
-        flat_data["label"].append(False)
-
-    return dataset.from_dict(flat_data)
+    dataset: str = field(
+        default="trl-internal-testing/hh-rlhf-trl-style", metadata={"help": "The name of the dataset to use."}
+    )
 
 
 if __name__ == "__main__":
-    parser = HfArgumentParser((ScriptArguments, KTOConfig, ModelConfig))
-    script_args, kto_args, model_args = parser.parse_args_into_dataclasses()
+    parser = HfArgumentParser((ScriptArguments, CPOConfig, ModelConfig))
+    args, cpo_args, model_config = parser.parse_args_into_dataclasses()
 
-    # 1. load a pretrained model
-    model = AutoModelForCausalLM.from_pretrained(model_args.model_name_or_path)
-    model_ref = AutoModelForCausalLM.from_pretrained(model_args.model_name_or_path)
-
-    tokenizer = AutoTokenizer.from_pretrained(model_args.model_name_or_path)
+    ################
+    # Model & Tokenizer
+    ################
+    model = AutoModelForCausalLM.from_pretrained(model_config.model_name_or_path)
+    peft_config = get_peft_config(model_config)
+    tokenizer = AutoTokenizer.from_pretrained(model_config.model_name_or_path)
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
 
-    # 2. Load the Anthropic Helpful-Harmless dataset
-    train_dataset = get_hh("train", sanity_check=script_args.sanity_check)
-
-    # 3. Load evaluation dataset
-    eval_dataset = get_hh("test", sanity_check=script_args.sanity_check)
+    ################
+    # Dataset
+    ################
+    ds = load_dataset(args.dataset)
+    if cpo_args.debug:
+        for key in ds:
+            ds[key] = ds[key].select(range(50))
+    if tokenizer.chat_template is None:
+        tokenizer.chat_template = "{% if not add_generation_prompt is defined %}{% set add_generation_prompt = false %}{% endif %}{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}"
+
+    def process(row):
+        row["chosen"] = tokenizer.apply_chat_template(row["chosen"], tokenize=False)
+        row["rejected"] = tokenizer.apply_chat_template(row["rejected"], tokenize=False)
+        return row
+
+    ds = ds.map(
+        process,
+        num_proc=1 if cpo_args.debug else multiprocessing.cpu_count(),
+        load_from_cache_file=False,
+    )
+    train_dataset = ds["train"]
+    eval_dataset = ds["test"]
 
-    # 4. initialize the KTO trainer
-    kto_trainer = KTOTrainer(
+    ################
+    # Training
+    ################
+    trainer = CPOTrainer(
         model,
-        model_ref,
-        args=kto_args,
+        args=cpo_args,
         train_dataset=train_dataset,
         eval_dataset=eval_dataset,
         tokenizer=tokenizer,
-        peft_config=get_peft_config(model_args),
+        peft_config=get_peft_config(model_config),
     )
 
-    # 5. train
-    kto_trainer.train()
+    # train and save the model
+    trainer.train()
+    trainer.save_model(cpo_args.output_dir)
```

### Comparing `trl-0.8.1/examples/scripts/ppo.py` & `trl-0.8.2/examples/scripts/ppo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/scripts/ppo_multi_adapter.py` & `trl-0.8.2/examples/scripts/ppo_multi_adapter.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/scripts/reward_modeling.py` & `trl-0.8.2/examples/scripts/reward_modeling.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/examples/scripts/sft.py` & `trl-0.8.2/examples/scripts/sft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/setup.py` & `trl-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
    Then push the change with a message 'set dev version'
 """
 import os
 
 from setuptools import find_packages, setup
 
 
-__version__ = "0.8.1"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+__version__ = "0.8.2"  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
 
 REQUIRED_PKGS = [
     "torch>=1.4.0",
     "transformers>=4.31.0",
     "numpy>=1.18.2",
     "accelerate",
     "datasets",
```

### Comparing `trl-0.8.1/tests/slow/test_dpo_slow.py` & `trl-0.8.2/tests/slow/test_dpo_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/slow/test_sft_slow.py` & `trl-0.8.2/tests/slow/test_sft_slow.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/slow/testing_constants.py` & `trl-0.8.2/tests/slow/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_best_of_n_sampler.py` & `trl-0.8.2/tests/test_best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_cli.py` & `trl-0.8.2/tests/test_cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,13 +28,13 @@
         raise AssertionError("An error occured while running the CLI, please double check") from exc
 
 
 @unittest.skipIf(sys.platform.startswith("win"), "Skipping on Windows")
 def test_dpo_cli():
     try:
         subprocess.run(
-            "trl dpo --max_steps 1 --output_dir tmp-sft --model_name_or_path HuggingFaceM4/tiny-random-LlamaForCausalLM --dataset_name trl-internal-testing/Anthropic-hh-rlhf-processed --learning_rate 1e-4 --lr_scheduler_type cosine",
+            "trl dpo --max_steps 1 --output_dir tmp-sft --model_name_or_path HuggingFaceM4/tiny-random-LlamaForCausalLM --dataset_name trl-internal-testing/hh-rlhf-trl-style --learning_rate 1e-4 --lr_scheduler_type cosine --sanity_check",
             shell=True,
             check=True,
         )
     except BaseException as exc:
         raise AssertionError("An error occured while running the CLI, please double check") from exc
```

### Comparing `trl-0.8.1/tests/test_core.py` & `trl-0.8.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_data_collator_completion_only.py` & `trl-0.8.2/tests/test_data_collator_completion_only.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_dataset_formatting.py` & `trl-0.8.2/tests/test_dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_ddpo_trainer.py` & `trl-0.8.2/tests/test_ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_dpo_trainer.py` & `trl-0.8.2/tests/test_dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_environments.py` & `trl-0.8.2/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_iterative_sft_trainer.py` & `trl-0.8.2/tests/test_iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_kto_trainer.py` & `trl-0.8.2/tests/test_kto_trainer.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import torch
 from datasets import Dataset
 from parameterized import parameterized
 from pytest import mark
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoTokenizer
 
 from trl import KTOConfig, KTOTrainer
+from trl.trainer.kto_trainer import _get_kl_dataset, _process_tokens, _tokenize
 
 from .testing_utils import require_no_wandb, require_peft
 
 
 class KTOTrainerTester(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
@@ -127,15 +128,15 @@
             # check the params have changed
             for n, param in previous_trainable_params.items():
                 new_param = trainer.model.get_parameter(n)
                 # check the params have changed - ignore 0 biases
                 if param.sum() != 0:
                     self.assertFalse(torch.equal(param, new_param))
 
-    def test_kto_trainer_tokenize_row(self):
+    def test_tokenize_and_process_tokens(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             training_args = KTOConfig(
                 output_dir=tmp_dir,
                 per_device_train_batch_size=2,
                 max_steps=3,
                 remove_unused_columns=False,
                 gradient_accumulation_steps=1,
@@ -151,24 +152,70 @@
                 ref_model=self.ref_model,
                 args=training_args,
                 tokenizer=self.tokenizer,
                 train_dataset=dummy_dataset,
                 eval_dataset=dummy_dataset,
             )
 
-            row = dummy_dataset[0]
-
-            # test that the row can be tokenized
-            tokenized_row = trainer.tokenize_row(row)
-
-            # Assert bos_token_id and eos_token_id (latter only for completion)
-            assert tokenized_row["prompt_input_ids"][0] == self.tokenizer.bos_token_id
-            assert tokenized_row["completion_input_ids"][0] == self.tokenizer.bos_token_id
-            assert tokenized_row["prompt_input_ids"][-1] != self.tokenizer.eos_token_id
-            assert tokenized_row["completion_input_ids"][-1] == self.tokenizer.eos_token_id
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                tokenized_dataset = dummy_dataset.map(
+                    _tokenize,
+                    fn_kwargs={"tokenizer": trainer.tokenizer},
+                    batched=True,
+                    batch_size=2,
+                )
+                self.assertListEqual(tokenized_dataset["prompt"], dummy_dataset["prompt"])
+                self.assertListEqual(tokenized_dataset["completion"], dummy_dataset["completion"])
+                self.assertListEqual(tokenized_dataset["label"], dummy_dataset["label"])
+                self.assertListEqual(tokenized_dataset["prompt_input_ids"][0], [10814, 11])
+                self.assertListEqual(tokenized_dataset["prompt_attention_mask"][0], [1, 1])
+                self.assertListEqual(tokenized_dataset["answer_input_ids"][0], [5968, 1219, 72, 3621, 284, 1826, 345])
+                self.assertListEqual(tokenized_dataset["answer_attention_mask"][0], [1, 1, 1, 1, 1, 1, 1])
+
+                # Test reversal of (prompt, completion) pairs for KL dataset
+                tokenized_kl_dataset = tokenized_dataset.map(_get_kl_dataset, batched=True, batch_size=2)
+                self.assertListEqual(
+                    tokenized_kl_dataset["prompt_input_ids"][0], tokenized_dataset["prompt_input_ids"][0]
+                )
+                self.assertListEqual(
+                    tokenized_kl_dataset["prompt_attention_mask"][0], tokenized_dataset["prompt_attention_mask"][0]
+                )
+                self.assertListEqual(
+                    tokenized_kl_dataset["answer_input_ids"][0], tokenized_dataset["answer_input_ids"][1]
+                )
+                self.assertListEqual(
+                    tokenized_kl_dataset["answer_attention_mask"][0], tokenized_dataset["answer_attention_mask"][1]
+                )
+
+                fn_kwargs = {
+                    "prefix": "",
+                    "is_encoder_decoder": trainer.is_encoder_decoder,
+                    "tokenizer": trainer.tokenizer,
+                    "max_length": trainer.max_length,
+                    "truncation_mode": trainer.truncation_mode,
+                    "label_pad_token_id": trainer.label_pad_token_id,
+                    "max_prompt_length": trainer.max_prompt_length,
+                }
+                processed_dataset = tokenized_dataset.map(_process_tokens, fn_kwargs=fn_kwargs, num_proc=2)
+                self.assertListEqual(processed_dataset["prompt"], dummy_dataset["prompt"])
+                self.assertListEqual(processed_dataset["completion"], dummy_dataset["completion"])
+                self.assertListEqual(processed_dataset["label"], dummy_dataset["label"])
+                self.assertListEqual(processed_dataset["prompt_input_ids"][0], [50256, 10814, 11])
+                self.assertListEqual(processed_dataset["prompt_attention_mask"][0], [1, 1, 1])
+                self.assertListEqual(
+                    processed_dataset["completion_input_ids"][0],
+                    [50256, 10814, 11, 5968, 1219, 72, 3621, 284, 1826, 345, 50256],
+                )
+                self.assertListEqual(
+                    processed_dataset["completion_attention_mask"][0], [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1]
+                )
+                self.assertListEqual(
+                    processed_dataset["completion_labels"][0],
+                    [-100, -100, -100, 5968, 1219, 72, 3621, 284, 1826, 345, 50256],
+                )
 
     def test_kto_trainer_without_providing_ref_model(self):
         with tempfile.TemporaryDirectory() as tmp_dir:
             training_args = KTOConfig(
                 output_dir=tmp_dir,
                 per_device_train_batch_size=2,
                 max_steps=3,
```

### Comparing `trl-0.8.1/tests/test_modeling_value_head.py` & `trl-0.8.2/tests/test_modeling_value_head.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_no_peft.py` & `trl-0.8.2/tests/test_no_peft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_peft_models.py` & `trl-0.8.2/tests/test_peft_models.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_ppo_trainer.py` & `trl-0.8.2/tests/test_ppo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/test_reward_trainer.py` & `trl-0.8.2/tests/test_reward_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,16 @@
                     assert not torch.equal(param, new_param)
 
             preds = trainer.predict(dummy_dataset)
             assert preds.predictions.shape == (4, 2)
 
     @require_peft
     def test_reward_trainer_peft(self):
-        import peft
         from peft import LoraConfig, TaskType
 
-        peft_version = peft.__version__
-
         peft_config = LoraConfig(
             task_type=TaskType.SEQ_CLS,
             inference_mode=False,
             r=8,
             lora_alpha=32,
             lora_dropout=0.1,
         )
@@ -168,15 +165,15 @@
                 eval_dataset=dummy_dataset,
                 peft_config=peft_config,
             )
             previous_trainable_params = {}
             previous_non_trainable_params = {}
 
             # due to a change in the way the modules to save are dealt in PEFT.
-            trainable_params_name = ["lora", "score"] if peft_version < "0.3.0" else ["lora", "modules_to_save"]
+            trainable_params_name = ["lora", "modules_to_save"]
 
             # check gradients are not None
             for n, param in trainer.model.named_parameters():
                 if any(t in n for t in trainable_params_name):
                     previous_trainable_params[n] = param.clone()
                 else:
                     previous_non_trainable_params[n] = param.clone()
```

### Comparing `trl-0.8.1/tests/test_sft_trainer.py` & `trl-0.8.2/tests/test_sft_trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,22 +15,28 @@
 import os
 import tempfile
 import unittest
 
 import numpy as np
 import pytest
 import torch
-from datasets import Dataset
-from transformers import AutoModelForCausalLM, AutoTokenizer, TrainingArguments
+from datasets import Dataset, Image, Sequence
+from transformers import (
+    AutoModelForCausalLM,
+    AutoProcessor,
+    AutoTokenizer,
+    LlavaForConditionalGeneration,
+    TrainingArguments,
+)
 
 from trl import SFTTrainer
-from trl.import_utils import is_peft_available
+from trl.import_utils import is_peft_available, is_pil_available
 from trl.trainer import ConstantLengthDataset, DataCollatorForCompletionOnlyLM
 
-from .testing_utils import require_peft
+from .testing_utils import require_peft, requires_pil
 
 
 def formatting_prompts_func(example):
     text = f"### Question: {example['question']}\n ### Answer: {example['answer']}"
     return text
 
 
@@ -41,14 +47,17 @@
         output_text.append(text)
     return output_text
 
 
 if is_peft_available():
     from peft import LoraConfig, PeftModel
 
+if is_pil_available():
+    from PIL import Image as PILImage
+
 
 class SFTTrainerTester(unittest.TestCase):
     r""" """
 
     @classmethod
     def setUpClass(cls):
         cls.model_id = "trl-internal-testing/dummy-GPT2-correct-vocab"
@@ -119,14 +128,57 @@
                 {"prompt": "What is 4+4?", "completion": "8"},
                 {"prompt": "What is 2+2?", "completion": "4"},
                 {"prompt": "What is 3+3?", "completion": "6"},
                 {"prompt": "What is 4+4?", "completion": "8"},
             ]
         )
 
+        if is_pil_available():
+            cls.dummy_vsft_instruction_dataset = Dataset.from_dict(
+                {
+                    "messages": [
+                        [
+                            {
+                                "role": "user",
+                                "content": [{"type": "text", "text": "What is in this image?"}, {"type": "image"}],
+                            },
+                            {
+                                "role": "assistant",
+                                "content": [{"type": "text", "text": "It is random noise."}],
+                            },
+                            {
+                                "role": "user",
+                                "content": [{"type": "text", "text": "Oh ye, you are right, what is 1+1"}],
+                            },
+                            {
+                                "role": "assistant",
+                                "content": [{"type": "text", "text": "2"}],
+                            },
+                        ],
+                        [
+                            {
+                                "role": "user",
+                                "content": [{"type": "text", "text": "What is in this image?"}, {"type": "image"}],
+                            },
+                            {
+                                "role": "assistant",
+                                "content": [{"type": "text", "text": "It is random noise."}],
+                            },
+                        ],
+                    ],
+                    "images": [
+                        [PILImage.fromarray((np.random.rand(40, 50, 3) * 255).astype("uint8")).convert("RGBA")],
+                        [PILImage.fromarray((np.random.rand(50, 60, 3) * 255).astype("uint8")).convert("RGBA")],
+                    ],
+                }
+            )
+            cls.dummy_vsft_instruction_dataset = cls.dummy_vsft_instruction_dataset.cast_column(
+                "images", Sequence(Image())
+            )
+
         cls.train_dataset = ConstantLengthDataset(
             cls.tokenizer,
             cls.dummy_dataset,
             dataset_text_field=None,
             formatting_func=formatting_prompts_func,
             seq_length=16,
             num_of_sequences=16,
@@ -976,7 +1028,99 @@
                 eval_dataset=self.dummy_chatml_dataset,
                 max_seq_length=32,  # make sure there is at least 1 packed sequence
                 packing=False,
             )
 
             assert len(trainer.train_dataset["input_ids"]) != 1
             assert len(trainer.eval_dataset["input_ids"]) != 1
+
+    @requires_pil
+    def test_sft_trainer_skip_prepare_dataset(self):
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            training_args = TrainingArguments(
+                output_dir=tmp_dir,
+                dataloader_drop_last=True,
+                evaluation_strategy="steps",
+                max_steps=4,
+                eval_steps=2,
+                save_steps=2,
+                per_device_train_batch_size=2,
+                gradient_checkpointing=True,
+                remove_unused_columns=False,
+            )
+
+            trainer = SFTTrainer(
+                model=self.model_id,
+                args=training_args,
+                train_dataset=self.dummy_vsft_instruction_dataset,
+                eval_dataset=self.dummy_vsft_instruction_dataset,
+                dataset_text_field="text",  # need a dummy field
+                dataset_kwargs={"skip_prepare_dataset": True},
+            )
+            assert trainer.train_dataset.features == self.dummy_vsft_instruction_dataset.features
+            assert trainer.eval_dataset.features == self.dummy_vsft_instruction_dataset.features
+
+    @requires_pil
+    def test_sft_trainer_llava(self):
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            training_args = TrainingArguments(
+                output_dir=tmp_dir,
+                dataloader_drop_last=True,
+                evaluation_strategy="steps",
+                max_steps=4,
+                eval_steps=2,
+                save_steps=2,
+                per_device_train_batch_size=2,
+                per_device_eval_batch_size=2,
+                remove_unused_columns=False,
+            )
+            tiny_llava = LlavaForConditionalGeneration.from_pretrained(
+                "trl-internal-testing/tiny-random-LlavaForConditionalGeneration"
+            )
+            processor = AutoProcessor.from_pretrained("trl-internal-testing/tiny-random-LlavaForConditionalGeneration")
+
+            processor.tokenizer.chat_template = """A chat between a curious user and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the user's questions. {% for message in messages %}{% if message['role'] == 'user' %}USER: {% else %}ASSISTANT: {% endif %}{% for item in message['content'] %}{% if item['type'] == 'text' %}{{ item['text'] }}{% elif item['type'] == 'image' %}<image>{% endif %}{% endfor %}{% if message['role'] == 'user' %} {% else %}{{eos_token}}{% endif %}{% endfor %}"""
+
+            class LLavaDataCollator:
+                def __init__(self, processor):
+                    self.processor = processor
+
+                def __call__(self, examples):
+                    texts = []
+                    images = []
+                    for example in examples:
+                        if len(example["images"]) > 1:
+                            raise ValueError("This collator only supports one image per example")
+                        messages = example["messages"]
+                        text = self.processor.tokenizer.apply_chat_template(
+                            messages, tokenize=False, add_generation_prompt=False
+                        )
+                        texts.append(text)
+                        images.append(example["images"][0])
+
+                    batch = self.processor(texts, images, return_tensors="pt", padding=True)
+
+                    labels = batch["input_ids"].clone()
+                    if self.processor.tokenizer.pad_token_id is not None:
+                        labels[labels == self.processor.tokenizer.pad_token_id] = -100
+                    batch["labels"] = labels
+
+                    return batch
+
+            data_collator = LLavaDataCollator(processor)
+
+            trainer = SFTTrainer(
+                model=tiny_llava,
+                args=training_args,
+                train_dataset=self.dummy_vsft_instruction_dataset,
+                eval_dataset=self.dummy_vsft_instruction_dataset,
+                dataset_text_field="text",  # need a dummy field
+                dataset_kwargs={"skip_prepare_dataset": True},
+                data_collator=data_collator,
+            )
+
+            trainer.train()
+
+            assert trainer.state.log_history[(-1)]["train_loss"] is not None
+            assert trainer.state.log_history[0]["eval_loss"] is not None
+
+            assert "model.safetensors" in os.listdir(tmp_dir + "/checkpoint-2")
```

### Comparing `trl-0.8.1/tests/testing_constants.py` & `trl-0.8.2/tests/testing_constants.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/tests/testing_utils.py` & `trl-0.8.2/tests/testing_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import torch
 
 from trl import (
     is_bitsandbytes_available,
     is_diffusers_available,
     is_peft_available,
+    is_pil_available,
     is_wandb_available,
     is_xpu_available,
 )
 
 
 def require_peft(test_case):
     """
@@ -47,14 +48,23 @@
     Decorator marking a test that requires diffusers. Skips the test if diffusers is not available.
     """
     if not is_diffusers_available():
         test_case = unittest.skip("test requires diffusers")(test_case)
     return test_case
 
 
+def requires_pil(test_case):
+    """
+    Decorator marking a test that requires PIL. Skips the test if pil is not available.
+    """
+    if not is_pil_available():
+        test_case = unittest.skip("test requires PIL")(test_case)
+    return test_case
+
+
 def require_wandb(test_case, required: bool = True):
     """
     Decorator marking a test that requires wandb. Skips the test if wandb is not available.
     """
     # XOR, i.e.:
     # skip if available and required = False and
     # skip if not available and required = True
```

### Comparing `trl-0.8.1/trl/__init__.py` & `trl-0.8.2/trl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # flake8: noqa
 
-__version__ = "0.8.1"
+__version__ = "0.8.2"
 
 from typing import TYPE_CHECKING
 from .import_utils import _LazyModule, is_diffusers_available, OptionalDependencyNotAvailable
 
 _import_structure = {
     "core": [
         "set_seed",
@@ -17,32 +17,37 @@
         "BestOfNSampler",
     ],
     "import_utils": [
         "is_bitsandbytes_available",
         "is_diffusers_available",
         "is_npu_available",
         "is_peft_available",
+        "is_pil_available",
         "is_wandb_available",
         "is_xpu_available",
     ],
     "models": [
         "AutoModelForCausalLMWithValueHead",
         "AutoModelForSeq2SeqLMWithValueHead",
         "PreTrainedModelWrapper",
         "create_reference_model",
         "setup_chat_format",
         "SUPPORTED_ARCHITECTURES",
     ],
     "trainer": [
         "DataCollatorForCompletionOnlyLM",
         "DPOTrainer",
+        "CPOConfig",
+        "CPOTrainer",
         "IterativeSFTTrainer",
         "KTOConfig",
         "KTOTrainer",
         "ModelConfig",
+        "ORPOConfig",
+        "ORPOTrainer",
         "PPOConfig",
         "PPOTrainer",
         "RewardConfig",
         "RewardTrainer",
         "SFTTrainer",
     ],
     "commands": [],
@@ -76,32 +81,37 @@
     from .environment import TextEnvironment, TextHistory
     from .extras import BestOfNSampler
     from .import_utils import (
         is_bitsandbytes_available,
         is_diffusers_available,
         is_npu_available,
         is_peft_available,
+        is_pil_available,
         is_wandb_available,
         is_xpu_available,
     )
     from .models import (
         AutoModelForCausalLMWithValueHead,
         AutoModelForSeq2SeqLMWithValueHead,
         PreTrainedModelWrapper,
         create_reference_model,
         setup_chat_format,
         SUPPORTED_ARCHITECTURES,
     )
     from .trainer import (
         DataCollatorForCompletionOnlyLM,
         DPOTrainer,
+        CPOConfig,
+        CPOTrainer,
         IterativeSFTTrainer,
         KTOConfig,
         KTOTrainer,
         ModelConfig,
+        ORPOConfig,
+        ORPOTrainer,
         PPOConfig,
         PPOTrainer,
         RewardConfig,
         RewardTrainer,
         SFTTrainer,
     )
     from .trainer.utils import get_kbit_device_map, get_peft_config, get_quantization_config, RichProgressCallback
```

### Comparing `trl-0.8.1/trl/commands/__init__.py` & `trl-0.8.2/trl/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/cli.py` & `trl-0.8.2/trl/commands/cli.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/cli_utils.py` & `trl-0.8.2/trl/commands/cli_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     dataset_name: str = field(default=None, metadata={"help": "the dataset name"})
     beta: float = field(default=0.1, metadata={"help": "the beta parameter for DPO loss"})
     max_length: int = field(default=512, metadata={"help": "max length of each sample"})
     max_prompt_length: int = field(default=128, metadata={"help": "max length of each sample's prompt"})
     max_target_length: int = field(
         default=128, metadata={"help": "Only used for encoder decoder model. Max target of each sample's prompt"}
     )
-    sanity_check: bool = field(default=True, metadata={"help": "only train on 1000 samples"})
+    sanity_check: bool = field(default=False, metadata={"help": "only train on 1000 samples"})
     ignore_bias_buffers: bool = field(
         default=False,
         metadata={
             "help": "debug argument for distributed training;"
             "fix for DDP issues with LM bias/mask buffers - invalid scalar type,`inplace operation. See"
             "https://github.com/huggingface/transformers/issues/22482#issuecomment-1595790992"
         },
```

### Comparing `trl-0.8.1/trl/commands/scripts/chat.py` & `trl-0.8.2/trl/commands/scripts/chat.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/scripts/ddpo.py` & `trl-0.8.2/trl/commands/scripts/ddpo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/scripts/dpo.py` & `trl-0.8.2/trl/commands/scripts/dpo.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 # regular:
 python examples/scripts/dpo.py \
+    --dataset_name=trl-internal-testing/hh-rlhf-trl-style \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
-    --max_steps 1000 \
     --learning_rate 1e-3 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
     --output_dir="dpo_anthropic_hh" \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns
 
 # peft:
 python examples/scripts/dpo.py \
+    --dataset_name=trl-internal-testing/hh-rlhf-trl-style \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
-    --max_steps 1000 \
     --learning_rate 1e-3 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
     --output_dir="dpo_anthropic_hh" \
     --optim rmsprop \
     --warmup_steps 150 \
@@ -46,14 +46,15 @@
     --logging_first_step \
     --no_remove_unused_columns \
     --use_peft \
     --lora_r=16 \
     --lora_alpha=16
 """
 import logging
+import multiprocessing
 import os
 from contextlib import nullcontext
 
 TRL_USE_RICH = os.environ.get("TRL_USE_RICH", False)
 
 from trl.commands.cli_utils import DpoScriptArguments, init_zero_verbose, TrlParser
 
@@ -114,14 +115,16 @@
     if peft_config is None:
         model_ref = AutoModelForCausalLM.from_pretrained(model_config.model_name_or_path, **model_kwargs)
     else:
         model_ref = None
     tokenizer = AutoTokenizer.from_pretrained(model_config.model_name_or_path)
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
+    if tokenizer.chat_template is None:
+        tokenizer.chat_template = "{% for message in messages %}{{message['role'] + ': ' + message['content'] + '\n\n'}}{% endfor %}{{ eos_token }}"
     if args.ignore_bias_buffers:
         # torch distributed hack
         model._ddp_params_and_buffers_to_ignore = [
             name for name, buffer in model.named_buffers() if buffer.dtype == torch.bool
         ]
 
     ################
@@ -133,16 +136,31 @@
         if not TRL_USE_RICH
         else console.status(f"[bold green]Training completed! Saving the model to {training_args.output_dir}")
     )
 
     ################
     # Dataset
     ################
-    train_dataset = load_dataset(args.dataset_name, split="train")
-    eval_dataset = load_dataset(args.dataset_name, split="test")
+    ds = load_dataset(args.dataset_name)
+    if args.sanity_check:
+        for key in ds:
+            ds[key] = ds[key].select(range(50))
+
+    def process(row):
+        row["chosen"] = tokenizer.apply_chat_template(row["chosen"], tokenize=False)
+        row["rejected"] = tokenizer.apply_chat_template(row["rejected"], tokenize=False)
+        return row
+
+    ds = ds.map(
+        process,
+        num_proc=multiprocessing.cpu_count(),
+        load_from_cache_file=False,
+    )
+    train_dataset = ds["train"]
+    eval_dataset = ds["test"]
 
     ################
     # Training
     ################
     with init_context:
         trainer = DPOTrainer(
             model,
```

### Comparing `trl-0.8.1/trl/commands/scripts/kto.py` & `trl-0.8.2/trl/commands/scripts/orpo.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,146 +7,115 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """
-Run the KTO training script with the following command with some example arguments.
-In general, the optimal configuration for KTO will be similar to that of DPO:
+Run the ORPO training script with the following command with some example arguments.
+In general, the optimal configuration for ORPO will be similar to that of DPO without the need for a reference model:
 
 # regular:
-python examples/scripts/kto.py \
+python examples/scripts/orpo.py \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
     --max_steps 1000 \
-    --learning_rate 1e-3 \
+    --learning_rate 8e-6 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
-    --output_dir="kto_anthropic_hh" \
+    --output_dir="gpt2-aligned-orpo" \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns
 
 # peft:
-python examples/scripts/kto.py \
+python examples/scripts/orpo.py \
     --model_name_or_path=gpt2 \
     --per_device_train_batch_size 4 \
     --max_steps 1000 \
-    --learning_rate 1e-3 \
+    --learning_rate 8e-5 \
     --gradient_accumulation_steps 1 \
     --logging_steps 10 \
     --eval_steps 500 \
-    --output_dir="kto_anthropic_hh" \
+    --output_dir="gpt2-lora-aligned-orpo" \
     --optim rmsprop \
     --warmup_steps 150 \
     --report_to wandb \
     --bf16 \
     --logging_first_step \
     --no_remove_unused_columns \
     --use_peft \
     --lora_r=16 \
     --lora_alpha=16
 """
 
+import multiprocessing
 from dataclasses import dataclass, field
-from typing import Optional
 
-from datasets import Dataset, load_dataset
+from datasets import load_dataset
 from transformers import AutoModelForCausalLM, AutoTokenizer, HfArgumentParser
 
-from trl import KTOConfig, KTOTrainer, ModelConfig, get_peft_config
+from trl import ModelConfig, ORPOConfig, ORPOTrainer, get_peft_config
 
 
-# Define and parse arguments.
 @dataclass
 class ScriptArguments:
-    """
-    The arguments for the KTO training script.
-    """
-
-    # debugging
-    sanity_check: Optional[bool] = field(default=True, metadata={"help": "only train on 1000 samples"})
-
-
-def extract_anthropic_prompt(prompt_and_response):
-    """Extract the anthropic prompt from a prompt and response pair."""
-    search_term = "\n\nAssistant:"
-    search_term_idx = prompt_and_response.rfind(search_term)
-
-    if search_term_idx == -1:
-        raise ValueError(f"Prompt and response does not contain '{search_term}'")
-
-    return prompt_and_response[: search_term_idx + len(search_term)]
-
-
-def get_hh(split: str, sanity_check: bool = False, silent: bool = False, cache_dir: str = None) -> Dataset:
-    """Load the Anthropic Helpful-Harmless dataset from Hugging Face and convert it to the necessary format.
-
-    The dataset is converted to a dictionary with the following structure:
-    {
-        'prompt': List[str],
-        'completion': List[str],
-        'label': List[bool],
-    }
-
-    Prompts should be structured as follows:
-      \n\nHuman: <prompt>\n\nAssistant:
-    Multiple turns are allowed, but the prompt should always start with \n\nHuman: and end with \n\nAssistant:.
-    """
-    dataset = load_dataset("Anthropic/hh-rlhf", split=split, cache_dir=cache_dir)
-    if sanity_check:
-        dataset = dataset.select(range(min(len(dataset), 1000)))
-
-    flat_data = {
-        "prompt": [],
-        "completion": [],
-        "label": [],
-    }
-    for sample in dataset:
-        prompt = extract_anthropic_prompt(sample["chosen"])
-        flat_data["prompt"].append(prompt)
-        flat_data["completion"].append(sample["chosen"][len(prompt) :])
-        flat_data["label"].append(True)
-        flat_data["prompt"].append(prompt)
-        flat_data["completion"].append(sample["rejected"][len(prompt) :])
-        flat_data["label"].append(False)
-
-    return dataset.from_dict(flat_data)
+    dataset: str = field(
+        default="trl-internal-testing/hh-rlhf-trl-style", metadata={"help": "The name of the dataset to use."}
+    )
 
 
 if __name__ == "__main__":
-    parser = HfArgumentParser((ScriptArguments, KTOConfig, ModelConfig))
-    script_args, kto_args, model_args = parser.parse_args_into_dataclasses()
+    parser = HfArgumentParser((ScriptArguments, ORPOConfig, ModelConfig))
+    args, orpo_args, model_config = parser.parse_args_into_dataclasses()
 
-    # 1. load a pretrained model
-    model = AutoModelForCausalLM.from_pretrained(model_args.model_name_or_path)
-    model_ref = AutoModelForCausalLM.from_pretrained(model_args.model_name_or_path)
-
-    tokenizer = AutoTokenizer.from_pretrained(model_args.model_name_or_path)
+    ################
+    # Model & Tokenizer
+    ################
+    model = AutoModelForCausalLM.from_pretrained(model_config.model_name_or_path)
+    peft_config = get_peft_config(model_config)
+    tokenizer = AutoTokenizer.from_pretrained(model_config.model_name_or_path)
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
 
-    # 2. Load the Anthropic Helpful-Harmless dataset
-    train_dataset = get_hh("train", sanity_check=script_args.sanity_check)
-
-    # 3. Load evaluation dataset
-    eval_dataset = get_hh("test", sanity_check=script_args.sanity_check)
+    ################
+    # Dataset
+    ################
+    ds = load_dataset(args.dataset)
+    if orpo_args.debug:
+        for key in ds:
+            ds[key] = ds[key].select(range(50))
+    if tokenizer.chat_template is None:
+        tokenizer.chat_template = "{% if not add_generation_prompt is defined %}{% set add_generation_prompt = false %}{% endif %}{% for message in messages %}{{'<|im_start|>' + message['role'] + '\n' + message['content'] + '<|im_end|>' + '\n'}}{% endfor %}{% if add_generation_prompt %}{{ '<|im_start|>assistant\n' }}{% endif %}"
+
+    def process(row):
+        row["chosen"] = tokenizer.apply_chat_template(row["chosen"], tokenize=False)
+        row["rejected"] = tokenizer.apply_chat_template(row["rejected"], tokenize=False)
+        return row
+
+    ds = ds.map(
+        process,
+        num_proc=1 if orpo_args.debug else multiprocessing.cpu_count(),
+        load_from_cache_file=False,
+    )
+    train_dataset = ds["train"]
+    eval_dataset = ds["test"]
 
-    # 4. initialize the KTO trainer
-    kto_trainer = KTOTrainer(
+    ################
+    # Training
+    ################
+    trainer = ORPOTrainer(
         model,
-        model_ref,
-        args=kto_args,
+        args=orpo_args,
         train_dataset=train_dataset,
         eval_dataset=eval_dataset,
         tokenizer=tokenizer,
-        peft_config=get_peft_config(model_args),
+        peft_config=get_peft_config(model_config),
     )
 
-    # 5. train
-    kto_trainer.train()
+    # train and save the model
+    trainer.train()
+    trainer.save_model(orpo_args.output_dir)
```

### Comparing `trl-0.8.1/trl/commands/scripts/ppo.py` & `trl-0.8.2/trl/commands/scripts/ppo.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/scripts/ppo_multi_adapter.py` & `trl-0.8.2/trl/commands/scripts/ppo_multi_adapter.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/scripts/reward_modeling.py` & `trl-0.8.2/trl/commands/scripts/reward_modeling.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/commands/scripts/sft.py` & `trl-0.8.2/trl/commands/scripts/sft.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/core.py` & `trl-0.8.2/trl/core.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/environment/base_environment.py` & `trl-0.8.2/trl/environment/base_environment.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/extras/__init__.py` & `trl-0.8.2/trl/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/extras/best_of_n_sampler.py` & `trl-0.8.2/trl/extras/best_of_n_sampler.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/extras/dataset_formatting.py` & `trl-0.8.2/trl/extras/dataset_formatting.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/import_utils.py` & `trl-0.8.2/trl/import_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,18 @@
     return torch_version >= "2.0"
 
 
 def is_diffusers_available() -> bool:
     return find_spec("diffusers") is not None
 
 
+def is_pil_available() -> bool:
+    return find_spec("PIL") is not None
+
+
 def is_bitsandbytes_available() -> bool:
     import torch
 
     # bnb can be imported without GPU but is not usable.
     return find_spec("bitsandbytes") is not None and torch.cuda.is_available()
```

### Comparing `trl-0.8.1/trl/models/__init__.py` & `trl-0.8.2/trl/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 _import_structure = {
     "modeling_base": ["PreTrainedModelWrapper", "create_reference_model"],
     "modeling_value_head": [
         "AutoModelForCausalLMWithValueHead",
         "AutoModelForSeq2SeqLMWithValueHead",
     ],
-    "utils": ["setup_chat_format", "SUPPORTED_ARCHITECTURES"],
+    "utils": ["setup_chat_format", "SUPPORTED_ARCHITECTURES", "unwrap_model_for_generation"],
 }
 
 try:
     if not is_diffusers_available():
         raise OptionalDependencyNotAvailable()
 except OptionalDependencyNotAvailable:
     pass
```

### Comparing `trl-0.8.1/trl/models/modeling_base.py` & `trl-0.8.2/trl/models/modeling_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/models/modeling_sd_base.py` & `trl-0.8.2/trl/models/modeling_sd_base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/models/modeling_value_head.py` & `trl-0.8.2/trl/models/modeling_value_head.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import torch
 import torch.nn as nn
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM
 
+from ..import_utils import is_npu_available, is_xpu_available
 from .modeling_base import PreTrainedModelWrapper
 
 
 class ValueHead(nn.Module):
     r"""
     The ValueHead class implements a head for GPT2 that returns a scalar for each output token.
     """
@@ -241,15 +242,21 @@
                 or "disk" in self.pretrained_model.hf_device_map.values()
             ):
                 raise ValueError(
                     "The model is offloaded on CPU or disk - CPU & disk offloading is not supported for ValueHead models."
                 )
 
             first_device = list(set(self.pretrained_model.hf_device_map.values()))[0]
-
+            if isinstance(first_device, int):
+                if is_npu_available():
+                    first_device = f"npu:{first_device}"
+                elif is_xpu_available():
+                    first_device = f"xpu:{first_device}"
+                else:
+                    first_device = f"cuda:{first_device}"
             self.v_head = self.v_head.to(first_device)
 
             def set_device_hook(module, input, outputs):
                 new_output = ()
                 for output in outputs:
                     if isinstance(output, torch.Tensor):
                         new_output += (output.to(first_device),)
```

### Comparing `trl-0.8.1/trl/models/sd_utils.py` & `trl-0.8.2/trl/models/sd_utils.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/__init__.py` & `trl-0.8.2/trl/trainer/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,20 +28,24 @@
         "disable_dropout_in_model",
         "peft_module_casting_to_bf16",
         "RichProgressCallback",
     ],
     "dpo_trainer": [
         "DPOTrainer",
     ],
+    "cpo_config": ["CPOConfig"],
+    "cpo_trainer": ["CPOTrainer"],
     "iterative_sft_trainer": [
         "IterativeSFTTrainer",
     ],
     "kto_config": ["KTOConfig"],
     "kto_trainer": ["KTOTrainer"],
     "model_config": ["ModelConfig"],
+    "orpo_config": ["ORPOConfig"],
+    "orpo_trainer": ["ORPOTrainer"],
     "ppo_config": ["PPOConfig"],
     "ppo_trainer": ["PPOTrainer"],
     "reward_config": ["RewardConfig"],
     "reward_trainer": ["RewardTrainer", "compute_accuracy"],
     "sft_trainer": ["SFTTrainer"],
     "base": ["BaseTrainer"],
     "ddpo_config": ["DDPOConfig"],
@@ -72,17 +76,21 @@
     # isort: on
 
     from .base import BaseTrainer
     from .ddpo_config import DDPOConfig
 
     from .dpo_trainer import DPOTrainer
     from .iterative_sft_trainer import IterativeSFTTrainer
+    from .cpo_config import CPOConfig
+    from .cpo_trainer import CPOTrainer
     from .kto_config import KTOConfig
     from .kto_trainer import KTOTrainer
     from .model_config import ModelConfig
+    from .orpo_config import ORPOConfig
+    from .orpo_trainer import ORPOTrainer
     from .ppo_config import PPOConfig
     from .ppo_trainer import PPOTrainer
     from .reward_config import RewardConfig
     from .reward_trainer import RewardTrainer, compute_accuracy
     from .sft_trainer import SFTTrainer
 
     try:
```

### Comparing `trl-0.8.1/trl/trainer/base.py` & `trl-0.8.2/trl/trainer/base.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/ddpo_config.py` & `trl-0.8.2/trl/trainer/ddpo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/ddpo_trainer.py` & `trl-0.8.2/trl/trainer/ddpo_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/dpo_trainer.py` & `trl-0.8.2/trl/trainer/dpo_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             # get peft model with the given config
             model = get_peft_model(model, peft_config)
             if args.bf16 and getattr(model, "is_loaded_in_4bit", False):
                 peft_module_casting_to_bf16(model)
                 # If args.bf16 we need to explicitly call `generate` with torch amp autocast context manager
                 self._peft_has_been_casted_to_bf16 = True
 
-        # For models that use gradient_checkpoiting, we need to attach a hook that enables input
+        # For models that use gradient_checkpointing, we need to attach a hook that enables input
         # to explicitly have `requires_grad=True`, otherwise training will either silently
         # fail or completely fail.
         elif getattr(args, "gradient_checkpointing", False):
             # For backward compatibility with older versions of transformers
             if hasattr(model, "enable_input_require_grads"):
                 model.enable_input_require_grads()
             else:
@@ -1088,15 +1088,15 @@
         if return_outputs:
             return (loss, metrics)
         return loss
 
     def get_batch_samples(self, model, batch: Dict[str, torch.LongTensor]) -> Tuple[str, str]:
         """Generate samples from the model and reference model for the given batch of inputs."""
 
-        # If one uses `generate_during_eval` with peft + bf16, we need to explictly call generate with
+        # If one uses `generate_during_eval` with peft + bf16, we need to explicitly call generate with
         # the torch cuda amp context manager as some hidden states are silently casted to full precision.
         generate_context_manager = nullcontext if not self._peft_has_been_casted_to_bf16 else torch.cuda.amp.autocast
 
         with generate_context_manager():
             policy_output = model.generate(
                 input_ids=batch["prompt_input_ids"],
                 attention_mask=batch["prompt_attention_mask"],
@@ -1244,13 +1244,13 @@
             logs[key] = torch.tensor(metrics).mean().item()
         del self._stored_metrics[train_eval]
         return super().log(logs)
 
     @wraps(Trainer.push_to_hub)
     def push_to_hub(self, commit_message: Optional[str] = "End of training", blocking: bool = True, **kwargs) -> str:
         """
-        Overwrite the `push_to_hub` method in order to force-add the tag "sft" when pushing the
+        Overwrite the `push_to_hub` method in order to force-add the tag "dpo" when pushing the
         model on the Hub. Please refer to `~transformers.Trainer.push_to_hub` for more details.
         """
         kwargs = trl_sanitze_kwargs_for_tagging(model=self.model, tag_names=self._tag_names, kwargs=kwargs)
 
         return super().push_to_hub(commit_message=commit_message, blocking=blocking, **kwargs)
```

### Comparing `trl-0.8.1/trl/trainer/iterative_sft_trainer.py` & `trl-0.8.2/trl/trainer/iterative_sft_trainer.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/kto_config.py` & `trl-0.8.2/trl/trainer/kto_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,16 @@
         precompute_ref_log_probs (`bool`, defaults to `False`):
             Flag to precompute reference model log probabilities for training and evaluation datasets. This is useful if you want to train
             without the reference model and reduce the total GPU memory needed.
         model_init_kwargs: (`Optional[Dict]`, *optional*):
             Dict of Optional kwargs to pass when instantiating the model from a string.
         ref_model_init_kwargs: (`Optional[Dict]`, *optional*):
             Dict of Optional kwargs to pass when instantiating the ref model from a string.
+        dataset_num_proc: (`Optional[int]`, *optional*, defaults to `None`):
+            Number of processes to use for processing the datasets.
     """
 
     max_length: Optional[int] = None
     """The maximum length of the sequences in the batch. This argument is required if you want to use the default data collator."""
     max_prompt_length: Optional[int] = None
     """The maximum length of the prompt. This argument is required if you want to use the default data collator."""
     max_completion_length: Optional[int] = None
@@ -75,7 +77,8 @@
     padding_value: int = None
     truncation_mode: str = "keep_end"
     generate_during_eval: bool = False
     is_encoder_decoder: Optional[bool] = None
     precompute_ref_log_probs: bool = False
     model_init_kwargs: Optional[Dict] = None
     ref_model_init_kwargs: Optional[Dict] = None
+    dataset_num_proc: Optional[int] = None
```

### Comparing `trl-0.8.1/trl/trainer/kto_trainer.py` & `trl-0.8.2/trl/trainer/kto_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 import random
 import warnings
 from collections import defaultdict
 from contextlib import nullcontext
 from copy import deepcopy
 from functools import wraps
 from operator import itemgetter
-from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+from accelerate import PartialState
 from accelerate.utils import is_deepspeed_available, tqdm
-from datasets import Dataset, concatenate_datasets, interleave_datasets
+from datasets import Dataset, concatenate_datasets
 from torch.utils.data import DataLoader, SequentialSampler
 from transformers import (
     AutoModelForCausalLM,
     DataCollator,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     Trainer,
@@ -58,14 +59,171 @@
 
 if is_wandb_available():
     import wandb
 
 if is_deepspeed_available():
     import deepspeed
 
+if TYPE_CHECKING:
+    from transformers import PreTrainedModel, PreTrainedTokenizer
+
+
+def _get_kl_dataset(batch: Dict[str, List[Any]]) -> Dict[str, List[Any]]:
+    """Creates mismatched pairs of prompts and completions for the KL dataset by reversing the order of completions."""
+    batch["answer_input_ids"] = batch["answer_input_ids"][::-1]
+    batch["answer_attention_mask"] = batch["answer_attention_mask"][::-1]
+    return batch
+
+
+def _tokenize(batch: Dict[str, List[Any]], tokenizer: "PreTrainedTokenizer") -> Dict[str, List[Any]]:
+    """Tokenize a batch from a KTO specific dataset."""
+    prompt_tokenized = tokenizer(batch["prompt"], add_special_tokens=False)
+    prompt_input_ids = prompt_tokenized["input_ids"]
+    prompt_attention_mask = prompt_tokenized["attention_mask"]
+    prompt_and_completion = [prompt + completion for prompt, completion in zip(batch["prompt"], batch["completion"])]
+    full_tokenized = tokenizer(prompt_and_completion, add_special_tokens=False)
+    full_input_ids = full_tokenized["input_ids"]
+    full_attention_mask = full_tokenized["attention_mask"]
+
+    answer_input_ids = [f[len(p) :] for f, p in zip(full_input_ids, prompt_input_ids)]
+    answer_attention_mask = [f[len(p) :] for f, p in zip(full_attention_mask, prompt_attention_mask)]
+
+    # Concat tokens to form `enc(a) + enc(a + b)[len(enc(a)):]`
+    full_concat_input_ids = [np.concatenate([p, a]) for p, a in zip(prompt_input_ids, answer_input_ids)]
+    # Prepare input tokens for token by token comparison
+    full_input_ids = [np.array(f) for f in full_input_ids]
+    for full, concat in zip(full_input_ids, full_concat_input_ids):
+        if len(full) != len(concat):
+            raise ValueError("Prompt input ids and answer input ids should have the same length.")
+
+    # On some tokenizers, like Llama-2 tokenizer, there are occasions where tokens
+    # can be merged together when tokenizing prompt+answer. This could result
+    # on the last token from the prompt being different when tokenized on its own
+    # vs when done as prompt+answer.
+    response_token_ids_start_idx = [len(p) for p in prompt_input_ids]
+
+    # If tokenized prompt is different than both prompt+answer, then it means the
+    # last token has changed due to merging.
+    for idx, (p, f, r) in enumerate(zip(prompt_input_ids, full_input_ids, response_token_ids_start_idx)):
+        if not np.array_equal(p, f[:r]):
+            response_token_ids_start_idx[idx] -= 1
+
+    prompt_input_ids = [f[:r] for f, r in zip(full_input_ids, response_token_ids_start_idx)]
+    prompt_attention_mask = [f[:r] for f, r in zip(full_attention_mask, response_token_ids_start_idx)]
+
+    for p, m in zip(prompt_input_ids, prompt_attention_mask):
+        if len(p) != len(m):
+            raise ValueError("Prompt input ids and attention mask should have the same length.")
+
+    answer_input_ids = [f[r:] for f, r in zip(full_input_ids, response_token_ids_start_idx)]
+    answer_attention_mask = [f[r:] for f, r in zip(full_attention_mask, response_token_ids_start_idx)]
+
+    return dict(
+        prompt_input_ids=prompt_input_ids,
+        prompt_attention_mask=prompt_attention_mask,
+        answer_input_ids=answer_input_ids,
+        answer_attention_mask=answer_attention_mask,
+    )
+
+
+def _process_tokens(example: Dict[str, Any], model: "PreTrainedModel" = None, **kwargs) -> Dict:
+    """Process tokens of a KTO specific dataset.
+
+    At this stage, we don't convert to PyTorch tensors yet; we just handle the truncation
+    in case the prompt + completion responses is/are too long. First
+        we truncate the prompt; if we're still too long, we truncate the completion.
+
+    We also create the labels for the completion responses, which are of length equal to
+        the sum of the length of the prompt and the completion response, with
+        label_pad_token_id  for the prompt tokens.
+    """
+    prompt = example["prompt"]
+    completion = example["completion"]
+
+    batch = {
+        f"{kwargs['prefix']}prompt": prompt,
+        f"{kwargs['prefix']}completion": completion,
+        f"{kwargs['prefix']}label": example["label"],
+    }
+
+    if not kwargs["is_encoder_decoder"]:
+        # Check issues below for more details
+        #  1. https://github.com/huggingface/trl/issues/907
+        #  2. https://github.com/EleutherAI/lm-evaluation-harness/pull/531#issuecomment-1595586257
+        #  3. https://github.com/LianjiaTech/BELLE/issues/337
+
+        if not isinstance(prompt, str):
+            raise ValueError(f"prompt should be an str but got {type(prompt)}")
+
+        if not isinstance(completion, str):
+            raise ValueError(f"completion should be an str but got {type(completion)}")
+
+        # keys of format prompt_* refers to just the prompt and answer_* refers to just the answer
+        all_tokens = {
+            "prompt_input_ids": example["prompt_input_ids"],
+            "prompt_attention_mask": example["prompt_attention_mask"],
+            "answer_input_ids": example["answer_input_ids"],
+            "answer_attention_mask": example["answer_attention_mask"],
+        }
+
+        max_length = kwargs["max_length"] - 2
+        # if combined sequence is too long (> max_length - 1 for BOS token - 1 for EOS), truncate the prompt
+        if len(all_tokens["prompt_input_ids"]) + len(all_tokens["answer_input_ids"]) > max_length:
+            for k in ["prompt_input_ids", "prompt_attention_mask"]:
+                if kwargs["truncation_mode"] == "keep_start":
+                    all_tokens[k] = all_tokens[k][: kwargs["max_prompt_length"]]
+                elif kwargs["truncation_mode"] == "keep_end":
+                    all_tokens[k] = all_tokens[k][-kwargs["max_prompt_length"] :]
+                else:
+                    raise ValueError(f"Unknown truncation mode: {kwargs['truncation_mode']}")
+
+        # if that's still too long, truncate the response
+        if len(all_tokens["prompt_input_ids"]) + len(all_tokens["answer_input_ids"]) > max_length:
+            for k in ["answer_input_ids", "answer_attention_mask"]:
+                all_tokens[k] = all_tokens[k][: max_length - kwargs["max_prompt_length"]]
+
+        # for legacy reasons, use the completion_* prefix to now refer to the joint sequence
+        batch[f"{kwargs['prefix']}prompt_input_ids"] = [kwargs["tokenizer"].bos_token_id] + all_tokens[
+            "prompt_input_ids"
+        ]
+        batch[f"{kwargs['prefix']}prompt_attention_mask"] = [1] + all_tokens["prompt_attention_mask"]
+        batch[f"{kwargs['prefix']}completion_input_ids"] = (
+            [kwargs["tokenizer"].bos_token_id]
+            + all_tokens["prompt_input_ids"]
+            + all_tokens["answer_input_ids"]
+            + [kwargs["tokenizer"].eos_token_id]
+        )
+        batch[f"{kwargs['prefix']}completion_attention_mask"] = (
+            [1] + all_tokens["prompt_attention_mask"] + all_tokens["answer_attention_mask"] + [1]
+        )
+
+        batch[f"{kwargs['prefix']}completion_labels"] = batch[f"{kwargs['prefix']}completion_input_ids"][:]
+        batch[f"{kwargs['prefix']}completion_labels"][: len(batch[f"{kwargs['prefix']}prompt_input_ids"])] = [
+            kwargs["label_pad_token_id"]
+        ] * len(batch[f"{kwargs['prefix']}prompt_input_ids"])
+    else:
+        completion_tokens = kwargs["tokenizer"](
+            completion, truncation=True, max_length=kwargs["max_completion_length"], add_special_tokens=True
+        )
+        prompt_tokens = kwargs["tokenizer"](
+            prompt, truncation=True, max_length=kwargs["max_prompt_length"], add_special_tokens=True
+        )
+
+        batch[f"{kwargs['prefix']}prompt_input_ids"] = prompt_tokens["input_ids"]
+        batch[f"{kwargs['prefix']}prompt_attention_mask"] = prompt_tokens["attention_mask"]
+
+        batch[f"{kwargs['prefix']}completion_labels"] = completion_tokens["input_ids"]
+        batch[f"{kwargs['prefix']}completion_attention_mask"] = completion_tokens["attention_mask"]
+        if model is not None and hasattr(model, "prepare_decoder_input_ids_from_labels"):
+            batch[f"{kwargs['prefix']}completion_decoder_input_ids"] = model.prepare_decoder_input_ids_from_labels(
+                labels=torch.tensor(batch["completion_labels"])
+            )
+
+    return batch
+
 
 class KTOTrainer(Trainer):
     r"""
     Initialize KTOTrainer.
 
     Args:
         model (`transformers.PreTrainedModel`):
@@ -322,93 +480,141 @@
         self._stored_metrics = defaultdict(lambda: defaultdict(list))
 
         # KTO parameter
         self.beta = args.beta
         self.desirable_weight = args.desirable_weight
         self.undesirable_weight = args.undesirable_weight
 
-        # get KL datasets
-        total_batch_size = (
-            max(torch.cuda.device_count(), 1) * args.per_device_train_batch_size * args.gradient_accumulation_steps
-        )
-        if total_batch_size <= 1:
-            raise ValueError(
-                "Batch size is 1 (too small). KTO will not work properly because the KL term will be equivalent to the implied reward."
+        with PartialState().local_main_process_first():
+            # Shuffle the datasets
+            train_dataset = train_dataset.shuffle(seed=args.data_seed)
+            if eval_dataset is not None:
+                eval_dataset = eval_dataset.shuffle(seed=args.data_seed)
+            # Tokenize and prepare the training datasets
+            train_dataset = train_dataset.map(
+                _tokenize,
+                fn_kwargs={"tokenizer": self.tokenizer},
+                batched=True,
+                desc="Tokenizing train dataset",
+            )
+            # Get KL datasets
+            total_batch_size = (
+                max(torch.cuda.device_count(), 1) * args.per_device_train_batch_size * args.gradient_accumulation_steps
             )
-        # note: for best results, mismatched outputs y' used to estimate the KL term for a batch should be the
-        # same as the matched outputs y used to estimate the rewards in that batch, just paired with different x
-        train_KL_dataset = train_dataset.map(self.get_KL_dataset, batched=True, batch_size=total_batch_size)
-        if eval_dataset is not None:
-            eval_KL_dataset = eval_dataset.map(self.get_KL_dataset, batched=True, batch_size=total_batch_size)
-
-        # tokenize the datasets
-        train_dataset = train_dataset.map(
-            lambda row: self.tokenize_row(row, prefix=""), remove_columns=train_dataset.column_names
-        )
-        train_KL_dataset = train_KL_dataset.map(
-            lambda row: self.tokenize_row(row, prefix="KL_"), remove_columns=train_KL_dataset.column_names
-        )
-        # merge the datasets
-        train_dataset = concatenate_datasets([train_dataset, train_KL_dataset], axis=1)
-
-        if eval_dataset is not None:
-            eval_dataset = eval_dataset.map(
-                lambda row: self.tokenize_row(row, prefix=""), remove_columns=eval_dataset.column_names
-            )
-            eval_KL_dataset = eval_KL_dataset.map(
-                lambda row: self.tokenize_row(row, prefix="KL_"), remove_columns=eval_KL_dataset.column_names
+            if total_batch_size <= 1:
+                raise ValueError(
+                    "Batch size is 1 (too small). KTO will not work properly because the KL term will be equivalent to the implied reward."
+                )
+            # create pairs for estimating the KL term by flipping the matched pairs in each batch of size total_batch_size
+            # i.e., (x_1, y_1), ..., (x_n, y_n) --> (x_1, y_n), ..., (x_n, y_1) = (x'_1, y'_1), ..., (x'_n, y'_n)
+            train_kl_dataset = train_dataset.map(
+                _get_kl_dataset, batched=True, batch_size=total_batch_size, desc="Extracting KL train dataset"
+            )
+            # Prepare the datasets
+            fn_kwargs = {
+                "prefix": "",
+                "is_encoder_decoder": self.is_encoder_decoder,
+                "tokenizer": self.tokenizer,
+                "max_length": self.max_length,
+                "truncation_mode": self.truncation_mode,
+                "label_pad_token_id": self.label_pad_token_id,
+                "max_prompt_length": self.max_prompt_length,
+            }
+            train_dataset = train_dataset.map(
+                _process_tokens,
+                fn_kwargs=fn_kwargs,
+                num_proc=args.dataset_num_proc,
+                desc="Processing tokenized train dataset",
+            )
+            fn_kwargs["prefix"] = "KL_"
+            train_kl_dataset = train_kl_dataset.map(
+                _process_tokens,
+                fn_kwargs=fn_kwargs,
+                num_proc=args.dataset_num_proc,
+                remove_columns=[c for c in train_kl_dataset.column_names if c in train_dataset.column_names],
+                desc="Processing tokenized train KL dataset",
             )
-            # merge the datasets
-            eval_dataset = concatenate_datasets([eval_dataset, eval_KL_dataset], axis=1)
-
-        desirable = train_dataset.filter(lambda x: x["label"])
-        undesirable = train_dataset.filter(lambda x: not x["label"])
 
-        if len(desirable) != len(undesirable):
-            # The lower and upper bounds come from Eq. (8) of https://arxiv.org/abs/2402.01306
-            des_weight_lower_bound = round((len(undesirable) * self.undesirable_weight / len(desirable)) * 1, 2)
-            des_weight_upper_bound = round((len(undesirable) * self.undesirable_weight / len(desirable)) * 1.33, 2)
-            und_weight_lower_bound = round((len(desirable) * self.desirable_weight / len(undesirable)) / 1.33, 2)
-            und_weight_upper_bound = round((len(desirable) * self.desirable_weight / len(undesirable)) / 1, 2)
-
-            des_weight_in_range = des_weight_lower_bound <= self.desirable_weight <= des_weight_upper_bound
-            und_weight_in_range = und_weight_lower_bound <= self.undesirable_weight <= und_weight_upper_bound
+            # merge the datasets
+            train_dataset = concatenate_datasets([train_dataset, train_kl_dataset], axis=1)
 
-            if not (des_weight_in_range or und_weight_in_range):
-                warnings.warn(
-                    f"""
-                    You have different amounts of desirable/positive and undesirable/negative examples but the
-                    weights on the desirable and undesirable losses don't seem to be in an ideal range. Based
-                    on your data, we recommend EITHER desirable_weight in [{des_weight_lower_bound}, {des_weight_upper_bound}]
-                    or undesirable_weight in [{und_weight_lower_bound}, {und_weight_upper_bound}] (but NOT BOTH).
-                    See the documentation on how to optimally set these weights.""",
-                    UserWarning,
+            if eval_dataset is not None:
+                # Tokenize
+                eval_dataset = eval_dataset.map(
+                    _tokenize,
+                    fn_kwargs={"tokenizer": self.tokenizer},
+                    batched=True,
+                    desc="Tokenizing eval dataset",
+                )
+                # Get KL dataset
+                eval_kl_dataset = eval_dataset.map(
+                    _get_kl_dataset, batched=True, batch_size=total_batch_size, desc="Extracting eval KL dataset"
+                )
+                # Process
+                fn_kwargs = {
+                    "prefix": "",
+                    "is_encoder_decoder": self.is_encoder_decoder,
+                    "tokenizer": self.tokenizer,
+                    "max_length": self.max_length,
+                    "truncation_mode": self.truncation_mode,
+                    "label_pad_token_id": self.label_pad_token_id,
+                    "max_prompt_length": self.max_prompt_length,
+                }
+                eval_dataset = eval_dataset.map(
+                    _process_tokens,
+                    fn_kwargs=fn_kwargs,
+                    num_proc=args.dataset_num_proc,
+                    desc="Processing tokenized eval dataset",
+                )
+                fn_kwargs["prefix"] = "KL_"
+                eval_kl_dataset = eval_kl_dataset.map(
+                    _process_tokens,
+                    fn_kwargs=fn_kwargs,
+                    num_proc=args.dataset_num_proc,
+                    remove_columns=[c for c in eval_kl_dataset.column_names if c in eval_dataset.column_names],
+                    desc="Processing tokenized eval KL dataset",
                 )
 
-        # split the dataset and interleave them together with equal probability of choosing chosen or rejected
-        interleaved_train_dataset = interleave_datasets(
-            [desirable, undesirable],
-            stopping_strategy="all_exhausted",
-        )
-        interleaved_train_dataset = interleaved_train_dataset.shuffle(seed=args.data_seed)
+                # merge the datasets
+                eval_dataset = concatenate_datasets([eval_dataset, eval_kl_dataset], axis=1)
 
-        if eval_dataset is not None:
-            interleaved_eval_dataset = interleave_datasets(
-                [eval_dataset.filter(lambda x: x["label"]), eval_dataset.filter(lambda x: not x["label"])],
-                stopping_strategy="all_exhausted",
+            desirable = train_dataset.filter(
+                lambda x: x["label"], num_proc=args.dataset_num_proc, desc="Filtering desirable examples"
+            )
+            undesirable = train_dataset.filter(
+                lambda x: not x["label"], num_proc=args.dataset_num_proc, desc="Filtering undesirable examples"
             )
-        else:
-            interleaved_eval_dataset = None
+
+            if len(desirable) != len(undesirable):
+                # The lower and upper bounds come from Eq. (8) of https://arxiv.org/abs/2402.01306
+                des_weight_lower_bound = round((len(undesirable) * self.undesirable_weight / len(desirable)) * 1, 2)
+                des_weight_upper_bound = round((len(undesirable) * self.undesirable_weight / len(desirable)) * 1.33, 2)
+                und_weight_lower_bound = round((len(desirable) * self.desirable_weight / len(undesirable)) / 1.33, 2)
+                und_weight_upper_bound = round((len(desirable) * self.desirable_weight / len(undesirable)) / 1, 2)
+
+                des_weight_in_range = des_weight_lower_bound <= self.desirable_weight <= des_weight_upper_bound
+                und_weight_in_range = und_weight_lower_bound <= self.undesirable_weight <= und_weight_upper_bound
+
+                if not (des_weight_in_range or und_weight_in_range):
+                    warnings.warn(
+                        f"""
+                        You have different amounts of desirable/positive and undesirable/negative examples but the
+                        weights on the desirable and undesirable losses don't seem to be in an ideal range. Based
+                        on your data, we recommend EITHER desirable_weight in [{des_weight_lower_bound}, {des_weight_upper_bound}]
+                        or undesirable_weight in [{und_weight_lower_bound}, {und_weight_upper_bound}] (but NOT BOTH).
+                        See the documentation on how to optimally set these weights.""",
+                        UserWarning,
+                    )
 
         super().__init__(
             model=model,
             args=args,
             data_collator=data_collator,
-            train_dataset=interleaved_train_dataset,
-            eval_dataset=interleaved_eval_dataset,
+            train_dataset=train_dataset,
+            eval_dataset=eval_dataset,
             tokenizer=tokenizer,
             model_init=model_init,
             compute_metrics=compute_metrics,
             callbacks=callbacks,
             optimizers=optimizers,
             preprocess_logits_for_metrics=preprocess_logits_for_metrics,
         )
@@ -635,157 +841,14 @@
             average_log_prob=False,
             is_encoder_decoder=self.is_encoder_decoder,
             label_pad_token_id=self.label_pad_token_id,
         )
 
         return completion_logps, KL_logps
 
-    def build_tokenized_answer(self, prompt, answer):
-        """
-        Llama tokenizer does not satisfy `enc(a + b) = enc(a) + enc(b)`.
-        It does ensure `enc(a + b) = enc(a) + enc(a + b)[len(enc(a)):]`.
-        Reference:
-            https://github.com/EleutherAI/lm-evaluation-harness/pull/531#issuecomment-1595586257
-        """
-
-        full_tokenized = self.tokenizer(prompt + answer, add_special_tokens=False)
-        prompt_input_ids = self.tokenizer(prompt, add_special_tokens=False)["input_ids"]
-
-        answer_input_ids = full_tokenized["input_ids"][len(prompt_input_ids) :]
-        answer_attention_mask = full_tokenized["attention_mask"][len(prompt_input_ids) :]
-
-        # Concat tokens to form `enc(a) + enc(a + b)[len(enc(a)):]`
-        full_concat_input_ids = np.concatenate([prompt_input_ids, answer_input_ids])
-
-        # Prepare input tokens for token by token comparison
-        full_input_ids = np.array(full_tokenized["input_ids"])
-
-        if len(full_input_ids) != len(full_concat_input_ids):
-            raise ValueError("Prompt input ids and answer input ids should have the same length.")
-
-        # On some tokenizers, like Llama-2 tokenizer, there are occasions where tokens
-        # can be merged together when tokenizing prompt+answer. This could result
-        # on the last token from the prompt being different when tokenized on its own
-        # vs when done as prompt+answer.
-        response_token_ids_start_idx = len(prompt_input_ids)
-
-        # If tokenized prompt is different than both prompt+answer, then it means the
-        # last token has changed due to merging.
-        if prompt_input_ids != full_tokenized["input_ids"][:response_token_ids_start_idx]:
-            response_token_ids_start_idx -= 1
-
-        prompt_input_ids = full_tokenized["input_ids"][:response_token_ids_start_idx]
-        prompt_attention_mask = full_tokenized["attention_mask"][:response_token_ids_start_idx]
-
-        if len(prompt_input_ids) != len(prompt_attention_mask):
-            raise ValueError("Prompt input ids and attention mask should have the same length.")
-
-        answer_input_ids = full_tokenized["input_ids"][response_token_ids_start_idx:]
-        answer_attention_mask = full_tokenized["attention_mask"][response_token_ids_start_idx:]
-
-        return dict(
-            prompt_input_ids=prompt_input_ids,
-            prompt_attention_mask=prompt_attention_mask,
-            answer_input_ids=answer_input_ids,
-            answer_attention_mask=answer_attention_mask,
-        )
-
-    def get_KL_dataset(self, batch) -> Dict:
-        """Creates mismatched pairs of prompts and completions for the KL dataset."""
-        batch["completion"] = batch["completion"][::-1]
-        return batch
-
-    def tokenize_row(self, feature, model: Union[PreTrainedModel, nn.Module] = None, prefix="") -> Dict:
-        """Tokenize a single row from a KTO specific dataset.
-
-        At this stage, we don't convert to PyTorch tensors yet; we just handle the truncation
-        in case the prompt + completion responses is/are too long. First
-            we truncate the prompt; if we're still too long, we truncate the completion.
-
-        We also create the labels for the completion responses, which are of length equal to
-            the sum of the length of the prompt and the completion response, with
-            label_pad_token_id  for the prompt tokens.
-        """
-        prompt = feature["prompt"]
-        completion = feature["completion"]
-
-        batch = {
-            f"{prefix}prompt": prompt,
-            f"{prefix}completion": completion,
-            f"{prefix}label": feature["label"],
-        }
-
-        if not self.is_encoder_decoder:
-            # Check issues below for more details
-            #  1. https://github.com/huggingface/trl/issues/907
-            #  2. https://github.com/EleutherAI/lm-evaluation-harness/pull/531#issuecomment-1595586257
-            #  3. https://github.com/LianjiaTech/BELLE/issues/337
-
-            if not isinstance(prompt, str):
-                raise ValueError(f"prompt should be an str but got {type(prompt)}")
-
-            if not isinstance(completion, str):
-                raise ValueError(f"completion should be an str but got {type(completion)}")
-
-            # keys of format prompt_* refers to just the prompt and answer_* refers to just the answer
-            all_tokens = self.build_tokenized_answer(prompt, completion)
-
-            max_length = self.max_length - 2
-            # if combined sequence is too long (> max_length - 1 for BOS token - 1 for EOS), truncate the prompt
-            if len(all_tokens["prompt_input_ids"]) + len(all_tokens["answer_input_ids"]) > max_length:
-                for k in ["prompt_input_ids", "prompt_attention_mask"]:
-                    if self.truncation_mode == "keep_start":
-                        all_tokens[k] = all_tokens[k][: self.max_prompt_length]
-                    elif self.truncation_mode == "keep_end":
-                        all_tokens[k] = all_tokens[k][-self.max_prompt_length :]
-                    else:
-                        raise ValueError(f"Unknown truncation mode: {self.truncation_mode}")
-
-            # if that's still too long, truncate the response
-            if len(all_tokens["prompt_input_ids"]) + len(all_tokens["answer_input_ids"]) > max_length:
-                for k in ["answer_input_ids", "answer_attention_mask"]:
-                    all_tokens[k] = all_tokens[k][: max_length - self.max_prompt_length]
-
-            # for legacy reasons, use the completion_* prefix to now refer to the joint sequence
-            batch[f"{prefix}prompt_input_ids"] = [self.tokenizer.bos_token_id] + all_tokens["prompt_input_ids"]
-            batch[f"{prefix}prompt_attention_mask"] = [1] + all_tokens["prompt_attention_mask"]
-            batch[f"{prefix}completion_input_ids"] = (
-                [self.tokenizer.bos_token_id]
-                + all_tokens["prompt_input_ids"]
-                + all_tokens["answer_input_ids"]
-                + [self.tokenizer.eos_token_id]
-            )
-            batch[f"{prefix}completion_attention_mask"] = (
-                [1] + all_tokens["prompt_attention_mask"] + all_tokens["answer_attention_mask"] + [1]
-            )
-
-            batch[f"{prefix}completion_labels"] = batch[f"{prefix}completion_input_ids"][:]
-            batch[f"{prefix}completion_labels"][: len(batch[f"{prefix}prompt_input_ids"])] = [
-                self.label_pad_token_id
-            ] * len(batch[f"{prefix}prompt_input_ids"])
-        else:
-            completion_tokens = self.tokenizer(
-                completion, truncation=True, max_length=self.max_completion_length, add_special_tokens=True
-            )
-            prompt_tokens = self.tokenizer(
-                prompt, truncation=True, max_length=self.max_prompt_length, add_special_tokens=True
-            )
-
-            batch[f"{prefix}prompt_input_ids"] = prompt_tokens["input_ids"]
-            batch[f"{prefix}prompt_attention_mask"] = prompt_tokens["attention_mask"]
-
-            batch[f"{prefix}completion_labels"] = completion_tokens["input_ids"]
-            batch[f"{prefix}completion_attention_mask"] = completion_tokens["attention_mask"]
-            if model is not None and hasattr(model, "prepare_decoder_input_ids_from_labels"):
-                batch[f"{prefix}completion_decoder_input_ids"] = model.prepare_decoder_input_ids_from_labels(
-                    labels=torch.tensor(batch["completion_labels"])
-                )
-
-        return batch
-
     @staticmethod
     def get_batch_logps(
         logits: torch.FloatTensor,
         labels: torch.LongTensor,
         average_log_prob: bool = False,
         label_pad_token_id: int = -100,
         is_encoder_decoder: bool = False,
@@ -893,60 +956,59 @@
         reference_chosen_logps: torch.FloatTensor,
         reference_rejected_logps: torch.FloatTensor,
         reference_KL_logps: torch.FloatTensor,
     ) -> Tuple[torch.FloatTensor, torch.FloatTensor, torch.FloatTensor, torch.FloatTensor]:
         """Compute the KTO loss for a batch of policy and reference model log probabilities.
 
         Args:
-            policy_chosen_logps: Log probabilities of the policy model for the chosen responses. Shape: (batch_size,)
-            policy_rejected_logps: Log probabilities of the policy model for the rejected responses. Shape: (batch_size,)
+            policy_chosen_logps: Log probabilities of the policy model for the chosen responses. Shape: (num(chosen) in batch_size,)
+            policy_rejected_logps: Log probabilities of the policy model for the rejected responses. Shape: (num(rejected) in batch_size,)
             policy_KL_logps: Log probabilities of the policy model for the KL responses. Shape: (batch_size,)
-            reference_chosen_logps: Log probabilities of the reference model for the chosen responses. Shape: (batch_size,)
-            reference_rejected_logps: Log probabilities of the reference model for the rejected responses. Shape: (batch_size,)
+            reference_chosen_logps: Log probabilities of the reference model for the chosen responses. Shape: (num(chosen) in batch_size,)
+            reference_rejected_logps: Log probabilities of the reference model for the rejected responses. Shape: (num(rejected) in batch_size,)
             reference_KL_logps: Log probabilities of the reference model for the KL responses. Shape: (batch_size,)
 
         Returns:
             A tuple of four tensors: (losses, chosen_rewards, rejected_rewards, KL).
             The losses tensor contains the KTO loss for each example in the batch.
             The chosen_rewards and rejected_rewards tensors contain the rewards for the chosen and rejected responses, respectively.
             The KL tensor contains the detached KL divergence estimate between the policy and reference models.
         """
-        KL = (policy_KL_logps - reference_KL_logps).mean().detach()
-        KL = self.accelerator.gather(KL).mean().clamp(min=0)
+        kl = (policy_KL_logps - reference_KL_logps).mean().detach()
+        kl = self.accelerator.gather(kl).mean().clamp(min=0)
 
         if policy_chosen_logps.shape[0] != 0 or reference_chosen_logps.shape[0] != 0:
             chosen_logratios = policy_chosen_logps - reference_chosen_logps
-            chosen_losses = 1 - F.sigmoid(self.beta * (chosen_logratios - KL))
+            chosen_losses = 1 - F.sigmoid(self.beta * (chosen_logratios - kl))
             chosen_rewards = self.beta * chosen_logratios.detach()
         else:
             # lists can't be empty -- if they are, then accelerate.gather will hang
-            chosen_losses = torch.Tensor([torch.nan]).to(self.accelerator.device)
-            chosen_rewards = torch.Tensor([torch.nan]).to(self.accelerator.device)
+            chosen_losses = torch.Tensor([]).to(self.accelerator.device)
+            chosen_rewards = torch.Tensor([]).to(self.accelerator.device)
 
         if policy_rejected_logps.shape[0] != 0 or reference_rejected_logps.shape[0] != 0:
             rejected_logratios = policy_rejected_logps - reference_rejected_logps
-            rejected_losses = 1 - F.sigmoid(self.beta * (KL - rejected_logratios))
+            rejected_losses = 1 - F.sigmoid(self.beta * (kl - rejected_logratios))
             rejected_rewards = self.beta * rejected_logratios.detach()
         else:
             # lists can't be empty -- if they are, then accelerate.gather will hang
-            rejected_losses = torch.Tensor([torch.nan]).to(self.accelerator.device)
-            rejected_rewards = torch.Tensor([torch.nan]).to(self.accelerator.device)
+            rejected_losses = torch.Tensor([]).to(self.accelerator.device)
+            rejected_rewards = torch.Tensor([]).to(self.accelerator.device)
 
         losses = torch.cat(
             (self.desirable_weight * chosen_losses, self.undesirable_weight * rejected_losses),
             0,
         )
 
-        return losses, chosen_rewards, rejected_rewards, KL
+        return losses, chosen_rewards, rejected_rewards, kl
 
     def get_batch_loss_metrics(
         self,
         model,
         batch: Dict[str, Union[List, torch.LongTensor]],
-        train_eval: Literal["train", "eval"] = "train",
     ):
         """Compute the KTO loss and other metrics for the given batch of inputs for train or test."""
         metrics = {}
         batch = {k: (v.to(self.accelerator.device) if isinstance(v, torch.Tensor) else v) for k, v in batch.items()}
 
         (
             policy_chosen_logps,
@@ -989,70 +1051,73 @@
             policy_rejected_logps,
             policy_KL_logps,
             reference_chosen_logps,
             reference_rejected_logps,
             reference_KL_logps,
         )
 
-        mean_chosen_reward = chosen_rewards.nanmean().detach()
-        mean_rejected_reward = rejected_rewards.nanmean().detach()
-        mean_chosen_logps = policy_chosen_logps.nanmean().detach()
-        mean_rejected_logps = policy_rejected_logps.nanmean().detach()
-
-        prefix = "eval_" if train_eval == "eval" else ""
-        metrics[f"{prefix}rewards/chosen"] = self.accelerator.gather(mean_chosen_reward).nanmean().cpu()
-        metrics[f"{prefix}rewards/rejected"] = self.accelerator.gather(mean_rejected_reward).nanmean().cpu()
-        metrics[f"{prefix}rewards/margins"] = metrics[f"{prefix}rewards/chosen"] - metrics[f"{prefix}rewards/rejected"]
-        metrics[f"{prefix}kl"] = kl.item()  # has already been gathered in kto_loss
-        metrics[f"{prefix}logps/chosen"] = self.accelerator.gather(mean_chosen_logps).nanmean().cpu()
-        metrics[f"{prefix}logps/rejected"] = self.accelerator.gather(mean_rejected_logps).nanmean().cpu()
-
-        loss = (
-            losses.mean()
-            if losses.shape[0] != 0
-            else torch.tensor(float("nan"), requires_grad=True).to(self.accelerator.device)
-        )
-        return loss, metrics
+        num_chosen = torch.Tensor([len(chosen_rewards)]).to(self.accelerator.device)
+        num_rejected = torch.Tensor([len(rejected_rewards)]).to(self.accelerator.device)
+
+        all_num_chosen = self.accelerator.gather(num_chosen).sum().item()
+        all_num_rejected = self.accelerator.gather(num_rejected).sum().item()
+
+        if all_num_chosen > 0:
+            metrics["rewards/chosen_sum"] = self.accelerator.gather(chosen_rewards.nansum()).nansum().item()
+            metrics["logps/chosen_sum"] = self.accelerator.gather(policy_chosen_logps.nansum()).nansum().item()
+            metrics["count/chosen"] = all_num_chosen
+
+        if all_num_rejected > 0:
+            metrics["rewards/rejected_sum"] = self.accelerator.gather(rejected_rewards.nansum()).nansum().item()
+            metrics["logps/rejected_sum"] = self.accelerator.gather(policy_rejected_logps.nansum()).nansum().item()
+            metrics["count/rejected"] = all_num_rejected
+
+        metrics["kl"] = kl.item()
+
+        return losses.nanmean(), metrics
 
     def compute_loss(
         self,
         model: Union[PreTrainedModel, nn.Module],
         inputs: Dict[str, Union[torch.Tensor, Any]],
         return_outputs=False,
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, Dict[str, torch.Tensor]]]:
         if not self.use_dpo_data_collator:
             warnings.warn(
                 "compute_loss is only implemented for DPODataCollatorWithPadding, and you passed a datacollator that is different than "
                 "DPODataCollatorWithPadding - you might see unexpected behavior. Alternatively, you can implement your own prediction_step method if you are using a custom data collator"
             )
+        compute_loss_context_manager = torch.cuda.amp.autocast if self._peft_has_been_casted_to_bf16 else nullcontext
 
-        loss, metrics = self.get_batch_loss_metrics(model, inputs, train_eval="train")
+        with compute_loss_context_manager():
+            loss, metrics = self.get_batch_loss_metrics(model, inputs)
 
+        # Make sure to move the loss to the device the original accumulating loss is at back in the `Trainer` class:
+        loss = loss.to(self.args.device)
         # force log the metrics
         if self.accelerator.is_main_process:
             self.store_metrics(metrics, train_eval="train")
 
         if return_outputs:
             return (loss, metrics)
         return loss
 
     def store_metrics(self, metrics: Dict[str, float], train_eval: Literal["train", "eval"] = "train") -> None:
         for key, value in metrics.items():
             self._stored_metrics[train_eval][key].append(value)
 
     def _get_train_sampler(self) -> Optional[torch.utils.data.Sampler]:
-        # We use a sequential sampler for training as the order of the interleaved dataset is important
         if self.train_dataset is None or not has_length(self.train_dataset):
             return None
         return SequentialSampler(self.train_dataset)
 
     def get_batch_samples(self, model, batch: Dict[str, torch.LongTensor]) -> Tuple[str, str]:
         """Generate samples from the model and reference model for the given batch of inputs."""
 
-        # If one uses `generate_during_eval` with peft + bf16, we need to explictly call generate with
+        # If one uses `generate_during_eval` with peft + bf16, we need to explicitly call generate with
         # the torch cuda amp context manager as some hidden states are silently casted to full precision.
         generate_context_manager = nullcontext if not self._peft_has_been_casted_to_bf16 else torch.cuda.amp.autocast
 
         with generate_context_manager():
             policy_output = model.generate(
                 input_ids=batch["prompt_input_ids"],
                 attention_mask=batch["prompt_attention_mask"],
@@ -1107,27 +1172,27 @@
             if hasattr(model, "config"):
                 ignore_keys = getattr(model.config, "keys_to_ignore_at_inference", [])
             else:
                 ignore_keys = []
 
         prediction_context_manager = torch.cuda.amp.autocast if self._peft_has_been_casted_to_bf16 else nullcontext
         with torch.no_grad(), prediction_context_manager():
-            loss, metrics = self.get_batch_loss_metrics(model, inputs, train_eval="eval")
+            loss, metrics = self.get_batch_loss_metrics(model, inputs)
 
         # force log the metrics
         if self.accelerator.is_main_process:
             self.store_metrics(metrics, train_eval="eval")
 
         if prediction_loss_only:
             return (loss.detach(), None, None)
 
         # logits for the chosen and rejected samples from model
         logits_dict = {
-            "eval_logits/chosen": metrics["eval_logits/chosen"],
-            "eval_logits/rejected": metrics["eval_logits/rejected"],
+            "eval_logits/chosen": metrics["logits/chosen"],
+            "eval_logits/rejected": metrics["logits/rejected"],
         }
         logits = tuple(v.unsqueeze(dim=0) for k, v in logits_dict.items() if k not in ignore_keys)
         logits = torch.stack(logits).mean(axis=1).to(self.accelerator.device)
         labels = torch.zeros(logits.shape[0], device=self.accelerator.device)
 
         return (loss.detach(), logits, labels)
 
@@ -1193,22 +1258,39 @@
 
         Args:
             logs (`Dict[str, float]`):
                 The values to log.
         """
         # logs either has 'loss' or 'eval_loss'
         train_eval = "train" if "loss" in logs else "eval"
+        # accumulate average metrics from sums and lengths
+        for split in ["chosen", "rejected"]:
+            if f"count/{split}" in self._stored_metrics[train_eval]:
+                count_sum = torch.Tensor(self._stored_metrics[train_eval][f"count/{split}"]).sum().item()
+                logs[f"{train_eval}/rewards/{split}"] = (
+                    torch.Tensor(self._stored_metrics[train_eval][f"rewards/{split}_sum"]).sum().item() / count_sum
+                )
+                logs[f"{train_eval}/logps/{split}"] = (
+                    torch.Tensor(self._stored_metrics[train_eval][f"logps/{split}_sum"]).sum().item() / count_sum
+                )
+                for key in [f"count/{split}", f"rewards/{split}_sum", f"logps/{split}_sum"]:
+                    del self._stored_metrics[train_eval][key]
+        # calculate reward margin
+        if f"{train_eval}/rewards/chosen" in logs and f"{train_eval}/rewards/rejected" in logs:
+            logs[f"{train_eval}/rewards/margins"] = (
+                logs[f"{train_eval}/rewards/chosen"] - logs[f"{train_eval}/rewards/rejected"]
+            )
         # Add averaged stored metrics to logs
         for key, metrics in self._stored_metrics[train_eval].items():
-            logs[key] = torch.tensor(metrics).mean().item()
+            logs[f"{train_eval}/{key}"] = torch.Tensor(metrics).mean().item()
         del self._stored_metrics[train_eval]
         return super().log(logs)
 
     @wraps(Trainer.push_to_hub)
     def push_to_hub(self, commit_message: Optional[str] = "End of training", blocking: bool = True, **kwargs) -> str:
         """
-        Overwrite the `push_to_hub` method in order to force-add the tag "sft" when pushing the
+        Overwrite the `push_to_hub` method in order to force-add the tag "kto" when pushing the
         model on the Hub. Please refer to `~transformers.Trainer.push_to_hub` for more details.
         """
         kwargs = trl_sanitze_kwargs_for_tagging(model=self.model, tag_names=self._tag_names, kwargs=kwargs)
 
         return super().push_to_hub(commit_message=commit_message, blocking=blocking, **kwargs)
```

### Comparing `trl-0.8.1/trl/trainer/model_config.py` & `trl-0.8.2/trl/trainer/model_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,7 +81,10 @@
         for key, value in self.__dict__.items():
             output_dict[key] = value
         return flatten_dict(output_dict)
 
     def __post_init__(self):
         if self.load_in_8bit and self.load_in_4bit:
             raise ValueError("You can't use 8 bit and 4 bit precision at the same time")
+
+        if self.lora_target_modules == ["all-linear"]:
+            self.lora_target_modules = "all-linear"
```

### Comparing `trl-0.8.1/trl/trainer/ppo_config.py` & `trl-0.8.2/trl/trainer/ppo_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/ppo_trainer.py` & `trl-0.8.2/trl/trainer/ppo_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,20 @@
     masked_var,
     masked_whiten,
     set_seed,
     stack_dicts,
     stats_to_np,
 )
 from ..import_utils import is_npu_available, is_torch_greater_2_0, is_xpu_available
-from ..models import SUPPORTED_ARCHITECTURES, PreTrainedModelWrapper, create_reference_model
+from ..models import (
+    SUPPORTED_ARCHITECTURES,
+    PreTrainedModelWrapper,
+    create_reference_model,
+    unwrap_model_for_generation,
+)
 from . import AdaptiveKLController, BaseTrainer, FixedKLController, PPOConfig, RunningMoments
 
 
 if is_deepspeed_available():
     import deepspeed
 
 MODEL_CARD_TEMPLATE = """---
@@ -466,38 +471,42 @@
                 query_tensor,
                 length_sampler=length_sampler,
                 batch_size=batch_size,
                 return_prompt=return_prompt,
                 **generation_kwargs,
             )
             if generate_ref_response:
-                with self.optional_peft_ctx():
-                    ref_response = self._generate_batched(
-                        ref_model,
-                        query_tensor,
-                        length_sampler=length_sampler,
-                        batch_size=batch_size,
-                        return_prompt=return_prompt,
-                        **generation_kwargs,
-                    )
+                ref_response = self._generate_batched(
+                    ref_model,
+                    query_tensor,
+                    length_sampler=length_sampler,
+                    batch_size=batch_size,
+                    return_prompt=return_prompt,
+                    **generation_kwargs,
+                )
 
         else:
             if len(query_tensor.shape) == 2:
                 raise ValueError(
                     "query_tensor must be a tensor of shape (`seq_len`) or a list of tensors of shape (`seq_len`)"
                 )
 
             if length_sampler is not None:
                 generation_kwargs["max_new_tokens"] = length_sampler()
-            response = self.accelerator.unwrap_model(self.model).generate(
-                input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs
-            )
+
+            with unwrap_model_for_generation(self.model, self.accelerator) as unwrapped_model:
+                response = unwrapped_model.generate(input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs)
+
             if generate_ref_response:
-                with self.optional_peft_ctx():
-                    ref_response = ref_model.generate(input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs)
+                with unwrap_model_for_generation(
+                    self.model, self.accelerator, is_peft_model=self.is_peft_model
+                ) as unwrapped_model:
+                    ref_response = unwrapped_model.generate(
+                        input_ids=query_tensor.unsqueeze(dim=0), **generation_kwargs
+                    )
 
             if not return_prompt and not self.is_encoder_decoder:
                 response = response[:, query_tensor.shape[0] :]
                 if generate_ref_response:
                     ref_response = ref_response[:, query_tensor.shape[0] :]
 
         if generate_ref_response:
@@ -539,15 +548,16 @@
                 inputs,
                 padding=True,
                 max_length=None,
                 pad_to_multiple_of=pad_to_multiple_of,
                 return_tensors="pt",
             ).to(self.current_device)
 
-            generations = self.accelerator.unwrap_model(model).generate(**padded_inputs, **generation_kwargs)
+            with unwrap_model_for_generation(model, self.accelerator) as unwrapped_model:
+                generations = unwrapped_model.generate(**padded_inputs, **generation_kwargs)
 
             for generation, mask in zip(generations, padded_inputs["attention_mask"]):
                 if not self.is_encoder_decoder:
                     output = generation[(1 - mask).sum() :]  # remove padding
                 else:
                     output = generation
```

### Comparing `trl-0.8.1/trl/trainer/reward_config.py` & `trl-0.8.2/trl/trainer/reward_config.py`

 * *Files identical despite different names*

### Comparing `trl-0.8.1/trl/trainer/reward_trainer.py` & `trl-0.8.2/trl/trainer/reward_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,25 +192,25 @@
                     UserWarning,
                 )
 
             self.use_reward_data_collator = True
         else:
             self.use_reward_data_collator = False
         super().__init__(
-            model,
-            args,
-            data_collator,
-            train_dataset,
-            eval_dataset,
-            tokenizer,
-            model_init,
-            compute_metrics,
-            callbacks,
-            optimizers,
-            preprocess_logits_for_metrics,
+            model=model,
+            args=args,
+            data_collator=data_collator,
+            train_dataset=train_dataset,
+            eval_dataset=eval_dataset,
+            tokenizer=tokenizer,
+            model_init=model_init,
+            compute_metrics=compute_metrics,
+            callbacks=callbacks,
+            optimizers=optimizers,
+            preprocess_logits_for_metrics=preprocess_logits_for_metrics,
         )
 
         # Add tags for models that have been loaded with the correct transformers version
         if hasattr(self.model, "add_model_tags"):
             self.model.add_model_tags(self._tag_names)
 
     def compute_loss(
```

### Comparing `trl-0.8.1/trl/trainer/sft_trainer.py` & `trl-0.8.2/trl/trainer/sft_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 import dataclasses
 import inspect
 import warnings
 from functools import wraps
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
+import datasets
 import torch
 import torch.nn as nn
 from accelerate.state import PartialState
 from datasets import Dataset
 from datasets.arrow_writer import SchemaInferenceError
 from datasets.builder import DatasetGenerationError
 from transformers import (
@@ -392,20 +393,35 @@
         max_seq_length,
         formatting_func,
         num_of_sequences,
         chars_per_token,
         remove_unused_columns=True,
         append_concat_token=True,
         add_special_tokens=True,
+        skip_prepare_dataset=False,
     ):
         if dataset is None:
             raise ValueError("The dataset should not be None")
 
+        if skip_prepare_dataset:
+            return dataset
+
+        # If the dataset is already preprocessed (tokenized), return as-is. Only works if dataset is
+        # a datasets.Dataset or datasets.IterableDataset -- not for torch Dataset
+        column_names = (
+            dataset.column_names if isinstance(dataset, (datasets.Dataset, datasets.IterableDataset)) else None
+        )
+        if column_names and "input_ids" in column_names:
+            return dataset
+
         # check if torch dataset / dataloader and do nothing
-        if isinstance(dataset, (torch.utils.data.IterableDataset, torch.utils.data.Dataset, ConstantLengthDataset)):
+        # see https://github.com/huggingface/trl/pull/1468 for why datasets.IterableDataset needs a separate check
+        if isinstance(
+            dataset, (torch.utils.data.IterableDataset, torch.utils.data.Dataset, ConstantLengthDataset)
+        ) and not isinstance(dataset, datasets.IterableDataset):
             return dataset
 
         if not packing:
             return self._prepare_non_packed_dataloader(
                 tokenizer,
                 dataset,
                 dataset_text_field,
@@ -509,14 +525,17 @@
                 num_of_sequences=num_of_sequences,
                 chars_per_token=chars_per_token,
                 eos_token_id=tokenizer.eos_token_id,
                 append_concat_token=append_concat_token,
                 add_special_tokens=add_special_tokens,
             )
 
+            if isinstance(dataset, datasets.IterableDataset):
+                return constant_length_iterator
+
             def data_generator(constant_length_iterator):
                 yield from constant_length_iterator
 
             try:
                 packed_dataset = Dataset.from_generator(
                     data_generator, gen_kwargs={"constant_length_iterator": constant_length_iterator}
                 )
```

### Comparing `trl-0.8.1/trl/trainer/utils.py` & `trl-0.8.2/trl/trainer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -742,66 +742,76 @@
 
 class RichProgressCallback(TrainerCallback):
     """
     A [`TrainerCallback`] that displays the progress of training or evaluation using Rich.
     """
 
     def __init__(self):
-        self.training_bar = Progress()
-        self.prediction_bar = Progress()
+        self.training_bar = None
+        self.prediction_bar = None
 
         self.training_task_id = None
         self.prediction_task_id = None
 
         self.rich_group = None
         self.rich_console = None
 
+        self.training_status = None
+        self.current_step = None
+
     def on_train_begin(self, args, state, control, **kwargs):
         if state.is_world_process_zero:
+            self.training_bar = Progress()
+            self.prediction_bar = Progress()
+
             self.rich_console = Console()
 
             self.training_status = self.rich_console.status("Nothing to log yet ...")
 
             self.rich_group = Live(Panel(Group(self.training_bar, self.prediction_bar, self.training_status)))
             self.rich_group.start()
 
-            # self.training_bar.start()
             self.training_task_id = self.training_bar.add_task("[blue]Training the model", total=state.max_steps)
-        self.current_step = 0
+            self.current_step = 0
 
     def on_step_end(self, args, state, control, **kwargs):
         if state.is_world_process_zero:
             self.training_bar.update(self.training_task_id, advance=state.global_step - self.current_step, update=True)
             self.current_step = state.global_step
 
     def on_prediction_step(self, args, state, control, eval_dataloader=None, **kwargs):
         if state.is_world_process_zero and has_length(eval_dataloader):
-            if self.prediction_bar is None:
-                # self.prediction_bar.start()
+            if self.prediction_task_id is None:
                 self.prediction_task_id = self.prediction_bar.add_task(
-                    "[blue]Predicting on the evaluation dataset", total=state.max_steps
+                    "[blue]Predicting on the evaluation dataset", total=len(eval_dataloader)
                 )
             self.prediction_bar.update(self.prediction_task_id, advance=1, update=True)
 
     def on_evaluate(self, args, state, control, **kwargs):
         if state.is_world_process_zero:
-            if self.prediction_bar is not None:
-                self.prediction_bar.close()
-            self.prediction_bar = None
+            if self.prediction_task_id is not None:
+                self.prediction_bar.remove_task(self.prediction_task_id)
+                self.prediction_task_id = None
 
     def on_predict(self, args, state, control, **kwargs):
         if state.is_world_process_zero:
-            if self.prediction_bar is not None:
-                self.prediction_bar.stop()
+            if self.prediction_task_id is not None:
                 self.prediction_bar.remove_task(self.prediction_task_id)
-            self.prediction_bar = None
+                self.prediction_task_id = None
 
     def on_log(self, args, state, control, logs=None, **kwargs):
         if state.is_world_process_zero and self.training_bar is not None:
             _ = logs.pop("total_flos", None)
             self.training_status.update(f"[bold green]Status = {str(logs)}")
 
     def on_train_end(self, args, state, control, **kwargs):
         if state.is_world_process_zero:
-            self.training_bar.stop()
             self.rich_group.stop()
+
             self.training_bar = None
+            self.prediction_bar = None
+            self.training_task_id = None
+            self.prediction_task_id = None
+            self.rich_group = None
+            self.rich_console = None
+            self.training_status = None
+            self.current_step = None
```

### Comparing `trl-0.8.1/trl.egg-info/PKG-INFO` & `trl-0.8.2/trl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trl
-Version: 0.8.1
+Version: 0.8.2
 Summary: Train transformer language models with reinforcement learning.
 Home-page: https://github.com/huggingface/trl
 Author: Leandro von Werra
 Author-email: leandro.vonwerra@gmail.com
 License: Apache 2.0
 Keywords: ppo,transformers,huggingface,gpt2,language modeling,rlhf
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -59,15 +59,15 @@
 ## Highlights
 
 - **`Efficient and scalable`**: 
     - [`accelerate`](https://github.com/huggingface/accelerate) is the backbone of `trl` which allows to scale model training from a single GPU to a large scale multi-node cluster with methods such as DDP and DeepSpeed.
     - [`PEFT`](https://github.com/huggingface/peft) is fully integrated and allows to train even the largest models on modest hardware with quantisation and methods such as LoRA or QLoRA.
     - [`unsloth`](https://github.com/unslothai/unsloth) is also integrated and allows to significantly speed up training with dedicated kernels.
 - **`CLI`**: With the [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with LLMs without writing any code using a single command and a flexible config system.
-- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer).
+- **`Trainers`**: The Trainer classes are an abstraction to apply many fine-tuning methods with ease such as the [`SFTTrainer`](https://huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/trainer#trl.ORPOTrainer).
 - **`AutoModels`**: The [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForCausalLMWithValueHead) & [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value head to the model which allows to train them with RL algorithms such as PPO.
 - **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT sentiment classifier, full RLHF using adapters only, train GPT-j to be less toxic, [StackLlama example](https://huggingface.co/blog/stackllama), etc. following the [examples](https://github.com/huggingface/trl/tree/main/examples).
 
 ## Installation
 
 ### Python package
 Install the library with `pip`:
@@ -96,32 +96,32 @@
 ```bash
 trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --output_dir opt-sft-imdb
 ```
 
 **DPO:**
 
 ```bash
-trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-processed --output_dir opt-sft-hh-rlhf 
+trl dpo --model_name_or_path facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --output_dir opt-sft-hh-rlhf 
 ```
 
 **Chat:**
 
 ```bash
 trl chat --model_name_or_path Qwen/Qwen1.5-0.5B-Chat
 ```
 
 Read more about CLI in the [relevant documentation section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more details.
 
 ## How to use
 
-For more flexibility and control over the training you can use the dedicated trainer classes to fine-tune the model in Python.
+For more flexibility and control over the training, you can use the dedicated trainer classes to fine-tune the model in Python.
 
 ### `SFTTrainer`
 
-This is a basic example on how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
+This is a basic example of how to use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer to easily fine-tune language models or adapters on a custom dataset.
 
 ```python
 # imports
 from datasets import load_dataset
 from trl import SFTTrainer
 
 # get dataset
@@ -137,15 +137,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `RewardTrainer`
 
-This is a basic example on how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+This is a basic example of how to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForSequenceClassification, AutoTokenizer
 from trl import RewardTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -163,15 +163,15 @@
 
 # train
 trainer.train()
 ```
 
 ### `PPOTrainer`
 
-This is a basic example on how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
+This is a basic example of how to use the `PPOTrainer` from the library. Based on a query the language model creates a response which is then evaluated. The evaluation could be a human in the loop or another model's output.
 
 ```python
 # imports
 import torch
 from transformers import AutoTokenizer
 from trl import PPOTrainer, PPOConfig, AutoModelForCausalLMWithValueHead, create_reference_model
 from trl.core import respond_to_batch
@@ -202,15 +202,15 @@
 
 # train model for one step with ppo
 train_stats = ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward)
 ```
 
 ### `DPOTrainer`
 
-`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
+`DPOTrainer` is a trainer that uses [Direct Preference Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a wrapper around the `transformers` Trainer to easily fine-tune reward models or adapters on a custom preference dataset.
 
 ```python
 # imports
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from trl import DPOTrainer
 
 # load model and dataset - dataset needs to be in a specific format
@@ -242,15 +242,15 @@
 
 ## References
 
 ### Proximal Policy Optimisation
 The PPO implementation largely follows the structure introduced in the paper **"Fine-Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper](https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-human-preferences)].
 
 ### Direct Preference Optimization
-DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
+DPO is based on the original implementation of **"Direct Preference Optimization: Your Language Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-preference-optimization)]
 
 
 ## Citation
 
 ```bibtex
 @misc{vonwerra2022trl,
   author = {Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert and Shengyi Huang},
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trl Version: 0.8.1 Summary: Train transformer
+Metadata-Version: 2.1 Name: trl Version: 0.8.2 Summary: Train transformer
 language models with reinforcement learning. Home-page: https://github.com/
 huggingface/trl Author: Leandro von Werra Author-email:
 leandro.vonwerra@gmail.com License: Apache 2.0 Keywords:
 ppo,transformers,huggingface,gpt2,language modeling,rlhf Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
@@ -35,16 +35,18 @@
 significantly speed up training with dedicated kernels. - **`CLI`**: With the
 [CLI](https://huggingface.co/docs/trl/clis) you can fine-tune and chat with
 LLMs without writing any code using a single command and a flexible config
 system. - **`Trainers`**: The Trainer classes are an abstraction to apply many
 fine-tuning methods with ease such as the [`SFTTrainer`](https://
 huggingface.co/docs/trl/sft_trainer), [`DPOTrainer`](https://huggingface.co/
 docs/trl/trainer#trl.DPOTrainer), [`RewardTrainer`](https://huggingface.co/
-docs/trl/reward_trainer), and [`PPOTrainer`](https://huggingface.co/docs/trl/
-trainer#trl.PPOTrainer). - **`AutoModels`**: The
+docs/trl/reward_trainer), [`PPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.PPOTrainer), [`CPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.CPOTrainer), and [`ORPOTrainer`](https://huggingface.co/docs/trl/
+trainer#trl.ORPOTrainer). - **`AutoModels`**: The
 [`AutoModelForCausalLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForCausalLMWithValueHead) &
 [`AutoModelForSeq2SeqLMWithValueHead`](https://huggingface.co/docs/trl/
 models#trl.AutoModelForSeq2SeqLMWithValueHead) classes add an additional value
 head to the model which allows to train them with RL algorithms such as PPO. -
 **`Examples`**: Train GPT2 to generate positive movie reviews with a BERT
 sentiment classifier, full RLHF using adapters only, train GPT-j to be less
@@ -57,37 +59,37 @@
 want to use the examples you can clone the repository with the following
 command: ```bash git clone https://github.com/huggingface/trl.git ``` ##
 Command Line Interface (CLI) You can use TRL Command Line Interface (CLI) to
 quickly get started with Supervised Fine-tuning (SFT), Direct Preference
 Optimization (DPO) and test your aligned model with the chat CLI: **SFT:**
 ```bash trl sft --model_name_or_path facebook/opt-125m --dataset_name imdb --
 output_dir opt-sft-imdb ``` **DPO:** ```bash trl dpo --model_name_or_path
-facebook/opt-125m --dataset_name trl-internal-testing/Anthropic-hh-rlhf-
-processed --output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --
-model_name_or_path Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the
-[relevant documentation section](https://huggingface.co/docs/trl/main/en/clis)
-or use `--help` for more details. ## How to use For more flexibility and
-control over the training you can use the dedicated trainer classes to fine-
-tune the model in Python. ### `SFTTrainer` This is a basic example on how to
-use the `SFTTrainer` from the library. The `SFTTrainer` is a light wrapper
-around the `transformers` Trainer to easily fine-tune language models or
-adapters on a custom dataset. ```python # imports from datasets import
-load_dataset from trl import SFTTrainer # get dataset dataset = load_dataset
-("imdb", split="train") # get trainer trainer = SFTTrainer( "facebook/opt-
-350m", train_dataset=dataset, dataset_text_field="text", max_seq_length=512, )
-# train trainer.train() ``` ### `RewardTrainer` This is a basic example on how
-to use the `RewardTrainer` from the library. The `RewardTrainer` is a wrapper
-around the `transformers` Trainer to easily fine-tune reward models or adapters
-on a custom preference dataset. ```python # imports from transformers import
+facebook/opt-125m --dataset_name trl-internal-testing/hh-rlhf-trl-style --
+output_dir opt-sft-hh-rlhf ``` **Chat:** ```bash trl chat --model_name_or_path
+Qwen/Qwen1.5-0.5B-Chat ``` Read more about CLI in the [relevant documentation
+section](https://huggingface.co/docs/trl/main/en/clis) or use `--help` for more
+details. ## How to use For more flexibility and control over the training, you
+can use the dedicated trainer classes to fine-tune the model in Python. ###
+`SFTTrainer` This is a basic example of how to use the `SFTTrainer` from the
+library. The `SFTTrainer` is a light wrapper around the `transformers` Trainer
+to easily fine-tune language models or adapters on a custom dataset. ```python
+# imports from datasets import load_dataset from trl import SFTTrainer # get
+dataset dataset = load_dataset("imdb", split="train") # get trainer trainer =
+SFTTrainer( "facebook/opt-350m", train_dataset=dataset,
+dataset_text_field="text", max_seq_length=512, ) # train trainer.train() ```
+### `RewardTrainer` This is a basic example of how to use the `RewardTrainer`
+from the library. The `RewardTrainer` is a wrapper around the `transformers`
+Trainer to easily fine-tune reward models or adapters on a custom preference
+dataset. ```python # imports from transformers import
 AutoModelForSequenceClassification, AutoTokenizer from trl import RewardTrainer
 # load model and dataset - dataset needs to be in a specific format model =
 AutoModelForSequenceClassification.from_pretrained("gpt2", num_labels=1)
 tokenizer = AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer =
 RewardTrainer( model=model, tokenizer=tokenizer, train_dataset=dataset, ) #
-train trainer.train() ``` ### `PPOTrainer` This is a basic example on how to
+train trainer.train() ``` ### `PPOTrainer` This is a basic example of how to
 use the `PPOTrainer` from the library. Based on a query the language model
 creates a response which is then evaluated. The evaluation could be a human in
 the loop or another model's output. ```python # imports import torch from
 transformers import AutoTokenizer from trl import PPOTrainer, PPOConfig,
 AutoModelForCausalLMWithValueHead, create_reference_model from trl.core import
 respond_to_batch # get models model =
 AutoModelForCausalLMWithValueHead.from_pretrained('gpt2') model_ref =
@@ -99,15 +101,15 @@
 (model, query_tensor) # create a ppo trainer ppo_trainer = PPOTrainer
 (ppo_config, model, model_ref, tokenizer) # define a reward for response #
 (this could be any reward such as human feedback or output from another model)
 reward = [torch.tensor(1.0)] # train model for one step with ppo train_stats =
 ppo_trainer.step([query_tensor[0]], [response_tensor[0]], reward) ``` ###
 `DPOTrainer` `DPOTrainer` is a trainer that uses [Direct Preference
 Optimization algorithm](https://arxiv.org/abs/2305.18290). This is a basic
-example on how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
+example of how to use the `DPOTrainer` from the library. The `DPOTrainer` is a
 wrapper around the `transformers` Trainer to easily fine-tune reward models or
 adapters on a custom preference dataset. ```python # imports from transformers
 import AutoModelForCausalLM, AutoTokenizer from trl import DPOTrainer # load
 model and dataset - dataset needs to be in a specific format model =
 AutoModelForCausalLM.from_pretrained("gpt2") tokenizer =
 AutoTokenizer.from_pretrained("gpt2") ... # load trainer trainer = DPOTrainer
 ( model=model, tokenizer=tokenizer, train_dataset=dataset, ) # train
@@ -117,14 +119,15 @@
 dev install: ```bash git clone https://github.com/huggingface/trl.git cd trl/
 make dev ``` ## References ### Proximal Policy Optimisation The PPO
 implementation largely follows the structure introduced in the paper **"Fine-
 Tuning Language Models from Human Preferences"** by D. Ziegler et al. \[[paper]
 (https://arxiv.org/pdf/1909.08593.pdf), [code](https://github.com/openai/lm-
 human-preferences)]. ### Direct Preference Optimization DPO is based on the
 original implementation of **"Direct Preference Optimization: Your Language
-Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](), [code]
-(https://github.com/eric-mitchell/direct-preference-optimization)] ## Citation
-```bibtex @misc{vonwerra2022trl, author = {Leandro von Werra and Younes Belkada
-and Lewis Tunstall and Edward Beeching and Tristan Thrush and Nathan Lambert
-and Shengyi Huang}, title = {TRL: Transformer Reinforcement Learning}, year =
-{2020}, publisher = {GitHub}, journal = {GitHub repository}, howpublished =
-{\url{https://github.com/huggingface/trl}} } ```
+Model is Secretly a Reward Model"** by E. Mitchell et al. \[[paper](https://
+arxiv.org/pdf/2305.18290.pdf), [code](https://github.com/eric-mitchell/direct-
+preference-optimization)] ## Citation ```bibtex @misc{vonwerra2022trl, author =
+{Leandro von Werra and Younes Belkada and Lewis Tunstall and Edward Beeching
+and Tristan Thrush and Nathan Lambert and Shengyi Huang}, title = {TRL:
+Transformer Reinforcement Learning}, year = {2020}, publisher = {GitHub},
+journal = {GitHub repository}, howpublished = {\url{https://github.com/
+huggingface/trl}} } ```
```

### Comparing `trl-0.8.1/trl.egg-info/SOURCES.txt` & `trl-0.8.2/trl.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 examples/scripts/ppo_multi_adapter.py
 examples/scripts/reward_modeling.py
 examples/scripts/sft.py
 tests/__init__.py
 tests/test_best_of_n_sampler.py
 tests/test_cli.py
 tests/test_core.py
+tests/test_cpo_trainer.py
 tests/test_data_collator_completion_only.py
 tests/test_dataset_formatting.py
 tests/test_ddpo_trainer.py
 tests/test_dpo_trainer.py
 tests/test_e2e.py
 tests/test_environments.py
 tests/test_iterative_sft_trainer.py
 tests/test_kto_trainer.py
 tests/test_modeling_value_head.py
 tests/test_no_peft.py
+tests/test_orpo_trainer.py
 tests/test_peft_models.py
 tests/test_ppo_trainer.py
 tests/test_reward_trainer.py
+tests/test_rich_progress_callback.py
 tests/test_sft_trainer.py
 tests/testing_constants.py
 tests/testing_utils.py
 tests/slow/__init__.py
 tests/slow/test_dpo_slow.py
 tests/slow/test_sft_slow.py
 tests/slow/testing_constants.py
@@ -57,41 +60,48 @@
 trl/../examples/scripts/ppo_multi_adapter.py
 trl/../examples/scripts/reward_modeling.py
 trl/../examples/scripts/sft.py
 trl/commands/__init__.py
 trl/commands/cli.py
 trl/commands/cli_utils.py
 trl/commands/scripts/chat.py
+trl/commands/scripts/cpo.py
 trl/commands/scripts/ddpo.py
 trl/commands/scripts/dpo.py
 trl/commands/scripts/kto.py
+trl/commands/scripts/orpo.py
 trl/commands/scripts/ppo.py
 trl/commands/scripts/ppo_multi_adapter.py
 trl/commands/scripts/reward_modeling.py
 trl/commands/scripts/sft.py
+trl/commands/scripts/vsft_llava.py
 trl/commands/scripts/config/default_chat_config.yaml
 trl/environment/__init__.py
 trl/environment/base_environment.py
 trl/extras/__init__.py
 trl/extras/best_of_n_sampler.py
 trl/extras/dataset_formatting.py
 trl/models/__init__.py
 trl/models/modeling_base.py
 trl/models/modeling_sd_base.py
 trl/models/modeling_value_head.py
 trl/models/sd_utils.py
 trl/models/utils.py
 trl/trainer/__init__.py
 trl/trainer/base.py
+trl/trainer/cpo_config.py
+trl/trainer/cpo_trainer.py
 trl/trainer/ddpo_config.py
 trl/trainer/ddpo_trainer.py
 trl/trainer/dpo_trainer.py
 trl/trainer/iterative_sft_trainer.py
 trl/trainer/kto_config.py
 trl/trainer/kto_trainer.py
 trl/trainer/model_config.py
+trl/trainer/orpo_config.py
+trl/trainer/orpo_trainer.py
 trl/trainer/ppo_config.py
 trl/trainer/ppo_trainer.py
 trl/trainer/reward_config.py
 trl/trainer/reward_trainer.py
 trl/trainer/sft_trainer.py
 trl/trainer/utils.py
```

### Comparing `trl-0.8.1/trl.egg-info/requires.txt` & `trl-0.8.2/trl.egg-info/requires.txt`

 * *Files identical despite different names*

