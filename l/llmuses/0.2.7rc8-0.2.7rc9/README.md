# Comparing `tmp/llmuses-0.2.7rc8.tar.gz` & `tmp/llmuses-0.2.7rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmuses-0.2.7rc8.tar", last modified: Wed Apr 10 07:35:06 2024, max compression
+gzip compressed data, was "llmuses-0.2.7rc9.tar", last modified: Wed Apr 10 14:36:34 2024, max compression
```

## Comparing `llmuses-0.2.7rc8.tar` & `llmuses-0.2.7rc9.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.305132 llmuses-0.2.7rc8/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 07:35:06.304745 llmuses-0.2.7rc8/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)    11285 2024-04-10 07:35:05.000000 llmuses-0.2.7rc8/README.md
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.230765 llmuses-0.2.7rc8/llmuses/
--rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.233787 llmuses-0.2.7rc8/llmuses/benchmarks/
--rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.235146 llmuses-0.2.7rc8/llmuses/benchmarks/arc/
--rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/ai2_arc.py
--rw-r--r--   0 jason      (501) staff       (20)     8983 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/arc/arc_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.236594 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/
--rw-r--r--   0 jason      (501) staff       (20)      300 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    10792 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/bbh_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.253681 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/
--rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
--rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
--rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
--rw-r--r--   0 jason      (501) staff       (20)     2155 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/benchmark.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.255445 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/
--rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    15844 2024-04-09 10:23:04.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_exam.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.257622 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/
--rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math.py
--rw-r--r--   0 jason      (501) staff       (20)    19079 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)    10091 2024-04-09 13:29:59.000000 llmuses-0.2.7rc8/llmuses/benchmarks/data_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.259332 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/
--rw-r--r--   0 jason      (501) staff       (20)      340 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     6087 2024-04-10 07:29:44.000000 llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/general_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.261947 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/
--rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k.py
--rw-r--r--   0 jason      (501) staff       (20)    13761 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.264678 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/
--rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag.py
--rw-r--r--   0 jason      (501) staff       (20)     8547 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.266946 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/
--rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval.py
--rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.269402 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/
--rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu.py
--rw-r--r--   0 jason      (501) staff       (20)    16393 2024-04-09 12:38:11.000000 llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.271353 llmuses-0.2.7rc8/llmuses/benchmarks/race/
--rw-r--r--   0 jason      (501) staff       (20)      331 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3835 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/race.py
--rw-r--r--   0 jason      (501) staff       (20)     9892 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/race/race_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.273146 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/
--rw-r--r--   0 jason      (501) staff       (20)      345 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3296 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa.py
--rw-r--r--   0 jason      (501) staff       (20)     7653 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.274581 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/
--rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa.py
--rw-r--r--   0 jason      (501) staff       (20)    14944 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3284 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cache.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.276501 llmuses-0.2.7rc8/llmuses/cli/
--rw-r--r--   0 jason      (501) staff       (20)       50 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)      404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/base.py
--rw-r--r--   0 jason      (501) staff       (20)      549 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/cli.py
--rw-r--r--   0 jason      (501) staff       (20)     3865 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/cli/start_server.py
--rw-r--r--   0 jason      (501) staff       (20)     6552 2024-04-09 13:25:19.000000 llmuses-0.2.7rc8/llmuses/config.py
--rw-r--r--   0 jason      (501) staff       (20)     2632 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/constants.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.277975 llmuses-0.2.7rc8/llmuses/evaluator/
--rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    28598 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/evaluator/evaluator.py
--rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/rating_eval.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.279020 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/evaluator/reviewer/auto_reviewer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.281610 llmuses-0.2.7rc8/llmuses/metrics/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.282563 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/
--rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
--rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/code_metric.py
--rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/metrics/math_accuracy.py
--rw-r--r--   0 jason      (501) staff       (20)    12545 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/metrics/metrics.py
--rw-r--r--   0 jason      (501) staff       (20)     4516 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/metrics/rouge_metric.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.285526 llmuses-0.2.7rc8/llmuses/models/
--rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.286906 llmuses-0.2.7rc8/llmuses/models/custom/
--rw-r--r--   0 jason      (501) staff       (20)      101 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/custom/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1380 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/custom/custom_model.py
--rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/models/dummy_chat_model.py
--rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/model.py
--rw-r--r--   0 jason      (501) staff       (20)    21702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/models/model_adapter.py
--rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/models/openai_model.py
--rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/models/template.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.291862 llmuses-0.2.7rc8/llmuses/perf/
--rw-r--r--   0 jason      (501) staff       (20)        0 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     1034 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/_logging.py
--rw-r--r--   0 jason      (501) staff       (20)     1080 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/dashscope_message.py
--rw-r--r--   0 jason      (501) staff       (20)     1057 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/generate_zhipu_token.py
--rw-r--r--   0 jason      (501) staff       (20)    29573 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/http_client.py
--rw-r--r--   0 jason      (501) staff       (20)     3685 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/monitor.py
--rw-r--r--   0 jason      (501) staff       (20)     1153 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/server_sent_event.py
--rw-r--r--   0 jason      (501) staff       (20)     1092 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/vllm_qwen_openai_completion.py
--rw-r--r--   0 jason      (501) staff       (20)     1043 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/perf/zhipu_message.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.292376 llmuses-0.2.7rc8/llmuses/preprocess/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/preprocess/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.293394 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/
--rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.293973 llmuses-0.2.7rc8/llmuses/registry/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/registry/__init__.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.299580 llmuses-0.2.7rc8/llmuses/registry/tasks/
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/arc.yaml
--rw-r--r--   0 jason      (501) staff       (20)      700 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/bbh.yaml
--rw-r--r--   0 jason      (501) staff       (20)      774 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/bbh_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/ceval.yaml
--rw-r--r--   0 jason      (501) staff       (20)      768 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/ceval_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)      806 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
--rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 13:25:19.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/general_qa.yaml
--rw-r--r--   0 jason      (501) staff       (20)      703 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/gsm8k.yaml
--rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu.yaml
--rw-r--r--   0 jason      (501) staff       (20)      777 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu_mini.yaml
--rw-r--r--   0 jason      (501) staff       (20)    14577 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/run.py
--rw-r--r--   0 jason      (501) staff       (20)     8511 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/run_arena.py
--rw-r--r--   0 jason      (501) staff       (20)     5996 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/run_ms.py
--rw-r--r--   0 jason      (501) staff       (20)     3227 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/summarizer.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.300935 llmuses-0.2.7rc8/llmuses/tools/
--rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/tools/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     3233 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/tools/combine_reports.py
--rw-r--r--   0 jason      (501) staff       (20)     3277 2024-04-01 07:18:15.000000 llmuses-0.2.7rc8/llmuses/tools/gen_mmlu_subject_mapping.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.304188 llmuses-0.2.7rc8/llmuses/utils/
--rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/__init__.py
--rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/arena_utils.py
--rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc8/llmuses/utils/completion_parsers.py
--rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc8/llmuses/utils/logger.py
--rw-r--r--   0 jason      (501) staff       (20)      138 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/utils/task_cfg_parser.py
--rw-r--r--   0 jason      (501) staff       (20)    11952 2024-04-09 03:19:53.000000 llmuses-0.2.7rc8/llmuses/utils/utils.py
--rw-r--r--   0 jason      (501) staff       (20)      121 2024-04-10 07:34:50.000000 llmuses-0.2.7rc8/llmuses/version.py
-drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 07:35:06.232517 llmuses-0.2.7rc8/llmuses.egg-info/
--rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/PKG-INFO
--rw-r--r--   0 jason      (501) staff       (20)     5315 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/SOURCES.txt
--rw-r--r--   0 jason      (501) staff       (20)        1 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/dependency_links.txt
--rw-r--r--   0 jason      (501) staff       (20)        8 2024-04-10 07:35:06.000000 llmuses-0.2.7rc8/llmuses.egg-info/top_level.txt
--rw-r--r--   0 jason      (501) staff       (20)       38 2024-04-10 07:35:06.305217 llmuses-0.2.7rc8/setup.cfg
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.950085 llmuses-0.2.7rc9/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 14:36:34.949613 llmuses-0.2.7rc9/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)    11285 2024-04-10 14:36:34.000000 llmuses-0.2.7rc9/README.md
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.753187 llmuses-0.2.7rc9/llmuses/
+-rw-r--r--   0 jason      (501) staff       (20)      106 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.756999 llmuses-0.2.7rc9/llmuses/benchmarks/
+-rw-r--r--   0 jason      (501) staff       (20)      158 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.758920 llmuses-0.2.7rc9/llmuses/benchmarks/arc/
+-rw-r--r--   0 jason      (501) staff       (20)      308 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/arc/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5608 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/arc/ai2_arc.py
+-rw-r--r--   0 jason      (501) staff       (20)     9221 2024-04-10 14:22:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/arc/arc_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.760011 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/
+-rw-r--r--   0 jason      (501) staff       (20)      300 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    10792 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/bbh_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.774609 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/
+-rwxr-xr-x   0 jason      (501) staff       (20)     1780 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3652 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1166 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3567 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4476 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     4830 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2504 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2120 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2146 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/navigate.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     1417 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2385 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2294 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3480 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     6140 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3113 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/snarks.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)      820 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     3022 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2603 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2944 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt
+-rwxr-xr-x   0 jason      (501) staff       (20)     2163 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt
+-rw-r--r--   0 jason      (501) staff       (20)     2155 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/benchmark.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.847815 llmuses-0.2.7rc9/llmuses/benchmarks/ceval/
+-rw-r--r--   0 jason      (501) staff       (20)      337 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/ceval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    15844 2024-04-09 10:23:04.000000 llmuses-0.2.7rc9/llmuses/benchmarks/ceval/ceval_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     5063 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/ceval/ceval_exam.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.850120 llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/
+-rw-r--r--   0 jason      (501) staff       (20)      387 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     2678 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/competition_math.py
+-rw-r--r--   0 jason      (501) staff       (20)    19079 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/competition_math_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)    10427 2024-04-10 14:22:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/data_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.851410 llmuses-0.2.7rc9/llmuses/benchmarks/general_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      340 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/general_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     6087 2024-04-10 07:29:44.000000 llmuses-0.2.7rc9/llmuses/benchmarks/general_qa/general_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.853227 llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/
+-rw-r--r--   0 jason      (501) staff       (20)      309 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4282 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/gsm8k.py
+-rw-r--r--   0 jason      (501) staff       (20)    13761 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/gsm8k_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.855087 llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/
+-rw-r--r--   0 jason      (501) staff       (20)      351 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     4690 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/hellaswag.py
+-rw-r--r--   0 jason      (501) staff       (20)     8547 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/hellaswag_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.857053 llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/
+-rw-r--r--   0 jason      (501) staff       (20)      329 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3482 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/humaneval.py
+-rw-r--r--   0 jason      (501) staff       (20)     1661 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/humaneval_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.859218 llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     5256 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/mmlu.py
+-rw-r--r--   0 jason      (501) staff       (20)    16393 2024-04-09 12:38:11.000000 llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/mmlu_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.861697 llmuses-0.2.7rc9/llmuses/benchmarks/race/
+-rw-r--r--   0 jason      (501) staff       (20)      331 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/race/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3835 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/race/race.py
+-rw-r--r--   0 jason      (501) staff       (20)     9892 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/race/race_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.863733 llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      345 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3296 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/trivia_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)     7653 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.865389 llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/
+-rw-r--r--   0 jason      (501) staff       (20)      361 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7017 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/truthful_qa.py
+-rw-r--r--   0 jason      (501) staff       (20)    14944 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3284 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/cache.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.868129 llmuses-0.2.7rc9/llmuses/cli/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/cli/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)      404 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/cli/base.py
+-rw-r--r--   0 jason      (501) staff       (20)      549 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/cli/cli.py
+-rw-r--r--   0 jason      (501) staff       (20)     3865 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/cli/start_server.py
+-rw-r--r--   0 jason      (501) staff       (20)     6737 2024-04-10 14:27:06.000000 llmuses-0.2.7rc9/llmuses/config.py
+-rw-r--r--   0 jason      (501) staff       (20)     2632 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/constants.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.869864 llmuses-0.2.7rc9/llmuses/evaluator/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/evaluator/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    28598 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/evaluator/evaluator.py
+-rw-r--r--   0 jason      (501) staff       (20)     5760 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/evaluator/rating_eval.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.870983 llmuses-0.2.7rc9/llmuses/evaluator/reviewer/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/evaluator/reviewer/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    17034 2024-03-18 05:46:13.000000 llmuses-0.2.7rc9/llmuses/evaluator/reviewer/auto_reviewer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.874096 llmuses-0.2.7rc9/llmuses/metrics/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/metrics/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.875398 llmuses-0.2.7rc9/llmuses/metrics/bundled_rouge_score/
+-rw-r--r--   0 jason      (501) staff       (20)      650 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/metrics/bundled_rouge_score/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)    11450 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/metrics/bundled_rouge_score/rouge_scorer.py
+-rw-r--r--   0 jason      (501) staff       (20)     3462 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/metrics/code_metric.py
+-rw-r--r--   0 jason      (501) staff       (20)     1986 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/metrics/math_accuracy.py
+-rw-r--r--   0 jason      (501) staff       (20)    12545 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/metrics/metrics.py
+-rw-r--r--   0 jason      (501) staff       (20)     4516 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/metrics/rouge_metric.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.924806 llmuses-0.2.7rc9/llmuses/models/
+-rw-r--r--   0 jason      (501) staff       (20)      141 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/models/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.926191 llmuses-0.2.7rc9/llmuses/models/custom/
+-rw-r--r--   0 jason      (501) staff       (20)      101 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/models/custom/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1380 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/models/custom/custom_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     1321 2024-03-18 05:46:13.000000 llmuses-0.2.7rc9/llmuses/models/dummy_chat_model.py
+-rw-r--r--   0 jason      (501) staff       (20)     3020 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/models/model.py
+-rw-r--r--   0 jason      (501) staff       (20)    21702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/models/model_adapter.py
+-rw-r--r--   0 jason      (501) staff       (20)     3448 2024-03-18 05:46:13.000000 llmuses-0.2.7rc9/llmuses/models/openai_model.py
+-rw-r--r--   0 jason      (501) staff       (20)    25273 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/models/template.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.931550 llmuses-0.2.7rc9/llmuses/perf/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     1034 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/_logging.py
+-rw-r--r--   0 jason      (501) staff       (20)     1080 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/dashscope_message.py
+-rw-r--r--   0 jason      (501) staff       (20)     1057 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/generate_zhipu_token.py
+-rw-r--r--   0 jason      (501) staff       (20)    29573 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/http_client.py
+-rw-r--r--   0 jason      (501) staff       (20)     3685 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/monitor.py
+-rw-r--r--   0 jason      (501) staff       (20)     1153 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/server_sent_event.py
+-rw-r--r--   0 jason      (501) staff       (20)     1092 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/vllm_qwen_openai_completion.py
+-rw-r--r--   0 jason      (501) staff       (20)     1043 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/perf/zhipu_message.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.932208 llmuses-0.2.7rc9/llmuses/preprocess/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/preprocess/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.933338 llmuses-0.2.7rc9/llmuses/preprocess/tokenizers/
+-rw-r--r--   0 jason      (501) staff       (20)        0 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/preprocess/tokenizers/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7810 2024-03-18 05:46:13.000000 llmuses-0.2.7rc9/llmuses/preprocess/tokenizers/gpt2_tokenizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.934010 llmuses-0.2.7rc9/llmuses/registry/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/registry/__init__.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.940859 llmuses-0.2.7rc9/llmuses/registry/tasks/
+-rw-r--r--   0 jason      (501) staff       (20)      862 2024-04-10 14:31:15.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/arc.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      700 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/bbh.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      774 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/bbh_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/ceval.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      768 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/ceval_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      806 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      702 2024-04-09 13:25:19.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/general_qa.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      703 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/gsm8k.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      701 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/mmlu.yaml
+-rw-r--r--   0 jason      (501) staff       (20)      777 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/registry/tasks/mmlu_mini.yaml
+-rw-r--r--   0 jason      (501) staff       (20)    14779 2024-04-10 14:22:53.000000 llmuses-0.2.7rc9/llmuses/run.py
+-rw-r--r--   0 jason      (501) staff       (20)     8511 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/run_arena.py
+-rw-r--r--   0 jason      (501) staff       (20)     5996 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/run_ms.py
+-rw-r--r--   0 jason      (501) staff       (20)     3227 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/summarizer.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.943771 llmuses-0.2.7rc9/llmuses/tools/
+-rw-r--r--   0 jason      (501) staff       (20)       50 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/tools/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     3233 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/tools/combine_reports.py
+-rw-r--r--   0 jason      (501) staff       (20)     3277 2024-04-01 07:18:15.000000 llmuses-0.2.7rc9/llmuses/tools/gen_mmlu_subject_mapping.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.948747 llmuses-0.2.7rc9/llmuses/utils/
+-rw-r--r--   0 jason      (501) staff       (20)       85 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/utils/__init__.py
+-rw-r--r--   0 jason      (501) staff       (20)     7668 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/utils/arena_utils.py
+-rw-r--r--   0 jason      (501) staff       (20)     2993 2024-03-18 05:46:13.000000 llmuses-0.2.7rc9/llmuses/utils/completion_parsers.py
+-rw-r--r--   0 jason      (501) staff       (20)     1855 2023-12-18 07:51:14.000000 llmuses-0.2.7rc9/llmuses/utils/logger.py
+-rw-r--r--   0 jason      (501) staff       (20)      138 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/utils/task_cfg_parser.py
+-rw-r--r--   0 jason      (501) staff       (20)    11952 2024-04-09 03:19:53.000000 llmuses-0.2.7rc9/llmuses/utils/utils.py
+-rw-r--r--   0 jason      (501) staff       (20)      121 2024-04-10 14:33:10.000000 llmuses-0.2.7rc9/llmuses/version.py
+drwxr-xr-x   0 jason      (501) staff       (20)        0 2024-04-10 14:36:34.755359 llmuses-0.2.7rc9/llmuses.egg-info/
+-rw-r--r--   0 jason      (501) staff       (20)    11944 2024-04-10 14:36:34.000000 llmuses-0.2.7rc9/llmuses.egg-info/PKG-INFO
+-rw-r--r--   0 jason      (501) staff       (20)     5315 2024-04-10 14:36:34.000000 llmuses-0.2.7rc9/llmuses.egg-info/SOURCES.txt
+-rw-r--r--   0 jason      (501) staff       (20)        1 2024-04-10 14:36:34.000000 llmuses-0.2.7rc9/llmuses.egg-info/dependency_links.txt
+-rw-r--r--   0 jason      (501) staff       (20)        8 2024-04-10 14:36:34.000000 llmuses-0.2.7rc9/llmuses.egg-info/top_level.txt
+-rw-r--r--   0 jason      (501) staff       (20)       38 2024-04-10 14:36:34.950184 llmuses-0.2.7rc9/setup.cfg
```

### Comparing `llmuses-0.2.7rc8/PKG-INFO` & `llmuses-0.2.7rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc8
+Version: 0.2.7rc9
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc8/README.md` & `llmuses-0.2.7rc9/README.md`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/arc/ai2_arc.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/arc/ai2_arc.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/arc/arc_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/arc/arc_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     def __init__(self,
                  subset_list: list = None,
                  metric_list: list = None,
                  few_shot_num: int = None,
                  train_split: str = 'train',
                  eval_split: str = 'test',
+                 prompt_template: str = '',
                  **kwargs):
 
         if subset_list is None:
             subset_list = SUBSET_LIST
 
         if metric_list is None:
             metric_list = [{'name': 'WeightedAverageAccuracy', 'object': weighted_mean}]
@@ -44,14 +45,15 @@
             logger.warning(f'few_shot_num should be 0 for ARC, but got {few_shot_num}. Use 0-shot by default.')
 
         super().__init__(subset_list=subset_list,
                          metric_list=metric_list,
                          few_shot_num=few_shot_num,
                          train_split=train_split,
                          eval_split=eval_split,
+                         prompt_template=prompt_template,
                          **kwargs)
 
     def load_from_disk(self, dataset_name_or_path, subset_list, work_dir, **kwargs) -> dict:
         """
         Load the dataset from local disk.
 
         dataset_name_or_path: str, the dataset id or path. e.g. 'arc'
@@ -109,17 +111,20 @@
                 'answerKey': 'B'
             }
 
         Returns:
             {'data': ['xxx'], 'multi_choices': ['A', 'B', 'C', 'D']}
         """
         few_shot_prompts = [self._generate_prompt(input_d=sample, include_answer=True) for sample in few_shot_list]
-        context: str = '\n'.join(few_shot_prompts) + '\n'
-        # context = f'The following are multiple choice questions, please output correct answer\n\n: {context}'
-        full_prompt: str = context.strip() + self._generate_prompt(input_d=input_d, include_answer=False)
+        context: str = '\n'.join(few_shot_prompts)
+
+        context = f'{self.prompt_template}\n{context}' if self.prompt_template else context
+
+        # context = f'The following are multiple choice questions, please output correct answer in the form of A or B or C or D, do not output explanation:\n {context}'
+        full_prompt: str = context + self._generate_prompt(input_d=input_d, include_answer=False)
 
         return {'data': [full_prompt], 'multi_choices': self.choices}
 
     def get_gold_answer(self, input_d: dict) -> str:
         # Get the gold choice
         return input_d.get('answerKey', '')
```

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/bbh_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/bbh_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/boolean_expressions.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/causal_judgement.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/date_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/disambiguation_qa.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/dyck_languages.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/formal_fallacies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/geometric_shapes.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/hyperbaton.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/logical_deduction_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/movie_recommendation.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/multistep_arithmetic_two.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/navigate.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/navigate.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/object_counting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/penguins_in_a_table.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/reasoning_about_colored_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/ruin_names.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/salient_translation_error_detection.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/snarks.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/snarks.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/sports_understanding.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/temporal_sequences.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_five_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_seven_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/tracking_shuffled_objects_three_objects.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/web_of_lies.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt` & `llmuses-0.2.7rc9/llmuses/benchmarks/bbh/cot_prompts/word_sorting.txt`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/benchmark.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/ceval/ceval_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/ceval/ceval_exam.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/ceval/ceval_exam.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/competition_math.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/competition_math/competition_math_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/competition_math/competition_math_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/data_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/data_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,32 @@
 
     def __init__(self,
                  subset_list: list,
                  metric_list: list,
                  few_shot_num: Optional[int] = 0,
                  train_split: Optional[str] = None,
                  eval_split: Optional[str] = None,
+                 prompt_template: str = '',
                  **kwargs):
         """
         Args:
             subset_list: list of subset names for the dataset.
             metric_list: list, the metric list to evaluate the model on specific benchmark.
             few_shot_num: int, number of few-shot examples. Default: 0
             train_split: str, usually for few-shot examples. e.g. 'train'
             eval_split: str, the target eval split name. e.g. 'test'
+            prompt_template: str, the prompt template for the benchmark,
+                e.g. for ARC, it is `The following are multiple choice questions, please output correct answer in the form of A or B or C or D, do not output explanation:`
         """
         self.subset_list = subset_list
         self.metric_list = metric_list
         self.few_shot_num = few_shot_num
         self.train_split = train_split
         self.eval_split = eval_split
+        self.prompt_template = prompt_template
         self.config_kwargs = kwargs
 
     def load(self,
              dataset_name_or_path: str,
              subset_list: list = None,
              work_dir: Optional[str] = DEFAULT_ROOT_CACHE_DIR,
              datasets_hub: str = 'ModelScope',
```

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/general_qa/general_qa_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/general_qa/general_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/gsm8k.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/gsm8k/gsm8k_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/gsm8k/gsm8k_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/hellaswag.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/hellaswag/hellaswag_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/hellaswag/hellaswag_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/humaneval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/humaneval/humaneval_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/humaneval/humaneval_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/mmlu.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/mmlu/mmlu_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/mmlu/mmlu_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/race/race.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/race/race.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/race/race_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/race/race_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/trivia_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/trivia_qa/trivia_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/truthful_qa.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py` & `llmuses-0.2.7rc9/llmuses/benchmarks/truthful_qa/truthful_qa_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/cache.py` & `llmuses-0.2.7rc9/llmuses/cache.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/cli/cli.py` & `llmuses-0.2.7rc9/llmuses/cli/cli.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/cli/start_server.py` & `llmuses-0.2.7rc9/llmuses/cli/start_server.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/config.py` & `llmuses-0.2.7rc9/llmuses/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,19 @@
 
         # Reuse the existing task config and update the datasets
         pattern_config = registry_tasks.get(data_pattern)
 
         custom_config = copy.deepcopy(pattern_config)
         custom_config.update({'datasets': [data_pattern]})
         custom_config.update({'dataset_hub': 'Local'})     # TODO: to support `ModelScope`
