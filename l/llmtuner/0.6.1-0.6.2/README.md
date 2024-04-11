# Comparing `tmp/llmtuner-0.6.1.tar.gz` & `tmp/llmtuner-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.6.1.tar", last modified: Fri Mar 29 03:35:01 2024, max compression
+gzip compressed data, was "llmtuner-0.6.2.tar", last modified: Thu Apr 11 12:07:25 2024, max compression
```

## Comparing `llmtuner-0.6.1.tar` & `llmtuner-0.6.2.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:35:01.229349 llmtuner-0.6.1/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-03-29 03:32:57.000000 llmtuner-0.6.1/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    39488 2024-03-29 03:35:01.101348 llmtuner-0.6.1/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    37039 2024-03-29 03:32:58.000000 llmtuner-0.6.1/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-03-29 03:32:58.000000 llmtuner-0.6.1/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-03-29 03:35:01.229349 llmtuner-0.6.1/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2498 2024-03-29 03:32:58.000000 llmtuner-0.6.1/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:56.165334 llmtuner-0.6.1/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:56.357334 llmtuner-0.6.1/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-03-29 03:32:56.000000 llmtuner-0.6.1/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:56.737335 llmtuner-0.6.1/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8252 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2760 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:56.905336 llmtuner-0.6.1/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-03-29 03:32:44.000000 llmtuner-0.6.1/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1858 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/chat/base_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3334 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/chat/chat_model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9969 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/chat/hf_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5974 2024-03-29 03:32:43.000000 llmtuner-0.6.1/src/llmtuner/chat/vllm_engine.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:57.413337 llmtuner-0.6.1/src/llmtuner/data/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      257 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/data/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5505 2024-03-29 03:32:44.000000 llmtuner-0.6.1/src/llmtuner/data/aligner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-03-29 03:32:44.000000 llmtuner-0.6.1/src/llmtuner/data/formatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6849 2024-03-29 03:32:44.000000 llmtuner-0.6.1/src/llmtuner/data/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4590 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/data/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11267 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/data/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    28616 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/data/template.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3681 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/data/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:57.553338 llmtuner-0.6.1/src/llmtuner/eval/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/eval/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5718 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/eval/evaluator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-03-29 03:32:45.000000 llmtuner-0.6.1/src/llmtuner/eval/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:57.797338 llmtuner-0.6.1/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6419 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    30707 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7162 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1316 2024-03-29 03:32:46.000000 llmtuner-0.6.1/src/llmtuner/extras/packages.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:57.865339 llmtuner-0.6.1/src/llmtuner/extras/patches/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/extras/patches/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8841 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/extras/patches/llama_patch.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1852 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/extras/patches/mixtral_patch.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1832 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/extras/ploting.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:58.229340 llmtuner-0.6.1/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3871 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-03-29 03:32:47.000000 llmtuner-0.6.1/src/llmtuner/hparams/evaluation_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10454 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1915 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6773 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/hparams/model_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12677 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/hparams/parser.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:58.433340 llmtuner-0.6.1/src/llmtuner/model/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      287 2024-03-29 03:32:49.000000 llmtuner-0.6.1/src/llmtuner/model/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7413 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/model/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5361 2024-03-29 03:32:48.000000 llmtuner-0.6.1/src/llmtuner/model/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    16776 2024-03-29 03:32:49.000000 llmtuner-0.6.1/src/llmtuner/model/patcher.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4705 2024-03-29 03:32:49.000000 llmtuner-0.6.1/src/llmtuner/model/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:58.581341 llmtuner-0.6.1/src/llmtuner/train/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/train/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:58.733341 llmtuner-0.6.1/src/llmtuner/train/dpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-03-29 03:32:50.000000 llmtuner-0.6.1/src/llmtuner/train/dpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2258 2024-03-29 03:32:49.000000 llmtuner-0.6.1/src/llmtuner/train/dpo/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6926 2024-03-29 03:32:49.000000 llmtuner-0.6.1/src/llmtuner/train/dpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3079 2024-03-29 03:32:50.000000 llmtuner-0.6.1/src/llmtuner/train/dpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:58.989342 llmtuner-0.6.1/src/llmtuner/train/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-03-29 03:32:50.000000 llmtuner-0.6.1/src/llmtuner/train/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    20560 2024-03-29 03:33:03.000000 llmtuner-0.6.1/src/llmtuner/train/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-03-29 03:32:50.000000 llmtuner-0.6.1/src/llmtuner/train/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2634 2024-03-29 03:32:50.000000 llmtuner-0.6.1/src/llmtuner/train/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:59.157343 llmtuner-0.6.1/src/llmtuner/train/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-03-29 03:32:51.000000 llmtuner-0.6.1/src/llmtuner/train/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1107 2024-03-29 03:32:51.000000 llmtuner-0.6.1/src/llmtuner/train/pt/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2024-03-29 03:32:51.000000 llmtuner-0.6.1/src/llmtuner/train/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:59.377343 llmtuner-0.6.1/src/llmtuner/train/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      942 2024-03-29 03:32:51.000000 llmtuner-0.6.1/src/llmtuner/train/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-03-29 03:32:51.000000 llmtuner-0.6.1/src/llmtuner/train/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5077 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3045 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:59.585344 llmtuner-0.6.1/src/llmtuner/train/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/train/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2504 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5073 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4300 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/sft/workflow.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4124 2024-03-29 03:32:52.000000 llmtuner-0.6.1/src/llmtuner/train/tuner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13871 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/train/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:35:00.541347 llmtuner-0.6.1/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-03-29 03:32:56.000000 llmtuner-0.6.1/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5107 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/webui/chatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4102 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:35:00.905348 llmtuner-0.6.1/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2017 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3421 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2641 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3675 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1272 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2373 2024-03-29 03:32:54.000000 llmtuner-0.6.1/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9116 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/components/train.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-03-29 03:32:53.000000 llmtuner-0.6.1/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2608 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2553 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    39264 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1105 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13187 2024-03-29 03:32:55.000000 llmtuner-0.6.1/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3314 2024-03-29 03:32:56.000000 llmtuner-0.6.1/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:34:56.613335 llmtuner-0.6.1/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    39488 2024-03-29 03:34:55.000000 llmtuner-0.6.1/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2984 2024-03-29 03:34:56.000000 llmtuner-0.6.1/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-03-29 03:34:55.000000 llmtuner-0.6.1/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      536 2024-03-29 03:34:55.000000 llmtuner-0.6.1/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-03-29 03:34:55.000000 llmtuner-0.6.1/src/llmtuner.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-03-29 03:35:00.997348 llmtuner-0.6.1/tests/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-03-29 03:32:56.000000 llmtuner-0.6.1/tests/test_throughput.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2399 2024-03-29 03:32:56.000000 llmtuner-0.6.1/tests/test_toolcall.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.949448 llmtuner-0.6.2/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-11 12:07:00.000000 llmtuner-0.6.2/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    32281 2024-04-11 12:07:24.913448 llmtuner-0.6.2/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    29705 2024-04-11 12:07:00.000000 llmtuner-0.6.2/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-11 12:07:00.000000 llmtuner-0.6.2/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-11 12:07:24.949448 llmtuner-0.6.2/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2572 2024-04-11 12:07:00.000000 llmtuner-0.6.2/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.641434 llmtuner-0.6.2/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.765434 llmtuner-0.6.2/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-11 12:06:59.000000 llmtuner-0.6.2/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.153435 llmtuner-0.6.2/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.389436 llmtuner-0.6.2/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1858 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/base_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3334 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/chat_model.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    10056 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/hf_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5974 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/chat/vllm_engine.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.869438 llmtuner-0.6.2/src/llmtuner/data/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/data/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5505 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/aligner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/formatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7364 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4989 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11328 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    29041 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/template.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.049438 llmtuner-0.6.2/src/llmtuner/eval/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/evaluator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.361440 llmtuner-0.6.2/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    32324 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7411 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1316 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/packages.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.409440 llmtuner-0.6.2/src/llmtuner/extras/patches/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/patches/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8841 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/patches/llama_patch.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/ploting.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.729441 llmtuner-0.6.2/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3871 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/evaluation_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    10631 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1915 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7154 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/model_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12665 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/parser.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.909441 llmtuner-0.6.2/src/llmtuner/model/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      229 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7413 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4780 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18170 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/patcher.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5277 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.053442 llmtuner-0.6.2/src/llmtuner/train/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.169442 llmtuner-0.6.2/src/llmtuner/train/dpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7335 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3090 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.289443 llmtuner-0.6.2/src/llmtuner/train/orpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5517 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2654 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.445443 llmtuner-0.6.2/src/llmtuner/train/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    20565 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2634 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.673444 llmtuner-0.6.2/src/llmtuner/train/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1107 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.905445 llmtuner-0.6.2/src/llmtuner/train/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5077 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3041 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.085446 llmtuner-0.6.2/src/llmtuner/train/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2504 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5073 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4300 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/workflow.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3969 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/tuner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14011 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.401446 llmtuner-0.6.2/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-11 12:06:59.000000 llmtuner-0.6.2/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4997 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/chatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4799 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.713448 llmtuner-0.6.2/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2021 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3393 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2719 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3671 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1274 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2313 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9869 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/components/train.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2784 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2519 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    42316 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2004 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16024 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3260 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.977435 llmtuner-0.6.2/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    32281 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3007 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      580 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.829448 llmtuner-0.6.2/tests/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-11 12:06:59.000000 llmtuner-0.6.2/tests/test_throughput.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-11 12:06:59.000000 llmtuner-0.6.2/tests/test_toolcall.py
```

### Comparing `llmtuner-0.6.1/LICENSE` & `llmtuner-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/PKG-INFO` & `llmtuner-0.6.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.6.1
+Version: 0.6.2
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -24,60 +24,63 @@
 License-File: LICENSE
 Requires-Dist: torch>=1.13.1
 Requires-Dist: transformers>=4.37.2
 Requires-Dist: datasets>=2.14.3
 Requires-Dist: accelerate>=0.27.2
 Requires-Dist: peft>=0.10.0
 Requires-Dist: trl>=0.8.1
-Requires-Dist: gradio<4.0.0,>=3.38.0
+Requires-Dist: gradio<=4.21.0,>=4.0.0
 Requires-Dist: scipy
 Requires-Dist: einops
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
 Requires-Dist: fastapi
 Requires-Dist: sse-starlette
 Requires-Dist: matplotlib
 Requires-Dist: fire
-Requires-Dist: galore-torch
 Provides-Extra: deepspeed
-Requires-Dist: deepspeed; extra == "deepspeed"
+Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
 Provides-Extra: metrics
 Requires-Dist: nltk; extra == "metrics"
 Requires-Dist: jieba; extra == "metrics"
 Requires-Dist: rouge-chinese; extra == "metrics"
 Provides-Extra: unsloth
 Requires-Dist: torch==2.2.0; extra == "unsloth"
 Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
+Provides-Extra: galore
+Requires-Dist: galore-torch; extra == "galore"
 Provides-Extra: vllm
 Requires-Dist: vllm>=0.3.3; extra == "vllm"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
 Requires-Dist: optimum>=1.16.0; extra == "gptq"
 Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
 Provides-Extra: awq
 Requires-Dist: autoawq; extra == "awq"
 Provides-Extra: aqlm
 Requires-Dist: aqlm[gpu]>=1.1.0; extra == "aqlm"
 Provides-Extra: qwen
 Requires-Dist: tiktoken; extra == "qwen"
 Requires-Dist: transformers_stream_generator; extra == "qwen"
