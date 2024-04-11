# Comparing `tmp/syntheseus-0.3.0.tar.gz` & `tmp/syntheseus-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntheseus-0.3.0.tar", last modified: Wed Dec 20 02:09:06 2023, max compression
+gzip compressed data, was "syntheseus-0.4.0.tar", last modified: Thu Apr 11 11:14:44 2024, max compression
```

## Comparing `syntheseus-0.3.0.tar` & `syntheseus-0.4.0.tar`

### file list

```diff
@@ -1,204 +1,203 @@
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.171556 syntheseus-0.3.0/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      513 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.coveragerc
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.147555 syntheseus-0.3.0/.github/
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/.github/azure_pipelines/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      528 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.github/azure_pipelines/code-security-analysis.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/.github/workflows/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      939 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.github/workflows/ci.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      723 2023-12-18 16:37:45.000000 syntheseus-0.3.0/.github/workflows/ci_integration.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      780 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.github/workflows/docs.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      477 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.gitignore
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1645 2023-12-15 17:07:59.000000 syntheseus-0.3.0/.pre-commit-config.yaml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4705 2023-12-20 01:50:34.000000 syntheseus-0.3.0/CHANGELOG.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      444 2023-12-15 17:07:59.000000 syntheseus-0.3.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1141 2023-12-15 17:07:59.000000 syntheseus-0.3.0/LICENSE
--rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6329 2023-12-20 02:09:06.171556 syntheseus-0.3.0/PKG-INFO
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3428 2023-12-19 14:07:36.000000 syntheseus-0.3.0/README.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2756 2023-12-15 17:07:59.000000 syntheseus-0.3.0/SECURITY.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      504 2023-12-15 17:07:59.000000 syntheseus-0.3.0/SUPPORT.md
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/docs/
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/docs/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2654 2023-12-15 17:07:59.000000 syntheseus-0.3.0/docs/cli/eval_single_step.md
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/docs/images/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    95644 2023-12-15 17:07:59.000000 syntheseus-0.3.0/docs/images/logo.png
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2023-12-15 17:07:59.000000 syntheseus-0.3.0/docs/images/logo.svg
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1148 2023-12-19 12:59:37.000000 syntheseus-0.3.0/docs/index.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2276 2023-12-15 17:07:59.000000 syntheseus-0.3.0/docs/installation.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2292 2023-12-15 17:07:59.000000 syntheseus-0.3.0/docs/single_step.md
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      130 2023-12-15 17:07:59.000000 syntheseus-0.3.0/environment.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      341 2023-12-18 14:47:14.000000 syntheseus-0.3.0/environment_full.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      930 2023-12-15 17:07:59.000000 syntheseus-0.3.0/mkdocs.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2619 2023-12-20 02:08:41.000000 syntheseus-0.3.0/pyproject.toml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       38 2023-12-20 02:09:06.171556 syntheseus-0.3.0/setup.cfg
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/syntheseus/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/cli/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    17410 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/cli/eval_single_step.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      722 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/cli/main.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15311 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/cli/search.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1247 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/cli/search_config.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/interface/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/interface/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1174 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/interface/bag.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4541 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/interface/models.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2767 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/interface/molecule.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      372 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/interface/typed_dict.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/py.typed
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/chem/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/chem/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1311 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/chem/utils.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/cli/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/data/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/data/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5585 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/data/dataset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3685 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/data/reaction_sample.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/environment_gln/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1321 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/environment_gln/Dockerfile
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      455 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/environment_gln/environment.yml
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      694 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1442 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5192 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/chemformer.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1141 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/config.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      500 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3229 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/gln.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5961 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/local_retro.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6034 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/megan.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6753 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/mhnreact.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4767 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/retro_knn.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10714 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/inference/root_aligned.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.155556 syntheseus-0.3.0/syntheseus/reaction_prediction/models/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/models/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2363 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/models/retro_knn.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2081 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/config.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2378 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/downloading.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2068 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/inference.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1618 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/metrics.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3819 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/misc.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1280 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/model_loading.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1843 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/parallel.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2146 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/reaction_prediction/utils/syntheseus_wrapper.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       95 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/algorithms/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15285 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/base.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/algorithms/best_first/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/best_first/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5166 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/best_first/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10080 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/best_first/retro_star.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2103 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/breadth_first.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/algorithms/mcts/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/mcts/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    12493 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/mcts/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      299 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/mcts/molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      895 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/mixins.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    18072 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/algorithms/pdvn.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/analysis/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/analysis/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10168 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/analysis/diversity.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9772 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/analysis/route_extraction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2622 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/analysis/solution_time.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1877 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/chem.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/graph/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8882 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/and_or.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4834 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/base_graph.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.159556 syntheseus-0.3.0/syntheseus/search/graph/message_passing/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      266 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/message_passing/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6413 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/message_passing/run.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      834 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/message_passing/update_functions.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7456 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3913 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/node.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2819 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/route.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6796 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/graph/standardization.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1894 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/mol_inventory.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/search/node_evaluation/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      102 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/node_evaluation/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6058 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/node_evaluation/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2206 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/node_evaluation/common.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/search/reaction_models/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      110 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/reaction_models/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5349 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/reaction_models/base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3745 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/reaction_models/toy.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/search/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       69 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/utils/misc.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6477 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/search/visualization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/interface/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/interface/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      556 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/interface/test_bag.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      920 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/interface/test_models.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      545 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/interface/test_molecule.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/chem/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/chem/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      561 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/chem/test_utils.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/cli/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/cli/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3722 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/cli/test_eval.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/data/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/data/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4545 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/data/test_dataset.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/inference/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/inference/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2265 2023-12-18 16:37:45.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/inference/test_models.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/utils/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/utils/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      573 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/utils/test_misc.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1463 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/reaction_prediction/utils/test_syntheseus_wrapper.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/search/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/__init__.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.163556 syntheseus-0.3.0/syntheseus/tests/search/algorithms/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    23252 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    12841 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_best_first.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10793 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_breadth_first.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13280 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_mcts.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15452 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_pdvn.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.167556 syntheseus-0.3.0/syntheseus/tests/search/analysis/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/analysis/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1691 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/analysis/conftest.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4029 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/analysis/test_diversity.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9974 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/analysis/test_route_extraction.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      109 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/analysis/test_solution_time.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    14956 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/conftest.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.167556 syntheseus-0.3.0/syntheseus/tests/search/graph/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7101 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_andor.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      541 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_base.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4587 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_message_passing.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5015 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_molset.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      285 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_route.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      776 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/graph/test_standardization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.167556 syntheseus-0.3.0/syntheseus/tests/search/node_evaluation/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/node_evaluation/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5848 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/node_evaluation/test_common.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6800 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/test_chem.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2314 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/test_mol_inventory.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6796 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/test_reaction_models.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2094 2023-12-15 17:07:59.000000 syntheseus-0.3.0/syntheseus/tests/search/test_visualization.py
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.167556 syntheseus-0.3.0/syntheseus.egg-info/
--rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6329 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/PKG-INFO
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6510 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/SOURCES.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        1 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/dependency_links.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       56 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/entry_points.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      469 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/requires.txt
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       11 2023-12-20 02:09:06.000000 syntheseus-0.3.0/syntheseus.egg-info/top_level.txt
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.151556 syntheseus-0.3.0/tutorials/
-drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-20 02:09:06.167556 syntheseus-0.3.0/tutorials/search/
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)   232161 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/1- end to end retrosynthesis with a toy model.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    41952 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/2a- advanced algorithms on PaRoutes.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8765 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/2b- PaRoutes in-depth analysis.ipynb
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/__init__.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5231 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/paroutes.py
--rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      475 2023-12-15 17:07:59.000000 syntheseus-0.3.0/tutorials/search/paroutes_setup.sh
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.921803 syntheseus-0.4.0/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      509 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.coveragerc
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.897803 syntheseus-0.4.0/.github/
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/.github/azure_pipelines/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      528 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/azure_pipelines/code-security-analysis.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/.github/workflows/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2618 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/workflows/ci.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      991 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.github/workflows/docs.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      701 2024-04-11 11:13:41.000000 syntheseus-0.4.0/.github/workflows/release.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      382 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.gitignore
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1643 2024-04-11 11:13:34.000000 syntheseus-0.4.0/.pre-commit-config.yaml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7228 2024-04-11 11:13:34.000000 syntheseus-0.4.0/CHANGELOG.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      444 2024-04-11 11:13:34.000000 syntheseus-0.4.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1141 2024-04-11 11:13:34.000000 syntheseus-0.4.0/LICENSE
+-rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-04-11 11:14:44.921803 syntheseus-0.4.0/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3747 2024-04-11 11:13:34.000000 syntheseus-0.4.0/README.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2756 2024-04-11 11:13:34.000000 syntheseus-0.4.0/SECURITY.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      504 2024-04-11 11:13:34.000000 syntheseus-0.4.0/SUPPORT.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.901803 syntheseus-0.4.0/docs/
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2662 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/cli/eval_single_step.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1579 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/cli/search.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/images/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    95644 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/images/logo.png
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/images/logo.svg
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1242 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/index.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3157 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/installation.md
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2381 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/single_step.md
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/docs/tutorials/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       65 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/.gitignore
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11918 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/custom_model.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    44305 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/paroutes_benchmark.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8296 2024-04-11 11:13:34.000000 syntheseus-0.4.0/docs/tutorials/quick_start.ipynb
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      130 2024-04-11 11:13:34.000000 syntheseus-0.4.0/environment.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      341 2024-04-11 11:13:34.000000 syntheseus-0.4.0/environment_full.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1290 2024-04-11 11:13:34.000000 syntheseus-0.4.0/mkdocs.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2794 2024-04-11 11:13:34.000000 syntheseus-0.4.0/pyproject.toml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       38 2024-04-11 11:14:44.921803 syntheseus-0.4.0/setup.cfg
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      430 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    17900 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/eval_single_step.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      714 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/main.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15167 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/search.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1247 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/cli/search_config.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/interface/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1174 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/bag.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7054 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/models.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3186 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/molecule.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2933 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/reaction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      372 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/interface/typed_dict.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/py.typed
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1192 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/chem/utils.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/cli/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.905803 syntheseus-0.4.0/syntheseus/reaction_prediction/data/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5378 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/dataset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2858 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/data/reaction_sample.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1321 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/Dockerfile
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      455 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/environment.yml
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      988 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1491 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6156 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/chemformer.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1198 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/config.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      563 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/default_checkpoint_links.yml
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3265 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/gln.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3862 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/graph2edits.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5742 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/local_retro.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7142 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/megan.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7138 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/mhnreact.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4882 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/retro_knn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11041 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/root_aligned.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3943 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/inference/toy_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/models/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/models/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2363 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/models/retro_knn.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2246 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/config.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2378 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/downloading.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3281 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/inference.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1618 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/metrics.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3968 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/misc.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1644 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/model_loading.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1855 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/parallel.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      737 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/reaction_prediction/utils/testing.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/search/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       95 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.909803 syntheseus-0.4.0/syntheseus/search/algorithms/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15847 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/base.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     8108 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    11974 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/best_first/retro_star.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2103 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/breadth_first.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    12737 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      299 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mcts/molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      895 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/mixins.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    18103 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/pdvn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2133 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/algorithms/random.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/analysis/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10226 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/diversity.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9772 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/route_extraction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2622 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/analysis/solution_time.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/graph/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9079 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/and_or.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4892 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/base_graph.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/graph/message_passing/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      266 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6413 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/run.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      834 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/message_passing/update_functions.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7558 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3984 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/node.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2897 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/route.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6861 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/graph/standardization.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1901 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/mol_inventory.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/node_evaluation/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      102 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6048 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2201 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/node_evaluation/common.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/search/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       69 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/utils/misc.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6477 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/search/visualization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/cli/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5562 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/test_cli.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6166 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/cli/test_eval_single_step.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      925 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/conftest.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/interface/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      556 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_bag.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5867 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_models.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4595 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_molecule.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     3146 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_reaction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1331 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/interface/test_toy_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.913803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      561 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/test_utils.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5288 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/test_dataset.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1773 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/inference/test_models.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      573 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/test_misc.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/__init__.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/algorithms/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    25001 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13331 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_best_first.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    10793 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_breadth_first.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    13280 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_mcts.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    15592 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_pdvn.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1703 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_random.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/analysis/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     1691 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/conftest.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4029 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_diversity.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     9974 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_route_extraction.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      109 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/analysis/test_solution_time.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)    14701 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/conftest.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/graph/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     7208 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_andor.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      541 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_base.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     4587 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_message_passing.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5132 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_molset.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      292 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_route.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      776 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/graph/test_standardization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/__init__.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     5848 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/test_common.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2321 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/test_mol_inventory.py
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     2094 2024-04-11 11:13:34.000000 syntheseus-0.4.0/syntheseus/tests/search/test_visualization.py
+drwxrwxr-x   0 krmaziar  (1001) krmaziar  (1002)        0 2024-04-11 11:14:44.917803 syntheseus-0.4.0/syntheseus.egg-info/
+-rw-r--r--   0 krmaziar  (1001) krmaziar  (1002)     6793 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/PKG-INFO
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)     6416 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/SOURCES.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)        1 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/dependency_links.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       56 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/entry_points.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)      562 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/requires.txt
+-rw-rw-r--   0 krmaziar  (1001) krmaziar  (1002)       11 2024-04-11 11:14:44.000000 syntheseus-0.4.0/syntheseus.egg-info/top_level.txt
```

### Comparing `syntheseus-0.3.0/.github/azure_pipelines/code-security-analysis.yml` & `syntheseus-0.4.0/.github/azure_pipelines/code-security-analysis.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/.github/workflows/ci_integration.yml` & `syntheseus-0.4.0/.github/workflows/docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-name: CI (integration tests)
+name: Docs
 
 on:
   push:
     branches: [ main ]
-  pull_request:
-    branches: [ main ]
+  workflow_call:
+    inputs:
+      versions:
+        required: true
+        type: string
   workflow_dispatch:
 
+permissions:
+  contents: write
+
 jobs:
-  build:
+  deploy:
     runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
-    name: build
     steps:
-    - uses: actions/checkout@v3
-    - uses: conda-incubator/setup-miniconda@v2
-      with:
-        mamba-version: "*"
-        channels: conda-forge,defaults
-        channel-priority: true
-        environment-file: environment_full.yml
-    - name: Install syntheseus with all single-step models
-      run: |
-        pip install .[all]
-    - name: Run single-step model tests
-      run: |
-        python -m pytest ./syntheseus/tests/reaction_prediction/inference/test_models.py
+      - uses: actions/checkout@v4
+      - name: Configure Git
+        run: |
+          git config user.name github-actions[bot]
+          git config user.email 41898282+github-actions[bot]@users.noreply.github.com
+          git fetch origin gh-pages --depth=1
+      - uses: actions/setup-python@v4
+        with:
+          python-version: 3.x
+      - run: echo "cache_id=$(date --utc '+%V')" >> $GITHUB_ENV
+      - uses: actions/cache@v3
+        with:
+          key: mkdocs-material-${{ env.cache_id }}
+          path: .cache
+          restore-keys: |
+            mkdocs-material-
+      - run: pip install mkdocs-material mkdocs-jupyter mike
+      - run: mike deploy --push --update-aliases ${{ inputs.versions != '' && inputs.versions || 'dev' }}
```

### Comparing `syntheseus-0.3.0/.pre-commit-config.yaml` & `syntheseus-0.4.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -42,11 +42,11 @@
       - id: mypy
         name: "mypy"
         files: "syntheseus/"
         args: ["--install-types", "--non-interactive"]
 
   # Latest ruff (does linting + more)
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: 'v0.0.263'
+    rev: 'v0.2.1'
     hooks:
       - id: ruff
         args: [--fix]
```

### Comparing `syntheseus-0.3.0/CHANGELOG.md` & `syntheseus-0.4.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,53 @@
 All notable changes to the project are documented in this file.
 
 The format follows [Common Changelog](https://common-changelog.org/),
 and the project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
-## [0.3.0] - 2023-12-19
+## [0.4.0] - 2024-04-10
+
+### Changed
+
+- Merge reaction and reaction model base classes in `search` and `reaction_predction` ([#63](https://github.com/microsoft/syntheseus/pull/63), [#67](https://github.com/microsoft/syntheseus/pull/67), [#73](https://github.com/microsoft/syntheseus/pull/73), [#74](https://github.com/microsoft/syntheseus/pull/74), [#76](https://github.com/microsoft/syntheseus/pull/76), [#84](https://github.com/microsoft/syntheseus/pull/84)) ([@austint], [@kmaziarz])
+- Make reaction models return `Sequence[Reaction]` instead of `PredictionList` objects ([#61](https://github.com/microsoft/syntheseus/pull/61)) ([@austint])
+- Suppress the remaining noisy logs and warnings coming from single-step models ([#53](https://github.com/microsoft/syntheseus/pull/53)) ([@kmaziarz])
+- Improve efficiency and logging of retro* algorithm ([#62](https://github.com/microsoft/syntheseus/pull/62)) ([@austint])
+- Improve error handling in single-step evaluation and allow CLI to use the default checkpoints ([#75](https://github.com/microsoft/syntheseus/pull/75)) ([@kmaziarz])
+- Make basic classes from `interface` importable from top-level ([#81](https://github.com/microsoft/syntheseus/pull/81)) ([@austint])
 
 ### Added
 
-- Add a general CLI endpoint ([#44](https://github.com/microsoft/syntheseus/pull/44)) ([@kmaziarz])
-- Add support for PDVN to the search CLI ([#46](https://github.com/microsoft/syntheseus/pull/46)) ([@fiberleif])
-- Add initial static documentation ([#45](https://github.com/microsoft/syntheseus/pull/45)) ([@kmaziarz])
+- Integrate the Graph2Edits model ([#65](https://github.com/microsoft/syntheseus/pull/65), [#66](https://github.com/microsoft/syntheseus/pull/66)) ([@kmaziarz])
+- Improve the docs and add tutorials ([#54](https://github.com/microsoft/syntheseus/pull/54), [#77](https://github.com/microsoft/syntheseus/pull/77), [#78](https://github.com/microsoft/syntheseus/pull/78), [#79](https://github.com/microsoft/syntheseus/pull/79), [#82](https://github.com/microsoft/syntheseus/pull/82)) ([@kmaziarz], [@austint])
+- Add random search algorithm as a simple baseline ([#83](https://github.com/microsoft/syntheseus/pull/83)) ([@austint])
+- Add optional argument `limit_graph_nodes` to base search algorithm class to stop search after the search graph exceeds a certain number of nodes ([#85](https://github.com/microsoft/syntheseus/pull/85)) ([@austint])
+
+### Fixed
+
+- Fix small issues in Chemformer, MEGAN and RootAligned ([#80](https://github.com/microsoft/syntheseus/pull/80)) ([@kmaziarz])
+- Get all single-step models to work on CPU ([#57](https://github.com/microsoft/syntheseus/pull/57)) ([@kmaziarz])
+- Make the data loader class work with relative paths ([#69](https://github.com/microsoft/syntheseus/pull/69)) ([@kmaziarz])
+
+## [0.3.0] - 2023-12-19
 
 ### Changed
 
 - Simplify single-step model setup ([#41](https://github.com/microsoft/syntheseus/pull/41), [#48](https://github.com/microsoft/syntheseus/pull/48)) ([@kmaziarz])
 - Refactor single-step evaluation script and move it to cli/ ([#43](https://github.com/microsoft/syntheseus/pull/43)) ([@kmaziarz])
 - Return model predictions as dataclasses instead of pydantic models ([#47](https://github.com/microsoft/syntheseus/pull/47)) ([@kmaziarz])
 - Make the package compatible with PyPI ([#50](https://github.com/microsoft/syntheseus/pull/50)) ([@kmaziarz])
 
+### Added
+
+- Add a general CLI endpoint ([#44](https://github.com/microsoft/syntheseus/pull/44)) ([@kmaziarz])
+- Add support for PDVN to the search CLI ([#46](https://github.com/microsoft/syntheseus/pull/46)) ([@fiberleif])
+- Add initial static documentation ([#45](https://github.com/microsoft/syntheseus/pull/45)) ([@kmaziarz])
+
 ## [0.2.0] - 2023-11-21
 
 ### Changed
 
 - Select search hyperparameters depending on which algorithm and single-step model are used ([#30](https://github.com/microsoft/syntheseus/pull/30)) ([@kmaziarz])
 - Improve the heuristic used for estimating diversity ([#22](https://github.com/microsoft/syntheseus/pull/22), [#28](https://github.com/microsoft/syntheseus/pull/28)) ([@kmaziarz])
 
@@ -52,16 +76,17 @@
 - Fix compatibility with Python 3.7 ([#5](https://github.com/microsoft/syntheseus/pull/5)) ([@kmaziarz])
 - Correct some typos and unclear error messages ([#39](https://github.com/microsoft/syntheseus/pull/39)) ([@austint])
 
 ## [0.1.0] - 2023-05-25
 
 :seedling: Initial public release, containing several multi-step search algorithms and a minimal interface for single-step models.
 
-[Unreleased]: https://github.com/microsoft/syntheseus/compare/v0.3.0...HEAD
+[Unreleased]: https://github.com/microsoft/syntheseus/compare/v0.4.0...HEAD
 [0.1.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.1.0
 [0.2.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.2.0
 [0.3.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.3.0
+[0.4.0]: https://github.com/microsoft/syntheseus/releases/tag/v0.4.0
 
 [@austint]: https://github.com/AustinT
 [@kmaziarz]: https://github.com/kmaziarz
 [@jagarridotorres]: https://github.com/jagarridotorres
 [@fiberleif]: https://github.com/fiberleif
```

### Comparing `syntheseus-0.3.0/LICENSE` & `syntheseus-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/PKG-INFO` & `syntheseus-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7379 6e74  : 2.1.Name: synt
 00000020: 6865 7365 7573 0a56 6572 7369 6f6e 3a20  heseus.Version: 
-00000030: 302e 332e 300a 5375 6d6d 6172 793a 2041  0.3.0.Summary: A
+00000030: 302e 342e 300a 5375 6d6d 6172 793a 2041  0.4.0.Summary: A
 00000040: 2070 6163 6b61 6765 2066 6f72 2072 6574   package for ret
 00000050: 726f 7379 6e74 6865 7469 6320 706c 616e  rosynthetic plan
 00000060: 6e69 6e67 2e0a 4175 7468 6f72 3a20 4175  ning..Author: Au
 00000070: 7374 696e 2054 7269 7070 2c20 4b72 7a79  stin Tripp, Krzy
 00000080: 737a 746f 6620 4d61 7a69 6172 7a2c 2047  sztof Maziarz, G
 00000090: 756f 7169 6e67 204c 6975 2c20 4d65 6761  uoqing Liu, Mega
 000000a0: 6e20 5374 616e 6c65 792c 204d 6172 7769  n Stanley, Marwi
@@ -129,268 +129,297 @@
 00000800: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
 00000810: 6972 6573 2d44 6973 743a 2070 7265 2d63  ires-Dist: pre-c
 00000820: 6f6d 6d69 743b 2065 7874 7261 203d 3d20  ommit; extra == 
 00000830: 2264 6576 220a 5072 6f76 6964 6573 2d45  "dev".Provides-E
 00000840: 7874 7261 3a20 6368 656d 666f 726d 6572  xtra: chemformer
 00000850: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 00000860: 7379 6e74 6865 7365 7573 2d63 6865 6d66  syntheseus-chemf
-00000870: 6f72 6d65 723b 2065 7874 7261 203d 3d20  ormer; extra == 
-00000880: 2263 6865 6d66 6f72 6d65 7222 0a50 726f  "chemformer".Pro
-00000890: 7669 6465 732d 4578 7472 613a 206c 6f63  vides-Extra: loc
-000008a0: 616c 2d72 6574 726f 0a52 6571 7569 7265  al-retro.Require
-000008b0: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
-000008c0: 7573 2d6c 6f63 616c 2d72 6574 726f 3b20  us-local-retro; 
-000008d0: 6578 7472 6120 3d3d 2022 6c6f 6361 6c2d  extra == "local-
-000008e0: 7265 7472 6f22 0a50 726f 7669 6465 732d  retro".Provides-
-000008f0: 4578 7472 613a 206d 6567 616e 0a52 6571  Extra: megan.Req
-00000900: 7569 7265 732d 4469 7374 3a20 7379 6e74  uires-Dist: synt
-00000910: 6865 7365 7573 2d6d 6567 616e 3b20 6578  heseus-megan; ex
-00000920: 7472 6120 3d3d 2022 6d65 6761 6e22 0a50  tra == "megan".P
-00000930: 726f 7669 6465 732d 4578 7472 613a 206d  rovides-Extra: m
-00000940: 686e 2d72 6561 6374 0a52 6571 7569 7265  hn-react.Require
-00000950: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
-00000960: 7573 2d6d 686e 7265 6163 743b 2065 7874  us-mhnreact; ext
-00000970: 7261 203d 3d20 226d 686e 2d72 6561 6374  ra == "mhn-react
-00000980: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
-00000990: 3a20 7265 7472 6f2d 6b6e 6e0a 5265 7175  : retro-knn.Requ
-000009a0: 6972 6573 2d44 6973 743a 2073 796e 7468  ires-Dist: synth
-000009b0: 6573 6575 732d 6c6f 6361 6c2d 7265 7472  eseus-local-retr
-000009c0: 6f3b 2065 7874 7261 203d 3d20 2272 6574  o; extra == "ret
-000009d0: 726f 2d6b 6e6e 220a 5265 7175 6972 6573  ro-knn".Requires
-000009e0: 2d44 6973 743a 2074 6f72 6368 2d73 6361  -Dist: torch-sca
-000009f0: 7474 6572 3b20 6578 7472 6120 3d3d 2022  tter; extra == "
-00000a00: 7265 7472 6f2d 6b6e 6e22 0a50 726f 7669  retro-knn".Provi
-00000a10: 6465 732d 4578 7472 613a 2072 6f6f 742d  des-Extra: root-
-00000a20: 616c 6967 6e65 640a 5265 7175 6972 6573  aligned.Requires
-00000a30: 2d44 6973 743a 2073 796e 7468 6573 6575  -Dist: syntheseu
-00000a40: 732d 726f 6f74 2d61 6c69 676e 6564 3b20  s-root-aligned; 
-00000a50: 6578 7472 6120 3d3d 2022 726f 6f74 2d61  extra == "root-a
-00000a60: 6c69 676e 6564 220a 5072 6f76 6964 6573  ligned".Provides
-00000a70: 2d45 7874 7261 3a20 616c 6c2d 7369 6e67  -Extra: all-sing
-00000a80: 6c65 2d73 7465 700a 5265 7175 6972 6573  le-step.Requires
-00000a90: 2d44 6973 743a 2073 796e 7468 6573 6575  -Dist: syntheseu
-00000aa0: 735b 6368 656d 666f 726d 6572 2c6c 6f63  s[chemformer,loc
-00000ab0: 616c 2d72 6574 726f 2c6d 6567 616e 2c6d  al-retro,megan,m
-00000ac0: 686e 2d72 6561 6374 2c72 6574 726f 2d6b  hn-react,retro-k
-00000ad0: 6e6e 2c72 6f6f 742d 616c 6967 6e65 645d  nn,root-aligned]
-00000ae0: 3b20 6578 7472 6120 3d3d 2022 616c 6c2d  ; extra == "all-
-00000af0: 7369 6e67 6c65 2d73 7465 7022 0a50 726f  single-step".Pro
-00000b00: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
-00000b10: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b20: 7379 6e74 6865 7365 7573 5b61 6c6c 2d73  syntheseus[all-s
-00000b30: 696e 676c 652d 7374 6570 2c64 6576 2c76  ingle-step,dev,v
-00000b40: 697a 5d3b 2065 7874 7261 203d 3d20 2261  iz]; extra == "a
-00000b50: 6c6c 220a 0a3c 6469 7620 616c 6967 6e3d  ll"..<div align=
-00000b60: 2263 656e 7465 7222 3e0a 2020 2020 3c69  "center">.    <i
-00000b70: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000b80: 6769 7468 7562 2e63 6f6d 2f6d 6963 726f  github.com/micro
-00000b90: 736f 6674 2f73 796e 7468 6573 6575 732f  soft/syntheseus/
-00000ba0: 6173 7365 7473 2f36 3134 3730 3932 332f  assets/61470923/
-00000bb0: 6630 3161 3939 3339 2d36 3166 612d 3434  f01a9939-61fa-44
-00000bc0: 3631 2d61 3132 342d 6331 3365 6464 6364  61-a124-c13eddcd
-00000bd0: 6437 3561 2220 6865 6967 6874 3d22 3530  d75a" height="50
-00000be0: 7078 223e 0a20 2020 203c 6833 3e3c 693e  px">.    <h3><i>
-00000bf0: 4e61 7669 6761 7469 6e67 2074 6865 206c  Navigating the l
-00000c00: 6162 7972 696e 7468 206f 6620 7379 6e74  abyrinth of synt
-00000c10: 6865 7369 7320 706c 616e 6e69 6e67 3c2f  hesis planning</
-00000c20: 693e 3c2f 6833 3e0a 3c2f 6469 763e 0a0a  i></h3>.</div>..
-00000c30: 2d2d 2d0a 0a5b 215b 4349 5d28 6874 7470  ---..[![CI](http
-00000c40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000c50: 6963 726f 736f 6674 2f73 796e 7468 6573  icrosoft/synthes
-00000c60: 6575 732f 6163 7469 6f6e 732f 776f 726b  eus/actions/work
-00000c70: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
-00000c80: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-00000c90: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
-00000ca0: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
-00000cb0: 742f 7379 6e74 6865 7365 7573 2f61 6374  t/syntheseus/act
-00000cc0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
-00000cd0: 692e 796d 6c29 0a5b 215b 5079 7468 6f6e  i.yml).[![Python
-00000ce0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
-00000cf0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000d00: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
-00000d10: 372b 2d62 6c75 652e 7376 6729 5d28 6874  7+-blue.svg)](ht
-00000d20: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000d30: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000d40: 0a5b 215b 636f 6465 2073 7479 6c65 5d28  .[![code style](
-00000d50: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000d60: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-00000d70: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000d80: 3230 3230 3230 2e73 7667 295d 2868 7474  202020.svg)](htt
-00000d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000da0: 616d 6276 2f62 6c61 636b 290a 5b21 5b4c  ambv/black).[![L
-00000db0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
-00000dc0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000dd0: 6164 6765 2f6c 6963 656e 7365 2d4d 4954  adge/license-MIT
-00000de0: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
-00000df0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e00: 6d69 6372 6f73 6f66 742f 7379 6e74 6865  microsoft/synthe
-00000e10: 7365 7573 2f62 6c6f 622f 6d61 696e 2f4c  seus/blob/main/L
-00000e20: 4943 454e 5345 290a 0a53 796e 7468 6573  ICENSE)..Synthes
-00000e30: 6575 7320 6973 2061 2070 6163 6b61 6765  eus is a package
-00000e40: 2066 6f72 2065 6e64 2d74 6f2d 656e 6420   for end-to-end 
-00000e50: 7265 7472 6f73 796e 7468 6574 6963 2070  retrosynthetic p
-00000e60: 6c61 6e6e 696e 672e 0a2d 20e2 9a92 efb8  lanning..- .....
-00000e70: 8f20 436f 6d62 696e 6573 2073 6561 7263  . Combines searc
-00000e80: 6820 616c 676f 7269 7468 6d73 2061 6e64  h algorithms and
-00000e90: 2072 6561 6374 696f 6e20 6d6f 6465 6c73   reaction models
-00000ea0: 2069 6e20 6120 7374 616e 6461 7264 697a   in a standardiz
-00000eb0: 6564 2077 6179 0a2d 20f0 9fa7 ad20 496e  ed way.- .... In
-00000ec0: 636c 7564 6573 2069 6d70 6c65 6d65 6e74  cludes implement
-00000ed0: 6174 696f 6e73 206f 6620 636f 6d6d 6f6e  ations of common
-00000ee0: 2073 6561 7263 6820 616c 676f 7269 7468   search algorith
-00000ef0: 6d73 0a2d 20f0 9fa7 aa20 496e 636c 7564  ms.- .... Includ
-00000f00: 6573 2077 7261 7070 6572 7320 666f 7220  es wrappers for 
-00000f10: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
-00000f20: 2072 6561 6374 696f 6e20 6d6f 6465 6c73   reaction models
-00000f30: 0a2d 20e2 9a99 efb8 8f20 4578 706f 7365  .- ...... Expose
-00000f40: 7320 6120 7369 6d70 6c65 2041 5049 2074  s a simple API t
-00000f50: 6f20 706c 7567 2069 6e20 6375 7374 6f6d  o plug in custom
-00000f60: 206d 6f64 656c 7320 616e 6420 616c 676f   models and algo
-00000f70: 7269 7468 6d73 0a2d 20f0 9f93 8820 4361  rithms.- .... Ca
-00000f80: 6e20 6265 2075 7365 6420 746f 2062 656e  n be used to ben
-00000f90: 6368 6d61 726b 2063 6f6d 706f 6e65 6e74  chmark component
-00000fa0: 7320 6f66 2061 2072 6574 726f 7379 6e74  s of a retrosynt
-00000fb0: 6865 7369 7320 7069 7065 6c69 6e65 0a0a  hesis pipeline..
-00000fc0: 546f 206c 6561 726e 2061 626f 7574 2060  To learn about `
-00000fd0: 7379 6e74 6865 7365 7573 6027 7320 6665  syntheseus`'s fe
-00000fe0: 6174 7572 6573 2061 6e64 2041 5049 2076  atures and API v
-00000ff0: 6973 6974 205b 6d69 6372 6f73 6f66 742e  isit [microsoft.
-00001000: 6769 7468 7562 2e69 6f2f 7379 6e74 6865  github.io/synthe
-00001010: 7365 7573 5d28 6874 7470 733a 2f2f 6d69  seus](https://mi
-00001020: 6372 6f73 6f66 742e 6769 7468 7562 2e69  crosoft.github.i
-00001030: 6f2f 7379 6e74 6865 7365 7573 292e 0a0a  o/syntheseus)...
-00001040: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
-00001050: 546f 2069 6e73 7461 6c6c 2060 7379 6e74  To install `synt
-00001060: 6865 7365 7573 6020 7769 7468 2061 6c6c  heseus` with all
-00001070: 2074 6865 2065 7874 7261 732c 2072 756e   the extras, run
-00001080: 0a0a 6060 6062 6173 680a 636f 6e64 6120  ..```bash.conda 
-00001090: 656e 7620 6372 6561 7465 202d 6620 656e  env create -f en
-000010a0: 7669 726f 6e6d 656e 745f 6675 6c6c 2e79  vironment_full.y
-000010b0: 6d6c 0a63 6f6e 6461 2061 6374 6976 6174  ml.conda activat
-000010c0: 6520 7379 6e74 6865 7365 7573 2d66 756c  e syntheseus-ful
-000010d0: 6c0a 0a70 6970 2069 6e73 7461 6c6c 202d  l..pip install -
-000010e0: 6520 222e 5b61 6c6c 5d22 0a60 6060 0a0a  e ".[all]".```..
-000010f0: 5365 6520 5b64 6f63 756d 656e 7461 7469  See [documentati
-00001100: 6f6e 5d28 6874 7470 733a 2f2f 6d69 6372  on](https://micr
-00001110: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
-00001120: 7379 6e74 6865 7365 7573 2f69 6e73 7461  syntheseus/insta
-00001130: 6c6c 6174 696f 6e29 2069 6620 796f 7520  llation) if you 
-00001140: 7072 6566 6572 2061 206d 6f72 6520 6c69  prefer a more li
-00001150: 6768 7477 6569 6768 7420 696e 7374 616c  ghtweight instal
-00001160: 6c61 7469 6f6e 2074 6861 7420 6f6e 6c79  lation that only
-00001170: 2069 6e63 6c75 6465 7320 7468 6520 7061   includes the pa
-00001180: 7274 7320 796f 7520 6163 7475 616c 6c79  rts you actually
-00001190: 206e 6565 642e 0a0a 2323 2044 6576 656c   need...## Devel
-000011a0: 6f70 6d65 6e74 0a0a 5379 6e74 6865 7365  opment..Synthese
-000011b0: 7573 2069 7320 6375 7272 656e 746c 7920  us is currently 
-000011c0: 756e 6465 7220 6163 7469 7665 2064 6576  under active dev
-000011d0: 656c 6f70 6d65 6e74 2e0a 4966 2079 6f75  elopment..If you
-000011e0: 2077 616e 7420 746f 2068 656c 7020 7573   want to help us
-000011f0: 2064 6576 656c 6f70 2073 796e 7468 6573   develop synthes
-00001200: 6575 7320 706c 6561 7365 2069 6e73 7461  eus please insta
-00001210: 6c6c 2061 6e64 2072 756e 2060 7072 652d  ll and run `pre-
-00001220: 636f 6d6d 6974 600a 6368 6563 6b73 2062  commit`.checks b
-00001230: 6566 6f72 6520 636f 6d6d 6974 7469 6e67  efore committing
-00001240: 2063 6f64 652e 0a0a 5765 2075 7365 2060   code...We use `
-00001250: 7079 7465 7374 6020 666f 7220 7465 7374  pytest` for test
-00001260: 696e 672e 2050 6c65 6173 6520 6d61 6b65  ing. Please make
-00001270: 2073 7572 6520 7465 7374 7320 7061 7373   sure tests pass
-00001280: 206f 6e20 796f 7572 2062 7261 6e63 6820   on your branch 
-00001290: 6265 666f 7265 0a73 7562 6d69 7474 696e  before.submittin
-000012a0: 6720 6120 5052 2028 616e 6420 7472 7920  g a PR (and try 
-000012b0: 746f 206d 6169 6e74 6169 6e20 6869 6768  to maintain high
-000012c0: 2074 6573 7420 636f 7665 7261 6765 292e   test coverage).
-000012d0: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
-000012e0: 202d 6d20 7079 7465 7374 202d 2d63 6f76   -m pytest --cov
-000012f0: 2073 796e 7468 6573 6575 732f 7465 7374   syntheseus/test
-00001300: 730a 6060 600a 0a23 2320 436f 6e74 7269  s.```..## Contri
-00001310: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
-00001320: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
-00001330: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
-00001340: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
-00001350: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
-00001360: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
-00001370: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
-00001380: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
-00001390: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
-000013a0: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
-000013b0: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
-000013c0: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
-000013d0: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
-000013e0: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
-000013f0: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
-00001400: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
-00001410: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
-00001420: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
-00001430: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
-00001440: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
-00001450: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
-00001460: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
-00001470: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
-00001480: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
-00001490: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
-000014a0: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
-000014b0: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
-000014c0: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
-000014d0: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
-000014e0: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
-000014f0: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
-00001500: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
-00001510: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
-00001520: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
-00001530: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
-00001540: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
-00001550: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
-00001560: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
-00001570: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
-00001580: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
-00001590: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
-000015a0: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
-000015b0: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
-000015c0: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
-000015d0: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
-000015e0: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
-000015f0: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
-00001600: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
-00001610: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
-00001620: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
-00001630: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
-00001640: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
-00001650: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
-00001660: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
-00001670: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
-00001680: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
-00001690: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
-000016a0: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
-000016b0: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
-000016c0: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
-000016d0: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
-000016e0: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
-000016f0: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
-00001700: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
-00001710: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
-00001720: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
-00001730: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
-00001740: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
-00001750: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
-00001760: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
-00001770: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
-00001780: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00001790: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
-000017a0: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
-000017b0: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
-000017c0: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
-000017d0: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
-000017e0: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
-000017f0: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
-00001800: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
-00001810: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
-00001820: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
-00001830: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
-00001840: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
-00001850: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
-00001860: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
-00001870: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
-00001880: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
-00001890: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
-000018a0: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
-000018b0: 6f6c 6963 6965 732e 0a                   olicies..
+00000870: 6f72 6d65 723d 3d30 2e31 2e31 3b20 6578  ormer==0.1.1; ex
+00000880: 7472 6120 3d3d 2022 6368 656d 666f 726d  tra == "chemform
+00000890: 6572 220a 5072 6f76 6964 6573 2d45 7874  er".Provides-Ext
+000008a0: 7261 3a20 6772 6170 6832 6564 6974 730a  ra: graph2edits.
+000008b0: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+000008c0: 796e 7468 6573 6575 732d 6772 6170 6832  yntheseus-graph2
+000008d0: 6564 6974 733d 3d30 2e32 2e30 3b20 6578  edits==0.2.0; ex
+000008e0: 7472 6120 3d3d 2022 6772 6170 6832 6564  tra == "graph2ed
+000008f0: 6974 7322 0a50 726f 7669 6465 732d 4578  its".Provides-Ex
+00000900: 7472 613a 206c 6f63 616c 2d72 6574 726f  tra: local-retro
+00000910: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000920: 7379 6e74 6865 7365 7573 2d6c 6f63 616c  syntheseus-local
+00000930: 2d72 6574 726f 3d3d 302e 342e 303b 2065  -retro==0.4.0; e
+00000940: 7874 7261 203d 3d20 226c 6f63 616c 2d72  xtra == "local-r
+00000950: 6574 726f 220a 5072 6f76 6964 6573 2d45  etro".Provides-E
+00000960: 7874 7261 3a20 6d65 6761 6e0a 5265 7175  xtra: megan.Requ
+00000970: 6972 6573 2d44 6973 743a 2073 796e 7468  ires-Dist: synth
+00000980: 6573 6575 732d 6d65 6761 6e3d 3d30 2e31  eseus-megan==0.1
+00000990: 2e30 3b20 6578 7472 6120 3d3d 2022 6d65  .0; extra == "me
+000009a0: 6761 6e22 0a50 726f 7669 6465 732d 4578  gan".Provides-Ex
+000009b0: 7472 613a 206d 686e 2d72 6561 6374 0a52  tra: mhn-react.R
+000009c0: 6571 7569 7265 732d 4469 7374 3a20 7379  equires-Dist: sy
+000009d0: 6e74 6865 7365 7573 2d6d 686e 7265 6163  ntheseus-mhnreac
+000009e0: 743d 3d31 2e30 2e30 3b20 6578 7472 6120  t==1.0.0; extra 
+000009f0: 3d3d 2022 6d68 6e2d 7265 6163 7422 0a50  == "mhn-react".P
+00000a00: 726f 7669 6465 732d 4578 7472 613a 2072  rovides-Extra: r
+00000a10: 6574 726f 2d6b 6e6e 0a52 6571 7569 7265  etro-knn.Require
+00000a20: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
+00000a30: 7573 5b6c 6f63 616c 2d72 6574 726f 5d3b  us[local-retro];
+00000a40: 2065 7874 7261 203d 3d20 2272 6574 726f   extra == "retro
+00000a50: 2d6b 6e6e 220a 5265 7175 6972 6573 2d44  -knn".Requires-D
+00000a60: 6973 743a 2074 6f72 6368 2d73 6361 7474  ist: torch-scatt
+00000a70: 6572 3b20 6578 7472 6120 3d3d 2022 7265  er; extra == "re
+00000a80: 7472 6f2d 6b6e 6e22 0a50 726f 7669 6465  tro-knn".Provide
+00000a90: 732d 4578 7472 613a 2072 6f6f 742d 616c  s-Extra: root-al
+00000aa0: 6967 6e65 640a 5265 7175 6972 6573 2d44  igned.Requires-D
+00000ab0: 6973 743a 2073 796e 7468 6573 6575 732d  ist: syntheseus-
+00000ac0: 726f 6f74 2d61 6c69 676e 6564 3d3d 302e  root-aligned==0.
+00000ad0: 312e 303b 2065 7874 7261 203d 3d20 2272  1.0; extra == "r
+00000ae0: 6f6f 742d 616c 6967 6e65 6422 0a50 726f  oot-aligned".Pro
+00000af0: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
+00000b00: 2d73 696e 676c 652d 7374 6570 0a52 6571  -single-step.Req
+00000b10: 7569 7265 732d 4469 7374 3a20 7379 6e74  uires-Dist: synt
+00000b20: 6865 7365 7573 5b63 6865 6d66 6f72 6d65  heseus[chemforme
+00000b30: 722c 6772 6170 6832 6564 6974 732c 6c6f  r,graph2edits,lo
+00000b40: 6361 6c2d 7265 7472 6f2c 6d65 6761 6e2c  cal-retro,megan,
+00000b50: 6d68 6e2d 7265 6163 742c 7265 7472 6f2d  mhn-react,retro-
+00000b60: 6b6e 6e2c 726f 6f74 2d61 6c69 676e 6564  knn,root-aligned
+00000b70: 5d3b 2065 7874 7261 203d 3d20 2261 6c6c  ]; extra == "all
+00000b80: 2d73 696e 676c 652d 7374 6570 220a 5072  -single-step".Pr
+00000b90: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
+00000ba0: 6c0a 5265 7175 6972 6573 2d44 6973 743a  l.Requires-Dist:
+00000bb0: 2073 796e 7468 6573 6575 735b 616c 6c2d   syntheseus[all-
+00000bc0: 7369 6e67 6c65 2d73 7465 702c 6465 762c  single-step,dev,
+00000bd0: 7669 7a5d 3b20 6578 7472 6120 3d3d 2022  viz]; extra == "
+00000be0: 616c 6c22 0a0a 3c64 6976 2061 6c69 676e  all"..<div align
+00000bf0: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00000c00: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000c10: 2f67 6974 6875 622e 636f 6d2f 6d69 6372  /github.com/micr
+00000c20: 6f73 6f66 742f 7379 6e74 6865 7365 7573  osoft/syntheseus
+00000c30: 2f61 7373 6574 732f 3631 3437 3039 3233  /assets/61470923
+00000c40: 2f66 3031 6139 3933 392d 3631 6661 2d34  /f01a9939-61fa-4
+00000c50: 3436 312d 6131 3234 2d63 3133 6564 6463  461-a124-c13eddc
+00000c60: 6464 3735 6122 2068 6569 6768 743d 2235  dd75a" height="5
+00000c70: 3070 7822 3e0a 2020 2020 3c68 333e 3c69  0px">.    <h3><i
+00000c80: 3e4e 6176 6967 6174 696e 6720 7468 6520  >Navigating the 
+00000c90: 6c61 6279 7269 6e74 6820 6f66 2073 796e  labyrinth of syn
+00000ca0: 7468 6573 6973 2070 6c61 6e6e 696e 673c  thesis planning<
+00000cb0: 2f69 3e3c 2f68 333e 0a0a 2d2d 2d0a 0a3c  /i></h3>..---..<
+00000cc0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000cd0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000ce0: 7073 3a2f 2f6d 6963 726f 736f 6674 2e67  ps://microsoft.g
+00000cf0: 6974 6875 622e 696f 2f73 796e 7468 6573  ithub.io/synthes
+00000d00: 6575 732f 7374 6162 6c65 223e 446f 6373  eus/stable">Docs
+00000d10: 3c2f 613e 20e2 80a2 0a20 203c 6120 6872  </a> ....  <a hr
+00000d20: 6566 3d22 6874 7470 733a 2f2f 6d69 6372  ef="https://micr
+00000d30: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
+00000d40: 7379 6e74 6865 7365 7573 2f73 7461 626c  syntheseus/stabl
+00000d50: 652f 636c 692f 6576 616c 5f73 696e 676c  e/cli/eval_singl
+00000d60: 655f 7374 6570 2f22 3e43 4c49 3c2f 613e  e_step/">CLI</a>
+00000d70: 20e2 80a2 0a20 203c 6120 6872 6566 3d22   ....  <a href="
+00000d80: 6874 7470 733a 2f2f 6d69 6372 6f73 6f66  https://microsof
+00000d90: 742e 6769 7468 7562 2e69 6f2f 7379 6e74  t.github.io/synt
+00000da0: 6865 7365 7573 2f73 7461 626c 652f 7475  heseus/stable/tu
+00000db0: 746f 7269 616c 732f 7175 6963 6b5f 7374  torials/quick_st
+00000dc0: 6172 742f 223e 5475 746f 7269 616c 733c  art/">Tutorials<
+00000dd0: 2f61 3e20 e280 a20a 2020 3c61 2068 7265  /a> ....  <a hre
+00000de0: 663d 2268 7474 7073 3a2f 2f61 7278 6976  f="https://arxiv
+00000df0: 2e6f 7267 2f61 6273 2f32 3331 302e 3139  .org/abs/2310.19
+00000e00: 3739 3622 3e50 6170 6572 3c2f 613e 0a3c  796">Paper</a>.<
+00000e10: 2f70 3e0a 0a5b 215b 4349 5d28 6874 7470  /p>..[![CI](http
+00000e20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000e30: 6963 726f 736f 6674 2f73 796e 7468 6573  icrosoft/synthes
+00000e40: 6575 732f 6163 7469 6f6e 732f 776f 726b  eus/actions/work
+00000e50: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
+00000e60: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000e70: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000e80: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
+00000e90: 742f 7379 6e74 6865 7365 7573 2f61 6374  t/syntheseus/act
+00000ea0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
+00000eb0: 692e 796d 6c29 0a5b 215b 5079 7468 6f6e  i.yml).[![Python
+00000ec0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000ed0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000ee0: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+00000ef0: 372b 2d62 6c75 652e 7376 6729 5d28 6874  7+-blue.svg)](ht
+00000f00: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
+00000f10: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
+00000f20: 0a5b 215b 7079 7069 5d28 6874 7470 733a  .[![pypi](https:
+00000f30: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000f40: 2f70 7970 692f 762f 7379 6e74 6865 7365  /pypi/v/synthese
+00000f50: 7573 2e73 7667 295d 2868 7474 7073 3a2f  us.svg)](https:/
+00000f60: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000f70: 742f 7379 6e74 6865 7365 7573 2f29 0a5b  t/syntheseus/).[
+00000f80: 215b 636f 6465 2073 7479 6c65 5d28 6874  ![code style](ht
+00000f90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000fa0: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+00000fb0: 3230 7374 796c 652d 626c 6163 6b2d 3230  20style-black-20
+00000fc0: 3230 3230 2e73 7667 295d 2868 7474 7073  2020.svg)](https
+00000fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616d  ://github.com/am
+00000fe0: 6276 2f62 6c61 636b 290a 5b21 5b4c 6963  bv/black).[![Lic
+00000ff0: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
+00001000: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00001010: 6765 2f6c 6963 656e 7365 2d4d 4954 2d67  ge/license-MIT-g
+00001020: 7265 656e 2e73 7667 295d 2868 7474 7073  reen.svg)](https
+00001030: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d69  ://github.com/mi
+00001040: 6372 6f73 6f66 742f 7379 6e74 6865 7365  crosoft/synthese
+00001050: 7573 2f62 6c6f 622f 6d61 696e 2f4c 4943  us/blob/main/LIC
+00001060: 454e 5345 290a 0a3c 2f64 6976 3e0a 0a23  ENSE)..</div>..#
+00001070: 2320 4f76 6572 7669 6577 0a0a 5379 6e74  # Overview..Synt
+00001080: 6865 7365 7573 2069 7320 6120 7061 636b  heseus is a pack
+00001090: 6167 6520 666f 7220 656e 642d 746f 2d65  age for end-to-e
+000010a0: 6e64 2072 6574 726f 7379 6e74 6865 7469  nd retrosyntheti
+000010b0: 6320 706c 616e 6e69 6e67 2e0a 2d20 e29a  c planning..- ..
+000010c0: 92ef b88f 2043 6f6d 6269 6e65 7320 7365  .... Combines se
+000010d0: 6172 6368 2061 6c67 6f72 6974 686d 7320  arch algorithms 
+000010e0: 616e 6420 7265 6163 7469 6f6e 206d 6f64  and reaction mod
+000010f0: 656c 7320 696e 2061 2073 7461 6e64 6172  els in a standar
+00001100: 6469 7a65 6420 7761 790a 2d20 f09f a7ad  dized way.- ....
+00001110: 2049 6e63 6c75 6465 7320 696d 706c 656d   Includes implem
+00001120: 656e 7461 7469 6f6e 7320 6f66 2063 6f6d  entations of com
+00001130: 6d6f 6e20 7365 6172 6368 2061 6c67 6f72  mon search algor
+00001140: 6974 686d 730a 2d20 f09f a7aa 2049 6e63  ithms.- .... Inc
+00001150: 6c75 6465 7320 7772 6170 7065 7273 2066  ludes wrappers f
+00001160: 6f72 2073 7461 7465 2d6f 662d 7468 652d  or state-of-the-
+00001170: 6172 7420 7265 6163 7469 6f6e 206d 6f64  art reaction mod
+00001180: 656c 730a 2d20 e29a 99ef b88f 2045 7870  els.- ...... Exp
+00001190: 6f73 6573 2061 2073 696d 706c 6520 4150  oses a simple AP
+000011a0: 4920 746f 2070 6c75 6720 696e 2063 7573  I to plug in cus
+000011b0: 746f 6d20 6d6f 6465 6c73 2061 6e64 2061  tom models and a
+000011c0: 6c67 6f72 6974 686d 730a 2d20 f09f 9388  lgorithms.- ....
+000011d0: 2043 616e 2062 6520 7573 6564 2074 6f20   Can be used to 
+000011e0: 6265 6e63 686d 6172 6b20 636f 6d70 6f6e  benchmark compon
+000011f0: 656e 7473 206f 6620 6120 7265 7472 6f73  ents of a retros
+00001200: 796e 7468 6573 6973 2070 6970 656c 696e  ynthesis pipelin
+00001210: 650a 0a23 2320 5175 6963 6b20 5374 6172  e..## Quick Star
+00001220: 740a 0a54 6f20 696e 7374 616c 6c20 6073  t..To install `s
+00001230: 796e 7468 6573 6575 7360 2077 6974 6820  yntheseus` with 
+00001240: 616c 6c20 7468 6520 6578 7472 6173 2c20  all the extras, 
+00001250: 7275 6e0a 0a60 6060 6261 7368 0a63 6f6e  run..```bash.con
+00001260: 6461 2065 6e76 2063 7265 6174 6520 2d66  da env create -f
+00001270: 2065 6e76 6972 6f6e 6d65 6e74 5f66 756c   environment_ful
+00001280: 6c2e 796d 6c0a 636f 6e64 6120 6163 7469  l.yml.conda acti
+00001290: 7661 7465 2073 796e 7468 6573 6575 732d  vate syntheseus-
+000012a0: 6675 6c6c 0a0a 7069 7020 696e 7374 616c  full..pip instal
+000012b0: 6c20 2273 796e 7468 6573 6575 735b 616c  l "syntheseus[al
+000012c0: 6c5d 220a 6060 600a 0a53 6565 205b 6865  l]".```..See [he
+000012d0: 7265 5d28 6874 7470 733a 2f2f 6d69 6372  re](https://micr
+000012e0: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
+000012f0: 7379 6e74 6865 7365 7573 2f69 6e73 7461  syntheseus/insta
+00001300: 6c6c 6174 696f 6e29 2069 6620 796f 7520  llation) if you 
+00001310: 7072 6566 6572 2061 206d 6f72 6520 6c69  prefer a more li
+00001320: 6768 7477 6569 6768 7420 696e 7374 616c  ghtweight instal
+00001330: 6c61 7469 6f6e 2074 6861 7420 6f6e 6c79  lation that only
+00001340: 2069 6e63 6c75 6465 7320 7468 6520 7061   includes the pa
+00001350: 7274 7320 796f 7520 6163 7475 616c 6c79  rts you actually
+00001360: 206e 6565 642e 0a0a 2323 2044 6576 656c   need...## Devel
+00001370: 6f70 6d65 6e74 0a0a 5379 6e74 6865 7365  opment..Synthese
+00001380: 7573 2069 7320 6375 7272 656e 746c 7920  us is currently 
+00001390: 756e 6465 7220 6163 7469 7665 2064 6576  under active dev
+000013a0: 656c 6f70 6d65 6e74 2e0a 4966 2079 6f75  elopment..If you
+000013b0: 2077 616e 7420 746f 2068 656c 7020 7573   want to help us
+000013c0: 2064 6576 656c 6f70 2073 796e 7468 6573   develop synthes
+000013d0: 6575 7320 706c 6561 7365 2069 6e73 7461  eus please insta
+000013e0: 6c6c 2061 6e64 2072 756e 2060 7072 652d  ll and run `pre-
+000013f0: 636f 6d6d 6974 600a 6368 6563 6b73 2062  commit`.checks b
+00001400: 6566 6f72 6520 636f 6d6d 6974 7469 6e67  efore committing
+00001410: 2063 6f64 652e 0a0a 5765 2075 7365 2060   code...We use `
+00001420: 7079 7465 7374 6020 666f 7220 7465 7374  pytest` for test
+00001430: 696e 672e 2050 6c65 6173 6520 6d61 6b65  ing. Please make
+00001440: 2073 7572 6520 7465 7374 7320 7061 7373   sure tests pass
+00001450: 206f 6e20 796f 7572 2062 7261 6e63 6820   on your branch 
+00001460: 6265 666f 7265 0a73 7562 6d69 7474 696e  before.submittin
+00001470: 6720 6120 5052 2028 616e 6420 7472 7920  g a PR (and try 
+00001480: 746f 206d 6169 6e74 6169 6e20 6869 6768  to maintain high
+00001490: 2074 6573 7420 636f 7665 7261 6765 292e   test coverage).
+000014a0: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+000014b0: 202d 6d20 7079 7465 7374 202d 2d63 6f76   -m pytest --cov
+000014c0: 2073 796e 7468 6573 6575 732f 7465 7374   syntheseus/test
+000014d0: 730a 6060 600a 0a23 2320 436f 6e74 7269  s.```..## Contri
+000014e0: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
+000014f0: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
+00001500: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
+00001510: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
+00001520: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
+00001530: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
+00001540: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
+00001550: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
+00001560: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
+00001570: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
+00001580: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
+00001590: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
+000015a0: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
+000015b0: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
+000015c0: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
+000015d0: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
+000015e0: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
+000015f0: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
+00001600: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
+00001610: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
+00001620: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
+00001630: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
+00001640: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
+00001650: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
+00001660: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+00001670: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
+00001680: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
+00001690: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
+000016a0: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
+000016b0: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
+000016c0: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
+000016d0: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
+000016e0: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
+000016f0: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
+00001700: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
+00001710: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
+00001720: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
+00001730: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
+00001740: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
+00001750: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
+00001760: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
+00001770: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
+00001780: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
+00001790: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
+000017a0: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
+000017b0: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
+000017c0: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
+000017d0: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
+000017e0: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
+000017f0: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
+00001800: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
+00001810: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
+00001820: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
+00001830: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
+00001840: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
+00001850: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
+00001860: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
+00001870: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
+00001880: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
+00001890: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
+000018a0: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
+000018b0: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
+000018c0: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
+000018d0: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
+000018e0: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
+000018f0: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
+00001900: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
+00001910: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
+00001920: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
+00001930: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
+00001940: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
+00001950: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
+00001960: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
+00001970: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
+00001980: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
+00001990: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
+000019a0: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
+000019b0: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
+000019c0: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
+000019d0: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
+000019e0: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
+000019f0: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
+00001a00: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
+00001a10: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
+00001a20: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
+00001a30: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
+00001a40: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
+00001a50: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
+00001a60: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
+00001a70: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
+00001a80: 6f6c 6963 6965 732e 0a                   olicies..
```

### Comparing `syntheseus-0.3.0/README.md` & `syntheseus-0.4.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,209 +7,229 @@
 00000060: 3933 392d 3631 6661 2d34 3436 312d 6131  939-61fa-4461-a1
 00000070: 3234 2d63 3133 6564 6463 6464 3735 6122  24-c13eddcdd75a"
 00000080: 2068 6569 6768 743d 2235 3070 7822 3e0a   height="50px">.
 00000090: 2020 2020 3c68 333e 3c69 3e4e 6176 6967      <h3><i>Navig
 000000a0: 6174 696e 6720 7468 6520 6c61 6279 7269  ating the labyri
 000000b0: 6e74 6820 6f66 2073 796e 7468 6573 6973  nth of synthesis
 000000c0: 2070 6c61 6e6e 696e 673c 2f69 3e3c 2f68   planning</i></h
-000000d0: 333e 0a3c 2f64 6976 3e0a 0a2d 2d2d 0a0a  3>.</div>..---..
-000000e0: 5b21 5b43 495d 2868 7474 7073 3a2f 2f67  [![CI](https://g
-000000f0: 6974 6875 622e 636f 6d2f 6d69 6372 6f73  ithub.com/micros
-00000100: 6f66 742f 7379 6e74 6865 7365 7573 2f61  oft/syntheseus/a
-00000110: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
-00000120: 2f63 692e 796d 6c2f 6261 6467 652e 7376  /ci.yml/badge.sv
-00000130: 673f 6272 616e 6368 3d6d 6169 6e29 5d28  g?branch=main)](
-00000140: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000150: 6f6d 2f6d 6963 726f 736f 6674 2f73 796e  om/microsoft/syn
-00000160: 7468 6573 6575 732f 6163 7469 6f6e 732f  theseus/actions/
-00000170: 776f 726b 666c 6f77 732f 6369 2e79 6d6c  workflows/ci.yml
-00000180: 290a 5b21 5b50 7974 686f 6e20 5665 7273  ).[![Python Vers
-00000190: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
-000001a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000001b0: 652f 7079 7468 6f6e 2d33 2e37 2b2d 626c  e/python-3.7+-bl
-000001c0: 7565 2e73 7667 295d 2868 7474 7073 3a2f  ue.svg)](https:/
-000001d0: 2f77 7777 2e70 7974 686f 6e2e 6f72 672f  /www.python.org/
-000001e0: 646f 776e 6c6f 6164 732f 290a 5b21 5b63  downloads/).[![c
-000001f0: 6f64 6520 7374 796c 655d 2868 7474 7073  ode style](https
-00000200: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000210: 6f2f 6261 6467 652f 636f 6465 2532 3073  o/badge/code%20s
-00000220: 7479 6c65 2d62 6c61 636b 2d32 3032 3032  tyle-black-20202
-00000230: 302e 7376 6729 5d28 6874 7470 733a 2f2f  0.svg)](https://
-00000240: 6769 7468 7562 2e63 6f6d 2f61 6d62 762f  github.com/ambv/
-00000250: 626c 6163 6b29 0a5b 215b 4c69 6365 6e73  black).[![Licens
-00000260: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
-00000270: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000280: 6c69 6365 6e73 652d 4d49 542d 6772 6565  license-MIT-gree
-00000290: 6e2e 7376 6729 5d28 6874 7470 733a 2f2f  n.svg)](https://
-000002a0: 6769 7468 7562 2e63 6f6d 2f6d 6963 726f  github.com/micro
-000002b0: 736f 6674 2f73 796e 7468 6573 6575 732f  soft/syntheseus/
-000002c0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
-000002d0: 4529 0a0a 5379 6e74 6865 7365 7573 2069  E)..Syntheseus i
-000002e0: 7320 6120 7061 636b 6167 6520 666f 7220  s a package for 
-000002f0: 656e 642d 746f 2d65 6e64 2072 6574 726f  end-to-end retro
-00000300: 7379 6e74 6865 7469 6320 706c 616e 6e69  synthetic planni
-00000310: 6e67 2e0a 2d20 e29a 92ef b88f 2043 6f6d  ng..- ...... Com
-00000320: 6269 6e65 7320 7365 6172 6368 2061 6c67  bines search alg
-00000330: 6f72 6974 686d 7320 616e 6420 7265 6163  orithms and reac
-00000340: 7469 6f6e 206d 6f64 656c 7320 696e 2061  tion models in a
-00000350: 2073 7461 6e64 6172 6469 7a65 6420 7761   standardized wa
-00000360: 790a 2d20 f09f a7ad 2049 6e63 6c75 6465  y.- .... Include
-00000370: 7320 696d 706c 656d 656e 7461 7469 6f6e  s implementation
-00000380: 7320 6f66 2063 6f6d 6d6f 6e20 7365 6172  s of common sear
-00000390: 6368 2061 6c67 6f72 6974 686d 730a 2d20  ch algorithms.- 
-000003a0: f09f a7aa 2049 6e63 6c75 6465 7320 7772  .... Includes wr
-000003b0: 6170 7065 7273 2066 6f72 2073 7461 7465  appers for state
-000003c0: 2d6f 662d 7468 652d 6172 7420 7265 6163  -of-the-art reac
-000003d0: 7469 6f6e 206d 6f64 656c 730a 2d20 e29a  tion models.- ..
-000003e0: 99ef b88f 2045 7870 6f73 6573 2061 2073  .... Exposes a s
-000003f0: 696d 706c 6520 4150 4920 746f 2070 6c75  imple API to plu
-00000400: 6720 696e 2063 7573 746f 6d20 6d6f 6465  g in custom mode
-00000410: 6c73 2061 6e64 2061 6c67 6f72 6974 686d  ls and algorithm
-00000420: 730a 2d20 f09f 9388 2043 616e 2062 6520  s.- .... Can be 
-00000430: 7573 6564 2074 6f20 6265 6e63 686d 6172  used to benchmar
-00000440: 6b20 636f 6d70 6f6e 656e 7473 206f 6620  k components of 
-00000450: 6120 7265 7472 6f73 796e 7468 6573 6973  a retrosynthesis
-00000460: 2070 6970 656c 696e 650a 0a54 6f20 6c65   pipeline..To le
-00000470: 6172 6e20 6162 6f75 7420 6073 796e 7468  arn about `synth
-00000480: 6573 6575 7360 2773 2066 6561 7475 7265  eseus`'s feature
-00000490: 7320 616e 6420 4150 4920 7669 7369 7420  s and API visit 
-000004a0: 5b6d 6963 726f 736f 6674 2e67 6974 6875  [microsoft.githu
-000004b0: 622e 696f 2f73 796e 7468 6573 6575 735d  b.io/syntheseus]
-000004c0: 2868 7474 7073 3a2f 2f6d 6963 726f 736f  (https://microso
-000004d0: 6674 2e67 6974 6875 622e 696f 2f73 796e  ft.github.io/syn
-000004e0: 7468 6573 6575 7329 2e0a 0a23 2320 5175  theseus)...## Qu
-000004f0: 6963 6b20 5374 6172 740a 0a54 6f20 696e  ick Start..To in
-00000500: 7374 616c 6c20 6073 796e 7468 6573 6575  stall `syntheseu
-00000510: 7360 2077 6974 6820 616c 6c20 7468 6520  s` with all the 
-00000520: 6578 7472 6173 2c20 7275 6e0a 0a60 6060  extras, run..```
-00000530: 6261 7368 0a63 6f6e 6461 2065 6e76 2063  bash.conda env c
-00000540: 7265 6174 6520 2d66 2065 6e76 6972 6f6e  reate -f environ
-00000550: 6d65 6e74 5f66 756c 6c2e 796d 6c0a 636f  ment_full.yml.co
-00000560: 6e64 6120 6163 7469 7661 7465 2073 796e  nda activate syn
-00000570: 7468 6573 6575 732d 6675 6c6c 0a0a 7069  theseus-full..pi
-00000580: 7020 696e 7374 616c 6c20 2d65 2022 2e5b  p install -e ".[
-00000590: 616c 6c5d 220a 6060 600a 0a53 6565 205b  all]".```..See [
-000005a0: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-000005b0: 7474 7073 3a2f 2f6d 6963 726f 736f 6674  ttps://microsoft
-000005c0: 2e67 6974 6875 622e 696f 2f73 796e 7468  .github.io/synth
-000005d0: 6573 6575 732f 696e 7374 616c 6c61 7469  eseus/installati
-000005e0: 6f6e 2920 6966 2079 6f75 2070 7265 6665  on) if you prefe
-000005f0: 7220 6120 6d6f 7265 206c 6967 6874 7765  r a more lightwe
-00000600: 6967 6874 2069 6e73 7461 6c6c 6174 696f  ight installatio
-00000610: 6e20 7468 6174 206f 6e6c 7920 696e 636c  n that only incl
-00000620: 7564 6573 2074 6865 2070 6172 7473 2079  udes the parts y
-00000630: 6f75 2061 6374 7561 6c6c 7920 6e65 6564  ou actually need
-00000640: 2e0a 0a23 2320 4465 7665 6c6f 706d 656e  ...## Developmen
-00000650: 740a 0a53 796e 7468 6573 6575 7320 6973  t..Syntheseus is
-00000660: 2063 7572 7265 6e74 6c79 2075 6e64 6572   currently under
-00000670: 2061 6374 6976 6520 6465 7665 6c6f 706d   active developm
-00000680: 656e 742e 0a49 6620 796f 7520 7761 6e74  ent..If you want
-00000690: 2074 6f20 6865 6c70 2075 7320 6465 7665   to help us deve
-000006a0: 6c6f 7020 7379 6e74 6865 7365 7573 2070  lop syntheseus p
-000006b0: 6c65 6173 6520 696e 7374 616c 6c20 616e  lease install an
-000006c0: 6420 7275 6e20 6070 7265 2d63 6f6d 6d69  d run `pre-commi
-000006d0: 7460 0a63 6865 636b 7320 6265 666f 7265  t`.checks before
-000006e0: 2063 6f6d 6d69 7474 696e 6720 636f 6465   committing code
-000006f0: 2e0a 0a57 6520 7573 6520 6070 7974 6573  ...We use `pytes
-00000700: 7460 2066 6f72 2074 6573 7469 6e67 2e20  t` for testing. 
-00000710: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
-00000720: 2074 6573 7473 2070 6173 7320 6f6e 2079   tests pass on y
-00000730: 6f75 7220 6272 616e 6368 2062 6566 6f72  our branch befor
-00000740: 650a 7375 626d 6974 7469 6e67 2061 2050  e.submitting a P
-00000750: 5220 2861 6e64 2074 7279 2074 6f20 6d61  R (and try to ma
-00000760: 696e 7461 696e 2068 6967 6820 7465 7374  intain high test
-00000770: 2063 6f76 6572 6167 6529 2e0a 0a60 6060   coverage)...```
-00000780: 6261 7368 0a70 7974 686f 6e20 2d6d 2070  bash.python -m p
-00000790: 7974 6573 7420 2d2d 636f 7620 7379 6e74  ytest --cov synt
-000007a0: 6865 7365 7573 2f74 6573 7473 0a60 6060  heseus/tests.```
-000007b0: 0a0a 2323 2043 6f6e 7472 6962 7574 696e  ..## Contributin
-000007c0: 670a 0a54 6869 7320 7072 6f6a 6563 7420  g..This project 
-000007d0: 7765 6c63 6f6d 6573 2063 6f6e 7472 6962  welcomes contrib
-000007e0: 7574 696f 6e73 2061 6e64 2073 7567 6765  utions and sugge
-000007f0: 7374 696f 6e73 2e20 204d 6f73 7420 636f  stions.  Most co
-00000800: 6e74 7269 6275 7469 6f6e 7320 7265 7175  ntributions requ
-00000810: 6972 6520 796f 7520 746f 2061 6772 6565  ire you to agree
-00000820: 2074 6f20 610a 436f 6e74 7269 6275 746f   to a.Contributo
-00000830: 7220 4c69 6365 6e73 6520 4167 7265 656d  r License Agreem
-00000840: 656e 7420 2843 4c41 2920 6465 636c 6172  ent (CLA) declar
-00000850: 696e 6720 7468 6174 2079 6f75 2068 6176  ing that you hav
-00000860: 6520 7468 6520 7269 6768 7420 746f 2c20  e the right to, 
-00000870: 616e 6420 6163 7475 616c 6c79 2064 6f2c  and actually do,
-00000880: 2067 7261 6e74 2075 730a 7468 6520 7269   grant us.the ri
-00000890: 6768 7473 2074 6f20 7573 6520 796f 7572  ghts to use your
-000008a0: 2063 6f6e 7472 6962 7574 696f 6e2e 2046   contribution. F
-000008b0: 6f72 2064 6574 6169 6c73 2c20 7669 7369  or details, visi
-000008c0: 7420 6874 7470 733a 2f2f 636c 612e 6f70  t https://cla.op
-000008d0: 656e 736f 7572 6365 2e6d 6963 726f 736f  ensource.microso
-000008e0: 6674 2e63 6f6d 2e0a 0a57 6865 6e20 796f  ft.com...When yo
-000008f0: 7520 7375 626d 6974 2061 2070 756c 6c20  u submit a pull 
-00000900: 7265 7175 6573 742c 2061 2043 4c41 2062  request, a CLA b
-00000910: 6f74 2077 696c 6c20 6175 746f 6d61 7469  ot will automati
-00000920: 6361 6c6c 7920 6465 7465 726d 696e 6520  cally determine 
-00000930: 7768 6574 6865 7220 796f 7520 6e65 6564  whether you need
-00000940: 2074 6f20 7072 6f76 6964 650a 6120 434c   to provide.a CL
-00000950: 4120 616e 6420 6465 636f 7261 7465 2074  A and decorate t
-00000960: 6865 2050 5220 6170 7072 6f70 7269 6174  he PR appropriat
-00000970: 656c 7920 2865 2e67 2e2c 2073 7461 7475  ely (e.g., statu
-00000980: 7320 6368 6563 6b2c 2063 6f6d 6d65 6e74  s check, comment
-00000990: 292e 2053 696d 706c 7920 666f 6c6c 6f77  ). Simply follow
-000009a0: 2074 6865 2069 6e73 7472 7563 7469 6f6e   the instruction
-000009b0: 730a 7072 6f76 6964 6564 2062 7920 7468  s.provided by th
-000009c0: 6520 626f 742e 2059 6f75 2077 696c 6c20  e bot. You will 
-000009d0: 6f6e 6c79 206e 6565 6420 746f 2064 6f20  only need to do 
-000009e0: 7468 6973 206f 6e63 6520 6163 726f 7373  this once across
-000009f0: 2061 6c6c 2072 6570 6f73 2075 7369 6e67   all repos using
-00000a00: 206f 7572 2043 4c41 2e0a 0a54 6869 7320   our CLA...This 
-00000a10: 7072 6f6a 6563 7420 6861 7320 6164 6f70  project has adop
-00000a20: 7465 6420 7468 6520 5b4d 6963 726f 736f  ted the [Microso
-00000a30: 6674 204f 7065 6e20 536f 7572 6365 2043  ft Open Source C
-00000a40: 6f64 6520 6f66 2043 6f6e 6475 6374 5d28  ode of Conduct](
-00000a50: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00000a60: 6365 2e6d 6963 726f 736f 6674 2e63 6f6d  ce.microsoft.com
-00000a70: 2f63 6f64 656f 6663 6f6e 6475 6374 2f29  /codeofconduct/)
-00000a80: 2e0a 466f 7220 6d6f 7265 2069 6e66 6f72  ..For more infor
-00000a90: 6d61 7469 6f6e 2073 6565 2074 6865 205b  mation see the [
-00000aa0: 436f 6465 206f 6620 436f 6e64 7563 7420  Code of Conduct 
-00000ab0: 4641 515d 2868 7474 7073 3a2f 2f6f 7065  FAQ](https://ope
-00000ac0: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
-00000ad0: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
-00000ae0: 7563 742f 6661 712f 2920 6f72 0a63 6f6e  uct/faq/) or.con
-00000af0: 7461 6374 205b 6f70 656e 636f 6465 406d  tact [opencode@m
-00000b00: 6963 726f 736f 6674 2e63 6f6d 5d28 6d61  icrosoft.com](ma
-00000b10: 696c 746f 3a6f 7065 6e63 6f64 6540 6d69  ilto:opencode@mi
-00000b20: 6372 6f73 6f66 742e 636f 6d29 2077 6974  crosoft.com) wit
-00000b30: 6820 616e 7920 6164 6469 7469 6f6e 616c  h any additional
-00000b40: 2071 7565 7374 696f 6e73 206f 7220 636f   questions or co
-00000b50: 6d6d 656e 7473 2e0a 0a23 2320 5472 6164  mments...## Trad
-00000b60: 656d 6172 6b73 0a0a 5468 6973 2070 726f  emarks..This pro
-00000b70: 6a65 6374 206d 6179 2063 6f6e 7461 696e  ject may contain
-00000b80: 2074 7261 6465 6d61 726b 7320 6f72 206c   trademarks or l
-00000b90: 6f67 6f73 2066 6f72 2070 726f 6a65 6374  ogos for project
-00000ba0: 732c 2070 726f 6475 6374 732c 206f 7220  s, products, or 
-00000bb0: 7365 7276 6963 6573 2e20 4175 7468 6f72  services. Author
-00000bc0: 697a 6564 2075 7365 206f 6620 4d69 6372  ized use of Micr
-00000bd0: 6f73 6f66 740a 7472 6164 656d 6172 6b73  osoft.trademarks
-00000be0: 206f 7220 6c6f 676f 7320 6973 2073 7562   or logos is sub
-00000bf0: 6a65 6374 2074 6f20 616e 6420 6d75 7374  ject to and must
-00000c00: 2066 6f6c 6c6f 770a 5b4d 6963 726f 736f   follow.[Microso
-00000c10: 6674 2773 2054 7261 6465 6d61 726b 2026  ft's Trademark &
-00000c20: 2042 7261 6e64 2047 7569 6465 6c69 6e65   Brand Guideline
-00000c30: 735d 2868 7474 7073 3a2f 2f77 7777 2e6d  s](https://www.m
-00000c40: 6963 726f 736f 6674 2e63 6f6d 2f65 6e2d  icrosoft.com/en-
-00000c50: 7573 2f6c 6567 616c 2f69 6e74 656c 6c65  us/legal/intelle
-00000c60: 6374 7561 6c70 726f 7065 7274 792f 7472  ctualproperty/tr
-00000c70: 6164 656d 6172 6b73 2f75 7361 6765 2f67  ademarks/usage/g
-00000c80: 656e 6572 616c 292e 0a55 7365 206f 6620  eneral)..Use of 
-00000c90: 4d69 6372 6f73 6f66 7420 7472 6164 656d  Microsoft tradem
-00000ca0: 6172 6b73 206f 7220 6c6f 676f 7320 696e  arks or logos in
-00000cb0: 206d 6f64 6966 6965 6420 7665 7273 696f   modified versio
-00000cc0: 6e73 206f 6620 7468 6973 2070 726f 6a65  ns of this proje
-00000cd0: 6374 206d 7573 7420 6e6f 7420 6361 7573  ct must not caus
-00000ce0: 6520 636f 6e66 7573 696f 6e20 6f72 2069  e confusion or i
-00000cf0: 6d70 6c79 204d 6963 726f 736f 6674 2073  mply Microsoft s
-00000d00: 706f 6e73 6f72 7368 6970 2e0a 416e 7920  ponsorship..Any 
-00000d10: 7573 6520 6f66 2074 6869 7264 2d70 6172  use of third-par
-00000d20: 7479 2074 7261 6465 6d61 726b 7320 6f72  ty trademarks or
-00000d30: 206c 6f67 6f73 2061 7265 2073 7562 6a65   logos are subje
-00000d40: 6374 2074 6f20 7468 6f73 6520 7468 6972  ct to those thir
-00000d50: 642d 7061 7274 7927 7320 706f 6c69 6369  d-party's polici
-00000d60: 6573 2e0a                                es..
+000000d0: 333e 0a0a 2d2d 2d0a 0a3c 7020 616c 6967  3>..---..<p alig
+000000e0: 6e3d 2263 656e 7465 7222 3e0a 2020 3c61  n="center">.  <a
+000000f0: 2068 7265 663d 2268 7474 7073 3a2f 2f6d   href="https://m
+00000100: 6963 726f 736f 6674 2e67 6974 6875 622e  icrosoft.github.
+00000110: 696f 2f73 796e 7468 6573 6575 732f 7374  io/syntheseus/st
+00000120: 6162 6c65 223e 446f 6373 3c2f 613e 20e2  able">Docs</a> .
+00000130: 80a2 0a20 203c 6120 6872 6566 3d22 6874  ...  <a href="ht
+00000140: 7470 733a 2f2f 6d69 6372 6f73 6f66 742e  tps://microsoft.
+00000150: 6769 7468 7562 2e69 6f2f 7379 6e74 6865  github.io/synthe
+00000160: 7365 7573 2f73 7461 626c 652f 636c 692f  seus/stable/cli/
+00000170: 6576 616c 5f73 696e 676c 655f 7374 6570  eval_single_step
+00000180: 2f22 3e43 4c49 3c2f 613e 20e2 80a2 0a20  /">CLI</a> .... 
+00000190: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
+000001a0: 2f2f 6d69 6372 6f73 6f66 742e 6769 7468  //microsoft.gith
+000001b0: 7562 2e69 6f2f 7379 6e74 6865 7365 7573  ub.io/syntheseus
+000001c0: 2f73 7461 626c 652f 7475 746f 7269 616c  /stable/tutorial
+000001d0: 732f 7175 6963 6b5f 7374 6172 742f 223e  s/quick_start/">
+000001e0: 5475 746f 7269 616c 733c 2f61 3e20 e280  Tutorials</a> ..
+000001f0: a20a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+00000200: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000210: 6273 2f32 3331 302e 3139 3739 3622 3e50  bs/2310.19796">P
+00000220: 6170 6572 3c2f 613e 0a3c 2f70 3e0a 0a5b  aper</a>.</p>..[
+00000230: 215b 4349 5d28 6874 7470 733a 2f2f 6769  ![CI](https://gi
+00000240: 7468 7562 2e63 6f6d 2f6d 6963 726f 736f  thub.com/microso
+00000250: 6674 2f73 796e 7468 6573 6575 732f 6163  ft/syntheseus/ac
+00000260: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000270: 6369 2e79 6d6c 2f62 6164 6765 2e73 7667  ci.yml/badge.svg
+00000280: 3f62 7261 6e63 683d 6d61 696e 295d 2868  ?branch=main)](h
+00000290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002a0: 6d2f 6d69 6372 6f73 6f66 742f 7379 6e74  m/microsoft/synt
+000002b0: 6865 7365 7573 2f61 6374 696f 6e73 2f77  heseus/actions/w
+000002c0: 6f72 6b66 6c6f 7773 2f63 692e 796d 6c29  orkflows/ci.yml)
+000002d0: 0a5b 215b 5079 7468 6f6e 2056 6572 7369  .[![Python Versi
+000002e0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
+000002f0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000300: 2f70 7974 686f 6e2d 332e 372b 2d62 6c75  /python-3.7+-blu
+00000310: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000320: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
+00000330: 6f77 6e6c 6f61 6473 2f29 0a5b 215b 7079  ownloads/).[![py
+00000340: 7069 5d28 6874 7470 733a 2f2f 696d 672e  pi](https://img.
+00000350: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000360: 762f 7379 6e74 6865 7365 7573 2e73 7667  v/syntheseus.svg
+00000370: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
+00000380: 6f72 672f 7072 6f6a 6563 742f 7379 6e74  org/project/synt
+00000390: 6865 7365 7573 2f29 0a5b 215b 636f 6465  heseus/).[![code
+000003a0: 2073 7479 6c65 5d28 6874 7470 733a 2f2f   style](https://
+000003b0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000003c0: 6164 6765 2f63 6f64 6525 3230 7374 796c  adge/code%20styl
+000003d0: 652d 626c 6163 6b2d 3230 3230 3230 2e73  e-black-202020.s
+000003e0: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+000003f0: 6875 622e 636f 6d2f 616d 6276 2f62 6c61  hub.com/ambv/bla
+00000400: 636b 290a 5b21 5b4c 6963 656e 7365 5d28  ck).[![License](
+00000410: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000420: 6c64 732e 696f 2f62 6164 6765 2f6c 6963  lds.io/badge/lic
+00000430: 656e 7365 2d4d 4954 2d67 7265 656e 2e73  ense-MIT-green.s
+00000440: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000450: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
+00000460: 742f 7379 6e74 6865 7365 7573 2f62 6c6f  t/syntheseus/blo
+00000470: 622f 6d61 696e 2f4c 4943 454e 5345 290a  b/main/LICENSE).
+00000480: 0a3c 2f64 6976 3e0a 0a23 2320 4f76 6572  .</div>..## Over
+00000490: 7669 6577 0a0a 5379 6e74 6865 7365 7573  view..Syntheseus
+000004a0: 2069 7320 6120 7061 636b 6167 6520 666f   is a package fo
+000004b0: 7220 656e 642d 746f 2d65 6e64 2072 6574  r end-to-end ret
+000004c0: 726f 7379 6e74 6865 7469 6320 706c 616e  rosynthetic plan
+000004d0: 6e69 6e67 2e0a 2d20 e29a 92ef b88f 2043  ning..- ...... C
+000004e0: 6f6d 6269 6e65 7320 7365 6172 6368 2061  ombines search a
+000004f0: 6c67 6f72 6974 686d 7320 616e 6420 7265  lgorithms and re
+00000500: 6163 7469 6f6e 206d 6f64 656c 7320 696e  action models in
+00000510: 2061 2073 7461 6e64 6172 6469 7a65 6420   a standardized 
+00000520: 7761 790a 2d20 f09f a7ad 2049 6e63 6c75  way.- .... Inclu
+00000530: 6465 7320 696d 706c 656d 656e 7461 7469  des implementati
+00000540: 6f6e 7320 6f66 2063 6f6d 6d6f 6e20 7365  ons of common se
+00000550: 6172 6368 2061 6c67 6f72 6974 686d 730a  arch algorithms.
+00000560: 2d20 f09f a7aa 2049 6e63 6c75 6465 7320  - .... Includes 
+00000570: 7772 6170 7065 7273 2066 6f72 2073 7461  wrappers for sta
+00000580: 7465 2d6f 662d 7468 652d 6172 7420 7265  te-of-the-art re
+00000590: 6163 7469 6f6e 206d 6f64 656c 730a 2d20  action models.- 
+000005a0: e29a 99ef b88f 2045 7870 6f73 6573 2061  ...... Exposes a
+000005b0: 2073 696d 706c 6520 4150 4920 746f 2070   simple API to p
+000005c0: 6c75 6720 696e 2063 7573 746f 6d20 6d6f  lug in custom mo
+000005d0: 6465 6c73 2061 6e64 2061 6c67 6f72 6974  dels and algorit
+000005e0: 686d 730a 2d20 f09f 9388 2043 616e 2062  hms.- .... Can b
+000005f0: 6520 7573 6564 2074 6f20 6265 6e63 686d  e used to benchm
+00000600: 6172 6b20 636f 6d70 6f6e 656e 7473 206f  ark components o
+00000610: 6620 6120 7265 7472 6f73 796e 7468 6573  f a retrosynthes
+00000620: 6973 2070 6970 656c 696e 650a 0a23 2320  is pipeline..## 
+00000630: 5175 6963 6b20 5374 6172 740a 0a54 6f20  Quick Start..To 
+00000640: 696e 7374 616c 6c20 6073 796e 7468 6573  install `synthes
+00000650: 6575 7360 2077 6974 6820 616c 6c20 7468  eus` with all th
+00000660: 6520 6578 7472 6173 2c20 7275 6e0a 0a60  e extras, run..`
+00000670: 6060 6261 7368 0a63 6f6e 6461 2065 6e76  ``bash.conda env
+00000680: 2063 7265 6174 6520 2d66 2065 6e76 6972   create -f envir
+00000690: 6f6e 6d65 6e74 5f66 756c 6c2e 796d 6c0a  onment_full.yml.
+000006a0: 636f 6e64 6120 6163 7469 7661 7465 2073  conda activate s
+000006b0: 796e 7468 6573 6575 732d 6675 6c6c 0a0a  yntheseus-full..
+000006c0: 7069 7020 696e 7374 616c 6c20 2273 796e  pip install "syn
+000006d0: 7468 6573 6575 735b 616c 6c5d 220a 6060  theseus[all]".``
+000006e0: 600a 0a53 6565 205b 6865 7265 5d28 6874  `..See [here](ht
+000006f0: 7470 733a 2f2f 6d69 6372 6f73 6f66 742e  tps://microsoft.
+00000700: 6769 7468 7562 2e69 6f2f 7379 6e74 6865  github.io/synthe
+00000710: 7365 7573 2f69 6e73 7461 6c6c 6174 696f  seus/installatio
+00000720: 6e29 2069 6620 796f 7520 7072 6566 6572  n) if you prefer
+00000730: 2061 206d 6f72 6520 6c69 6768 7477 6569   a more lightwei
+00000740: 6768 7420 696e 7374 616c 6c61 7469 6f6e  ght installation
+00000750: 2074 6861 7420 6f6e 6c79 2069 6e63 6c75   that only inclu
+00000760: 6465 7320 7468 6520 7061 7274 7320 796f  des the parts yo
+00000770: 7520 6163 7475 616c 6c79 206e 6565 642e  u actually need.
+00000780: 0a0a 2323 2044 6576 656c 6f70 6d65 6e74  ..## Development
+00000790: 0a0a 5379 6e74 6865 7365 7573 2069 7320  ..Syntheseus is 
+000007a0: 6375 7272 656e 746c 7920 756e 6465 7220  currently under 
+000007b0: 6163 7469 7665 2064 6576 656c 6f70 6d65  active developme
+000007c0: 6e74 2e0a 4966 2079 6f75 2077 616e 7420  nt..If you want 
+000007d0: 746f 2068 656c 7020 7573 2064 6576 656c  to help us devel
+000007e0: 6f70 2073 796e 7468 6573 6575 7320 706c  op syntheseus pl
+000007f0: 6561 7365 2069 6e73 7461 6c6c 2061 6e64  ease install and
+00000800: 2072 756e 2060 7072 652d 636f 6d6d 6974   run `pre-commit
+00000810: 600a 6368 6563 6b73 2062 6566 6f72 6520  `.checks before 
+00000820: 636f 6d6d 6974 7469 6e67 2063 6f64 652e  committing code.
+00000830: 0a0a 5765 2075 7365 2060 7079 7465 7374  ..We use `pytest
+00000840: 6020 666f 7220 7465 7374 696e 672e 2050  ` for testing. P
+00000850: 6c65 6173 6520 6d61 6b65 2073 7572 6520  lease make sure 
+00000860: 7465 7374 7320 7061 7373 206f 6e20 796f  tests pass on yo
+00000870: 7572 2062 7261 6e63 6820 6265 666f 7265  ur branch before
+00000880: 0a73 7562 6d69 7474 696e 6720 6120 5052  .submitting a PR
+00000890: 2028 616e 6420 7472 7920 746f 206d 6169   (and try to mai
+000008a0: 6e74 6169 6e20 6869 6768 2074 6573 7420  ntain high test 
+000008b0: 636f 7665 7261 6765 292e 0a0a 6060 6062  coverage)...```b
+000008c0: 6173 680a 7079 7468 6f6e 202d 6d20 7079  ash.python -m py
+000008d0: 7465 7374 202d 2d63 6f76 2073 796e 7468  test --cov synth
+000008e0: 6573 6575 732f 7465 7374 730a 6060 600a  eseus/tests.```.
+000008f0: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00000900: 0a0a 5468 6973 2070 726f 6a65 6374 2077  ..This project w
+00000910: 656c 636f 6d65 7320 636f 6e74 7269 6275  elcomes contribu
+00000920: 7469 6f6e 7320 616e 6420 7375 6767 6573  tions and sugges
+00000930: 7469 6f6e 732e 2020 4d6f 7374 2063 6f6e  tions.  Most con
+00000940: 7472 6962 7574 696f 6e73 2072 6571 7569  tributions requi
+00000950: 7265 2079 6f75 2074 6f20 6167 7265 6520  re you to agree 
+00000960: 746f 2061 0a43 6f6e 7472 6962 7574 6f72  to a.Contributor
+00000970: 204c 6963 656e 7365 2041 6772 6565 6d65   License Agreeme
+00000980: 6e74 2028 434c 4129 2064 6563 6c61 7269  nt (CLA) declari
+00000990: 6e67 2074 6861 7420 796f 7520 6861 7665  ng that you have
+000009a0: 2074 6865 2072 6967 6874 2074 6f2c 2061   the right to, a
+000009b0: 6e64 2061 6374 7561 6c6c 7920 646f 2c20  nd actually do, 
+000009c0: 6772 616e 7420 7573 0a74 6865 2072 6967  grant us.the rig
+000009d0: 6874 7320 746f 2075 7365 2079 6f75 7220  hts to use your 
+000009e0: 636f 6e74 7269 6275 7469 6f6e 2e20 466f  contribution. Fo
+000009f0: 7220 6465 7461 696c 732c 2076 6973 6974  r details, visit
+00000a00: 2068 7474 7073 3a2f 2f63 6c61 2e6f 7065   https://cla.ope
+00000a10: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
+00000a20: 742e 636f 6d2e 0a0a 5768 656e 2079 6f75  t.com...When you
+00000a30: 2073 7562 6d69 7420 6120 7075 6c6c 2072   submit a pull r
+00000a40: 6571 7565 7374 2c20 6120 434c 4120 626f  equest, a CLA bo
+00000a50: 7420 7769 6c6c 2061 7574 6f6d 6174 6963  t will automatic
+00000a60: 616c 6c79 2064 6574 6572 6d69 6e65 2077  ally determine w
+00000a70: 6865 7468 6572 2079 6f75 206e 6565 6420  hether you need 
+00000a80: 746f 2070 726f 7669 6465 0a61 2043 4c41  to provide.a CLA
+00000a90: 2061 6e64 2064 6563 6f72 6174 6520 7468   and decorate th
+00000aa0: 6520 5052 2061 7070 726f 7072 6961 7465  e PR appropriate
+00000ab0: 6c79 2028 652e 672e 2c20 7374 6174 7573  ly (e.g., status
+00000ac0: 2063 6865 636b 2c20 636f 6d6d 656e 7429   check, comment)
+00000ad0: 2e20 5369 6d70 6c79 2066 6f6c 6c6f 7720  . Simply follow 
+00000ae0: 7468 6520 696e 7374 7275 6374 696f 6e73  the instructions
+00000af0: 0a70 726f 7669 6465 6420 6279 2074 6865  .provided by the
+00000b00: 2062 6f74 2e20 596f 7520 7769 6c6c 206f   bot. You will o
+00000b10: 6e6c 7920 6e65 6564 2074 6f20 646f 2074  nly need to do t
+00000b20: 6869 7320 6f6e 6365 2061 6372 6f73 7320  his once across 
+00000b30: 616c 6c20 7265 706f 7320 7573 696e 6720  all repos using 
+00000b40: 6f75 7220 434c 412e 0a0a 5468 6973 2070  our CLA...This p
+00000b50: 726f 6a65 6374 2068 6173 2061 646f 7074  roject has adopt
+00000b60: 6564 2074 6865 205b 4d69 6372 6f73 6f66  ed the [Microsof
+00000b70: 7420 4f70 656e 2053 6f75 7263 6520 436f  t Open Source Co
+00000b80: 6465 206f 6620 436f 6e64 7563 745d 2868  de of Conduct](h
+00000b90: 7474 7073 3a2f 2f6f 7065 6e73 6f75 7263  ttps://opensourc
+00000ba0: 652e 6d69 6372 6f73 6f66 742e 636f 6d2f  e.microsoft.com/
+00000bb0: 636f 6465 6f66 636f 6e64 7563 742f 292e  codeofconduct/).
+00000bc0: 0a46 6f72 206d 6f72 6520 696e 666f 726d  .For more inform
+00000bd0: 6174 696f 6e20 7365 6520 7468 6520 5b43  ation see the [C
+00000be0: 6f64 6520 6f66 2043 6f6e 6475 6374 2046  ode of Conduct F
+00000bf0: 4151 5d28 6874 7470 733a 2f2f 6f70 656e  AQ](https://open
+00000c00: 736f 7572 6365 2e6d 6963 726f 736f 6674  source.microsoft
+00000c10: 2e63 6f6d 2f63 6f64 656f 6663 6f6e 6475  .com/codeofcondu
+00000c20: 6374 2f66 6171 2f29 206f 720a 636f 6e74  ct/faq/) or.cont
+00000c30: 6163 7420 5b6f 7065 6e63 6f64 6540 6d69  act [opencode@mi
+00000c40: 6372 6f73 6f66 742e 636f 6d5d 286d 6169  crosoft.com](mai
+00000c50: 6c74 6f3a 6f70 656e 636f 6465 406d 6963  lto:opencode@mic
+00000c60: 726f 736f 6674 2e63 6f6d 2920 7769 7468  rosoft.com) with
+00000c70: 2061 6e79 2061 6464 6974 696f 6e61 6c20   any additional 
+00000c80: 7175 6573 7469 6f6e 7320 6f72 2063 6f6d  questions or com
+00000c90: 6d65 6e74 732e 0a0a 2323 2054 7261 6465  ments...## Trade
+00000ca0: 6d61 726b 730a 0a54 6869 7320 7072 6f6a  marks..This proj
+00000cb0: 6563 7420 6d61 7920 636f 6e74 6169 6e20  ect may contain 
+00000cc0: 7472 6164 656d 6172 6b73 206f 7220 6c6f  trademarks or lo
+00000cd0: 676f 7320 666f 7220 7072 6f6a 6563 7473  gos for projects
+00000ce0: 2c20 7072 6f64 7563 7473 2c20 6f72 2073  , products, or s
+00000cf0: 6572 7669 6365 732e 2041 7574 686f 7269  ervices. Authori
+00000d00: 7a65 6420 7573 6520 6f66 204d 6963 726f  zed use of Micro
+00000d10: 736f 6674 0a74 7261 6465 6d61 726b 7320  soft.trademarks 
+00000d20: 6f72 206c 6f67 6f73 2069 7320 7375 626a  or logos is subj
+00000d30: 6563 7420 746f 2061 6e64 206d 7573 7420  ect to and must 
+00000d40: 666f 6c6c 6f77 0a5b 4d69 6372 6f73 6f66  follow.[Microsof
+00000d50: 7427 7320 5472 6164 656d 6172 6b20 2620  t's Trademark & 
+00000d60: 4272 616e 6420 4775 6964 656c 696e 6573  Brand Guidelines
+00000d70: 5d28 6874 7470 733a 2f2f 7777 772e 6d69  ](https://www.mi
+00000d80: 6372 6f73 6f66 742e 636f 6d2f 656e 2d75  crosoft.com/en-u
+00000d90: 732f 6c65 6761 6c2f 696e 7465 6c6c 6563  s/legal/intellec
+00000da0: 7475 616c 7072 6f70 6572 7479 2f74 7261  tualproperty/tra
+00000db0: 6465 6d61 726b 732f 7573 6167 652f 6765  demarks/usage/ge
+00000dc0: 6e65 7261 6c29 2e0a 5573 6520 6f66 204d  neral)..Use of M
+00000dd0: 6963 726f 736f 6674 2074 7261 6465 6d61  icrosoft tradema
+00000de0: 726b 7320 6f72 206c 6f67 6f73 2069 6e20  rks or logos in 
+00000df0: 6d6f 6469 6669 6564 2076 6572 7369 6f6e  modified version
+00000e00: 7320 6f66 2074 6869 7320 7072 6f6a 6563  s of this projec
+00000e10: 7420 6d75 7374 206e 6f74 2063 6175 7365  t must not cause
+00000e20: 2063 6f6e 6675 7369 6f6e 206f 7220 696d   confusion or im
+00000e30: 706c 7920 4d69 6372 6f73 6f66 7420 7370  ply Microsoft sp
+00000e40: 6f6e 736f 7273 6869 702e 0a41 6e79 2075  onsorship..Any u
+00000e50: 7365 206f 6620 7468 6972 642d 7061 7274  se of third-part
+00000e60: 7920 7472 6164 656d 6172 6b73 206f 7220  y trademarks or 
+00000e70: 6c6f 676f 7320 6172 6520 7375 626a 6563  logos are subjec
+00000e80: 7420 746f 2074 686f 7365 2074 6869 7264  t to those third
+00000e90: 2d70 6172 7479 2773 2070 6f6c 6963 6965  -party's policie
+00000ea0: 732e 0a                                  s..
```

### Comparing `syntheseus-0.3.0/SECURITY.md` & `syntheseus-0.4.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/docs/cli/eval_single_step.md` & `syntheseus-0.4.0/docs/cli/eval_single_step.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Single-step Evaluation
 
 ## Usage
 
-To run single-step model evaluation, run
-
 ```
 syntheseus eval-single-step \
     data_dir=[DATA_DIR] \
+    fold=[TRAIN, VAL or TEST] \
     model_class=[MODEL_CLASS] \
     model_dir=[MODEL_DIR]
 ```
 
-The script accepts further arguments to customize the evaluation such as which data fold to use; see `BaseEvalConfig` for the complete list.
+The `eval-single-step` command accepts further arguments to customize the evaluation; see `BaseEvalConfig` in `cli/eval_single_step.py` for the complete list.
 
 The code will scan `data_dir` looking for files matching `*{train, val, test}.{jsonl, csv, smi}` and select the right data format based on the file extension. An error will be raised in case of ambiguity. Only the fold that was selected for evaluation has to be present.
 
 ## Data format
 
 The single-step evaluation script supports reaction data in one of three formats.
```

### Comparing `syntheseus-0.3.0/docs/images/logo.png` & `syntheseus-0.4.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/docs/images/logo.svg` & `syntheseus-0.4.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/docs/index.md` & `syntheseus-0.4.0/docs/index.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
   <figcaption><h3>Navigating the labyrinth of synthesis planning</h3></figcaption>
 </figure>
 
 ---
 
 [![CI](https://github.com/microsoft/syntheseus/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/microsoft/syntheseus/actions/workflows/ci.yml)
 [![Python Version](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
+[![pypi](https://img.shields.io/pypi/v/syntheseus.svg)](https://pypi.org/project/syntheseus/)
 [![code style](https://img.shields.io/badge/code%20style-black-202020.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/microsoft/syntheseus/blob/main/LICENSE)
 
 Syntheseus is a package for end-to-end retrosynthetic planning.
 
 - ⚒️ Combines search algorithms and reaction models in a standardized way
 - 🧭 Includes implementations of common search algorithms
```

### Comparing `syntheseus-0.3.0/docs/installation.md` & `syntheseus-0.4.0/docs/installation.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,60 @@
 We support two installation modes:
 
 - *core installation* allows you to build and benchmark your own models or search algorithms
 - *full installation* also allows you to perform end-to-end search using the supported models
 
-=== "Core installation"
+There are also two installation sources:
+
+- *pip*, which provides the most recent released version
+- *GitHub*, which provides the latest changes but may be less stable and may not be
+  backward-compatible with the latest released version
+
+=== "Core (pip)"
+
+    ```bash
+    conda env create -f environment.yml
+    conda activate syntheseus
+
+    pip install syntheseus
+    ```
+
+=== "Full (pip)"
+
+    ```bash
+    conda env create -f environment_full.yml
+    conda activate syntheseus-full
+
+    pip install "syntheseus[all]"
+    ```
+
+=== "Core (GitHub)"
 
     ```bash
     conda env create -f environment.yml
     conda activate syntheseus
 
     pip install -e .
     ```
 
-=== "Full installation"
+=== "Full (GitHub)"
 
     ```bash
     conda env create -f environment_full.yml
     conda activate syntheseus-full
 
     pip install -e ".[all]"
     ```
 
+!!! note
+
+    Make sure you are viewing the version of the docs matching your `syntheseus` installation.
+    Select the `x.y.z` version you installed if you used `pip` (go [here](https://microsoft.github.io/syntheseus/stable/) for the latest one),
+    or [dev](https://microsoft.github.io/syntheseus/dev/) if you installed `syntheseus` directly from GitHub.
+
 Core installation includes only minimal dependencies (no ML libraries), while full installation includes all supported models and also dependencies for visualization/development.
 
 Instructions above assume you already cloned the repository via
 
 ```bash
 git clone https://github.com/microsoft/syntheseus.git
 cd syntheseus
```

### Comparing `syntheseus-0.3.0/docs/single_step.md` & `syntheseus-0.4.0/docs/single_step.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Syntheseus currently supports 7 established single-step models.
+Syntheseus currently supports 8 established single-step models.
 
 For convenience, for each model we include a default checkpoint trained on USPTO-50K.
 If no checkpoint directory is provided during model loading, `syntheseus` will automatically download a default checkpoint and cache it on disk for future use.
 The default path for the cache is `$HOME/.cache/torch/syntheseus`, but it can be overriden by setting the `SYNTHESEUS_CACHE_DIR` environment variable.
 See table below for the links to the default checkpoints.
 
 | Model checkpoint link                                          | Source |
 |----------------------------------------------------------------|--------|
 | [Chemformer](https://figshare.com/ndownloader/files/42009888)  | finetuned by us starting from checkpoint released by authors |
 | [GLN](https://figshare.com/ndownloader/files/42012720)         | released by authors |
+| [Graph2Edits](https://figshare.com/ndownloader/files/44194301) | released by authors |
 | [LocalRetro](https://figshare.com/ndownloader/files/42287319)  | trained by us |
 | [MEGAN](https://figshare.com/ndownloader/files/42012732)       | trained by us |
 | [MHNreact](https://figshare.com/ndownloader/files/42012777)    | trained by us |
 | [RetroKNN](https://figshare.com/ndownloader/files/43636584)    | trained by us |
 | [RootAligned](https://figshare.com/ndownloader/files/42012792) | released by authors |
 
 ??? note "More advanced datasets"
```

### Comparing `syntheseus-0.3.0/mkdocs.yml` & `syntheseus-0.4.0/mkdocs.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 site_name: Syntheseus
+site_url: https://microsoft.github.io/syntheseus/
 
 repo_name: microsoft/syntheseus
 repo_url: https://github.com/microsoft/syntheseus
 edit_uri: edit/main/docs/
 
 theme:
   name: material
@@ -28,16 +29,29 @@
 nav:
 - Get Started:
   - Overview: index.md
   - Installation: installation.md
   - Single-Step Models: single_step.md
 - CLI:
   - Single-Step Evaluation: cli/eval_single_step.md
+  - Running Search: cli/search.md
+- Tutorials:
+  - Quick Start: tutorials/quick_start.ipynb
+  - Integrating a Custom Model: tutorials/custom_model.ipynb
+  - Multi-step Search on PaRoutes: tutorials/paroutes_benchmark.ipynb
+
+plugins:
+  - mkdocs-jupyter
 
 markdown_extensions:
   - admonition
   - attr_list
   - md_in_html
   - pymdownx.details
   - pymdownx.superfences
   - pymdownx.tabbed:
       alternate_style: true
+
+extra:
+  version:
+    default: stable
+    provider: mike
```

### Comparing `syntheseus-0.3.0/pyproject.toml` & `syntheseus-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,23 @@
   "graphviz"
 ]
 dev = [
   "pytest",
   "pytest-cov",
   "pre-commit"
 ]
-chemformer = ["syntheseus-chemformer"]
-local-retro = ["syntheseus-local-retro"]
-megan = ["syntheseus-megan"]
-mhn-react = ["syntheseus-mhnreact"]
-retro-knn = ["syntheseus-local-retro", "torch-scatter"]
-root-aligned = ["syntheseus-root-aligned"]
+chemformer = ["syntheseus-chemformer==0.1.1"]
+graph2edits = ["syntheseus-graph2edits==0.2.0"]
+local-retro = ["syntheseus-local-retro==0.4.0"]
+megan = ["syntheseus-megan==0.1.0"]
+mhn-react = ["syntheseus-mhnreact==1.0.0"]
+retro-knn = ["syntheseus[local-retro]", "torch-scatter"]
+root-aligned = ["syntheseus-root-aligned==0.1.0"]
 all-single-step = [
-  "syntheseus[chemformer,local-retro,megan,mhn-react,retro-knn,root-aligned]"
+  "syntheseus[chemformer,graph2edits,local-retro,megan,mhn-react,retro-knn,root-aligned]"
 ]
 all = [
   "syntheseus[viz,dev,all-single-step]"
 ]
 
 [project.urls]
 Documentation = "https://microsoft.github.io/syntheseus"
@@ -74,20 +75,21 @@
 [tool.mypy]
 python_version = 3.9  # pin modern python version
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 100
 # Check https://beta.ruff.rs/docs/rules/ for full list of rules
-select = [
+lint.select = [
   "E", "W",  # pycodestyle
   "F",  # Pyflakes
   "I",  # isort
+  "NPY201",  # check for functions/constants deprecated in numpy 2.*
 ]
-ignore = [
+lint.ignore = [
   # W605: invalid escape sequence -- triggered by pseudo-LaTeX in comments
   "W605",
   # E501: Line too long -- triggered by comments and such. black deals with shortening.
   "E501",
   # E741:  Do not use variables named 'l', 'o', or 'i' -- disagree with PEP8
   "E741",
 ]
```

### Comparing `syntheseus-0.3.0/syntheseus/cli/eval_single_step.py` & `syntheseus-0.4.0/syntheseus/cli/eval_single_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,48 +18,60 @@
 import math
 import os
 import time
 from dataclasses import dataclass, field, fields
 from functools import partial
 from itertools import islice
 from statistics import mean, median
-from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Set, cast
+from typing import Any, Callable, Dict, Generic, Iterable, List, Optional, Sequence, Tuple, cast
 
 from more_itertools import batched
 from omegaconf import MISSING, OmegaConf
 from tqdm import tqdm
 
-from syntheseus.interface.bag import Bag
 from syntheseus.interface.models import (
+    ForwardReactionModel,
     InputType,
-    OutputType,
-    Prediction,
-    PredictionList,
     ReactionModel,
+    ReactionType,
 )
-from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import Reaction, SingleProductReaction
 from syntheseus.reaction_prediction.data.dataset import (
     DataFold,
     DiskReactionDataset,
     ReactionDataset,
 )
 from syntheseus.reaction_prediction.data.reaction_sample import ReactionSample
-from syntheseus.reaction_prediction.inference.config import BackwardModelConfig, ForwardModelConfig
-from syntheseus.reaction_prediction.utils.config import get_config as cli_get_config
+from syntheseus.reaction_prediction.inference.config import (
+    BackwardModelClass,
+    BackwardModelConfig,
+    ForwardModelConfig,
+)
+from syntheseus.reaction_prediction.utils.config import (
+    get_config as cli_get_config,
+)
+from syntheseus.reaction_prediction.utils.config import (
+    get_error_message_for_missing_value,
+)
 from syntheseus.reaction_prediction.utils.metrics import (
     ModelTimingResults,
     TopKMetricsAccumulator,
     compute_total_time,
 )
 from syntheseus.reaction_prediction.utils.misc import asdict_extended, set_random_seed
 from syntheseus.reaction_prediction.utils.model_loading import get_model
 
 logger = logging.getLogger(__file__)
 
 
+_RXN_WTIH_IDENTIFIER_ERROR = (
+    "Reactions with the `identifier` field currently not supported in evaluation"
+)
+
+
 @dataclass
 class BaseEvalConfig:
     data_dir: str = MISSING  # Directory containing preprocessed data
     num_top_results: int = 100  # Number of results to request from the model
     fold: DataFold = DataFold.TEST  # Dataset fold to evaluate on
     batch_size: int = 16  # Batch size to use
     skip_repeats: bool = True  # Whether repeated results should be skipped
@@ -86,16 +98,16 @@
 class EvalConfig(BackwardModelConfig, BaseEvalConfig):
     """Config for running evaluation on a given dataset."""
 
     pass
 
 
 @dataclass(frozen=True)
-class ModelResults(Generic[InputType, OutputType]):
-    results: List[PredictionList[InputType, OutputType]]
+class ModelResults(Generic[ReactionType]):
+    results: List[Sequence[ReactionType]]
     model_timing_results: Optional[ModelTimingResults] = None
 
 
 @dataclass(frozen=True)
 class EvalResults:
     eval_args: Dict[str, Any]
     model_info: Dict[str, Any]
@@ -107,40 +119,39 @@
     min_num_predictions: int
     max_num_predictions: int
     mean_num_predictions: float
     median_num_predictions: float
     model_time_total: ModelTimingResults
     back_translation_top_k: Optional[List[float]] = None
     back_translation_mrr: Optional[float] = None
-    predictions: Optional[List[PredictionList]] = None
-    back_translation_predictions: Optional[List[List[PredictionList]]] = None
+    predictions: Optional[List[Sequence[Reaction]]] = None
+    back_translation_predictions: Optional[List[List[Sequence[Reaction]]]] = None
     back_translation_time_total: Optional[ModelTimingResults] = None
 
 
 def get_results(
-    model: ReactionModel[InputType, OutputType],
+    model: ReactionModel[InputType, ReactionType],
     inputs: List[InputType],
     num_results: int,
-    skip_repeats: bool = True,
     measure_time: bool = False,
-) -> ModelResults[InputType, OutputType]:
+) -> ModelResults[ReactionType]:
     """Given a batch of inputs to the reaction model, return a batch of (possibly filtered) results.
 
     Args:
         model: Reaction model to use.
         inputs: Batch of inputs to the reaction model, each either a molecule or a set of molecules,
             depending on directionality.
         num_results: Number of results we want to try to obtain for each input.
-        skip_repeats: Whether repeated results should be skipped and not count towards
-            `num_results`.
         measure_time: Whether to measure time taken by the different parts of the code.
 
     Returns:
         A dataclass containing the model outputs and (optionally) time measurements.
     """
+
+    # Handle case of empty inputs without calling the model.
     if not inputs:
         return ModelResults(
             results=[],
             model_timing_results=(
                 ModelTimingResults(time_model_call=0, time_post_processing=0)
                 if measure_time
                 else None
@@ -154,74 +165,58 @@
 
     raw_batch_outputs = model(inputs, num_results=num_results)
 
     if measure_time:
         time_model_call_end = time.time()
         timing_results["time_model_call"] = time_model_call_end - time_model_call_start
 
-    batch_outputs: List[PredictionList[InputType, OutputType]] = []
+    batch_outputs: List[Sequence[ReactionType]] = []
 
     for outputs in raw_batch_outputs:
-        if len(outputs.predictions) > num_results:
-            raise ValueError(
-                f"Requested {num_results} results, but model produced {len(outputs.predictions)}"
-            )
-
-        seen_outputs: Set[OutputType] = set()
-        selected_predictions: List[Prediction[InputType, OutputType]] = []
-
-        for prediction in outputs.predictions:
-            if skip_repeats:
-                if prediction.output in seen_outputs:
-                    continue
-                seen_outputs.add(prediction.output)
-
-            selected_predictions.append(prediction)
-
-        if len(selected_predictions) < num_results:
-            logger.debug(
-                f"Tried to get {num_results} results, but only got {len(selected_predictions)}"
-            )
-
-        batch_outputs.append(
-            PredictionList(
-                input=outputs.input, predictions=selected_predictions, metadata=outputs.metadata
-            )
-        )
+        if len(outputs) > num_results:
+            raise ValueError(f"Requested {num_results} results, but model produced {len(outputs)}")
+
+        # Check identifiers are not set
+        if any(reaction.identifier is not None for reaction in outputs):
+            raise NotImplementedError(_RXN_WTIH_IDENTIFIER_ERROR)
+
+        # Check for length
+        if len(outputs) < num_results:
+            logger.debug(f"Tried to get {num_results} results, but only got {len(outputs)}")
+
+        batch_outputs.append(list(outputs))
 
     if measure_time:
         timing_results["time_post_processing"] = time.time() - time_model_call_end
 
     return ModelResults(
         results=batch_outputs,
         model_timing_results=ModelTimingResults(**timing_results) if measure_time else None,
     )
 
 
 def compute_metrics(
-    model: ReactionModel[InputType, OutputType],
+    model: ReactionModel[InputType, ReactionType],
     dataset: ReactionDataset,
     num_dataset_truncation: Optional[int],
     num_top_results: int,
-    back_translation_model: Optional[ReactionModel[OutputType, InputType]] = None,
+    back_translation_model: Optional[ForwardReactionModel] = None,
     back_translation_num_results: int = 1,
     fold: DataFold = DataFold.VALIDATION,
     batch_size: int = 16,
-    skip_repeats: bool = True,
     include_predictions: bool = False,
 ) -> EvalResults:
     """Compute top-k accuracies and Mean Reciprocal Rank of a model on a given dataset."""
 
     # Gather all evaluation args for the record.
     eval_args = {
         "model_class": model.__class__.__name__,
         "num_top_results": num_top_results,
         "fold": fold.name,
         "batch_size": batch_size,
-        "skip_repeats": skip_repeats,
     }
 
     ground_truth_match_metrics = TopKMetricsAccumulator(max_num_results=num_top_results)
 
     if back_translation_model is not None:
         eval_args.update(
             back_translation_model_class=back_translation_model.__class__.__name__,
@@ -234,16 +229,16 @@
         if not back_translation_model.is_forward():
             raise ValueError("Back translation model should be a forward model")
 
         back_translation_metrics = TopKMetricsAccumulator(max_num_results=num_top_results)
 
     print(f"Testing model {model.__class__.__name__} with args {eval_args}")
 
-    all_predictions: List[PredictionList] = []
-    all_back_translation_predictions: List[List[PredictionList]] = []
+    all_predictions: List[Sequence[Reaction]] = []
+    all_back_translation_predictions: List[List[Sequence[Reaction]]] = []
 
     model_timing_results: List[ModelTimingResults] = []
     back_translation_timing_results: List[ModelTimingResults] = []
 
     test_dataset: Iterable[ReactionSample] = dataset[fold]
     test_dataset_size = dataset.get_num_samples(fold)
 
@@ -257,66 +252,73 @@
         test_dataset = islice(test_dataset, num_dataset_truncation)
         test_dataset_size = num_dataset_truncation
 
     for batch in tqdm(
         batched(test_dataset, batch_size),
         total=math.ceil(test_dataset_size / batch_size),
     ):
+        # Tell mypy what the type of `batch` is as `batched` seems to lose it.
+        batch = cast(Tuple[ReactionSample], batch)
+
         inputs: List[InputType] = []
-        outputs: List[OutputType] = []
+        outputs: List[ReactionType] = []
 
         for sample in batch:
+            # We need to cast when appending to `inputs`/`outputs` because link between types and
+            # reaction models is unclear to mypy.
+
+            output: Reaction
             if model.is_forward():
                 inputs.append(sample.reactants)
-                outputs.append(sample.products)
+                output = Reaction(reactants=sample.reactants, products=sample.products)
             else:
-                num_products = len(sample.products)
-                if num_products > 1:
-                    raise ValueError(
-                        f"Model expected a single target product, got {len(sample.products)}"
-                    )
+                assert (
+                    len(sample.products) == 1
+                ), f"Model expected a single target product, got {len(sample.products)}"
+                [single_product] = sample.products
+
+                inputs.append(cast(InputType, single_product))
+                output = SingleProductReaction(reactants=sample.reactants, product=single_product)
 
-                inputs.append(list(sample.products)[0])
-                outputs.append(sample.reactants)
+            outputs.append(cast(ReactionType, output))
+            del output
 
         results_with_timing = get_results(
             model,
             inputs=inputs,
             num_results=num_top_results,
-            skip_repeats=skip_repeats,
             measure_time=True,
         )
 
         assert results_with_timing.model_timing_results is not None
         model_timing_results.append(results_with_timing.model_timing_results)
 
-        batch_predictions: List[PredictionList[InputType, OutputType]] = results_with_timing.results
+        batch_predictions: List[Sequence[ReactionType]] = results_with_timing.results
 
-        batch_back_translation_predictions: List[List[PredictionList]] = []
-        for input, output, prediction_list in zip(inputs, outputs, batch_predictions):
-            num_predictions.append(len(prediction_list.predictions))
-
-            ground_truth_matches = [
-                prediction.output == output for prediction in prediction_list.predictions
-            ]
+        batch_back_translation_predictions: List[List[Sequence[Reaction]]] = []
+        for input, output, reaction_list in zip(inputs, outputs, batch_predictions):
+            num_predictions.append(len(reaction_list))
+
+            # Check that the identifier field is not used in the evaluation,
+            # otherwise `==` below will not work as intended.
+            if output.identifier is not None:
+                raise NotImplementedError(_RXN_WTIH_IDENTIFIER_ERROR)
+            ground_truth_matches = [rxn == output for rxn in reaction_list]
             ground_truth_match_metrics.add(ground_truth_matches)
 
-            for prediction, ground_truth_match in zip(
-                prediction_list.predictions, ground_truth_matches
-            ):
-                prediction.metadata["ground_truth_match"] = ground_truth_match
+            for rxn, ground_truth_match in zip(reaction_list, ground_truth_matches):
+                rxn.metadata["ground_truth_match"] = ground_truth_match
 
             if back_translation_model is not None:
                 assert back_translation_metrics is not None
 
                 back_translation_results_with_timing = get_results(
                     back_translation_model,
-                    [prediction.output for prediction in prediction_list.predictions],
+                    [rxn.reactants for rxn in reaction_list],
                     num_results=back_translation_num_results,
-                    skip_repeats=False,
                     measure_time=True,
                 )
 
                 assert back_translation_results_with_timing.model_timing_results is not None
                 back_translation_timing_results.append(
                     back_translation_results_with_timing.model_timing_results
                 )
@@ -325,18 +327,15 @@
 
                 if include_predictions:
                     batch_back_translation_predictions.append(back_translation_results)
 
                 # Back translation is successful if any of the `back_translation_num_results` bags
                 # of products returned by the forward model contains the input.
                 back_translation_matches = [
-                    any(
-                        input in cast(Bag[Molecule], prediction.output)
-                        for prediction in result.predictions
-                    )
+                    any(input in rxn.products for rxn in result)
                     for result in back_translation_results
                 ]
 
                 back_translation_metrics.add(back_translation_matches)
 
         if include_predictions:
             all_predictions.extend(batch_predictions)
@@ -373,45 +372,48 @@
         median_num_predictions=float(median(num_predictions)),
         model_time_total=compute_total_time(model_timing_results),
         **extra_args,
     )
 
 
 def compute_metrics_from_config(
-    model: ReactionModel[InputType, OutputType],
+    model: ReactionModel[InputType, ReactionType],
     dataset: ReactionDataset,
-    back_translation_model: Optional[ReactionModel[OutputType, InputType]],
+    back_translation_model: Optional[ForwardReactionModel],
     config: BaseEvalConfig,
 ) -> EvalResults:
     """Variant of `compute_metrics` that uses an eval config instead of explicit arguments."""
 
     return compute_metrics(
         model,
         dataset=dataset,
         num_dataset_truncation=config.num_dataset_truncation,
         num_top_results=config.num_top_results,
         back_translation_model=back_translation_model,
         back_translation_num_results=config.back_translation_num_results,
         fold=config.fold,
         batch_size=config.batch_size,
-        skip_repeats=config.skip_repeats,
         include_predictions=config.include_predictions,
     )
 
 
 def print_and_save(results: EvalResults, config: EvalConfig, suffix: str = "") -> None:
     # Extract the top_k results for the chosen values of `k`; the other values are not printed.
     chosen_topk_results = {x: results.top_k[x - 1] for x in config.print_idxs}
 
     # Print the results in a concise form.
     for f in fields(results):
         if f.name not in ("model_info", "top_k", "predictions", "back_translation_predictions"):
             print(f"{f.name}: {getattr(results, f.name)}")
 
-    print(f"top_k results {suffix}:")
+    if suffix:
+        print(f"top_k results {suffix}:")
+    else:
+        print("top_k results:")
+
     for k, result in chosen_topk_results.items():
         print(f"{k}: {result}", flush=True)
 
     # Save the results into a json file, generate its name from the timestamp for uniqueness.
     if config.save_outputs:
         filestr = ("_" + config.filestring) if config.filestring else ""
         suffix = ("_" + suffix) if suffix else ""
@@ -434,21 +436,32 @@
     extra_steps: List[Callable[[ReactionModel, ReactionDataset, Optional[ReactionModel]], None]],
 ) -> None:
     set_random_seed(0)
 
     print("Running eval with the following config:")
     print(config)
 
+    if OmegaConf.is_missing(config, "data_dir"):
+        raise ValueError("data_dir should be set to a directory containing a reaction dataset")
+
+    if OmegaConf.is_missing(config, "model_class"):
+        raise ValueError(
+            get_error_message_for_missing_value("model_class", [c.name for c in BackwardModelClass])
+        )
+
     get_model_fn = partial(get_model, batch_size=config.batch_size, num_gpus=config.num_gpus)
-    model = get_model_fn(config)
+    model = get_model_fn(config, remove_duplicates=config.skip_repeats)
 
     if OmegaConf.is_missing(config.back_translation_config, "model_class"):
         back_translation_model = None
     else:
-        back_translation_model = get_model_fn(config.back_translation_config)
+        # Back translation model must be a forward model (checked in `compute_metrics`).
+        back_translation_model = cast(
+            ForwardReactionModel, get_model_fn(config.back_translation_config)
+        )
 
     dataset = DiskReactionDataset(config.data_dir, sample_cls=ReactionSample)
     results = compute_metrics_from_config(
         model=model, dataset=dataset, back_translation_model=back_translation_model, config=config
     )
     print_and_save(results, config)
```

### Comparing `syntheseus-0.3.0/syntheseus/cli/main.py` & `syntheseus-0.4.0/syntheseus/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 
 
 def main() -> None:
     supported_commands = {"search": search.main, "eval-single-step": eval_single_step.main}
     supported_command_names = ", ".join(supported_commands.keys())
 
     if len(sys.argv) == 1:
-        print(f"Please choose a command from: {supported_command_names}")
-        return
+        raise ValueError(f"Please choose a command from: {supported_command_names}")
 
     command = sys.argv[1]
     if command not in supported_commands:
-        print(f"Command {command} not supported; choose from: {supported_command_names}")
-        return
+        raise ValueError(f"Command {command} not supported; choose from: {supported_command_names}")
 
     # Drop the subcommand name and let the chosen command parse the rest of the arguments.
     del sys.argv[1]
     supported_commands[command]()
 
 
 if __name__ == "__main__":
```

### Comparing `syntheseus-0.3.0/syntheseus/cli/search.py` & `syntheseus-0.4.0/syntheseus/cli/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,26 @@
 from pprint import pformat
 from typing import Any, Dict, Iterator, List, Optional, cast
 
 import yaml
 from omegaconf import MISSING, DictConfig, OmegaConf
 from tqdm import tqdm
 
-from syntheseus.interface.models import BackwardReactionModel
+from syntheseus.interface.molecule import Molecule
 from syntheseus.reaction_prediction.inference.config import BackwardModelConfig
 from syntheseus.reaction_prediction.utils.config import get_config as cli_get_config
 from syntheseus.reaction_prediction.utils.misc import set_random_seed
 from syntheseus.reaction_prediction.utils.model_loading import get_model
-from syntheseus.reaction_prediction.utils.syntheseus_wrapper import SyntheseusBackwardReactionModel
+from syntheseus.search import INT_INF
 from syntheseus.search.algorithms.best_first.retro_star import RetroStarSearch
 from syntheseus.search.algorithms.mcts import base as mcts_base
 from syntheseus.search.algorithms.mcts.molset import MolSetMCTS
 from syntheseus.search.algorithms.pdvn import PDVN_MCTS
 from syntheseus.search.analysis.route_extraction import iter_routes_time_order
 from syntheseus.search.analysis.solution_time import get_first_solution_time
-from syntheseus.search.chem import Molecule
 from syntheseus.search.graph.and_or import AndOrGraph
 from syntheseus.search.graph.molset import MolSetGraph
 from syntheseus.search.mol_inventory import SmilesListInventory
 from syntheseus.search.node_evaluation import common as node_evaluation_common
 from syntheseus.search.utils.misc import lookup_by_name
 from syntheseus.search.visualization import visualize_andor, visualize_molset
 
@@ -112,14 +111,15 @@
     inventory_smiles_file: str = MISSING  # Purchasable molecules
     results_dir: str = "."  # Directory to save the results in
 
     # By default limit search time (but set very high iteration limits just in case)
     time_limit_s: float = 600
     limit_reaction_model_calls: int = 1_000_000
     limit_iterations: int = 1_000_000
+    limit_graph_nodes: int = INT_INF
     prevent_repeat_mol_in_trees: bool = True
 
     use_gpu: bool = True  # Whether to use a GPU
     canonicalize_inventory: bool = False  # Whether to canonicalize the inventory SMILES
 
     # Fields configuring the reaction model (on top of the arguments from `BackwardModelConfig`)
     num_top_results: int = 50  # Number of results to request
@@ -161,21 +161,20 @@
 
     if not config.save_graph and config.num_routes_to_plot == 0:
         logger.warning(
             "Neither 'save_graph' nor 'num_routes_to_plot' is set; output saved will be minimal"
         )
 
     # Load the single-step model
-    base_model = get_model(config, batch_size=1, num_gpus=int(config.use_gpu))  # type: ignore
-
-    # Set up the search algorithm
-    search_rxn_model = SyntheseusBackwardReactionModel(
-        cast(BackwardReactionModel, base_model),
-        num_results=config.num_top_results,
+    search_rxn_model = get_model(  # type: ignore
+        config,
+        batch_size=1,
+        num_gpus=int(config.use_gpu),
         use_cache=config.reaction_model_use_cache,
+        default_num_results=config.num_top_results,
     )
 
     # Set up the inventory
     with open(config.inventory_smiles_file, "rt") as f_inventory:
         inventory_smiles = [line.strip() for line in f_inventory]
     mol_inventory = SmilesListInventory(
         inventory_smiles, canonicalize=config.canonicalize_inventory
@@ -185,14 +184,15 @@
     alg_kwargs.update(
         **{
             key: cast(DictConfig, config).get(key)
             for key in [
                 "time_limit_s",
                 "limit_reaction_model_calls",
                 "limit_iterations",
+                "limit_graph_nodes",
                 "prevent_repeat_mol_in_trees",
             ]
         }
     )
 
     def build_node_evaluator(key: str) -> None:
         # Build a node evaluator based on chosen class and args
```

### Comparing `syntheseus-0.3.0/syntheseus/cli/search_config.yml` & `syntheseus-0.4.0/syntheseus/cli/search_config.yml`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/interface/bag.py` & `syntheseus-0.4.0/syntheseus/interface/bag.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/interface/models.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/misc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,114 @@
-from __future__ import annotations
+import logging
+import multiprocessing
+import os
+import random
+from contextlib import contextmanager, redirect_stderr, redirect_stdout
+from dataclasses import fields, is_dataclass
+from itertools import islice
+from os import devnull
+from typing import Any, Dict, Iterable, Iterator, List, Optional
 
-import math
-from abc import abstractmethod
-from dataclasses import dataclass, field
-from typing import Any, Dict, Generic, List, Optional, TypeVar
+import numpy as np
 
 from syntheseus.interface.bag import Bag
 from syntheseus.interface.molecule import Molecule
 
-InputType = TypeVar("InputType")
-OutputType = TypeVar("OutputType")
 
+def set_random_seed(seed: int = 0) -> None:
+    """Set random seed for `Python`, `torch` and `numpy`."""
+    random.seed(seed)
+    np.random.seed(seed)
+
+    # If `torch` is installed set its seed as well.
+    try:
+        import torch
 
-@dataclass(frozen=True, order=False)
-class Prediction(Generic[InputType, OutputType]):
-    """Reaction prediction from a model, either a forward or a backward one."""
-
-    # The molecule that the prediction is for and the predicted output:
-    input: InputType
-    output: OutputType
-
-    # Optional information that may be useful downstream:
-    probability: Optional[float] = None  # Prior probability.
-    log_prob: Optional[float] = None  # As above, but in log space.
-    score: Optional[float] = None  # Any other score.
-    reaction: Optional[str] = None  # Reaction smiles.
-    rxnid: Optional[int] = None  # Template id, if applicable.
-
-    # Dictionary to hold additional metadata.
-    metadata: Dict[str, Any] = field(default_factory=dict)
-
-    def __post_init__(self):
-        if self.probability is not None and self.log_prob is not None:
-            raise ValueError(
-                "Probability can be stored as probability or log probability, not both"
-            )
-
-    def get_prob(self) -> float:
-        if self.probability is not None:
-            return self.probability
-        elif self.log_prob is not None:
-            return math.exp(self.log_prob)
-        else:
-            raise ValueError("Prediction does not have associated probability or log prob value.")
-
-    def get_log_prob(self) -> float:
-        if self.log_prob is not None:
-            return self.log_prob
-        elif self.probability is not None:
-            return math.log(self.probability)
-        else:
-            raise ValueError("Prediction does not have associated log prob or probability value.")
-
-
-@dataclass(frozen=True, order=False)
-class PredictionList(Generic[InputType, OutputType]):
-    """Several possible predictions."""
-
-    input: InputType
-    predictions: List[Prediction[InputType, OutputType]]
-
-    # Dictionary to hold additional metadata.
-    metadata: Dict[str, Any] = field(default_factory=dict)
-
-    def truncated(self, num_results: int) -> PredictionList[InputType, OutputType]:
-        return PredictionList(
-            input=self.input, predictions=self.predictions[:num_results], metadata=self.metadata
-        )
-
-
-class ReactionModel(Generic[InputType, OutputType]):
-    """Base class for all reaction models, both backward and forward."""
-
-    @abstractmethod
-    def __call__(
-        self, inputs: List[InputType], num_results: int
-    ) -> List[PredictionList[InputType, OutputType]]:
-        """Given a batch of inputs to the reaction model, return a batch of results.
-
-        Args:
-            inputs: Batch of inputs to the reaction model, each either a molecule or a set of
-                molecules, depending on directionality.
-            num_results: Number of results to return for each input in the batch. Many models may
-                only be able to produce a finite number of candidate outputs, thus the returned
-                lists are allowed to be shorter than `num_results`.
-        """
+        torch.manual_seed(seed)
+    except ModuleNotFoundError:
         pass
 
-    def get_model_info(self) -> dict[str, Any]:
-        return {}
 
-    @abstractmethod
-    def is_forward(self) -> bool:
-        pass
-
-    def is_backward(self) -> bool:
-        return not self.is_forward()
-
-    def get_parameters(self):
-        """Return an iterator over parameters (used for computing total parameter count).
-
-        If accurate reporting of number of parameters during evaluation is not important, subclasses
-        are free to e.g. return an empty list.
-        """
-        raise NotImplementedError()
-
-
-# Below we define some aliases for forward and backward variants of prediction and model classes.
-# Model interfaces use bags of SMILES as output type to allow for salts and disconnected components.
-
-
-class BackwardReactionModel(ReactionModel[Molecule, Bag[Molecule]]):
-    def is_forward(self) -> bool:
-        return False
-
-
-class ForwardReactionModel(ReactionModel[Bag[Molecule], Bag[Molecule]]):
-    def is_forward(self) -> bool:
-        return True
-
-
-BackwardPrediction = Prediction[Molecule, Bag[Molecule]]
-ForwardPrediction = Prediction[Bag[Molecule], Bag[Molecule]]
-
-BackwardPredictionList = PredictionList[Molecule, Bag[Molecule]]
-ForwardPredictionList = PredictionList[Bag[Molecule], Bag[Molecule]]
+@contextmanager
+def suppress_outputs():
+    """Suppress messages written to both stdout and stderr."""
+    with open(devnull, "w") as fnull:
+        with redirect_stderr(fnull), redirect_stdout(fnull):
+            # Save the root logger handlers in order to restore them afterwards.
+            root_handlers = list(logging.root.handlers)
+            logging.disable(logging.CRITICAL)
+
+            yield
+
+            logging.root.handlers = root_handlers
+            logging.disable(logging.NOTSET)
+
+
+def dictify(data: Any) -> Any:
+    # Need to ensure we make return objects fully serializable
+    if isinstance(data, (int, float, str)) or data is None:
+        return data
+    elif isinstance(data, Molecule):
+        return {"smiles": data.smiles}
+    elif isinstance(data, (List, tuple, Bag)):
+        # Captures lists of `Prediction`s
+        return [dictify(x) for x in data]
+    elif isinstance(data, dict):
+        return {k: dictify(v) for k, v in data.items()}
+    elif is_dataclass(data):
+        result = {}
+        for f in fields(data):
+            value = getattr(data, f.name)
+            result[f.name] = dictify(value)
+        return result
+    else:
+        raise TypeError(f"Type {type(data)} cannot be handled by `dictify`")
+
+
+def asdict_extended(data) -> Dict[str, Any]:
+    """Convert a dataclass containing various reaction-related objects into a dict."""
+    if not is_dataclass(data):
+        raise TypeError(f"asdict_extended only for use on dataclasses, input is type {type(data)}")
+
+    return dictify(data)
+
+
+def undictify_bag_of_molecules(data: List[Dict[str, str]]) -> Bag[Molecule]:
+    """Recovers a bag of molecules serialized with `dictify`."""
+    return Bag(Molecule(d["smiles"]) for d in data)
+
+
+def parallelize(
+    fn,
+    inputs: Iterable,
+    num_processes: int = 0,
+    chunksize: int = 32,
+    num_chunks_per_process_per_segment: Optional[int] = 64,
+) -> Iterator:
+    """Parallelize an appliation of an arbitrary function using a pool of processes."""
+    if num_processes == 0:
+        yield from map(fn, inputs)
+    else:
+        # Needed for the chunking code to work on repeatable iterables e.g. lists.
+        inputs = iter(inputs)
+
+        with multiprocessing.Pool(num_processes) as pool:
+            if num_chunks_per_process_per_segment is None:
+                yield from pool.imap(fn, inputs, chunksize=chunksize)
+            else:
+                # A new segment will only be started if the previous one was consumed; this avoids doing
+                # all the work upfront and storing it in memory if the consumer of the output is slow.
+                segmentsize = num_chunks_per_process_per_segment * num_processes * chunksize
+
+                non_empty = True
+                while non_empty:
+                    non_empty = False
+
+                    # Call `imap` segment-by-segment to make sure the consumer of the output keeps up.
+                    for result in pool.imap(fn, islice(inputs, segmentsize), chunksize=chunksize):
+                        yield result
+                        non_empty = True
+
+
+def cpu_count(default: int = 8) -> int:
+    """Return the number of CPUs, fallback to `default` if it cannot be determined."""
+    return os.cpu_count() or default
```

### Comparing `syntheseus-0.3.0/syntheseus/interface/molecule.py` & `syntheseus-0.4.0/syntheseus/interface/molecule.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 
 from dataclasses import InitVar, dataclass, field
 from typing import Optional, Union
 
 from rdkit import Chem
 
+from syntheseus.interface.bag import Bag
 from syntheseus.interface.typed_dict import TypedDict
 
 SMILES_SEPARATOR = "."
-REACTION_SEPARATOR = ">"
 
 
 class MoleculeMetaData(TypedDict, total=False):
     """Class to add typing to optional meta-data fields for molecules."""
 
     rdkit_mol: Chem.Mol
 
@@ -78,7 +78,16 @@
 
     @property
     def rdkit_mol(self) -> Chem.Mol:
         """Makes an rdkit mol if one does yet exist"""
         if "rdkit_mol" not in self.metadata:
             self.metadata["rdkit_mol"] = Chem.MolFromSmiles(self.smiles)
         return self.metadata["rdkit_mol"]
+
+
+def molecule_bag_to_smiles(mols: Bag[Molecule]) -> str:
+    """Combine SMILES strings of molecules in a `Bag` into a single string.
+
+    For two bags that represent the same multiset of molecules this function will return the same
+    result, because iteration order over a `Bag` is deterministic (sorted using default comparator).
+    """
+    return SMILES_SEPARATOR.join(mol.smiles for mol in mols)
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/chem/utils.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/chem/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,11 +35,7 @@
 
 def molecule_bag_from_smiles(smiles: str) -> Optional[Bag[Molecule]]:
     try:
         return molecule_bag_from_smiles_strict(smiles)
     except ValueError:
         # If any of the components ends up invalid we return `None` instead.
         return None
-
-
-def molecule_bag_to_smiles(mols: Bag[Molecule]) -> str:
-    return SMILES_SEPARATOR.join(mol.smiles for mol in mols)
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/data/dataset.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/data/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,48 +54,44 @@
         num_processes: int = 0,
         data_format: Optional[DataFormat] = None,
     ):
         self._data_dir = Path(data_dir)
         self._sample_cls = sample_cls
         self._num_processes = num_processes
 
-        filenames = [str(filename) for filename in self._data_dir.iterdir()]
+        paths = list(self._data_dir.iterdir())
 
         if data_format is None:
-            logger.info(f"Detecting data format from files: {filenames}")
+            logger.info(f"Detecting data format from files: {[path.name for path in paths]}")
             formats_to_try = list(DataFormat)
         else:
             formats_to_try = [data_format]
 
         matches = {
-            format: DiskReactionDataset.match_filenames_to_folds(format=format, filenames=filenames)
+            format: DiskReactionDataset.match_paths_to_folds(format=format, paths=paths)
             for format in formats_to_try
         }
         matches = {key: values for key, values in matches.items() if values}
 
         if data_format is None:
             if len(matches) != 1:
                 raise ValueError(
                     f"Format detection failed (formats matching the file list: {[f.name for f in matches]})"
                 )
         elif not matches:
             raise ValueError(
                 f"No files matching *{{train, val, test}}.{data_format.value} were found"
             )
 
-        [(self._data_format, fold_to_filename)] = matches.items()
+        [(self._data_format, self._fold_to_path)] = matches.items()
 
         if data_format is None:
             logger.info(f"Detected format: {self._data_format.name}")
 
-        logger.info(f"Loading data from files {fold_to_filename}")
-
-        self._fold_to_path = {
-            fold: self._data_dir / filename for fold, filename in fold_to_filename.items()
-        }
+        logger.info(f"Loading data from files {self._fold_to_path}")
         self._num_samples: Dict[DataFold, int] = {}
 
     def _get_lines(self, fold: DataFold) -> Iterable[str]:
         if fold not in self._fold_to_path:
             return []
         else:
             with open(self._fold_to_path[fold]) as f:
@@ -121,30 +117,30 @@
     def get_num_samples(self, fold: DataFold) -> int:
         if fold not in self._num_samples:
             self._num_samples[fold] = ilen(self._get_lines(fold))
 
         return self._num_samples[fold]
 
     @staticmethod
-    def match_filenames_to_folds(format: DataFormat, filenames: List[str]) -> Dict[DataFold, str]:
-        fold_to_filename: Dict[DataFold, str] = {}
+    def match_paths_to_folds(format: DataFormat, paths: List[Path]) -> Dict[DataFold, Path]:
+        fold_to_path: Dict[DataFold, Path] = {}
         for fold in DataFold:
             suffix = DiskReactionDataset.get_filename_suffix(format, fold)
-            matching_filenames = [filename for filename in filenames if filename.endswith(suffix)]
+            matching_paths = [path for path in paths if path.name.endswith(suffix)]
 
-            if len(matching_filenames) > 1:
+            if len(matching_paths) > 1:
                 raise ValueError(
-                    f"Found more than one {format.value} file for fold {fold.name}: {matching_filenames}"
+                    f"Found more than one {format.value} file for fold {fold.name}: {matching_paths}"
                 )
 
-            if matching_filenames:
-                [filename] = matching_filenames
-                fold_to_filename[fold] = filename
+            if matching_paths:
+                [path] = matching_paths
+                fold_to_path[fold] = path
 
-        return fold_to_filename
+        return fold_to_path
 
     @staticmethod
     def get_filename_suffix(format: DataFormat, fold: DataFold) -> str:
         return f"{fold.value}.{format.value}"
 
     @staticmethod
     def sample_from_json(data: str, sample_cls: Type[SampleType]) -> SampleType:
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/data/reaction_sample.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/data/reaction_sample.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,35 @@
 from __future__ import annotations
 
 import inspect
 from dataclasses import dataclass, field
 from typing import Any, Dict, Optional, Type, TypeVar
 
 from syntheseus.interface.bag import Bag
-from syntheseus.interface.molecule import REACTION_SEPARATOR, SMILES_SEPARATOR, Molecule
-from syntheseus.reaction_prediction.chem.utils import (
-    molecule_bag_to_smiles,
-    remove_atom_mapping,
-)
+from syntheseus.interface.molecule import SMILES_SEPARATOR, Molecule
+from syntheseus.interface.reaction import REACTION_SEPARATOR, Reaction
+from syntheseus.reaction_prediction.chem.utils import remove_atom_mapping
 from syntheseus.reaction_prediction.utils.misc import undictify_bag_of_molecules
 
 ReactionType = TypeVar("ReactionType", bound="ReactionSample")
 
 
 @dataclass(frozen=True, order=False)
-class ReactionSample:
-    """
-    Wraps around a reaction.
-
-    It is frozen since it should not need to be edited,
-    and this will auto-implement __eq__ and __hash__ methods.
-    """
+class ReactionSample(Reaction):
+    """Extends a `Reaction` with fields and methods relevant to data loading and saving."""
 
-    reactants: Bag[Molecule] = field(hash=True, compare=True)
-    products: Bag[Molecule] = field(hash=True, compare=True)
     reagents: str = field(default="", hash=True, compare=True)
-    identifier: Optional[str] = field(default=None, hash=True, compare=True)
-
     mapped_reaction_smiles: Optional[str] = field(default=None, hash=False, compare=False)
-    template: Optional[str] = field(default=None, hash=False, compare=False)
-
-    metadata: Dict[str, Any] = field(
-        default_factory=lambda: dict(),
-        hash=False,
-        compare=False,
-    )
-
-    @property
-    def reactants_combined(self) -> str:
-        return molecule_bag_to_smiles(self.reactants)
-
-    @property
-    def products_combined(self) -> str:
-        return molecule_bag_to_smiles(self.products)
-
-    @property
-    def reaction_smiles(self) -> str:
-        return f"{self.reactants_combined}{2 * REACTION_SEPARATOR}{self.products_combined}"
 
     @property
     def reaction_smiles_with_reagents(self) -> str:
         return (
-            f"{self.reactants_combined}{REACTION_SEPARATOR}"
+            f"{self.reactants_str}{REACTION_SEPARATOR}"
             f"{self.reagents}{REACTION_SEPARATOR}"
-            f"{self.products_combined}"
+            f"{self.products_str}"
         )
 
     @classmethod
     def from_dict(cls: Type[ReactionType], data: Dict[str, Any]) -> ReactionType:
         """Creates a sample from the given arguments ignoring superfluous ones."""
         for key in ["reactants", "products"]:
             data[key] = undictify_bag_of_molecules(data[key])
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/environment_gln/Dockerfile` & `syntheseus-0.4.0/syntheseus/reaction_prediction/environment_gln/Dockerfile`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/__init__.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 from syntheseus.reaction_prediction.inference.chemformer import ChemformerModel
 from syntheseus.reaction_prediction.inference.gln import GLNModel
+from syntheseus.reaction_prediction.inference.graph2edits import Graph2EditsModel
 from syntheseus.reaction_prediction.inference.local_retro import LocalRetroModel
 from syntheseus.reaction_prediction.inference.megan import MEGANModel
 from syntheseus.reaction_prediction.inference.mhnreact import MHNreactModel
 from syntheseus.reaction_prediction.inference.retro_knn import RetroKNNModel
 from syntheseus.reaction_prediction.inference.root_aligned import RootAlignedModel
+from syntheseus.reaction_prediction.inference.toy_models import (
+    LinearMoleculesToyModel,
+    ListOfReactionsToyModel,
+)
 
 __all__ = [
     "ChemformerModel",
     "GLNModel",
+    "Graph2EditsModel",
+    "LinearMoleculesToyModel",
+    "ListOfReactionsToyModel",
     "LocalRetroModel",
     "MEGANModel",
     "MHNreactModel",
     "RetroKNNModel",
     "RootAlignedModel",
 ]
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/base.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from syntheseus.interface.models import (
     BackwardReactionModel,
     ForwardReactionModel,
     InputType,
-    OutputType,
     ReactionModel,
+    ReactionType,
 )
 from syntheseus.reaction_prediction.utils.downloading import get_default_model_dir_from_cache
 
 
-class ExternalReactionModel(ReactionModel[InputType, OutputType]):
+class ExternalReactionModel(ReactionModel[InputType, ReactionType]):
     """Base class for the external reaction models, abstracting out common functinality."""
 
     def __init__(
-        self, model_dir: Optional[Union[str, Path]] = None, device: Optional[str] = None
+        self, model_dir: Optional[Union[str, Path]] = None, device: Optional[str] = None, **kwargs
     ) -> None:
+        super().__init__(**kwargs)
         import torch
 
         self.model_dir = Path(model_dir or self.get_default_model_dir())
         self.device = device or ("cuda:0" if torch.cuda.is_available() else "cpu")
 
     def get_default_model_dir(self) -> Path:
         model_dir = get_default_model_dir_from_cache(self.name, is_forward=self.is_forward())
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/chemformer.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/chemformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,31 +2,35 @@
 
 Paper: https://chemrxiv.org/engage/chemrxiv/article-details/60ee8a3eb95bdd06d062074b
 Code: https://github.com/MolecularAI/Chemformer
 
 The original Chemformer code is released under the Apache 2.0 license.
 """
 
+import math
 import sys
+import warnings
 from pathlib import Path
-from typing import Any, Dict, List, Tuple, cast
+from typing import Any, Callable, Dict, List, Sequence, Tuple, cast
 
 from syntheseus.interface.bag import Bag
-from syntheseus.interface.models import InputType, OutputType, PredictionList
+from syntheseus.interface.models import InputType, ReactionType
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import ReactionMetaData
 from syntheseus.reaction_prediction.inference.base import ExternalReactionModel
 from syntheseus.reaction_prediction.utils.inference import (
     get_module_path,
     get_unique_file_in_dir,
-    process_raw_smiles_outputs,
+    process_raw_smiles_outputs_backwards,
+    process_raw_smiles_outputs_forwards,
 )
 from syntheseus.reaction_prediction.utils.misc import suppress_outputs
 
 
-class ChemformerModel(ExternalReactionModel[InputType, OutputType]):
+class ChemformerModel(ExternalReactionModel[InputType, ReactionType]):
     def __init__(self, *args, is_forward: bool = False, **kwargs) -> None:
         """Initializes the Chemformer model wrapper.
 
         Assumed format of the model directory:
         - `model_dir` contains the model checkpoint as the only `*.ckpt` file
         """
         self._is_forward = is_forward
@@ -100,34 +104,54 @@
 
         # Convert inputs to the model to tensors.
         return {
             "encoder_input": torch.tensor(token_ids).transpose(0, 1),
             "encoder_pad_mask": torch.tensor(mask, dtype=torch.bool).transpose(0, 1),
         }
 
-    def __call__(self, inputs: List[InputType], num_results: int) -> List[PredictionList]:
+    def _get_reactions(
+        self, inputs: List[InputType], num_results: int
+    ) -> List[Sequence[ReactionType]]:
         import torch
 
         # Get the data in to the right form to call the sampling method on the model.
         batch = self._mols_to_batch(inputs)
 
         device_batch = {
             key: val.to(self.device) if type(val) == torch.Tensor else val
             for key, val in batch.items()
         }
 
         # We have to set `num_beams` as an attribute of the model.
         self.model.num_beams = num_results
-        with torch.no_grad():
+
+        with torch.no_grad(), warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="__floordiv__ is deprecated")
+
             smiles_batch, batch_log_likelihoods = self.model.sample_molecules(
                 device_batch, sampling_alg="beam"
             )
 
+        # Choose processing function (controls reaction types).
+        # `type: ignore[assignment]` statements are because link between is_forward/is_backward
+        # and [InputType, ReactionType] is not visible to mypy.
+        if self.is_forward():
+            process_fn: Callable[
+                [InputType, List[str], List[ReactionMetaData]], Sequence[ReactionType]
+            ] = process_raw_smiles_outputs_forwards  # type: ignore[assignment]
+        else:
+            process_fn = process_raw_smiles_outputs_backwards  # type: ignore[assignment]
+
         return [
-            process_raw_smiles_outputs(
-                input, outputs, [{"log_prob": log_prob} for log_prob in log_probs]
+            process_fn(
+                input,
+                outputs,
+                [
+                    {"log_probability": log_prob, "probability": math.exp(log_prob)}
+                    for log_prob in log_probs
+                ],
             )
             for input, outputs, log_probs in zip(inputs, smiles_batch, batch_log_likelihoods)
         ]
 
     def is_forward(self):
         return self._is_forward
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/config.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Dict
 
 from omegaconf import MISSING
 
 from syntheseus.reaction_prediction.inference import (
     ChemformerModel,
     GLNModel,
+    Graph2EditsModel,
     LocalRetroModel,
     MEGANModel,
     MHNreactModel,
     RetroKNNModel,
     RootAlignedModel,
 )
 
@@ -18,14 +19,15 @@
 class ForwardModelClass(Enum):
     Chemformer = ChemformerModel
 
 
 class BackwardModelClass(Enum):
     Chemformer = ChemformerModel
     GLN = GLNModel
+    Graph2Edits = Graph2EditsModel
     LocalRetro = LocalRetroModel
     MEGAN = MEGANModel
     MHNreact = MHNreactModel
     RetroKNN = RetroKNNModel
     RootAligned = RootAlignedModel
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/gln.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/gln.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 Code: https://github.com/Hanjun-Dai/GLN
 
 The original GLN code is released under the MIT license.
 """
 
 import sys
 from pathlib import Path
-from typing import List
+from typing import List, Sequence
 
-from syntheseus.interface.models import BackwardPredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.reaction_prediction.inference.base import ExternalBackwardReactionModel
-from syntheseus.reaction_prediction.utils.inference import process_raw_smiles_outputs
+from syntheseus.reaction_prediction.utils.inference import process_raw_smiles_outputs_backwards
 from syntheseus.reaction_prediction.utils.misc import suppress_outputs
 
 
 class GLNModel(ExternalBackwardReactionModel):
     def __init__(self, *args, dataset_name: str = "schneider50k", **kwargs) -> None:
         """Initializes the GLN model wrapper.
 
@@ -56,23 +56,27 @@
             from gln.test.model_inference import RetroGLN
 
             self.model = RetroGLN(self.model_dir, chkpt_path)
 
     def get_parameters(self):
         return self.model.gln.parameters()
 
-    def _get_model_predictions(self, input: Molecule, num_results: int) -> BackwardPredictionList:
+    def _get_model_predictions(
+        self, input: Molecule, num_results: int
+    ) -> Sequence[SingleProductReaction]:
         with suppress_outputs():
             result = self.model.run(input.smiles, num_results, num_results)
 
         if result is None:
-            return BackwardPredictionList(input=input, predictions=[])
+            return []
         else:
             # `scores` are actually probabilities (produced by running `softmax`).
-            return process_raw_smiles_outputs(
+            return process_raw_smiles_outputs_backwards(
                 input=input,
                 output_list=result["reactants"],
-                kwargs_list=[{"probability": probability} for probability in result["scores"]],
+                metadata_list=[{"probability": probability} for probability in result["scores"]],
             )
 
-    def __call__(self, inputs: List[Molecule], num_results: int) -> List[BackwardPredictionList]:
+    def _get_reactions(
+        self, inputs: List[Molecule], num_results: int
+    ) -> List[Sequence[SingleProductReaction]]:
         return [self._get_model_predictions(input, num_results=num_results) for input in inputs]
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/local_retro.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/local_retro.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 Paper: https://pubs.acs.org/doi/10.1021/jacsau.1c00246
 Code: https://github.com/kaist-amsg/LocalRetro
 
 The original LocalRetro code is released under the Apache 2.0 license.
 Parts of this file are based on code from the GitHub repository above.
 """
 
-import sys
 from pathlib import Path
-from typing import Any, List
+from typing import Any, List, Sequence
 
-from syntheseus.interface.models import BackwardPredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.reaction_prediction.inference.base import ExternalBackwardReactionModel
 from syntheseus.reaction_prediction.utils.inference import (
-    get_module_path,
     get_unique_file_in_dir,
-    process_raw_smiles_outputs,
+    process_raw_smiles_outputs_backwards,
 )
 from syntheseus.reaction_prediction.utils.misc import suppress_outputs
 
 
 class LocalRetroModel(ExternalBackwardReactionModel):
     def __init__(self, *args, **kwargs) -> None:
         """Initializes the LocalRetro model wrapper.
@@ -29,21 +27,14 @@
         Assumed format of the model directory:
         - `model_dir` contains the model checkpoint as the only `*.pth` file
         - `model_dir` contains the config as the only `*.json` file
         - `model_dir/data` contains `*.csv` data files needed by LocalRetro
         """
         super().__init__(*args, **kwargs)
 
-        import local_retro
-        from local_retro import scripts
-
-        # We need to hack `sys.path` because LocalRetro uses relative imports.
-        sys.path.insert(0, get_module_path(local_retro))
-        sys.path.insert(0, get_module_path(scripts))
-
         from local_retro.Retrosynthesis import load_templates
         from local_retro.scripts.utils import init_featurizer, load_model
 
         data_dir = Path(self.model_dir) / "data"
         self.args = init_featurizer(
             {
                 "mode": "test",
@@ -82,15 +73,15 @@
             for mol in mols
         ]
 
         return collate_molgraphs_test([(None, graph, None) for graph in graphs])[1]
 
     def _build_batch_predictions(
         self, batch, num_results: int, inputs: List[Molecule], batch_atom_logits, batch_bond_logits
-    ) -> List[BackwardPredictionList]:
+    ) -> List[Sequence[SingleProductReaction]]:
         from local_retro.scripts.Decode_predictions import get_k_predictions
         from local_retro.scripts.get_edit import combined_edit, get_bg_partition
 
         graphs, nodes_sep, edges_sep = get_bg_partition(batch)
         start_node = 0
         start_edge = 0
 
@@ -128,24 +119,26 @@
 
             if raw_results:
                 raw_outputs, probabilities = zip(*raw_results)
             else:
                 raw_outputs = probabilities = []
 
             batch_predictions.append(
-                process_raw_smiles_outputs(
+                process_raw_smiles_outputs_backwards(
                     input=input,
                     output_list=raw_outputs,
-                    kwargs_list=[{"probability": probability} for probability in probabilities],
+                    metadata_list=[{"probability": probability} for probability in probabilities],
                 )
             )
 
         return batch_predictions
 
-    def __call__(self, inputs: List[Molecule], num_results: int) -> List[BackwardPredictionList]:
+    def _get_reactions(
+        self, inputs: List[Molecule], num_results: int
+    ) -> List[Sequence[SingleProductReaction]]:
         import torch
         from local_retro.scripts.utils import predict
 
         batch = self._mols_to_batch(inputs)
         batch_atom_logits, batch_bond_logits, _ = predict(self.args, self.model, batch)
 
         batch_atom_logits = torch.nn.Softmax(dim=1)(batch_atom_logits)
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/megan.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/megan.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 Code: https://github.com/molecule-one/megan
 
 The original MEGAN code is released under the MIT license.
 """
 
 from __future__ import annotations
 
+import logging
 import os
 import sys
+from logging.handlers import RotatingFileHandler
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Optional, Sequence
 
 from rdkit import Chem
 
-from syntheseus.interface.models import BackwardPredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.reaction_prediction.inference.base import ExternalBackwardReactionModel
 from syntheseus.reaction_prediction.utils.inference import (
     get_module_path,
     get_unique_file_in_dir,
-    process_raw_smiles_outputs,
+    process_raw_smiles_outputs_backwards,
 )
 from syntheseus.reaction_prediction.utils.misc import suppress_outputs
 
 
 class MEGANModel(ExternalBackwardReactionModel):
     def __init__(
         self,
@@ -40,30 +42,59 @@
         Assumed format of the model directory:
         - `model_dir` contains the config as the only `*.gin` file
         - `model_dir/model_best.pt` is the model checkpoint
         - `model_dir/{featurizer_key}` contains files needed to build MEGAN's featurizer
         """
         super().__init__(*args, **kwargs)
 
+        # Silence tensorflow's warnings.
+        os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
+
         import gin
         import megan
+        import torch
+
+        if self.device == "cpu" and torch.cuda.is_available():
+            raise ValueError(
+                "MEGAN currently does not support running on CPU if a GPU is available"
+            )
 
         # Extract the path to the `megan` module.
         module_path = Path(get_module_path(megan))
 
         os.environ["PROJECT_ROOT"] = str(module_path.parent)
         sys.path.insert(0, str(module_path))
 
+        def _get_root_logger_log_file_paths() -> set[Path]:
+            return set(
+                Path(handler.baseFilename)
+                for handler in logging.root.handlers
+                if isinstance(handler, RotatingFileHandler)
+            )
+
         # The (seemingly unused) import below is needed for `gin` configurables to get registered.
-        from bin.train import train_megan  # noqa: F401
-        from src.config import get_featurizer
-        from src.feat.megan_graph import MeganTrainingSamplesFeaturizer
-        from src.model.megan import Megan as MeganModel
-        from src.model.megan_utils import RdkitCache, get_base_action_masks
-        from src.utils import load_state_dict
+        with suppress_outputs():
+            preexisting_paths = _get_root_logger_log_file_paths()
+
+            from bin.train import train_megan  # noqa: F401
+            from src.config import get_featurizer
+            from src.feat.megan_graph import MeganTrainingSamplesFeaturizer
+            from src.model.megan import Megan as MeganModel
+            from src.model.megan_utils import RdkitCache, get_base_action_masks
+            from src.utils import load_state_dict
+
+            # Delete logging files created by MEGAN.
+            new_paths = _get_root_logger_log_file_paths() - preexisting_paths
+
+            for path in new_paths:
+                path.unlink()
+
+            for path in new_paths:
+                if path.parent.exists():
+                    path.parent.rmdir()
 
         self.n_max_atoms = n_max_atoms
         self.max_gen_steps = max_gen_steps
         self.beam_batch_size = beam_batch_size
 
         # Get the model config using `gin`.
         gin.parse_config_file(get_unique_file_in_dir(self.model_dir, pattern="*.gin"))
@@ -111,25 +142,27 @@
                 # MEGAN sometimes produces broken molecules containing C+ atoms which pass `rdkit`
                 # sanitization but fail in `fix_explicit_hs`. We block these here to avoid making
                 # predictions for them.
                 input_batch.append(None)
 
         return input_batch
 
-    def __call__(self, inputs: list[Molecule], num_results: int) -> list[BackwardPredictionList]:
+    def _get_reactions(
+        self, inputs: list[Molecule], num_results: int
+    ) -> list[Sequence[SingleProductReaction]]:
         import torch
         from src.model.beam_search import beam_search
 
         # Get the inputs into the right form to call the underlying model.
         batch = self._mols_to_batch(inputs)
         batch_valid = [mol for mol in batch if mol is not None]
         batch_valid_idxs = [idx for idx, mol in enumerate(batch) if mol is not None]
 
         if batch_valid:
-            with torch.no_grad(), suppress_outputs():
+            with torch.no_grad():
                 beam_search_results = beam_search(
                     [self.model],
                     batch_valid,
                     rdkit_cache=self.rdkit_cache,
                     max_steps=self.max_gen_steps,
                     beam_size=num_results,
                     batch_size=self.beam_batch_size,
@@ -144,14 +177,14 @@
         assert len(batch_valid_idxs) == len(beam_search_results)
 
         all_outputs: list[list[dict[str, Any]]] = [[] for _ in batch]
         for idx, raw_outputs in zip(batch_valid_idxs, beam_search_results):
             all_outputs[idx] = raw_outputs
 
         return [
-            process_raw_smiles_outputs(
+            process_raw_smiles_outputs_backwards(
                 input=input,
                 output_list=[prediction["final_smi_unmapped"] for prediction in raw_outputs],
-                kwargs_list=[{"probability": prediction["prob"]} for prediction in raw_outputs],
+                metadata_list=[{"probability": prediction["prob"]} for prediction in raw_outputs],
             )
             for input, raw_outputs in zip(inputs, all_outputs)
         ]
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/mhnreact.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/mhnreact.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 Code: https://github.com/ml-jku/mhn-react
 
 The original MHNreact code is released under the BSD-2-Clause license.
 """
 
 import json
 from collections import defaultdict
-from typing import List
+from functools import partial
+from typing import List, Sequence
+
+from tqdm.contrib import concurrent
 
-from syntheseus.interface.models import BackwardPredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.reaction_prediction.inference.base import ExternalBackwardReactionModel
 from syntheseus.reaction_prediction.utils.inference import (
     get_unique_file_in_dir,
-    process_raw_smiles_outputs,
+    process_raw_smiles_outputs_backwards,
 )
 from syntheseus.reaction_prediction.utils.misc import cpu_count, suppress_outputs
 
 
 class MHNreactModel(ExternalBackwardReactionModel):
     def __init__(
         self,
@@ -40,14 +43,16 @@
         super().__init__(*args, **kwargs)
 
         import torch
         from mhnreact import data, model
 
         with open(get_unique_file_in_dir(self.model_dir, pattern="*.json"), "r") as conf:
             conf_dict = json.load(conf)
+        conf_dict["device"] = self.device
+
         conf = model.ModelConfig(**conf_dict)
         self.model = model.MHN(config=conf)
 
         self.use_FPF = use_FPF
         self.num_processes = num_processes
         self.chunksize = chunksize
         self.num_additional_templates_to_run = num_additional_templates_to_run
@@ -86,15 +91,17 @@
             )
         self.model.eval()
         self.model.X = self.model.template_encoder(self.model.templates)
 
     def get_parameters(self):
         return self.model.parameters()
 
-    def __call__(self, inputs: List[Molecule], num_results: int) -> List[BackwardPredictionList]:
+    def _get_reactions(
+        self, inputs: List[Molecule], num_results: int
+    ) -> List[Sequence[SingleProductReaction]]:
         import pandas as pd
         import torch
 
         input_smiles_list = [inp.smiles for inp in inputs]
 
         with torch.no_grad():
             # Compute probabilities ranking the templates for each molecule.
@@ -127,27 +134,32 @@
         for batch_idx, top_templates in enumerate(top_k_templates):
             for template in top_templates:
                 # If `use_FPF` perform an extra filter to weed out most inapplicable templates.
                 if (not self.use_FPF) or ((appl[1][appl[0] == batch_idx] == template).any()):
                     batch_idxs.append(batch_idx)
                     templates_to_apply.append(template)
 
-        with suppress_outputs():
-            prod_idx_reactants, _ = run_templates(
-                input_smiles_list,
-                templates=self.model.template_list,
-                appl=[batch_idxs, templates_to_apply],
-                njobs=self.num_processes,
-                chunksize=self.chunksize,
-            )
+        # Temporarily disable tqdm (just the particular function used in MHNreact).
+        process_map_orig = concurrent.process_map
+        concurrent.process_map = partial(concurrent.process_map, disable=True)
+
+        prod_idx_reactants, _ = run_templates(
+            input_smiles_list,
+            templates=self.model.template_list,
+            appl=[batch_idxs, templates_to_apply],
+            njobs=self.num_processes,
+            chunksize=self.chunksize,
+        )
+
+        concurrent.process_map = process_map_orig
 
         # Now aggregate over same outcome (parts copied from `utils.sort_by_template_and_flatten`,
         # which does not expose the summed probabilities) and build the prediction objects.
 
-        batch_predictions: List[BackwardPredictionList] = []
+        batch_predictions: List[Sequence[SingleProductReaction]] = []
         for idx in range(len(template_scores)):
             idx_prod_reactants = defaultdict(list)
             for k, v in prod_idx_reactants[idx].items():
                 for iv in v:
                     idx_prod_reactants[iv].append(template_scores[idx, k])
             d2 = {k: sum(v) for k, v in idx_prod_reactants.items()}
 
@@ -162,15 +174,15 @@
                 # Limit to `num_results` results.
                 df_sorted = df_sorted.iloc[:num_results, :]
 
                 results = df_sorted.index.tolist()
                 probs = df_sorted.values.ravel().tolist()
 
             batch_predictions.append(
-                process_raw_smiles_outputs(
+                process_raw_smiles_outputs_backwards(
                     input=inputs[idx],
                     output_list=results,
-                    kwargs_list=[{"probability": probability} for probability in probs],
+                    metadata_list=[{"probability": probability} for probability in probs],
                 )
             )
 
         return batch_predictions
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/retro_knn.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/retro_knn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Inference wrapper for the RetroKNN model.
 
 Paper: https://arxiv.org/abs/2306.04123
 """
 
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Optional, Sequence, Union
 
 import numpy as np
 
-from syntheseus.interface.models import BackwardPredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.reaction_prediction.inference.local_retro import LocalRetroModel
 from syntheseus.reaction_prediction.utils.inference import get_unique_file_in_dir
 
 
 class RetroKNNModel(LocalRetroModel):
     """Warpper for RetroKNN model."""
 
@@ -34,78 +34,80 @@
 
         adapter_chkpt_path = get_unique_file_in_dir(Path(model_dir) / "knn", pattern="*.pt")
         datastore_path = Path(model_dir) / "knn" / "datastore"
 
         import faiss
         import faiss.contrib.torch_utils  # make faiss available for torch tensors
 
-        def load_data_store(path: Path):
+        def load_data_store(path: Path, device: str):
             index = faiss.read_index(str(path), faiss.IO_FLAG_ONDISK_SAME_DIR)
-            res = faiss.StandardGpuResources()
-            co = faiss.GpuClonerOptions()
-            co.useFloat16 = True
-            return faiss.index_cpu_to_gpu(res, 0, index, co)
 
-        self.atom_store = load_data_store(datastore_path / "data.atom_idx")
-        self.bond_store = load_data_store(datastore_path / "data.bond_idx")
+            if device == "cpu":
+                return index
+            else:
+                res = faiss.StandardGpuResources()
+                co = faiss.GpuClonerOptions()
+                co.useFloat16 = True
+                return faiss.index_cpu_to_gpu(res, 0, index, co)
+
+        self.atom_store = load_data_store(datastore_path / "data.atom_idx", device=self.device)
+        self.bond_store = load_data_store(datastore_path / "data.bond_idx", device=self.device)
         self.raw_data = np.load(datastore_path / "data.npz")
 
-        self.adapter = Adapter(self.model.linearB.weight.shape[0], k=32).to(self.args["device"])
-        self.adapter.load_state_dict(torch.load(adapter_chkpt_path))
+        self.adapter = Adapter(self.model.linearB.weight.shape[0], k=32).to(self.device)
+        self.adapter.load_state_dict(torch.load(adapter_chkpt_path, map_location=self.device))
         self.adapter.eval()
 
     def _forward_localretro(self, bg):
         from local_retro.scripts.model_utils import pair_atom_feats, unbatch_feats, unbatch_mask
 
-        bg = bg.to(self.args["device"])
-        node_feats = bg.ndata.pop("h").to(self.args["device"])
-        edge_feats = bg.edata.pop("e").to(self.args["device"])
+        bg = bg.to(self.device)
+        node_feats = bg.ndata.pop("h").to(self.device)
+        edge_feats = bg.edata.pop("e").to(self.device)
 
         node_feats = self.model.mpnn(bg, node_feats, edge_feats)
         atom_feats = node_feats
         bond_feats = self.model.linearB(pair_atom_feats(bg, node_feats))
         edit_feats, mask = unbatch_mask(bg, atom_feats, bond_feats)
         _, edit_feats = self.model.att(edit_feats, mask)
 
         atom_feats, bond_feats = unbatch_feats(bg, edit_feats)
         atom_outs = self.model.atom_linear(atom_feats)
         bond_outs = self.model.bond_linear(bond_feats)
 
         return atom_outs, bond_outs, atom_feats, bond_feats
 
-    def __call__(self, inputs: List[Molecule], num_results: int) -> List[BackwardPredictionList]:
+    def _get_reactions(
+        self, inputs: List[Molecule], num_results: int
+    ) -> List[Sequence[SingleProductReaction]]:
         import torch
 
         from syntheseus.reaction_prediction.models.retro_knn import knn_prob
 
         batch = self._mols_to_batch(inputs)
         (
             batch_atom_logits,
             batch_bond_logits,
             atom_feats,
             bond_feats,
         ) = self._forward_localretro(batch)
-        sg = batch.remove_self_loop().to(self.args["device"])
+        sg = batch.remove_self_loop().to(self.device)
 
         node_dis, _ = self.atom_store.search(atom_feats, k=32)
         edge_dis, _ = self.bond_store.search(bond_feats, k=32)
 
         node_t, node_p, edge_t, edge_p = self.adapter(
             sg, atom_feats, bond_feats, node_dis, edge_dis
         )
 
         batch_atom_prob_nn = torch.nn.Softmax(dim=1)(batch_atom_logits)
         batch_bond_prob_nn = torch.nn.Softmax(dim=1)(batch_bond_logits)
 
-        atom_output_label = torch.from_numpy(self.raw_data["atom_output_label"]).to(
-            self.args["device"]
-        )
-        bond_output_label = torch.from_numpy(self.raw_data["bond_output_label"]).to(
-            self.args["device"]
-        )
+        atom_output_label = torch.from_numpy(self.raw_data["atom_output_label"]).to(self.device)
+        bond_output_label = torch.from_numpy(self.raw_data["bond_output_label"]).to(self.device)
 
         batch_atom_prob_knn = knn_prob(
             atom_feats, self.atom_store, atom_output_label, batch_atom_logits.shape[1], 32, node_t
         )
         batch_bond_prob_knn = knn_prob(
             bond_feats, self.bond_store, bond_output_label, batch_bond_logits.shape[1], 32, edge_t
         )
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/inference/root_aligned.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/root_aligned.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 Parts of this file are based on code from the GitHub repository above.
 """
 
 import argparse
 import math
 import multiprocessing
 import random
+import warnings
 from collections import defaultdict
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional, Sequence
 
 import yaml
 from rdkit import Chem
 
-from syntheseus.interface.models import PredictionList
 from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import ReactionMetaData, SingleProductReaction
 from syntheseus.reaction_prediction.inference.base import ExternalBackwardReactionModel
 from syntheseus.reaction_prediction.utils.inference import (
     get_unique_file_in_dir,
-    process_raw_smiles_outputs,
+    process_raw_smiles_outputs_backwards,
 )
-from syntheseus.reaction_prediction.utils.misc import suppress_outputs
 
 
 class RootAlignedModel(ExternalBackwardReactionModel):
     def __init__(
         self,
         *args,
         num_augmentations: int = 20,
@@ -43,36 +43,37 @@
         """
         super().__init__(*args, **kwargs)
 
         # Parse arguments for calling external functions from `root_aligned/OpenNMT.py`.
         with open(get_unique_file_in_dir(self.model_dir, pattern="*.yml"), "r") as f:
             opt_from_config = yaml.safe_load(f)
 
+        import torch
+
         opt = argparse.Namespace()
         for key, value in opt_from_config.items():
             setattr(opt, key, value)
+
         opt.models = [get_unique_file_in_dir(self.model_dir, pattern="*.pt")]
         opt.output = "/dev/null"
+        opt.gpu = -1 if self.device == "cpu" else torch.device(self.device).index
+
         setattr(opt, "synthon", False)
 
         from root_aligned import score
 
         score.opt = opt
 
         # Import external functions from `root_aligned/OpenNMT.py`.
         from onmt.translate.translator import build_translator
-        from onmt.utils.logging import init_logger
         from onmt.utils.parse import ArgumentParser
 
         ArgumentParser.validate_translate_opts(opt)
 
-        with suppress_outputs():
-            logger = init_logger(opt.log_file)
-
-        self.translator = build_translator(opt, logger=logger, report_score=True)
+        self.translator = build_translator(opt, report_score=False)
         self.num_augmentations = num_augmentations
         self.probability_from_score_temperature = probability_from_score_temperature
         self.beam_size = opt.beam_size
 
     def get_parameters(self):
         """Return the model parameters."""
         return self.translator.model.parameters()
@@ -80,15 +81,15 @@
     def _mols_to_batch(self, inputs) -> List[bytes]:
         """Map `Molecule`s into SMILES bytes."""
         from root_aligned.score import smi_tokenizer
 
         # Example outcome: b'C C ( = O ) c 1 c c c 2 c ( c c n 2 C ( = O ) O C ( C ) ( C ) C ) c 1\n'.
         return [bytes(smi_tokenizer(input.smiles) + "\n", "utf-8") for input in inputs]
 
-    def _build_kwargs_from_scores(self, scores: List[float]) -> List[Dict[str, Any]]:
+    def _build_kwargs_from_scores(self, scores: List[float]) -> List[ReactionMetaData]:
         """Compute kwargs to save in the predictions given raw scores from the RootAligned model.
 
         The scores we get from the model cannot be directly interpreted as a (log) probability.
         In general, the model produces an array of `[num_augmentations, beam_size]` predictions, and
         computes the score of a given prediction `p` as `total_rr - best_pos * 1e8` where:
             `total_rr = sum_{(j, k) such that prediction[j, k] = p} (1 / (k + 1))`
             `best_pos = min_{(j, k) such that prediction[j, k] = p} k`
@@ -106,45 +107,53 @@
             assert score >= next_score
 
         # Maximum possible value `total_rr` could have.
         max_possible_total_rr = self.num_augmentations * sum(
             1.0 / (k + 1) for k in range(self.beam_size)
         )
 
-        kwargs_list: List[Dict[str, Any]] = []
+        kwargs_list: List[ReactionMetaData] = []
         for score in scores:
             best_pos = -math.floor(score / 1e8)
             total_rr = score + best_pos * 1e8
 
             assert 0 <= best_pos < self.beam_size
             assert 0.0 < total_rr <= max_possible_total_rr
 
-            metadata = {"original_score": score, "best_pos": best_pos, "total_rr": total_rr}
             new_score = total_rr - (best_pos + 1) * max_possible_total_rr
-
             assert new_score <= 0.0
-            kwargs_list.append({"score": new_score, "metadata": metadata})
+
+            kwargs_list.append(
+                {  # type: ignore[typeddict-unknown-key]
+                    "original_score": score,
+                    "best_pos": best_pos,
+                    "total_rr": total_rr,
+                    "score": new_score,
+                }
+            )
 
         # Make sure the new scores produce the same ranking.
         for kwargs, next_kwargs in zip(kwargs_list, kwargs_list[1:]):
             assert kwargs["score"] >= next_kwargs["score"]
 
         if self.probability_from_score_temperature is not None:
             scaled_scores = [
                 self.probability_from_score_temperature * kwargs["score"] / max_possible_total_rr
                 for kwargs in kwargs_list
             ]
             probabilities = torch.nn.functional.softmax(torch.as_tensor(scaled_scores), dim=-1)
 
-            for kwargs, probability in zip(kwargs_list, probabilities):
+            for kwargs, probability in zip(kwargs_list, probabilities.numpy().tolist()):
                 kwargs["probability"] = probability
 
         return kwargs_list
 
-    def __call__(self, inputs, num_results: int, random_augmentation=False) -> List[PredictionList]:
+    def _get_reactions(
+        self, inputs, num_results: int, random_augmentation=False
+    ) -> List[Sequence[SingleProductReaction]]:
         # Step 1: Perform data augmentation.
         augmented_inputs = []
         if random_augmentation:
             for input in inputs:
                 augmented_inputs.append(input)
                 for i in range(self.num_augmentations - 1):
                     randomized_smi = Chem.MolToSmiles(input.rdkit_mol, doRandom=True)
@@ -183,23 +192,26 @@
 
         assert len(augmented_inputs) == len(inputs) * self.num_augmentations
 
         # Step 2: Map from `Molecule`s to SMILES bytes to align with `root_aligned/OpenNMT.py`.
         augmented_batch = self._mols_to_batch(augmented_inputs)
 
         # Step 3: Translate.
-        _, augmented_predictions = self.translator.translate(
-            src=augmented_batch,
-            src_feats=defaultdict(list),
-            tgt=None,
-            batch_size=2048,
-            batch_type="tokens",
-            attn_debug=False,
-            align_debug=False,
-        )  # shape: `[data_size x augmentation_size, beam_size]`
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", message="__floordiv__ is deprecated")
+
+            _, augmented_predictions = self.translator.translate(
+                src=augmented_batch,
+                src_feats=defaultdict(list),
+                tgt=None,
+                batch_size=2048,
+                batch_type="tokens",
+                attn_debug=False,
+                align_debug=False,
+            )  # shape: `[data_size x augmentation_size, beam_size]`
 
         # Step 4: Unravel and canonicalize.
         lines = []  # shape: `[data_size x augmentation_size x beam_size]`
         for i in range(len(augmented_predictions)):
             for j in range(len(augmented_predictions[i])):
                 lines.append(augmented_predictions[i][j].replace(" ", ""))
 
@@ -234,10 +246,12 @@
             rank = list(zip(rank.keys(), rank.values()))
             rank.sort(key=lambda x: x[1], reverse=True)
             rank = rank[:num_results]  # Truncate to `num_results` results.
             ranked_results.append([item[0][0] for item in rank])  # Output reactant SMILES.
             ranked_scores.append([item[1] for item in rank])  # Output scores used for ranking.
 
         return [
-            process_raw_smiles_outputs(input, outputs, self._build_kwargs_from_scores(scores))
+            process_raw_smiles_outputs_backwards(
+                input, outputs, self._build_kwargs_from_scores(scores)
+            )
             for input, outputs, scores in zip(inputs, ranked_results, ranked_scores)
         ]
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/models/retro_knn.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/models/retro_knn.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/utils/config.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,7 +51,11 @@
 
     # Make merged config options
     # CLI options take priority over YAML file options
     schema = OmegaConf.structured(config_cls)
     config = OmegaConf.merge(schema, *conf_yamls, conf_cli)
     OmegaConf.set_readonly(config, True)  # should not be written to
     return cast(R, config)
+
+
+def get_error_message_for_missing_value(name: str, possible_values: List[str]) -> str:
+    return f"{name} should be set to one of [{', '.join(possible_values)}]"
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/utils/downloading.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/downloading.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/utils/metrics.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/utils/model_loading.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/model_loading.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 import logging
 from typing import Union
 
+from omegaconf import OmegaConf
+
 from syntheseus.interface.models import ReactionModel
 from syntheseus.reaction_prediction.inference.config import BackwardModelConfig, ForwardModelConfig
 
 logger = logging.getLogger(__file__)
 
 
 def get_model(
-    config: Union[BackwardModelConfig, ForwardModelConfig], batch_size: int, num_gpus: int
+    config: Union[BackwardModelConfig, ForwardModelConfig],
+    batch_size: int,
+    num_gpus: int,
+    **model_kwargs,
 ) -> ReactionModel:
+    # Check that model kwargs don't overlap
+    overlapping_kwargs = set(config.model_kwargs.keys()) & set(model_kwargs.keys())
+    if overlapping_kwargs:
+        raise ValueError(f"Model kwargs overlap: {overlapping_kwargs}")
+
     def model_fn(device):
         return config.model_class.value(
-            model_dir=config.model_dir, device=device, **config.model_kwargs
+            model_dir=OmegaConf.select(config, "model_dir"),
+            device=device,
+            **config.model_kwargs,
+            **model_kwargs,
         )
 
     if num_gpus == 0:
         return model_fn("cpu")
     elif num_gpus == 1:
         return model_fn("cuda:0")
     else:
```

### Comparing `syntheseus-0.3.0/syntheseus/reaction_prediction/utils/parallel.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/utils/parallel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import math
-from typing import Callable, List
+from typing import Callable, List, Sequence
 
 import torch
 from more_itertools import chunked
 
-from syntheseus.interface.models import InputType, OutputType, PredictionList, ReactionModel
+from syntheseus.interface.models import InputType, ReactionModel, ReactionType
 
 
-class ParallelReactionModel(ReactionModel):
+class ParallelReactionModel(ReactionModel[InputType, ReactionType]):
     """Wraps an arbitrary `ReactionModel` to enable multi-GPU inference.
 
     Unlike most off-the-shelf multi-GPU approaches (e.g. strategies in `pytorch_lightning`,
     `nn.DataParallel`, `nn.DistributedDataParallel`), this class only handles inference (not
     training), and because of that it can be much looser in terms of the constraints the
     parallelized model has to satisfy. It also works with lists of inputs (chunking them up
     appropriately), whereas other approaches usually only work with tensors.
     """
 
     def __init__(self, model_fn: Callable, devices: List) -> None:
         self._devices = devices
         self._model_replicas = [model_fn(device=device) for device in devices]
 
-    def __call__(
+    def _get_reactions(
         self, inputs: List[InputType], num_results: int
-    ) -> List[PredictionList[InputType, OutputType]]:
+    ) -> List[Sequence[ReactionType]]:
         # Chunk up the inputs into (roughly) equal-sized chunks.
         chunk_size = math.ceil(len(inputs) / len(self._devices))
         input_chunks = list((input,) for input in chunked(inputs, chunk_size))
 
         # If `len(inputs)` is not divisible by `len(self._devices)` the last chunk may end up empty.
         num_chunks = len(input_chunks)
```

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/base.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
 import abc
 import math
 import random
 import warnings
-from collections.abc import Collection, Sequence
+from collections.abc import Collection
 from datetime import datetime
-from typing import Generic, Optional, TypeVar
+from typing import Generic, Optional, Sequence, TypeVar
 
+from syntheseus.interface.models import BackwardReactionModel
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search import INT_INF
-from syntheseus.search.chem import BackwardReaction, Molecule
 from syntheseus.search.graph.and_or import AndOrGraph, OrNode
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.message_passing import (
     depth_update,
     has_solution_update,
     run_message_passing,
 )
 from syntheseus.search.graph.molset import MolSetGraph, MolSetNode
 from syntheseus.search.graph.node import BaseGraphNode
 from syntheseus.search.mol_inventory import BaseMolInventory
-from syntheseus.search.reaction_models import BackwardReactionModel
 
 AlgReturnType = TypeVar("AlgReturnType")
 GraphType = TypeVar("GraphType", bound=RetrosynthesisSearchGraph)
 
 
 class MinimalSearchAlgorithm(Generic[GraphType, AlgReturnType], abc.ABC):
     """Defines minimal interface for search algorithms."""
@@ -65,14 +66,15 @@
     some common functions for all algorithms to reduce code duplication.
     """
 
     def __init__(
         self,
         limit_iterations: int = INT_INF,
         limit_reaction_model_calls: int = INT_INF,
+        limit_graph_nodes: int = INT_INF,
         time_limit_s: float = math.inf,
         max_expansion_depth: int = 50,
         expand_purchasable_mols: bool = False,
         set_depth: bool = True,
         set_has_solution: bool = True,
         unique_nodes: bool = False,
         random_state: Optional[random.Random] = None,
@@ -80,14 +82,15 @@
         stop_on_first_solution: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.limit_iterations = limit_iterations
         self.limit_reaction_model_calls = limit_reaction_model_calls
+        self.limit_graph_nodes = limit_graph_nodes
         self.time_limit_s = time_limit_s
         self.max_expansion_depth = max_expansion_depth
         self.expand_purchasable_mols = expand_purchasable_mols
         self.set_depth = set_depth
         self.set_has_solution = set_has_solution
         self.stop_on_first_solution = stop_on_first_solution
 
@@ -103,14 +106,21 @@
         self.prevent_repeat_mol_in_trees = prevent_repeat_mol_in_trees
         if self.unique_nodes and self.prevent_repeat_mol_in_trees:
             warnings.warn(
                 "prevent_repeat_mol_in_trees=True when unique_nodes=True is redundant"
                 " since the graph will not be a tree and there will be no repeat mols."
             )
 
+        # Warning about lack of caching in reaction model
+        if not self.reaction_model._use_cache:
+            warnings.warn(
+                "The reaction model does not use caching, which may result "
+                "in unnecessary duplicate calls with the same input molecule."
+            )
+
     @property
     def requires_tree(self) -> bool:
         """Whether this algorithm must be run on a tree."""
         return True
 
     def run_from_mol(self, mol: Molecule) -> tuple[GraphType, AlgReturnType]:
         graph = self.create_graph(mol)
@@ -164,14 +174,15 @@
         """
         elapsed_time = (
             datetime.now() - self._start_time
         ).total_seconds()  # NOTE: `self._start_time` is set in `setup`
         return (
             (elapsed_time >= self.time_limit_s)
             or (self.reaction_model.num_calls() >= self.limit_reaction_model_calls)
+            or (len(graph) >= self.limit_graph_nodes)
             or (self.stop_on_first_solution and graph.root_node.has_solution)
         )
 
     def set_node_values(
         self, nodes: Collection[BaseGraphNode], graph: GraphType
     ) -> Collection[BaseGraphNode]:
         """
@@ -221,16 +232,16 @@
 
     @abc.abstractmethod
     def _get_mols_to_expand(self, node: BaseGraphNode, graph: GraphType) -> Collection[Molecule]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _filter_reactions(
-        self, reactions: list[BackwardReaction], node: BaseGraphNode, graph: GraphType
-    ) -> list[BackwardReaction]:
+        self, reactions: Sequence[SingleProductReaction], node: BaseGraphNode, graph: GraphType
+    ) -> list[SingleProductReaction]:
         """Remove unwanted reactions from the list."""
         raise NotImplementedError
 
     def can_expand_node(self, node: BaseGraphNode, graph: GraphType) -> bool:
         """
         Return whether a node is eligible to be expanded. It is used by self.expand_node below,
         but is made available so that algorithms can check whether a node *would* be expanded.
@@ -314,16 +325,16 @@
             assert len(or_predecessors) == 1, "This graph is not a tree!"
             curr_node = or_predecessors[0]  # type: ignore
             assert isinstance(curr_node, OrNode)
             mols.add(curr_node.mol)
         return mols
 
     def _filter_reactions(
-        self, reactions: list[BackwardReaction], node: BaseGraphNode, graph: AndOrGraph
-    ) -> list[BackwardReaction]:
+        self, reactions: Sequence[SingleProductReaction], node: BaseGraphNode, graph: AndOrGraph
+    ) -> list[SingleProductReaction]:
         # Filter out any reactions that contain the root molecule
         reactions = [rxn for rxn in reactions if graph.root_node.mol not in rxn.reactants]
 
         # Optionally filter out A -> ... -> A ... cycles
         if self.prevent_repeat_mol_in_trees:
             assert isinstance(node, OrNode)
             ancestor_mols = self._get_tree_ancestor_mols(node, graph)
@@ -368,25 +379,26 @@
             parents = list(graph.predecessors(curr_node))
             assert len(parents) == 1, "This graph is not a tree!"
             curr_node = parents[0]
             molsets.add(curr_node.mols)
         return molsets
 
     def _filter_reactions(
-        self, reactions: list[BackwardReaction], node: BaseGraphNode, graph: MolSetGraph
-    ) -> list[BackwardReaction]:
+        self, reactions: Sequence[SingleProductReaction], node: BaseGraphNode, graph: MolSetGraph
+    ) -> list[SingleProductReaction]:
         # Filter out any reactions that contain the root molecule
         assert len(graph.root_node.mols) == 1
         root_mol = list(graph.root_node.mols)[0]
         reactions = [rxn for rxn in reactions if root_mol not in rxn.reactants]
 
         # Optionally filter out A -> B -> A ... cycles
         if self.prevent_repeat_mol_in_trees:
             assert isinstance(node, MolSetNode)
             ancestor_molsets = self._get_tree_ancestor_molsets(node, graph)
             reactions = [
                 rxn
                 for rxn in reactions
-                if frozenset((node.mols - {rxn.product}) | rxn.reactants) not in ancestor_molsets
+                if frozenset((node.mols - {rxn.product}) | rxn.unique_reactants)
+                not in ancestor_molsets
             ]
 
         return reactions
```

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/best_first/retro_star.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/best_first/retro_star.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 import math
-from collections.abc import Sequence
 
 # NOTE: Collection imported here instead of from collections.abc
 # to make casting work for python <3.9
 from typing import (
     Collection,
     Optional,
+    Sequence,
     cast,
 )
 
 from syntheseus.search.algorithms.base import AndOrSearchAlgorithm
 from syntheseus.search.algorithms.best_first.base import GeneralBestFirstSearch
 from syntheseus.search.algorithms.mixins import ValueFunctionMixin
 from syntheseus.search.graph.and_or import ANDOR_NODE, AndNode, AndOrGraph, OrNode
@@ -88,15 +88,15 @@
         )
         self._set_reaction_number_estimate(  # only for leaf nodes
             or_nodes=[
                 node
                 for node in output_nodes
                 if isinstance(node, OrNode)
                 and "reaction_number_estimate" not in node.data
-                and not node.is_expanded
+                and self.can_expand_node(node, graph)
             ],
             graph=graph,
         )
 
         # Run updates of reaction number and retro-star value
         return self._run_retro_star_updates(output_nodes, graph)
 
@@ -119,20 +119,37 @@
             node.data["reaction_number_estimate"] = cost
 
     def _run_retro_star_updates(
         self, nodes: Collection[ANDOR_NODE], graph: AndOrGraph
     ) -> Collection[ANDOR_NODE]:
         # Initialize all reaction numbers and retro star values
         for node in nodes:
-            node.data.setdefault("reaction_number", math.inf)
+            node.data.setdefault("retro_star_min_cost", math.inf)
+            node.data.setdefault("retro_star_reaction_number", math.inf)
             node.data.setdefault("retro_star_value", math.inf)
         nodes_to_update = set(cast(Collection[ANDOR_NODE], nodes))
 
         # NOTE: the following updates assume that depth is set correctly.
 
+        # Perform bottom-up update of `retro_star_min_cost`,
+        # sorting by decreasing depth and not updating children for efficiency
+        # (min cost depends only on children)
+        nodes_to_update.update(
+            cast(  # mypy doesn't know that `run_message_passing` returns a `Collection[ANDOR_NODE]`
+                Collection[ANDOR_NODE],
+                run_message_passing(
+                    graph=graph,
+                    nodes=sorted(nodes_to_update, key=lambda node: node.depth, reverse=True),
+                    update_fns=[min_cost_update],  # type: ignore[list-item]  # confusion about AndOrGraph type
+                    update_predecessors=True,
+                    update_successors=False,
+                ),
+            )
+        )
+
         # Perform bottom-up update of `reaction number`,
         # sorting by decreasing depth and not updating children for efficiency
         # (reaction number depends only on children)
         nodes_to_update.update(
             cast(  # mypy doesn't know that `run_message_passing` returns a `Collection[ANDOR_NODE]`
                 Collection[ANDOR_NODE],
                 run_message_passing(
@@ -160,44 +177,70 @@
                 ),
             )
         )
 
         return nodes_to_update
 
 
+def min_cost_update(node: ANDOR_NODE, graph: AndOrGraph) -> bool:
+    """
+    Updates a node's `retro_star_min_cost` value (minimum cost route found so far).
+
+    Returns whether the value changed.
+    """
+    if isinstance(node, AndNode):
+        new_cost = node.data["retro_star_rxn_cost"] + sum(
+            c.data["retro_star_min_cost"] for c in graph.successors(node)
+        )
+    elif isinstance(node, OrNode):
+        possible_costs = [node.data["retro_star_mol_cost"]] + [
+            c.data["retro_star_min_cost"] for c in graph.successors(node)
+        ]
+        new_cost = min(possible_costs)
+    else:
+        raise TypeError(f"Unexpected node type: {type(node)}")
+
+    # Do update and return whether the value changed
+    old_cost = node.data["retro_star_min_cost"]
+    node.data["retro_star_min_cost"] = new_cost
+    return not math.isclose(new_cost, old_cost)
+
+
 def reaction_number_update(node: ANDOR_NODE, graph: AndOrGraph) -> bool:
     """
     Updates a node's "reaction number", which is the current minimum cost
     estimate of synthesizing a molecule from everything below it.
     Returns whether the node's reaction number was updated.
     """
     if isinstance(node, AndNode):
         # Reaction number from equation 7 in Retro*
         new_rn = node.data["retro_star_rxn_cost"] + sum(
-            c.data["reaction_number"] for c in graph.successors(node)
+            c.data["retro_star_reaction_number"] for c in graph.successors(node)
         )
     elif isinstance(node, OrNode):
         # Reaction number is the minimum the molecule's purchase cost
         # and the cost of all child synthesis paths,
         # and potentially its reaction number estimate
         possible_costs = [node.data["retro_star_mol_cost"]]
         if node.is_expanded:
             # If the node is expanded, the cost of each child is also an option
-            possible_costs.extend([c.data["reaction_number"] for c in graph.successors(node)])
-        else:
+            possible_costs.extend(
+                [c.data["retro_star_reaction_number"] for c in graph.successors(node)]
+            )
+        elif "reaction_number_estimate" in node.data:
             # Otherwise the cost of the reaction number estimate is an option.
-            # This estimate must be present!
+            # By design, it will only be present if the node can be expanded
             possible_costs.append(node.data["reaction_number_estimate"])
         new_rn = min(possible_costs)
     else:
         raise TypeError(f"Unexpected node type: {type(node)}")
 
     # Do update and return whether the value changed
-    old_rn = node.data["reaction_number"]
-    node.data["reaction_number"] = new_rn
+    old_rn = node.data["retro_star_reaction_number"]
+    node.data["retro_star_reaction_number"] = new_rn
     return not math.isclose(new_rn, old_rn)
 
 
 def retro_star_value_update(node: ANDOR_NODE, graph: AndOrGraph) -> bool:
     """
     Updates a node's "retro_star_value",
     which is the lowest total cost of any tree containing this node,
@@ -213,31 +256,31 @@
         # Cost is parent's value, - any contributions from other AND branches,
         # + the current reaction number
         assert len(parents) == 1
         parent = parents[0]
         assert isinstance(parent, OrNode)
         new_value = (
             parent.data["retro_star_value"]
-            - parent.data["reaction_number"]
-            + node.data["reaction_number"]
+            - parent.data["retro_star_reaction_number"]
+            + node.data["retro_star_reaction_number"]
         )
 
         # Special cases to prevent NaNs
         # Could happen if things are initialized as infs,
         # or in certain cases with non-purchasable molecules.
         # In both cases the cause is inf-inf = nan
         if math.isnan(new_value):
             new_value = math.inf
 
     elif isinstance(node, OrNode):
         # r* Value estimate is parent's value (this has no double counting)
         # Except the root node: it's r* value estimate is just its RN
         if len(parents) == 0:
             # Root node
-            new_value = node.data["reaction_number"]
+            new_value = node.data["retro_star_reaction_number"]
         elif len(parents) == 1:
             # r* is parent's r*
             parent = parents[0]
             assert isinstance(parent, AndNode)
             new_value = parent.data["retro_star_value"]
         else:
             raise ValueError(
```

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/breadth_first.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/breadth_first.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/mcts/base.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/mcts/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import abc
 import logging
 import math
 import random
 import warnings
-from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Callable, Generic, Optional, TypeVar, cast
+from typing import Callable, Generic, Optional, Sequence, TypeVar, cast
 
 import numpy as np
 
 from syntheseus.search import INT_INF
 from syntheseus.search.algorithms.base import GraphType, SearchAlgorithm
 from syntheseus.search.algorithms.mixins import ValueFunctionMixin
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
@@ -134,23 +133,26 @@
         self._check_infinite_runtime()
 
     def _check_infinite_runtime(self) -> None:
         """Perform a check to see if the algorithm could run forever and warn the user."""
         no_limit_iter = self.limit_iterations >= INT_INF
         no_limit_rxn = self.limit_reaction_model_calls >= INT_INF
         no_limit_time = self.time_limit_s >= math.inf
+        no_limit_nodes = self.limit_graph_nodes >= INT_INF
 
-        if no_limit_iter and no_limit_rxn and no_limit_time:
+        if no_limit_iter and no_limit_rxn and no_limit_time and no_limit_nodes:
             warnings.warn(
                 "No kind of run limit set. This algorithm will almost certainty run forever."
             )
         elif no_limit_iter and no_limit_time:
             warnings.warn(
-                "No iteration or time limit set. It is possible (but not certain) that MCTS "
-                "will run forever with these settings. At the very least, it could run for a very long time."
+                "No iteration or time limit set (although a reaction model call and/or graph node limit was set)."
+                " Under these conditions, it is possible (but not certain) that MCTS "
+                "will run forever (for example if there are no leaf nodes eligible for expansion in the graph)."
+                " At the very least, it could run for an unexpectedly long time."
                 " It is recommended to set either an iteration limit or a time limit."
             )
 
     def setup(self, graph) -> None:
         # If there is only one node in the initial graph (the root node),
         # then the first visit will call the value function unnecessarily.
         # Save one call by doing a "pseudo-visit" and setting the value arbitrarily.
```

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/mixins.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/mixins.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/search/algorithms/pdvn.py` & `syntheseus-0.4.0/syntheseus/search/algorithms/pdvn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 """
 
 from __future__ import annotations
 
 import enum
 import math
 from collections import defaultdict
-from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Callable
+from typing import Callable, Sequence
 
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.algorithms.base import AndOrSearchAlgorithm
 from syntheseus.search.algorithms.mcts.base import BaseMCTS, pucb_bound
-from syntheseus.search.chem import BackwardReaction, Molecule
 from syntheseus.search.graph.and_or import ANDOR_NODE, AndNode, AndOrGraph, OrNode
 from syntheseus.search.graph.message_passing import (
     depth_update,
     has_solution_update,
     run_message_passing,
 )
 from syntheseus.search.node_evaluation import BaseNodeEvaluator
@@ -36,15 +36,15 @@
 
 @dataclass
 class PDVNSearchData:
     """Container for all data extracted from a search graph used to train policies/value functions in PDVN."""
 
     mol_to_synthesizability: dict[Molecule, SynthesizabilityOutcome]
     mol_to_min_syn_cost: dict[Molecule, float]
-    mol_to_reactions_for_min_syn: dict[Molecule, set[BackwardReaction]]
+    mol_to_reactions_for_min_syn: dict[Molecule, set[SingleProductReaction]]
 
 
 class PDVN_MCTS(BaseMCTS[AndOrGraph, OrNode, AndNode], AndOrSearchAlgorithm[int]):
     """
     Code for the MCTS algorithm used to train PDVN. It is essentially a modified version of MCTS
     for AND/OR trees. At an OrNode, a child reaction is selection using P-UCB. At and AndNode,
     one unsolved child is chosen. Two separate rewards are received: one for synthesis success,
```

### Comparing `syntheseus-0.3.0/syntheseus/search/analysis/diversity.py` & `syntheseus-0.4.0/syntheseus/search/analysis/diversity.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import logging
 import random
 from collections.abc import Collection
 from typing import Callable, Optional
 
 import networkx as nx
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.route import SynthesisGraph
 
 ROUTE_DISTANCE_METRIC = Callable[[SynthesisGraph, SynthesisGraph], float]
 
 logger = logging.getLogger(__name__)
 
 
@@ -209,15 +210,15 @@
 
     if union_size == 0:
         return 0.0  # both sets are empty so distance is 0
     else:
         return 1.0 - intersection_size / union_size
 
 
-def _get_reactions(route: SynthesisGraph) -> set[BackwardReaction]:
+def _get_reactions(route: SynthesisGraph) -> set[SingleProductReaction]:
     return set(route._graph.nodes)
 
 
 def _get_molecules(route: SynthesisGraph) -> set[Molecule]:
     all_mols: set[Molecule] = set()
     for rxn in route._graph.nodes:
         all_mols.add(rxn.product)
```

### Comparing `syntheseus-0.3.0/syntheseus/search/analysis/route_extraction.py` & `syntheseus-0.4.0/syntheseus/search/analysis/route_extraction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/search/analysis/solution_time.py` & `syntheseus-0.4.0/syntheseus/search/analysis/solution_time.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/and_or.py` & `syntheseus-0.4.0/syntheseus/search/graph/and_or.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import datetime
 from collections import Counter
-from collections.abc import Collection, Sequence
+from collections.abc import Collection
 from dataclasses import dataclass
-from typing import Optional, Union
+from typing import Optional, Sequence, Union
 
 import networkx as nx
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.node import BaseGraphNode
 from syntheseus.search.graph.route import SynthesisGraph
 
 
 @dataclass(eq=False)
 class _BaseOrNode:
@@ -36,15 +37,15 @@
 @dataclass(eq=False)
 class _BaseAndNode:
     """
     This class exists due to restrictions on inheriting from dataclasses.
     E.g. https://stackoverflow.com/questions/51575931/class-inheritance-in-python-3-7-dataclasses
     """
 
-    reaction: BackwardReaction
+    reaction: SingleProductReaction
 
 
 @dataclass(eq=False)
 class AndNode(BaseGraphNode, _BaseAndNode):
     def _has_intrinsic_solution(self) -> bool:
         return False
 
@@ -102,17 +103,19 @@
                 # Parents should be OrNodes whose mol is the reaction product
                 for parent in self.predecessors(node):
                     assert isinstance(parent, OrNode)
                     assert parent.mol == node.reaction.product
 
                 # Should be 1 child OrNode for each reactant
                 all_children = list(self.successors(node))
-                assert len(all_children) == len(
-                    node.reaction.reactants
-                ), "Should have 1 child per reactant."
+                assert len(all_children) == len(node.reaction.unique_reactants), (
+                    f"Should have 1 child per reactant, but found {len(all_children)} "
+                    f"children for {len(node.reaction.unique_reactants)} reactants."
+                )
+
                 for child in all_children:
                     assert isinstance(child, OrNode)
                 assert set(child.mol for child in all_children) == set(node.reaction.reactants)  # type: ignore  # does not understand that all children are OrNode
             else:
                 raise TypeError(f"Unexpected node type: {type(node)}")
 
     def assert_validity(self) -> None:
@@ -126,15 +129,15 @@
             )
         else:
             # Check that this dictionary is empty (i.e. not used)
             assert len(self._mol_to_node) == 0
 
     def expand_with_reactions(  # type: ignore[override]  # because it only accepts OrNodes
         self,
-        reactions: list[BackwardReaction],
+        reactions: list[SingleProductReaction],
         node: OrNode,
         ensure_tree: bool,  # raises an error if something is done to make the graph no longer a tree
     ) -> Sequence[ANDOR_NODE]:
         # Check that parent is in the graph already
         assert node in self
 
         # Check that reactions are acceptable
@@ -158,15 +161,15 @@
                 creation_time=creation_time,
                 is_expanded=True,
             )
             self._graph.add_node(and_node)
             new_nodes.append(and_node)
             self._graph.add_edge(node, and_node)
 
-            for reactant_mol in reaction.reactants:
+            for reactant_mol in reaction.unique_reactants:
                 if reactant_mol in self._mol_to_node:
                     or_node = self._mol_to_node[reactant_mol]
                 else:
                     or_node = OrNode(
                         mol=reactant_mol,
                         creation_time=creation_time,
                     )
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/base_graph.py` & `syntheseus-0.4.0/syntheseus/search/graph/base_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import abc
-from collections.abc import Container, Iterable, Sequence, Sized
-from typing import Generic, TypeVar
+from collections.abc import Container, Iterable, Sized
+from typing import Generic, Sequence, TypeVar
 
 import networkx as nx
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.node import BaseGraphNode
 
 NodeType = TypeVar(
     "NodeType",
 )
 SearchNodeType = TypeVar("SearchNodeType", bound=BaseGraphNode)
 
@@ -97,15 +98,15 @@
             )
         else:
             return False
 
     @abc.abstractmethod
     def expand_with_reactions(
         self,
-        reactions: list[BackwardReaction],
+        reactions: list[SingleProductReaction],
         node: NodeType,
         ensure_tree: bool,
     ) -> Sequence[NodeType]:
         """
         Expands a node with a series of reactions.
         For reproducibility, it ensures that the order of the nodes is consistent,
         which is why a sequence is returned.
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/message_passing/run.py` & `syntheseus-0.4.0/syntheseus/search/graph/message_passing/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from collections import deque
-from collections.abc import Collection, Iterable, Sequence
-from typing import Callable, TypeVar
+from collections.abc import Collection, Iterable
+from typing import Callable, Sequence, TypeVar
 
 from syntheseus.search import INT_INF
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.node import BaseGraphNode
 
 NodeType = TypeVar("NodeType", bound=BaseGraphNode)
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/message_passing/update_functions.py` & `syntheseus-0.4.0/syntheseus/search/graph/message_passing/update_functions.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/molset.py` & `syntheseus-0.4.0/syntheseus/search/graph/molset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import datetime
 import warnings
 from collections import Counter
-from collections.abc import Collection, Sequence
+from collections.abc import Collection
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Sequence
 
 import networkx as nx
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.node import BaseGraphNode
 from syntheseus.search.graph.route import SynthesisGraph
 
 
 @dataclass(eq=False)
 class _BaseMolSetNode:
@@ -87,19 +88,19 @@
         # Check reactants and products match
         for node in self._graph.nodes:
             assert isinstance(node, MolSetNode)
             for child_node in self.successors(node):
                 edge_data = self._graph.get_edge_data(node, child_node)
                 assert "reaction" in edge_data
                 rxn = edge_data["reaction"]
-                assert ((set(node.mols) - {rxn.product}) | rxn.reactants) == child_node.mols
+                assert ((set(node.mols) - {rxn.product}) | rxn.unique_reactants) == child_node.mols
 
     def expand_with_reactions(
         self,
-        reactions: list[BackwardReaction],
+        reactions: list[SingleProductReaction],
         node: MolSetNode,
         ensure_tree: bool,
     ) -> Sequence[MolSetNode]:
         if not ensure_tree:
             warnings.warn("ensure_tree=False is not well-tested so be careful!")
 
         # Check that parent is in the graph already
@@ -115,15 +116,17 @@
         assert not node.is_expanded
 
         # Create and add nodes one at a time
         creation_time = datetime.datetime.now(datetime.timezone.utc)
         new_nodes: list[MolSetNode] = list()
         node.is_expanded = True
         for reaction in reactions:
-            new_mol_set = frozenset((set(node.mols) - {reaction.product}) | reaction.reactants)
+            new_mol_set = frozenset(
+                (set(node.mols) - {reaction.product}) | reaction.unique_reactants
+            )
             if new_mol_set in self._molset_to_node:
                 new_node = self._molset_to_node[new_mol_set]
             else:
                 new_node = MolSetNode(
                     mols=new_mol_set,
                     creation_time=creation_time,
                 )
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/node.py` & `syntheseus-0.4.0/syntheseus/search/graph/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     # General
     # ==================================================
     policy_score: float
 
     # ==================================================
     # Retro*
     # ==================================================
-    reaction_number: float
+    retro_star_min_cost: float  # minimum cost found so far
+    retro_star_reaction_number: float
     reaction_number_estimate: float
     retro_star_value: float
     retro_star_rxn_cost: float
     retro_star_mol_cost: float
 
     # ==================================================
     # MCTS
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/route.py` & `syntheseus-0.4.0/syntheseus/search/graph/route.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from __future__ import annotations
 
 from collections import Counter
-from collections.abc import Sequence
-from typing import Union
+from typing import Sequence, Union
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.base_graph import BaseReactionGraph
 
-MOL_AND_RXN = Union[Molecule, BackwardReaction]
+MOL_AND_RXN = Union[Molecule, SingleProductReaction]
 
 
-class SynthesisGraph(BaseReactionGraph[BackwardReaction]):
+class SynthesisGraph(BaseReactionGraph[SingleProductReaction]):
     """
     Data structure used to hold a retrosynthesis graph containing only
     reaction objects. The purpose of this class is as a minimal container
     for route objects, instead of storing them as AndOrGraphs or MolSetGraphs.
     """
 
-    def __init__(self, root_node: BackwardReaction, **kwargs) -> None:
+    def __init__(self, root_node: SingleProductReaction, **kwargs) -> None:
         super().__init__(**kwargs)
         self._root_node = root_node
         self._graph.add_node(self._root_node)
 
     @property
-    def root_node(self) -> BackwardReaction:
+    def root_node(self) -> SingleProductReaction:
         return self._root_node
 
     @property
     def root_mol(self) -> Molecule:
         return self.root_node.product
 
     def is_minimal(self) -> bool:
@@ -39,40 +39,40 @@
         return True
 
     def assert_validity(self) -> None:
         # Everything from superclass applies
         super().assert_validity()
 
         for node in self._graph.nodes:
-            assert isinstance(node, BackwardReaction)
+            assert isinstance(node, SingleProductReaction)
             for parent in self.predecessors(node):
-                assert isinstance(parent, BackwardReaction)
+                assert isinstance(parent, SingleProductReaction)
                 assert node.product in parent.reactants
             children = list(self.successors(node))
             assert len(children) == len(set(children))  # all children should be unique
             assert set([child.product for child in children]) <= set(
                 node.reactants
             )  # all children should be reactants
 
     def expand_with_reactions(
         self,
-        reactions: list[BackwardReaction],
-        node: BackwardReaction,
+        reactions: list[SingleProductReaction],
+        node: SingleProductReaction,
         ensure_tree: bool,
-    ) -> Sequence[BackwardReaction]:
+    ) -> Sequence[SingleProductReaction]:
         raise NotImplementedError
 
     def get_starting_molecules(self) -> set[Molecule]:
         """
         Get the 'starting molecules' for this route,
         i.e. reactant molecules which are not a product of a child reaction.
         """
         output: set[Molecule] = set()
         for rxn in self._graph.nodes:
             successor_products = {child_rxn.product for child_rxn in self.successors(rxn)}
-            for reactant in rxn.reactants:
+            for reactant in rxn.unique_reactants:
                 if reactant not in successor_products:
                     output.add(reactant)
         return output
 
     def __str__(self) -> str:
         return str([rxn.reaction_smiles for rxn in self.nodes()])
```

### Comparing `syntheseus-0.3.0/syntheseus/search/graph/standardization.py` & `syntheseus-0.4.0/syntheseus/search/graph/standardization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 from __future__ import annotations
 
 import math
 import warnings
 from typing import cast
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.and_or import ANDOR_NODE, AndNode, AndOrGraph, OrNode
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.message_passing import (
     depth_update,
     has_solution_update,
     run_message_passing,
 )
 from syntheseus.search.graph.molset import MolSetGraph, MolSetNode
 
 
 def _make_unique_node_andor_graph(
     root_mol: Molecule,
     mol_to_node: dict[Molecule, OrNode],
-    rxn_to_node: dict[BackwardReaction, AndNode],
+    rxn_to_node: dict[SingleProductReaction, AndNode],
 ) -> AndOrGraph:
     # Make new graph
     new_graph = AndOrGraph(root_node=mol_to_node[root_mol], one_node_per_molecule=True)
 
     # Add all nodes
     new_graph._graph.add_nodes_from(mol_to_node.values())
     new_graph._graph.add_nodes_from(rxn_to_node.values())
     new_graph._mol_to_node.update(mol_to_node)
 
     # Add all edges
     for rxn, and_node in rxn_to_node.items():
         new_graph._graph.add_edge(mol_to_node[rxn.product], and_node)
-        for reactant in rxn.reactants:
+        for reactant in rxn.unique_reactants:
             new_graph._graph.add_edge(and_node, mol_to_node[reactant])
 
         # Mark relevant nodes as expanded
         mol_to_node[rxn.product].is_expanded = True
         and_node.is_expanded = True
 
     # Validate graph (should be valid at this point)
```

### Comparing `syntheseus-0.3.0/syntheseus/search/mol_inventory.py` & `syntheseus-0.4.0/syntheseus/search/mol_inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import abc
 from collections.abc import Collection
 
-from syntheseus.search.chem import Molecule
+from syntheseus.interface.molecule import Molecule
 
 
 class BaseMolInventory(abc.ABC):
     @abc.abstractmethod
     def is_purchasable(self, mol: Molecule) -> bool:
         """Whether or not a molecule is purchasable."""
         raise NotImplementedError
```

### Comparing `syntheseus-0.3.0/syntheseus/search/node_evaluation/base.py` & `syntheseus-0.4.0/syntheseus/search/node_evaluation/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import abc
-from collections.abc import Sequence
-from typing import Generic, Optional, TypeVar
+from typing import Generic, Optional, Sequence, TypeVar
 
 import numpy as np
 
-from syntheseus.search.chem import BackwardReaction
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.node import BaseGraphNode
 
 NodeType = TypeVar("NodeType", bound=BaseGraphNode)
 
 
 class BaseNodeEvaluator(Generic[NodeType], abc.ABC):
@@ -126,15 +125,15 @@
         self._return_log = return_log
         self._normalize = normalize
         self._temperature = temperature
         self._clip_probability_min = clip_probability_min
         self._clip_probability_max = clip_probability_max
 
     @abc.abstractmethod
-    def _get_reaction(self, node, graph) -> BackwardReaction:
+    def _get_reaction(self, node, graph) -> SingleProductReaction:
         pass
 
     def _get_probability(self, node, graph) -> float:
         metadata = self._get_reaction(node, graph).metadata
 
         if "probability" not in metadata:
             raise ValueError("Cannot call node evaluator as reaction model probability is not set")
```

### Comparing `syntheseus-0.3.0/syntheseus/search/node_evaluation/common.py` & `syntheseus-0.4.0/syntheseus/search/node_evaluation/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Common node evaluation functions."""
 
 from __future__ import annotations
 
-from collections.abc import Sequence
-from typing import Union
+from typing import Sequence, Union
 
-from syntheseus.search.chem import BackwardReaction
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.and_or import AndNode
 from syntheseus.search.graph.molset import MolSetNode
 from syntheseus.search.node_evaluation.base import NoCacheNodeEvaluator, ReactionModelBasedEvaluator
 
 
 class ConstantNodeEvaluator(NoCacheNodeEvaluator):
     def __init__(self, constant: float, **kwargs):
@@ -27,29 +26,29 @@
 
 class ReactionModelLogProbCost(ReactionModelBasedEvaluator[AndNode]):
     """Evaluator that uses the reactions' negative logprob to form a cost (useful for Retro*)."""
 
     def __init__(self, **kwargs) -> None:
         super().__init__(return_log=True, **kwargs)
 
-    def _get_reaction(self, node: AndNode, graph) -> BackwardReaction:
+    def _get_reaction(self, node: AndNode, graph) -> SingleProductReaction:
         return node.reaction
 
     def _evaluate_nodes(self, nodes, graph=None) -> Sequence[float]:
         return [-v for v in super()._evaluate_nodes(nodes, graph)]
 
 
 class ReactionModelProbPolicy(ReactionModelBasedEvaluator[Union[MolSetNode, AndNode]]):
     """Evaluator that uses the reactions' probability to form a policy (useful for MCTS)."""
 
     def __init__(self, **kwargs) -> None:
         kwargs["normalize"] = kwargs.get("normalize", True)  # set `normalize = True` by default
         super().__init__(return_log=False, **kwargs)
 
-    def _get_reaction(self, node: Union[MolSetNode, AndNode], graph) -> BackwardReaction:
+    def _get_reaction(self, node: Union[MolSetNode, AndNode], graph) -> SingleProductReaction:
         if isinstance(node, MolSetNode):
             parents = list(graph.predecessors(node))
             assert len(parents) == 1, "Graph must be a tree"
             return graph._graph.edges[parents[0], node]["reaction"]
         elif isinstance(node, AndNode):
             return node.reaction
         else:
```

### Comparing `syntheseus-0.3.0/syntheseus/search/reaction_models/toy.py` & `syntheseus-0.4.0/syntheseus/reaction_prediction/inference/toy_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from __future__ import annotations
 
-from collections.abc import Sequence
+from typing import Sequence
 
-from syntheseus.search.chem import BackwardReaction, Molecule
-from syntheseus.search.reaction_models.base import BackwardReactionModel
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.models import BackwardReactionModel
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 
 
-class ListOfReactionsModel(BackwardReactionModel):
+class ListOfReactionsToyModel(BackwardReactionModel):
     """A model which returns reactions from a pre-defined list."""
 
-    def __init__(self, reaction_list: Sequence[BackwardReaction], **kwargs) -> None:
+    def __init__(self, reaction_list: Sequence[SingleProductReaction], **kwargs) -> None:
         super().__init__(**kwargs)
         self.reaction_list = list(reaction_list)
 
-    def _get_backward_reactions(self, mols: list[Molecule]) -> list[list[BackwardReaction]]:
-        return [[r for r in self.reaction_list if r.product == mol] for mol in mols]
+    def _get_reactions(
+        self, inputs: list[Molecule], num_results: int
+    ) -> list[Sequence[SingleProductReaction]]:
+        return [[r for r in self.reaction_list if r.product == mol] for mol in inputs]
 
 
-class LinearMolecules(BackwardReactionModel):
+class LinearMoleculesToyModel(BackwardReactionModel):
     """
     A simple toy model of "reactions" on linear "ball-and-stick" molecules,
     where the possible reactions involve string cuts and substitutions.
 
     Molecules in this model must be formed entirely from C,S, and O atoms with single bonds.
     The reactions allowed are:
     - string cuts, e.g. "CCOC" -> "CC" + "OC" (*see note 2 below)
@@ -36,27 +40,27 @@
     since "CO" and "OC" are the same molecule, but it may be confusing when debugging.
     """
 
     def __init__(self, allow_substitution: bool = True, **kwargs) -> None:
         super().__init__(**kwargs)
         self._allow_substitution = allow_substitution  # should not be modified after init
 
-    def _get_single_backward_reactions(self, mol: Molecule) -> list[BackwardReaction]:
+    def _get_single_backward_reactions(self, mol: Molecule) -> list[SingleProductReaction]:
         assert set(mol.smiles) <= set("COS"), "Molecules must be formed out of C,O, and S atoms."
         assert len(mol.smiles) > 0, "Molecules must have at least 1 atom."
-        output: list[BackwardReaction] = []
+        output: list[SingleProductReaction] = []
 
         # String cuts
         for cut_idx in range(1, len(mol.smiles)):
             mol1 = Molecule(mol.smiles[:cut_idx], make_rdkit_mol=False)
             mol2 = Molecule(mol.smiles[cut_idx:], make_rdkit_mol=False)
             output.append(
-                BackwardReaction(
+                SingleProductReaction(
                     product=mol,
-                    reactants=frozenset([mol1, mol2]),
+                    reactants=Bag({mol1, mol2}),  # don't include duplicates
                     metadata={"source": f"string cut at idx {cut_idx}"},
                 )
             )
 
         # Substitutions
         if self._allow_substitution:
             for sub_idx in {0, len(mol.smiles) - 1}:  # use set in case len(mol.smiles) == 1
@@ -65,18 +69,20 @@
                         continue
                     else:
                         new_mol = Molecule(
                             mol.smiles[:sub_idx] + sub_atom + mol.smiles[sub_idx + 1 :],
                             make_rdkit_mol=False,
                         )
                         output.append(
-                            BackwardReaction(
+                            SingleProductReaction(
                                 product=mol,
-                                reactants=frozenset([new_mol]),
+                                reactants=Bag([new_mol]),
                                 metadata={"source": f"substitution idx {sub_idx} with {sub_atom}"},
                             ),
                         )
 
         return output
 
-    def _get_backward_reactions(self, mols: list[Molecule]) -> list[list[BackwardReaction]]:
-        return [self._get_single_backward_reactions(mol) for mol in mols]
+    def _get_reactions(
+        self, inputs: list[Molecule], num_results: int
+    ) -> list[Sequence[SingleProductReaction]]:
+        return [self._get_single_backward_reactions(mol) for mol in inputs]
```

### Comparing `syntheseus-0.3.0/syntheseus/search/visualization.py` & `syntheseus-0.4.0/syntheseus/search/visualization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/interface/test_bag.py` & `syntheseus-0.4.0/syntheseus/tests/interface/test_bag.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/reaction_prediction/chem/test_utils.py` & `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/chem/test_utils.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/reaction_prediction/data/test_dataset.py` & `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/data/test_dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,85 @@
 import csv
+import os
 from pathlib import Path
+from typing import Generator
 
 import pytest
 
 from syntheseus.interface.bag import Bag
 from syntheseus.interface.molecule import Molecule
 from syntheseus.reaction_prediction.data.dataset import (
     CSV_REACTION_SMILES_COLUMN_NAME,
     DataFold,
     DataFormat,
     DiskReactionDataset,
 )
 from syntheseus.reaction_prediction.data.reaction_sample import ReactionSample
 
 
+@pytest.fixture(params=[False, True])
+def temp_path(request, tmp_path: Path) -> Generator[Path, None, None]:
+    """Fixture to provide a temporary path that is either absolute or relative."""
+    if request.param:
+        # The built-in `tmp_path` fixture is absolute; if the fixture parameter is `True` we convert
+        # that to a relative path. This is done by stripping away the root `/` that signifies an
+        # absolute path and changing the working directory to `/` so that the path remains correct.
+
+        old_working_dir = os.getcwd()
+        os.chdir("/")
+
+        yield Path(*list(tmp_path.parts)[1:])
+
+        os.chdir(old_working_dir)
+    else:
+        yield tmp_path
+
+
 @pytest.mark.parametrize("mapped", [False, True])
-def test_save_and_load(tmp_path: Path, mapped: bool) -> None:
+def test_save_and_load(temp_path: Path, mapped: bool) -> None:
     samples = [
         ReactionSample.from_reaction_smiles_strict(reaction_smiles, mapped=mapped)
         for reaction_smiles in [
             "O[c:1]1[cH:2][c:3](=[O:4])[nH:5][cH:6][cH:7]1>>[cH:1]1[cH:2][c:3](=[O:4])[nH:5][cH:6][cH:7]1",
             "CC(C)(C)OC(=O)[N:1]1[CH2:2][CH2:3][C@H:4]([F:5])[CH2:6]1>>[NH:1]1[CH2:2][CH2:3][C@H:4]([F:5])[CH2:6]1",
         ]
     ]
 
     for fold in DataFold:
-        DiskReactionDataset.save_samples_to_file(data_dir=tmp_path, fold=fold, samples=samples)
+        DiskReactionDataset.save_samples_to_file(data_dir=temp_path, fold=fold, samples=samples)
 
     for load_format in [None, DataFormat.JSONL]:
         # Now try to load the data we just saved.
-        dataset = DiskReactionDataset(tmp_path, sample_cls=ReactionSample, data_format=load_format)
+        dataset = DiskReactionDataset(temp_path, sample_cls=ReactionSample, data_format=load_format)
 
         for fold in DataFold:
             assert list(dataset[fold]) == samples
 
 
 @pytest.mark.parametrize("format", [DataFormat.CSV, DataFormat.SMILES])
-def test_load_external_format(tmp_path: Path, format: DataFormat) -> None:
+def test_load_external_format(temp_path: Path, format: DataFormat) -> None:
     # Example reaction SMILES, purposefully using non-canonical forms of reactants and product.
     reaction_smiles = (
         "[cH:1]1[cH:2][c:3]([CH3:4])[cH:5][cH:6][c:7]1Br.B(O)(O)[c:8]1[cH:9][cH:10][c:11]([CH3:12])[cH:13][cH:14]1>>"
         "[cH:1]1[cH:2][c:3]([CH3:4])[cH:5][cH:6][c:7]1[c:8]2[cH:14][cH:13][c:11]([CH3:12])[cH:10][cH:9]2"
     )
 
     filename = DiskReactionDataset.get_filename_suffix(format=format, fold=DataFold.TRAIN)
-    with open(tmp_path / filename, "wt") as f:
+    with open(temp_path / filename, "wt") as f:
         if format == DataFormat.CSV:
             writer = csv.DictWriter(f, fieldnames=["id", "class", CSV_REACTION_SMILES_COLUMN_NAME])
             writer.writeheader()
             writer.writerow(
                 {"id": 0, "class": "UNK", CSV_REACTION_SMILES_COLUMN_NAME: reaction_smiles}
             )
         else:
             f.write(f"{reaction_smiles}\n")
 
     for load_format in [None, format]:
-        dataset = DiskReactionDataset(tmp_path, sample_cls=ReactionSample, data_format=load_format)
+        dataset = DiskReactionDataset(temp_path, sample_cls=ReactionSample, data_format=load_format)
         assert dataset.get_num_samples(DataFold.TRAIN) == 1
 
         samples = list(dataset[DataFold.TRAIN])
         assert len(samples) == 1
 
         [sample] = samples
 
@@ -71,35 +91,35 @@
         )
 
         # The original reaction SMILES should have been saved separately.
         assert sample.mapped_reaction_smiles == reaction_smiles
 
 
 @pytest.mark.parametrize("format", [DataFormat.JSONL, DataFormat.CSV, DataFormat.SMILES])
-def test_format_detection(tmp_path: Path, format: DataFormat) -> None:
+def test_format_detection(temp_path: Path, format: DataFormat) -> None:
     other_format = (set(DataFormat) - {format}).pop()
 
     # Create two files with different extensions, so that it is ambiguous which format we want.
-    (tmp_path / DiskReactionDataset.get_filename_suffix(format, DataFold.TRAIN)).touch()
-    (tmp_path / DiskReactionDataset.get_filename_suffix(other_format, DataFold.TEST)).touch()
+    (temp_path / DiskReactionDataset.get_filename_suffix(format, DataFold.TRAIN)).touch()
+    (temp_path / DiskReactionDataset.get_filename_suffix(other_format, DataFold.TEST)).touch()
 
     # Loading with automatic resolution should fail.
     with pytest.raises(ValueError):
-        DiskReactionDataset(data_dir=tmp_path, sample_cls=ReactionSample)
+        DiskReactionDataset(data_dir=temp_path, sample_cls=ReactionSample)
 
     # Loading with an explicit format should succeed.
     for f in [format, other_format]:
-        DiskReactionDataset(data_dir=tmp_path, sample_cls=ReactionSample, data_format=f)
+        DiskReactionDataset(data_dir=temp_path, sample_cls=ReactionSample, data_format=f)
 
     # Loading with an explicit format but no matching files should fail.
     another_format = (set(DataFormat) - {format, other_format}).pop()
     with pytest.raises(ValueError):
         DiskReactionDataset(
-            data_dir=tmp_path, sample_cls=ReactionSample, data_format=another_format
+            data_dir=temp_path, sample_cls=ReactionSample, data_format=another_format
         )
 
     # Create another file with the right suffix.
-    (tmp_path / f"raw_{DiskReactionDataset.get_filename_suffix(format, DataFold.TRAIN)}").touch()
+    (temp_path / f"raw_{DiskReactionDataset.get_filename_suffix(format, DataFold.TRAIN)}").touch()
 
     # Loading with an explicit format should now fail due to ambiguity.
     with pytest.raises(ValueError):
-        DiskReactionDataset(data_dir=tmp_path, sample_cls=ReactionSample, data_format=format)
+        DiskReactionDataset(data_dir=temp_path, sample_cls=ReactionSample, data_format=format)
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/reaction_prediction/utils/test_misc.py` & `syntheseus-0.4.0/syntheseus/tests/reaction_prediction/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_base.py` & `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import abc
 import datetime
 import math
 import warnings
 
 import pytest
 
+from syntheseus.interface.molecule import Molecule
 from syntheseus.search import INT_INF
 from syntheseus.search.algorithms.base import SearchAlgorithm
 from syntheseus.search.analysis.route_extraction import iter_routes_cost_order
 from syntheseus.search.analysis.solution_time import get_first_solution_time
-from syntheseus.search.chem import Molecule
 from syntheseus.search.graph.and_or import AndNode, AndOrGraph, OrNode
 from syntheseus.search.graph.base_graph import RetrosynthesisSearchGraph
 from syntheseus.search.graph.message_passing import has_solution_update, run_message_passing
 from syntheseus.search.graph.molset import MolSetGraph, MolSetNode
 from syntheseus.search.graph.route import SynthesisGraph
 from syntheseus.search.mol_inventory import SmilesListInventory
 from syntheseus.tests.search.conftest import RetrosynthesisTask
@@ -153,14 +153,53 @@
             # This can happen if the last node to expand has more more than one molecule to be expanded
             # (e.g. 9/10 budget used up and the last node has 2 molecules to expand)
             assert alg.reaction_model.num_calls() in {limit, limit + 1}
         else:
             # Default case is to match exactly
             assert alg.reaction_model.num_calls() == limit
 
+    @pytest.mark.parametrize("limit", [0, 1, 2, 25, 100])
+    def test_limit_graph_nodes(
+        self,
+        retrosynthesis_task6: RetrosynthesisTask,
+        limit: int,
+    ) -> None:
+        """
+        Test that limiting the number of nodes in the graph works as intended.
+        The algorithm should run until the node limit is reached, and then stop
+        (without adding *too many* extra nodes).
+
+        `retrosynthesis_task6` is chosen because it can create a very large graph.
+        """
+
+        # Run algorithm
+        alg = self.setup_algorithm(
+            reaction_model=retrosynthesis_task6.reaction_model,
+            mol_inventory=retrosynthesis_task6.inventory,
+            limit_graph_nodes=limit,
+            limit_iterations=int(1e6),  # a very high limit, but avoids MCTS warnings
+        )
+        output_graph, _ = alg.run_from_mol(retrosynthesis_task6.target_mol)
+
+        # The algorithm will stop running when the graph size meets or exceeds the limit.
+        # However, since multiple nodes are added during each expansion, the node count might
+        # not exactly equal the limit. Therefore, we choose a variable tolerance.
+        # "Tolerance" here is len(graph) - limit
+        if limit == 0:
+            tolerance = 1  # will stop search immediately with only the root node
+        elif limit == 1:
+            tolerance = 0  # should not expand root node
+        elif limit == 2:
+            tolerance = 19  # a very high number, since first expansion brings node count to 21 for AND/OR graphs
+        else:
+            tolerance = 20  # a fairly high tolerance (should always be enough for one expansion)
+
+        # The actual test
+        assert limit <= len(output_graph) <= tolerance + limit
+
     @pytest.mark.parametrize("limit", [0, 1, 2, 100])
     def test_limit_iterations(
         self,
         retrosynthesis_task1: RetrosynthesisTask,
         retrosynthesis_task2: RetrosynthesisTask,
         retrosynthesis_task3: RetrosynthesisTask,
         limit: int,
@@ -188,15 +227,15 @@
             assert tasks_solved == [True, False, False]
 
         elif limit == 2:
             # The first task should be solved and the last task should not be solved. Second task may or may not be solved.
             assert tasks_solved[0]
             assert not tasks_solved[2]
 
-        elif limit == 100:
+        elif limit >= 100:
             # With this high number of iterations all tasks should be solved
             assert tasks_solved == [True, True, True]
 
         else:
             # this is just to make sure no tests are skipped accidentally by raising an error if the limit list
             # is changed without adding a corresponding elif clause here
             raise ValueError(f"Case of limit={limit} is not handled.")
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_best_first.py` & `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_best_first.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             "CO>>CC": 1,
             "CS>>CC": 1,
         }
         assert len(output_graph) == 7
         assert not output_graph.root_node.has_solution
         assert get_first_solution_time(output_graph) == math.inf
         assert math.isclose(output_graph.root_node.data["retro_star_value"], 0.6)
-        assert math.isclose(output_graph.root_node.data["reaction_number"], 0.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_reaction_number"], 0.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_min_cost"], math.inf)
         assert_retro_star_values_in_graph(output_graph, [1.9, 0.6, 1.1])
 
     def test_by_hand_step2(
         self,
         retrosynthesis_task5: RetrosynthesisTask,
         rxn_cost_fn: DictRxnCost,
         mol_value_fn: DictMolCost,
@@ -156,15 +157,16 @@
             "OS>>CO": 1,
             "CS>>CO": 1,
         }
         assert len(output_graph) == 16
         assert not output_graph.root_node.has_solution
         assert get_first_solution_time(output_graph) == math.inf
         assert math.isclose(output_graph.root_node.data["retro_star_value"], 0.6)
-        assert math.isclose(output_graph.root_node.data["reaction_number"], 0.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_reaction_number"], 0.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_min_cost"], math.inf)
         assert_retro_star_values_in_graph(output_graph, [5.6, 1.1, 0.6, 1.9])
 
     def test_by_hand_step3(
         self,
         retrosynthesis_task5: RetrosynthesisTask,
         rxn_cost_fn: DictRxnCost,
         mol_value_fn: DictMolCost,
@@ -201,15 +203,16 @@
             "CO>>OO": 1,
             "OS>>OO": 1,
         }
         assert len(output_graph) == 22
         assert output_graph.root_node.has_solution
         assert get_first_solution_time(output_graph) == 3
         assert math.isclose(output_graph.root_node.data["retro_star_value"], 1.1)
-        assert math.isclose(output_graph.root_node.data["reaction_number"], 1.1)
+        assert math.isclose(output_graph.root_node.data["retro_star_reaction_number"], 1.1)
+        assert math.isclose(output_graph.root_node.data["retro_star_min_cost"], 2.6)
         assert_retro_star_values_in_graph(output_graph, [5.6, 1.1, 2.6, 1.9, 5.7])
 
     def test_by_hand_step4(
         self,
         retrosynthesis_task5: RetrosynthesisTask,
         rxn_cost_fn: DictRxnCost,
         mol_value_fn: DictMolCost,
@@ -251,15 +254,16 @@
             "SS>>CS": 1,
             "CO>>CS": 1,
         }
         assert len(output_graph) == 31
         assert output_graph.root_node.has_solution
         assert get_first_solution_time(output_graph) == 3
         assert math.isclose(output_graph.root_node.data["retro_star_value"], 1.9)
-        assert math.isclose(output_graph.root_node.data["reaction_number"], 1.9)
+        assert math.isclose(output_graph.root_node.data["retro_star_reaction_number"], 1.9)
+        assert math.isclose(output_graph.root_node.data["retro_star_min_cost"], 2.6)
         assert_retro_star_values_in_graph(output_graph, [1.9, 5.6, 2.6, 2.1, 5.7])
 
     def test_by_hand_step5(
         self,
         retrosynthesis_task5: RetrosynthesisTask,
         rxn_cost_fn: DictRxnCost,
         mol_value_fn: DictMolCost,
@@ -300,9 +304,10 @@
             "O>>C": 1,
             "S>>C": 1,
         }
         assert len(output_graph) == 35
         assert output_graph.root_node.has_solution
         assert get_first_solution_time(output_graph) == 3
         assert math.isclose(output_graph.root_node.data["retro_star_value"], 1.6)
-        assert math.isclose(output_graph.root_node.data["reaction_number"], 1.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_reaction_number"], 1.6)
+        assert math.isclose(output_graph.root_node.data["retro_star_min_cost"], 1.6)
         assert_retro_star_values_in_graph(output_graph, [1.6, 2.6, 2.1])
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_breadth_first.py` & `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_breadth_first.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_mcts.py` & `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_mcts.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/algorithms/test_pdvn.py` & `syntheseus-0.4.0/syntheseus/tests/search/algorithms/test_pdvn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import math
 from collections import Counter
 
 import pytest
 
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
+from syntheseus.reaction_prediction.inference.toy_models import ListOfReactionsToyModel
 from syntheseus.search.algorithms.pdvn import PDVN_MCTS, pdvn_extract_training_data
-from syntheseus.search.chem import BackwardReaction, Molecule
 from syntheseus.search.node_evaluation.common import ConstantNodeEvaluator
-from syntheseus.search.reaction_models.toy import ListOfReactionsModel
 from syntheseus.tests.search.algorithms.test_base import BaseAlgorithmTest
 from syntheseus.tests.search.algorithms.test_best_first import (
     DictMolCost,
     DictRxnCost,
     rxn_cost_fn,  # noqa: F401
 )
 from syntheseus.tests.search.conftest import RetrosynthesisTask
@@ -397,20 +399,21 @@
 
     def test_system_with_dead_ends(
         self,
         retrosynthesis_task5: RetrosynthesisTask,
     ) -> None:
         """Test PDVN MCTS on a system with dead end reactions."""
 
-        rxn_model = ListOfReactionsModel(
+        rxn_model = ListOfReactionsToyModel(
             [
-                BackwardReaction(reactants=frozenset({Molecule("C")}), product=Molecule("CC")),
-                BackwardReaction(reactants=frozenset({Molecule("CO")}), product=Molecule("CC")),
-                BackwardReaction(reactants=frozenset({Molecule("O")}), product=Molecule("C")),
-            ]
+                SingleProductReaction(reactants=Bag({Molecule("C")}), product=Molecule("CC")),
+                SingleProductReaction(reactants=Bag({Molecule("CO")}), product=Molecule("CC")),
+                SingleProductReaction(reactants=Bag({Molecule("O")}), product=Molecule("C")),
+            ],
+            use_cache=True,
         )
         retrosynthesis_task = RetrosynthesisTask(
             inventory=retrosynthesis_task5.inventory,
             target_mol=retrosynthesis_task5.target_mol,
             reaction_model=rxn_model,
         )
         output_graph = self.run_alg_for_n_iterations(
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/analysis/conftest.py` & `syntheseus-0.4.0/syntheseus/tests/search/analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/analysis/test_diversity.py` & `syntheseus-0.4.0/syntheseus/tests/search/analysis/test_diversity.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/analysis/test_route_extraction.py` & `syntheseus-0.4.0/syntheseus/tests/search/analysis/test_route_extraction.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/conftest.py` & `syntheseus-0.4.0/syntheseus/tests/search/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,136 +2,121 @@
 from __future__ import annotations
 
 import collections
 from dataclasses import dataclass, field
 
 import pytest
 
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.models import BackwardReactionModel
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
+from syntheseus.reaction_prediction.inference.toy_models import (
+    LinearMoleculesToyModel,
+    ListOfReactionsToyModel,
+)
 from syntheseus.search.algorithms.breadth_first import (
     AndOr_BreadthFirstSearch,
     MolSet_BreadthFirstSearch,
 )
-from syntheseus.search.chem import BackwardReaction, Molecule
 from syntheseus.search.graph.and_or import AndOrGraph
 from syntheseus.search.graph.molset import MolSetGraph
 from syntheseus.search.graph.route import SynthesisGraph
 from syntheseus.search.mol_inventory import BaseMolInventory, SmilesListInventory
-from syntheseus.search.reaction_models import BackwardReactionModel
-from syntheseus.search.reaction_models.toy import LinearMolecules, ListOfReactionsModel
 
 
 @dataclass
 class RetrosynthesisTask:
     """Object to hold all the parts of a retrosynthesis problem. Used for testing."""
 
     target_mol: Molecule
     reaction_model: BackwardReactionModel
     inventory: BaseMolInventory
     known_routes: dict[str, SynthesisGraph] = field(default_factory=dict)
     incorrect_routes: dict[str, SynthesisGraph] = field(default_factory=dict)
 
 
 @pytest.fixture
-def cocs_mol() -> Molecule:
-    """Returns the molecule with smiles 'COCS'"""
-    return Molecule("COCS", make_rdkit_mol=False)
+def rxn_cs_from_co() -> SingleProductReaction:
+    return SingleProductReaction(product=Molecule("CS"), reactants=Bag([Molecule("CO")]))
 
 
 @pytest.fixture
-def rxn_cocs_from_co_cs(cocs_mol: Molecule) -> BackwardReaction:
-    """Returns a reaction with COCS as the product."""
-    return BackwardReaction(product=cocs_mol, reactants=frozenset([Molecule("CO"), Molecule("CS")]))
+def rxn_cocs_from_coco(cocs_mol: Molecule) -> SingleProductReaction:
+    return SingleProductReaction(product=cocs_mol, reactants=Bag([Molecule("COCO")]))
 
 
 @pytest.fixture
-def rxn_cs_from_cc() -> BackwardReaction:
-    return BackwardReaction(product=Molecule("CS"), reactants=frozenset([Molecule("CC")]))
-
-
-@pytest.fixture
-def rxn_cs_from_co() -> BackwardReaction:
-    return BackwardReaction(product=Molecule("CS"), reactants=frozenset([Molecule("CO")]))
-
-
-@pytest.fixture
-def rxn_cocs_from_cocc(cocs_mol: Molecule) -> BackwardReaction:
-    return BackwardReaction(product=cocs_mol, reactants=frozenset([Molecule("COCC")]))
-
-
-@pytest.fixture
-def rxn_cocs_from_coco(cocs_mol: Molecule) -> BackwardReaction:
-    return BackwardReaction(product=cocs_mol, reactants=frozenset([Molecule("COCO")]))
-
-
-@pytest.fixture
-def rxn_cocc_from_co_cc() -> BackwardReaction:
-    return BackwardReaction(
-        product=Molecule("COCC"), reactants=frozenset([Molecule("CO"), Molecule("CC")])
+def rxn_cocc_from_co_cc() -> SingleProductReaction:
+    return SingleProductReaction(
+        product=Molecule("COCC"), reactants=Bag([Molecule("CO"), Molecule("CC")])
     )
 
 
 @pytest.fixture
-def rxn_co_from_cc() -> BackwardReaction:
-    return BackwardReaction(product=Molecule("CO"), reactants=frozenset([Molecule("CC")]))
+def rxn_co_from_cc() -> SingleProductReaction:
+    return SingleProductReaction(product=Molecule("CO"), reactants=Bag([Molecule("CC")]))
 
 
 @pytest.fixture
-def rxn_cocc_from_coco() -> BackwardReaction:
-    return BackwardReaction(product=Molecule("COCC"), reactants=frozenset([Molecule("COCO")]))
+def rxn_cocc_from_coco() -> SingleProductReaction:
+    return SingleProductReaction(product=Molecule("COCC"), reactants=Bag([Molecule("COCO")]))
 
 
 @pytest.fixture
-def rxn_coco_from_co() -> BackwardReaction:
-    return BackwardReaction(product=Molecule("COCO"), reactants=frozenset([Molecule("CO")]))
+def rxn_coco_from_co() -> SingleProductReaction:
+    return SingleProductReaction(product=Molecule("COCO"), reactants=Bag([Molecule("CO")]))
 
 
 @pytest.fixture
-def bad_rxn_cc_from_cocs() -> BackwardReaction:
+def bad_rxn_cc_from_cocs() -> SingleProductReaction:
     """
     A reaction which is not possible with the LinearMolecules model,
     and has the root node of most tests as a reactant.
     Used to test illegal expansions.
     """
-    return BackwardReaction(product=Molecule("CC"), reactants=frozenset([Molecule("COCS")]))
+    return SingleProductReaction(product=Molecule("CC"), reactants=Bag([Molecule("COCS")]))
 
 
 @pytest.fixture
 def retrosynthesis_task1(
-    cocs_mol: Molecule, rxn_cocs_from_coco: BackwardReaction, rxn_coco_from_co: BackwardReaction
+    cocs_mol: Molecule,
+    rxn_cocs_from_coco: SingleProductReaction,
+    rxn_coco_from_co: SingleProductReaction,
 ) -> RetrosynthesisTask:
     """Returns a retrosynthesis task which can be solved in a single step."""
 
     # Object for best route
     best_route = SynthesisGraph(
-        BackwardReaction(product=cocs_mol, reactants=frozenset([Molecule("CO"), Molecule("CS")]))
+        SingleProductReaction(product=cocs_mol, reactants=Bag([Molecule("CO"), Molecule("CS")]))
     )
 
     # Object for route COCS -> COCO ; COCO -> CO
     other_route = SynthesisGraph(rxn_cocs_from_coco)
     other_route._graph.add_edge(other_route.root_node, rxn_coco_from_co)
     other_route.assert_validity()
 
     return RetrosynthesisTask(
         target_mol=cocs_mol,
-        reaction_model=LinearMolecules(),
+        reaction_model=LinearMoleculesToyModel(use_cache=True),
         inventory=SmilesListInventory(["CO", "CS"]),
         known_routes={"min-cost": best_route, "other": other_route},
     )
 
 
 @pytest.fixture
 def retrosynthesis_task2(
     cocs_mol: Molecule,
-    rxn_cocs_from_co_cs: BackwardReaction,
-    rxn_cs_from_cc: BackwardReaction,
-    rxn_cs_from_co: BackwardReaction,
-    rxn_cocs_from_cocc: BackwardReaction,
-    rxn_cocc_from_co_cc: BackwardReaction,
-    rxn_cocc_from_coco: BackwardReaction,
-    rxn_coco_from_co: BackwardReaction,
+    rxn_cocs_from_co_cs: SingleProductReaction,
+    rxn_cs_from_cc: SingleProductReaction,
+    rxn_cs_from_co: SingleProductReaction,
+    rxn_cocs_from_cocc: SingleProductReaction,
+    rxn_cocc_from_co_cc: SingleProductReaction,
+    rxn_cocc_from_coco: SingleProductReaction,
+    rxn_coco_from_co: SingleProductReaction,
 ) -> RetrosynthesisTask:
     """
     Returns a retrosynthesis task which requires 2 steps to solve.
 
     A 2 step solution is:
     COCS -> CO + CS
     CS -> CC
@@ -169,27 +154,27 @@
     del other_route1
 
     # Create some known incorrect routes
     incorrect_routes["1"] = SynthesisGraph(
         rxn_cocs_from_co_cs
     )  # incorrect because doesn't end in purchasable molecules
     incorrect_routes["2"] = SynthesisGraph(
-        BackwardReaction(product=cocs_mol, reactants=frozenset([Molecule("COCSCOCS")]))
+        SingleProductReaction(product=cocs_mol, reactants=Bag([Molecule("COCSCOCS")]))
     )  # incorrect because this reaction cannot be output by this reaction model
 
     # Check that all routes are valid
     for r in known_routes.values():
         r.assert_validity()
 
     for r in incorrect_routes.values():
         r.assert_validity()
 
     return RetrosynthesisTask(
         target_mol=cocs_mol,
-        reaction_model=LinearMolecules(),
+        reaction_model=LinearMoleculesToyModel(use_cache=True),
         inventory=SmilesListInventory(["CO", "CC"]),
         known_routes=known_routes,
         incorrect_routes=incorrect_routes,
     )
 
 
 @pytest.fixture
@@ -199,15 +184,17 @@
 
     The 3 step solution is:
     COCS -> CO + CS
     CS -> CC
     CO -> CC
     """
     return RetrosynthesisTask(
-        target_mol=cocs_mol, reaction_model=LinearMolecules(), inventory=SmilesListInventory(["CC"])
+        target_mol=cocs_mol,
+        reaction_model=LinearMoleculesToyModel(use_cache=True),
+        inventory=SmilesListInventory(["CC"]),
     )
 
 
 @pytest.fixture
 def retrosynthesis_task4(cocs_mol: Molecule) -> RetrosynthesisTask:
     """
     A small, *finite* retrosynthesis task which can be solved in 3 steps.
@@ -216,28 +203,29 @@
     The 3 step solution is:
     COCS -> CO + CS
     C -> C + S
     CO -> C + O
     """
     return RetrosynthesisTask(
         target_mol=cocs_mol,
-        reaction_model=LinearMolecules(allow_substitution=False),
+        reaction_model=LinearMoleculesToyModel(allow_substitution=False, use_cache=True),
         inventory=SmilesListInventory(["C", "O", "S"]),
     )
 
 
 @pytest.fixture
 def retrosynthesis_task5() -> RetrosynthesisTask:
     """
     A very small, *infinite* retrosynthesis task which cannot be solved in 1 step.
     Good for testing full expansion of trees.
     """
+
     return RetrosynthesisTask(
         target_mol=Molecule("CC", make_rdkit_mol=False),
-        reaction_model=LinearMolecules(allow_substitution=True),
+        reaction_model=LinearMoleculesToyModel(allow_substitution=True, use_cache=True),
         inventory=SmilesListInventory(["O"]),
     )
 
 
 @pytest.fixture
 def retrosynthesis_task6() -> RetrosynthesisTask:
     """
@@ -254,41 +242,44 @@
     CCCOC -> CCCOO
     CCCOO -> CCCO + O
 
     From route extraction, there appear to be 8 routes of length 3.
     """
     return RetrosynthesisTask(
         target_mol=Molecule("CCCOC", make_rdkit_mol=False),
-        reaction_model=LinearMolecules(allow_substitution=True),
+        reaction_model=LinearMoleculesToyModel(allow_substitution=True, use_cache=True),
         inventory=SmilesListInventory(["CCCO", "CC", "COC", "O"]),
     )
 
 
 @pytest.fixture
 def rxn_model_for_minimal_graphs(
-    rxn_cocs_from_co_cs: BackwardReaction,
-    rxn_co_from_cc: BackwardReaction,
-    rxn_cs_from_co: BackwardReaction,
-) -> ListOfReactionsModel:
+    rxn_cocs_from_co_cs: SingleProductReaction,
+    rxn_co_from_cc: SingleProductReaction,
+    rxn_cs_from_co: SingleProductReaction,
+) -> ListOfReactionsToyModel:
     """
     Return a reaction model to help build the minimal graphs.
     Contains the following reactions:
 
     COCS -> CO + CS
     CO -> CC
     CS -> CO
     """
-    return ListOfReactionsModel(reaction_list=[rxn_cocs_from_co_cs, rxn_co_from_cc, rxn_cs_from_co])
+    return ListOfReactionsToyModel(
+        reaction_list=[rxn_cocs_from_co_cs, rxn_co_from_cc, rxn_cs_from_co],
+        use_cache=True,
+    )
 
 
 @pytest.fixture
 def rxn_model_for_non_minimal_graphs(
-    rxn_model_for_minimal_graphs: ListOfReactionsModel,
-    rxn_cocs_from_cocc: BackwardReaction,
-    rxn_cocc_from_co_cc: BackwardReaction,
+    rxn_model_for_minimal_graphs: ListOfReactionsToyModel,
+    rxn_cocs_from_cocc: SingleProductReaction,
+    rxn_cocc_from_co_cc: SingleProductReaction,
 ) -> BackwardReactionModel:
     """Add reactions COCS -> COCC ; COCC -> CO + CC to the reaction model above."""
     rxn_model_for_minimal_graphs.reaction_list.extend([rxn_cocs_from_cocc, rxn_cocc_from_co_cc])
     return rxn_model_for_minimal_graphs
 
 
 @pytest.fixture
@@ -320,17 +311,17 @@
     output_graph, _ = bfs.run_from_mol(mol)
     output_graph.assert_validity()
     return output_graph
 
 
 @pytest.fixture
 def minimal_synthesis_graph(
-    rxn_cocs_from_co_cs: BackwardReaction,
-    rxn_co_from_cc: BackwardReaction,
-    rxn_cs_from_co: BackwardReaction,
+    rxn_cocs_from_co_cs: SingleProductReaction,
+    rxn_co_from_cc: SingleProductReaction,
+    rxn_cs_from_co: SingleProductReaction,
 ) -> SynthesisGraph:
     """
     Returns the synthesis graph for the minimal routes below.
     """
     g = SynthesisGraph(rxn_cocs_from_co_cs)
     g._graph.add_edge(rxn_cocs_from_co_cs, rxn_co_from_cc)
     g._graph.add_edge(rxn_cocs_from_co_cs, rxn_cs_from_co)
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/graph/test_andor.py` & `syntheseus-0.4.0/syntheseus/tests/search/graph/test_andor.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 Tests for AND/OR graph/nodes.
 
 Because a lot of the behaviour is implicitly tested when the algorithms are tested,
 the tests here are sparse and mainly check edge cases which won't come up in algorithms.
 """
 import pytest
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.and_or import AndNode, AndOrGraph, OrNode
 from syntheseus.search.graph.route import SynthesisGraph
 from syntheseus.tests.search.graph.test_base import BaseNodeTest
 
 
 class TestAndNode(BaseNodeTest):
     def get_node(self):
         return AndNode(
-            reaction=BackwardReaction(product=Molecule("CC"), reactants=frozenset([Molecule("C")]))
+            reaction=SingleProductReaction(product=Molecule("CC"), reactants=Bag([Molecule("C")]))
         )
 
     def test_nodes_not_frozen(self):
         node = self.get_node()
         node.reaction = None
 
 
@@ -106,15 +108,15 @@
             andor_graph_non_minimal.root_node.is_expanded = False
         elif reason == "reactions_dont_match":
             first_and_node: AndNode = list(  # type: ignore # doesn't understand OrNode children are always AndNode
                 andor_graph_non_minimal.successors(andor_graph_non_minimal.root_node)
             )[
                 0
             ]
-            first_and_node.reaction = BackwardReaction(
+            first_and_node.reaction = SingleProductReaction(
                 product=Molecule("CCC"), reactants=first_and_node.reaction.reactants
             )
 
             # Not only should the graph not be valid below,
             # but specifically the reaction should also be invalid
             with pytest.raises(AssertionError):
                 andor_graph_non_minimal._assert_valid_reactions()
@@ -127,16 +129,16 @@
 
     @pytest.mark.parametrize(
         "reason", ["root_as_reactant", "ensure_tree", "already_expanded", "wrong_product"]
     )
     def test_invalid_expansions(
         self,
         andor_graph_non_minimal: AndOrGraph,
-        bad_rxn_cc_from_cocs: BackwardReaction,
-        rxn_cs_from_cc: BackwardReaction,
+        bad_rxn_cc_from_cocs: SingleProductReaction,
+        rxn_cs_from_cc: SingleProductReaction,
         reason: str,
     ) -> None:
         """
         Test that invalid expansions raise an error.
         Note that valid expansions are tested implicitly elsewhere.
         """
         cc_nodes = [
@@ -150,16 +152,16 @@
                 andor_graph_non_minimal.expand_with_reactions(
                     reactions=[bad_rxn_cc_from_cocs], node=cc_nodes[0], ensure_tree=False
                 )
         elif reason == "ensure_tree":
             with pytest.raises(AssertionError):
                 andor_graph_non_minimal.expand_with_reactions(
                     reactions=[
-                        BackwardReaction(
-                            product=Molecule("CC"), reactants=frozenset([Molecule("CO")])
+                        SingleProductReaction(
+                            product=Molecule("CC"), reactants=Bag([Molecule("CO")])
                         )
                     ],
                     node=cc_nodes[0],
                     ensure_tree=True,
                 )
         elif reason == "already_expanded":
             with pytest.raises(AssertionError):
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/graph/test_base.py` & `syntheseus-0.4.0/syntheseus/tests/search/graph/test_base.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/graph/test_message_passing.py` & `syntheseus-0.4.0/syntheseus/tests/search/graph/test_message_passing.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/graph/test_molset.py` & `syntheseus-0.4.0/syntheseus/tests/search/graph/test_molset.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 Tests for MolSet graph/nodes.
 
 Because a lot of the behaviour is implicitly tested when the algorithms are tested,
 the tests here are sparse and mainly check edge cases which won't come up in algorithms.
 """
 import pytest
 
-from syntheseus.search.chem import BackwardReaction, Molecule
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
 from syntheseus.search.graph.molset import MolSetGraph, MolSetNode
 from syntheseus.search.graph.route import SynthesisGraph
 from syntheseus.tests.search.graph.test_base import BaseNodeTest
 
 
 class TestMolSetNode(BaseNodeTest):
     def get_node(self):
-        return MolSetNode(mols=frozenset([Molecule("CC")]))
+        return MolSetNode(mols=Bag([Molecule("CC")]))
 
     def test_nodes_not_frozen(self):
         node = self.get_node()
         node.mols = None
 
 
 class TestMolSetGraph:
@@ -75,31 +77,34 @@
             graph._graph.add_edge(random_node, graph.root_node)
         elif reason == "unexpanded_expanded":
             graph.root_node.is_expanded = False
         elif reason == "reactions_dont_match":
             child = list(graph.successors(graph.root_node))[0]
 
             # Set the reaction to a random incorrect reaction
-            graph._graph.edges[graph.root_node, child]["reaction"] = BackwardReaction(
-                reactants=frozenset([Molecule("OO")]), product=Molecule("CC")
+            graph._graph.edges[graph.root_node, child]["reaction"] = SingleProductReaction(
+                reactants=Bag([Molecule("OO")]), product=Molecule("CC")
             )
 
             # Not only should the graph not be valid below,
             # but specifically the reaction should also be invalid
             with pytest.raises(AssertionError):
                 graph._assert_valid_reactions()
         else:
             raise ValueError(f"Unsupported reason: {reason}")
 
         with pytest.raises(AssertionError):
             graph.assert_validity()
 
     @pytest.mark.parametrize("reason", ["already_expanded", "wrong_product"])
     def test_invalid_expansions(
-        self, molset_tree_non_minimal: MolSetGraph, rxn_cs_from_cc: BackwardReaction, reason: str
+        self,
+        molset_tree_non_minimal: MolSetGraph,
+        rxn_cs_from_cc: SingleProductReaction,
+        reason: str,
     ) -> None:
         """
         Test that invalid expansions raise an error.
         Note that valid expansions are tested implicitly elsewhere.
 
         NOTE: because graphs with 1 node per molset are not properly supported now,
         we don't test the case where the product of a reaction is the root mol.
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/graph/test_standardization.py` & `syntheseus-0.4.0/syntheseus/tests/search/graph/test_standardization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/node_evaluation/test_common.py` & `syntheseus-0.4.0/syntheseus/tests/search/node_evaluation/test_common.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/test_mol_inventory.py` & `syntheseus-0.4.0/syntheseus/tests/search/test_mol_inventory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for MolInventory objects, focusing on the provided SmilesListInventory."""
 
 import pytest
 
-from syntheseus.search.chem import Molecule
+from syntheseus.interface.molecule import Molecule
 from syntheseus.search.mol_inventory import SmilesListInventory
 
 PURCHASABLE_SMILES = ["CC", "c1ccccc1", "CCO"]
 NON_PURCHASABLE_SMILES = ["C", "C1CCCCC1", "OCCO"]
 
 
 @pytest.fixture
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/test_reaction_models.py` & `syntheseus-0.4.0/syntheseus/tests/interface/test_models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
+"""Tests of models. Note that models are tested implicitly in a lot of other places,
+so tests are somewhat minimal here.
 """
-Test reaction models.
-
-Note that some testing is done implicitly in the algorithm tests
-(i.e. those tests will only pass if the reaction models are working properly).
-Therefore the tests here are not super exhaustive: instead they try to explicitly
-look for some behaviours which might be overlooked by the algorithm tests.
-"""
+from __future__ import annotations
 
 import pytest
 
-from syntheseus.search.chem import BackwardReaction, Molecule
-from syntheseus.search.reaction_models.toy import LinearMolecules, ListOfReactionsModel
+from syntheseus.interface.bag import Bag
+from syntheseus.interface.models import DEFAULT_NUM_RESULTS
+from syntheseus.interface.molecule import Molecule
+from syntheseus.interface.reaction import SingleProductReaction
+from syntheseus.reaction_prediction.inference.toy_models import LinearMoleculesToyModel
 
 
 @pytest.mark.parametrize("remove", [True, False])
 def test_remove_duplicates(remove: bool) -> None:
     """
     Test the 'remove_duplicates' kwarg by calling the LinearMolecules model on "CC".
 
@@ -22,20 +21,20 @@
 
     With remove_duplicates=False there should be some duplicates:
     for example, CC -> CO and CC -> OC are the same reaction written 2 ways.
     """
 
     # Define mols and reactions
     CC = Molecule("CC")
-    rxn_C_C = BackwardReaction(product=CC, reactants=frozenset({Molecule("C")}))
-    rxn_CO = BackwardReaction(product=CC, reactants=frozenset({Molecule("CO")}))
-    rxn_CS = BackwardReaction(product=CC, reactants=frozenset({Molecule("CS")}))
+    rxn_C_C = SingleProductReaction(product=CC, reactants=Bag({Molecule("C")}))
+    rxn_CO = SingleProductReaction(product=CC, reactants=Bag({Molecule("CO")}))
+    rxn_CS = SingleProductReaction(product=CC, reactants=Bag({Molecule("CS")}))
 
     # Call reaction model
-    rxn_model = LinearMolecules(remove_duplicates=remove)
+    rxn_model = LinearMoleculesToyModel(remove_duplicates=remove)
     output = rxn_model([CC])
 
     # Check that outputs are what is expected.
     # NOTE: this test depends on the order of the outputs being consistent,
     # which is the case for this toy model but may not be true in general
     if remove:
         assert output == [[rxn_C_C, rxn_CO, rxn_CS]]
@@ -44,15 +43,15 @@
 
 
 @pytest.mark.parametrize("use_cache", [True, False])
 def test_caching(cocs_mol: Molecule, use_cache: bool) -> None:
     """Test all aspects of caching for reaction models."""
 
     # Call model twice on same molecule
-    rxn_model = LinearMolecules(use_cache=use_cache)
+    rxn_model = LinearMoleculesToyModel(use_cache=use_cache)
     output1 = rxn_model([cocs_mol])
     output2 = rxn_model([cocs_mol])
 
     # Test 1: regardless of caching, outputs should not change
     assert output1 == output2
 
     # Test 2: is number of calls correct?
@@ -99,69 +98,47 @@
     output7 = rxn_model([cocs_mol])
     assert output7 == output1
     assert rxn_model.num_calls() == 1
 
 
 @pytest.mark.parametrize("use_cache", [True, False])
 def test_initial_cache(
-    cocs_mol: Molecule, rxn_cocs_from_co_cs: BackwardReaction, use_cache: bool
+    cocs_mol: Molecule, rxn_cocs_from_co_cs: SingleProductReaction, use_cache: bool
 ) -> None:
     """Test that seeding the reaction model with an initial cache works as expected."""
 
     # Create initial cache.
     # NOTE: this is *not* what the reaction model would actually output if called.
     # If the cache works correctly then it will output this reaction instead of calling the model.
     CC = Molecule("CC")
-    initial_cache = {cocs_mol: [rxn_cocs_from_co_cs], CC: []}
+    initial_cache = {
+        (cocs_mol, DEFAULT_NUM_RESULTS): [rxn_cocs_from_co_cs],
+        (CC, DEFAULT_NUM_RESULTS): [],
+    }
 
     # Create reaction model, potentially checking for warning
     if use_cache:
-        rxn_model = LinearMolecules(use_cache=use_cache, initial_cache=initial_cache)
+        rxn_model = LinearMoleculesToyModel(use_cache=use_cache, initial_cache=initial_cache)
     else:
         # If caching is off then providing an initial cache should raise a warning
         with pytest.warns(UserWarning):
-            rxn_model = LinearMolecules(use_cache=use_cache, initial_cache=initial_cache)
+            rxn_model = LinearMoleculesToyModel(use_cache=use_cache, initial_cache=initial_cache)
 
     # Call reaction model
     outputs = rxn_model([cocs_mol, CC, Molecule("CCC")])
     if use_cache:
         # outputs should reflect initial cache
-        assert outputs[0] == initial_cache[cocs_mol]
-        assert outputs[1] == initial_cache[CC]
+        assert outputs[0] == initial_cache[(cocs_mol, DEFAULT_NUM_RESULTS)]
+        assert outputs[1] == initial_cache[(CC, DEFAULT_NUM_RESULTS)]
         assert rxn_model.num_calls() == 1
     else:
         # outputs should ignore initial cache
         assert len(outputs[0]) == 7
         assert len(outputs[1]) == 3
         assert rxn_model.num_calls() == 3
     assert (
         len(outputs[2]) == 3
     )  # not in initial cache, so in both cases model should actually be called
 
     # In all cases, resetting should clear the cache
     rxn_model.reset()
     assert len(rxn_model._cache) == 0
-
-
-def test_linear_molecules_invalid_molecule() -> None:
-    """
-    The LinearMolecules model is only defined on the space of linear molecules.
-    If called on a non-linear molecule (e.g. with branching) it is currently set up to throw an error.
-    This test ensures that this happens.
-
-    NOTE: in the future the behaviour could be changed to just return an empty list,
-    but for a toy example I thought it would be best to alert the user with a warning.
-    """
-    rxn_model = LinearMolecules()
-    with pytest.raises(AssertionError):
-        rxn_model([Molecule("CC(C)C")])
-
-
-def test_list_of_reactions_model(
-    rxn_cocs_from_co_cs: BackwardReaction,
-    rxn_cocs_from_cocc: BackwardReaction,
-    rxn_cs_from_cc: BackwardReaction,
-) -> None:
-    """Simple test of the ListOfReactionsModel class."""
-    model = ListOfReactionsModel([rxn_cocs_from_co_cs, rxn_cocs_from_cocc, rxn_cs_from_cc])
-    output = model([Molecule("COCS"), Molecule("CS"), Molecule("CO")])
-    assert output == [[rxn_cocs_from_co_cs, rxn_cocs_from_cocc], [rxn_cs_from_cc], []]
```

### Comparing `syntheseus-0.3.0/syntheseus/tests/search/test_visualization.py` & `syntheseus-0.4.0/syntheseus/tests/search/test_visualization.py`

 * *Files identical despite different names*

### Comparing `syntheseus-0.3.0/syntheseus.egg-info/PKG-INFO` & `syntheseus-0.4.0/syntheseus.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7379 6e74  : 2.1.Name: synt
 00000020: 6865 7365 7573 0a56 6572 7369 6f6e 3a20  heseus.Version: 
-00000030: 302e 332e 300a 5375 6d6d 6172 793a 2041  0.3.0.Summary: A
+00000030: 302e 342e 300a 5375 6d6d 6172 793a 2041  0.4.0.Summary: A
 00000040: 2070 6163 6b61 6765 2066 6f72 2072 6574   package for ret
 00000050: 726f 7379 6e74 6865 7469 6320 706c 616e  rosynthetic plan
 00000060: 6e69 6e67 2e0a 4175 7468 6f72 3a20 4175  ning..Author: Au
 00000070: 7374 696e 2054 7269 7070 2c20 4b72 7a79  stin Tripp, Krzy
 00000080: 737a 746f 6620 4d61 7a69 6172 7a2c 2047  sztof Maziarz, G
 00000090: 756f 7169 6e67 204c 6975 2c20 4d65 6761  uoqing Liu, Mega
 000000a0: 6e20 5374 616e 6c65 792c 204d 6172 7769  n Stanley, Marwi
@@ -129,268 +129,297 @@
 00000800: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
 00000810: 6972 6573 2d44 6973 743a 2070 7265 2d63  ires-Dist: pre-c
 00000820: 6f6d 6d69 743b 2065 7874 7261 203d 3d20  ommit; extra == 
 00000830: 2264 6576 220a 5072 6f76 6964 6573 2d45  "dev".Provides-E
 00000840: 7874 7261 3a20 6368 656d 666f 726d 6572  xtra: chemformer
 00000850: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
 00000860: 7379 6e74 6865 7365 7573 2d63 6865 6d66  syntheseus-chemf
-00000870: 6f72 6d65 723b 2065 7874 7261 203d 3d20  ormer; extra == 
-00000880: 2263 6865 6d66 6f72 6d65 7222 0a50 726f  "chemformer".Pro
-00000890: 7669 6465 732d 4578 7472 613a 206c 6f63  vides-Extra: loc
-000008a0: 616c 2d72 6574 726f 0a52 6571 7569 7265  al-retro.Require
-000008b0: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
-000008c0: 7573 2d6c 6f63 616c 2d72 6574 726f 3b20  us-local-retro; 
-000008d0: 6578 7472 6120 3d3d 2022 6c6f 6361 6c2d  extra == "local-
-000008e0: 7265 7472 6f22 0a50 726f 7669 6465 732d  retro".Provides-
-000008f0: 4578 7472 613a 206d 6567 616e 0a52 6571  Extra: megan.Req
-00000900: 7569 7265 732d 4469 7374 3a20 7379 6e74  uires-Dist: synt
-00000910: 6865 7365 7573 2d6d 6567 616e 3b20 6578  heseus-megan; ex
-00000920: 7472 6120 3d3d 2022 6d65 6761 6e22 0a50  tra == "megan".P
-00000930: 726f 7669 6465 732d 4578 7472 613a 206d  rovides-Extra: m
-00000940: 686e 2d72 6561 6374 0a52 6571 7569 7265  hn-react.Require
-00000950: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
-00000960: 7573 2d6d 686e 7265 6163 743b 2065 7874  us-mhnreact; ext
-00000970: 7261 203d 3d20 226d 686e 2d72 6561 6374  ra == "mhn-react
-00000980: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
-00000990: 3a20 7265 7472 6f2d 6b6e 6e0a 5265 7175  : retro-knn.Requ
-000009a0: 6972 6573 2d44 6973 743a 2073 796e 7468  ires-Dist: synth
-000009b0: 6573 6575 732d 6c6f 6361 6c2d 7265 7472  eseus-local-retr
-000009c0: 6f3b 2065 7874 7261 203d 3d20 2272 6574  o; extra == "ret
-000009d0: 726f 2d6b 6e6e 220a 5265 7175 6972 6573  ro-knn".Requires
-000009e0: 2d44 6973 743a 2074 6f72 6368 2d73 6361  -Dist: torch-sca
-000009f0: 7474 6572 3b20 6578 7472 6120 3d3d 2022  tter; extra == "
-00000a00: 7265 7472 6f2d 6b6e 6e22 0a50 726f 7669  retro-knn".Provi
-00000a10: 6465 732d 4578 7472 613a 2072 6f6f 742d  des-Extra: root-
-00000a20: 616c 6967 6e65 640a 5265 7175 6972 6573  aligned.Requires
-00000a30: 2d44 6973 743a 2073 796e 7468 6573 6575  -Dist: syntheseu
-00000a40: 732d 726f 6f74 2d61 6c69 676e 6564 3b20  s-root-aligned; 
-00000a50: 6578 7472 6120 3d3d 2022 726f 6f74 2d61  extra == "root-a
-00000a60: 6c69 676e 6564 220a 5072 6f76 6964 6573  ligned".Provides
-00000a70: 2d45 7874 7261 3a20 616c 6c2d 7369 6e67  -Extra: all-sing
-00000a80: 6c65 2d73 7465 700a 5265 7175 6972 6573  le-step.Requires
-00000a90: 2d44 6973 743a 2073 796e 7468 6573 6575  -Dist: syntheseu
-00000aa0: 735b 6368 656d 666f 726d 6572 2c6c 6f63  s[chemformer,loc
-00000ab0: 616c 2d72 6574 726f 2c6d 6567 616e 2c6d  al-retro,megan,m
-00000ac0: 686e 2d72 6561 6374 2c72 6574 726f 2d6b  hn-react,retro-k
-00000ad0: 6e6e 2c72 6f6f 742d 616c 6967 6e65 645d  nn,root-aligned]
-00000ae0: 3b20 6578 7472 6120 3d3d 2022 616c 6c2d  ; extra == "all-
-00000af0: 7369 6e67 6c65 2d73 7465 7022 0a50 726f  single-step".Pro
-00000b00: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
-00000b10: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b20: 7379 6e74 6865 7365 7573 5b61 6c6c 2d73  syntheseus[all-s
-00000b30: 696e 676c 652d 7374 6570 2c64 6576 2c76  ingle-step,dev,v
-00000b40: 697a 5d3b 2065 7874 7261 203d 3d20 2261  iz]; extra == "a
-00000b50: 6c6c 220a 0a3c 6469 7620 616c 6967 6e3d  ll"..<div align=
-00000b60: 2263 656e 7465 7222 3e0a 2020 2020 3c69  "center">.    <i
-00000b70: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000b80: 6769 7468 7562 2e63 6f6d 2f6d 6963 726f  github.com/micro
-00000b90: 736f 6674 2f73 796e 7468 6573 6575 732f  soft/syntheseus/
-00000ba0: 6173 7365 7473 2f36 3134 3730 3932 332f  assets/61470923/
-00000bb0: 6630 3161 3939 3339 2d36 3166 612d 3434  f01a9939-61fa-44
-00000bc0: 3631 2d61 3132 342d 6331 3365 6464 6364  61-a124-c13eddcd
-00000bd0: 6437 3561 2220 6865 6967 6874 3d22 3530  d75a" height="50
-00000be0: 7078 223e 0a20 2020 203c 6833 3e3c 693e  px">.    <h3><i>
-00000bf0: 4e61 7669 6761 7469 6e67 2074 6865 206c  Navigating the l
-00000c00: 6162 7972 696e 7468 206f 6620 7379 6e74  abyrinth of synt
-00000c10: 6865 7369 7320 706c 616e 6e69 6e67 3c2f  hesis planning</
-00000c20: 693e 3c2f 6833 3e0a 3c2f 6469 763e 0a0a  i></h3>.</div>..
-00000c30: 2d2d 2d0a 0a5b 215b 4349 5d28 6874 7470  ---..[![CI](http
-00000c40: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00000c50: 6963 726f 736f 6674 2f73 796e 7468 6573  icrosoft/synthes
-00000c60: 6575 732f 6163 7469 6f6e 732f 776f 726b  eus/actions/work
-00000c70: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
-00000c80: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
-00000c90: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
-00000ca0: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
-00000cb0: 742f 7379 6e74 6865 7365 7573 2f61 6374  t/syntheseus/act
-00000cc0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
-00000cd0: 692e 796d 6c29 0a5b 215b 5079 7468 6f6e  i.yml).[![Python
-00000ce0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
-00000cf0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000d00: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
-00000d10: 372b 2d62 6c75 652e 7376 6729 5d28 6874  7+-blue.svg)](ht
-00000d20: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000d30: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000d40: 0a5b 215b 636f 6465 2073 7479 6c65 5d28  .[![code style](
-00000d50: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000d60: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
-00000d70: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
-00000d80: 3230 3230 3230 2e73 7667 295d 2868 7474  202020.svg)](htt
-00000d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000da0: 616d 6276 2f62 6c61 636b 290a 5b21 5b4c  ambv/black).[![L
-00000db0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
-00000dc0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00000dd0: 6164 6765 2f6c 6963 656e 7365 2d4d 4954  adge/license-MIT
-00000de0: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
-00000df0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e00: 6d69 6372 6f73 6f66 742f 7379 6e74 6865  microsoft/synthe
-00000e10: 7365 7573 2f62 6c6f 622f 6d61 696e 2f4c  seus/blob/main/L
-00000e20: 4943 454e 5345 290a 0a53 796e 7468 6573  ICENSE)..Synthes
-00000e30: 6575 7320 6973 2061 2070 6163 6b61 6765  eus is a package
-00000e40: 2066 6f72 2065 6e64 2d74 6f2d 656e 6420   for end-to-end 
-00000e50: 7265 7472 6f73 796e 7468 6574 6963 2070  retrosynthetic p
-00000e60: 6c61 6e6e 696e 672e 0a2d 20e2 9a92 efb8  lanning..- .....
-00000e70: 8f20 436f 6d62 696e 6573 2073 6561 7263  . Combines searc
-00000e80: 6820 616c 676f 7269 7468 6d73 2061 6e64  h algorithms and
-00000e90: 2072 6561 6374 696f 6e20 6d6f 6465 6c73   reaction models
-00000ea0: 2069 6e20 6120 7374 616e 6461 7264 697a   in a standardiz
-00000eb0: 6564 2077 6179 0a2d 20f0 9fa7 ad20 496e  ed way.- .... In
-00000ec0: 636c 7564 6573 2069 6d70 6c65 6d65 6e74  cludes implement
-00000ed0: 6174 696f 6e73 206f 6620 636f 6d6d 6f6e  ations of common
-00000ee0: 2073 6561 7263 6820 616c 676f 7269 7468   search algorith
-00000ef0: 6d73 0a2d 20f0 9fa7 aa20 496e 636c 7564  ms.- .... Includ
-00000f00: 6573 2077 7261 7070 6572 7320 666f 7220  es wrappers for 
-00000f10: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
-00000f20: 2072 6561 6374 696f 6e20 6d6f 6465 6c73   reaction models
-00000f30: 0a2d 20e2 9a99 efb8 8f20 4578 706f 7365  .- ...... Expose
-00000f40: 7320 6120 7369 6d70 6c65 2041 5049 2074  s a simple API t
-00000f50: 6f20 706c 7567 2069 6e20 6375 7374 6f6d  o plug in custom
-00000f60: 206d 6f64 656c 7320 616e 6420 616c 676f   models and algo
-00000f70: 7269 7468 6d73 0a2d 20f0 9f93 8820 4361  rithms.- .... Ca
-00000f80: 6e20 6265 2075 7365 6420 746f 2062 656e  n be used to ben
-00000f90: 6368 6d61 726b 2063 6f6d 706f 6e65 6e74  chmark component
-00000fa0: 7320 6f66 2061 2072 6574 726f 7379 6e74  s of a retrosynt
-00000fb0: 6865 7369 7320 7069 7065 6c69 6e65 0a0a  hesis pipeline..
-00000fc0: 546f 206c 6561 726e 2061 626f 7574 2060  To learn about `
-00000fd0: 7379 6e74 6865 7365 7573 6027 7320 6665  syntheseus`'s fe
-00000fe0: 6174 7572 6573 2061 6e64 2041 5049 2076  atures and API v
-00000ff0: 6973 6974 205b 6d69 6372 6f73 6f66 742e  isit [microsoft.
-00001000: 6769 7468 7562 2e69 6f2f 7379 6e74 6865  github.io/synthe
-00001010: 7365 7573 5d28 6874 7470 733a 2f2f 6d69  seus](https://mi
-00001020: 6372 6f73 6f66 742e 6769 7468 7562 2e69  crosoft.github.i
-00001030: 6f2f 7379 6e74 6865 7365 7573 292e 0a0a  o/syntheseus)...
-00001040: 2323 2051 7569 636b 2053 7461 7274 0a0a  ## Quick Start..
-00001050: 546f 2069 6e73 7461 6c6c 2060 7379 6e74  To install `synt
-00001060: 6865 7365 7573 6020 7769 7468 2061 6c6c  heseus` with all
-00001070: 2074 6865 2065 7874 7261 732c 2072 756e   the extras, run
-00001080: 0a0a 6060 6062 6173 680a 636f 6e64 6120  ..```bash.conda 
-00001090: 656e 7620 6372 6561 7465 202d 6620 656e  env create -f en
-000010a0: 7669 726f 6e6d 656e 745f 6675 6c6c 2e79  vironment_full.y
-000010b0: 6d6c 0a63 6f6e 6461 2061 6374 6976 6174  ml.conda activat
-000010c0: 6520 7379 6e74 6865 7365 7573 2d66 756c  e syntheseus-ful
-000010d0: 6c0a 0a70 6970 2069 6e73 7461 6c6c 202d  l..pip install -
-000010e0: 6520 222e 5b61 6c6c 5d22 0a60 6060 0a0a  e ".[all]".```..
-000010f0: 5365 6520 5b64 6f63 756d 656e 7461 7469  See [documentati
-00001100: 6f6e 5d28 6874 7470 733a 2f2f 6d69 6372  on](https://micr
-00001110: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
-00001120: 7379 6e74 6865 7365 7573 2f69 6e73 7461  syntheseus/insta
-00001130: 6c6c 6174 696f 6e29 2069 6620 796f 7520  llation) if you 
-00001140: 7072 6566 6572 2061 206d 6f72 6520 6c69  prefer a more li
-00001150: 6768 7477 6569 6768 7420 696e 7374 616c  ghtweight instal
-00001160: 6c61 7469 6f6e 2074 6861 7420 6f6e 6c79  lation that only
-00001170: 2069 6e63 6c75 6465 7320 7468 6520 7061   includes the pa
-00001180: 7274 7320 796f 7520 6163 7475 616c 6c79  rts you actually
-00001190: 206e 6565 642e 0a0a 2323 2044 6576 656c   need...## Devel
-000011a0: 6f70 6d65 6e74 0a0a 5379 6e74 6865 7365  opment..Synthese
-000011b0: 7573 2069 7320 6375 7272 656e 746c 7920  us is currently 
-000011c0: 756e 6465 7220 6163 7469 7665 2064 6576  under active dev
-000011d0: 656c 6f70 6d65 6e74 2e0a 4966 2079 6f75  elopment..If you
-000011e0: 2077 616e 7420 746f 2068 656c 7020 7573   want to help us
-000011f0: 2064 6576 656c 6f70 2073 796e 7468 6573   develop synthes
-00001200: 6575 7320 706c 6561 7365 2069 6e73 7461  eus please insta
-00001210: 6c6c 2061 6e64 2072 756e 2060 7072 652d  ll and run `pre-
-00001220: 636f 6d6d 6974 600a 6368 6563 6b73 2062  commit`.checks b
-00001230: 6566 6f72 6520 636f 6d6d 6974 7469 6e67  efore committing
-00001240: 2063 6f64 652e 0a0a 5765 2075 7365 2060   code...We use `
-00001250: 7079 7465 7374 6020 666f 7220 7465 7374  pytest` for test
-00001260: 696e 672e 2050 6c65 6173 6520 6d61 6b65  ing. Please make
-00001270: 2073 7572 6520 7465 7374 7320 7061 7373   sure tests pass
-00001280: 206f 6e20 796f 7572 2062 7261 6e63 6820   on your branch 
-00001290: 6265 666f 7265 0a73 7562 6d69 7474 696e  before.submittin
-000012a0: 6720 6120 5052 2028 616e 6420 7472 7920  g a PR (and try 
-000012b0: 746f 206d 6169 6e74 6169 6e20 6869 6768  to maintain high
-000012c0: 2074 6573 7420 636f 7665 7261 6765 292e   test coverage).
-000012d0: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
-000012e0: 202d 6d20 7079 7465 7374 202d 2d63 6f76   -m pytest --cov
-000012f0: 2073 796e 7468 6573 6575 732f 7465 7374   syntheseus/test
-00001300: 730a 6060 600a 0a23 2320 436f 6e74 7269  s.```..## Contri
-00001310: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
-00001320: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
-00001330: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
-00001340: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
-00001350: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
-00001360: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
-00001370: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
-00001380: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
-00001390: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
-000013a0: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
-000013b0: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
-000013c0: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
-000013d0: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
-000013e0: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
-000013f0: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
-00001400: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
-00001410: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
-00001420: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
-00001430: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
-00001440: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
-00001450: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
-00001460: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
-00001470: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
-00001480: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
-00001490: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
-000014a0: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
-000014b0: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
-000014c0: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
-000014d0: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
-000014e0: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
-000014f0: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
-00001500: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
-00001510: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
-00001520: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
-00001530: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
-00001540: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
-00001550: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
-00001560: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
-00001570: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
-00001580: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
-00001590: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
-000015a0: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
-000015b0: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
-000015c0: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
-000015d0: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
-000015e0: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
-000015f0: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
-00001600: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
-00001610: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
-00001620: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
-00001630: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
-00001640: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
-00001650: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
-00001660: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
-00001670: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
-00001680: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
-00001690: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
-000016a0: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
-000016b0: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
-000016c0: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
-000016d0: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
-000016e0: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
-000016f0: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
-00001700: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
-00001710: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
-00001720: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
-00001730: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
-00001740: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
-00001750: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
-00001760: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
-00001770: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
-00001780: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
-00001790: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
-000017a0: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
-000017b0: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
-000017c0: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
-000017d0: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
-000017e0: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
-000017f0: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
-00001800: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
-00001810: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
-00001820: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
-00001830: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
-00001840: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
-00001850: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
-00001860: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
-00001870: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
-00001880: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
-00001890: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
-000018a0: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
-000018b0: 6f6c 6963 6965 732e 0a                   olicies..
+00000870: 6f72 6d65 723d 3d30 2e31 2e31 3b20 6578  ormer==0.1.1; ex
+00000880: 7472 6120 3d3d 2022 6368 656d 666f 726d  tra == "chemform
+00000890: 6572 220a 5072 6f76 6964 6573 2d45 7874  er".Provides-Ext
+000008a0: 7261 3a20 6772 6170 6832 6564 6974 730a  ra: graph2edits.
+000008b0: 5265 7175 6972 6573 2d44 6973 743a 2073  Requires-Dist: s
+000008c0: 796e 7468 6573 6575 732d 6772 6170 6832  yntheseus-graph2
+000008d0: 6564 6974 733d 3d30 2e32 2e30 3b20 6578  edits==0.2.0; ex
+000008e0: 7472 6120 3d3d 2022 6772 6170 6832 6564  tra == "graph2ed
+000008f0: 6974 7322 0a50 726f 7669 6465 732d 4578  its".Provides-Ex
+00000900: 7472 613a 206c 6f63 616c 2d72 6574 726f  tra: local-retro
+00000910: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00000920: 7379 6e74 6865 7365 7573 2d6c 6f63 616c  syntheseus-local
+00000930: 2d72 6574 726f 3d3d 302e 342e 303b 2065  -retro==0.4.0; e
+00000940: 7874 7261 203d 3d20 226c 6f63 616c 2d72  xtra == "local-r
+00000950: 6574 726f 220a 5072 6f76 6964 6573 2d45  etro".Provides-E
+00000960: 7874 7261 3a20 6d65 6761 6e0a 5265 7175  xtra: megan.Requ
+00000970: 6972 6573 2d44 6973 743a 2073 796e 7468  ires-Dist: synth
+00000980: 6573 6575 732d 6d65 6761 6e3d 3d30 2e31  eseus-megan==0.1
+00000990: 2e30 3b20 6578 7472 6120 3d3d 2022 6d65  .0; extra == "me
+000009a0: 6761 6e22 0a50 726f 7669 6465 732d 4578  gan".Provides-Ex
+000009b0: 7472 613a 206d 686e 2d72 6561 6374 0a52  tra: mhn-react.R
+000009c0: 6571 7569 7265 732d 4469 7374 3a20 7379  equires-Dist: sy
+000009d0: 6e74 6865 7365 7573 2d6d 686e 7265 6163  ntheseus-mhnreac
+000009e0: 743d 3d31 2e30 2e30 3b20 6578 7472 6120  t==1.0.0; extra 
+000009f0: 3d3d 2022 6d68 6e2d 7265 6163 7422 0a50  == "mhn-react".P
+00000a00: 726f 7669 6465 732d 4578 7472 613a 2072  rovides-Extra: r
+00000a10: 6574 726f 2d6b 6e6e 0a52 6571 7569 7265  etro-knn.Require
+00000a20: 732d 4469 7374 3a20 7379 6e74 6865 7365  s-Dist: synthese
+00000a30: 7573 5b6c 6f63 616c 2d72 6574 726f 5d3b  us[local-retro];
+00000a40: 2065 7874 7261 203d 3d20 2272 6574 726f   extra == "retro
+00000a50: 2d6b 6e6e 220a 5265 7175 6972 6573 2d44  -knn".Requires-D
+00000a60: 6973 743a 2074 6f72 6368 2d73 6361 7474  ist: torch-scatt
+00000a70: 6572 3b20 6578 7472 6120 3d3d 2022 7265  er; extra == "re
+00000a80: 7472 6f2d 6b6e 6e22 0a50 726f 7669 6465  tro-knn".Provide
+00000a90: 732d 4578 7472 613a 2072 6f6f 742d 616c  s-Extra: root-al
+00000aa0: 6967 6e65 640a 5265 7175 6972 6573 2d44  igned.Requires-D
+00000ab0: 6973 743a 2073 796e 7468 6573 6575 732d  ist: syntheseus-
+00000ac0: 726f 6f74 2d61 6c69 676e 6564 3d3d 302e  root-aligned==0.
+00000ad0: 312e 303b 2065 7874 7261 203d 3d20 2272  1.0; extra == "r
+00000ae0: 6f6f 742d 616c 6967 6e65 6422 0a50 726f  oot-aligned".Pro
+00000af0: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
+00000b00: 2d73 696e 676c 652d 7374 6570 0a52 6571  -single-step.Req
+00000b10: 7569 7265 732d 4469 7374 3a20 7379 6e74  uires-Dist: synt
+00000b20: 6865 7365 7573 5b63 6865 6d66 6f72 6d65  heseus[chemforme
+00000b30: 722c 6772 6170 6832 6564 6974 732c 6c6f  r,graph2edits,lo
+00000b40: 6361 6c2d 7265 7472 6f2c 6d65 6761 6e2c  cal-retro,megan,
+00000b50: 6d68 6e2d 7265 6163 742c 7265 7472 6f2d  mhn-react,retro-
+00000b60: 6b6e 6e2c 726f 6f74 2d61 6c69 676e 6564  knn,root-aligned
+00000b70: 5d3b 2065 7874 7261 203d 3d20 2261 6c6c  ]; extra == "all
+00000b80: 2d73 696e 676c 652d 7374 6570 220a 5072  -single-step".Pr
+00000b90: 6f76 6964 6573 2d45 7874 7261 3a20 616c  ovides-Extra: al
+00000ba0: 6c0a 5265 7175 6972 6573 2d44 6973 743a  l.Requires-Dist:
+00000bb0: 2073 796e 7468 6573 6575 735b 616c 6c2d   syntheseus[all-
+00000bc0: 7369 6e67 6c65 2d73 7465 702c 6465 762c  single-step,dev,
+00000bd0: 7669 7a5d 3b20 6578 7472 6120 3d3d 2022  viz]; extra == "
+00000be0: 616c 6c22 0a0a 3c64 6976 2061 6c69 676e  all"..<div align
+00000bf0: 3d22 6365 6e74 6572 223e 0a20 2020 203c  ="center">.    <
+00000c00: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000c10: 2f67 6974 6875 622e 636f 6d2f 6d69 6372  /github.com/micr
+00000c20: 6f73 6f66 742f 7379 6e74 6865 7365 7573  osoft/syntheseus
+00000c30: 2f61 7373 6574 732f 3631 3437 3039 3233  /assets/61470923
+00000c40: 2f66 3031 6139 3933 392d 3631 6661 2d34  /f01a9939-61fa-4
+00000c50: 3436 312d 6131 3234 2d63 3133 6564 6463  461-a124-c13eddc
+00000c60: 6464 3735 6122 2068 6569 6768 743d 2235  dd75a" height="5
+00000c70: 3070 7822 3e0a 2020 2020 3c68 333e 3c69  0px">.    <h3><i
+00000c80: 3e4e 6176 6967 6174 696e 6720 7468 6520  >Navigating the 
+00000c90: 6c61 6279 7269 6e74 6820 6f66 2073 796e  labyrinth of syn
+00000ca0: 7468 6573 6973 2070 6c61 6e6e 696e 673c  thesis planning<
+00000cb0: 2f69 3e3c 2f68 333e 0a0a 2d2d 2d0a 0a3c  /i></h3>..---..<
+00000cc0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
+00000cd0: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
+00000ce0: 7073 3a2f 2f6d 6963 726f 736f 6674 2e67  ps://microsoft.g
+00000cf0: 6974 6875 622e 696f 2f73 796e 7468 6573  ithub.io/synthes
+00000d00: 6575 732f 7374 6162 6c65 223e 446f 6373  eus/stable">Docs
+00000d10: 3c2f 613e 20e2 80a2 0a20 203c 6120 6872  </a> ....  <a hr
+00000d20: 6566 3d22 6874 7470 733a 2f2f 6d69 6372  ef="https://micr
+00000d30: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
+00000d40: 7379 6e74 6865 7365 7573 2f73 7461 626c  syntheseus/stabl
+00000d50: 652f 636c 692f 6576 616c 5f73 696e 676c  e/cli/eval_singl
+00000d60: 655f 7374 6570 2f22 3e43 4c49 3c2f 613e  e_step/">CLI</a>
+00000d70: 20e2 80a2 0a20 203c 6120 6872 6566 3d22   ....  <a href="
+00000d80: 6874 7470 733a 2f2f 6d69 6372 6f73 6f66  https://microsof
+00000d90: 742e 6769 7468 7562 2e69 6f2f 7379 6e74  t.github.io/synt
+00000da0: 6865 7365 7573 2f73 7461 626c 652f 7475  heseus/stable/tu
+00000db0: 746f 7269 616c 732f 7175 6963 6b5f 7374  torials/quick_st
+00000dc0: 6172 742f 223e 5475 746f 7269 616c 733c  art/">Tutorials<
+00000dd0: 2f61 3e20 e280 a20a 2020 3c61 2068 7265  /a> ....  <a hre
+00000de0: 663d 2268 7474 7073 3a2f 2f61 7278 6976  f="https://arxiv
+00000df0: 2e6f 7267 2f61 6273 2f32 3331 302e 3139  .org/abs/2310.19
+00000e00: 3739 3622 3e50 6170 6572 3c2f 613e 0a3c  796">Paper</a>.<
+00000e10: 2f70 3e0a 0a5b 215b 4349 5d28 6874 7470  /p>..[![CI](http
+00000e20: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000e30: 6963 726f 736f 6674 2f73 796e 7468 6573  icrosoft/synthes
+00000e40: 6575 732f 6163 7469 6f6e 732f 776f 726b  eus/actions/work
+00000e50: 666c 6f77 732f 6369 2e79 6d6c 2f62 6164  flows/ci.yml/bad
+00000e60: 6765 2e73 7667 3f62 7261 6e63 683d 6d61  ge.svg?branch=ma
+00000e70: 696e 295d 2868 7474 7073 3a2f 2f67 6974  in)](https://git
+00000e80: 6875 622e 636f 6d2f 6d69 6372 6f73 6f66  hub.com/microsof
+00000e90: 742f 7379 6e74 6865 7365 7573 2f61 6374  t/syntheseus/act
+00000ea0: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f63  ions/workflows/c
+00000eb0: 692e 796d 6c29 0a5b 215b 5079 7468 6f6e  i.yml).[![Python
+00000ec0: 2056 6572 7369 6f6e 5d28 6874 7470 733a   Version](https:
+00000ed0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000ee0: 2f62 6164 6765 2f70 7974 686f 6e2d 332e  /badge/python-3.
+00000ef0: 372b 2d62 6c75 652e 7376 6729 5d28 6874  7+-blue.svg)](ht
+00000f00: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
+00000f10: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
+00000f20: 0a5b 215b 7079 7069 5d28 6874 7470 733a  .[![pypi](https:
+00000f30: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000f40: 2f70 7970 692f 762f 7379 6e74 6865 7365  /pypi/v/synthese
+00000f50: 7573 2e73 7667 295d 2868 7474 7073 3a2f  us.svg)](https:/
+00000f60: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000f70: 742f 7379 6e74 6865 7365 7573 2f29 0a5b  t/syntheseus/).[
+00000f80: 215b 636f 6465 2073 7479 6c65 5d28 6874  ![code style](ht
+00000f90: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000fa0: 732e 696f 2f62 6164 6765 2f63 6f64 6525  s.io/badge/code%
+00000fb0: 3230 7374 796c 652d 626c 6163 6b2d 3230  20style-black-20
+00000fc0: 3230 3230 2e73 7667 295d 2868 7474 7073  2020.svg)](https
+00000fd0: 3a2f 2f67 6974 6875 622e 636f 6d2f 616d  ://github.com/am
+00000fe0: 6276 2f62 6c61 636b 290a 5b21 5b4c 6963  bv/black).[![Lic
+00000ff0: 656e 7365 5d28 6874 7470 733a 2f2f 696d  ense](https://im
+00001000: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00001010: 6765 2f6c 6963 656e 7365 2d4d 4954 2d67  ge/license-MIT-g
+00001020: 7265 656e 2e73 7667 295d 2868 7474 7073  reen.svg)](https
+00001030: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d69  ://github.com/mi
+00001040: 6372 6f73 6f66 742f 7379 6e74 6865 7365  crosoft/synthese
+00001050: 7573 2f62 6c6f 622f 6d61 696e 2f4c 4943  us/blob/main/LIC
+00001060: 454e 5345 290a 0a3c 2f64 6976 3e0a 0a23  ENSE)..</div>..#
+00001070: 2320 4f76 6572 7669 6577 0a0a 5379 6e74  # Overview..Synt
+00001080: 6865 7365 7573 2069 7320 6120 7061 636b  heseus is a pack
+00001090: 6167 6520 666f 7220 656e 642d 746f 2d65  age for end-to-e
+000010a0: 6e64 2072 6574 726f 7379 6e74 6865 7469  nd retrosyntheti
+000010b0: 6320 706c 616e 6e69 6e67 2e0a 2d20 e29a  c planning..- ..
+000010c0: 92ef b88f 2043 6f6d 6269 6e65 7320 7365  .... Combines se
+000010d0: 6172 6368 2061 6c67 6f72 6974 686d 7320  arch algorithms 
+000010e0: 616e 6420 7265 6163 7469 6f6e 206d 6f64  and reaction mod
+000010f0: 656c 7320 696e 2061 2073 7461 6e64 6172  els in a standar
+00001100: 6469 7a65 6420 7761 790a 2d20 f09f a7ad  dized way.- ....
+00001110: 2049 6e63 6c75 6465 7320 696d 706c 656d   Includes implem
+00001120: 656e 7461 7469 6f6e 7320 6f66 2063 6f6d  entations of com
+00001130: 6d6f 6e20 7365 6172 6368 2061 6c67 6f72  mon search algor
+00001140: 6974 686d 730a 2d20 f09f a7aa 2049 6e63  ithms.- .... Inc
+00001150: 6c75 6465 7320 7772 6170 7065 7273 2066  ludes wrappers f
+00001160: 6f72 2073 7461 7465 2d6f 662d 7468 652d  or state-of-the-
+00001170: 6172 7420 7265 6163 7469 6f6e 206d 6f64  art reaction mod
+00001180: 656c 730a 2d20 e29a 99ef b88f 2045 7870  els.- ...... Exp
+00001190: 6f73 6573 2061 2073 696d 706c 6520 4150  oses a simple AP
+000011a0: 4920 746f 2070 6c75 6720 696e 2063 7573  I to plug in cus
+000011b0: 746f 6d20 6d6f 6465 6c73 2061 6e64 2061  tom models and a
+000011c0: 6c67 6f72 6974 686d 730a 2d20 f09f 9388  lgorithms.- ....
+000011d0: 2043 616e 2062 6520 7573 6564 2074 6f20   Can be used to 
+000011e0: 6265 6e63 686d 6172 6b20 636f 6d70 6f6e  benchmark compon
+000011f0: 656e 7473 206f 6620 6120 7265 7472 6f73  ents of a retros
+00001200: 796e 7468 6573 6973 2070 6970 656c 696e  ynthesis pipelin
+00001210: 650a 0a23 2320 5175 6963 6b20 5374 6172  e..## Quick Star
+00001220: 740a 0a54 6f20 696e 7374 616c 6c20 6073  t..To install `s
+00001230: 796e 7468 6573 6575 7360 2077 6974 6820  yntheseus` with 
+00001240: 616c 6c20 7468 6520 6578 7472 6173 2c20  all the extras, 
+00001250: 7275 6e0a 0a60 6060 6261 7368 0a63 6f6e  run..```bash.con
+00001260: 6461 2065 6e76 2063 7265 6174 6520 2d66  da env create -f
+00001270: 2065 6e76 6972 6f6e 6d65 6e74 5f66 756c   environment_ful
+00001280: 6c2e 796d 6c0a 636f 6e64 6120 6163 7469  l.yml.conda acti
+00001290: 7661 7465 2073 796e 7468 6573 6575 732d  vate syntheseus-
+000012a0: 6675 6c6c 0a0a 7069 7020 696e 7374 616c  full..pip instal
+000012b0: 6c20 2273 796e 7468 6573 6575 735b 616c  l "syntheseus[al
+000012c0: 6c5d 220a 6060 600a 0a53 6565 205b 6865  l]".```..See [he
+000012d0: 7265 5d28 6874 7470 733a 2f2f 6d69 6372  re](https://micr
+000012e0: 6f73 6f66 742e 6769 7468 7562 2e69 6f2f  osoft.github.io/
+000012f0: 7379 6e74 6865 7365 7573 2f69 6e73 7461  syntheseus/insta
+00001300: 6c6c 6174 696f 6e29 2069 6620 796f 7520  llation) if you 
+00001310: 7072 6566 6572 2061 206d 6f72 6520 6c69  prefer a more li
+00001320: 6768 7477 6569 6768 7420 696e 7374 616c  ghtweight instal
+00001330: 6c61 7469 6f6e 2074 6861 7420 6f6e 6c79  lation that only
+00001340: 2069 6e63 6c75 6465 7320 7468 6520 7061   includes the pa
+00001350: 7274 7320 796f 7520 6163 7475 616c 6c79  rts you actually
+00001360: 206e 6565 642e 0a0a 2323 2044 6576 656c   need...## Devel
+00001370: 6f70 6d65 6e74 0a0a 5379 6e74 6865 7365  opment..Synthese
+00001380: 7573 2069 7320 6375 7272 656e 746c 7920  us is currently 
+00001390: 756e 6465 7220 6163 7469 7665 2064 6576  under active dev
+000013a0: 656c 6f70 6d65 6e74 2e0a 4966 2079 6f75  elopment..If you
+000013b0: 2077 616e 7420 746f 2068 656c 7020 7573   want to help us
+000013c0: 2064 6576 656c 6f70 2073 796e 7468 6573   develop synthes
+000013d0: 6575 7320 706c 6561 7365 2069 6e73 7461  eus please insta
+000013e0: 6c6c 2061 6e64 2072 756e 2060 7072 652d  ll and run `pre-
+000013f0: 636f 6d6d 6974 600a 6368 6563 6b73 2062  commit`.checks b
+00001400: 6566 6f72 6520 636f 6d6d 6974 7469 6e67  efore committing
+00001410: 2063 6f64 652e 0a0a 5765 2075 7365 2060   code...We use `
+00001420: 7079 7465 7374 6020 666f 7220 7465 7374  pytest` for test
+00001430: 696e 672e 2050 6c65 6173 6520 6d61 6b65  ing. Please make
+00001440: 2073 7572 6520 7465 7374 7320 7061 7373   sure tests pass
+00001450: 206f 6e20 796f 7572 2062 7261 6e63 6820   on your branch 
+00001460: 6265 666f 7265 0a73 7562 6d69 7474 696e  before.submittin
+00001470: 6720 6120 5052 2028 616e 6420 7472 7920  g a PR (and try 
+00001480: 746f 206d 6169 6e74 6169 6e20 6869 6768  to maintain high
+00001490: 2074 6573 7420 636f 7665 7261 6765 292e   test coverage).
+000014a0: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+000014b0: 202d 6d20 7079 7465 7374 202d 2d63 6f76   -m pytest --cov
+000014c0: 2073 796e 7468 6573 6575 732f 7465 7374   syntheseus/test
+000014d0: 730a 6060 600a 0a23 2320 436f 6e74 7269  s.```..## Contri
+000014e0: 6275 7469 6e67 0a0a 5468 6973 2070 726f  buting..This pro
+000014f0: 6a65 6374 2077 656c 636f 6d65 7320 636f  ject welcomes co
+00001500: 6e74 7269 6275 7469 6f6e 7320 616e 6420  ntributions and 
+00001510: 7375 6767 6573 7469 6f6e 732e 2020 4d6f  suggestions.  Mo
+00001520: 7374 2063 6f6e 7472 6962 7574 696f 6e73  st contributions
+00001530: 2072 6571 7569 7265 2079 6f75 2074 6f20   require you to 
+00001540: 6167 7265 6520 746f 2061 0a43 6f6e 7472  agree to a.Contr
+00001550: 6962 7574 6f72 204c 6963 656e 7365 2041  ibutor License A
+00001560: 6772 6565 6d65 6e74 2028 434c 4129 2064  greement (CLA) d
+00001570: 6563 6c61 7269 6e67 2074 6861 7420 796f  eclaring that yo
+00001580: 7520 6861 7665 2074 6865 2072 6967 6874  u have the right
+00001590: 2074 6f2c 2061 6e64 2061 6374 7561 6c6c   to, and actuall
+000015a0: 7920 646f 2c20 6772 616e 7420 7573 0a74  y do, grant us.t
+000015b0: 6865 2072 6967 6874 7320 746f 2075 7365  he rights to use
+000015c0: 2079 6f75 7220 636f 6e74 7269 6275 7469   your contributi
+000015d0: 6f6e 2e20 466f 7220 6465 7461 696c 732c  on. For details,
+000015e0: 2076 6973 6974 2068 7474 7073 3a2f 2f63   visit https://c
+000015f0: 6c61 2e6f 7065 6e73 6f75 7263 652e 6d69  la.opensource.mi
+00001600: 6372 6f73 6f66 742e 636f 6d2e 0a0a 5768  crosoft.com...Wh
+00001610: 656e 2079 6f75 2073 7562 6d69 7420 6120  en you submit a 
+00001620: 7075 6c6c 2072 6571 7565 7374 2c20 6120  pull request, a 
+00001630: 434c 4120 626f 7420 7769 6c6c 2061 7574  CLA bot will aut
+00001640: 6f6d 6174 6963 616c 6c79 2064 6574 6572  omatically deter
+00001650: 6d69 6e65 2077 6865 7468 6572 2079 6f75  mine whether you
+00001660: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+00001670: 0a61 2043 4c41 2061 6e64 2064 6563 6f72  .a CLA and decor
+00001680: 6174 6520 7468 6520 5052 2061 7070 726f  ate the PR appro
+00001690: 7072 6961 7465 6c79 2028 652e 672e 2c20  priately (e.g., 
+000016a0: 7374 6174 7573 2063 6865 636b 2c20 636f  status check, co
+000016b0: 6d6d 656e 7429 2e20 5369 6d70 6c79 2066  mment). Simply f
+000016c0: 6f6c 6c6f 7720 7468 6520 696e 7374 7275  ollow the instru
+000016d0: 6374 696f 6e73 0a70 726f 7669 6465 6420  ctions.provided 
+000016e0: 6279 2074 6865 2062 6f74 2e20 596f 7520  by the bot. You 
+000016f0: 7769 6c6c 206f 6e6c 7920 6e65 6564 2074  will only need t
+00001700: 6f20 646f 2074 6869 7320 6f6e 6365 2061  o do this once a
+00001710: 6372 6f73 7320 616c 6c20 7265 706f 7320  cross all repos 
+00001720: 7573 696e 6720 6f75 7220 434c 412e 0a0a  using our CLA...
+00001730: 5468 6973 2070 726f 6a65 6374 2068 6173  This project has
+00001740: 2061 646f 7074 6564 2074 6865 205b 4d69   adopted the [Mi
+00001750: 6372 6f73 6f66 7420 4f70 656e 2053 6f75  crosoft Open Sou
+00001760: 7263 6520 436f 6465 206f 6620 436f 6e64  rce Code of Cond
+00001770: 7563 745d 2868 7474 7073 3a2f 2f6f 7065  uct](https://ope
+00001780: 6e73 6f75 7263 652e 6d69 6372 6f73 6f66  nsource.microsof
+00001790: 742e 636f 6d2f 636f 6465 6f66 636f 6e64  t.com/codeofcond
+000017a0: 7563 742f 292e 0a46 6f72 206d 6f72 6520  uct/)..For more 
+000017b0: 696e 666f 726d 6174 696f 6e20 7365 6520  information see 
+000017c0: 7468 6520 5b43 6f64 6520 6f66 2043 6f6e  the [Code of Con
+000017d0: 6475 6374 2046 4151 5d28 6874 7470 733a  duct FAQ](https:
+000017e0: 2f2f 6f70 656e 736f 7572 6365 2e6d 6963  //opensource.mic
+000017f0: 726f 736f 6674 2e63 6f6d 2f63 6f64 656f  rosoft.com/codeo
+00001800: 6663 6f6e 6475 6374 2f66 6171 2f29 206f  fconduct/faq/) o
+00001810: 720a 636f 6e74 6163 7420 5b6f 7065 6e63  r.contact [openc
+00001820: 6f64 6540 6d69 6372 6f73 6f66 742e 636f  ode@microsoft.co
+00001830: 6d5d 286d 6169 6c74 6f3a 6f70 656e 636f  m](mailto:openco
+00001840: 6465 406d 6963 726f 736f 6674 2e63 6f6d  de@microsoft.com
+00001850: 2920 7769 7468 2061 6e79 2061 6464 6974  ) with any addit
+00001860: 696f 6e61 6c20 7175 6573 7469 6f6e 7320  ional questions 
+00001870: 6f72 2063 6f6d 6d65 6e74 732e 0a0a 2323  or comments...##
+00001880: 2054 7261 6465 6d61 726b 730a 0a54 6869   Trademarks..Thi
+00001890: 7320 7072 6f6a 6563 7420 6d61 7920 636f  s project may co
+000018a0: 6e74 6169 6e20 7472 6164 656d 6172 6b73  ntain trademarks
+000018b0: 206f 7220 6c6f 676f 7320 666f 7220 7072   or logos for pr
+000018c0: 6f6a 6563 7473 2c20 7072 6f64 7563 7473  ojects, products
+000018d0: 2c20 6f72 2073 6572 7669 6365 732e 2041  , or services. A
+000018e0: 7574 686f 7269 7a65 6420 7573 6520 6f66  uthorized use of
+000018f0: 204d 6963 726f 736f 6674 0a74 7261 6465   Microsoft.trade
+00001900: 6d61 726b 7320 6f72 206c 6f67 6f73 2069  marks or logos i
+00001910: 7320 7375 626a 6563 7420 746f 2061 6e64  s subject to and
+00001920: 206d 7573 7420 666f 6c6c 6f77 0a5b 4d69   must follow.[Mi
+00001930: 6372 6f73 6f66 7427 7320 5472 6164 656d  crosoft's Tradem
+00001940: 6172 6b20 2620 4272 616e 6420 4775 6964  ark & Brand Guid
+00001950: 656c 696e 6573 5d28 6874 7470 733a 2f2f  elines](https://
+00001960: 7777 772e 6d69 6372 6f73 6f66 742e 636f  www.microsoft.co
+00001970: 6d2f 656e 2d75 732f 6c65 6761 6c2f 696e  m/en-us/legal/in
+00001980: 7465 6c6c 6563 7475 616c 7072 6f70 6572  tellectualproper
+00001990: 7479 2f74 7261 6465 6d61 726b 732f 7573  ty/trademarks/us
+000019a0: 6167 652f 6765 6e65 7261 6c29 2e0a 5573  age/general)..Us
+000019b0: 6520 6f66 204d 6963 726f 736f 6674 2074  e of Microsoft t
+000019c0: 7261 6465 6d61 726b 7320 6f72 206c 6f67  rademarks or log
+000019d0: 6f73 2069 6e20 6d6f 6469 6669 6564 2076  os in modified v
+000019e0: 6572 7369 6f6e 7320 6f66 2074 6869 7320  ersions of this 
+000019f0: 7072 6f6a 6563 7420 6d75 7374 206e 6f74  project must not
+00001a00: 2063 6175 7365 2063 6f6e 6675 7369 6f6e   cause confusion
+00001a10: 206f 7220 696d 706c 7920 4d69 6372 6f73   or imply Micros
+00001a20: 6f66 7420 7370 6f6e 736f 7273 6869 702e  oft sponsorship.
+00001a30: 0a41 6e79 2075 7365 206f 6620 7468 6972  .Any use of thir
+00001a40: 642d 7061 7274 7920 7472 6164 656d 6172  d-party trademar
+00001a50: 6b73 206f 7220 6c6f 676f 7320 6172 6520  ks or logos are 
+00001a60: 7375 626a 6563 7420 746f 2074 686f 7365  subject to those
+00001a70: 2074 6869 7264 2d70 6172 7479 2773 2070   third-party's p
+00001a80: 6f6c 6963 6965 732e 0a                   olicies..
```

### Comparing `syntheseus-0.3.0/syntheseus.egg-info/SOURCES.txt` & `syntheseus-0.4.0/syntheseus.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,27 @@
 SUPPORT.md
 environment.yml
 environment_full.yml
 mkdocs.yml
 pyproject.toml
 .github/azure_pipelines/code-security-analysis.yml
 .github/workflows/ci.yml
-.github/workflows/ci_integration.yml
 .github/workflows/docs.yml
+.github/workflows/release.yml
 docs/index.md
 docs/installation.md
 docs/single_step.md
 docs/cli/eval_single_step.md
+docs/cli/search.md
 docs/images/logo.png
 docs/images/logo.svg
+docs/tutorials/.gitignore
+docs/tutorials/custom_model.ipynb
+docs/tutorials/paroutes_benchmark.ipynb
+docs/tutorials/quick_start.ipynb
 syntheseus/__init__.py
 syntheseus/py.typed
 syntheseus.egg-info/PKG-INFO
 syntheseus.egg-info/SOURCES.txt
 syntheseus.egg-info/dependency_links.txt
 syntheseus.egg-info/entry_points.txt
 syntheseus.egg-info/requires.txt
@@ -34,14 +39,15 @@
 syntheseus/cli/main.py
 syntheseus/cli/search.py
 syntheseus/cli/search_config.yml
 syntheseus/interface/__init__.py
 syntheseus/interface/bag.py
 syntheseus/interface/models.py
 syntheseus/interface/molecule.py
+syntheseus/interface/reaction.py
 syntheseus/interface/typed_dict.py
 syntheseus/reaction_prediction/__init__.py
 syntheseus/reaction_prediction/chem/__init__.py
 syntheseus/reaction_prediction/chem/utils.py
 syntheseus/reaction_prediction/cli/__init__.py
 syntheseus/reaction_prediction/data/__init__.py
 syntheseus/reaction_prediction/data/dataset.py
@@ -50,39 +56,41 @@
 syntheseus/reaction_prediction/environment_gln/environment.yml
 syntheseus/reaction_prediction/inference/__init__.py
 syntheseus/reaction_prediction/inference/base.py
 syntheseus/reaction_prediction/inference/chemformer.py
 syntheseus/reaction_prediction/inference/config.py
 syntheseus/reaction_prediction/inference/default_checkpoint_links.yml
 syntheseus/reaction_prediction/inference/gln.py
+syntheseus/reaction_prediction/inference/graph2edits.py
 syntheseus/reaction_prediction/inference/local_retro.py
 syntheseus/reaction_prediction/inference/megan.py
 syntheseus/reaction_prediction/inference/mhnreact.py
 syntheseus/reaction_prediction/inference/retro_knn.py
 syntheseus/reaction_prediction/inference/root_aligned.py
+syntheseus/reaction_prediction/inference/toy_models.py
 syntheseus/reaction_prediction/models/__init__.py
 syntheseus/reaction_prediction/models/retro_knn.py
 syntheseus/reaction_prediction/utils/__init__.py
 syntheseus/reaction_prediction/utils/config.py
 syntheseus/reaction_prediction/utils/downloading.py
 syntheseus/reaction_prediction/utils/inference.py
 syntheseus/reaction_prediction/utils/metrics.py
 syntheseus/reaction_prediction/utils/misc.py
 syntheseus/reaction_prediction/utils/model_loading.py
 syntheseus/reaction_prediction/utils/parallel.py
-syntheseus/reaction_prediction/utils/syntheseus_wrapper.py
+syntheseus/reaction_prediction/utils/testing.py
 syntheseus/search/__init__.py
-syntheseus/search/chem.py
 syntheseus/search/mol_inventory.py
 syntheseus/search/visualization.py
 syntheseus/search/algorithms/__init__.py
 syntheseus/search/algorithms/base.py
 syntheseus/search/algorithms/breadth_first.py
 syntheseus/search/algorithms/mixins.py
 syntheseus/search/algorithms/pdvn.py
+syntheseus/search/algorithms/random.py
 syntheseus/search/algorithms/best_first/__init__.py
 syntheseus/search/algorithms/best_first/base.py
 syntheseus/search/algorithms/best_first/retro_star.py
 syntheseus/search/algorithms/mcts/__init__.py
 syntheseus/search/algorithms/mcts/base.py
 syntheseus/search/algorithms/mcts/molset.py
 syntheseus/search/analysis/__init__.py
@@ -98,61 +106,54 @@
 syntheseus/search/graph/standardization.py
 syntheseus/search/graph/message_passing/__init__.py
 syntheseus/search/graph/message_passing/run.py
 syntheseus/search/graph/message_passing/update_functions.py
 syntheseus/search/node_evaluation/__init__.py
 syntheseus/search/node_evaluation/base.py
 syntheseus/search/node_evaluation/common.py
-syntheseus/search/reaction_models/__init__.py
-syntheseus/search/reaction_models/base.py
-syntheseus/search/reaction_models/toy.py
 syntheseus/search/utils/__init__.py
 syntheseus/search/utils/misc.py
 syntheseus/tests/__init__.py
+syntheseus/tests/conftest.py
+syntheseus/tests/cli/__init__.py
+syntheseus/tests/cli/test_cli.py
+syntheseus/tests/cli/test_eval_single_step.py
 syntheseus/tests/interface/__init__.py
 syntheseus/tests/interface/test_bag.py
 syntheseus/tests/interface/test_models.py
 syntheseus/tests/interface/test_molecule.py
+syntheseus/tests/interface/test_reaction.py
+syntheseus/tests/interface/test_toy_models.py
 syntheseus/tests/reaction_prediction/__init__.py
 syntheseus/tests/reaction_prediction/chem/__init__.py
 syntheseus/tests/reaction_prediction/chem/test_utils.py
-syntheseus/tests/reaction_prediction/cli/__init__.py
-syntheseus/tests/reaction_prediction/cli/test_eval.py
 syntheseus/tests/reaction_prediction/data/__init__.py
 syntheseus/tests/reaction_prediction/data/test_dataset.py
 syntheseus/tests/reaction_prediction/inference/__init__.py
 syntheseus/tests/reaction_prediction/inference/test_models.py
 syntheseus/tests/reaction_prediction/utils/__init__.py
 syntheseus/tests/reaction_prediction/utils/test_misc.py
-syntheseus/tests/reaction_prediction/utils/test_syntheseus_wrapper.py
 syntheseus/tests/search/__init__.py
 syntheseus/tests/search/conftest.py
-syntheseus/tests/search/test_chem.py
 syntheseus/tests/search/test_mol_inventory.py
-syntheseus/tests/search/test_reaction_models.py
 syntheseus/tests/search/test_visualization.py
 syntheseus/tests/search/algorithms/__init__.py
 syntheseus/tests/search/algorithms/test_base.py
 syntheseus/tests/search/algorithms/test_best_first.py
 syntheseus/tests/search/algorithms/test_breadth_first.py
 syntheseus/tests/search/algorithms/test_mcts.py
 syntheseus/tests/search/algorithms/test_pdvn.py
+syntheseus/tests/search/algorithms/test_random.py
 syntheseus/tests/search/analysis/__init__.py
 syntheseus/tests/search/analysis/conftest.py
 syntheseus/tests/search/analysis/test_diversity.py
 syntheseus/tests/search/analysis/test_route_extraction.py
 syntheseus/tests/search/analysis/test_solution_time.py
 syntheseus/tests/search/graph/__init__.py
 syntheseus/tests/search/graph/test_andor.py
 syntheseus/tests/search/graph/test_base.py
 syntheseus/tests/search/graph/test_message_passing.py
 syntheseus/tests/search/graph/test_molset.py
 syntheseus/tests/search/graph/test_route.py
 syntheseus/tests/search/graph/test_standardization.py
 syntheseus/tests/search/node_evaluation/__init__.py
-syntheseus/tests/search/node_evaluation/test_common.py
-tutorials/search/1- end to end retrosynthesis with a toy model.ipynb
-tutorials/search/2a- advanced algorithms on PaRoutes.ipynb
-tutorials/search/2b- PaRoutes in-depth analysis.ipynb
-tutorials/search/__init__.py
-tutorials/search/paroutes.py
-tutorials/search/paroutes_setup.sh
+syntheseus/tests/search/node_evaluation/test_common.py
```

### Comparing `syntheseus-0.3.0/tutorials/search/2a- advanced algorithms on PaRoutes.ipynb` & `syntheseus-0.4.0/docs/tutorials/paroutes_benchmark.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9408289187161469%*

 * *Differences: {"'cells'": "{0: {'id': '0ee7dba4-df57-472d-85c8-f9dbc5a50066', 'source': {insert: [(0, 'In this "*

 * *            'in-depth tutorial, we use `syntheseus` to run part of the PaRoutes search '*

 * *            "benchmark.\\n'), (1, 'This tutorial will focus on the details of configuring search "*

 * *            "algorithms and analyzing search results.\\n'), (2, 'Note that the entire PaRoutes "*

 * *            "benchmark contains $10\\\\,000$ test molecules,\\n'), (3, 'but to allow the tutorial "*

 * *            "to run quickly  […]*

```diff
@@ -1,66 +1,50 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "db86ceb7-d2df-40d9-9bbb-f437d6114259",
+            "id": "0ee7dba4-df57-472d-85c8-f9dbc5a50066",
             "metadata": {},
             "source": [
-                "# Overview\n",
+                "In this in-depth tutorial, we use `syntheseus` to run part of the PaRoutes search benchmark.\n",
+                "This tutorial will focus on the details of configuring search algorithms and analyzing search results.\n",
+                "Note that the entire PaRoutes benchmark contains $10\\,000$ test molecules,\n",
+                "but to allow the tutorial to run quickly we will only use a single test molecule.\n",
                 "\n",
-                "This is the first part of a 2 part tutorial which runs the PaRoutes benchmark.\n",
-                "In this half of the tutorial, we run search algorithms using a pre-trained reaction model.\n",
-                "Because these algorithms require policies and value functions,\n",
-                "these must be carefully chosen before running the algorithm.\n",
-                "\n",
-                "**NOTE:** the PaRoutes reaction model requires the following additional packages:\n",
-                "- `pandas` (to load data table)\n",
-                "- `rdchiral` (to apply reaction templates)\n",
-                "- `keras` (their pre-trained model is a template-classification model using keras)\n",
-                "\n",
-                "The model also requires some data files, which can be downloaded with `paroutes_setup.sh`.",
-                "Running the following commands should set up everything:\n",
-                "\n",
-                "```\n",
-                "pip install -U tensorflow keras\n",
-                "conda install -c conda-forge rdchiral_cpp  # faster C++ version\n",
-                "conda install -c conda-forge pandas\n",
-                "cd tutorials/search  # need to be in this directory for the setup script to run correctly\n",
-                "bash paroutes_setup.sh\n",
+                "This tutorial uses a 3rd party wrapper for the PaRoutes benchmark,\n",
+                "available at: <https://github.com/AustinT/syntheseus-paroutes>.\n",
+                "\n",
+                "It can be installed by cloning the repository and adding it to `PYTHONPATH`,\n",
+                "or directly running:\n",
+                "\n",
+                "```bash\n",
+                "pip install syntheseus-paroutes\n",
                 "```"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "9dbc23a9-f0cd-4619-97c9-c24bdae7025e",
-            "metadata": {},
-            "source": [
-                "## Imports"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 1,
-            "id": "8160f287-de1e-46f4-a255-6e62aab0a460",
+            "id": "ae5a1bcf-3897-408f-b18a-c471e5e19546",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "import math\n",
-                "import pprint"
+                "from pprint import pprint"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
-            "id": "b4bd66f4-7c84-4ee7-870e-0b580443c61c",
+            "id": "0f1d19a5-bd9d-49d0-9ca7-2c206c0d364b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from syntheseus.search.chem import Molecule, BackwardReaction"
+                "from syntheseus import Molecule, SingleProductReaction"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "23fcbd26-c250-4d39-a92b-f0dd14e2f36f",
             "metadata": {},
             "source": [
@@ -92,343 +76,234 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e470b5bb-ae52-40c4-a342-10af36be9a74",
             "metadata": {},
             "source": [
-                "## Step 1: load PaRoutes mol-inventory and reaction model\n",
+                "## Step 1: load PaRoutes reaction model, inventory, and target molecules\n",
                 "\n",
-                "PaRoutes has two tasks: `n=1` and `n=5`.\n",
+                "There are two version of the PaRoutes benchmark,\n",
+                "denoted by `n=1` and `n=5`.\n",
                 "This notebook uses the `n=5` task by default,\n",
                 "but this can be changed with the variable `PAROUTES_N`.\n",
-                "We use version 2.0 of this benchmark which was released in late 2022.\n",
-                "\n",
-                "The file `paroutes.py` which accompanies this notebook contains wrappers for the pre-trained reaction models and sets of purchasable molecules.\n",
-                "We load these below and briefly explore their properties."
+                "We use version 2.0 of this benchmark which was released in late 2022."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "id": "5b060b2c-83d2-4a00-a303-ab7a5b77f21b",
+            "id": "f0b82a83-fe8b-4d89-8e41-e9bb95860c22",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": []
-                }
-            ],
+            "outputs": [],
             "source": [
-                "import paroutes\n",
                 "PAROUTES_N = 5"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "74baf3d7-1d3c-4c1e-9b24-b2de62cd072e",
-            "metadata": {},
-            "source": [
-                "#### 1a: load PaRoutes standardized mol inventory"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": 5,
-            "id": "9e8d0b43-bd7a-40b0-b327-3edb00a63407",
+            "id": "256ce92a-5f1f-48af-bc72-e6dfa60e318c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Size of inventory: 13325\n",
-                        "First few molecules in inventory:\n",
-                        "[Molecule(smiles='Cc1cc(C(C)N)cnc1OCC(F)(F)F', identifier=None, metadata={}),\n",
-                        " Molecule(smiles='N#CC1Cc2ccc(Nc3ccncc3[N+](=O)[O-])cc2C1',\n",
-                        "          identifier=None,\n",
-                        "          metadata={}),\n",
-                        " Molecule(smiles='COC=CC1CCCOC1', identifier=None, metadata={}),\n",
-                        " Molecule(smiles='CC(O)c1cccc(NCC(=O)OC(C)(C)C)n1',\n",
-                        "          identifier=None,\n",
-                        "          metadata={}),\n",
-                        " Molecule(smiles='CC(C)C[C@@H](C(=O)O)N(C)C(=O)OC(C)(C)C',\n",
-                        "          identifier=None,\n",
-                        "          metadata={})]\n"
+                        "First few predicted reactions for decane:\n",
+                        "\n",
+                        "['CCCCCCCCCCCO>>CCCCCCCCCC',\n",
+                        " 'CCCCCCCCCCO>>CCCCCCCCCC',\n",
+                        " 'CCCCCCCCCCCCCCCC>>CCCCCCCCCC']\n",
+                        "\n",
+                        "\n",
+                        "\n",
+                        "First few predicted reactions for benzene:\n",
+                        "\n",
+                        "['Nc1ccccc1>>c1ccccc1', 'O=C(O)c1ccccc1>>c1ccccc1', 'Oc1ccccc1>>c1ccccc1']\n"
                     ]
                 }
             ],
             "source": [
-                "# Load the inventory and look at the first few mols\n",
-                "inventory = paroutes.PaRoutesInventory(n=PAROUTES_N)\n",
-                "print(f\"Size of inventory: {len(inventory.purchasable_mols())}\")\n",
-                "print(\"First few molecules in inventory:\")\n",
-                "pprint.pprint(list(inventory.purchasable_mols())[:5])"
+                "# Load reaction model (same model for both `n`)\n",
+                "from syntheseus_paroutes import PaRoutesModel\n",
+                "reaction_model = PaRoutesModel(\n",
+                "    use_cache=True  # IMPORTANT, since it will be used for search\n",
+                ")  \n",
+                "print(\"First few predicted reactions for decane:\\n\")\n",
+                "pprint(list(map(str, reaction_model([decane], num_results=3)[0])))\n",
+                "print(\"\\n\\n\\nFirst few predicted reactions for benzene:\\n\")\n",
+                "pprint(list(map(str, reaction_model([benzene], num_results=3)[0])))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "b1e8c7b7-ee82-452a-bfd6-2b23a1d30f6e",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "(Molecule(smiles='c1ccccc1', identifier=None, metadata={'is_purchasable': True}),\n",
-                            " Molecule(smiles='CCCCCCCCCC', identifier=None, metadata={'is_purchasable': False}))"
-                        ]
-                    },
-                    "execution_count": 6,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# Example: Use the inventory to label some molecules\n",
-                "# We find out that benzene is purchasable and decane is not\n",
-                "inventory.fill_metadata(benzene)\n",
-                "inventory.fill_metadata(decane)\n",
-                "benzene, decane"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "1876bb42-3d95-4104-8b43-3caf1179d1de",
-            "metadata": {},
-            "source": [
-                "#### 1b: load PaRoutes reaction model and look at outputs"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 7,
-            "id": "b101e2c0-be72-4d2a-b12e-d182aaa304fc",
+            "id": "05361a34-92b9-4f42-84f9-13a0daf86747",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Output type: <class 'list'>, len: 2\n"
+                        "Size of inventory: 13326\n",
+                        "First few molecules in inventory:\n",
+                        "[Molecule(smiles='N#Cc1ccc(F)c(Cl)c1', identifier=None, metadata={}),\n",
+                        " Molecule(smiles='CC=C(CC)c1ccc(F)cc1', identifier=None, metadata={}),\n",
+                        " Molecule(smiles='CS(=O)(=O)c1ccc(F)c(Br)c1', identifier=None, metadata={}),\n",
+                        " Molecule(smiles='Cc1cc(C=O)ccc1O', identifier=None, metadata={}),\n",
+                        " Molecule(smiles='CCOC(=O)[C@@H]1C[C@H]1C(=O)O', identifier=None, metadata={})]\n"
                     ]
                 }
             ],
             "source": [
-                "# Load the reaction model, which is a template classifier\n",
-                "rxn_model = paroutes.PaRoutesModel()\n",
-                "\n",
-                "# Example: call it on benzene and decane.\n",
-                "# Like all reaction models, it returns a list of reaction lists (1 per input molecule)\n",
-                "rxn_model_output = rxn_model([benzene, decane])\n",
-                "print(f\"Output type: {type(rxn_model_output)}, len: {len(rxn_model_output)}\")"
+                "# Load inventory and print some info\n",
+                "from syntheseus_paroutes import PaRoutesInventory\n",
+                "inventory = PaRoutesInventory(n=PAROUTES_N)\n",
+                "print(f\"Size of inventory: {len(inventory.purchasable_mols())}\")\n",
+                "print(\"First few molecules in inventory:\")\n",
+                "pprint(list(inventory.purchasable_mols())[:5])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "id": "dbb7e430-7eab-4947-9446-c34a2e6ad486",
+            "execution_count": 7,
+            "id": "256137ca-e572-4840-a47f-9ab386799c5a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Reaction #1 for mol #1:\n",
-                        "BackwardReaction(reactants=frozenset({Molecule(smiles='Nc1ccccc1',\n",
-                        "                                               identifier=None,\n",
-                        "                                               metadata={})}),\n",
-                        "                 product=Molecule(smiles='c1ccccc1',\n",
-                        "                                  identifier=None,\n",
-                        "                                  metadata={'is_purchasable': True}),\n",
-                        "                 identifier=None,\n",
-                        "                 metadata={'softmax': 0.05530696362257004,\n",
-                        "                           'template': '[c:2]:[cH;D2;+0:1]:[c:3]>>N-[c;H0;D3;+0:1](:[c:2]):[c:3]',\n",
-                        "                           'template_idx': 15583,\n",
-                        "                           'template_library_occurence': 326,\n",
-                        "                           'template_rank': 0})\n",
-                        "\n",
-                        "Reaction #11 for mol #1:\n",
-                        "BackwardReaction(reactants=frozenset({Molecule(smiles='Brc1ccccc1',\n",
-                        "                                               identifier=None,\n",
-                        "                                               metadata={})}),\n",
-                        "                 product=Molecule(smiles='c1ccccc1',\n",
-                        "                                  identifier=None,\n",
-                        "                                  metadata={'is_purchasable': True}),\n",
-                        "                 identifier=None,\n",
-                        "                 metadata={'softmax': 0.0013848659582436085,\n",
-                        "                           'template': '[c:2]:[cH;D2;+0:1]:[c:3]>>Br-[c;H0;D3;+0:1](:[c:2]):[c:3]',\n",
-                        "                           'template_idx': 685,\n",
-                        "                           'template_library_occurence': 433,\n",
-                        "                           'template_rank': 34})\n",
-                        "\n"
+                        "Number of test SMILES: 10000\n",
+                        "First test SMILES:\n",
+                        "['COc1ccc(F)c(-c2ccc(COc3cc(C(CC(=O)O)C4CC4)ccc3F)nc2CC(C)(C)C)c1',\n",
+                        " 'CCc1cc2nncc(N3CCc4[nH]nc(C(=O)NC5CC5)c4C3)c2cc1OC',\n",
+                        " 'Clc1ccc(-n2cncn2)c(Cc2nc3c(NCCC4CCCCN4)nccc3o2)c1',\n",
+                        " 'CCOCc1nc2c(N)nc3ccc(O)cc3c2n1CC(C)(C)NS(C)(=O)=O',\n",
+                        " 'O=C(O)CCNC(=O)c1nc(-c2ccncc2)c2c(cc(-c3ccccc3)c(=O)n2CC2CCCCC2)c1O']\n"
                     ]
                 }
             ],
             "source": [
-                "# Examine some sample reactions\n",
-                "# Notice that the model includes a lot of metadata in the reaction objects,\n",
-                "# not just the products and reactants.\n",
-                "# Here, the metadata is the template used, the rank of the template and its softmax value,\n",
-                "# and the number of times the template occurred in the training data\n",
-                "for (i, j) in [(0, 0), (0, 10)]:\n",
-                "    print(f\"Reaction #{j+1} for mol #{i+1}:\")\n",
-                "    pprint.pprint(rxn_model_output[i][j])\n",
-                "    print()"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "6b95208e-ce3d-430d-a3d1-42867c345414",
-            "metadata": {},
-            "source": [
-                "#### 1c: load list of target molecules for search"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "id": "a27056ca-79cf-4ce1-a618-1a7310e50926",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "['COc1ccc(F)c(-c2ccc(COc3cc(C(CC(=O)O)C4CC4)ccc3F)nc2CC(C)(C)C)c1',\n",
-                            " 'CCc1cc2nncc(N3CCc4[nH]nc(C(=O)NC5CC5)c4C3)c2cc1OC',\n",
-                            " 'Clc1ccc(-n2cncn2)c(Cc2nc3c(NCCC4CCCCN4)nccc3o2)c1',\n",
-                            " 'CCOCc1nc2c(N)nc3ccc(O)cc3c2n1CC(C)(C)NS(C)(=O)=O',\n",
-                            " 'O=C(O)CCNC(=O)c1nc(-c2ccncc2)c2c(cc(-c3ccccc3)c(=O)n2CC2CCCCC2)c1O']"
-                        ]
-                    },
-                    "execution_count": 9,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# List of target molecules to synthesize\n",
-                "target_smiles_list = paroutes.get_target_smiles(n=PAROUTES_N)\n",
-                "target_smiles_list[:5]"
+                "# Load test smiles\n",
+                "from syntheseus_paroutes import get_target_smiles_list\n",
+                "test_smiles = get_target_smiles_list(n=PAROUTES_N)\n",
+                "print(f\"Number of test SMILES: {len(test_smiles)}\")\n",
+                "print(\"First test SMILES:\")\n",
+                "pprint(test_smiles[:5])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3359f01d-ddd1-4ad9-857e-9b93c787c074",
             "metadata": {},
             "source": [
                 "## Step 2: set up algorithms"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 8,
             "id": "f25c0a2a-9bbc-4692-a384-93eb219d3261",
             "metadata": {},
             "outputs": [],
             "source": [
+                "# Some constants for all algorithms\n",
                 "RXN_MODEL_CALL_LIMIT = 100\n",
                 "TIME_LIMIT_S = 300"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "df4f6506-0dcd-4296-b590-994ea69e9fa3",
             "metadata": {},
             "source": [
                 "### 2a: Retro-star\n",
                 "\n",
                 "Retro-star is a best-first search algorithm for AND/OR trees\n",
                 "which tries to find minimum-cost routes.\n",
-                "It requires 3 \"value functions\" to be provided to the algorithm.\n",
+                "It requires 3 cost functions to be provided to the algorithm.\n",
                 "\n",
                 "1. A function to give the cost of each molecule (OrNode)\n",
                 "2. A function to give the cost of each reaction (AndNode)\n",
-                "3. A function to estimate the minimum cost of leaf OrNodes (called the \"reaction number\" in the paper). This is effectively a value function in RL (except lower values are better)\n",
-                "\n",
-                "We will implement these using subclasses of `BaseNodeEvaluator` class from `syntheseus.search.node_evaluation`."
+                "3. A function to estimate the future cost to synthesize molecules, which is used as the search heuristic. This is called the \"reaction number\" in the original paper."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
-            "id": "29e52211-0eac-4467-92cd-b6bc3fe67fdf",
+            "execution_count": 9,
+            "id": "1309f29d-d935-40f1-b673-67dfa2cd9b21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from syntheseus.search.algorithms.best_first import retro_star\n",
                 "from syntheseus.search.graph.and_or import AndNode, OrNode, AndOrGraph\n",
-                "from syntheseus.search.node_evaluation import BaseNodeEvaluator"
+                "from syntheseus.search.node_evaluation.common import ReactionModelLogProbCost"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "id": "c891cc66-016e-456b-ada5-5f9f980e07a2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#1: OrNode cost function.\n",
-                "# We will follow the paper and give molecules a cost of 0 if they are purchasable,\n",
-                "# and a cost of infinity otherwise. This class is provided as a default in retro_star.\n",
-                "# If purchasable molecules have non-zero costs then a different cost function could be used\n",
+                "# 1: OrNode cost function.\n",
+                "# We will follow the original paper and give molecules a\n",
+                "# cost of 0 if they are purchasable, and a cost of infinity\n",
+                "# otherwise. This class is provided as a default in retro_star.\n",
+                "# If purchasable molecules have non-zero costs then a different\n",
+                "# cost function could be used.\n",
                 "\n",
                 "or_node_cost_fn = retro_star.MolIsPurchasableCost()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 11,
             "id": "b6e6d682-756a-4dcd-931b-097b27ca0ddd",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#2: AndNode cost function\n",
-                "# We will follow the original paper and define the cost of the reaction as the -log(softmax)\n",
-                "# of the reaction model output, thresholded at a minimum value\n",
-                "# This cost function is very specific to reactions from this particular reaction model though.\n",
-                "\n",
-                "class NegLogSoftmaxRxnCost(BaseNodeEvaluator[AndNode]):\n",
-                "    def __call__(self, nodes: list[AndNode], graph: AndOrGraph=None) -> list[float]:\n",
-                "        softmax_vals = [\n",
-                "            node.reaction.metadata[\"softmax\"]\n",
-                "            for node in nodes\n",
-                "        ]\n",
-                "        return [-math.log(max(val, 1e-4)) for val in softmax_vals]\n",
+                "# 2: AndNode cost function\n",
+                "# We will follow the original paper and define the cost of the\n",
+                "# reaction as the -log(softmax) of the reaction model output,\n",
+                "# thresholded at a minimum value. We use the built-in\n",
+                "# `ReactionModelLogProbCost` class for this. This class simply\n",
+                "# reads out the \"probability\" value from `reaction.metadata`,\n",
+                "# which is provided by the PaRoutesModel.\n",
                 "\n",
-                "and_node_cost_fn = NegLogSoftmaxRxnCost()"
+                "and_node_cost_fn = ReactionModelLogProbCost(normalize=False)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
-            "id": "ca316b02-b56f-41f8-b1dd-c814f8ad265b",
+            "execution_count": 12,
+            "id": "29e949b1-abc5-4514-aba7-7f86571425a8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#3: value function\n",
+                "# 3: search heuristic (value function)\n",
                 "# Here we just use a constant value function which is always 0,\n",
-                "# corresponding to the \"retro*-0\" algorithm (the most optimistic)\n",
+                "# corresponding to the \"retro*-0\" algorithm (the most optimistic).\n",
                 "\n",
                 "from syntheseus.search.node_evaluation.common import ConstantNodeEvaluator\n",
-                "\n",
                 "retro_star_value_function = ConstantNodeEvaluator(0.0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
-            "id": "578c26a3-340a-478e-9bfd-30528e28dfba",
+            "execution_count": 13,
+            "id": "2112a548-e2e1-4e85-873f-8654fac0b11f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Set up algorithm\n",
                 "retro_star_alg = retro_star.RetroStarSearch(\n",
-                "    reaction_model=rxn_model,\n",
+                "    reaction_model=reaction_model,\n",
                 "    mol_inventory=inventory,\n",
                 "    or_node_cost_fn=or_node_cost_fn,\n",
                 "    and_node_cost_fn=and_node_cost_fn,\n",
                 "    value_function=retro_star_value_function,\n",
                 "    limit_reaction_model_calls=RXN_MODEL_CALL_LIMIT,\n",
                 "    time_limit_s=TIME_LIMIT_S,\n",
                 ")"
@@ -440,107 +315,91 @@
             "metadata": {},
             "source": [
                 "### 2b: MCTS\n",
                 "\n",
                 "MCTS is an RL algorithm that tries to find routes of maximum value.\n",
                 "Standard MCTS works on an MDP where states are sets of molecules\n",
                 "and actions are backward reactions.\n",
-                "MCTS requires 2 input functions, with an optional third.\n",
+                "MCTS requires the following functions:\n",
                 "\n",
                 "1. A _reward function_ which defines the rewards for terminal states\n",
                 "2. A _value function_ which estimates the rewards attainable from a state\n",
-                "3. (optional) a policy which assigns higher numbers to desirable actions\n",
-                "\n",
-                "We will implement these using subclasses of `BaseNodeEvaluator` class from `syntheseus.search.node_evaluation`."
+                "3. (optional, but very useful) a policy which assigns higher numbers to desirable actions"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 14,
             "id": "af997a32-1f39-4788-b88a-463d92b7c9c6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from syntheseus.search.graph.molset import MolSetNode, MolSetGraph"
+                "from syntheseus.search.graph.molset import MolSetNode, MolSetGraph\n",
+                "from syntheseus.search.node_evaluation.common import ReactionModelProbPolicy"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 15,
             "id": "aa02eecf-71c9-4f17-bc21-5df514e7d4a7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#1: reward function\n",
-                "# Here we use the most basic reward: 1.0 if a state is solved (all molecules are purchasable),\n",
-                "# and 0.0 otherwise.\n",
+                "# 1: reward function\n",
+                "# Here we use the most basic reward: 1.0 if a state is solved\n",
+                "# (all molecules are purchasable), and 0.0 otherwise.\n",
                 "from syntheseus.search.node_evaluation.common import HasSolutionValueFunction\n",
                 "\n",
                 "mcts_reward_function = HasSolutionValueFunction()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 16,
             "id": "5bfd9f29-58af-4dc5-b760-20ee65979777",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#2: value function\n",
-                "# while previous works have used rollouts,\n",
+                "# 2: value function\n",
+                "# While previous works have used rollouts,\n",
                 "# for demonstration purposes we just use a constant value function of 0.5\n",
-                "# (this number is chosen to be between the lowest and highest rewards of 0/1\n",
+                "# (this number is chosen to be between the lowest and highest rewards of 0 & 1).\n",
                 "\n",
                 "mcts_value_function = ConstantNodeEvaluator(0.5)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
-            "id": "9db78293-5fbc-4d8f-9c3c-dfb3e3b3d3b5",
+            "execution_count": 17,
+            "id": "d803a733-e39a-4cb5-83ac-c952a20b3d39",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#3: policy\n",
-                "# this could be anything, and would often be another neural network in RL.\n",
-                "# However, for this example we just use the softmax values from the reaction model,\n",
-                "# normalized by the total number of reactions\n",
-                "# (note: this implementation will always call the policy on all of a node's children simultaneously)\n",
-                "\n",
-                "class MCTS_Reaction_Softmax_Policy(BaseNodeEvaluator[MolSetNode]):\n",
-                "    def __call__(self, nodes: list[MolSetNode], graph: MolSetGraph=None) -> list[float]:\n",
-                "        \n",
-                "        # This policy requires accessing the underlying graph to get the reaction\n",
-                "        assert graph is not None\n",
-                "        non_normalized_softmaxes: list[float] = []\n",
-                "        for node in nodes:\n",
-                "            parent_nodes = list(graph.predecessors(node))\n",
-                "            assert len(parent_nodes) == 1\n",
-                "            parent_rxn: BackwardReaction = graph._graph.edges[parent_nodes[0], node][\"reaction\"]\n",
-                "            non_normalized_softmaxes.append(parent_rxn.metadata[\"softmax\"])\n",
-                "        \n",
-                "        # Normalize the results\n",
-                "        normalization_constant = sum(non_normalized_softmaxes)\n",
-                "        return [v / normalization_constant for v in non_normalized_softmaxes]\n",
+                "# 3: policy\n",
+                "# This could be anything, and would often be another neural network in RL.\n",
+                "# However, for this example we just use the softmax values from the\n",
+                "# reaction model, scaled by a temperature and normalized across the total\n",
+                "# number of reactions (note: this implementation will always call the \n",
+                "# policy on all of a node's children simultaneously).\n",
                 "\n",
-                "mcts_policy = MCTS_Reaction_Softmax_Policy()"
+                "mcts_policy = ReactionModelProbPolicy(normalize=True, temperature=3.0)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "id": "4321240d-a248-4acb-9b28-706ef5bace14",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Set up algorithm\n",
                 "from syntheseus.search.algorithms.mcts.base import pucb_bound\n",
                 "from syntheseus.search.algorithms.mcts.molset import MolSetMCTS\n",
                 "mcts_alg = MolSetMCTS(\n",
-                "    reaction_model=rxn_model,\n",
+                "    reaction_model=reaction_model,\n",
                 "    mol_inventory=inventory,\n",
                 "    reward_function=mcts_reward_function,\n",
                 "    value_function=mcts_value_function,\n",
                 "    policy=mcts_policy,\n",
                 "    limit_reaction_model_calls=RXN_MODEL_CALL_LIMIT,\n",
                 "    bound_constant=100.0,\n",
                 "    bound_function=pucb_bound,\n",
@@ -552,107 +411,337 @@
             "cell_type": "markdown",
             "id": "933ae569-8e5a-4109-876b-d4ebd18836eb",
             "metadata": {},
             "source": [
                 "## Step 3: run algorithms and save results\n",
                 "\n",
                 "The main result needed for analysis is the output graph.\n",
-                "We will save this as a pickle file and analyze this in the next notebook."
+                "We will save the results as pickle files.\n",
+                "\n",
+                "**NOTE:** we call `alg.reset()` before running both algorithms\n",
+                "to reset the underlying reaction model cache. Otherwise,\n",
+                "the algorithm which is run second will use the cached values \n",
+                "from the first search instead of actually calling the reaction model,\n",
+                "allowing it to run much faster. This is not necessarily a bad thing\n",
+                "(in fact in production it might actually be beneficial), but for the\n",
+                "purposes of comparing algorithms calling `reset()` ensures a fair comparsion."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 21,
+            "execution_count": 19,
             "id": "656bb71b-fabe-4b34-99cc-b0d9c43e65e9",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "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",
                         "text/plain": [
-                            "<rdkit.Chem.rdchem.Mol at 0x7f3724621850>"
+                            "<rdkit.Chem.rdchem.Mol at 0x7f98a412d350>"
                         ]
                     },
-                    "execution_count": 21,
+                    "execution_count": 19,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "target_mol = Molecule(target_smiles_list[100])\n",
+                "target_mol = Molecule(test_smiles[100])\n",
                 "target_mol.rdkit_mol"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 22,
+            "execution_count": 20,
             "id": "5af33f0f-daad-49ea-8d36-2d898fec07d6",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "CPU times: user 14 s, sys: 83.4 ms, total: 14.1 s\n",
-                        "Wall time: 12.6 s\n"
+                        "CPU times: user 5.24 s, sys: 2.61 ms, total: 5.24 s\n",
+                        "Wall time: 5.23 s\n"
                     ]
                 }
             ],
             "source": [
                 "%%time\n",
                 "# Run retro-star\n",
                 "retro_star_alg.reset()\n",
                 "retro_star_search_graph, _ = retro_star_alg.run_from_mol(target_mol)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": 21,
             "id": "d6af0d40-c7fb-48d8-b63c-42762e46976d",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "CPU times: user 14.7 s, sys: 168 ms, total: 14.9 s\n",
-                        "Wall time: 13.4 s\n"
+                        "CPU times: user 5.32 s, sys: 3.4 ms, total: 5.32 s\n",
+                        "Wall time: 5.27 s\n"
                     ]
                 }
             ],
             "source": [
                 "%%time\n",
                 "# Run MCTS\n",
                 "mcts_alg.reset()\n",
                 "mcts_search_graph, _ = mcts_alg.run_from_mol(target_mol)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 24,
+            "execution_count": 22,
             "id": "2907cca5-c96c-473b-b257-c5f333685b95",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "retro star graph size: 17108\n",
-                        "mcts graph size: 13380\n"
+                        "retro star graph size: 17950\n",
+                        "mcts graph size: 6182\n"
                     ]
                 }
             ],
             "source": [
                 "# Save graphs\n",
                 "import pickle\n",
-                "for graph, alg_name in [(retro_star_search_graph, \"retro star\"), (mcts_search_graph, \"mcts\")]:\n",
+                "for graph, alg_name in [\n",
+                "    (retro_star_search_graph, \"retro star\"),\n",
+                "    (mcts_search_graph, \"mcts\")\n",
+                "]:\n",
                 "    print(f\"{alg_name} graph size: {len(graph)}\")\n",
                 "    with open(f\"search-results-{alg_name}.pkl\", \"wb\") as f:\n",
                 "        pickle.dump(graph, f)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "af20ffc6-183a-4133-98da-fdba978ad270",
+            "metadata": {},
+            "source": [
+                "## Step 4: analyze search results\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 23,
+            "id": "65fb455b-5d25-4545-ba77-d88700e193d7",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# Create a dict to easily reference both search graphs\n",
+                "alg_name_to_graph = {\n",
+                "    \"retro star\": retro_star_search_graph,\n",
+                "    \"mcts\": mcts_search_graph,\n",
+                "}"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "8ae1c35a-cd8f-40f4-8a84-9d9f22ce7f07",
+            "metadata": {},
+            "source": [
+                "### 4a: time at which a solution is found\n",
+                "\n",
+                "The code is written in a way where nodes keep track of their own\n",
+                "creation time, so time-based measures can be computed retrospectively for\n",
+                "many time measures\n",
+                "(e.g. wallclock time, number of calls to reaction model).\n",
+                "For any analysis involving time, we need to choose how time is measured,\n",
+                "and this is left up to the user by filling in the `analysis_time` field of each node's data."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 24,
+            "id": "97c1fb44-3344-4031-9301-654689f6fc2b",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for graph in alg_name_to_graph.values():\n",
+                "    for node in graph.nodes():\n",
+                "        \n",
+                "        # Wallclock time: difference between this node's\n",
+                "        # creation time and that of the root node\n",
+                "        node.data[\"analysis_time\"] = (\n",
+                "            node.creation_time - \n",
+                "            graph.root_node.creation_time\n",
+                "        ).total_seconds()\n",
+                "        \n",
+                "        # Could alternatively use number of calls to reaction model\n",
+                "        # node.data[\"analysis_time\"] = node.data[\"num_calls_rxn_model\"]"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 25,
+            "id": "cd66b4b2-df67-4e78-8b30-cbae073bf9d8",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "retro star first solution: 0.652155\n",
+                        "mcts first solution: 2.286357\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# Now use a function to compute the first solution time\n",
+                "from syntheseus.search.analysis.solution_time import get_first_solution_time\n",
+                "for alg_name, graph in alg_name_to_graph.items():\n",
+                "    print(f\"{alg_name} first solution: {get_first_solution_time(graph)}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "e7d8de5d-cebf-486d-89db-3cf1d38da3e7",
+            "metadata": {},
+            "source": [
+                "### 4b: extract synthesis routes from the search graphs\n",
+                "\n",
+                "We extract individual synthesis routes from the graph\n",
+                "in order to later calculate their diversity.\n",
+                "However, there are many possible routes in a graph,\n",
+                "possibly too many to exhaustively enumerate.\n",
+                "Therefore we only extract the _minimum cost_ routes,\n",
+                "where the cost of each route is the sum of `node.data[\"route_cost\"]` for each\n",
+                "node in the route.\n",
+                "This cost could be anything: a constant,\n",
+                "something based on the policy, etc.\n",
+                "It is up to the user to set a route's cost.\n",
+                "Here we just assign a constant cost to each node which represents a reaction\n",
+                "(i.e. AndNodes and MolSetNodes).\n",
+                "This means that the lowest cost routes will be the shortest routes.\n",
+                "\n",
+                "We also limit the maximum number of routes extracted to speed up computation time."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 26,
+            "id": "a8858c30-4e71-42bd-b4cc-69e2bf855dae",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "for graph in alg_name_to_graph.values():\n",
+                "    for node in graph.nodes():\n",
+                "        \n",
+                "        if isinstance(node, (AndNode, MolSetNode)):\n",
+                "            node.data[\"route_cost\"] = 1.0\n",
+                "        else:\n",
+                "            node.data[\"route_cost\"] = 0.0"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 27,
+            "id": "80c86fd0-cc95-4daa-bed2-83dcb7fec0bd",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Found 10000 routes for retro star\n",
+                        "Found 14 routes for mcts\n",
+                        "CPU times: user 10.4 s, sys: 23.5 ms, total: 10.4 s\n",
+                        "Wall time: 10.4 s\n"
+                    ]
+                }
+            ],
+            "source": [
+                "%%time\n",
+                "from syntheseus.search.analysis import route_extraction\n",
+                "alg_name_to_routes = dict()\n",
+                "for alg_name, graph in alg_name_to_graph.items():\n",
+                "    routes = list(route_extraction.iter_routes_cost_order(graph, 10_000))\n",
+                "    print(f\"Found {len(routes)} routes for {alg_name}\", flush=True)\n",
+                "    alg_name_to_routes[alg_name] = routes\n",
+                "    del routes"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 28,
+            "id": "f7f427c0-fb49-4e99-ad40-1eb96c2f5f91",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "# The routes can be visualized with the code below.\n",
+                "from syntheseus.search import visualization\n",
+                "\n",
+                "visualization.visualize_andor(\n",
+                "    alg_name_to_graph[\"retro star\"],\n",
+                "    filename=\"retro star route.pdf\",\n",
+                "    nodes=alg_name_to_routes[\"retro star\"][0]\n",
+                ")\n",
+                "\n",
+                "visualization.visualize_molset(\n",
+                "    alg_name_to_graph[\"mcts\"],\n",
+                "    filename=\"mcts route.pdf\",\n",
+                "    nodes=alg_name_to_routes[\"mcts\"][0]\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "ae2107ac-d200-42b0-9f05-5fbc01fc048f",
+            "metadata": {},
+            "source": [
+                "### 4c: calculate diversity\n",
+                "\n",
+                "Specifically, we estimate the _packing number_ of the route set,\n",
+                "i.e. the number of distinct routes which are greater than a distance $r$ away from each other.\n",
+                "Here we use a stringent form of diversity: routes which have no common reactions,\n",
+                "which means that their Jaccard distance is 1.\n",
+                "To do this, we use the `to_synthesis_graph` method of each graph object\n",
+                "which converts them into a common format.\n",
+                "\n",
+                "However, because we considered only a limited number of synthesis routes,\n",
+                "the full diversity of routes from retro* might not be represented."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 29,
+            "id": "bfdad9e4-1b92-4214-808e-7652a2e4cbea",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "retro star: number of distinct routes = 1\n",
+                        "mcts: number of distinct routes = 2\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from syntheseus.search.analysis import diversity\n",
+                "for alg_name, graph in alg_name_to_graph.items():\n",
+                "    route_objects = [\n",
+                "        graph.to_synthesis_graph(nodes)\n",
+                "        for nodes in alg_name_to_routes[alg_name]\n",
+                "    ]\n",
+                "    packing_set = diversity.estimate_packing_number(\n",
+                "        routes=route_objects,\n",
+                "        distance_metric=diversity.reaction_jaccard_distance,\n",
+                "        radius=0.999  # because comparison uses \">\", not \">=\"\n",
+                "    )\n",
+                "    print(f\"{alg_name}: number of distinct routes = {len(packing_set)}\")"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -663,13 +752,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.9.7"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `syntheseus-0.3.0/tutorials/search/2b- PaRoutes in-depth analysis.ipynb` & `syntheseus-0.4.0/docs/tutorials/quick_start.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8020827090370855%*

 * *Differences: {"'cells'": '{1: {\'source\': ["Let\'s start by creating a test molecule and querying LocalRetro '*

 * *            'for proposed reactions."], delete: [\'id\']}, 2: {\'source\': [\'from syntheseus '*

 * *            "import Molecule\\n', 'from syntheseus.reaction_prediction.inference import "*

 * *            'LocalRetroModel\\n\', \'\\n\', \'test_mol = Molecule("Cc1ccc(-c2ccc(C)cc2)cc1")\\n\', '*

 * *            "'model = LocalRetroModel()'], delete: ['id']}, 4: {'outputs': [OrderedDict([('name', "*

 * *            "'stdout'), (' […]*

```diff
@@ -1,275 +1,300 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "id": "84a8ae1e-5fa1-417a-9653-a5de6447b464",
             "metadata": {},
             "source": [
-                "# Overview\n",
-                "\n",
-                "This is the second part of a 2 part tutorial which runs the PaRoutes benchmark.\n",
-                "Running this notebook requires that part 2a is already run.\n",
-                "In this half of the tutorial, we analyze the results of search algorithms.\n",
-                "\n",
-                "\"Analysis\" can be many things. In this notebook we focus on the time when a solution is found\n",
-                "and the number of diverse solutions found.\n",
-                "We also visualize the routes."
+                "## Setting up a single-step model"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 1,
-            "id": "a6ee7147-2dd0-4bc8-b54d-12744261fd32",
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "from __future__ import annotations\n",
-                "import math\n",
-                "from pathlib import Path\n",
-                "import pickle\n",
-                "import pprint"
+                "Let's start by creating a test molecule and querying LocalRetro for proposed reactions."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
-            "id": "a3c36718-1daa-406b-b87d-6913e60509c0",
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from syntheseus.search.graph.molset import MolSetNode, MolSetGraph\n",
-                "from syntheseus.search.graph.and_or import AndNode, OrNode, AndOrGraph"
+                "from syntheseus import Molecule\n",
+                "from syntheseus.reaction_prediction.inference import LocalRetroModel\n",
+                "\n",
+                "test_mol = Molecule(\"Cc1ccc(-c2ccc(C)cc2)cc1\")\n",
+                "model = LocalRetroModel()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c9e03f8a-9e46-4c26-9cdf-903da9db2b07",
             "metadata": {},
             "source": [
-                "## Step 1: load results from notebook 2a"
+                "Note that we didn't provide a path to the model checkpoint, so `syntheseus` will download a default checkpoint trained on USPTO-50K and cache it for later use. This behaviour can be overriden by providing a `model_dir` argument."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
-            "id": "cb398e9e-2ac7-4b5e-88ac-a6af3780881b",
+            "execution_count": 2,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "/home/krmaziar/.cache/torch/syntheseus/LocalRetro_backward\n"
+                    ]
+                }
+            ],
             "source": [
-                "# Load pickle files\n",
-                "alg_name_to_graph = dict()\n",
-                "for alg_name in [\"retro star\", \"mcts\"]:\n",
-                "    with open(f\"./search-results-{alg_name}.pkl\", \"rb\") as f: \n",
-                "        alg_name_to_graph[alg_name] = pickle.load(f)"
+                "print(model.model_dir)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "843e67fd-2521-485d-af19-643805800a7d",
             "metadata": {},
             "source": [
-                "## Step 2: time at which a solution is found \n",
-                "\n",
-                "The code is written in a way where nodes keep track of their own\n",
-                "creation time, so time-based measures can be computed retrospectively for\n",
-                "many time measures\n",
-                "(e.g. wallclock time, number of calls to reaction model).\n",
-                "For any analysis involving time, we need to choose how time is measured,\n",
-                "and this is left up to the user by filling in the `analysis_time` field of each node's data."
+                "Now let's print the top 5 predictions for our test molecule."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
-            "id": "97c1fb44-3344-4031-9301-654689f6fc2b",
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "1: Cc1ccc(B(O)O)cc1 + Cc1ccc(Br)cc1\n",
+                        "2: Cc1ccc(B(O)O)cc1 + Cc1ccc(I)cc1\n",
+                        "3: Cc1ccc(Br)cc1 + Cc1ccc([Mg+])cc1\n"
+                    ]
+                }
+            ],
             "source": [
-                "for graph in alg_name_to_graph.values():\n",
-                "    for node in graph.nodes():\n",
-                "        \n",
-                "        # Wallclock time: difference between this node's creation time and that of the root node\n",
-                "        node.data[\"analysis_time\"] = (node.creation_time - graph.root_node.creation_time).total_seconds()\n",
-                "        \n",
-                "        # Could alternatively use number of calls to reaction model\n",
-                "        # node.data[\"analysis_time\"] = node.data[\"num_calls_rxn_model\"]"
+                "def mols_to_str(mols) -> str:\n",
+                "    return \" + \".join([mol.smiles for mol in mols])\n",
+                "\n",
+                "def print_results(results) -> None:\n",
+                "    for idx, prediction in enumerate(results):\n",
+                "        print(f\"{idx + 1}: \" + mols_to_str(prediction.reactants))\n",
+                "\n",
+                "[results] = model([test_mol], num_results=5)\n",
+                "print_results(results)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We only got 3 results (despite requesting 5) as `syntheseus` automatically deduplicates the model outputs.\n",
+                "\n",
+                "As all single-step models are set up in a consistent way, it's easy to run several models and compare their outputs."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
-            "id": "cd66b4b2-df67-4e78-8b30-cbae073bf9d8",
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "retro star first solution: 1.205841\n",
-                        "mcts first solution: 1.267164\n"
+                        "Chemformer:  Cc1ccc(Br)cc1 + Cc1ccc(Br)cc1\n",
+                        "Graph2Edits: Cc1ccc(Br)cc1 + Cc1ccc([Sn](C)(C)C)cc1\n",
+                        "LocalRetro:  Cc1ccc(B(O)O)cc1 + Cc1ccc(Br)cc1\n",
+                        "MEGAN:       Cc1ccc(Br)cc1 + Cc1ccc([Mg+])cc1\n",
+                        "MHNreact:    Cc1ccc(Br)cc1 + Cc1ccc([Mg+])cc1\n",
+                        "RetroKNN:    Cc1ccc(B(O)O)cc1 + Cc1ccc(Br)cc1\n",
+                        "RootAligned: Cc1ccc(Br)cc1 + Cc1ccc([Mg+])cc1\n"
                     ]
                 }
             ],
             "source": [
-                "# Now use a function to compute the first solution time\n",
-                "from syntheseus.search.analysis.solution_time import get_first_solution_time\n",
-                "for alg_name, graph in alg_name_to_graph.items():\n",
-                "    print(f\"{alg_name} first solution: {get_first_solution_time(graph)}\")"
+                "from syntheseus.reaction_prediction.inference import *\n",
+                "\n",
+                "models = [\n",
+                "    ChemformerModel(),\n",
+                "    Graph2EditsModel(),\n",
+                "    LocalRetroModel(),\n",
+                "    MEGANModel(),\n",
+                "    MHNreactModel(),\n",
+                "    RetroKNNModel(),\n",
+                "    RootAlignedModel(),\n",
+                "]\n",
+                "\n",
+                "for model in models:\n",
+                "    # When interested in very few predictions (e.g. one), it may be\n",
+                "    # useful to set `num_results > 1`, as this will cause e.g.\n",
+                "    # larger beam size for models based on beam search.\n",
+                "    [results] = model([test_mol], num_results=5)\n",
+                "\n",
+                "    top_prediction = results[0].reactants\n",
+                "    print(f\"{model.name + ':':12} {mols_to_str(top_prediction)}\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Running search"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5a16439c-309d-4abe-854f-3010666a7f50",
             "metadata": {},
             "source": [
-                "## Step 3: extract routes\n",
+                "To run multi-step search we need three things:\n",
+                "- a reaction model\n",
+                "- an inventory of purchasable (building block) molecules\n",
+                "- a search algorithm"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 5,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from syntheseus.search.mol_inventory import SmilesListInventory\n",
+                "from syntheseus.search.algorithms.breadth_first import (\n",
+                "    AndOr_BreadthFirstSearch\n",
+                ")\n",
+                "\n",
+                "# Set up a reaction model with caching enabled. Number of reactions\n",
+                "# to request from the model at each step of the search needs to be\n",
+                "# provided at construction time.\n",
+                "model = LocalRetroModel(use_cache=True, default_num_results=10)\n",
                 "\n",
-                "We extract individual synthesis routes from the graph\n",
-                "in order to later calculate their diversity.\n",
-                "However, there are many possible routes in a graph,\n",
-                "possibly too many to exhaustively enumerate.\n",
-                "Therefore we only extract the _minimum cost_ routes,\n",
-                "where the cost of each route is the sum of `node.data[\"route_cost\"]` for each\n",
-                "node in the route.\n",
-                "This cost could be anything: a constant,\n",
-                "something based on the policy, etc.\n",
-                "It is up to the user to set a route's cost.\n",
-                "Here we just assign a constant cost to each node which represents a reaction\n",
-                "(i.e. AndNodes and MolSetNodes).\n",
-                "This means that the lowest cost routes will be the shortest routes.\n",
+                "# Dummy inventory with just two purchasable molecules.\n",
+                "inventory = SmilesListInventory(\n",
+                "    smiles_list=[\"Cc1ccc(B(O)O)cc1\", \"O=Cc1ccc(I)cc1\"]\n",
+                ")\n",
                 "\n",
-                "We also limit the maximum number of routes extracted to speed up computation time."
+                "search_algorithm = AndOr_BreadthFirstSearch(\n",
+                "    reaction_model=model,\n",
+                "    mol_inventory=inventory,\n",
+                "    limit_iterations=100,  # max number of algorithm iterations\n",
+                "    limit_reaction_model_calls=100,  # max number of model calls\n",
+                "    time_limit_s=60.0  # max runtime in seconds\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
-            "id": "a8858c30-4e71-42bd-b4cc-69e2bf855dae",
             "metadata": {},
             "outputs": [],
             "source": [
-                "for graph in alg_name_to_graph.values():\n",
-                "    for node in graph.nodes():\n",
-                "        \n",
-                "        if isinstance(node, (AndNode, MolSetNode)):\n",
-                "            node.data[\"route_cost\"] = 1.0\n",
-                "        else:\n",
-                "            node.data[\"route_cost\"] = 0.0"
+                "output_graph, _ = search_algorithm.run_from_mol(test_mol)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 7,
-            "id": "80c86fd0-cc95-4daa-bed2-83dcb7fec0bd",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Found 10000 routes for retro star\n",
-                        "Found 422 routes for mcts\n",
-                        "CPU times: user 11.3 s, sys: 54.8 ms, total: 11.4 s\n",
-                        "Wall time: 11.4 s\n"
+                        "Explored 1256 nodes\n"
                     ]
                 }
             ],
             "source": [
-                "%%time\n",
-                "from syntheseus.search.analysis import route_extraction\n",
-                "alg_name_to_routes = dict()\n",
-                "for alg_name, graph in alg_name_to_graph.items():\n",
-                "    routes = list(route_extraction.iter_routes_cost_order(graph, 10_000))\n",
-                "    print(f\"Found {len(routes)} routes for {alg_name}\", flush=True)\n",
-                "    alg_name_to_routes[alg_name] = routes\n",
-                "    del routes"
+                "print(f\"Explored {len(output_graph)} nodes\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The resulting graph contains all the explored molecules and reactions, some of which might have led to complete routes while others remained unsolved. From that we can extract complete routes."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
-            "id": "f7f427c0-fb49-4e99-ad40-1eb96c2f5f91",
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Route 1 consists of 2 reactions\n",
+                        "Route 2 consists of 3 reactions\n"
+                    ]
+                }
+            ],
             "source": [
-                "# We visualize the routes just to get a sense of what they look like\n",
-                "from syntheseus.search import visualization\n",
-                "\n",
-                "visualization.visualize_andor(\n",
-                "    alg_name_to_graph[\"retro star\"],\n",
-                "    filename=\"retro star route.pdf\",\n",
-                "    nodes=alg_name_to_routes[\"retro star\"][0]\n",
+                "from syntheseus.search.analysis.route_extraction import (\n",
+                "    iter_routes_time_order,\n",
                 ")\n",
+                "from syntheseus.search.graph.and_or import AndNode\n",
                 "\n",
-                "visualization.visualize_molset(\n",
-                "    alg_name_to_graph[\"mcts\"],\n",
-                "    filename=\"mcts route.pdf\",\n",
-                "    nodes=alg_name_to_routes[\"mcts\"][0]\n",
-                ")"
+                "# Extract the routes simply in the order they were found.\n",
+                "routes = list(iter_routes_time_order(output_graph, max_routes=10))\n",
+                "\n",
+                "for idx, route in enumerate(routes):\n",
+                "    num_reactions = len({n for n in route if isinstance(n, AndNode)})\n",
+                "    print(f\"Route {idx + 1} consists of {num_reactions} reactions\")"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "5c849f47-899d-44ba-8e54-a25dadeececa",
             "metadata": {},
             "source": [
-                "## Step 4: calculate diversity\n",
-                "\n",
-                "Specifically, we estimate the _packing number_ of the route set,\n",
-                "i.e. the number of distinct routes which are greater than a distance $r$ away from each other.\n",
-                "Here we use a stringent form of diversity: routes which have no common reactions,\n",
-                "which means that their Jaccard distance is 1.\n",
-                "To do this, we use the `to_synthesis_graph` method of each graph object\n",
-                "which converts them into a common format."
+                "We can use visualization utilities to get a quick look at the routes found."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
-            "id": "bfdad9e4-1b92-4214-808e-7652a2e4cbea",
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "retro star: number of distinct routes = 2\n",
-                        "mcts: number of distinct routes = 4\n"
-                    ]
-                }
-            ],
+            "outputs": [],
+            "source": [
+                "from syntheseus.search.visualization import visualize_andor\n",
+                "\n",
+                "for idx, route in enumerate(routes):\n",
+                "    visualize_andor(\n",
+                "        output_graph, filename=f\"route_{idx + 1}.pdf\", nodes=route\n",
+                "    )"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
             "source": [
-                "from syntheseus.search.analysis import diversity\n",
-                "for alg_name, graph in alg_name_to_graph.items():\n",
-                "    route_objects = [graph.to_synthesis_graph(nodes) for nodes in alg_name_to_routes[alg_name]]\n",
-                "    packing_set = diversity.estimate_packing_number(\n",
-                "        routes=route_objects,\n",
-                "        distance_metric=diversity.reaction_jaccard_distance,\n",
-                "        radius=0.999  # because comparison is > not >=\n",
-                "    )\n",
-                "    print(f\"{alg_name}: number of distinct routes = {len(packing_set)}\")"
+                "The contents of the files `route_{1, 2}.pdf` should look roughly like the below.\n",
+                "\n",
+                "<img align=\"top\" src=\"https://github.com/microsoft/syntheseus/assets/61470923/f3d93324-9920-43b1-9d61-a4386e20a654\" width=\"320px\">\n",
+                "<img align=\"top\" src=\"https://github.com/microsoft/syntheseus/assets/61470923/e12489b4-e129-4d7e-822f-75da5aaf7af5\" width=\"320px\">"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "syntheseus-single-step",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.9.7"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 2
 }
```