-        custom_config.update({'dataset_args': {data_pattern: {}}})
+        if 'dataset_args' in custom_config:
+            if data_pattern not in custom_config:
+                custom_config['dataset_args'].update({data_pattern: {}})
+        else:
+            custom_config.update({'dataset_args': {data_pattern: {}}})
 
         if dataset_dir is not None:
             custom_config['dataset_args'][data_pattern].update({'local_path': dataset_dir})
 
         if subset_list is not None:
             # custom_config['dataset_args'].get(data_pattern, {}).update({'subset_list': subset_list})
             custom_config['dataset_args'][data_pattern].update({'subset_list': subset_list})
```

### Comparing `llmuses-0.2.7rc8/llmuses/constants.py` & `llmuses-0.2.7rc9/llmuses/constants.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/evaluator/evaluator.py` & `llmuses-0.2.7rc9/llmuses/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/evaluator/rating_eval.py` & `llmuses-0.2.7rc9/llmuses/evaluator/rating_eval.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/evaluator/reviewer/auto_reviewer.py` & `llmuses-0.2.7rc9/llmuses/evaluator/reviewer/auto_reviewer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/__init__.py` & `llmuses-0.2.7rc9/llmuses/metrics/bundled_rouge_score/__init__.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/bundled_rouge_score/rouge_scorer.py` & `llmuses-0.2.7rc9/llmuses/metrics/bundled_rouge_score/rouge_scorer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/code_metric.py` & `llmuses-0.2.7rc9/llmuses/metrics/code_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/math_accuracy.py` & `llmuses-0.2.7rc9/llmuses/metrics/math_accuracy.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/metrics.py` & `llmuses-0.2.7rc9/llmuses/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/metrics/rouge_metric.py` & `llmuses-0.2.7rc9/llmuses/metrics/rouge_metric.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/custom/custom_model.py` & `llmuses-0.2.7rc9/llmuses/models/custom/custom_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/dummy_chat_model.py` & `llmuses-0.2.7rc9/llmuses/models/dummy_chat_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/model.py` & `llmuses-0.2.7rc9/llmuses/models/model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/model_adapter.py` & `llmuses-0.2.7rc9/llmuses/models/model_adapter.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/openai_model.py` & `llmuses-0.2.7rc9/llmuses/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/models/template.py` & `llmuses-0.2.7rc9/llmuses/models/template.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/_logging.py` & `llmuses-0.2.7rc9/llmuses/perf/_logging.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/dashscope_message.py` & `llmuses-0.2.7rc9/llmuses/perf/dashscope_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/generate_zhipu_token.py` & `llmuses-0.2.7rc9/llmuses/perf/generate_zhipu_token.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/http_client.py` & `llmuses-0.2.7rc9/llmuses/perf/http_client.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/monitor.py` & `llmuses-0.2.7rc9/llmuses/perf/monitor.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/server_sent_event.py` & `llmuses-0.2.7rc9/llmuses/perf/server_sent_event.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/vllm_qwen_openai_completion.py` & `llmuses-0.2.7rc9/llmuses/perf/vllm_qwen_openai_completion.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/perf/zhipu_message.py` & `llmuses-0.2.7rc9/llmuses/perf/zhipu_message.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/preprocess/tokenizers/gpt2_tokenizer.py` & `llmuses-0.2.7rc9/llmuses/preprocess/tokenizers/gpt2_tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/arc.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/bbh.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 #  eos_token_id: null
 #  pad_token_id: null
 dataset_args: {}
 dry_run: false
 model: null   # Note: to be implemented as CustomModel
 eval_type: custom
 datasets:
-  - arc
+  - bbh
 outputs: null    # structure: configs, logs, predictions, reviews, reports # TODO: need to parse
 use_cache: true
 stage: all
 dataset_hub: ModelScope    # `Local` or `ModelScope`
-limit: null
+limit: null
```

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/bbh.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/gsm8k.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 #  eos_token_id: null
 #  pad_token_id: null
 dataset_args: {}
 dry_run: false
 model: null   # Note: to be implemented as CustomModel
 eval_type: custom
 datasets:
-  - bbh
+  - gsm8k
 outputs: null    # structure: configs, logs, predictions, reviews, reports # TODO: need to parse
 use_cache: true
 stage: all
 dataset_hub: ModelScope    # `Local` or `ModelScope`
-limit: null
+limit: null
```

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/bbh_mini.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/bbh_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/ceval.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/ceval.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/ceval_mini.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/ceval_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/eval_qwen-7b-chat_v100.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/general_qa.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/general_qa.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/gsm8k.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/mmlu.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 #  eos_token_id: null
 #  pad_token_id: null
 dataset_args: {}
 dry_run: false
 model: null   # Note: to be implemented as CustomModel
 eval_type: custom
 datasets:
-  - gsm8k
+  - mmlu
 outputs: null    # structure: configs, logs, predictions, reviews, reports # TODO: need to parse
 use_cache: true
 stage: all
 dataset_hub: ModelScope    # `Local` or `ModelScope`