+Provides-Extra: modelscope
+Requires-Dist: modelscope; extra == "modelscope"
 Provides-Extra: quality
 Requires-Dist: ruff; extra == "quality"
 
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-27-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-28-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
@@ -108,48 +111,50 @@
 - [License](#license)
 - [Citation](#citation)
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
 - **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
-- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO and DPO.
+- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
 - **Advanced algorithms**: GaLore, DoRA, LongLoRA, LLaMA Pro, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
 
-Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA-Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA-Factory's QLoRA further improves the efficiency regarding the GPU memory.
+Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA Factory's QLoRA further improves the efficiency regarding the GPU memory.
 
 ![benchmark](assets/benchmark.svg)
 
 <details><summary>Definitions</summary>
 
 - **Training Speed**: the number of training samples processed per second during the training. (bs=4, cutoff_len=1024)
 - **Rouge Score**: Rouge-2 score on the development set of the [advertising text generation](https://aclanthology.org/D19-1321.pdf) task. (bs=4, cutoff_len=1024)
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
-- We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA-Factory's LoRA tuning.
+- We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
+[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
+
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
-[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/fsdp_qlora` for usage.
+[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
+
+<details><summary>Full Changelog</summary>
 
 [24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
 
 [24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
 
-<details><summary>Full Changelog</summary>
-
 [24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
 
 [24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
 
 [24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See `examples/extras/llama_pro` for usage.
 
 [24/02/05] Qwen1.5 (Qwen2 beta version) series models are supported in LLaMA-Factory. Check this [blog post](https://qwenlm.github.io/blog/qwen1.5/) for details.
@@ -200,20 +205,19 @@
 | [ChatGLM3](https://huggingface.co/THUDM/chatglm3-6b)     | 6B                          | query_key_value   | chatglm3  |
 | [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
 | [Gemma](https://huggingface.co/google)                   | 2B/7B                       | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [Mistral](https://huggingface.co/mistralai)              | 7B                          | q_proj,v_proj     | mistral   |
-| [Mixtral](https://huggingface.co/mistralai)              | 8x7B                        | q_proj,v_proj     | mistral   |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B                     | q_proj,v_proj     | mistral   |
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5](https://huggingface.co/Qwen)                   | 0.5B/1.8B/4B/7B/14B/72B     | q_proj,v_proj     | qwen      |
+| [Qwen1.5 (MoE)](https://huggingface.co/Qwen)             | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
 | [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
@@ -229,17 +233,15 @@
 | Approach               |     Full-tuning    |    Freeze-tuning   |       LoRA         |       QLoRA        |
 | ---------------------- | ------------------ | ------------------ | ------------------ | ------------------ |
 | Pre-Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | Supervised Fine-Tuning | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | Reward Modeling        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | PPO Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | DPO Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
-
-> [!NOTE]
-> Use `--quantization_bit 4` argument to enable QLoRA.
+| ORPO Training          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 ## Provided Datasets
 
 <details><summary>Pre-training datasets</summary>
 
 - [Wiki Demo (en)](data/wiki_demo.txt)
 - [RefinedWeb (en)](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)
@@ -310,31 +312,29 @@
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
-Please refer to [data/README.md](data/README.md) for details.
-
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
 pip install --upgrade huggingface_hub
 huggingface-cli login
 ```
 
 ## Requirement
 
 | Mandatory    | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | python       | 3.8     | 3.10      |
 | torch        | 1.13.1  | 2.2.0     |
-| transformers | 4.37.2  | 4.39.1    |
-| datasets     | 2.14.3  | 2.17.1    |
+| transformers | 4.37.2  | 4.39.3    |
+| datasets     | 2.14.3  | 2.18.0    |
 | accelerate   | 0.27.2  | 0.28.0    |
 | peft         | 0.9.0   | 0.10.0    |
 | trl          | 0.8.1   | 0.8.1     |
 
 | Optional     | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | CUDA         | 11.6    | 12.2      |
@@ -355,414 +355,117 @@
 | LoRA   |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
 | QLoRA  |   8  |  10GB |  20GB |  40GB |   80GB |   60GB |
 | QLoRA  |   4  |   6GB |  12GB |  24GB |   48GB |   30GB |
 | QLoRA  |   2  |   4GB |   8GB |  16GB |   24GB |   18GB |
 
 ## Getting Started
 
-### Data Preparation (optional)
+### Data Preparation
 
-Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use a single `.json` file or a [dataset loading script](https://huggingface.co/docs/datasets/dataset_script) with multiple files to create a custom dataset.
+Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
 > [!NOTE]
-> Please update `data/dataset_info.json` to use your custom dataset. About the format of this file, please refer to `data/README.md`.
+> Please update `data/dataset_info.json` to use your custom dataset.
 
-### Dependence Installation (optional)
+### Dependence Installation
 
 ```bash
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
-pip install -r requirements.txt
+pip install -e .[metrics]
 ```
 
+Extra dependencies available: deepspeed, metrics, unsloth, galore, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+
+<details><summary>For Windows users</summary>
+
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
-### Use ModelScope Hub (optional)
-
-If you have trouble with downloading models and datasets from Hugging Face, you can use LLaMA-Factory together with ModelScope in the following manner.
-
-```bash
-export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
-```
-
-Then you can train the corresponding model by specifying a model ID of the ModelScope Hub. (find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models))
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --model_name_or_path modelscope/Llama-2-7b-ms \
-    ... # arguments (same as below)
-```
-
-LLaMA Board also supports using the models and datasets on the ModelScope Hub.
-
-```bash
-CUDA_VISIBLE_DEVICES=0 USE_MODELSCOPE_HUB=1 python src/train_web.py
-```
+</details>
 
-### Train on a single GPU
+### LLaMA Board GUI
 
 > [!IMPORTANT]
-> If you want to train models on multiple GPUs, please refer to [Distributed Training](#distributed-training).
-
-
-#### LLaMA Board GUI
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_web.py
-```
+> LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
-#### Pre-Training
+#### Use local environment
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage pt \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --dataset wiki_demo \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_pt_checkpoint \
-    --overwrite_cache \
-    --per_device_train_batch_size 4 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 5e-5 \
-    --num_train_epochs 3.0 \
-    --plot_loss \
-    --fp16
+export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
+python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
-#### Supervised Fine-Tuning
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage sft \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_sft_checkpoint \
-    --overwrite_cache \
-    --per_device_train_batch_size 4 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 5e-5 \
-    --num_train_epochs 3.0 \
-    --plot_loss \
-    --fp16
-```
-
-#### Reward Modeling
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage rm \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset comparison_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_rm_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-#### PPO Training
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage ppo \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --reward_model path_to_rm_checkpoint \
-    --output_dir path_to_ppo_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --top_k 0 \
-    --top_p 0.9 \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-> [!TIP]
-> Use `--adapter_name_or_path path_to_sft_checkpoint,path_to_ppo_checkpoint` to infer the fine-tuned model if `--create_new_adapter` was enabled.
-
-> [!WARNING]
-> Use `--per_device_train_batch_size=1` for LLaMA-2 models in fp16 PPO training.
-
-#### DPO Training
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage dpo \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset comparison_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_dpo_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-> [!TIP]
-> Use `--adapter_name_or_path path_to_sft_checkpoint,path_to_dpo_checkpoint` to infer the fine-tuned model if `--create_new_adapter` was enabled.
-
-### Distributed Training
-
-#### Use Huggingface Accelerate
+#### Use Docker
 
 ```bash
-accelerate launch --config_file config.yaml src/train_bash.py \
-    --ddp_timeout 180000000 \
-    ... # arguments (same as above)
-```
-
-<details><summary>Example config.yaml for LoRA training</summary>
-
-```yaml
-compute_environment: LOCAL_MACHINE
-debug: false
-distributed_type: MULTI_GPU
-downcast_bf16: 'no'
-gpu_ids: all
-machine_rank: 0
-main_training_function: main
-mixed_precision: fp16
-num_machines: 1
-num_processes: 4
-rdzv_backend: static
-same_network: true
-tpu_env: []
-tpu_use_cluster: false
-tpu_use_sudo: false
-use_cpu: false
+docker build -f ./Dockerfile -t llama-factory:latest .
+docker run --gpus=all \
+    -v ./hf_cache:/root/.cache/huggingface/ \
+    -v ./data:/app/data \
+    -v ./output:/app/output \
+    -e CUDA_VISIBLE_DEVICES=0 \
+    -p 7860:7860 \
+    --shm-size 16G \
+    --name llama_factory \
+    -d llama-factory:latest
 ```
 
-</details>
-
-> [!TIP]
-> We commend using Accelerate for LoRA tuning.
-
-#### Use DeepSpeed
+#### Use Docker Compose
 
 ```bash
-deepspeed --num_gpus 8 src/train_bash.py \
-    --deepspeed ds_config.json \
-    --ddp_timeout 180000000 \
-    ... # arguments (same as above)
+docker compose -f ./docker-compose.yml up -d
 ```
 
-<details><summary>Example ds_config.json for full-parameter training with DeepSpeed ZeRO-2</summary>
+<details><summary>Details about volume</summary>
 
-```json
-{
-  "train_batch_size": "auto",
-  "train_micro_batch_size_per_gpu": "auto",
-  "gradient_accumulation_steps": "auto",
-  "gradient_clipping": "auto",
-  "zero_allow_untested_optimizer": true,
-  "fp16": {
-    "enabled": "auto",
-    "loss_scale": 0,
-    "loss_scale_window": 1000,
-    "initial_scale_power": 16,
-    "hysteresis": 2,
-    "min_loss_scale": 1
-  },
-  "bf16": {
-    "enabled": "auto"
-  },
-  "zero_optimization": {
-    "stage": 2,
-    "allgather_partitions": true,
-    "allgather_bucket_size": 5e8,
-    "overlap_comm": true,
-    "reduce_scatter": true,
-    "reduce_bucket_size": 5e8,
-    "contiguous_gradients": true,
-    "round_robin_gradients": true
-  }
-}
-```
+- hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
+- data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
+- output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-> [!TIP]
-> Refer to [examples](examples) for more training scripts.
-
-### Merge LoRA weights and export model
-
-```bash
-CUDA_VISIBLE_DEVICES= python src/export_model.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora \
-    --export_dir path_to_export \
-    --export_size 2 \
-    --export_legacy_format False
-```
-
-> [!WARNING]
-> Merging LoRA weights into a quantized model is not supported.
-
-> [!TIP]
-> Use `--model_name_or_path path_to_export` solely to use the exported model.
-> 
-> Use `CUDA_VISIBLE_DEVICES=0`, `--export_quantization_bit 4` and `--export_quantization_dataset data/c4_demo.json` to quantize the model with AutoGPTQ after merging the LoRA weights.
-
-### Inference with OpenAI-style API
-
-```bash
-CUDA_VISIBLE_DEVICES=0 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
-```
-
-> [!TIP]
-> Visit `http://localhost:8000/docs` for API documentation.
-
-### Inference with command line
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/cli_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
-```
-
-### Inference with web browser
+### Command Line Interface
 
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/web_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
-```
+See [examples/README.md](examples/README.md) for usage.
 
-### Evaluation
+Use `python src/train_bash.py -h` to display arguments description.
 
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/evaluate.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template vanilla \
-    --finetuning_type lora \
-    --task mmlu \
-    --split test \
-    --lang en \
-    --n_shot 5 \
-    --batch_size 4
-```
-
-### Predict
+### Deploy with OpenAI-style API and vLLM
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage sft \
-    --do_predict \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --output_dir path_to_predict_result \
-    --per_device_eval_batch_size 1 \
-    --max_samples 100 \
-    --predict_with_generate \
-    --fp16
+CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
+    --model_name_or_path mistralai/Mistral-7B-Instruct-v0.2 \
+    --template mistral \
+    --infer_backend vllm \
+    --vllm_enforce_eager
 ```
 
-> [!WARNING]
-> Use `--per_device_train_batch_size=1` for LLaMA-2 models in fp16 predict.
-
-> [!TIP]
-> We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit predict.
+### Use ModelScope Hub
 
-### Dockerize Training
-
-#### Use Docker
+If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
-docker build -f ./Dockerfile -t llama-factory:latest .
-
-docker run --gpus=all \
-    -v ./hf_cache:/root/.cache/huggingface/ \
-    -v ./data:/app/data \
-    -v ./output:/app/output \
-    -e CUDA_VISIBLE_DEVICES=0 \
-    -p 7860:7860 \
-    --shm-size 16G \
-    --name llama_factory \
-    -d llama-factory:latest
+export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
 ```
 
-#### Use Docker Compose
+Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `modelscope/Llama-2-7b-ms`.
 
-```bash
-docker compose -f ./docker-compose.yml up -d
-```
+## Projects using LLaMA Factory
 
-> [!TIP]
-> Details about volume:
-> * hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
-> * data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
-> * output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
+If you have a project that should be incorporated, please contact via email or create a pull request.
 
-## Projects using LLaMA Factory
+<details><summary>Click to show</summary>
 
 1. Wang et al. ESRL: Efficient Sampling-based Reinforcement Learning for Sequence Generation. 2023. [[arxiv]](https://arxiv.org/abs/2308.02223)
 1. Yu et al. Open, Closed, or Small Language Models for Text Classification? 2023. [[arxiv]](https://arxiv.org/abs/2308.10092)
 1. Wang et al. UbiPhysio: Support Daily Functioning, Fitness, and Rehabilitation with Action Understanding and Feedback in Natural Language. 2023. [[arxiv]](https://arxiv.org/abs/2308.10526)
 1. Luceri et al. Leveraging Large Language Models to Detect Influence Campaigns in Social Media. 2023. [[arxiv]](https://arxiv.org/abs/2311.07816)
 1. Zhang et al. Alleviating Hallucinations of Large Language Models through Induced Hallucinations. 2023. [[arxiv]](https://arxiv.org/abs/2312.15710)
 1. Wang et al. Know Your Needs Better: Towards Structured Understanding of Marketer Demands with Analogical Reasoning Augmented LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2401.04319)
@@ -777,44 +480,44 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
 
-> [!TIP]
-> If you have a project that should be incorporated, please contact via email or create a pull request.
+</details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
-  title={LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models}, 
+  title={LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models},
   author={Yaowei Zheng and Richong Zhang and Junhao Zhang and Yanhan Ye and Zheyan Luo and Yongqiang Ma},
   journal={arXiv preprint arXiv:2403.13372},
   year={2024},
   url={http://arxiv.org/abs/2403.13372}
 }
 ```
 
 ## Acknowledgement
 
-This repo benefits from [PEFT](https://github.com/huggingface/peft), [QLoRA](https://github.com/artidoro/qlora) and [FastChat](https://github.com/lm-sys/FastChat). Thanks for their wonderful works.
+This repo benefits from [PEFT](https://github.com/huggingface/peft), [TRL](https://github.com/huggingface/trl), [QLoRA](https://github.com/artidoro/qlora) and [FastChat](https://github.com/lm-sys/FastChat). Thanks for their wonderful works.
 
 ## Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=hiyouga/LLaMA-Factory&type=Date)
```

### Comparing `llmtuner-0.6.1/README.md` & `llmtuner-0.6.2/src/llmtuner.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,86 @@
+Metadata-Version: 2.1
+Name: llmtuner
+Version: 0.6.2
+Summary: Easy-to-use LLM fine-tuning framework
+Home-page: https://github.com/hiyouga/LLaMA-Factory
+Author: hiyouga
+Author-email: hiyouga@buaa.edu.cn
+License: Apache 2.0 License
+Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch>=1.13.1
+Requires-Dist: transformers>=4.37.2
+Requires-Dist: datasets>=2.14.3
+Requires-Dist: accelerate>=0.27.2
+Requires-Dist: peft>=0.10.0
+Requires-Dist: trl>=0.8.1
+Requires-Dist: gradio<=4.21.0,>=4.0.0
+Requires-Dist: scipy
+Requires-Dist: einops
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf
+Requires-Dist: uvicorn
+Requires-Dist: pydantic
+Requires-Dist: fastapi
+Requires-Dist: sse-starlette
+Requires-Dist: matplotlib
+Requires-Dist: fire
+Provides-Extra: deepspeed
+Requires-Dist: deepspeed>=0.10.0; extra == "deepspeed"
+Provides-Extra: metrics
+Requires-Dist: nltk; extra == "metrics"
+Requires-Dist: jieba; extra == "metrics"
+Requires-Dist: rouge-chinese; extra == "metrics"
+Provides-Extra: unsloth
+Requires-Dist: torch==2.2.0; extra == "unsloth"
+Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
+Provides-Extra: galore
+Requires-Dist: galore-torch; extra == "galore"
+Provides-Extra: vllm
+Requires-Dist: vllm>=0.3.3; extra == "vllm"
+Provides-Extra: bitsandbytes
+Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
+Provides-Extra: gptq
+Requires-Dist: optimum>=1.16.0; extra == "gptq"
+Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
+Provides-Extra: awq
+Requires-Dist: autoawq; extra == "awq"
+Provides-Extra: aqlm
+Requires-Dist: aqlm[gpu]>=1.1.0; extra == "aqlm"
+Provides-Extra: qwen
+Requires-Dist: tiktoken; extra == "qwen"
+Requires-Dist: transformers_stream_generator; extra == "qwen"
+Provides-Extra: modelscope
+Requires-Dist: modelscope; extra == "modelscope"
+Provides-Extra: quality
+Requires-Dist: ruff; extra == "quality"
+
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-27-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-28-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
@@ -40,48 +111,50 @@
 - [License](#license)
 - [Citation](#citation)
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
 - **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
-- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO and DPO.
+- **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
 - **Advanced algorithms**: GaLore, DoRA, LongLoRA, LLaMA Pro, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
 
-Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA-Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA-Factory's QLoRA further improves the efficiency regarding the GPU memory.
+Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA Factory's QLoRA further improves the efficiency regarding the GPU memory.
 
 ![benchmark](assets/benchmark.svg)
 
 <details><summary>Definitions</summary>
 
 - **Training Speed**: the number of training samples processed per second during the training. (bs=4, cutoff_len=1024)
 - **Rouge Score**: Rouge-2 score on the development set of the [advertising text generation](https://aclanthology.org/D19-1321.pdf) task. (bs=4, cutoff_len=1024)
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
-- We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA-Factory's LoRA tuning.
+- We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
+[24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
+
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
-[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/fsdp_qlora` for usage.
+[24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
+
+<details><summary>Full Changelog</summary>
 
 [24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
 
 [24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
 
-<details><summary>Full Changelog</summary>
-
 [24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
 
 [24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
 
 [24/02/15] We supported **block expansion** proposed by [LLaMA Pro](https://github.com/TencentARC/LLaMA-Pro). See `examples/extras/llama_pro` for usage.
 
 [24/02/05] Qwen1.5 (Qwen2 beta version) series models are supported in LLaMA-Factory. Check this [blog post](https://qwenlm.github.io/blog/qwen1.5/) for details.
@@ -132,20 +205,19 @@
 | [ChatGLM3](https://huggingface.co/THUDM/chatglm3-6b)     | 6B                          | query_key_value   | chatglm3  |
 | [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
 | [Gemma](https://huggingface.co/google)                   | 2B/7B                       | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [Mistral](https://huggingface.co/mistralai)              | 7B                          | q_proj,v_proj     | mistral   |
-| [Mixtral](https://huggingface.co/mistralai)              | 8x7B                        | q_proj,v_proj     | mistral   |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B                     | q_proj,v_proj     | mistral   |
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5](https://huggingface.co/Qwen)                   | 0.5B/1.8B/4B/7B/14B/72B     | q_proj,v_proj     | qwen      |
+| [Qwen1.5 (MoE)](https://huggingface.co/Qwen)             | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
 | [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
@@ -161,17 +233,15 @@
 | Approach               |     Full-tuning    |    Freeze-tuning   |       LoRA         |       QLoRA        |
 | ---------------------- | ------------------ | ------------------ | ------------------ | ------------------ |
 | Pre-Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | Supervised Fine-Tuning | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | Reward Modeling        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | PPO Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | DPO Training           | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
-
-> [!NOTE]
-> Use `--quantization_bit 4` argument to enable QLoRA.
+| ORPO Training          | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 
 ## Provided Datasets
 
 <details><summary>Pre-training datasets</summary>
 
 - [Wiki Demo (en)](data/wiki_demo.txt)
 - [RefinedWeb (en)](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)
@@ -242,31 +312,29 @@
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
-Please refer to [data/README.md](data/README.md) for details.
-
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
 pip install --upgrade huggingface_hub
 huggingface-cli login
 ```
 
 ## Requirement
 
 | Mandatory    | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | python       | 3.8     | 3.10      |
 | torch        | 1.13.1  | 2.2.0     |
-| transformers | 4.37.2  | 4.39.1    |
-| datasets     | 2.14.3  | 2.17.1    |
+| transformers | 4.37.2  | 4.39.3    |
+| datasets     | 2.14.3  | 2.18.0    |
 | accelerate   | 0.27.2  | 0.28.0    |
 | peft         | 0.9.0   | 0.10.0    |
 | trl          | 0.8.1   | 0.8.1     |
 
 | Optional     | Minimum | Recommend |
 | ------------ | ------- | --------- |
 | CUDA         | 11.6    | 12.2      |
@@ -287,414 +355,117 @@
 | LoRA   |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
 | QLoRA  |   8  |  10GB |  20GB |  40GB |   80GB |   60GB |
 | QLoRA  |   4  |   6GB |  12GB |  24GB |   48GB |   30GB |
 | QLoRA  |   2  |   4GB |   8GB |  16GB |   24GB |   18GB |
 
 ## Getting Started
 
-### Data Preparation (optional)
+### Data Preparation
 
-Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use a single `.json` file or a [dataset loading script](https://huggingface.co/docs/datasets/dataset_script) with multiple files to create a custom dataset.
+Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
 > [!NOTE]
-> Please update `data/dataset_info.json` to use your custom dataset. About the format of this file, please refer to `data/README.md`.
+> Please update `data/dataset_info.json` to use your custom dataset.
 
-### Dependence Installation (optional)
+### Dependence Installation
 
 ```bash
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
-pip install -r requirements.txt
+pip install -e .[metrics]
 ```
 
+Extra dependencies available: deepspeed, metrics, unsloth, galore, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+
+<details><summary>For Windows users</summary>
+
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
 ```
 
 To enable FlashAttention-2 on the Windows platform, you need to install the precompiled `flash-attn` library, which supports CUDA 12.1 to 12.2. Please download the corresponding version from [flash-attention](https://github.com/bdashore3/flash-attention/releases) based on your requirements.
 
-### Use ModelScope Hub (optional)
-
-If you have trouble with downloading models and datasets from Hugging Face, you can use LLaMA-Factory together with ModelScope in the following manner.
-
-```bash
-export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
-```
-
-Then you can train the corresponding model by specifying a model ID of the ModelScope Hub. (find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models))
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --model_name_or_path modelscope/Llama-2-7b-ms \
-    ... # arguments (same as below)
-```
-
-LLaMA Board also supports using the models and datasets on the ModelScope Hub.
-
-```bash
-CUDA_VISIBLE_DEVICES=0 USE_MODELSCOPE_HUB=1 python src/train_web.py
-```
+</details>
 
-### Train on a single GPU
+### LLaMA Board GUI
 
 > [!IMPORTANT]
-> If you want to train models on multiple GPUs, please refer to [Distributed Training](#distributed-training).
-
+> LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
-#### LLaMA Board GUI
+#### Use local environment
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_web.py
+export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
+python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
-#### Pre-Training
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage pt \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --dataset wiki_demo \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_pt_checkpoint \
-    --overwrite_cache \
-    --per_device_train_batch_size 4 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 5e-5 \
-    --num_train_epochs 3.0 \
-    --plot_loss \
-    --fp16
-```
-
-#### Supervised Fine-Tuning
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage sft \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_sft_checkpoint \
-    --overwrite_cache \
-    --per_device_train_batch_size 4 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 5e-5 \
-    --num_train_epochs 3.0 \
-    --plot_loss \
-    --fp16
-```
-
-#### Reward Modeling
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage rm \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset comparison_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_rm_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-#### PPO Training
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage ppo \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --reward_model path_to_rm_checkpoint \
-    --output_dir path_to_ppo_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --top_k 0 \
-    --top_p 0.9 \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-> [!TIP]
-> Use `--adapter_name_or_path path_to_sft_checkpoint,path_to_ppo_checkpoint` to infer the fine-tuned model if `--create_new_adapter` was enabled.
-
-> [!WARNING]
-> Use `--per_device_train_batch_size=1` for LLaMA-2 models in fp16 PPO training.
-
-#### DPO Training
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage dpo \
-    --do_train \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_sft_checkpoint \
-    --create_new_adapter \
-    --dataset comparison_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --lora_target q_proj,v_proj \
-    --output_dir path_to_dpo_checkpoint \
-    --per_device_train_batch_size 2 \
-    --gradient_accumulation_steps 4 \
-    --lr_scheduler_type cosine \
-    --logging_steps 10 \
-    --save_steps 1000 \
-    --learning_rate 1e-5 \
-    --num_train_epochs 1.0 \
-    --plot_loss \
-    --fp16
-```
-
-> [!TIP]
-> Use `--adapter_name_or_path path_to_sft_checkpoint,path_to_dpo_checkpoint` to infer the fine-tuned model if `--create_new_adapter` was enabled.
-
-### Distributed Training
-
-#### Use Huggingface Accelerate
+#### Use Docker
 
 ```bash
-accelerate launch --config_file config.yaml src/train_bash.py \
-    --ddp_timeout 180000000 \
-    ... # arguments (same as above)
-```
-
-<details><summary>Example config.yaml for LoRA training</summary>
-
-```yaml
-compute_environment: LOCAL_MACHINE
-debug: false
-distributed_type: MULTI_GPU
-downcast_bf16: 'no'
-gpu_ids: all
-machine_rank: 0
-main_training_function: main
-mixed_precision: fp16
-num_machines: 1
-num_processes: 4
-rdzv_backend: static
-same_network: true
-tpu_env: []
-tpu_use_cluster: false
-tpu_use_sudo: false
-use_cpu: false
+docker build -f ./Dockerfile -t llama-factory:latest .
+docker run --gpus=all \
+    -v ./hf_cache:/root/.cache/huggingface/ \
+    -v ./data:/app/data \
+    -v ./output:/app/output \
+    -e CUDA_VISIBLE_DEVICES=0 \
+    -p 7860:7860 \
+    --shm-size 16G \
+    --name llama_factory \
+    -d llama-factory:latest
 ```
 
-</details>
-
-> [!TIP]
-> We commend using Accelerate for LoRA tuning.
-
-#### Use DeepSpeed
+#### Use Docker Compose
 
 ```bash
-deepspeed --num_gpus 8 src/train_bash.py \
-    --deepspeed ds_config.json \
-    --ddp_timeout 180000000 \
-    ... # arguments (same as above)
+docker compose -f ./docker-compose.yml up -d
 ```
 
-<details><summary>Example ds_config.json for full-parameter training with DeepSpeed ZeRO-2</summary>
+<details><summary>Details about volume</summary>
 
-```json
-{
-  "train_batch_size": "auto",
-  "train_micro_batch_size_per_gpu": "auto",
-  "gradient_accumulation_steps": "auto",
-  "gradient_clipping": "auto",
-  "zero_allow_untested_optimizer": true,
-  "fp16": {
-    "enabled": "auto",
-    "loss_scale": 0,
-    "loss_scale_window": 1000,
-    "initial_scale_power": 16,
-    "hysteresis": 2,
-    "min_loss_scale": 1
-  },
-  "bf16": {
-    "enabled": "auto"
-  },
-  "zero_optimization": {
-    "stage": 2,
-    "allgather_partitions": true,
-    "allgather_bucket_size": 5e8,
-    "overlap_comm": true,
-    "reduce_scatter": true,
-    "reduce_bucket_size": 5e8,
-    "contiguous_gradients": true,
-    "round_robin_gradients": true
-  }
-}
-```
+- hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
+- data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
+- output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
 
 </details>
 
-> [!TIP]
-> Refer to [examples](examples) for more training scripts.
+### Command Line Interface
 
-### Merge LoRA weights and export model
+See [examples/README.md](examples/README.md) for usage.
 
-```bash
-CUDA_VISIBLE_DEVICES= python src/export_model.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora \
-    --export_dir path_to_export \
-    --export_size 2 \
-    --export_legacy_format False
-```
-
-> [!WARNING]
-> Merging LoRA weights into a quantized model is not supported.
-
-> [!TIP]
-> Use `--model_name_or_path path_to_export` solely to use the exported model.
-> 
-> Use `CUDA_VISIBLE_DEVICES=0`, `--export_quantization_bit 4` and `--export_quantization_dataset data/c4_demo.json` to quantize the model with AutoGPTQ after merging the LoRA weights.
-
-### Inference with OpenAI-style API
-
-```bash
-CUDA_VISIBLE_DEVICES=0 API_PORT=8000 python src/api_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
-```
+Use `python src/train_bash.py -h` to display arguments description.
 
-> [!TIP]
-> Visit `http://localhost:8000/docs` for API documentation.
-
-### Inference with command line
+### Deploy with OpenAI-style API and vLLM
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/cli_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
+CUDA_VISIBLE_DEVICES=0,1 API_PORT=8000 python src/api_demo.py \
+    --model_name_or_path mistralai/Mistral-7B-Instruct-v0.2 \
+    --template mistral \
+    --infer_backend vllm \
+    --vllm_enforce_eager
 ```
 
-### Inference with web browser
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/web_demo.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template default \
-    --finetuning_type lora
-```
+### Use ModelScope Hub
 
-### Evaluation
+If you have trouble with downloading models and datasets from Hugging Face, you can use ModelScope.
 
 ```bash
-CUDA_VISIBLE_DEVICES=0 python src/evaluate.py \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --template vanilla \
-    --finetuning_type lora \
-    --task mmlu \
-    --split test \
-    --lang en \
-    --n_shot 5 \
-    --batch_size 4
-```
-
-### Predict
-
-```bash
-CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
-    --stage sft \
-    --do_predict \
-    --model_name_or_path path_to_llama_model \
-    --adapter_name_or_path path_to_checkpoint \
-    --dataset alpaca_gpt4_en \
-    --template default \
-    --finetuning_type lora \
-    --output_dir path_to_predict_result \
-    --per_device_eval_batch_size 1 \
-    --max_samples 100 \
-    --predict_with_generate \
-    --fp16
-```
-
-> [!WARNING]
-> Use `--per_device_train_batch_size=1` for LLaMA-2 models in fp16 predict.
-
-> [!TIP]
-> We recommend using `--per_device_eval_batch_size=1` and `--max_target_length 128` at 4/8-bit predict.
-
-### Dockerize Training
-
-#### Use Docker
-
-```bash
-docker build -f ./Dockerfile -t llama-factory:latest .
-
-docker run --gpus=all \
-    -v ./hf_cache:/root/.cache/huggingface/ \
-    -v ./data:/app/data \
-    -v ./output:/app/output \
-    -e CUDA_VISIBLE_DEVICES=0 \
-    -p 7860:7860 \
-    --shm-size 16G \
-    --name llama_factory \
-    -d llama-factory:latest
+export USE_MODELSCOPE_HUB=1 # `set USE_MODELSCOPE_HUB=1` for Windows
 ```
 
-#### Use Docker Compose
+Train the model by specifying a model ID of the ModelScope Hub as the `--model_name_or_path`. You can find a full list of model IDs at [ModelScope Hub](https://modelscope.cn/models), e.g., `modelscope/Llama-2-7b-ms`.
 
-```bash
-docker compose -f ./docker-compose.yml up -d
-```
+## Projects using LLaMA Factory
 
-> [!TIP]
-> Details about volume:
-> * hf_cache: Utilize Hugging Face cache on the host machine. Reassignable if a cache already exists in a different directory.
-> * data: Place datasets on this dir of the host machine so that they can be selected on LLaMA Board GUI.
-> * output: Set export dir to this location so that the merged result can be accessed directly on the host machine.
+If you have a project that should be incorporated, please contact via email or create a pull request.
 
-## Projects using LLaMA Factory
+<details><summary>Click to show</summary>
 
 1. Wang et al. ESRL: Efficient Sampling-based Reinforcement Learning for Sequence Generation. 2023. [[arxiv]](https://arxiv.org/abs/2308.02223)
 1. Yu et al. Open, Closed, or Small Language Models for Text Classification? 2023. [[arxiv]](https://arxiv.org/abs/2308.10092)
 1. Wang et al. UbiPhysio: Support Daily Functioning, Fitness, and Rehabilitation with Action Understanding and Feedback in Natural Language. 2023. [[arxiv]](https://arxiv.org/abs/2308.10526)
 1. Luceri et al. Leveraging Large Language Models to Detect Influence Campaigns in Social Media. 2023. [[arxiv]](https://arxiv.org/abs/2311.07816)
 1. Zhang et al. Alleviating Hallucinations of Large Language Models through Induced Hallucinations. 2023. [[arxiv]](https://arxiv.org/abs/2312.15710)
 1. Wang et al. Know Your Needs Better: Towards Structured Understanding of Marketer Demands with Analogical Reasoning Augmented LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2401.04319)
@@ -709,44 +480,44 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
 
-> [!TIP]
-> If you have a project that should be incorporated, please contact via email or create a pull request.
+</details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
-  title={LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models}, 
+  title={LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models},
   author={Yaowei Zheng and Richong Zhang and Junhao Zhang and Yanhan Ye and Zheyan Luo and Yongqiang Ma},
   journal={arXiv preprint arXiv:2403.13372},
   year={2024},
   url={http://arxiv.org/abs/2403.13372}
 }
 ```
 
 ## Acknowledgement
 
-This repo benefits from [PEFT](https://github.com/huggingface/peft), [QLoRA](https://github.com/artidoro/qlora) and [FastChat](https://github.com/lm-sys/FastChat). Thanks for their wonderful works.
+This repo benefits from [PEFT](https://github.com/huggingface/peft), [TRL](https://github.com/huggingface/trl), [QLoRA](https://github.com/artidoro/qlora) and [FastChat](https://github.com/lm-sys/FastChat). Thanks for their wonderful works.
 
 ## Star History
 
 ![Star History Chart](https://api.star-history.com/svg?repos=hiyouga/LLaMA-Factory&type=Date)
```

### Comparing `llmtuner-0.6.1/pyproject.toml` & `llmtuner-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/setup.py` & `llmtuner-0.6.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     with open("requirements.txt", "r", encoding="utf-8") as f:
         file_content = f.read()
         lines = [line.strip() for line in file_content.strip().split("\n") if not line.startswith("#")]
         return lines
 
 
 extra_require = {
-    "deepspeed": ["deepspeed"],
+    "deepspeed": ["deepspeed>=0.10.0"],
     "metrics": ["nltk", "jieba", "rouge-chinese"],
     "unsloth": ["torch==2.2.0", "unsloth[cu121-ampere-torch220]"],
+    "galore": ["galore-torch"],
     "vllm": ["vllm>=0.3.3"],
     "bitsandbytes": ["bitsandbytes>=0.39.0"],
     "gptq": ["optimum>=1.16.0", "auto-gptq>=0.5.0"],
     "awq": ["autoawq"],
     "aqlm": ["aqlm[gpu]>=1.1.0"],
     "qwen": ["tiktoken", "transformers_stream_generator"],
+    "modelscope": ["modelscope"],
     "quality": ["ruff"],
 }
 
 
 def main():
     setup(
         name="llmtuner",
```

### Comparing `llmtuner-0.6.1/src/llmtuner/api/app.py` & `llmtuner-0.6.2/src/llmtuner/api/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,20 +104,26 @@
         input_messages = []
         for i, message in enumerate(request.messages):
             if i % 2 == 0 and message.role not in [Role.USER, Role.TOOL]:
                 raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
             elif i % 2 == 1 and message.role not in [Role.ASSISTANT, Role.FUNCTION]:
                 raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid role")
 
-            input_messages.append({"role": role_mapping[message.role], "content": message.content})
+            if message.role == Role.ASSISTANT and isinstance(message.tool_calls, list) and len(message.tool_calls):
+                name = message.tool_calls[0].function.name
+                arguments = message.tool_calls[0].function.arguments
+                content = json.dumps({"name": name, "argument": arguments}, ensure_ascii=False)
+                input_messages.append({"role": role_mapping[Role.FUNCTION], "content": content})
+            else:
+                input_messages.append({"role": role_mapping[message.role], "content": message.content})
 
         tool_list = request.tools
         if isinstance(tool_list, list) and len(tool_list):
             try:
-                tools = json.dumps([tool["function"] for tool in tool_list], ensure_ascii=False)
+                tools = json.dumps([dictify(tool.function) for tool in tool_list], ensure_ascii=False)
             except Exception:
                 raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="Invalid tools")
         else:
             tools = ""
 
         if request.stream:
             if tools:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/api/protocol.py` & `llmtuner-0.6.2/src/llmtuner/api/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from enum import Enum, unique
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
 
 @unique
 class Role(str, Enum):
@@ -35,35 +35,47 @@
 
 
 class Function(BaseModel):
     name: str
     arguments: str
 
 
+class FunctionDefinition(BaseModel):
+    name: str
+    description: str
+    parameters: Dict[str, Any]
+
+
+class FunctionAvailable(BaseModel):
+    type: Literal["function", "code_interpreter"] = "function"
+    function: Optional[FunctionDefinition] = None
+
+
 class FunctionCall(BaseModel):
     id: Literal["call_default"] = "call_default"
     type: Literal["function"] = "function"
     function: Function
 
 
 class ChatMessage(BaseModel):
     role: Role
-    content: str
+    content: Optional[str] = None
+    tool_calls: Optional[List[FunctionCall]] = None
 
 
 class ChatCompletionMessage(BaseModel):
     role: Optional[Role] = None
     content: Optional[str] = None
     tool_calls: Optional[List[FunctionCall]] = None
 
 
 class ChatCompletionRequest(BaseModel):
     model: str
     messages: List[ChatMessage]
-    tools: list = []
+    tools: Optional[List[FunctionAvailable]] = None
     do_sample: bool = True
     temperature: Optional[float] = None
     top_p: Optional[float] = None
     n: int = 1
     max_tokens: Optional[int] = None
     stream: bool = False
```

### Comparing `llmtuner-0.6.1/src/llmtuner/chat/base_engine.py` & `llmtuner-0.6.2/src/llmtuner/chat/base_engine.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/chat/chat_model.py` & `llmtuner-0.6.2/src/llmtuner/chat/chat_model.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/chat/hf_engine.py` & `llmtuner-0.6.2/src/llmtuner/chat/hf_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Callable, Dict, List, Optional, Sequence, Tuple
 
 import torch
 from transformers import GenerationConfig, TextIteratorStreamer
 
 from ..data import get_template_and_fix_tokenizer
 from ..extras.misc import get_logits_processor
-from ..model import load_model_and_tokenizer
+from ..model import load_model, load_tokenizer
 from .base_engine import BaseEngine, Response
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel, PreTrainedTokenizer
     from trl import PreTrainedModelWrapper
 
@@ -26,19 +26,20 @@
         self,
         model_args: "ModelArguments",
         data_args: "DataArguments",
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments",
     ) -> None:
         self.can_generate = finetuning_args.stage == "sft"
-        self.model, self.tokenizer = load_model_and_tokenizer(
-            model_args, finetuning_args, is_trainable=False, add_valuehead=(not self.can_generate)
-        )
+        self.tokenizer = load_tokenizer(model_args)
         self.tokenizer.padding_side = "left" if self.can_generate else "right"
         self.template = get_template_and_fix_tokenizer(self.tokenizer, data_args.template)
+        self.model = load_model(
+            self.tokenizer, model_args, finetuning_args, is_trainable=False, add_valuehead=(not self.can_generate)
+        )  # must after fixing tokenizer to resize vocab
         self.generating_args = generating_args.to_dict()
 
     @staticmethod
     def _process_args(
         model: "PreTrainedModel",
         tokenizer: "PreTrainedTokenizer",
         template: "Template",
```

### Comparing `llmtuner-0.6.1/src/llmtuner/chat/vllm_engine.py` & `llmtuner-0.6.2/src/llmtuner/chat/vllm_engine.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/data/aligner.py` & `llmtuner-0.6.2/src/llmtuner/data/aligner.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/data/formatter.py` & `llmtuner-0.6.2/src/llmtuner/data/formatter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/data/loader.py` & `llmtuner-0.6.2/src/llmtuner/data/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 from typing import TYPE_CHECKING, Literal, Union
 
 from datasets import load_dataset, load_from_disk
 
 from ..extras.constants import FILEEXT2TYPE
 from ..extras.logging import get_logger
+from ..extras.misc import has_tokenized_data
 from .aligner import align_dataset
 from .parser import get_dataset_list
 from .preprocess import get_preprocess_and_print_func
 from .template import get_template_and_fix_tokenizer
 from .utils import checksum, merge_dataset
 
 
@@ -76,15 +77,17 @@
                 subset_name=data_name,
                 data_dir=data_dir,
                 data_files=data_files,
                 split=data_args.split,
                 cache_dir=cache_dir,
                 token=model_args.ms_hub_token,
                 use_streaming=(data_args.streaming and (dataset_attr.load_from != "file")),
-            ).to_hf_dataset()
+            )
+            if isinstance(dataset, MsDataset):
+                dataset = dataset.to_hf_dataset()
         except ImportError:
             raise ImportError("Please install modelscope via `pip install modelscope -U`")
     else:
         if "trust_remote_code" in inspect.signature(load_dataset).parameters:  # for datasets==2.16.0
             kwargs = {"trust_remote_code": True}
         else:
             kwargs = {}
@@ -113,35 +116,38 @@
 
 def get_dataset(
     tokenizer: "PreTrainedTokenizer",
     model_args: "ModelArguments",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     stage: Literal["pt", "sft", "rm", "ppo"],
-    # split: Optional[str] = "train", # TODO: add split
 ) -> Union["Dataset", "IterableDataset"]:
     template = get_template_and_fix_tokenizer(tokenizer, data_args.template)
     if data_args.train_on_prompt and template.efficient_eos:
         raise ValueError("Current template does not support `train_on_prompt`.")
 
-    # Load from cache
-    if data_args.cache_path is not None:
-        if os.path.exists(data_args.cache_path):
+    # Load tokenized dataset
+    if data_args.tokenized_path is not None:
+        if has_tokenized_data(data_args.tokenized_path):
             logger.warning("Loading dataset from disk will ignore other data arguments.")
-            dataset = load_from_disk(data_args.cache_path)
+            dataset = load_from_disk(data_args.tokenized_path)
+            logger.info("Loaded tokenized dataset from {}.".format(data_args.tokenized_path))
             if data_args.streaming:
                 dataset = dataset.to_iterable_dataset()
             return dataset
 
         if data_args.streaming:
             raise ValueError("Turn off `streaming` when saving dataset to disk.")
 
     with training_args.main_process_first(desc="load dataset"):
         all_datasets = []
         for dataset_attr in get_dataset_list(data_args):
+            if (stage == "rm" and dataset_attr.ranking is False) or (stage != "rm" and dataset_attr.ranking is True):
+                raise ValueError("The dataset is not applicable in the current training stage.")
+
             all_datasets.append(load_single_dataset(dataset_attr, model_args, data_args))
         dataset = merge_dataset(all_datasets, data_args, training_args)
 
     with training_args.main_process_first(desc="pre-process dataset"):
         preprocess_func, print_function = get_preprocess_and_print_func(
             tokenizer, template, data_args, training_args, stage
         )
@@ -152,18 +158,21 @@
                 num_proc=data_args.preprocessing_num_workers,
                 load_from_cache_file=(not data_args.overwrite_cache),
                 desc="Running tokenizer on dataset",
             )
 
         dataset = dataset.map(preprocess_func, batched=True, remove_columns=column_names, **kwargs)
 
-        if data_args.cache_path is not None and not os.path.exists(data_args.cache_path):
+        if data_args.tokenized_path is not None:
             if training_args.should_save:
-                dataset.save_to_disk(data_args.cache_path)
-                logger.info("Dataset cache saved at {}.".format(data_args.cache_path))
+                dataset.save_to_disk(data_args.tokenized_path)
+                logger.info("Tokenized dataset saved at {}.".format(data_args.tokenized_path))
+                logger.info("Please restart the training with `--tokenized_path {}`.".format(data_args.tokenized_path))
+
+            exit(0)
 
         if training_args.should_log:
             try:
                 print_function(next(iter(dataset)))
             except StopIteration:
                 raise RuntimeError("Cannot find valid samples, check `data/README.md` for the data format.")
```

### Comparing `llmtuner-0.6.1/src/llmtuner/data/parser.py` & `llmtuner-0.6.2/src/llmtuner/data/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,30 +49,43 @@
         return self.dataset_name
 
     def set_attr(self, key: str, obj: Dict[str, Any], default: Optional[Any] = None) -> None:
         setattr(self, key, obj.get(key, default))
 
 
 def get_dataset_list(data_args: "DataArguments") -> List["DatasetAttr"]:
-    dataset_names = [ds.strip() for ds in data_args.dataset.split(",")] if data_args.dataset is not None else []
-    try:
-        with open(os.path.join(data_args.dataset_dir, DATA_CONFIG), "r") as f:
-            dataset_info = json.load(f)
-    except Exception as err:
-        if data_args.dataset is not None:
-            raise ValueError(
-                "Cannot open {} due to {}.".format(os.path.join(data_args.dataset_dir, DATA_CONFIG), str(err))
-            )
+    if data_args.dataset is not None:
+        dataset_names = [ds.strip() for ds in data_args.dataset.split(",")]
+    else:
+        dataset_names = []
+
+    if data_args.dataset_dir == "ONLINE":
         dataset_info = None
+    else:
+        try:
+            with open(os.path.join(data_args.dataset_dir, DATA_CONFIG), "r") as f:
+                dataset_info = json.load(f)
+        except Exception as err:
+            if len(dataset_names) != 0:
+                raise ValueError(
+                    "Cannot open {} due to {}.".format(os.path.join(data_args.dataset_dir, DATA_CONFIG), str(err))
+                )
+            dataset_info = None
 
     if data_args.interleave_probs is not None:
         data_args.interleave_probs = [float(prob.strip()) for prob in data_args.interleave_probs.split(",")]
 
     dataset_list: List[DatasetAttr] = []
     for name in dataset_names:
+        if dataset_info is None:
+            load_from = "ms_hub" if use_modelscope() else "hf_hub"
+            dataset_attr = DatasetAttr(load_from, dataset_name=name)
+            dataset_list.append(dataset_attr)
+            continue
+
         if name not in dataset_info:
             raise ValueError("Undefined dataset {} in {}.".format(name, DATA_CONFIG))
 
         has_hf_url = "hf_hub_url" in dataset_info[name]
         has_ms_url = "ms_hub_url" in dataset_info[name]
 
         if has_hf_url or has_ms_url:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/data/preprocess.py` & `llmtuner-0.6.2/src/llmtuner/data/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,31 +19,33 @@
 
 
 def preprocess_pretrain_dataset(
     examples: Dict[str, List[Any]], tokenizer: "PreTrainedTokenizer", data_args: "DataArguments"
 ) -> Dict[str, List[List[int]]]:
     # build grouped texts with format `X1 X2 X3 ...` if packing is enabled
     text_examples = [messages[0]["content"] + tokenizer.eos_token for messages in examples["prompt"]]
+
     if not data_args.packing:
-        return tokenizer(text_examples, add_special_tokens=False, max_length=data_args.cutoff_len)
+        if data_args.template == "gemma":
+            text_examples = [tokenizer.bos_token + example for example in text_examples]
 
-    tokenized_examples = tokenizer(text_examples, add_special_tokens=False)
-    concatenated_examples = {k: list(chain(*tokenized_examples[k])) for k in tokenized_examples.keys()}
-    total_length = len(concatenated_examples[list(concatenated_examples.keys())[0]])
-    block_size = data_args.cutoff_len
-    # we drop the small remainder, and if the total_length < block_size, we exclude this batch
-    total_length = (total_length // block_size) * block_size
-    # split by chunks of cutoff_len
-    result = {
-        k: [t[i : i + block_size] for i in range(0, total_length, block_size)]
-        for k, t in concatenated_examples.items()
-    }
-    if data_args.template == "gemma":
-        for i in range(len(result["input_ids"])):
-            result["input_ids"][i][0] = tokenizer.bos_token_id
+        result = tokenizer(text_examples, add_special_tokens=False, max_length=data_args.cutoff_len)
+    else:
+        tokenized_examples = tokenizer(text_examples, add_special_tokens=False)
+        concatenated_examples = {k: list(chain(*tokenized_examples[k])) for k in tokenized_examples.keys()}
+        total_length = len(concatenated_examples[list(concatenated_examples.keys())[0]])
+        block_size = data_args.cutoff_len
+        total_length = (total_length // block_size) * block_size
+        result = {
+            k: [t[i : i + block_size] for i in range(0, total_length, block_size)]
+            for k, t in concatenated_examples.items()
+        }
+        if data_args.template == "gemma":
+            for i in range(len(result["input_ids"])):
+                result["input_ids"][i][0] = tokenizer.bos_token_id
 
     return result
 
 
 def preprocess_supervised_dataset(
     examples: Dict[str, List[Any]],
     tokenizer: "PreTrainedTokenizer",
```

### Comparing `llmtuner-0.6.1/src/llmtuner/data/template.py` & `llmtuner-0.6.2/src/llmtuner/data/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     ),
     format_assistant=StringFormatter(slots=["{{content}}\n", {"eos_token"}]),
 )
 
 
 _register_template(
     name="baichuan",
-    format_user=StringFormatter(slots=["<reserved_102>{{content}}<reserved_103>"]),
+    format_user=StringFormatter(slots=[{"token": "<reserved_102>"}, "{{content}}", {"token": "<reserved_103>"}]),
     efficient_eos=True,
 )
 
 
 _register_template(
     name="baichuan2",
     format_user=StringFormatter(slots=["<reserved_106>{{content}}<reserved_107>"]),
@@ -438,14 +438,26 @@
 _register_template(
     name="bluelm",
     format_user=StringFormatter(slots=[{"token": "[|Human|]:"}, "{{content}}", {"token": "[|AI|]:"}]),
 )
 
 
 _register_template(
+    name="breeze",
+    format_user=StringFormatter(slots=["[INST] {{content}} [/INST] "]),
+    format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
+    default_system=(
+        "You are a helpful AI assistant built by MediaTek Research. "
+        "The user you are helping speaks Traditional Chinese and comes from Taiwan."
+    ),
+    efficient_eos=True,
+)
+
+
+_register_template(
     name="chatglm2",
     format_user=StringFormatter(slots=["[Round {{idx}}]\n\n问：{{content}}\n\n答："]),
     format_system=StringFormatter(slots=[{"token": "[gMASK]"}, {"token": "sop"}, "{{content}}"]),
     format_separator=EmptyFormatter(slots=["\n\n"]),
     efficient_eos=True,
     force_system=True,
 )
```

### Comparing `llmtuner-0.6.1/src/llmtuner/data/utils.py` & `llmtuner-0.6.2/src/llmtuner/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if sha1 != file_sha1:
             logger.warning("Checksum failed: mismatched SHA-1 hash value at {}.".format(data_files[0]))
 
 
 def infer_max_len(source_len: int, target_len: int, max_len: int, reserved_label_len: int) -> Tuple[int, int]:
     max_target_len = int(max_len * (target_len / (source_len + target_len)))
     max_target_len = max(max_target_len, reserved_label_len)
-    max_source_len = max_len - max_target_len
+    max_source_len = max_len - min(max_target_len, target_len)
     return max_source_len, max_target_len
 
 
 def merge_dataset(
     all_datasets: List[Union["Dataset", "IterableDataset"]],
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
```

### Comparing `llmtuner-0.6.1/src/llmtuner/eval/evaluator.py` & `llmtuner-0.6.2/src/llmtuner/eval/evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,24 +10,25 @@
 from datasets import load_dataset
 from tqdm import tqdm, trange
 from transformers.utils import cached_file
 
 from ..data import get_template_and_fix_tokenizer
 from ..extras.constants import CHOICES, SUBJECTS
 from ..hparams import get_eval_args
-from ..model import load_model_and_tokenizer
+from ..model import load_model, load_tokenizer
 from .template import get_eval_template
 
 
 class Evaluator:
     def __init__(self, args: Optional[Dict[str, Any]] = None) -> None:
         self.model_args, self.data_args, self.eval_args, finetuning_args = get_eval_args(args)
-        self.model, self.tokenizer = load_model_and_tokenizer(self.model_args, finetuning_args)
+        self.tokenizer = load_tokenizer(self.model_args)
         self.tokenizer.padding_side = "right"  # avoid overflow issue in batched inference for llama2
         self.template = get_template_and_fix_tokenizer(self.tokenizer, self.data_args.template)
+        self.model = load_model(self.tokenizer, self.model_args, finetuning_args)
         self.eval_template = get_eval_template(self.eval_args.lang)
         self.choice_inputs = [
             self.tokenizer.encode(self.eval_template.prefix + ch, add_special_tokens=False)[-1] for ch in CHOICES
         ]
 
     @torch.inference_mode()
     def batch_inference(self, batch_input: Dict[str, torch.Tensor]) -> List[str]:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/eval/template.py` & `llmtuner-0.6.2/src/llmtuner/eval/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/callbacks.py` & `llmtuner-0.6.2/src/llmtuner/extras/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         logs = dict(
             current_steps=self.cur_steps,
             total_steps=self.max_steps,
             loss=state.log_history[-1].get("loss", None),
             eval_loss=state.log_history[-1].get("eval_loss", None),
             predict_loss=state.log_history[-1].get("predict_loss", None),
             reward=state.log_history[-1].get("reward", None),
+            accuracy=state.log_history[-1].get("rewards/accuracies", None),
             learning_rate=state.log_history[-1].get("learning_rate", None),
             epoch=state.log_history[-1].get("epoch", None),
             percentage=round(self.cur_steps / self.max_steps * 100, 2) if self.max_steps != 0 else 100,
             elapsed_time=self.elapsed_time,
             remaining_time=self.remaining_time,
         )
         if self.runner is not None:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/constants.py` & `llmtuner-0.6.2/src/llmtuner/extras/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,20 @@
 SUPPORTED_MODELS = OrderedDict()
 
 TRAINING_STAGES = {
     "Supervised Fine-Tuning": "sft",
     "Reward Modeling": "rm",
     "PPO": "ppo",
     "DPO": "dpo",
+    "ORPO": "orpo",
     "Pre-Training": "pt",
 }
 
+STAGES_USE_PAIR_DATA = ["rm", "dpo", "orpo"]
+
 V_HEAD_WEIGHTS_NAME = "value_head.bin"
 
 V_HEAD_SAFE_WEIGHTS_NAME = "value_head.safetensors"
 
 
 class DownloadSource(str, Enum):
     DEFAULT = "hf"
@@ -165,14 +168,27 @@
     },
     template="bluelm",
 )
 
 
 register_model_group(
     models={
+        "Breeze-7B": {
+            DownloadSource.DEFAULT: "MediaTek-Research/Breeze-7B-Base-v1_0",
+        },
+        "Breeze-7B-Chat": {
+            DownloadSource.DEFAULT: "MediaTek-Research/Breeze-7B-Instruct-v1_0",
+        },
+    },
+    template="breeze",
+)
+
+
+register_model_group(
+    models={
         "ChatGLM2-6B-Chat": {
             DownloadSource.DEFAULT: "THUDM/chatglm2-6b",
             DownloadSource.MODELSCOPE: "ZhipuAI/chatglm2-6b",
         }
     },
     module="query_key_value",
     template="chatglm2",
@@ -456,22 +472,26 @@
     },
     template="llama2",
 )
 
 
 register_model_group(
     models={
-        "Mistral-7B": {
+        "Mistral-7B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-v0.1",
         },
-        "Mistral-7B-Chat": {
+        "Mistral-7B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-Instruct-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-Instruct-v0.1",
         },
+        "Mistral-7B-v0.2": {
+            DownloadSource.DEFAULT: "alpindale/Mistral-7B-v0.2-hf",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-v0.2-hf",
+        },
         "Mistral-7B-v0.2-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-Instruct-v0.2",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-Instruct-v0.2",
         },
     },
     template="mistral",
 )
@@ -652,18 +672,26 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-7B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-7B",
         },
         "Qwen1.5-14B": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-14B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-14B",
         },
+        "Qwen1.5-32B": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-32B",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-32B",
+        },
         "Qwen1.5-72B": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B",
         },
+        "Qwen1.5-MoE-A2.7B": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B",
+        },
         "Qwen1.5-0.5B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat",
         },
         "Qwen1.5-1.8B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-1.8B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-1.8B-Chat",
@@ -676,18 +704,26 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-7B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-7B-Chat",
         },
         "Qwen1.5-14B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-14B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-14B-Chat",
         },
+        "Qwen1.5-32B-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-32B-Chat",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-32B-Chat",
+        },
         "Qwen1.5-72B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat",
         },
+        "Qwen1.5-MoE-A2.7B-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat",
+        },
         "Qwen1.5-0.5B-int8-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8",
         },
         "Qwen1.5-0.5B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat-AWQ",
@@ -720,22 +756,30 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-14B-Chat-GPTQ-Int8",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-14B-Chat-GPTQ-Int8",
         },
         "Qwen1.5-14B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-14B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-14B-Chat-AWQ",
         },
+        "Qwen1.5-32B-int4-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-32B-Chat-AWQ",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-32B-Chat-AWQ",
+        },
         "Qwen1.5-72B-int8-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat-GPTQ-Int8",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat-GPTQ-Int8",
         },
         "Qwen1.5-72B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat-AWQ",
         },
+        "Qwen1.5-MoE-A2.7B-int4-Chat": {
+            DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
+            DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
+        },
     },
     template="qwen",
 )
 
 
 register_model_group(
     models={
```

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/logging.py` & `llmtuner-0.6.2/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/misc.py` & `llmtuner-0.6.2/src/llmtuner/extras/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         logger.warning("Version checking has been disabled, may lead to unexpected behaviors.")
     else:
         require_version("transformers>=4.37.2", "To fix: pip install transformers>=4.37.2")
         require_version("datasets>=2.14.3", "To fix: pip install datasets>=2.14.3")
         require_version("accelerate>=0.27.2", "To fix: pip install accelerate>=0.27.2")
         require_version("peft>=0.10.0", "To fix: pip install peft>=0.10.0")
         require_version("trl>=0.8.1", "To fix: pip install trl>=0.8.1")
+        require_version("gradio>=4.0.0,<=4.21.0", "To fix: pip install gradio==4.21.0")
 
 
 def count_parameters(model: torch.nn.Module) -> Tuple[int, int]:
     r"""
     Returns the number of trainable parameters and number of all parameters in the model.
     """
     trainable_params, all_param = 0, 0
@@ -188,34 +189,39 @@
         return torch.bfloat16
     elif _is_fp16_available:
         return torch.float16
     else:
         return torch.float32
 
 
+def has_tokenized_data(path: os.PathLike) -> bool:
+    r"""
+    Checks if the path has a tokenized dataset.
+    """
+    return os.path.isdir(path) and len(os.listdir(path)) > 0
+
+
 def torch_gc() -> None:
     r"""
     Collects GPU memory.
     """
     gc.collect()
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
         torch.cuda.ipc_collect()
 
 
-def try_download_model_from_ms(model_args: "ModelArguments") -> None:
+def try_download_model_from_ms(model_args: "ModelArguments") -> str:
     if not use_modelscope() or os.path.exists(model_args.model_name_or_path):
-        return
+        return model_args.model_name_or_path
 
     try:
         from modelscope import snapshot_download
 
         revision = "master" if model_args.model_revision == "main" else model_args.model_revision
-        model_args.model_name_or_path = snapshot_download(
-            model_args.model_name_or_path, revision=revision, cache_dir=model_args.cache_dir
-        )
+        return snapshot_download(model_args.model_name_or_path, revision=revision, cache_dir=model_args.cache_dir)
     except ImportError:
         raise ImportError("Please install modelscope via `pip install modelscope -U`")
 
 
 def use_modelscope() -> bool:
     return bool(int(os.environ.get("USE_MODELSCOPE_HUB", "0")))
```

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/packages.py` & `llmtuner-0.6.2/src/llmtuner/extras/packages.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/patches/llama_patch.py` & `llmtuner-0.6.2/src/llmtuner/extras/patches/llama_patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,10 +189,10 @@
     if not output_attentions:
         attn_weights = None
 
     return attn_output, attn_weights, past_key_value
 
 
 def apply_llama_patch() -> None:
-    require_version("transformers==4.39.1", "To fix: pip install transformers==4.39.1")
+    require_version("transformers==4.39.3", "To fix: pip install transformers==4.39.3")
     LlamaAttention.forward = llama_torch_attn_forward
     LlamaFlashAttention2.forward = llama_flash_attn_forward
```

### Comparing `llmtuner-0.6.1/src/llmtuner/extras/ploting.py` & `llmtuner-0.6.2/src/llmtuner/extras/ploting.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,10 +48,10 @@
         plt.figure()
         plt.plot(steps, metrics, color="#1f77b4", alpha=0.4, label="original")
         plt.plot(steps, smooth(metrics), color="#1f77b4", label="smoothed")
         plt.title("training {} of {}".format(key, save_dictionary))
         plt.xlabel("step")
         plt.ylabel(key)
         plt.legend()
-        figure_path = os.path.join(save_dictionary, "training_{}.png".format(key.replace(os.path.sep, "_")))
+        figure_path = os.path.join(save_dictionary, "training_{}.png".format(key.replace("/", "_")))
         plt.savefig(figure_path, format="png", dpi=100)
         print("Figure saved at:", figure_path)
```

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/data_args.py` & `llmtuner-0.6.2/src/llmtuner/hparams/data_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     )
     packing: Optional[bool] = field(
         default=None,
         metadata={
             "help": "Whether or not to pack the sequences in training. Will automatically enable in pre-training."
         },
     )
-    cache_path: Optional[str] = field(
+    tokenized_path: Optional[str] = field(
         default=None,
-        metadata={"help": "Path to save or load the pre-processed datasets."},
+        metadata={"help": "Path to save or load the tokenized datasets."},
     )
 
     def __post_init__(self):
         if self.reserved_label_len >= self.cutoff_len:
             raise ValueError("`reserved_label_len` must be smaller than `cutoff_len`.")
 
         if self.streaming and self.val_size > 1e-6 and self.val_size < 1:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/evaluation_args.py` & `llmtuner-0.6.2/src/llmtuner/hparams/evaluation_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.6.2/src/llmtuner/hparams/finetuning_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,18 @@
         default=0.0,
         metadata={"help": "The robust DPO label smoothing parameter in cDPO that should be between 0 and 0.5."},
     )
     dpo_ftx: float = field(
         default=0.0,
         metadata={"help": "The supervised fine-tuning loss coefficient in DPO training."},
     )
+    orpo_beta: float = field(
+        default=0.1,
+        metadata={"help": "The beta (lambda) parameter in ORPO loss representing the weight of the SFT loss."},
+    )
     ppo_buffer_size: int = field(
         default=1,
         metadata={"help": "The number of mini-batches to make experience buffer in a PPO optimization step."},
     )
     ppo_epochs: int = field(
         default=4,
         metadata={"help": "The number of epochs to perform in a PPO optimization step."},
@@ -205,15 +209,15 @@
     Arguments pertaining to which techniques we are going to fine-tuning with.
     """
 
     pure_bf16: bool = field(
         default=False,
         metadata={"help": "Whether or not to train model in purely bf16 precision (without AMP)."},
     )
-    stage: Literal["pt", "sft", "rm", "ppo", "dpo"] = field(
+    stage: Literal["pt", "sft", "rm", "ppo", "dpo", "orpo"] = field(
         default="sft",
         metadata={"help": "Which stage will be performed in training."},
     )
     finetuning_type: Literal["lora", "freeze", "full"] = field(
         default="lora",
         metadata={"help": "Which fine-tuning method to use."},
     )
```

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.6.2/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/model_args.py` & `llmtuner-0.6.2/src/llmtuner/hparams/model_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,18 @@
         default="nf4",
         metadata={"help": "Quantization data type to use in int4 training."},
     )
     double_quantization: bool = field(
         default=True,
         metadata={"help": "Whether or not to use double quantization in int4 training."},
     )
+    quantization_device_map: Optional[Literal["auto"]] = field(
+        default=None,
+        metadata={"help": "Device map used for loading the 4-bit quantized model, needs bitsandbytes>=0.43.0."},
+    )
     rope_scaling: Optional[Literal["linear", "dynamic"]] = field(
         default=None,
         metadata={"help": "Which scaling strategy should be adopted for the RoPE embeddings."},
     )
     flash_attn: bool = field(
         default=False,
         metadata={"help": "Enable FlashAttention-2 for faster training."},
@@ -65,14 +69,18 @@
         default=False,
         metadata={"help": "Enable shift short attention (S^2-Attn) proposed by LongLoRA."},
     )
     use_unsloth: bool = field(
         default=False,
         metadata={"help": "Whether or not to use unsloth's optimization for the LoRA training."},
     )
+    moe_aux_loss_coef: Optional[float] = field(
+        default=None,
+        metadata={"help": "Coefficient of the auxiliary router loss in mixture-of-experts model."},
+    )
     disable_gradient_checkpointing: bool = field(
         default=False,
         metadata={"help": "Whether or not to disable gradient checkpointing."},
     )
     upcast_layernorm: bool = field(
         default=False,
         metadata={"help": "Whether or not to upcast the layernorm weights in fp32."},
```

### Comparing `llmtuner-0.6.1/src/llmtuner/hparams/parser.py` & `llmtuner-0.6.2/src/llmtuner/hparams/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         raise ValueError("PPO training is incompatible with S^2-Attn.")
 
     if finetuning_args.stage == "ppo" and finetuning_args.reward_model_type == "lora" and model_args.use_unsloth:
         raise ValueError("Unsloth does not support lora reward model.")
 
     if (
         finetuning_args.stage == "ppo"
-        and training_args.report_to is not None
+        and training_args.report_to
         and training_args.report_to[0] not in ["wandb", "tensorboard"]
     ):
         raise ValueError("PPO only accepts wandb or tensorboard logger.")
 
     if training_args.max_steps == -1 and data_args.streaming:
         raise ValueError("Please specify `max_steps` in streaming mode.")
```

### Comparing `llmtuner-0.6.1/src/llmtuner/model/adapter.py` & `llmtuner-0.6.2/src/llmtuner/model/adapter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/model/loader.py` & `llmtuner-0.6.2/src/llmtuner/model/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Any, Dict, Tuple
+from typing import TYPE_CHECKING, Any, Dict
 
 from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 from trl import AutoModelForCausalLMWithValueHead
 
 from ..extras.logging import get_logger
 from ..extras.misc import count_parameters, get_current_device, try_download_model_from_ms
 from .adapter import init_adapter
@@ -16,31 +16,30 @@
     from ..hparams import FinetuningArguments, ModelArguments
 
 
 logger = get_logger(__name__)
 
 
 def _get_init_kwargs(model_args: "ModelArguments") -> Dict[str, Any]:
+    model_args.model_name_or_path = try_download_model_from_ms(model_args)
     return {
         "trust_remote_code": True,
         "cache_dir": model_args.cache_dir,
         "revision": model_args.model_revision,
         "token": model_args.hf_hub_token,
     }
 
 
 def load_tokenizer(model_args: "ModelArguments") -> "PreTrainedTokenizer":
     r"""
     Loads pretrained tokenizer. Must before load_model.
 
     Note: including inplace operation of model_args.
     """
-    try_download_model_from_ms(model_args)
     init_kwargs = _get_init_kwargs(model_args)
-
     tokenizer = AutoTokenizer.from_pretrained(
         model_args.model_name_or_path,
         use_fast=model_args.use_fast_tokenizer,
         split_special_tokens=model_args.split_special_tokens,
         padding_side="right",
         **init_kwargs,
     )
@@ -106,17 +105,14 @@
         if vhead_params is not None:
             model.load_state_dict(vhead_params, strict=False)
             logger.info("Loaded valuehead from checkpoint: {}".format(vhead_path))
 
     if not is_trainable:
         model.requires_grad_(False)
         model.eval()
-        for param in model.parameters():
-            if param.device.type == "cuda":
-                param.data = param.data.to(model_args.compute_dtype)
     else:
         model.train()
 
     trainable_params, all_param = count_parameters(model)
     if is_trainable:
         param_stats = "trainable params: {:d} || all params: {:d} || trainable%: {:.4f}".format(
             trainable_params, all_param, 100 * trainable_params / all_param
@@ -130,21 +126,7 @@
             print(
                 "name: {}, dtype: {}, device: {}, trainable: {}".format(
                     name, param.dtype, param.device, param.requires_grad
                 )
             )
 
     return model
-
-
-def load_model_and_tokenizer(
-    model_args: "ModelArguments",
-    finetuning_args: "FinetuningArguments",
-    is_trainable: bool = False,
-    add_valuehead: bool = False,
-) -> Tuple["PreTrainedModel", "PreTrainedTokenizer"]:
-    r"""
-    Loads pretrained model and tokenizer.
-    """
-    tokenizer = load_tokenizer(model_args)
-    model = load_model(tokenizer, model_args, finetuning_args, is_trainable, add_valuehead)
-    return model, tokenizer
```

### Comparing `llmtuner-0.6.1/src/llmtuner/model/patcher.py` & `llmtuner-0.6.2/src/llmtuner/model/patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,70 +13,28 @@
 from transformers.utils.versions import require_version
 
 from ..extras.constants import FILEEXT2TYPE, LAYERNORM_NAMES
 from ..extras.logging import get_logger
 from ..extras.misc import get_current_device, infer_optim_dtype
 from ..extras.packages import is_flash_attn2_available
 from ..extras.patches.llama_patch import apply_llama_patch
-from ..extras.patches.mixtral_patch import patch_mixtral_replace_moe_impl
-from .utils import QuantizationMethod
+from .utils import QuantizationMethod, add_z3_leaf_module
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedTokenizer
     from trl import AutoModelForCausalLMWithValueHead
 
     from ..hparams import ModelArguments
 
 
 logger = get_logger(__name__)
 SUPPORTED_CLASS_FOR_S2ATTN = ["llama"]
 
 
-def _noisy_mean_initialization(embed_weight: torch.Tensor, num_new_tokens: int):
-    embedding_dim = embed_weight.size(1)
-    avg_weight = embed_weight[:-num_new_tokens].mean(dim=0, keepdim=True)
-    noise_weight = torch.empty_like(embed_weight[-num_new_tokens:])
-    noise_weight.normal_(mean=0, std=(1.0 / math.sqrt(embedding_dim)))
-    embed_weight[-num_new_tokens:] = avg_weight + noise_weight
-
-
-def _resize_embedding_layer(model: "PreTrainedModel", tokenizer: "PreTrainedTokenizer") -> None:
-    r"""
-    Resize token embeddings.
-    """
-    if is_deepspeed_zero3_enabled():
-        import deepspeed  # type: ignore
-
-        params = [model.get_input_embeddings().weight]
-        if model.get_output_embeddings() is not None and not model.config.tie_word_embeddings:
-            params.append(model.get_output_embeddings().weight)
-
-        context_maybe_zero3 = deepspeed.zero.GatheredParameters(params, modifier_rank=0)
-    else:
-        context_maybe_zero3 = nullcontext()
-
-    with context_maybe_zero3:
-        current_embedding_size = model.get_input_embeddings().weight.size(0)
-
-    if len(tokenizer) > current_embedding_size:
-        if not isinstance(model.get_output_embeddings(), torch.nn.Linear):
-            logger.warning("Current model does not support resizing token embeddings.")
-            return
-
-        model.resize_token_embeddings(len(tokenizer), pad_to_multiple_of=64)
-        with context_maybe_zero3:
-            new_embedding_size = model.get_input_embeddings().weight.size(0)
-            num_new_tokens = new_embedding_size - current_embedding_size
-            _noisy_mean_initialization(model.get_input_embeddings().weight.data, num_new_tokens)
-            _noisy_mean_initialization(model.get_output_embeddings().weight.data, num_new_tokens)
-
-        logger.info("Resized token embeddings from {} to {}.".format(current_embedding_size, new_embedding_size))
-
-
 def _get_quantization_dataset(tokenizer: "PreTrainedTokenizer", model_args: "ModelArguments") -> List[str]:
     r"""
     Inspired by: https://github.com/huggingface/optimum/blob/v1.16.0/optimum/gptq/data.py#L133
     TODO: remove tokenizer.decode() https://github.com/huggingface/optimum/pull/1600
     """
     if os.path.isfile(model_args.export_quantization_dataset):
         data_path = FILEEXT2TYPE.get(model_args.export_quantization_dataset.split(".")[-1], None)
@@ -176,16 +134,20 @@
             raise ValueError("DeepSpeed ZeRO-3 is incompatible with quantized models.")
 
         init_kwargs["device_map"] = {"": get_current_device()}
         quantization_config: Dict[str, Any] = getattr(config, "quantization_config", None)
         quant_method = quantization_config.get("quant_method", "")
 
         if quant_method == QuantizationMethod.GPTQ:
+            require_version("auto_gptq>=0.5.0", "To fix: pip install auto_gptq>=0.5.0")
             quantization_config["use_exllama"] = False  # disable exllama
 
+        if quant_method == QuantizationMethod.AWQ:
+            require_version("autoawq", "To fix: pip install autoawq")
+
         if quant_method == QuantizationMethod.AQLM:
             require_version("transformers>=4.39.0", "To fix: pip install transformers>=4.39.0")
             require_version("aqlm>=1.1.0", "To fix: pip install aqlm[gpu]>=1.1.0")
             quantization_config["bits"] = 2
 
         quant_bits = quantization_config.get("bits", "?")
         logger.info("Loading {}-bit {}-quantized model.".format(quant_bits, quant_method.upper()))
@@ -204,37 +166,88 @@
             dataset=_get_quantization_dataset(tokenizer, model_args),
         )
         init_kwargs["device_map"] = "auto"
         init_kwargs["max_memory"] = get_max_memory()
         logger.info("Quantizing model to {} bit.".format(model_args.export_quantization_bit))
 
     elif model_args.quantization_bit is not None:  # bnb
-        if is_deepspeed_zero3_enabled():
-            require_version("transformers>=4.39.0", "To fix: pip install transformers>=4.39.0")
-            require_version("accelerate>=0.28.0", "To fix: pip install accelerate>=0.28.0")
-            require_version("bitsandbytes>=0.43.0", "To fix: pip install bitsandbytes>=0.43.0")
-
         if model_args.quantization_bit == 8:
             require_version("bitsandbytes>=0.37.0", "To fix: pip install bitsandbytes>=0.37.0")
             init_kwargs["quantization_config"] = BitsAndBytesConfig(load_in_8bit=True)
 
         elif model_args.quantization_bit == 4:
             require_version("bitsandbytes>=0.39.0", "To fix: pip install bitsandbytes>=0.39.0")
             init_kwargs["quantization_config"] = BitsAndBytesConfig(
                 load_in_4bit=True,
                 bnb_4bit_compute_dtype=model_args.compute_dtype,
                 bnb_4bit_use_double_quant=model_args.double_quantization,
                 bnb_4bit_quant_type=model_args.quantization_type,
                 bnb_4bit_quant_storage=model_args.compute_dtype,  # crucial for fsdp qlora
             )
 
-        init_kwargs["device_map"] = {"": get_current_device()}
+        if is_deepspeed_zero3_enabled() or model_args.quantization_device_map == "auto":
+            if model_args.quantization_bit != 4:
+                raise ValueError("Only 4-bit quantized model can use auto device map.")
+
+            require_version("transformers>=4.39.0", "To fix: pip install transformers>=4.39.0")
+            require_version("accelerate>=0.28.0", "To fix: pip install accelerate>=0.28.0")
+            require_version("bitsandbytes>=0.43.0", "To fix: pip install bitsandbytes>=0.43.0")
+        else:
+            init_kwargs["device_map"] = {"": get_current_device()}
+
         logger.info("Quantizing model to {} bit.".format(model_args.quantization_bit))
 
 
+def _noisy_mean_initialization(embed_weight: torch.Tensor, num_new_tokens: int):
+    embedding_dim = embed_weight.size(1)
+    avg_weight = embed_weight[:-num_new_tokens].mean(dim=0, keepdim=True)
+    noise_weight = torch.empty_like(embed_weight[-num_new_tokens:])
+    noise_weight.normal_(mean=0, std=(1.0 / math.sqrt(embedding_dim)))
+    embed_weight[-num_new_tokens:] = avg_weight + noise_weight
+
+
+def _resize_embedding_layer(model: "PreTrainedModel", tokenizer: "PreTrainedTokenizer") -> None:
+    r"""
+    Resize token embeddings.
+    """
+    if is_deepspeed_zero3_enabled():
+        import deepspeed  # type: ignore
+
+        params = [model.get_input_embeddings().weight]
+        if model.get_output_embeddings() is not None and not model.config.tie_word_embeddings:
+            params.append(model.get_output_embeddings().weight)
+
+        context_maybe_zero3 = deepspeed.zero.GatheredParameters(params, modifier_rank=0)
+    else:
+        context_maybe_zero3 = nullcontext()
+
+    with context_maybe_zero3:
+        current_embedding_size = model.get_input_embeddings().weight.size(0)
+
+    if len(tokenizer) > current_embedding_size:
+        if not isinstance(model.get_output_embeddings(), torch.nn.Linear):
+            logger.warning("Current model does not support resizing token embeddings.")
+            return
+
+        model.resize_token_embeddings(len(tokenizer), pad_to_multiple_of=64)
+        with context_maybe_zero3:
+            new_embedding_size = model.get_input_embeddings().weight.size(0)
+            num_new_tokens = new_embedding_size - current_embedding_size
+            _noisy_mean_initialization(model.get_input_embeddings().weight.data, num_new_tokens)
+            _noisy_mean_initialization(model.get_output_embeddings().weight.data, num_new_tokens)
+
+        logger.info("Resized token embeddings from {} to {}.".format(current_embedding_size, new_embedding_size))
+
+
+def _fp32_forward_post_hook(
+    module: "torch.nn.Module", args: Tuple["torch.Tensor"], output: "torch.Tensor"
+) -> "torch.Tensor":
+    return output.to(torch.float32)
+
+
 def _prepare_model_for_training(
     model: "PreTrainedModel", model_args: "ModelArguments", output_layer_name: str = "lm_head"
 ) -> None:
     r"""
     Includes:
         (1) cast the layernorm in fp32
         (2) make output embedding layer require grads
@@ -255,22 +268,18 @@
             # According to: https://github.com/huggingface/transformers/issues/28339
             model.gradient_checkpointing_enable(gradient_checkpointing_kwargs={"use_reentrant": True})
             model.enable_input_require_grads()
             setattr(model.config, "use_cache", False)  # turn off when gradient checkpointing is enabled
             logger.info("Gradient checkpointing enabled.")
 
     if hasattr(model, output_layer_name) and model_args.upcast_lmhead_output:
-
-        def fp32_forward_post_hook(module: torch.nn.Module, args: Tuple[torch.Tensor], output: torch.Tensor):
-            return output.to(torch.float32)
-
         logger.info("Upcasting lm_head outputs in float32.")
         output_layer = getattr(model, output_layer_name)
         if isinstance(output_layer, torch.nn.Linear) and output_layer.weight.dtype != torch.float32:
-            output_layer.register_forward_hook(fp32_forward_post_hook)
+            output_layer.register_forward_hook(_fp32_forward_post_hook)
 
 
 def patch_tokenizer(tokenizer: "PreTrainedTokenizer") -> None:
     if "PreTrainedTokenizerBase" not in str(tokenizer._pad.__func__):
         tokenizer._pad = MethodType(PreTrainedTokenizerBase._pad, tokenizer)
 
 
@@ -280,64 +289,84 @@
     model_args: "ModelArguments",
     init_kwargs: Dict[str, Any],
     is_trainable: bool,
 ) -> None:
     if model_args.compute_dtype is None:  # priority: bf16 > fp16 > fp32
         model_args.compute_dtype = infer_optim_dtype(model_dtype=getattr(config, "torch_dtype", None))
 
-    if getattr(config, "model_type", None) == "qwen":
-        setattr(config, "use_flash_attn", model_args.flash_attn)
-        for dtype_name, dtype in [("fp16", torch.float16), ("bf16", torch.bfloat16), ("fp32", torch.float32)]:
-            setattr(config, dtype_name, model_args.compute_dtype == dtype)
-
     _configure_attn_implementation(config, model_args, init_kwargs)
     _configure_rope(config, model_args, is_trainable)
     _configure_longlora(config, model_args, is_trainable)
     _configure_quantization(config, tokenizer, model_args, init_kwargs)
 
     if model_args.use_cache and not is_trainable:
         setattr(config, "use_cache", True)
         logger.info("Using KV cache for faster generation.")
 
+    if model_args.moe_aux_loss_coef is not None:
+        if getattr(config, "model_type", None) in ["mixtral", "qwen2_moe"]:
+            setattr(config, "router_aux_loss_coef", model_args.moe_aux_loss_coef)
+        elif getattr(config, "model_type", None) == "deepseek":
+            setattr(config, "aux_loss_alpha", model_args.moe_aux_loss_coef)
+
+    if getattr(config, "model_type", None) == "qwen":
+        setattr(config, "use_flash_attn", model_args.flash_attn)
+        for dtype_name, dtype in [("fp16", torch.float16), ("bf16", torch.bfloat16), ("fp32", torch.float32)]:
+            setattr(config, dtype_name, model_args.compute_dtype == dtype)
+
+    if getattr(config, "model_type", None) == "qwen2" and is_trainable and model_args.flash_attn:
+        setattr(config, "use_cache", False)  # qwen2 does not support use_cache when using flashattn
+
+    if getattr(config, "model_type", None) == "qwen2_moe" and is_trainable:
+        setattr(config, "output_router_logits", True)
+
     init_kwargs["torch_dtype"] = model_args.compute_dtype
     if not is_deepspeed_zero3_enabled():
         init_kwargs["low_cpu_mem_usage"] = model_args.low_cpu_mem_usage
         if init_kwargs["low_cpu_mem_usage"]:
-            if "device_map" not in init_kwargs:  # quant models cannot use auto device map
+            if "device_map" not in init_kwargs:
                 init_kwargs["device_map"] = model_args.device_map or {"": get_current_device()}
 
             if init_kwargs["device_map"] == "auto":
                 init_kwargs["offload_folder"] = model_args.offload_folder
 
 
 def patch_model(
     model: "PreTrainedModel", tokenizer: "PreTrainedTokenizer", model_args: "ModelArguments", is_trainable: bool
 ) -> None:
+    gen_config = model.generation_config  # check and fix generation config
+    if not gen_config.do_sample and (
+        (gen_config.temperature is not None and gen_config.temperature != 1.0)
+        or (gen_config.top_p is not None and gen_config.top_p != 1.0)
+        or (gen_config.typical_p is not None and gen_config.typical_p != 1.0)
+    ):
+        gen_config.do_sample = True
+
     if "GenerationMixin" not in str(model.generate.__func__):
         model.generate = MethodType(PreTrainedModel.generate, model)
 
-    if getattr(model.config, "model_type", None) == "chatglm":
+    if is_trainable and getattr(model.config, "model_type", None) == "chatglm":
         setattr(model, "lm_head", model.transformer.output_layer)
         setattr(model, "_keys_to_ignore_on_save", ["lm_head.weight"])
 
     if model_args.resize_vocab:
         _resize_embedding_layer(model, tokenizer)
 
     if is_trainable:
         _prepare_model_for_training(model, model_args)
 
-    if getattr(model.config, "model_type", None) == "mixtral" and is_deepspeed_zero3_enabled():
-        require_version("deepspeed>=0.13.0", "To fix: pip install deepspeed>=0.13.0")
-        from deepspeed.utils import set_z3_leaf_modules  # type: ignore
+    if getattr(model.config, "model_type", None) == "mixtral":
         from transformers.models.mixtral.modeling_mixtral import MixtralSparseMoeBlock
 
-        set_z3_leaf_modules(model, [MixtralSparseMoeBlock])
+        add_z3_leaf_module(model, MixtralSparseMoeBlock)
+
+    if getattr(model.config, "model_type", None) == "qwen2moe":
+        from transformers.models.qwen2_moe.modeling_qwen2_moe import Qwen2MoeSparseMoeBlock
 
-        if is_trainable:
-            patch_mixtral_replace_moe_impl()
+        add_z3_leaf_module(model, Qwen2MoeSparseMoeBlock)
 
     try:
         model.add_model_tags(["llama-factory"])
     except Exception:
         logger.warning("Cannot properly tag the model.")
```

### Comparing `llmtuner-0.6.1/src/llmtuner/model/utils.py` & `llmtuner-0.6.2/src/llmtuner/model/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from enum import Enum, unique
 from typing import TYPE_CHECKING, Dict, List
 
 import torch
 from transformers import PreTrainedModel
+from transformers.integrations import is_deepspeed_zero3_enabled
 from transformers.utils import cached_file
+from transformers.utils.versions import require_version
 
 from ..extras.constants import V_HEAD_SAFE_WEIGHTS_NAME, V_HEAD_WEIGHTS_NAME
 from ..extras.logging import get_logger
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedTokenizer
@@ -24,19 +26,31 @@
     Borrowed from `transformers.utils.quantization_config.QuantizationMethod`.
     """
 
     BITS_AND_BYTES = "bitsandbytes"
     GPTQ = "gptq"
     AWQ = "awq"
     AQLM = "aqlm"
+    QUANTO = "quanto"
+
+
+def add_z3_leaf_module(model: "PreTrainedModel", module: "torch.nn.Module") -> None:
+    r"""
+    Sets module as a leaf module to skip partitioning in deepspeed zero3.
+    """
+    if is_deepspeed_zero3_enabled():
+        require_version("deepspeed>=0.13.0", "To fix: pip install deepspeed>=0.13.0")
+        from deepspeed.utils import set_z3_leaf_modules  # type: ignore
+
+        set_z3_leaf_modules(model, [module])
 
 
 def find_all_linear_modules(model: "PreTrainedModel") -> List[str]:
     r"""
-    Finds all available modules to apply lora.
+    Finds all available modules to apply lora or galore.
     """
     quantization_method = getattr(model, "quantization_method", None)
     if quantization_method is None:
         linear_cls = torch.nn.Linear
     elif quantization_method == QuantizationMethod.BITS_AND_BYTES:
         import bitsandbytes as bnb
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/dpo/collator.py` & `llmtuner-0.6.2/src/llmtuner/data/collator.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from typing import Any, Dict, List, Sequence, Tuple
 
 import torch
 from transformers import DataCollatorForSeq2Seq
 
 
 @dataclass
-class DPODataCollatorWithPadding(DataCollatorForSeq2Seq):
+class PairwiseDataCollatorWithPadding(DataCollatorForSeq2Seq):
     r"""
     Data collator for pairwise data.
     """
 
     def _pad_labels(self, batch: torch.Tensor, positions: List[Tuple[int, int]]) -> torch.Tensor:
+        r"""
+        Masks out the input ids except for the responses.
+        """
         padded_labels = []
         for feature, (prompt_len, answer_len) in zip(batch, positions):
             if self.tokenizer.padding_side == "left":
                 start, end = feature.size(0) - answer_len, feature.size(0)
             else:
                 start, end = prompt_len, prompt_len + answer_len
             padded_tensor = self.label_pad_token_id * torch.ones_like(feature)
@@ -39,16 +42,10 @@
                     {
                         "input_ids": feature["prompt_ids"] + feature[key],
                         "attention_mask": [1] * (prompt_len + answer_len),
                     }
                 )
                 label_positions.append((prompt_len, answer_len))
 
-        batch = self.tokenizer.pad(
-            concatenated_features,
-            padding=self.padding,
-            max_length=self.max_length,
-            pad_to_multiple_of=self.pad_to_multiple_of,
-            return_tensors=self.return_tensors,
-        )
+        batch = super().__call__(concatenated_features)
         batch["labels"] = self._pad_labels(batch["input_ids"], label_positions)
         return batch
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/dpo/trainer.py` & `llmtuner-0.6.2/src/llmtuner/train/dpo/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,50 +70,59 @@
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
     ) -> "torch.optim.lr_scheduler.LRScheduler":
         create_custom_scheduler(self.args, num_training_steps, optimizer)
         return super().create_scheduler(num_training_steps, optimizer)
 