-limit: null
+limit: null
```

### Comparing `llmuses-0.2.7rc8/llmuses/registry/tasks/mmlu_mini.yaml` & `llmuses-0.2.7rc9/llmuses/registry/tasks/mmlu_mini.yaml`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/run.py` & `llmuses-0.2.7rc9/llmuses/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,19 +252,22 @@
                                            outputs_dir=outputs,
                                            is_custom_outputs_dir=False, )
         else:
             # TODO: CHECK dataset_args
             dataset_name_or_path: str = dataset_args.get(dataset_name, {}).get('local_path') or imported_modules[
                 'DATASET_ID']
 
+            in_prompt_template: str = dataset_args.get(dataset_name, {}).get('prompt_template', '')
+
             # Init data adapter
             few_shot_num: int = dataset_args.get(dataset_name, {}).get('few_shot_num', None)
             few_shot_random: bool = dataset_args.get(dataset_name, {}).get('few_shot_random', True)
             data_adapter = imported_modules['DataAdapterClass'](few_shot_num=few_shot_num,
-                                                                few_shot_random=few_shot_random)
+                                                                few_shot_random=few_shot_random,
+                                                                prompt_template=in_prompt_template,)
 
             in_subset_list: list = dataset_args.get(dataset_name, {})\
                 .get('subset_list', imported_modules['SUBSET_LIST'])
             logger.info(f'\n** Evaluating on subsets for {dataset_name}: {in_subset_list}\n')
 
             evaluator = Evaluator(
                 dataset_name_or_path=dataset_name_or_path,
```