-    def sft_loss(self, chosen_logits: torch.FloatTensor, chosen_labels: torch.LongTensor) -> torch.Tensor:
+    def sft_loss(self, chosen_logits: "torch.FloatTensor", chosen_labels: "torch.LongTensor") -> "torch.Tensor":
         r"""
         Computes supervised cross-entropy loss of given labels under the given logits.
 
         Returns:
             A tensor of shape (batch_size,) containing the cross-entropy loss of each samples.
         """
         all_logps = self.get_batch_logps(chosen_logits, chosen_labels, average_log_prob=True)
         return -all_logps
 
     def concatenated_forward(
-        self, model: "PreTrainedModel", batch: Dict[str, torch.Tensor]
-    ) -> Tuple[torch.FloatTensor, torch.FloatTensor, torch.FloatTensor, torch.FloatTensor]:
+        self, model: "PreTrainedModel", batch: Dict[str, "torch.Tensor"]
+    ) -> Tuple["torch.Tensor", "torch.Tensor", "torch.Tensor", "torch.Tensor"]:
+        r"""
+        Computes the sum log probabilities of the labels under the given logits if loss_type != IPO.
+
+        Otherwise the average log probabilities.
+        """
         batch_copied = BatchEncoding({k: v.detach().clone() for k, v in batch.items()})  # avoid error
 
-        all_logits = model(
-            input_ids=batch_copied["input_ids"], attention_mask=batch_copied["attention_mask"], return_dict=True
+        all_logits: "torch.Tensor" = model(
+            input_ids=batch_copied["input_ids"],
+            attention_mask=batch_copied["attention_mask"],
+            return_dict=True,
+            use_cache=False,
         ).logits.to(torch.float32)
 
         all_logps = self.get_batch_logps(
-            all_logits,
-            batch["labels"],
-            average_log_prob=False,
+            logits=all_logits,
+            labels=batch_copied["labels"],
+            average_log_prob=(self.loss_type == "ipo"),
+            is_encoder_decoder=self.is_encoder_decoder,
             label_pad_token_id=self.label_pad_token_id,
         )
         batch_size = batch["input_ids"].size(0) // 2
         chosen_logps, rejected_logps = all_logps.split(batch_size, dim=0)
         chosen_logits, rejected_logits = all_logits.split(batch_size, dim=0)
         return chosen_logps, rejected_logps, chosen_logits, rejected_logits
 
     def get_batch_loss_metrics(
         self,
         model: "PreTrainedModel",
-        batch: Dict[str, torch.Tensor],
+        batch: Dict[str, "torch.Tensor"],
         train_eval: Literal["train", "eval"] = "train",
-    ) -> Tuple[torch.Tensor, Dict[str, torch.Tensor]]:
+    ) -> Tuple["torch.Tensor", Dict[str, "torch.Tensor"]]:
         r"""
         Computes the DPO loss and other metrics for the given batch of inputs for train or test.
         """
         metrics = {}
         (
             policy_chosen_logps,
             policy_rejected_logps,
@@ -146,17 +155,17 @@
             batch_size = batch["input_ids"].size(0) // 2
             chosen_labels, _ = batch["labels"].split(batch_size, dim=0)
             losses += self.ftx_gamma * self.sft_loss(policy_chosen_logits, chosen_labels)
 
         reward_accuracies = (chosen_rewards > rejected_rewards).float()
 
         prefix = "eval_" if train_eval == "eval" else ""
-        metrics[f"{prefix}rewards/chosen"] = chosen_rewards.cpu().mean()
-        metrics[f"{prefix}rewards/rejected"] = rejected_rewards.cpu().mean()
-        metrics[f"{prefix}rewards/accuracies"] = reward_accuracies.cpu().mean()
-        metrics[f"{prefix}rewards/margins"] = (chosen_rewards - rejected_rewards).cpu().mean()
-        metrics[f"{prefix}logps/rejected"] = policy_rejected_logps.detach().cpu().mean()
-        metrics[f"{prefix}logps/chosen"] = policy_chosen_logps.detach().cpu().mean()
-        metrics[f"{prefix}logits/rejected"] = policy_rejected_logits.detach().cpu().mean()
-        metrics[f"{prefix}logits/chosen"] = policy_chosen_logits.detach().cpu().mean()
+        metrics["{}rewards/chosen".format(prefix)] = chosen_rewards.cpu().mean()
+        metrics["{}rewards/rejected".format(prefix)] = rejected_rewards.cpu().mean()
+        metrics["{}rewards/accuracies".format(prefix)] = reward_accuracies.cpu().mean()
+        metrics["{}rewards/margins".format(prefix)] = (chosen_rewards - rejected_rewards).cpu().mean()
+        metrics["{}logps/rejected".format(prefix)] = policy_rejected_logps.detach().cpu().mean()
+        metrics["{}logps/chosen".format(prefix)] = policy_chosen_logps.detach().cpu().mean()
+        metrics["{}logits/rejected".format(prefix)] = policy_rejected_logits.detach().cpu().mean()
+        metrics["{}logits/chosen".format(prefix)] = policy_chosen_logits.detach().cpu().mean()
 
         return losses.mean(), metrics
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/dpo/workflow.py` & `llmtuner-0.6.2/src/llmtuner/train/dpo/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Inspired by: https://github.com/huggingface/trl/blob/main/examples/research_projects/stack_llama_2/scripts/dpo_llama2.py
 
 from typing import TYPE_CHECKING, List, Optional
 
-from ...data import get_dataset, split_dataset
+from ...data import PairwiseDataCollatorWithPadding, get_dataset, split_dataset
 from ...extras.constants import IGNORE_INDEX
 from ...extras.ploting import plot_loss
 from ...hparams import ModelArguments
 from ...model import load_model, load_tokenizer
 from ..utils import create_modelcard_and_push, create_ref_model
-from .collator import DPODataCollatorWithPadding
 from .trainer import CustomDPOTrainer
 
 
 if TYPE_CHECKING:
     from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
     from ...hparams import DataArguments, FinetuningArguments
@@ -25,15 +24,15 @@
     finetuning_args: "FinetuningArguments",
     callbacks: Optional[List["TrainerCallback"]] = None,
 ):
     tokenizer = load_tokenizer(model_args)
     dataset = get_dataset(tokenizer, model_args, data_args, training_args, stage="rm")
     model = load_model(tokenizer, model_args, finetuning_args, training_args.do_train)
 
-    data_collator = DPODataCollatorWithPadding(
+    data_collator = PairwiseDataCollatorWithPadding(
         tokenizer=tokenizer,
         pad_to_multiple_of=8,
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id,
     )
 
     # Create reference model
     if finetuning_args.ref_model is None and (not training_args.do_train):  # use the model itself
@@ -60,15 +59,15 @@
     if training_args.do_train:
         train_result = trainer.train(resume_from_checkpoint=training_args.resume_from_checkpoint)
         trainer.save_model()
         trainer.log_metrics("train", train_result.metrics)
         trainer.save_metrics("train", train_result.metrics)
         trainer.save_state()
         if trainer.is_world_process_zero() and finetuning_args.plot_loss:
-            plot_loss(training_args.output_dir, keys=["loss", "eval_loss"])
+            plot_loss(training_args.output_dir, keys=["loss", "eval_loss", "rewards/accuracies"])
 
     # Evaluation
     if training_args.do_eval:
         metrics = trainer.evaluate(metric_key_prefix="eval")
         if id(model) == id(ref_model):  # unable to compute rewards without a reference model
             remove_keys = [key for key in metrics.keys() if "rewards" in key]
             for key in remove_keys:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/ppo/trainer.py` & `llmtuner-0.6.2/src/llmtuner/train/ppo/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             seed=training_args.seed,
             optimize_device_cache=True,
             target=finetuning_args.ppo_target,
             use_score_scaling=finetuning_args.ppo_score_norm,
             use_score_norm=finetuning_args.ppo_score_norm,
             whiten_rewards=finetuning_args.ppo_whiten_rewards,
             accelerator_kwargs={"step_scheduler_with_optimizer": False},
-            log_with=training_args.report_to[0] if training_args.report_to is not None else None,
+            log_with=training_args.report_to[0] if training_args.report_to else None,
             project_kwargs={"logging_dir": training_args.logging_dir},
         )
 
         # Create optimizer and scheduler
         if training_args.max_steps > 0:
             num_training_steps = training_args.max_steps
         else:
@@ -349,15 +349,15 @@
             reward_model = self.model
         else:
             reward_model = self.reward_model
 
         batch = self.prepare_model_inputs(queries, responses)
 
         with torch.cuda.amp.autocast(dtype=self.model_args.compute_dtype):  # support bf16
-            _, _, values = reward_model(**batch, output_hidden_states=True, return_dict=True)
+            _, _, values = reward_model(**batch, output_hidden_states=True, return_dict=True, use_cache=False)
 
         if getattr(unwrapped_model.config, "model_type", None) == "chatglm":  # assume same architecture
             values = torch.transpose(values, 0, 1)
 
         rewards = []
         for i in range(values.size(0)):
             end_indexes = (batch["input_ids"][i] != self.tokenizer.pad_token_id).nonzero()
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/ppo/utils.py` & `llmtuner-0.6.2/src/llmtuner/train/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/ppo/workflow.py` & `llmtuner-0.6.2/src/llmtuner/train/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/pt/trainer.py` & `llmtuner-0.6.2/src/llmtuner/train/pt/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/pt/workflow.py` & `llmtuner-0.6.2/src/llmtuner/train/pt/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/rm/trainer.py` & `llmtuner-0.6.2/src/llmtuner/train/rm/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/rm/workflow.py` & `llmtuner-0.6.2/src/llmtuner/train/rm/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Inspired by: https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
 from typing import TYPE_CHECKING, List, Optional
 
-from ...data import get_dataset, split_dataset
+from ...data import PairwiseDataCollatorWithPadding, get_dataset, split_dataset
 from ...extras.callbacks import FixValueHeadModelCallback
 from ...extras.misc import fix_valuehead_checkpoint
 from ...extras.ploting import plot_loss
 from ...model import load_model, load_tokenizer
 from ..utils import create_modelcard_and_push
-from .collator import PairwiseDataCollatorWithPadding
 from .metric import compute_accuracy
 from .trainer import PairwiseTrainer
 
 
 if TYPE_CHECKING:
     from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
@@ -52,15 +51,15 @@
         trainer.save_model()
         if training_args.should_save:
             fix_valuehead_checkpoint(model, training_args.output_dir, training_args.save_safetensors)
         trainer.log_metrics("train", train_result.metrics)
         trainer.save_metrics("train", train_result.metrics)
         trainer.save_state()
         if trainer.is_world_process_zero() and finetuning_args.plot_loss:
-            plot_loss(training_args.output_dir, keys=["loss", "eval_loss"])
+            plot_loss(training_args.output_dir, keys=["loss", "eval_loss", "eval_accuracy"])
 
     # Evaluation
     if training_args.do_eval:
         metrics = trainer.evaluate(metric_key_prefix="eval")
         trainer.log_metrics("eval", metrics)
         trainer.save_metrics("eval", metrics)
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/sft/metric.py` & `llmtuner-0.6.2/src/llmtuner/train/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/sft/trainer.py` & `llmtuner-0.6.2/src/llmtuner/train/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/sft/workflow.py` & `llmtuner-0.6.2/src/llmtuner/train/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/train/tuner.py` & `llmtuner-0.6.2/src/llmtuner/train/tuner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import torch
 from transformers import PreTrainedModel
 
 from ..data import get_template_and_fix_tokenizer
 from ..extras.callbacks import LogCallback
 from ..extras.logging import get_logger
 from ..hparams import get_infer_args, get_train_args
-from ..model import load_model_and_tokenizer
+from ..model import load_model, load_tokenizer
 from .dpo import run_dpo
+from .orpo import run_orpo
 from .ppo import run_ppo
 from .pt import run_pt
 from .rm import run_rm
 from .sft import run_sft
 
 
 if TYPE_CHECKING:
@@ -32,50 +33,45 @@
         run_sft(model_args, data_args, training_args, finetuning_args, generating_args, callbacks)
     elif finetuning_args.stage == "rm":
         run_rm(model_args, data_args, training_args, finetuning_args, callbacks)
     elif finetuning_args.stage == "ppo":
         run_ppo(model_args, data_args, training_args, finetuning_args, generating_args, callbacks)
     elif finetuning_args.stage == "dpo":
         run_dpo(model_args, data_args, training_args, finetuning_args, callbacks)
+    elif finetuning_args.stage == "orpo":
+        run_orpo(model_args, data_args, training_args, finetuning_args, callbacks)
     else:
         raise ValueError("Unknown task.")
 
 
 def export_model(args: Optional[Dict[str, Any]] = None):
     model_args, data_args, finetuning_args, _ = get_infer_args(args)
 
     if model_args.export_dir is None:
         raise ValueError("Please specify `export_dir` to save model.")
 
     if model_args.adapter_name_or_path is not None and model_args.export_quantization_bit is not None:
         raise ValueError("Please merge adapters before quantizing the model.")
 
-    model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args)
+    tokenizer = load_tokenizer(model_args)
     get_template_and_fix_tokenizer(tokenizer, data_args.template)
+    model = load_model(tokenizer, model_args, finetuning_args)  # must after fixing tokenizer to resize vocab
 
     if getattr(model, "quantization_method", None) and model_args.adapter_name_or_path is not None:
         raise ValueError("Cannot merge adapters to a quantized model.")
 
     if not isinstance(model, PreTrainedModel):
         raise ValueError("The model is not a `PreTrainedModel`, export aborted.")
 
     if getattr(model, "quantization_method", None) is None:  # cannot convert dtype of a quantized model
         output_dtype = getattr(model.config, "torch_dtype", torch.float16)
         setattr(model.config, "torch_dtype", output_dtype)
         for param in model.parameters():
             param.data = param.data.to(output_dtype)
 
-    gen_config = model.generation_config  # check and fix generation config
-    if not gen_config.do_sample and (
-        (gen_config.temperature is not None and gen_config.temperature != 1.0)
-        or (gen_config.top_p is not None and gen_config.top_p != 1.0)
-        or (gen_config.typical_p is not None and gen_config.typical_p != 1.0)
-    ):
-        gen_config.do_sample = True
-
     model.save_pretrained(
         save_directory=model_args.export_dir,
         max_shard_size="{}GB".format(model_args.export_size),
         safe_serialization=(not model_args.export_legacy_format),
     )
     if model_args.export_hub_model_id is not None:
         model.push_to_hub(
```

### Comparing `llmtuner-0.6.1/src/llmtuner/train/utils.py` & `llmtuner-0.6.2/src/llmtuner/train/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from transformers.pytorch_utils import ALL_LAYERNORM_LAYERS
 from transformers.trainer_pt_utils import get_parameter_names
 from transformers.utils.versions import require_version
 
 from ..extras.logging import get_logger
 from ..extras.packages import is_galore_available
 from ..hparams import FinetuningArguments, ModelArguments
-from ..model import find_all_linear_modules, load_model_and_tokenizer, load_valuehead_params
+from ..model import find_all_linear_modules, load_model, load_tokenizer, load_valuehead_params
 
 
 if is_galore_available():
     from galore_torch import GaLoreAdafactor, GaLoreAdamW, GaLoreAdamW8bit
 
 
 if TYPE_CHECKING:
@@ -83,24 +83,26 @@
                 model_name_or_path=finetuning_args.ref_model,
                 adapter_name_or_path=finetuning_args.ref_model_adapters,
                 quantization_bit=finetuning_args.ref_model_quantization_bit,
             )
         )
         ref_model_args = ModelArguments(**ref_model_args_dict)
         ref_finetuning_args = FinetuningArguments(finetuning_type="lora")