### Comparing `llmuses-0.2.7rc8/llmuses/run_arena.py` & `llmuses-0.2.7rc9/llmuses/run_arena.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/run_ms.py` & `llmuses-0.2.7rc9/llmuses/run_ms.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/summarizer.py` & `llmuses-0.2.7rc9/llmuses/summarizer.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/tools/combine_reports.py` & `llmuses-0.2.7rc9/llmuses/tools/combine_reports.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/tools/gen_mmlu_subject_mapping.py` & `llmuses-0.2.7rc9/llmuses/tools/gen_mmlu_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/utils/arena_utils.py` & `llmuses-0.2.7rc9/llmuses/utils/arena_utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/utils/completion_parsers.py` & `llmuses-0.2.7rc9/llmuses/utils/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/utils/logger.py` & `llmuses-0.2.7rc9/llmuses/utils/logger.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses/utils/utils.py` & `llmuses-0.2.7rc9/llmuses/utils/utils.py`

 * *Files identical despite different names*

### Comparing `llmuses-0.2.7rc8/llmuses.egg-info/PKG-INFO` & `llmuses-0.2.7rc9/llmuses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmuses
-Version: 0.2.7rc8
+Version: 0.2.7rc9
 Summary: LLMs Evaluation Framework
 Home-page: 
 Author: ModelScope team
 Author-email: contact@modelscope.cn
 Keywords: python,llm,evaluation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `llmuses-0.2.7rc8/llmuses.egg-info/SOURCES.txt` & `llmuses-0.2.7rc9/llmuses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