-        ref_model, _ = load_model_and_tokenizer(
-            ref_model_args, ref_finetuning_args, is_trainable=False, add_valuehead=add_valuehead
+        tokenizer = load_tokenizer(ref_model_args)
+        ref_model = load_model(
+            tokenizer, ref_model_args, ref_finetuning_args, is_trainable=False, add_valuehead=add_valuehead
         )
         logger.info("Created reference model from {}".format(finetuning_args.ref_model))
     else:
         if finetuning_args.finetuning_type == "lora":
             ref_model = None
         else:
-            ref_model, _ = load_model_and_tokenizer(
-                model_args, finetuning_args, is_trainable=False, add_valuehead=add_valuehead
+            tokenizer = load_tokenizer(model_args)
+            ref_model = load_model(
+                tokenizer, model_args, finetuning_args, is_trainable=False, add_valuehead=add_valuehead
             )
             logger.info("Created reference model from the model itself.")
 
     return ref_model
 
 
 def create_reward_model(
@@ -137,16 +139,17 @@
                 model_name_or_path=finetuning_args.reward_model,
                 adapter_name_or_path=finetuning_args.reward_model_adapters,
                 quantization_bit=finetuning_args.reward_model_quantization_bit,
             )
         )
         reward_model_args = ModelArguments(**reward_model_args_dict)
         reward_finetuning_args = FinetuningArguments(finetuning_type="lora")
-        reward_model, _ = load_model_and_tokenizer(
-            reward_model_args, reward_finetuning_args, is_trainable=False, add_valuehead=True
+        tokenizer = load_tokenizer(reward_model_args)
+        reward_model = load_model(
+            tokenizer, reward_model_args, reward_finetuning_args, is_trainable=False, add_valuehead=True
         )
         logger.info("Loaded full weights of reward model from {}".format(finetuning_args.reward_model))
         logger.warning("Please ensure the ppo model and reward model share SAME tokenizer and vocabulary.")
         return reward_model
 
 
 def _get_decay_parameter_names(model: "PreTrainedModel") -> List[str]:
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/chatter.py` & `llmtuner-0.6.2/src/llmtuner/webui/chatter.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             super().__init__(dict(model_name_or_path=model_name_or_path, template=template))
 
     @property
     def loaded(self) -> bool:
         return self.engine is not None
 
     def load_model(self, data: Dict[Component, Any]) -> Generator[str, None, None]:
-        get = lambda name: data[self.manager.get_elem_by_name(name)]
+        get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         lang = get("top.lang")
         error = ""
         if self.loaded:
             error = ALERTS["err_exists"][lang]
         elif not get("top.model_name"):
             error = ALERTS["err_no_model"][lang]
         elif not get("top.model_path"):
@@ -76,62 +76,61 @@
             infer_backend=get("infer.infer_backend"),
         )
         super().__init__(args)
 
         yield ALERTS["info_loaded"][lang]
 
     def unload_model(self, data: Dict[Component, Any]) -> Generator[str, None, None]:
-        lang = data[self.manager.get_elem_by_name("top.lang")]
+        lang = data[self.manager.get_elem_by_id("top.lang")]
 
         if self.demo_mode:
             gr.Warning(ALERTS["err_demo"][lang])
             yield ALERTS["err_demo"][lang]
             return
 
         yield ALERTS["info_unloading"][lang]
         self.engine = None
         torch_gc()
         yield ALERTS["info_unloaded"][lang]
 
-    def predict(
+    def append(
         self,
-        chatbot: List[Tuple[str, str]],
+        chatbot: List[List[Optional[str]]],
+        messages: Sequence[Dict[str, str]],
         role: str,
         query: str,
-        messages: Sequence[Tuple[str, str]],
+    ) -> Tuple[List[List[Optional[str]]], List[Dict[str, str]], str]:
+        return chatbot + [[query, None]], messages + [{"role": role, "content": query}], ""
+
+    def stream(
+        self,
+        chatbot: List[List[Optional[str]]],
+        messages: Sequence[Dict[str, str]],
         system: str,
         tools: str,
         max_new_tokens: int,
         top_p: float,
         temperature: float,
-    ) -> Generator[Tuple[Sequence[Tuple[str, str]], Sequence[Tuple[str, str]]], None, None]:
-        chatbot.append([query, ""])
-        query_messages = messages + [{"role": role, "content": query}]
+    ) -> Generator[Tuple[List[List[Optional[str]]], List[Dict[str, str]]], None, None]:
+        chatbot[-1][1] = ""
         response = ""
         for new_text in self.stream_chat(
-            query_messages, system, tools, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
+            messages, system, tools, max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature
         ):
             response += new_text
             if tools:
                 result = self.engine.template.format_tools.extract(response)
             else:
                 result = response
 
             if isinstance(result, tuple):
                 name, arguments = result
                 arguments = json.loads(arguments)
                 tool_call = json.dumps({"name": name, "arguments": arguments}, ensure_ascii=False)
-                output_messages = query_messages + [{"role": Role.FUNCTION.value, "content": tool_call}]
+                output_messages = messages + [{"role": Role.FUNCTION.value, "content": tool_call}]
                 bot_text = "```json\n" + tool_call + "\n```"
             else:
-                output_messages = query_messages + [{"role": Role.ASSISTANT.value, "content": result}]
+                output_messages = messages + [{"role": Role.ASSISTANT.value, "content": result}]
                 bot_text = result
 
-            chatbot[-1] = [query, self.postprocess(bot_text)]
+            chatbot[-1][1] = bot_text
             yield chatbot, output_messages
-
-    def postprocess(self, response: str) -> str:
-        blocks = response.split("```")
-        for i, block in enumerate(blocks):
-            if i % 2 == 0:
-                blocks[i] = block.replace("<", "&lt;").replace(">", "&gt;")
-        return "```".join(blocks)
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/common.py` & `llmtuner-0.6.2/src/llmtuner/webui/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,36 +7,42 @@
 from peft.utils import SAFETENSORS_WEIGHTS_NAME, WEIGHTS_NAME
 
 from ..extras.constants import (
     DATA_CONFIG,
     DEFAULT_MODULE,
     DEFAULT_TEMPLATE,
     PEFT_METHODS,
+    STAGES_USE_PAIR_DATA,
     SUPPORTED_MODELS,
     TRAINING_STAGES,
     DownloadSource,
 )
 from ..extras.misc import use_modelscope
 
 
 ADAPTER_NAMES = {WEIGHTS_NAME, SAFETENSORS_WEIGHTS_NAME}
 DEFAULT_CACHE_DIR = "cache"
+DEFAULT_CONFIG_DIR = "config"
 DEFAULT_DATA_DIR = "data"
 DEFAULT_SAVE_DIR = "saves"
 USER_CONFIG = "user.config"
 
 
 def get_save_dir(*args) -> os.PathLike:
     return os.path.join(DEFAULT_SAVE_DIR, *args)
 
 
 def get_config_path() -> os.PathLike:
     return os.path.join(DEFAULT_CACHE_DIR, USER_CONFIG)
 
 
+def get_save_path(config_path: str) -> os.PathLike:
+    return os.path.join(DEFAULT_CONFIG_DIR, config_path)
+
+
 def load_config() -> Dict[str, Any]:
     try:
         with open(get_config_path(), "r", encoding="utf-8") as f:
             return json.load(f)
     except Exception:
         return {"lang": None, "last_model": None, "path_dict": {}, "cache_dir": None}
 
@@ -48,14 +54,30 @@
     if model_name:
         user_config["last_model"] = model_name
         user_config["path_dict"][model_name] = model_path
     with open(get_config_path(), "w", encoding="utf-8") as f:
         json.dump(user_config, f, indent=2, ensure_ascii=False)
 
 
+def load_args(config_path: str) -> Optional[Dict[str, Any]]:
+    try:
+        with open(get_save_path(config_path), "r", encoding="utf-8") as f:
+            return json.load(f)
+    except Exception:
+        return None
+
+
+def save_args(config_path: str, config_dict: Dict[str, Any]) -> str:
+    os.makedirs(DEFAULT_CONFIG_DIR, exist_ok=True)
+    with open(get_save_path(config_path), "w", encoding="utf-8") as f:
+        json.dump(config_dict, f, indent=2, ensure_ascii=False)
+
+    return str(get_save_path(config_path))
+
+
 def get_model_path(model_name: str) -> str:
     user_config = load_config()
     path_dict: Dict[DownloadSource, str] = SUPPORTED_MODELS.get(model_name, defaultdict(str))
     model_path = user_config["path_dict"].get(model_name, None) or path_dict.get(DownloadSource.DEFAULT, None)
     if (
         use_modelscope()
         and path_dict.get(DownloadSource.MODELSCOPE)
@@ -75,41 +97,41 @@
 
 def get_template(model_name: str) -> str:
     if model_name and model_name.endswith("Chat") and get_prefix(model_name) in DEFAULT_TEMPLATE:
         return DEFAULT_TEMPLATE[get_prefix(model_name)]
     return "default"
 
 
-def list_adapters(model_name: str, finetuning_type: str) -> Dict[str, Any]:
+def list_adapters(model_name: str, finetuning_type: str) -> "gr.Dropdown":
     if finetuning_type not in PEFT_METHODS:
-        return gr.update(value=[], choices=[], interactive=False)
+        return gr.Dropdown(value=[], choices=[], interactive=False)
 
     adapters = []
     if model_name and finetuning_type == "lora":
         save_dir = get_save_dir(model_name, finetuning_type)
         if save_dir and os.path.isdir(save_dir):
             for adapter in os.listdir(save_dir):
                 if os.path.isdir(os.path.join(save_dir, adapter)) and any(
                     os.path.isfile(os.path.join(save_dir, adapter, name)) for name in ADAPTER_NAMES
                 ):
                     adapters.append(adapter)
-    return gr.update(value=[], choices=adapters, interactive=True)
+    return gr.Dropdown(value=[], choices=adapters, interactive=True)
 
 
 def load_dataset_info(dataset_dir: str) -> Dict[str, Dict[str, Any]]:
     try:
         with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
             return json.load(f)
     except Exception as err:
         print("Cannot open {} due to {}.".format(os.path.join(dataset_dir, DATA_CONFIG), str(err)))
         return {}
 
 
-def list_dataset(dataset_dir: str = None, training_stage: str = list(TRAINING_STAGES.keys())[0]) -> Dict[str, Any]:
+def list_dataset(dataset_dir: str = None, training_stage: str = list(TRAINING_STAGES.keys())[0]) -> "gr.Dropdown":
     dataset_info = load_dataset_info(dataset_dir if dataset_dir is not None else DEFAULT_DATA_DIR)
-    ranking = TRAINING_STAGES[training_stage] in ["rm", "dpo"]
+    ranking = TRAINING_STAGES[training_stage] in STAGES_USE_PAIR_DATA
     datasets = [k for k, v in dataset_info.items() if v.get("ranking", False) == ranking]
-    return gr.update(value=[], choices=datasets)
+    return gr.Dropdown(value=[], choices=datasets)
 
 
-def autoset_packing(training_stage: str = list(TRAINING_STAGES.keys())[0]) -> Dict[str, Any]:
-    return gr.update(value=(TRAINING_STAGES[training_stage] == "pt"))
+def autoset_packing(training_stage: str = list(TRAINING_STAGES.keys())[0]) -> "gr.Button":
+    return gr.Button(value=(TRAINING_STAGES[training_stage] == "pt"))
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/chatbot.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 import gradio as gr
 
 from ...data import Role
 from ..utils import check_json_schema
 
 
 if TYPE_CHECKING:
-    from gradio.blocks import Block
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_chat_box(
     engine: "Engine", visible: bool = False
-) -> Tuple["Block", "Component", "Component", Dict[str, "Component"]]:
-    with gr.Box(visible=visible) as chat_box:
-        chatbot = gr.Chatbot()
+) -> Tuple["gr.Column", "Component", "Component", Dict[str, "Component"]]:
+    with gr.Column(visible=visible) as chat_box:
+        chatbot = gr.Chatbot(show_copy_button=True)
         messages = gr.State([])
         with gr.Row():
             with gr.Column(scale=4):
                 role = gr.Dropdown(choices=[Role.USER.value, Role.OBSERVATION.value], value=Role.USER.value)
                 system = gr.Textbox(show_label=False)
                 tools = gr.Textbox(show_label=False, lines=2)
                 query = gr.Textbox(show_label=False, lines=8)
@@ -29,24 +28,26 @@
 
             with gr.Column(scale=1):
                 max_new_tokens = gr.Slider(8, 4096, value=512, step=1)
                 top_p = gr.Slider(0.01, 1.0, value=0.7, step=0.01)
                 temperature = gr.Slider(0.01, 1.5, value=0.95, step=0.01)
                 clear_btn = gr.Button()
 
-    tools.input(check_json_schema, [tools, engine.manager.get_elem_by_name("top.lang")])
+    tools.input(check_json_schema, inputs=[tools, engine.manager.get_elem_by_id("top.lang")])
 
     submit_btn.click(
-        engine.chatter.predict,
-        [chatbot, role, query, messages, system, tools, max_new_tokens, top_p, temperature],
+        engine.chatter.append,
+        [chatbot, messages, role, query],
+        [chatbot, messages, query],
+    ).then(
+        engine.chatter.stream,
+        [chatbot, messages, system, tools, max_new_tokens, top_p, temperature],
         [chatbot, messages],
-        show_progress=True,
-    ).then(lambda: gr.update(value=""), outputs=[query])
-
-    clear_btn.click(lambda: ([], []), outputs=[chatbot, messages], show_progress=True)
+    )
+    clear_btn.click(lambda: ([], []), outputs=[chatbot, messages])
 
     return (
         chat_box,
         chatbot,
         messages,
         dict(
             role=role,
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/data.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import os
-from typing import TYPE_CHECKING, Any, Dict, Tuple
+from typing import TYPE_CHECKING, Dict, Tuple
 
 import gradio as gr
 
 from ...extras.constants import DATA_CONFIG
 
 
 if TYPE_CHECKING:
@@ -18,44 +18,44 @@
     return page_index - 1 if page_index > 0 else page_index
 
 
 def next_page(page_index: int, total_num: int) -> int:
     return page_index + 1 if (page_index + 1) * PAGE_SIZE < total_num else page_index
 
 
-def can_preview(dataset_dir: str, dataset: list) -> Dict[str, Any]:
+def can_preview(dataset_dir: str, dataset: list) -> "gr.Button":
     try:
         with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
             dataset_info = json.load(f)
     except Exception:
-        return gr.update(interactive=False)
+        return gr.Button(interactive=False)
 
     if (
         len(dataset) > 0
         and "file_name" in dataset_info[dataset[0]]
         and os.path.isfile(os.path.join(dataset_dir, dataset_info[dataset[0]]["file_name"]))
     ):
-        return gr.update(interactive=True)
+        return gr.Button(interactive=True)
     else:
-        return gr.update(interactive=False)
+        return gr.Button(interactive=False)
 
 
-def get_preview(dataset_dir: str, dataset: list, page_index: int) -> Tuple[int, list, Dict[str, Any]]:
+def get_preview(dataset_dir: str, dataset: list, page_index: int) -> Tuple[int, list, "gr.Column"]:
     with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
 
     data_file: str = dataset_info[dataset[0]]["file_name"]
     with open(os.path.join(dataset_dir, data_file), "r", encoding="utf-8") as f:
         if data_file.endswith(".json"):
             data = json.load(f)
         elif data_file.endswith(".jsonl"):
             data = [json.loads(line) for line in f]
         else:
             data = [line for line in f]  # noqa: C416
-    return len(data), data[PAGE_SIZE * page_index : PAGE_SIZE * (page_index + 1)], gr.update(visible=True)
+    return len(data), data[PAGE_SIZE * page_index : PAGE_SIZE * (page_index + 1)], gr.Column(visible=True)
 
 
 def create_preview_box(dataset_dir: "gr.Textbox", dataset: "gr.Dropdown") -> Dict[str, "Component"]:
     data_preview_btn = gr.Button(interactive=False, scale=1)
     with gr.Column(visible=False, elem_classes="modal-box") as preview_box:
         with gr.Row():
             preview_count = gr.Number(value=0, interactive=False, precision=0)
@@ -63,29 +63,29 @@
 
         with gr.Row():
             prev_btn = gr.Button()
             next_btn = gr.Button()
             close_btn = gr.Button()
 
         with gr.Row():
-            preview_samples = gr.JSON(interactive=False)
+            preview_samples = gr.JSON()
 
     dataset.change(can_preview, [dataset_dir, dataset], [data_preview_btn], queue=False).then(
         lambda: 0, outputs=[page_index], queue=False
     )
     data_preview_btn.click(
         get_preview, [dataset_dir, dataset, page_index], [preview_count, preview_samples, preview_box], queue=False
     )
     prev_btn.click(prev_page, [page_index], [page_index], queue=False).then(
         get_preview, [dataset_dir, dataset, page_index], [preview_count, preview_samples, preview_box], queue=False
     )
     next_btn.click(next_page, [page_index, preview_count], [page_index], queue=False).then(
         get_preview, [dataset_dir, dataset, page_index], [preview_count, preview_samples, preview_box], queue=False
     )
-    close_btn.click(lambda: gr.update(visible=False), outputs=[preview_box], queue=False)
+    close_btn.click(lambda: gr.Column(visible=False), outputs=[preview_box], queue=False)
     return dict(
         data_preview_btn=data_preview_btn,
         preview_count=preview_count,
         page_index=page_index,
         prev_btn=prev_btn,
         next_btn=next_btn,
         close_btn=close_btn,
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/eval.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/eval.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,17 @@
 
 def create_eval_tab(engine: "Engine") -> Dict[str, "Component"]:
     input_elems = engine.manager.get_base_elems()
     elem_dict = dict()
 
     with gr.Row():
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
-        dataset = gr.Dropdown(multiselect=True, scale=4)
+        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
-    dataset_dir.change(list_dataset, [dataset_dir], [dataset], queue=False)
-
     input_elems.update({dataset_dir, dataset})
     elem_dict.update(dict(dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
         cutoff_len = gr.Slider(value=1024, minimum=4, maximum=8192, step=1)
         max_samples = gr.Textbox(value="100000")
         batch_size = gr.Slider(value=8, minimum=1, maximum=512, step=1)
@@ -42,35 +40,37 @@
         output_dir = gr.Textbox()
 
     input_elems.update({max_new_tokens, top_p, temperature, output_dir})
     elem_dict.update(dict(max_new_tokens=max_new_tokens, top_p=top_p, temperature=temperature, output_dir=output_dir))
 
     with gr.Row():
         cmd_preview_btn = gr.Button()
-        start_btn = gr.Button()
-        stop_btn = gr.Button()
+        start_btn = gr.Button(variant="primary")
+        stop_btn = gr.Button(variant="stop")
 
     with gr.Row():
-        resume_btn = gr.Checkbox(visible=False, interactive=False, value=False)
+        resume_btn = gr.Checkbox(visible=False, interactive=False)
         process_bar = gr.Slider(visible=False, interactive=False)
 
-    with gr.Box():
+    with gr.Row():
         output_box = gr.Markdown()
 
     output_elems = [output_box, process_bar]
     elem_dict.update(
         dict(
             cmd_preview_btn=cmd_preview_btn,
             start_btn=start_btn,
             stop_btn=stop_btn,
             resume_btn=resume_btn,
             process_bar=process_bar,
             output_box=output_box,
         )
     )
 
-    cmd_preview_btn.click(engine.runner.preview_eval, input_elems, output_elems)
+    cmd_preview_btn.click(engine.runner.preview_eval, input_elems, output_elems, concurrency_limit=None)
     start_btn.click(engine.runner.run_eval, input_elems, output_elems)
-    stop_btn.click(engine.runner.set_abort, queue=False)
-    resume_btn.change(engine.runner.monitor, outputs=output_elems)
+    stop_btn.click(engine.runner.set_abort)
+    resume_btn.change(engine.runner.monitor, outputs=output_elems, concurrency_limit=None)
+
+    dataset_dir.change(list_dataset, [dataset_dir], [dataset], queue=False)
 
     return elem_dict
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/export.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,35 +70,35 @@
     yield ALERTS["info_exporting"][lang]
     export_model(args)
     yield ALERTS["info_exported"][lang]
 
 
 def create_export_tab(engine: "Engine") -> Dict[str, "Component"]:
     with gr.Row():
-        max_shard_size = gr.Slider(value=1, minimum=1, maximum=100)
+        max_shard_size = gr.Slider(value=1, minimum=1, maximum=100, step=1)
         export_quantization_bit = gr.Dropdown(choices=["none", "8", "4", "3", "2"], value="none")
         export_quantization_dataset = gr.Textbox(value="data/c4_demo.json")
         export_legacy_format = gr.Checkbox()
 
     with gr.Row():
         export_dir = gr.Textbox()
         export_hub_model_id = gr.Textbox()
 
     export_btn = gr.Button()
     info_box = gr.Textbox(show_label=False, interactive=False)
 
     export_btn.click(
         save_model,
         [
-            engine.manager.get_elem_by_name("top.lang"),
-            engine.manager.get_elem_by_name("top.model_name"),
-            engine.manager.get_elem_by_name("top.model_path"),
-            engine.manager.get_elem_by_name("top.adapter_path"),
-            engine.manager.get_elem_by_name("top.finetuning_type"),
-            engine.manager.get_elem_by_name("top.template"),
+            engine.manager.get_elem_by_id("top.lang"),
+            engine.manager.get_elem_by_id("top.model_name"),
+            engine.manager.get_elem_by_id("top.model_path"),
+            engine.manager.get_elem_by_id("top.adapter_path"),
+            engine.manager.get_elem_by_id("top.finetuning_type"),
+            engine.manager.get_elem_by_id("top.template"),
             max_shard_size,
             export_quantization_bit,
             export_quantization_dataset,
             export_legacy_format,
             export_dir,
             export_hub_model_id,
         ],
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/infer.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/infer.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         unload_btn = gr.Button()
 
     info_box = gr.Textbox(show_label=False, interactive=False)
 
     input_elems.update({infer_backend})
     elem_dict.update(dict(infer_backend=infer_backend, load_btn=load_btn, unload_btn=unload_btn, info_box=info_box))
 
-    chat_box, chatbot, history, chat_elems = create_chat_box(engine, visible=False)
+    chat_box, chatbot, messages, chat_elems = create_chat_box(engine, visible=False)
     elem_dict.update(dict(chat_box=chat_box, **chat_elems))
 
     load_btn.click(engine.chatter.load_model, input_elems, [info_box]).then(
-        lambda: gr.update(visible=engine.chatter.loaded), outputs=[chat_box]
+        lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_box]
     )
 
     unload_btn.click(engine.chatter.unload_model, input_elems, [info_box]).then(
-        lambda: ([], []), outputs=[chatbot, history]
-    ).then(lambda: gr.update(visible=engine.chatter.loaded), outputs=[chat_box])
+        lambda: ([], []), outputs=[chatbot, messages]
+    ).then(lambda: gr.Column(visible=engine.chatter.loaded), outputs=[chat_box])
 
     return elem_dict
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/top.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/top.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from typing import TYPE_CHECKING, Dict, Tuple
+from typing import TYPE_CHECKING, Dict
 
 import gradio as gr
 
 from ...data import templates
 from ...extras.constants import METHODS, SUPPORTED_MODELS
 from ..common import get_model_path, get_template, list_adapters, save_config
 from ..utils import can_quantize
 
 
 if TYPE_CHECKING:
     from gradio.components import Component
 
 
-def create_top() -> Tuple["gr.Dropdown", Dict[str, "Component"]]:
+def create_top() -> Dict[str, "Component"]:
     available_models = list(SUPPORTED_MODELS.keys()) + ["Custom"]
 
     with gr.Row():
         lang = gr.Dropdown(choices=["en", "ru", "zh"], scale=1)
         model_name = gr.Dropdown(choices=available_models, scale=3)
         model_path = gr.Textbox(scale=3)
 
     with gr.Row():
         finetuning_type = gr.Dropdown(choices=METHODS, value="lora", scale=1)
         adapter_path = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=5)
         refresh_btn = gr.Button(scale=1)
 
-    with gr.Accordion(label="Advanced config", open=False) as advanced_tab:
+    with gr.Accordion(open=False) as advanced_tab:
         with gr.Row():
             quantization_bit = gr.Dropdown(choices=["none", "8", "4"], value="none")
             template = gr.Dropdown(choices=list(templates.keys()), value="default")
             rope_scaling = gr.Radio(choices=["none", "linear", "dynamic"], value="none")
             booster = gr.Radio(choices=["none", "flashattn", "unsloth"], value="none")
 
     model_name.change(list_adapters, [model_name, finetuning_type], [adapter_path], queue=False).then(
@@ -40,15 +40,15 @@
 
     finetuning_type.change(list_adapters, [model_name, finetuning_type], [adapter_path], queue=False).then(
         can_quantize, [finetuning_type], [quantization_bit], queue=False
     )
 
     refresh_btn.click(list_adapters, [model_name, finetuning_type], [adapter_path], queue=False)
 
-    return lang, dict(
+    return dict(
         lang=lang,
         model_name=model_name,
         model_path=model_path,
         finetuning_type=finetuning_type,
         adapter_path=adapter_path,
         refresh_btn=refresh_btn,
         advanced_tab=advanced_tab,
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/components/train.py` & `llmtuner-0.6.2/src/llmtuner/webui/components/train.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,37 +2,34 @@
 
 import gradio as gr
 from transformers.trainer_utils import SchedulerType
 
 from ...extras.constants import TRAINING_STAGES
 from ..common import DEFAULT_DATA_DIR, autoset_packing, list_adapters, list_dataset
 from ..components.data import create_preview_box
-from ..utils import gen_plot
 
 
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_train_tab(engine: "Engine") -> Dict[str, "Component"]:
     input_elems = engine.manager.get_base_elems()
     elem_dict = dict()
 
     with gr.Row():
         training_stage = gr.Dropdown(
-            choices=list(TRAINING_STAGES.keys()), value=list(TRAINING_STAGES.keys())[0], scale=2
+            choices=list(TRAINING_STAGES.keys()), value=list(TRAINING_STAGES.keys())[0], scale=1
         )
-        dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
-        dataset = gr.Dropdown(multiselect=True, scale=4)
+        dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=1)
+        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
-    dataset_dir.change(list_dataset, [dataset_dir, training_stage], [dataset], queue=False)
-
     input_elems.update({training_stage, dataset_dir, dataset})
     elem_dict.update(dict(training_stage=training_stage, dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
         learning_rate = gr.Textbox(value="5e-5")
         num_train_epochs = gr.Textbox(value="3.0")
         max_grad_norm = gr.Textbox(value="1.0")
@@ -64,41 +61,48 @@
             batch_size=batch_size,
             gradient_accumulation_steps=gradient_accumulation_steps,
             val_size=val_size,
             lr_scheduler_type=lr_scheduler_type,
         )
     )
 
-    with gr.Accordion(label="Extra config", open=False) as extra_tab:
+    with gr.Accordion(open=False) as extra_tab:
         with gr.Row():
             logging_steps = gr.Slider(value=5, minimum=5, maximum=1000, step=5)
             save_steps = gr.Slider(value=100, minimum=10, maximum=5000, step=10)
             warmup_steps = gr.Slider(value=0, minimum=0, maximum=5000, step=1)
             neftune_alpha = gr.Slider(value=0, minimum=0, maximum=10, step=0.1)
             optim = gr.Textbox(value="adamw_torch")
 
         with gr.Row():
-            resize_vocab = gr.Checkbox()
-            packing = gr.Checkbox()
-            upcast_layernorm = gr.Checkbox()
-            use_llama_pro = gr.Checkbox()
-            shift_attn = gr.Checkbox()
+            with gr.Column():
+                resize_vocab = gr.Checkbox()
+                packing = gr.Checkbox()
+
+            with gr.Column():
+                upcast_layernorm = gr.Checkbox()
+                use_llama_pro = gr.Checkbox()
+
+            with gr.Column():
+                shift_attn = gr.Checkbox()
+                report_to = gr.Checkbox()
 
     input_elems.update(
         {
             logging_steps,
             save_steps,
             warmup_steps,
             neftune_alpha,
             optim,
             resize_vocab,
             packing,
             upcast_layernorm,
             use_llama_pro,
             shift_attn,
+            report_to,
         }
     )
     elem_dict.update(
         dict(
             extra_tab=extra_tab,
             logging_steps=logging_steps,
             save_steps=save_steps,
@@ -106,82 +110,93 @@
             neftune_alpha=neftune_alpha,
             optim=optim,
             resize_vocab=resize_vocab,
             packing=packing,
             upcast_layernorm=upcast_layernorm,
             use_llama_pro=use_llama_pro,
             shift_attn=shift_attn,
+            report_to=report_to,
         )
     )
 
-    with gr.Accordion(label="Freeze config", open=False) as freeze_tab:
+    with gr.Accordion(open=False) as freeze_tab:
         with gr.Row():
-            num_layer_trainable = gr.Slider(value=3, minimum=1, maximum=128, step=1, scale=2)
-            name_module_trainable = gr.Textbox(value="all", scale=3)
+            num_layer_trainable = gr.Slider(value=3, minimum=1, maximum=128, step=1)
+            name_module_trainable = gr.Textbox(value="all")
 
     input_elems.update({num_layer_trainable, name_module_trainable})
     elem_dict.update(
         dict(
             freeze_tab=freeze_tab, num_layer_trainable=num_layer_trainable, name_module_trainable=name_module_trainable
         )
     )
 
-    with gr.Accordion(label="LoRA config", open=False) as lora_tab:
+    with gr.Accordion(open=False) as lora_tab:
         with gr.Row():
-            lora_rank = gr.Slider(value=8, minimum=1, maximum=1024, step=1, scale=1)
-            lora_alpha = gr.Slider(value=16, minimum=1, maximum=2048, step=1, scale=1)
-            lora_dropout = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01, scale=1)
-            lora_target = gr.Textbox(scale=2)
+            lora_rank = gr.Slider(value=8, minimum=1, maximum=1024, step=1)
+            lora_alpha = gr.Slider(value=16, minimum=1, maximum=2048, step=1)
+            lora_dropout = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
+            loraplus_lr_ratio = gr.Slider(value=0, minimum=0, maximum=64, step=0.01)
+            create_new_adapter = gr.Checkbox()
 
         with gr.Row():
-            use_rslora = gr.Checkbox(scale=1)
-            use_dora = gr.Checkbox(scale=1)
-            create_new_adapter = gr.Checkbox(scale=1)
+            with gr.Column(scale=1):
+                use_rslora = gr.Checkbox()
+                use_dora = gr.Checkbox()
+
+            lora_target = gr.Textbox(scale=2)
             additional_target = gr.Textbox(scale=2)
 
     input_elems.update(
-        {lora_rank, lora_alpha, lora_dropout, lora_target, use_rslora, use_dora, create_new_adapter, additional_target}
+        {
+            lora_rank,
+            lora_alpha,
+            lora_dropout,
+            loraplus_lr_ratio,
+            create_new_adapter,
+            use_rslora,
+            use_dora,
+            lora_target,
+            additional_target,
+        }
     )
     elem_dict.update(
         dict(
             lora_tab=lora_tab,
             lora_rank=lora_rank,
             lora_alpha=lora_alpha,
             lora_dropout=lora_dropout,
-            lora_target=lora_target,
+            loraplus_lr_ratio=loraplus_lr_ratio,
+            create_new_adapter=create_new_adapter,
             use_rslora=use_rslora,
             use_dora=use_dora,
-            create_new_adapter=create_new_adapter,
+            lora_target=lora_target,
             additional_target=additional_target,
         )
     )
 
-    with gr.Accordion(label="RLHF config", open=False) as rlhf_tab:
+    with gr.Accordion(open=False) as rlhf_tab:
         with gr.Row():
-            dpo_beta = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01, scale=1)
-            dpo_ftx = gr.Slider(value=0, minimum=0, maximum=10, step=0.01, scale=1)
-            reward_model = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=2)
-
-    training_stage.change(list_dataset, [dataset_dir, training_stage], [dataset], queue=False).then(
-        list_adapters,
-        [engine.manager.get_elem_by_name("top.model_name"), engine.manager.get_elem_by_name("top.finetuning_type")],
-        [reward_model],
-        queue=False,
-    ).then(autoset_packing, [training_stage], [packing], queue=False)
+            dpo_beta = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
+            dpo_ftx = gr.Slider(value=0, minimum=0, maximum=10, step=0.01)
+            orpo_beta = gr.Slider(value=0.1, minimum=0, maximum=1, step=0.01)
+            reward_model = gr.Dropdown(multiselect=True, allow_custom_value=True)
 
-    input_elems.update({dpo_beta, dpo_ftx, reward_model})
-    elem_dict.update(dict(rlhf_tab=rlhf_tab, dpo_beta=dpo_beta, dpo_ftx=dpo_ftx, reward_model=reward_model))
+    input_elems.update({dpo_beta, dpo_ftx, orpo_beta, reward_model})
+    elem_dict.update(
+        dict(rlhf_tab=rlhf_tab, dpo_beta=dpo_beta, dpo_ftx=dpo_ftx, orpo_beta=orpo_beta, reward_model=reward_model)
+    )
 
-    with gr.Accordion(label="GaLore config", open=False) as galore_tab:
+    with gr.Accordion(open=False) as galore_tab:
         with gr.Row():
-            use_galore = gr.Checkbox(scale=1)
-            galore_rank = gr.Slider(value=16, minimum=1, maximum=1024, step=1, scale=2)
-            galore_update_interval = gr.Slider(value=200, minimum=1, maximum=1024, step=1, scale=2)
-            galore_scale = gr.Slider(value=0.25, minimum=0, maximum=1, step=0.01, scale=2)
-            galore_target = gr.Textbox(value="mlp,attn", scale=3)
+            use_galore = gr.Checkbox()
+            galore_rank = gr.Slider(value=16, minimum=1, maximum=1024, step=1)
+            galore_update_interval = gr.Slider(value=200, minimum=1, maximum=1024, step=1)
+            galore_scale = gr.Slider(value=0.25, minimum=0, maximum=1, step=0.01)
+            galore_target = gr.Textbox(value="all")
 
     input_elems.update({use_galore, galore_rank, galore_update_interval, galore_scale, galore_target})
     elem_dict.update(
         dict(
             galore_tab=galore_tab,
             use_galore=use_galore,
             galore_rank=galore_rank,
@@ -189,58 +204,68 @@
             galore_scale=galore_scale,
             galore_target=galore_target,
         )
     )
 
     with gr.Row():
         cmd_preview_btn = gr.Button()
-        start_btn = gr.Button()
-        stop_btn = gr.Button()
+        arg_save_btn = gr.Button()
+        arg_load_btn = gr.Button()
+        start_btn = gr.Button(variant="primary")
+        stop_btn = gr.Button(variant="stop")
 
     with gr.Row():
         with gr.Column(scale=3):
             with gr.Row():
                 output_dir = gr.Textbox()
+                config_path = gr.Textbox()
 
             with gr.Row():
                 resume_btn = gr.Checkbox(visible=False, interactive=False)
                 process_bar = gr.Slider(visible=False, interactive=False)
 
-            with gr.Box():
+            with gr.Row():
                 output_box = gr.Markdown()
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot()
 
-    input_elems.add(output_dir)
-    output_elems = [output_box, process_bar]
-
-    cmd_preview_btn.click(engine.runner.preview_train, input_elems, output_elems)
-    start_btn.click(engine.runner.run_train, input_elems, output_elems)
-    stop_btn.click(engine.runner.set_abort, queue=False)
-    resume_btn.change(engine.runner.monitor, outputs=output_elems)
-
     elem_dict.update(
         dict(
             cmd_preview_btn=cmd_preview_btn,
+            arg_save_btn=arg_save_btn,
+            arg_load_btn=arg_load_btn,
             start_btn=start_btn,
             stop_btn=stop_btn,
             output_dir=output_dir,
+            config_path=config_path,
             resume_btn=resume_btn,
             process_bar=process_bar,
             output_box=output_box,
             loss_viewer=loss_viewer,
         )
     )
 
-    output_box.change(
-        gen_plot,
-        [
-            engine.manager.get_elem_by_name("top.model_name"),
-            engine.manager.get_elem_by_name("top.finetuning_type"),
-            output_dir,
-        ],
-        loss_viewer,
-        queue=False,
+    input_elems.update({output_dir, config_path})
+    output_elems = [output_box, process_bar, loss_viewer]
+
+    cmd_preview_btn.click(engine.runner.preview_train, input_elems, output_elems, concurrency_limit=None)
+    arg_save_btn.click(engine.runner.save_args, input_elems, output_elems, concurrency_limit=None)
+    arg_load_btn.click(
+        engine.runner.load_args,
+        [engine.manager.get_elem_by_id("top.lang"), config_path],
+        list(input_elems) + [output_box],
+        concurrency_limit=None,
     )
+    start_btn.click(engine.runner.run_train, input_elems, output_elems)
+    stop_btn.click(engine.runner.set_abort)
+    resume_btn.change(engine.runner.monitor, outputs=output_elems, concurrency_limit=None)
+
+    dataset_dir.change(list_dataset, [dataset_dir, training_stage], [dataset], queue=False)
+    training_stage.change(list_dataset, [dataset_dir, training_stage], [dataset], queue=False).then(
+        list_adapters,
+        [engine.manager.get_elem_by_id("top.model_name"), engine.manager.get_elem_by_id("top.finetuning_type")],
+        [reward_model],
+        queue=False,
+    ).then(autoset_packing, [training_stage], [packing], queue=False)
 
     return elem_dict
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/css.py` & `llmtuner-0.6.2/src/llmtuner/webui/css.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/engine.py` & `llmtuner-0.6.2/src/llmtuner/webui/engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Any, Dict, Generator
 
-import gradio as gr
 from gradio.components import Component  # cannot use TYPE_CHECKING here
 
 from .chatter import WebChatModel
 from .common import get_model_path, list_dataset, load_config
 from .locales import LOCALES
 from .manager import Manager
 from .runner import Runner
@@ -15,48 +14,50 @@
     def __init__(self, demo_mode: bool = False, pure_chat: bool = False) -> None:
         self.demo_mode = demo_mode
         self.pure_chat = pure_chat
         self.manager = Manager()
         self.runner = Runner(self.manager, demo_mode)
         self.chatter = WebChatModel(self.manager, demo_mode, lazy_init=(not pure_chat))
 
-    def _form_dict(self, resume_dict: Dict[str, Dict[str, Any]]):
-        return {self.manager.get_elem_by_name(k): gr.update(**v) for k, v in resume_dict.items()}
+    def _update_component(self, input_dict: Dict[str, Dict[str, Any]]) -> Dict["Component", "Component"]:
+        r"""
+        Gets the dict to update the components.
+        """
+        output_dict: Dict["Component", "Component"] = {}
+        for elem_id, elem_attr in input_dict.items():
+            elem = self.manager.get_elem_by_id(elem_id)
+            output_dict[elem] = elem.__class__(**elem_attr)
 
-    def resume(self) -> Generator[Dict[Component, Dict[str, Any]], None, None]:
+        return output_dict
+
+    def resume(self) -> Generator[Dict[Component, Component], None, None]:
         user_config = load_config() if not self.demo_mode else {}
         lang = user_config.get("lang", None) or "en"
 
         init_dict = {"top.lang": {"value": lang}, "infer.chat_box": {"visible": self.chatter.loaded}}
 
         if not self.pure_chat:
-            init_dict["train.dataset"] = {"choices": list_dataset()["choices"]}
-            init_dict["eval.dataset"] = {"choices": list_dataset()["choices"]}
+            init_dict["train.dataset"] = {"choices": list_dataset().choices}
+            init_dict["eval.dataset"] = {"choices": list_dataset().choices}
+            init_dict["train.output_dir"] = {"value": "train_{}".format(get_time())}
+            init_dict["train.config_path"] = {"value": "{}.json".format(get_time())}
+            init_dict["eval.output_dir"] = {"value": "eval_{}".format(get_time())}
 
             if user_config.get("last_model", None):
                 init_dict["top.model_name"] = {"value": user_config["last_model"]}
                 init_dict["top.model_path"] = {"value": get_model_path(user_config["last_model"])}
 
-        yield self._form_dict(init_dict)
+        yield self._update_component(init_dict)
 
-        if not self.pure_chat:
-            if self.runner.alive and not self.demo_mode:
-                yield {elem: gr.update(value=value) for elem, value in self.runner.running_data.items()}
-                if self.runner.do_train:
-                    yield self._form_dict({"train.resume_btn": {"value": True}})
-                else:
-                    yield self._form_dict({"eval.resume_btn": {"value": True}})
+        if self.runner.alive and not self.demo_mode and not self.pure_chat:
+            yield {elem: elem.__class__(value=value) for elem, value in self.runner.running_data.items()}
+            if self.runner.do_train:
+                yield self._update_component({"train.resume_btn": {"value": True}})
             else:
-                yield self._form_dict(
-                    {
-                        "train.output_dir": {"value": "train_" + get_time()},
-                        "eval.output_dir": {"value": "eval_" + get_time()},
-                    }
-                )
+                yield self._update_component({"eval.resume_btn": {"value": True}})
 
-    def change_lang(self, lang: str) -> Dict[Component, Dict[str, Any]]:
+    def change_lang(self, lang: str) -> Dict[Component, Component]:
         return {
-            component: gr.update(**LOCALES[name][lang])
-            for elems in self.manager.all_elems.values()
-            for name, component in elems.items()
-            if name in LOCALES
+            elem: elem.__class__(**LOCALES[elem_name][lang])
+            for elem_name, elem in self.manager.get_elem_iter()
+            if elem_name in LOCALES
         }
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/locales.py` & `llmtuner-0.6.2/src/llmtuner/webui/locales.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,14 +532,28 @@
             "info": "Использовать сдвиг внимания на короткие дистанции предложенный LongLoRA.",
         },
         "zh": {
             "label": "使用 S^2 Attention",
             "info": "使用 LongLoRA 提出的 shift short attention。",
         },
     },
+    "report_to": {
+        "en": {
+            "label": "Enable external logger",
+            "info": "Use TensorBoard or wandb to log experiment.",
+        },
+        "ru": {
+            "label": "Включить внешний регистратор",
+            "info": "Использовать TensorBoard или wandb для ведения журнала экспериментов.",
+        },
+        "zh": {
+            "label": "启用外部记录面板",
+            "info": "使用 TensorBoard 或 wandb 记录实验。",
+        },
+    },
     "freeze_tab": {
         "en": {
             "label": "Freeze tuning configurations",
         },
         "ru": {
             "label": "конфигурации для настройки заморозки",
         },
@@ -624,26 +638,40 @@
             "info": "Вероятность отсева весов LoRA.",
         },
         "zh": {
             "label": "LoRA 随机丢弃",
             "info": "LoRA 权重随机丢弃的概率。",
         },
     },
-    "lora_target": {
+    "loraplus_lr_ratio": {
         "en": {
-            "label": "LoRA modules (optional)",
-            "info": "Name(s) of modules to apply LoRA. Use commas to separate multiple modules.",
+            "label": "LoRA+ LR ratio",
+            "info": "The LR ratio of the B matrices in LoRA.",
         },
         "ru": {
-            "label": "Модули LoRA (опционально)",
-            "info": "Имена модулей для применения LoRA. Используйте запятые для разделения нескольких модулей.",
+            "label": "LoRA+ LR коэффициент",
+            "info": "Коэффициент LR матриц B в LoRA.",
         },
         "zh": {
-            "label": "LoRA 作用模块（非必填）",
-            "info": "应用 LoRA 的模块名称。使用英文逗号分隔多个名称。",
+            "label": "LoRA+ 学习率比例",
+            "info": "LoRA+ 中 B 矩阵的学习率倍数。",
+        },
+    },
+    "create_new_adapter": {
+        "en": {
+            "label": "Create new adapter",
+            "info": "Create a new adapter with randomly initialized weight upon the existing one.",
+        },
+        "ru": {
+            "label": "Создать новый адаптер",
+            "info": "Создать новый адаптер с случайной инициализацией веса на основе существующего.",
+        },
+        "zh": {
+            "label": "新建适配器",
+            "info": "在现有的适配器上创建一个随机初始化后的新适配器。",
         },
     },
     "use_rslora": {
         "en": {
             "label": "Use rslora",
             "info": "Use the rank stabilization scaling factor for LoRA layer.",
         },
@@ -666,26 +694,26 @@
             "info": "Используйте LoRA с декомпозицией весов.",
         },
         "zh": {
             "label": "使用 DoRA",
             "info": "使用权重分解的 LoRA。",
         },
     },
-    "create_new_adapter": {
+    "lora_target": {
         "en": {
-            "label": "Create new adapter",
-            "info": "Create a new adapter with randomly initialized weight upon the existing one.",
+            "label": "LoRA modules (optional)",
+            "info": "Name(s) of modules to apply LoRA. Use commas to separate multiple modules.",
         },
         "ru": {
-            "label": "Создать новый адаптер",
-            "info": "Создать новый адаптер с случайной инициализацией веса на основе существующего.",
+            "label": "Модули LoRA (опционально)",
+            "info": "Имена модулей для применения LoRA. Используйте запятые для разделения нескольких модулей.",
         },
         "zh": {
-            "label": "新建适配器",
-            "info": "在现有的适配器上创建一个随机初始化后的新适配器。",
+            "label": "LoRA 作用模块（非必填）",
+            "info": "应用 LoRA 的模块名称。使用英文逗号分隔多个名称。",
         },
     },
     "additional_target": {
         "en": {
             "label": "Additional modules (optional)",
             "info": (
                 "Name(s) of modules apart from LoRA layers to be set as trainable. "
@@ -739,14 +767,28 @@
             "info": "Вес функции потерь SFT в DPO-ftx.",
         },
         "zh": {
             "label": "DPO-ftx 权重",
             "info": "DPO-ftx 中 SFT 损失的权重大小。",
         },
     },
+    "orpo_beta": {
+        "en": {
+            "label": "ORPO beta",
+            "info": "Value of the beta parameter in the ORPO loss.",
+        },
+        "ru": {
+            "label": "ORPO бета",
+            "info": "Значение параметра бета в функции потерь ORPO.",
+        },
+        "zh": {
+            "label": "ORPO beta 参数",
+            "info": "ORPO 损失函数中 beta 超参数大小。",
+        },
+    },
     "reward_model": {
         "en": {
             "label": "Reward model",
             "info": "Adapter of the reward model for PPO training.",
         },
         "ru": {
             "label": "Модель вознаграждения",
@@ -845,14 +887,36 @@
         "ru": {
             "value": "Просмотр команды",
         },
         "zh": {
             "value": "预览命令",
         },
     },
+    "arg_save_btn": {
+        "en": {
+            "value": "Save arguments",
+        },
+        "ru": {
+            "value": "Сохранить аргументы",
+        },
+        "zh": {
+            "value": "保存训练参数",
+        },
+    },
+    "arg_load_btn": {
+        "en": {
+            "value": "Load arguments",
+        },
+        "ru": {
+            "value": "Загрузить аргументы",
+        },
+        "zh": {
+            "value": "载入训练参数",
+        },
+    },
     "start_btn": {
         "en": {
             "value": "Start",
         },
         "ru": {
             "value": "Начать",
         },
@@ -881,14 +945,28 @@
             "info": "Каталог для сохранения результатов.",
         },
         "zh": {
             "label": "输出目录",
             "info": "保存结果的路径。",
         },
     },
+    "config_path": {
+        "en": {
+            "label": "Config path",
+            "info": "Path to config saving arguments.",
+        },
+        "ru": {
+            "label": "Путь к конфигурации",
+            "info": "Путь для сохранения аргументов конфигурации.",
+        },
+        "zh": {
+            "label": "配置路径",
+            "info": "保存训练参数的配置文件路径。",
+        },
+    },
     "output_box": {
         "en": {
             "value": "Ready.",
         },
         "ru": {
             "value": "Готово.",
         },
@@ -1232,14 +1310,19 @@
         "zh": "工具名称未找到。",
     },
     "err_json_schema": {
         "en": "Invalid JSON schema.",
         "ru": "Неверная схема JSON.",
         "zh": "Json 格式错误。",
     },
+    "err_config_not_found": {
+        "en": "Config file is not found.",
+        "ru": "Файл конфигурации не найден.",
+        "zh": "未找到配置文件。",
+    },
     "warn_no_cuda": {
         "en": "CUDA environment was not detected.",
         "ru": "Среда CUDA не обнаружена.",
         "zh": "未检测到 CUDA 环境。",
     },
     "info_aborting": {
         "en": "Aborted, wait for terminating...",
@@ -1252,14 +1335,24 @@
         "zh": "准备就绪。",
     },
     "info_finished": {
         "en": "Finished.",
         "ru": "Завершено.",
         "zh": "训练完毕。",
     },
+    "info_config_saved": {
+        "en": "Arguments have been saved at: ",
+        "ru": "Аргументы были сохранены по адресу: ",
+        "zh": "训练参数已保存至：",
+    },
+    "info_config_loaded": {
+        "en": "Arguments have been restored.",
+        "ru": "Аргументы были восстановлены.",
+        "zh": "训练参数已载入。",
+    },
     "info_loading": {
         "en": "Loading model...",
         "ru": "Загрузка модели...",
         "zh": "加载中……",
     },
     "info_unloading": {
         "en": "Unloading model...",
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/runner.py` & `llmtuner-0.6.2/src/llmtuner/webui/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import logging
 import os
 import time
 from threading import Thread
-from typing import TYPE_CHECKING, Any, Dict, Generator, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Generator
 
 import gradio as gr
 import transformers
 from gradio.components import Component  # cannot use TYPE_CHECKING here
 from transformers.trainer import TRAINING_ARGS_NAME
 from transformers.utils import is_torch_cuda_available
 
 from ..extras.callbacks import LogCallback
 from ..extras.constants import TRAINING_STAGES
 from ..extras.logging import LoggerHandler
 from ..extras.misc import get_device_count, torch_gc
 from ..train import run_exp
-from .common import get_module, get_save_dir, load_config
+from .common import get_module, get_save_dir, load_args, load_config, save_args
 from .locales import ALERTS
-from .utils import gen_cmd, get_eval_results, update_process_bar
+from .utils import gen_cmd, gen_plot, get_eval_results, update_process_bar
 
 
 if TYPE_CHECKING:
     from .manager import Manager
 
 
 class Runner:
@@ -44,16 +44,16 @@
     @property
     def alive(self) -> bool:
         return self.thread is not None
 
     def set_abort(self) -> None:
         self.aborted = True
 
-    def _initialize(self, data: Dict[Component, Any], do_train: bool, from_preview: bool) -> str:
-        get = lambda name: data[self.manager.get_elem_by_name(name)]
+    def _initialize(self, data: Dict["Component", Any], do_train: bool, from_preview: bool) -> str:
+        get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         lang, model_name, model_path = get("top.lang"), get("top.model_name"), get("top.model_path")
         dataset = get("train.dataset") if do_train else get("eval.dataset")
 
         if self.running:
             return ALERTS["err_conflict"][lang]
 
         if not model_name:
@@ -76,31 +76,29 @@
             reward_model = get("train.reward_model")
             if stage == "ppo" and not reward_model:
                 return ALERTS["err_no_reward_model"][lang]
 
         if not from_preview and not is_torch_cuda_available():
             gr.Warning(ALERTS["warn_no_cuda"][lang])
 
-        self.aborted = False
         self.logger_handler.reset()
         self.trainer_callback = LogCallback(self)
         return ""
 
     def _finalize(self, lang: str, finish_info: str) -> str:
+        finish_info = ALERTS["info_aborted"][lang] if self.aborted else finish_info
         self.thread = None
-        self.running_data = None
+        self.aborted = False
         self.running = False
+        self.running_data = None
         torch_gc()
-        if self.aborted:
-            return ALERTS["info_aborted"][lang]
-        else:
-            return finish_info
+        return finish_info
 
-    def _parse_train_args(self, data: Dict[Component, Any]) -> Dict[str, Any]:
-        get = lambda name: data[self.manager.get_elem_by_name(name)]
+    def _parse_train_args(self, data: Dict["Component", Any]) -> Dict[str, Any]:
+        get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         user_config = load_config()
 
         if get("top.adapter_path"):
             adapter_name_or_path = ",".join(
                 [
                     get_save_dir(get("top.model_name"), get("top.finetuning_type"), adapter)
                     for adapter in get("top.adapter_path")
@@ -137,53 +135,53 @@
             neftune_noise_alpha=get("train.neftune_alpha") or None,
             optim=get("train.optim"),
             resize_vocab=get("train.resize_vocab"),
             packing=get("train.packing"),
             upcast_layernorm=get("train.upcast_layernorm"),
             use_llama_pro=get("train.use_llama_pro"),
             shift_attn=get("train.shift_attn"),
+            report_to="all" if get("train.report_to") else "none",
             use_galore=get("train.use_galore"),
             output_dir=get_save_dir(get("top.model_name"), get("top.finetuning_type"), get("train.output_dir")),
             fp16=(get("train.compute_type") == "fp16"),
             bf16=(get("train.compute_type") == "bf16"),
             pure_bf16=(get("train.compute_type") == "pure_bf16"),
         )
         args["disable_tqdm"] = True
 
         if args["finetuning_type"] == "freeze":
-            args["num_layer_trainable"] = int(get("train.num_layer_trainable"))
+            args["num_layer_trainable"] = get("train.num_layer_trainable")
             args["name_module_trainable"] = get("train.name_module_trainable")
         elif args["finetuning_type"] == "lora":
-            args["lora_rank"] = int(get("train.lora_rank"))
-            args["lora_alpha"] = int(get("train.lora_alpha"))
-            args["lora_dropout"] = float(get("train.lora_dropout"))
-            args["lora_target"] = get("train.lora_target") or get_module(get("top.model_name"))
+            args["lora_rank"] = get("train.lora_rank")
+            args["lora_alpha"] = get("train.lora_alpha")
+            args["lora_dropout"] = get("train.lora_dropout")
+            args["loraplus_lr_ratio"] = get("train.loraplus_lr_ratio") or None
+            args["create_new_adapter"] = get("train.create_new_adapter")
             args["use_rslora"] = get("train.use_rslora")
             args["use_dora"] = get("train.use_dora")
+            args["lora_target"] = get("train.lora_target") or get_module(get("top.model_name"))
             args["additional_target"] = get("train.additional_target") or None
-            if args["stage"] in ["rm", "ppo", "dpo"]:
-                args["create_new_adapter"] = args["quantization_bit"] is None
-            else:
-                args["create_new_adapter"] = get("train.create_new_adapter")
 
             if args["use_llama_pro"]:
-                args["num_layer_trainable"] = int(get("train.num_layer_trainable"))
+                args["num_layer_trainable"] = get("train.num_layer_trainable")
 
         if args["stage"] == "ppo":
             args["reward_model"] = ",".join(
                 [
                     get_save_dir(get("top.model_name"), get("top.finetuning_type"), adapter)
                     for adapter in get("train.reward_model")
                 ]
             )
             args["reward_model_type"] = "lora" if args["finetuning_type"] == "lora" else "full"
-
-        if args["stage"] == "dpo":
+        elif args["stage"] == "dpo":
             args["dpo_beta"] = get("train.dpo_beta")
             args["dpo_ftx"] = get("train.dpo_ftx")
+        elif args["stage"] == "orpo":
+            args["orpo_beta"] = get("train.orpo_beta")
 
         if get("train.val_size") > 1e-6 and args["stage"] != "ppo":
             args["val_size"] = get("train.val_size")
             args["evaluation_strategy"] = "steps"
             args["eval_steps"] = args["save_steps"]
             args["per_device_eval_batch_size"] = args["per_device_train_batch_size"]
             args["load_best_model_at_end"] = args["stage"] not in ["rm", "ppo"]
@@ -192,16 +190,16 @@
             args["galore_rank"] = get("train.galore_rank")
             args["galore_update_interval"] = get("train.galore_update_interval")
             args["galore_scale"] = get("train.galore_scale")
             args["galore_target"] = get("train.galore_target")
 
         return args
 
-    def _parse_eval_args(self, data: Dict[Component, Any]) -> Dict[str, Any]:
-        get = lambda name: data[self.manager.get_elem_by_name(name)]
+    def _parse_eval_args(self, data: Dict["Component", Any]) -> Dict[str, Any]:
+        get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         user_config = load_config()
 
         if get("top.adapter_path"):
             adapter_name_or_path = ",".join(
                 [
                     get_save_dir(get("top.model_name"), get("top.finetuning_type"), adapter)
                     for adapter in get("top.adapter_path")
@@ -228,80 +226,140 @@
             per_device_eval_batch_size=get("eval.batch_size"),
             predict_with_generate=True,
             max_new_tokens=get("eval.max_new_tokens"),
             top_p=get("eval.top_p"),
             temperature=get("eval.temperature"),
             output_dir=get_save_dir(get("top.model_name"), get("top.finetuning_type"), get("eval.output_dir")),
         )
+        args["disable_tqdm"] = True
 
         if get("eval.predict"):
             args["do_predict"] = True
         else:
             args["do_eval"] = True
 
         return args
 
-    def _preview(
-        self, data: Dict[Component, Any], do_train: bool
-    ) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def _preview(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict[Component, str], None, None]:
+        output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if do_train else "eval"))
         error = self._initialize(data, do_train, from_preview=True)
         if error:
             gr.Warning(error)
-            yield error, gr.update(visible=False)
+            yield {output_box: error}
         else:
             args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
-            yield gen_cmd(args), gr.update(visible=False)
+            yield {output_box: gen_cmd(args)}
 
-    def _launch(self, data: Dict[Component, Any], do_train: bool) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def _launch(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict[Component, Any], None, None]:
+        output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if do_train else "eval"))
         error = self._initialize(data, do_train, from_preview=False)
         if error:
             gr.Warning(error)
-            yield error, gr.update(visible=False)
+            yield {output_box: error}
         else:
             args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
             run_kwargs = dict(args=args, callbacks=[self.trainer_callback])
             self.do_train, self.running_data = do_train, data
             self.thread = Thread(target=run_exp, kwargs=run_kwargs)
             self.thread.start()
             yield from self.monitor()
 
-    def preview_train(self, data: Dict[Component, Any]) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def preview_train(self, data: Dict[Component, Any]) -> Generator[Dict[Component, str], None, None]:
         yield from self._preview(data, do_train=True)
 
-    def preview_eval(self, data: Dict[Component, Any]) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def preview_eval(self, data: Dict[Component, Any]) -> Generator[Dict[Component, str], None, None]:
         yield from self._preview(data, do_train=False)
 
-    def run_train(self, data: Dict[Component, Any]) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def run_train(self, data: Dict[Component, Any]) -> Generator[Dict[Component, Any], None, None]:
         yield from self._launch(data, do_train=True)
 
-    def run_eval(self, data: Dict[Component, Any]) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
+    def run_eval(self, data: Dict[Component, Any]) -> Generator[Dict[Component, Any], None, None]:
         yield from self._launch(data, do_train=False)
 
-    def monitor(self) -> Generator[Tuple[str, Dict[str, Any]], None, None]:
-        get = lambda name: self.running_data[self.manager.get_elem_by_name(name)]
+    def monitor(self) -> Generator[Dict[Component, Any], None, None]:
+        get = lambda elem_id: self.running_data[self.manager.get_elem_by_id(elem_id)]
+        self.aborted = False
         self.running = True
+
         lang = get("top.lang")
-        output_dir = get_save_dir(
-            get("top.model_name"),
-            get("top.finetuning_type"),
-            get("{}.output_dir".format("train" if self.do_train else "eval")),
-        )
+        model_name = get("top.model_name")
+        finetuning_type = get("top.finetuning_type")
+        output_dir = get("{}.output_dir".format("train" if self.do_train else "eval"))
+        output_path = get_save_dir(model_name, finetuning_type, output_dir)
+
+        output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if self.do_train else "eval"))
+        process_bar = self.manager.get_elem_by_id("{}.process_bar".format("train" if self.do_train else "eval"))
+        loss_viewer = self.manager.get_elem_by_id("train.loss_viewer") if self.do_train else None
 
-        while self.thread.is_alive():
-            time.sleep(2)
+        while self.thread is not None and self.thread.is_alive():
             if self.aborted:
-                yield ALERTS["info_aborting"][lang], gr.update(visible=False)
+                yield {
+                    output_box: ALERTS["info_aborting"][lang],
+                    process_bar: gr.Slider(visible=False),
+                }
             else:
-                yield self.logger_handler.log, update_process_bar(self.trainer_callback)
+                return_dict = {
+                    output_box: self.logger_handler.log,
+                    process_bar: update_process_bar(self.trainer_callback),
+                }
+                if self.do_train:
+                    plot = gen_plot(output_path)
+                    if plot is not None:
+                        return_dict[loss_viewer] = plot
+
+                yield return_dict
+
+            time.sleep(2)
 
         if self.do_train:
-            if os.path.exists(os.path.join(output_dir, TRAINING_ARGS_NAME)):
+            if os.path.exists(os.path.join(output_path, TRAINING_ARGS_NAME)):
                 finish_info = ALERTS["info_finished"][lang]
             else:
                 finish_info = ALERTS["err_failed"][lang]
         else:
-            if os.path.exists(os.path.join(output_dir, "all_results.json")):
-                finish_info = get_eval_results(os.path.join(output_dir, "all_results.json"))
+            if os.path.exists(os.path.join(output_path, "all_results.json")):
+                finish_info = get_eval_results(os.path.join(output_path, "all_results.json"))
             else:
                 finish_info = ALERTS["err_failed"][lang]
 
-        yield self._finalize(lang, finish_info), gr.update(visible=False)
+        return_dict = {
+            output_box: self._finalize(lang, finish_info),
+            process_bar: gr.Slider(visible=False),
+        }
+        if self.do_train:
+            plot = gen_plot(output_path)
+            if plot is not None:
+                return_dict[loss_viewer] = plot
+
+        yield return_dict
+
+    def save_args(self, data: Dict[Component, Any]) -> Dict[Component, str]:
+        output_box = self.manager.get_elem_by_id("train.output_box")
+        error = self._initialize(data, do_train=True, from_preview=True)
+        if error:
+            gr.Warning(error)
+            return {output_box: error}
+
+        config_dict: Dict[str, Any] = {}
+        lang = data[self.manager.get_elem_by_id("top.lang")]
+        config_path = data[self.manager.get_elem_by_id("train.config_path")]
+        skip_ids = ["top.lang", "top.model_path", "train.output_dir", "train.config_path"]
+        for elem, value in data.items():
+            elem_id = self.manager.get_id_by_elem(elem)
+            if elem_id not in skip_ids:
+                config_dict[elem_id] = value
+
+        save_path = save_args(config_path, config_dict)
+        return {output_box: ALERTS["info_config_saved"][lang] + save_path}
+
+    def load_args(self, lang: str, config_path: str) -> Dict[Component, Any]:
+        output_box = self.manager.get_elem_by_id("train.output_box")
+        config_dict = load_args(config_path)
+        if config_dict is None:
+            gr.Warning(ALERTS["err_config_not_found"][lang])
+            return {output_box: ALERTS["err_config_not_found"][lang]}
+
+        output_dict: Dict["Component", Any] = {output_box: ALERTS["info_config_loaded"][lang]}
+        for elem_id, value in config_dict.items():
+            output_dict[self.manager.get_elem_by_id(elem_id)] = value
+
+        return output_dict
```

### Comparing `llmtuner-0.6.1/src/llmtuner/webui/utils.py` & `llmtuner-0.6.2/src/llmtuner/webui/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 import json
 import os
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, Optional
 
 import gradio as gr
 
 from ..extras.packages import is_matplotlib_available
 from ..extras.ploting import smooth
-from .common import get_save_dir
 from .locales import ALERTS
 
 
 if TYPE_CHECKING:
     from ..extras.callbacks import LogCallback
 
 if is_matplotlib_available():
     import matplotlib.figure
     import matplotlib.pyplot as plt
 
 
-def update_process_bar(callback: "LogCallback") -> Dict[str, Any]:
+def update_process_bar(callback: "LogCallback") -> "gr.Slider":
     if not callback.max_steps:
-        return gr.update(visible=False)
+        return gr.Slider(visible=False)
 
     percentage = round(100 * callback.cur_steps / callback.max_steps, 0) if callback.max_steps != 0 else 100.0
     label = "Running {:d}/{:d}: {} < {}".format(
         callback.cur_steps, callback.max_steps, callback.elapsed_time, callback.remaining_time
     )
-    return gr.update(label=label, value=percentage, visible=True)
+    return gr.Slider(label=label, value=percentage, visible=True)
 
 
 def get_time() -> str:
-    return datetime.now().strftime("%Y-%m-%d-%H-%M-%S")
+    return datetime.now().strftime(r"%Y-%m-%d-%H-%M-%S")
 
 
-def can_quantize(finetuning_type: str) -> Dict[str, Any]:
+def can_quantize(finetuning_type: str) -> "gr.Dropdown":
     if finetuning_type != "lora":
-        return gr.update(value="None", interactive=False)
+        return gr.Dropdown(value="none", interactive=False)
     else:
-        return gr.update(interactive=True)
+        return gr.Dropdown(interactive=True)
 
 
 def check_json_schema(text: str, lang: str) -> None:
     try:
         tools = json.loads(text)
         if tools:
             assert isinstance(tools, list)
             for tool in tools:
                 if "name" not in tool:
-                    raise ValueError("Name not found.")
-    except ValueError:
+                    raise NotImplementedError("Name not found.")
+    except NotImplementedError:
         gr.Warning(ALERTS["err_tool_name"][lang])
     except Exception:
         gr.Warning(ALERTS["err_json_schema"][lang])
 
 
 def gen_cmd(args: Dict[str, Any]) -> str:
     args.pop("disable_tqdm", None)
@@ -70,35 +69,33 @@
 
 def get_eval_results(path: os.PathLike) -> str:
     with open(path, "r", encoding="utf-8") as f:
         result = json.dumps(json.load(f), indent=4)
     return "```json\n{}\n```\n".format(result)
 
 
-def gen_plot(base_model: str, finetuning_type: str, output_dir: str) -> "matplotlib.figure.Figure":
-    if not base_model:
-        return
-    log_file = get_save_dir(base_model, finetuning_type, output_dir, "trainer_log.jsonl")
-    if not os.path.isfile(log_file):
+def gen_plot(output_path: str) -> Optional["matplotlib.figure.Figure"]:
+    log_file = os.path.join(output_path, "trainer_log.jsonl")
+    if not os.path.isfile(log_file) or not is_matplotlib_available():
         return
 
     plt.close("all")
     plt.switch_backend("agg")
     fig = plt.figure()
     ax = fig.add_subplot(111)
     steps, losses = [], []
     with open(log_file, "r", encoding="utf-8") as f:
         for line in f:
-            log_info = json.loads(line)
+            log_info: Dict[str, Any] = json.loads(line)
             if log_info.get("loss", None):
                 steps.append(log_info["current_steps"])
                 losses.append(log_info["loss"])
 
     if len(losses) == 0:
-        return None
+        return
 
     ax.plot(steps, losses, color="#1f77b4", alpha=0.4, label="original")
     ax.plot(steps, smooth(losses), color="#1f77b4", label="smoothed")
     ax.legend()
     ax.set_xlabel("step")
     ax.set_ylabel("loss")
     return fig
```

### Comparing `llmtuner-0.6.1/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.6.2/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/llmtuner/chat/__init__.py
 src/llmtuner/chat/base_engine.py
 src/llmtuner/chat/chat_model.py
 src/llmtuner/chat/hf_engine.py
 src/llmtuner/chat/vllm_engine.py
 src/llmtuner/data/__init__.py
 src/llmtuner/data/aligner.py
+src/llmtuner/data/collator.py
 src/llmtuner/data/formatter.py
 src/llmtuner/data/loader.py
 src/llmtuner/data/parser.py
 src/llmtuner/data/preprocess.py
 src/llmtuner/data/template.py
 src/llmtuner/data/utils.py
 src/llmtuner/eval/__init__.py
@@ -32,15 +33,14 @@
 src/llmtuner/extras/constants.py
 src/llmtuner/extras/logging.py
 src/llmtuner/extras/misc.py
 src/llmtuner/extras/packages.py
 src/llmtuner/extras/ploting.py
 src/llmtuner/extras/patches/__init__.py
 src/llmtuner/extras/patches/llama_patch.py
-src/llmtuner/extras/patches/mixtral_patch.py
 src/llmtuner/hparams/__init__.py
 src/llmtuner/hparams/data_args.py
 src/llmtuner/hparams/evaluation_args.py
 src/llmtuner/hparams/finetuning_args.py
 src/llmtuner/hparams/generating_args.py
 src/llmtuner/hparams/model_args.py
 src/llmtuner/hparams/parser.py
@@ -49,26 +49,27 @@
 src/llmtuner/model/loader.py
 src/llmtuner/model/patcher.py
 src/llmtuner/model/utils.py
 src/llmtuner/train/__init__.py
 src/llmtuner/train/tuner.py
 src/llmtuner/train/utils.py
 src/llmtuner/train/dpo/__init__.py
-src/llmtuner/train/dpo/collator.py
 src/llmtuner/train/dpo/trainer.py
 src/llmtuner/train/dpo/workflow.py
+src/llmtuner/train/orpo/__init__.py
+src/llmtuner/train/orpo/trainer.py
+src/llmtuner/train/orpo/workflow.py
 src/llmtuner/train/ppo/__init__.py
 src/llmtuner/train/ppo/trainer.py
 src/llmtuner/train/ppo/utils.py
 src/llmtuner/train/ppo/workflow.py
 src/llmtuner/train/pt/__init__.py
 src/llmtuner/train/pt/trainer.py
 src/llmtuner/train/pt/workflow.py
 src/llmtuner/train/rm/__init__.py
-src/llmtuner/train/rm/collator.py
 src/llmtuner/train/rm/metric.py
 src/llmtuner/train/rm/trainer.py
 src/llmtuner/train/rm/workflow.py
 src/llmtuner/train/sft/__init__.py
 src/llmtuner/train/sft/metric.py
 src/llmtuner/train/sft/trainer.py
 src/llmtuner/train/sft/workflow.py
```

### Comparing `llmtuner-0.6.1/src/llmtuner.egg-info/requires.txt` & `llmtuner-0.6.2/src/llmtuner.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 torch>=1.13.1
 transformers>=4.37.2
 datasets>=2.14.3
 accelerate>=0.27.2
 peft>=0.10.0
 trl>=0.8.1
-gradio<4.0.0,>=3.38.0
+gradio<=4.21.0,>=4.0.0
 scipy
 einops
 sentencepiece
 protobuf
 uvicorn
 pydantic
 fastapi
 sse-starlette
 matplotlib
 fire
-galore-torch
 
 [aqlm]
 aqlm[gpu]>=1.1.0
 
 [awq]
 autoawq
 
 [bitsandbytes]
 bitsandbytes>=0.39.0
 
 [deepspeed]
-deepspeed
+deepspeed>=0.10.0
+
+[galore]
+galore-torch
 
 [gptq]
 optimum>=1.16.0
 auto-gptq>=0.5.0
 
 [metrics]
 nltk
 jieba
 rouge-chinese
 
+[modelscope]
+modelscope
+
 [quality]
 ruff
 
 [qwen]
 tiktoken
 transformers_stream_generator
```

### Comparing `llmtuner-0.6.1/tests/test_throughput.py` & `llmtuner-0.6.2/tests/test_throughput.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.1/tests/test_toolcall.py` & `llmtuner-0.6.2/tests/test_toolcall.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def calculate_gpa(grades: Sequence[str], hours: Sequence[int]) -> float:
     grade_to_score = {"A": 4, "B": 3, "C": 2}
     total_score, total_hour = 0, 0
     for grade, hour in zip(grades, hours):
         total_score += grade_to_score[grade] * hour
         total_hour += hour
-    return total_score / total_hour
+    return round(total_score / total_hour, 2)
 
 
 def main():
     client = OpenAI(
         api_key="0",
         base_url="http://localhost:{}/v1".format(os.environ.get("API_PORT", 8000)),
     )
@@ -41,21 +41,24 @@
         }
     ]
     tool_map = {"calculate_gpa": calculate_gpa}
 
     messages = []
     messages.append({"role": "user", "content": "My grades are A, A, B, and C. The credit hours are 3, 4, 3, and 2."})
     result = client.chat.completions.create(messages=messages, model="test", tools=tools)
+    if result.choices[0].message.tool_calls is None:
+        raise ValueError("Cannot retrieve function call from the response.")
+
+    messages.append(result.choices[0].message)
     tool_call = result.choices[0].message.tool_calls[0].function
+    print(tool_call)
+    # Function(arguments='{"grades": ["A", "A", "B", "C"], "hours": [3, 4, 3, 2]}', name='calculate_gpa')
     name, arguments = tool_call.name, json.loads(tool_call.arguments)
-    messages.append(
-        {"role": "function", "content": json.dumps({"name": name, "argument": arguments}, ensure_ascii=False)}
-    )
     tool_result = tool_map[name](**arguments)
     messages.append({"role": "tool", "content": json.dumps({"gpa": tool_result}, ensure_ascii=False)})
     result = client.chat.completions.create(messages=messages, model="test", tools=tools)
     print(result.choices[0].message.content)
-    # Based on your grades and credit hours, your calculated Grade Point Average (GPA) is 3.4166666666666665.
+    # Based on the grades and credit hours you provided, your Grade Point Average (GPA) is 3.42.
 
 
 if __name__ == "__main__":
     main()
```

