# Comparing `tmp/lambeq-0.4.0.tar.gz` & `tmp/lambeq-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambeq-0.4.0.tar", last modified: Thu Jan 11 15:17:28 2024, max compression
+gzip compressed data, was "lambeq-0.4.1.tar", last modified: Thu Apr 11 10:31:25 2024, max compression
```

## Comparing `lambeq-0.4.0.tar` & `lambeq-0.4.1.tar`

### file list

```diff
@@ -1,277 +1,280 @@
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.947606 lambeq-0.4.0/
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.905514 lambeq-0.4.0/.github/
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.909038 lambeq-0.4.0/.github/workflows/
--rwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)       42 2024-01-11 15:15:59.000000 lambeq-0.4.0/.github/workflows/build-docs
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4229 2024-01-11 15:15:59.000000 lambeq-0.4.0/.github/workflows/build_test.yml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)       22 2024-01-11 15:15:59.000000 lambeq-0.4.0/.github/workflows/clear-target-files
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1352 2024-01-11 15:15:59.000000 lambeq-0.4.0/.github/workflows/docs.yml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      368 2024-01-11 15:15:59.000000 lambeq-0.4.0/.gitignore
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    10173 2024-01-11 15:15:59.000000 lambeq-0.4.0/LICENSE
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5731 2024-01-11 15:17:28.947522 lambeq-0.4.0/PKG-INFO
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3795 2024-01-11 15:15:59.000000 lambeq-0.4.0/README.md
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.909177 lambeq-0.4.0/contrib/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      721 2024-01-11 15:15:59.000000 lambeq-0.4.0/contrib/download_depccg_model.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.914307 lambeq-0.4.0/docs/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5335 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/CONTRIBUTING.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      758 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/Makefile
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.905894 lambeq-0.4.0/docs/_static/
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.914499 lambeq-0.4.0/docs/_static/css/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      177 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/css/table-wrap.css
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.917013 lambeq-0.4.0/docs/_static/images/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    14749 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/CQ-logo.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    18245 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/Quantinuum_logo.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    46537 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/ccg-diagram.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   146116 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/ccgbank.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    35508 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/comm-diagram.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      456 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/favicon.ico
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3455 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/lambeq_logo.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   123764 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/linear.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    75455 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/pipeline.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    46789 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/pregroups.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4159 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/snake-2.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3372 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/snake.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    58067 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/string_diagram.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   305861 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/string_diagram_with_swaps.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    81612 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/_static/images/use_cases.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      438 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/advanced.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4969 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/bibliography.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15675 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/cli.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3459 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/conf.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.919555 lambeq-0.4.0/docs/examples/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    69889 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/circuit.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    74666 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/classical-pipeline.ipynb
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.920266 lambeq-0.4.0/docs/examples/datasets/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      953 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/datasets/mc_dev_data.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      903 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/datasets/mc_test_data.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2085 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/datasets/mc_train_data.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      946 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/datasets/rp_test_data.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2288 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/datasets/rp_train_data.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    20821 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/parser.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    94305 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/pennylane.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   172655 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/quantum-pipeline-jax.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   174159 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/quantum-pipeline.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    22899 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/reader.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   283289 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/rewrite.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   150421 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/rotosolve-optimizer.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    68555 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/tensor.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    79953 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/tokenisation.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    48398 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/tree-reader.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   123968 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/examples/unk-words.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      562 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/extract_code_cells.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)       12 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/genindex.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15849 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/glossary.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3849 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/index.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1044 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/installation.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      113 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.ansatz.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1035 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.backend.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      113 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.bobcat.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      154 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.rewrite.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      470 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.text2diagram.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      122 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.tokeniser.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      150 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/lambeq.training.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1765 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/manual-training.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    10192 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/models.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5932 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/nlp-class.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9485 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/nlp-data.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     6399 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/nlp-intro.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3980 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/nlp-ml.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2293 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/nlp-refs.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      498 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/notebooks.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     6287 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/package-api.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3562 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/parsing.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2389 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/pipeline.rst
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.921824 lambeq-0.4.0/docs/puml/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      609 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/README.md
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1523 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/ansatz.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1428 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/backend-inheritance.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1576 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/backend-quantum-inheritance.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2578 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/backend.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      644 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/bobcat.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      611 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/legend.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      289 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/pregroups.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1720 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/rewrite.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2552 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/text2diagram.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      468 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/tokeniser.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2499 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/puml/training.puml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    21406 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/release-notes.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      134 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/requirements.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      242 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/root-api.rst
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.922373 lambeq-0.4.0/docs/scripts/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      508 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/scripts/check_errors.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3440 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/scripts/clean_notebooks.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3226 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/scripts/compare_execution_times.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5404 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/scripts/track_execution_time.sh
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4443 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/string-diagrams.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3791 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/training.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1547 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/troubleshooting.rst
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.924783 lambeq-0.4.0/docs/tutorials/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   219824 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/discocat.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   190360 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/extend-lambeq.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    70468 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/monoidal.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   250274 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/parameterise.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   133806 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/rewrite.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   184697 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/sentence-input.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   143016 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/trainer-classical.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   156804 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/trainer-hybrid.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   246192 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/trainer-quantum.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)   145991 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/training-symbols.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    51122 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/tutorials/training-usecase.ipynb
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1821 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/uml-diagrams.rst
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    13492 2024-01-11 15:15:59.000000 lambeq-0.4.0/docs/use-cases.rst
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.925481 lambeq-0.4.0/lambeq/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4278 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/__init__.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.926911 lambeq-0.4.0/lambeq/ansatz/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1097 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/ansatz/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3831 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/ansatz/base.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    14931 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/ansatz/circuit.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7735 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/ansatz/tensor.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.928079 lambeq-0.4.0/lambeq/backend/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1092 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/__init__.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.928560 lambeq-0.4.0/lambeq/backend/converters/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      242 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/converters/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    17681 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/converters/discopy.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    17315 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/converters/tk.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.929824 lambeq-0.4.0/lambeq/backend/drawing/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      443 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    19934 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/drawable.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    23898 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/drawing.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4176 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/drawing_backend.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1236 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/helpers.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4955 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/mat_backend.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9266 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/text_printer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     8054 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/drawing/tikz_backend.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    62191 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/grammar.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3293 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/numerical_backend.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    16713 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/pennylane.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    33699 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/quantum.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    11119 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/snake_removal.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    16652 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/backend/tensor.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.931043 lambeq-0.4.0/lambeq/bobcat/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      999 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2826 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/fast_int_enum.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4310 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/grammar.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9887 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/lexicon.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    17742 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    18534 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/rules.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15875 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/tagger.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    13094 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/bobcat/tree.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    27513 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/cli.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.931579 lambeq-0.4.0/lambeq/core/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/core/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1513 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/core/globals.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1197 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/core/types.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1965 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/core/utils.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.931960 lambeq-0.4.0/lambeq/rewrite/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1392 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/rewrite/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    16826 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/rewrite/base.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15826 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/rewrite/rewrite_diagram.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.934546 lambeq-0.4.0/lambeq/text2diagram/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2228 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2711 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/base.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    14315 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/bobcat_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9632 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/ccg_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15560 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/ccg_rule.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    20059 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/ccg_tree.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    18330 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/ccg_type.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    16572 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/ccgbank_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    19303 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/depccg_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4083 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/linear_reader.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9265 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/model_downloader.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1849 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/spiders_reader.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     8197 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/tree_reader.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     6084 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/text2diagram/web_parser.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.935069 lambeq-0.4.0/lambeq/tokeniser/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      749 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/tokeniser/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2002 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/tokeniser/base.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2777 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/tokeniser/spacy_tokeniser.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.937995 lambeq-0.4.0/lambeq/training/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2137 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3699 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/checkpoint.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4194 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/dataset.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7081 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/loss.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5590 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    15078 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/nelder_mead_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5594 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/numpy_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3321 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9217 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/pennylane_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5490 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/pytorch_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7384 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/pytorch_trainer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5811 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/quantum_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7233 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/quantum_trainer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4389 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/rotosolve_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7536 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/spsa_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4374 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/tket_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    23977 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/training/trainer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      749 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/typing.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      411 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq/version.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)       86 2024-01-11 15:15:59.000000 lambeq-0.4.0/lambeq/version.pyi
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.946691 lambeq-0.4.0/lambeq.egg-info/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5731 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/PKG-INFO
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7263 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        1 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)       43 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/entry_points.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      273 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/requires.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        7 2024-01-11 15:17:28.000000 lambeq-0.4.0/lambeq.egg-info/top_level.txt
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      937 2024-01-11 15:15:59.000000 lambeq-0.4.0/pyproject.toml
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2086 2024-01-11 15:17:28.948011 lambeq-0.4.0/setup.cfg
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.939836 lambeq-0.4.0/tests/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/__init__.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.941178 lambeq-0.4.0/tests/backend/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/__init__.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.941472 lambeq-0.4.0/tests/backend/converters/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/__init__.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.942050 lambeq-0.4.0/tests/backend/converters/discopy/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/discopy/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2851 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/discopy/test_grammar_conversion.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3010 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/discopy/test_quantum_conversion.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1590 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/discopy/test_tensor_conversion.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3480 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/converters/test_tket_conversion.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    35101 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_circuit_drawing.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    40664 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_drawing.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    11150 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_grammar.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9481 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_pennylane_interface.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4164 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_quantum.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4039 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_rewriting.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2568 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/backend/test_tensor.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.942571 lambeq-0.4.0/tests/src/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9963 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/src/alice-loves-bob.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2650 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/src/alice-loves-bob.tikz
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    20852 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/src/gave-up.png
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      144 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_bobcat.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9703 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_circuit.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    25088 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_cli.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1887 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_pregroups.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    16719 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_rewrite.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      322 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_symbol.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2547 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_tensor.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     7590 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_text_printer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1795 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_tokeniser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      879 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/test_utils.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.944252 lambeq-0.4.0/tests/text2diagram/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5661 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_bobcat_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      705 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_ccg_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    10335 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_ccg_rule.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)    12417 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_ccg_tree.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      514 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_ccg_type.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     6543 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_ccgbank_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5802 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_depccg_parser.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3521 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_model_download.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4123 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_reader.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2803 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/text2diagram/test_web_parser.py
-drwxr-xr-x   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:17:28.946456 lambeq-0.4.0/tests/training/
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)        0 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/__init__.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     2155 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_chckpoint.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1369 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_dataset.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3498 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_loss.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1488 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5468 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_nelder_mead_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5732 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_numpy_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     9505 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_pennylane_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4687 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_pytorch_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4923 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_pytorch_trainer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     4096 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_quantum_trainer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     1716 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_rotosolve_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     5500 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_spsa_optimizer.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)     3700 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_tket_model.py
--rw-r--r--   0 thomas.hoffmann   (501) staff       (20)      972 2024-01-11 15:15:59.000000 lambeq-0.4.0/tests/training/test_trainer.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.282185 lambeq-0.4.1/
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.186423 lambeq-0.4.1/.github/
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.190437 lambeq-0.4.1/.github/workflows/
+-rwxr-xr-x   0 nikhilkhatri   (502) staff       (20)       42 2024-04-11 10:30:56.000000 lambeq-0.4.1/.github/workflows/build-docs
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4515 2024-04-11 10:30:56.000000 lambeq-0.4.1/.github/workflows/build_test.yml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)       22 2024-04-11 10:30:56.000000 lambeq-0.4.1/.github/workflows/clear-target-files
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1352 2024-04-11 10:30:56.000000 lambeq-0.4.1/.github/workflows/docs.yml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      368 2024-04-11 10:30:56.000000 lambeq-0.4.1/.gitignore
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    10173 2024-04-11 10:30:56.000000 lambeq-0.4.1/LICENSE
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5807 2024-04-11 10:31:25.282109 lambeq-0.4.1/PKG-INFO
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3795 2024-04-11 10:30:56.000000 lambeq-0.4.1/README.md
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.190899 lambeq-0.4.1/contrib/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2349 2024-04-11 10:30:56.000000 lambeq-0.4.1/contrib/convert_discopy_to_lambeq.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      721 2024-04-11 10:30:56.000000 lambeq-0.4.1/contrib/download_depccg_model.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.200935 lambeq-0.4.1/docs/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5335 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/CONTRIBUTING.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      758 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/Makefile
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.186789 lambeq-0.4.1/docs/_static/
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.201246 lambeq-0.4.1/docs/_static/css/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      177 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/css/table-wrap.css
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.209484 lambeq-0.4.1/docs/_static/images/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    14749 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/CQ-logo.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    18245 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/Quantinuum_logo.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    46537 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/ccg-diagram.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   146116 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/ccgbank.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    35508 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/comm-diagram.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      456 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/favicon.ico
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3455 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/lambeq_logo.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   123764 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/linear.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    75455 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/pipeline.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    46789 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/pregroups.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4159 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/snake-2.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3372 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/snake.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    58067 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/string_diagram.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   305861 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/string_diagram_with_swaps.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    81612 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/_static/images/use_cases.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      438 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/advanced.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4969 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/bibliography.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15675 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/cli.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3459 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/conf.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.220271 lambeq-0.4.1/docs/examples/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    69889 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/circuit.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    74666 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/classical-pipeline.ipynb
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.222378 lambeq-0.4.1/docs/examples/datasets/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      953 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/datasets/mc_dev_data.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      903 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/datasets/mc_test_data.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2085 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/datasets/mc_train_data.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      946 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/datasets/rp_test_data.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2288 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/datasets/rp_train_data.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    20821 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/parser.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    94305 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/pennylane.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   172655 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/quantum-pipeline-jax.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   174159 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/quantum-pipeline.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    22899 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/reader.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   283289 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/rewrite.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   150421 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/rotosolve-optimizer.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    68555 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/tensor.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    79953 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/tokenisation.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    48398 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/tree-reader.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   123968 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/examples/unk-words.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      562 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/extract_code_cells.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)       12 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/genindex.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15849 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/glossary.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3849 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/index.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1044 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/installation.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      113 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.ansatz.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1035 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.backend.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      113 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.bobcat.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      154 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.rewrite.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      470 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.text2diagram.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      122 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.tokeniser.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      150 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/lambeq.training.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1765 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/manual-training.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    10192 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/models.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5932 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/nlp-class.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9485 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/nlp-data.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6399 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/nlp-intro.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3980 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/nlp-ml.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2293 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/nlp-refs.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      498 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/notebooks.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6316 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/package-api.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3562 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/parsing.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2389 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/pipeline.rst
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.225745 lambeq-0.4.1/docs/puml/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      609 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/README.md
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1573 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/ansatz.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1428 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/backend-inheritance.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1576 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/backend-quantum-inheritance.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2578 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/backend.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      644 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/bobcat.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      611 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/legend.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      289 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/pregroups.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1720 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/rewrite.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2552 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/text2diagram.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      468 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/tokeniser.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2499 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/puml/training.puml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    22551 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/release-notes.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      134 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/requirements.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      242 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/root-api.rst
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.226451 lambeq-0.4.1/docs/scripts/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      508 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/scripts/check_errors.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3440 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/scripts/clean_notebooks.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3226 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/scripts/compare_execution_times.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5404 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/scripts/track_execution_time.sh
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4443 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/string-diagrams.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3791 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/training.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1547 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/troubleshooting.rst
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.236310 lambeq-0.4.1/docs/tutorials/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      116 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/config.toml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   219824 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/discocat.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   190360 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/extend-lambeq.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    70468 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/monoidal.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   250431 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/parameterise.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   133806 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/rewrite.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   184697 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/sentence-input.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   143016 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/trainer-classical.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   156804 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/trainer-hybrid.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   232263 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/trainer-quantum.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)   145991 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/training-symbols.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    51122 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/tutorials/training-usecase.ipynb
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1821 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/uml-diagrams.rst
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    13492 2024-04-11 10:30:56.000000 lambeq-0.4.1/docs/use-cases.rst
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.237923 lambeq-0.4.1/lambeq/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4228 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/__init__.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.241959 lambeq-0.4.1/lambeq/ansatz/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1123 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/ansatz/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3831 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/ansatz/base.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    17403 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/ansatz/circuit.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7735 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/ansatz/tensor.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.244788 lambeq-0.4.1/lambeq/backend/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1092 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/__init__.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.245606 lambeq-0.4.1/lambeq/backend/converters/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      242 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/converters/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    18705 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/converters/discopy.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    17315 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/converters/tk.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.248036 lambeq-0.4.1/lambeq/backend/drawing/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      479 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    19934 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/drawable.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    25590 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/drawing.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4176 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/drawing_backend.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1236 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/helpers.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4955 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/mat_backend.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     8489 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/text_printer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     8054 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/drawing/tikz_backend.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    63188 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/grammar.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3293 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/numerical_backend.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    16713 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/pennylane.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    33785 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/quantum.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    11119 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/snake_removal.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    16652 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/backend/tensor.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.251815 lambeq-0.4.1/lambeq/bobcat/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      999 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2826 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/fast_int_enum.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4310 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/grammar.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9887 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/lexicon.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    17742 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    18534 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/rules.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15875 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/tagger.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    13094 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/bobcat/tree.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    27445 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/cli.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.252601 lambeq-0.4.1/lambeq/core/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/core/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1514 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/core/globals.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1197 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/core/types.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1965 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/core/utils.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.253658 lambeq-0.4.1/lambeq/rewrite/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1392 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/rewrite/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    16826 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/rewrite/base.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15600 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/rewrite/rewrite_diagram.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.257296 lambeq-0.4.1/lambeq/text2diagram/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2228 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2711 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/base.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    14389 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/bobcat_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    10604 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/ccg_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15560 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/ccg_rule.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    20766 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/ccg_tree.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    18816 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/ccg_type.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    16634 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/ccgbank_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    19833 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/depccg_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4083 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/linear_reader.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9313 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/model_downloader.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1849 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/spiders_reader.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     8595 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/tree_reader.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6084 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/text2diagram/web_parser.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.257984 lambeq-0.4.1/lambeq/tokeniser/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      749 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/tokeniser/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2002 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/tokeniser/base.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2777 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/tokeniser/spacy_tokeniser.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.263928 lambeq-0.4.1/lambeq/training/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2137 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3699 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/checkpoint.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4194 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/dataset.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7081 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/loss.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5590 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    15078 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/nelder_mead_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5594 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/numpy_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3321 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9217 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/pennylane_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5490 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/pytorch_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7384 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/pytorch_trainer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5811 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/quantum_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7421 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/quantum_trainer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4389 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/rotosolve_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7536 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/spsa_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4417 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/tket_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    27335 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/training/trainer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      749 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/typing.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      411 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq/version.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)       86 2024-04-11 10:30:56.000000 lambeq-0.4.1/lambeq/version.pyi
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.281014 lambeq-0.4.1/lambeq.egg-info/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5807 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7388 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        1 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)       43 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      283 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/requires.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        7 2024-04-11 10:31:25.000000 lambeq-0.4.1/lambeq.egg-info/top_level.txt
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      937 2024-04-11 10:30:56.000000 lambeq-0.4.1/pyproject.toml
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2137 2024-04-11 10:31:25.282620 lambeq-0.4.1/setup.cfg
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.270850 lambeq-0.4.1/tests/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/__init__.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.273386 lambeq-0.4.1/tests/backend/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/__init__.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.273745 lambeq-0.4.1/tests/backend/converters/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/__init__.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.274483 lambeq-0.4.1/tests/backend/converters/discopy/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/discopy/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2851 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/discopy/test_grammar_conversion.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1605 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/discopy/test_old_discopy.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3010 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/discopy/test_quantum_conversion.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1590 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/discopy/test_tensor_conversion.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3480 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/converters/test_tket_conversion.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    35101 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_circuit_drawing.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    40664 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_drawing.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    11150 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_grammar.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9481 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_pennylane_interface.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4164 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_quantum.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4039 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_rewriting.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2568 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_tensor.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     7951 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/backend/test_text_printer.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.275043 lambeq-0.4.1/tests/src/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9963 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/src/alice-loves-bob.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2650 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/src/alice-loves-bob.tikz
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    20852 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/src/gave-up.png
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      144 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_bobcat.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    11076 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_circuit.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    25088 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_cli.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1887 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_pregroups.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    16719 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_rewrite.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      322 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_symbol.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2547 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_tensor.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1795 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_tokeniser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      879 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/test_utils.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.277736 lambeq-0.4.1/tests/text2diagram/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5668 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_bobcat_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      705 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_ccg_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    10335 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_ccg_rule.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)    12417 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_ccg_tree.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      514 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_ccg_type.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6543 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_ccgbank_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5802 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_depccg_parser.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3521 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_model_download.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4317 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_reader.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2803 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/text2diagram/test_web_parser.py
+drwxr-xr-x   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:31:25.280785 lambeq-0.4.1/tests/training/
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)        0 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/__init__.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     2155 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_chckpoint.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1369 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_dataset.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3498 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_loss.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1488 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5468 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_nelder_mead_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6208 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_numpy_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     9505 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_pennylane_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4687 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_pytorch_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     6977 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_pytorch_trainer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     4096 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_quantum_trainer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     1716 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_rotosolve_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     5500 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_spsa_optimizer.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)     3700 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_tket_model.py
+-rw-r--r--   0 nikhilkhatri   (502) staff       (20)      972 2024-04-11 10:30:56.000000 lambeq-0.4.1/tests/training/test_trainer.py
```

### Comparing `lambeq-0.4.0/.github/workflows/build_test.yml` & `lambeq-0.4.1/.github/workflows/build_test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   DOCS_DIR: docs
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ 3.9, "3.10", "3.11" ]
+        python-version: [ 3.9, "3.10", "3.11", "3.12" ]
     outputs:
       error-check: ${{ steps.error-check.conclusion }}
     steps:
     - uses: actions/checkout@v3
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
@@ -45,25 +45,29 @@
         flake8 ${{ env.SRC_DIR }} --count --exit-zero --isolated --max-complexity=10 --max-doc-length=72 --select=C901,W505 --statistics
   build_and_test:
     needs: lint
     if: ${{ always() && needs.lint.outputs.error-check == 'success' }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ 3.9, "3.10", "3.11" ]
+        python-version: [ 3.9, "3.10", "3.11", "3.12" ]
     steps:
     - uses: actions/checkout@v3
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install base package
       run: pip install .
     - name: Check package import works
       run: python -c 'import lambeq'
+    - name: Install downgraded Qiskit (for compatibility reasons)
+      # This should be removed once the following PR is merged:
+      # https://github.com/PennyLaneAI/pennylane-qiskit/pull/493
+      run: pip install 'qiskit<1' pytket-qiskit qiskit-ibm-runtime
     - name: Install extra dependencies and tester
       run: pip install .[extras] .[test]
     - name: Locate bobcat pre-trained model cache
       id: loc-bobcat-cache
       run: echo "dir=$(python -c 'from lambeq.text2diagram.model_downloader import ModelDownloader; print(ModelDownloader("bert").model_dir)')" >> $GITHUB_OUTPUT
     - name: Restore bobcat pre-trained model from cache
       id: bobcat-cache
@@ -98,15 +102,15 @@
       run: coverage report -m
   type_check:
     needs: lint
     if: ${{ always() && needs.lint.outputs.error-check == 'success' }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ 3.9, "3.10", "3.11" ]
+        python-version: [ 3.9, "3.10", "3.11", "3.12" ]
     steps:
     - uses: actions/checkout@v3
     - name: Setup Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies with type hints
```

### Comparing `lambeq-0.4.0/.github/workflows/docs.yml` & `lambeq-0.4.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/LICENSE` & `lambeq-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/PKG-INFO` & `lambeq-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambeq
-Version: 0.4.0
+Version: 0.4.1
 Summary: A QNLP toolkit
 Home-page: https://cqcl.github.io/lambeq
 Download-URL: https://pypi.org/project/lambeq
 Author: Cambridge Quantum QNLP team
 Author-email: lambeq-support@cambridgequantum.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/CQCL/lambeq
@@ -15,27 +15,29 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: packaging
 Requires-Dist: pillow>=6.2.1
 Requires-Dist: pytket>=0.19.2
 Requires-Dist: pyyaml
 Requires-Dist: spacy>=3.0
 Requires-Dist: tensornetwork
 Requires-Dist: torch>=1.12.1
 Requires-Dist: transformers
 Provides-Extra: extras
-Requires-Dist: discopy==1.1.4; extra == "extras"
+Requires-Dist: discopy>=1.1.7; extra == "extras"
 Requires-Dist: jax; extra == "extras"
 Requires-Dist: jaxlib; extra == "extras"
 Requires-Dist: pennylane>=0.29.1; extra == "extras"
 Requires-Dist: pennylane-honeywell; extra == "extras"
 Requires-Dist: pennylane-qiskit; extra == "extras"
 Requires-Dist: pytket-qiskit>=0.21.0; extra == "extras"
 Requires-Dist: tensorboard>=2.7.0; extra == "extras"
```

### Comparing `lambeq-0.4.0/README.md` & `lambeq-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/contrib/download_depccg_model.py` & `lambeq-0.4.1/contrib/download_depccg_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/CONTRIBUTING.rst` & `lambeq-0.4.1/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/Makefile` & `lambeq-0.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/CQ-logo.png` & `lambeq-0.4.1/docs/_static/images/CQ-logo.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/Quantinuum_logo.png` & `lambeq-0.4.1/docs/_static/images/Quantinuum_logo.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/ccg-diagram.png` & `lambeq-0.4.1/docs/_static/images/ccg-diagram.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/ccgbank.png` & `lambeq-0.4.1/docs/_static/images/ccgbank.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/comm-diagram.png` & `lambeq-0.4.1/docs/_static/images/comm-diagram.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/lambeq_logo.png` & `lambeq-0.4.1/docs/_static/images/lambeq_logo.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/linear.png` & `lambeq-0.4.1/docs/_static/images/linear.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/pipeline.png` & `lambeq-0.4.1/docs/_static/images/pipeline.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/pregroups.png` & `lambeq-0.4.1/docs/_static/images/pregroups.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/snake-2.png` & `lambeq-0.4.1/docs/_static/images/snake-2.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/snake.png` & `lambeq-0.4.1/docs/_static/images/snake.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/string_diagram.png` & `lambeq-0.4.1/docs/_static/images/string_diagram.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/string_diagram_with_swaps.png` & `lambeq-0.4.1/docs/_static/images/string_diagram_with_swaps.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/_static/images/use_cases.png` & `lambeq-0.4.1/docs/_static/images/use_cases.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/bibliography.rst` & `lambeq-0.4.1/docs/bibliography.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/cli.rst` & `lambeq-0.4.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/conf.py` & `lambeq-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/circuit.ipynb` & `lambeq-0.4.1/docs/examples/circuit.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/classical-pipeline.ipynb` & `lambeq-0.4.1/docs/examples/classical-pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/datasets/mc_dev_data.txt` & `lambeq-0.4.1/docs/examples/datasets/mc_dev_data.txt`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/datasets/mc_test_data.txt` & `lambeq-0.4.1/docs/examples/datasets/mc_test_data.txt`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/datasets/mc_train_data.txt` & `lambeq-0.4.1/docs/examples/datasets/mc_train_data.txt`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/datasets/rp_test_data.txt` & `lambeq-0.4.1/docs/examples/datasets/rp_test_data.txt`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/datasets/rp_train_data.txt` & `lambeq-0.4.1/docs/examples/datasets/rp_train_data.txt`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/parser.ipynb` & `lambeq-0.4.1/docs/examples/parser.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/pennylane.ipynb` & `lambeq-0.4.1/docs/examples/pennylane.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/quantum-pipeline-jax.ipynb` & `lambeq-0.4.1/docs/examples/quantum-pipeline-jax.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/quantum-pipeline.ipynb` & `lambeq-0.4.1/docs/examples/quantum-pipeline.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/reader.ipynb` & `lambeq-0.4.1/docs/examples/reader.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/rewrite.ipynb` & `lambeq-0.4.1/docs/examples/rewrite.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/rotosolve-optimizer.ipynb` & `lambeq-0.4.1/docs/examples/rotosolve-optimizer.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/tensor.ipynb` & `lambeq-0.4.1/docs/examples/tensor.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/tokenisation.ipynb` & `lambeq-0.4.1/docs/examples/tokenisation.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/tree-reader.ipynb` & `lambeq-0.4.1/docs/examples/tree-reader.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/examples/unk-words.ipynb` & `lambeq-0.4.1/docs/examples/unk-words.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/extract_code_cells.py` & `lambeq-0.4.1/docs/extract_code_cells.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/glossary.rst` & `lambeq-0.4.1/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/index.rst` & `lambeq-0.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/installation.rst` & `lambeq-0.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/lambeq.backend.rst` & `lambeq-0.4.1/docs/lambeq.backend.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/manual-training.rst` & `lambeq-0.4.1/docs/manual-training.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/models.rst` & `lambeq-0.4.1/docs/models.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/nlp-class.rst` & `lambeq-0.4.1/docs/nlp-class.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/nlp-data.rst` & `lambeq-0.4.1/docs/nlp-data.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/nlp-intro.rst` & `lambeq-0.4.1/docs/nlp-intro.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/nlp-ml.rst` & `lambeq-0.4.1/docs/nlp-ml.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/nlp-refs.rst` & `lambeq-0.4.1/docs/nlp-refs.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/package-api.rst` & `lambeq-0.4.1/docs/package-api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .. rubric:: Classes:
 
 .. inheritance-diagram::
     lambeq.ansatz.IQPAnsatz
     lambeq.ansatz.MPSAnsatz
     lambeq.ansatz.Sim14Ansatz
     lambeq.ansatz.Sim15Ansatz
+    lambeq.ansatz.Sim4Ansatz
     lambeq.ansatz.SpiderAnsatz
     lambeq.ansatz.StronglyEntanglingAnsatz
     lambeq.ansatz.Symbol
    :top-classes: lambeq.ansatz.base.Symbol
    :parts: 1
 
 |
```

### Comparing `lambeq-0.4.0/docs/parsing.rst` & `lambeq-0.4.1/docs/parsing.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/pipeline.rst` & `lambeq-0.4.1/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/README.md` & `lambeq-0.4.1/docs/puml/README.md`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/ansatz.puml` & `lambeq-0.4.1/docs/puml/ansatz.puml`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     tensor_functor
 }
 
 class IQPAnsatz {}
 class StronglyEntanglingAnsatz {}
 class Sim14Ansatz {}
 class Sim15Ansatz {}
+class Sim4Ansatz {}
 
 class Symbol {
     size: int
     sort_key(order)
 }
 class sympy.core.symbol.Symbol #back:wheat;line:tomato {}
 
@@ -51,14 +52,15 @@
 BaseAnsatz <|-- CircuitAnsatz
 TensorAnsatz <|-- MPSAnsatz
 TensorAnsatz <|-- SpiderAnsatz
 CircuitAnsatz <|-- IQPAnsatz
 CircuitAnsatz <|-- StronglyEntanglingAnsatz
 CircuitAnsatz <|-- Sim14Ansatz
 CircuitAnsatz <|-- Sim15Ansatz
+CircuitAnsatz <|-- Sim4Ansatz
 
 MPSAnsatz::split_functor *-left- backend.grammar.Functor
 MPSAnsatz::tensor_functor *-- backend.grammar.Functor
 SpiderAnsatz::split_functor *-- backend.grammar.Functor
 SpiderAnsatz::tensor_functor *-- backend.grammar.Functor
 MPSAnsatz::BOND_TYPE *--left backend.grammar.Ty
 CircuitAnsatz::functor *-- backend.grammar.Functor
```

### Comparing `lambeq-0.4.0/docs/puml/backend-inheritance.puml` & `lambeq-0.4.1/docs/puml/backend-inheritance.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/backend-quantum-inheritance.puml` & `lambeq-0.4.1/docs/puml/backend-quantum-inheritance.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/backend.puml` & `lambeq-0.4.1/docs/puml/backend.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/bobcat.puml` & `lambeq-0.4.1/docs/puml/bobcat.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/legend.puml` & `lambeq-0.4.1/docs/puml/legend.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/rewrite.puml` & `lambeq-0.4.1/docs/puml/rewrite.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/text2diagram.puml` & `lambeq-0.4.1/docs/puml/text2diagram.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/puml/training.puml` & `lambeq-0.4.1/docs/puml/training.puml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/release-notes.rst` & `lambeq-0.4.1/docs/release-notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,35 @@
 .. _sec-release-notes:
 
 Release notes
 =============
 
+.. _rel-0.4.1:
+
+`0.4.1 <https://github.com/CQCL/lambeq/releases/tag/0.4.1>`_
+------------------------------------------------------------
+
+Added:
+
+- Support for Python 3.12.
+- A new :py:class:`~lambeq.Sim4Ansatz` based on the Sim `et al.` paper [SJA2019]_.
+- A new argument in :py:meth:`.Trainer.fit` for specifying an :py:attr:`early_stopping_criterion` other than validation loss.
+- A new argument :py:attr:`collapse_noun_phrases` in methods of :py:class:`.CCGParser` and :py:class:`.CCGTree` classes (for example, see :py:meth:`.CCGParser.sentence2diagram`) that allows the user to maintain noun phrases in the derivation or collapse them into nouns as desired.
+- Raised meaningful exception when users try to convert to/from DisCoPy 1.1.0
+
+Changed:
+
+- An internal refactoring of module :py:mod:`.backend.drawing` in view of planned new features.
+- Updated random number generation in :py:class:`~lambeq.TketModel` by using the recommended :py:meth:`numpy.random.default_rnd` method.
+
+Fixed:
+
+- Handling of possible empty ``Bra`` s and ``Ket`` s during conversion from DisCoPy.
+- Fixed a bug in JIT compilation of mixed circuit evaluations.
+
 .. _rel-0.4.0:
 
 `0.4.0 <https://github.com/CQCL/lambeq/releases/tag/0.4.0>`_
 ------------------------------------------------------------
 
 Added:
```

### Comparing `lambeq-0.4.0/docs/scripts/clean_notebooks.py` & `lambeq-0.4.1/docs/scripts/clean_notebooks.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/scripts/compare_execution_times.py` & `lambeq-0.4.1/docs/scripts/compare_execution_times.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/scripts/track_execution_time.sh` & `lambeq-0.4.1/docs/scripts/track_execution_time.sh`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/string-diagrams.rst` & `lambeq-0.4.1/docs/string-diagrams.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/training.rst` & `lambeq-0.4.1/docs/training.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/troubleshooting.rst` & `lambeq-0.4.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/discocat.ipynb` & `lambeq-0.4.1/docs/tutorials/discocat.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/extend-lambeq.ipynb` & `lambeq-0.4.1/docs/tutorials/extend-lambeq.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/monoidal.ipynb` & `lambeq-0.4.1/docs/tutorials/monoidal.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/parameterise.ipynb` & `lambeq-0.4.1/docs/tutorials/parameterise.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999245169082125%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(10, \'   ":py:class:`~.Sim4Ansatz`", "Circuit 4 from '*

 * *            '[SJA2019]_. Uses a layer each of Rx and Rz gates, followed by a ladder of CRx gates '*

 * *            'per layer. "\\n\')]}}}'}*

```diff
@@ -37,14 +37,15 @@
                 ".. csv-table::\n",
                 "   :header: \"Ansatz\", \"Description\"\n",
                 "   :widths: 20, 60\n",
                 "\n",
                 "   \":py:class:`~.IQPAnsatz`\", \"Instantaneous Quantum Polynomial ansatz. An IQP ansatz interleaves layers of Hadamard gates with diagonal unitaries. This class uses ``n_layers-1`` adjacent CRz gates to implement each diagonal unitary (see [Hea2019]_)\"\n",
                 "   \":py:class:`~.Sim14Ansatz`\", \"A modification of Circuit 14 from [SJA2019]_. Replaces circuit-block construction with two rings of CRx gates, in opposite orientation.\"\n",
                 "   \":py:class:`~.Sim15Ansatz`\", \"A modification of Circuit 15 from [SJA2019]_. Replaces circuit-block construction with two rings of CNOT gates, in opposite orientation.\"\n",
+                "   \":py:class:`~.Sim4Ansatz`\", \"Circuit 4 from [SJA2019]_. Uses a layer each of Rx and Rz gates, followed by a ladder of CRx gates per layer. \"\n",
                 "   \":py:class:`~.StronglyEntanglingAnsatz`\", \"Ansatz using three single qubit rotations (RzRyRz) followed by a ladder of CNOT gates with different ranges per layer. Adapted from the :term:`PennyLane` implementation of :py:mod:`StronglyEntanglingLayers`.\""
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "raw_mimetype": "text/restructuredtext"
```

### Comparing `lambeq-0.4.0/docs/tutorials/rewrite.ipynb` & `lambeq-0.4.1/docs/tutorials/rewrite.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/sentence-input.ipynb` & `lambeq-0.4.1/docs/tutorials/sentence-input.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/trainer-classical.ipynb` & `lambeq-0.4.1/docs/tutorials/trainer-classical.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/trainer-hybrid.ipynb` & `lambeq-0.4.1/docs/tutorials/trainer-hybrid.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/trainer-quantum.ipynb` & `lambeq-0.4.1/docs/tutorials/trainer-quantum.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989816196812308%*

 * *Differences: {"'cells'": "{19: {'outputs': {0: {'data': {'image/png': "*

 * *            "'iVBORw0KGgoAAAANSUhEUgAAA5cAAAIHCAYAAAALhKgSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAABAyElEQVR4nO3deViU9f7/8dewCir7rrniAqi5pOZR01zzGGWWmmVqrh2zsvXbqng87SdbPLmklnayMstKtCjtmFlZWtpuaa4VKqIibiAw9+8PL+bnCCj6Qe+BeT6ui0u4GYb3ONzzmeesDsuyLAEAAAAAYMDH7gEAAAAAAJUfcQkAAAAAMEZcAgAAAACMEZcAAAAAAGPEJQAAAADAGHEJAAAAADBGXAIAAAAAjBGXAAAAAABjxCUAAAAAwBhxCQAAAAAwRlwCAAAAAIw […]*

```diff
@@ -267,15 +267,15 @@
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5cAAAIHCAYAAAALhKgSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAABAyElEQVR4nO3deViU9f7/8dewCir7rrniAqi5pOZR01zzGGWWmmVqrh2zsvXbqng87SdbPLmklnayMstKtCjtmFlZWtpuaa4VKqIibiAw9+8PL+bnCCj6Qe+BeT6ui0u4GYb3ONzzmeesDsuyLAEAAAAAYMDH7gEAAAAAAJUfcQkAAAAAMEZcAgAAAACMEZcAAAAAAGPEJQAAAADAGHEJAAAAADBGXAIAAAAAjBGXAAAAAABjxCUAAAAAwBhxCQAAAAAwRlwCAAAAAIwRlwAAAAAAY8QlAAAAAMAYcQkAAAAAMEZcAgAAAACMEZcAAAAAAGPEJQAAAADAGHEJAAAAADBGXAIAAAAAjBGXAAAAAABjxCUAAAAAwBhxCQAAAAAwRlwCAAAAAIwRlwAAAAAAY8QlAAAAAMAYcQkAAAAAMEZcAgAAAACMEZcAAAAAAGPEJQAAAADAGHEJAAAAADBGXAIAAAAAjBGXAAAAAABjxCUAAAAAwBhxCQAAAAAwRlwCAAAAAIwRlwAAAAAAY8QlAAAAAMAYcQkAAAAAMEZcAgAAAACMEZcAAAAAAGPEJQAAAADAGHEJAAAAADBGXAIAAAAAjBGXAAAAAABjxCUAAAAAwBhxCQAAAAAwRlwCAAAAAIwRlwAAAAAAY8QlAAAAAMCYn90DVKSdO3cqOzvb7jFKFRUVpTp16tg9xnnnyecBAHgKb1kTJM9eF7zlfPDk8wDACVXl8qjKxOXOnTuVlJSko0eP2j1KqYKDg7Vx48Yq8UdTFk8/DwDAU3jDmiB5/rrgDeeDp58HAE6oKpdHVSYus7OzdfToUb322mtKSkqyexw3Gzdu1JAhQ5SdnV3p/2BOx5PPAwDwFN6yJkievS54y/ngyecBgBOq0uVRlYnLYklJSWrdurXdY3g1zgMAwMlYF+zHeQDgQuAFfQAAAAAAxohLAAAAAIAx4hIAAAAAYIy4BAAAAAAYIy4BAAAAAMaISwAAAACAMeISAAAAAGCMuAQAAAAAGCMuAQAAAADGiEsAAAAAgDHiEgAAAABgjLgEAAAAABgjLgEAAAAAxojLU6SlpcnhcHjN7wUqO4fDofHjx9s9BoDTWLJkiRwOh7755hu7R3EZM2aM3SMA56xevXq68sorz3i4Tz/9VA6HQ59++qlr2/Dhw1WvXr2z+n3z5s3zuH0Ynom4vICOHTumtLQ0tx0cQPl8+eWXSktLU05Oznn9Pb/88ovS0tK0ffv28/p7AADe6UKtZ4AdiMtTPPzwwzp27Nh5Oe68vDxNnjy51Lg8n78XqAq+/PJLTZ48+YLE5eTJk4lLAMB5caHWs7LMnj1bv/32my2/G1WfR8XlkSNH7B5Bfn5+qlatmtf8XgAAqgpPuB4BeDp/f38FBgbaPQaqqPMWlxs2bFCfPn0UEhKiGjVqqHv37vrqq69c3y9+7PaqVas0btw4xcTEqHbt2q7vv/jii2rQoIGCgoLUrl07rV69Wl27dlXXrl1dhzl+/LgmTpyoNm3a6LLLLpMkjRw5UitXrnSbZfv27XI4HPr3v/+tl156SQ0bNlRgYKDatm2rdevWuR321Oc+Dh8+XA6Ho9SPtLS0EnOEhoaqevXq6ty5c4k5evToIUmaPHlyieMo7TmXhYWFmjJlimveevXq6cEHH1R+fr7b4Yofd//555+rXbt2qlatmho0aKBXX331TGcTUCmkpaXp3nvvlSTVr1/ftf+cfO/ie++9p2bNmikwMFApKSnKyMhwO44dO3Zo3LhxatKkiYKCghQZGakBAwa4Hce8efM0YMAASdLll1/u+j08lB04s7/++ksjR45UQkKCAgMDVb9+fT322GNuh8nPz9ddd92l6OhoVa9eXddcc4327t3rdpiT18aT1atXT8OHD3d9fabrER9++KG6dOmimjVrKiQkRG3bttXrr79e4ni3bt2qyy+/XMHBwapVq5aeeuops/8IVGl//fWXRowYodjYWNd68/LLL7sdZtq0aUpJSVFwcLDCw8N1ySWXuP72zrSevfLKK+rWrZtiYmIUGBio5ORkzZgxo8x5Pv74Y7Vs2VLVqlVTcnKyFi9efMbTUNpzLt988021adPGtb80b95czz//fImfLc8+DO/mdz6O9Oeff1bnzp0VEhKi++67T/7+/po1a5a6du2qVatWqX379q7Djhs3TtHR0Zo4caLrFscZM2Zo/Pjx6ty5s+68805t375d/fr1U3h4uNvCkZubqzlz5mjw4MHq3bu3Hn/8cR04cEC9e/fW2rVr1bJlS7e5Xn/9dR06dEhjx46Vw+HQU089pf79+2vr1q3y9/cv9bSMHTvWFYXFMjIytGDBAsXExJSYY/To0Tp06JDmzp3rmqPYAw88oMcff1zXXHON+vfvL0lq0aJFmf+Po0aN0vz583Xdddfp7rvv1tdff63HH39cGzdu1Lvvvut22N9//13XXXedRo4cqWHDhunll1/W8OHD1aZNG6WkpJT5O4DKoH///tq0aZPeeOMNPfvss4qKipIkRUdHS5I+//xzLV68WOPGjVPNmjX1wgsv6Nprr9XOnTsVGRkpSVq3bp2+/PJLXX/99apdu7a2b9+uGTNmqGvXrvrll18UHBysyy67TLfffrteeOEFPfjgg0pKSpIk178ASpeZmal27dopJydHY8aMUdOmTfXXX3/ptddeczvcbbfdpvDwcE2aNEnbt2/Xc889p/Hjx2vhwoXn/LtLux4xb948jRgxQikpKXrggQcUFhamDRs2KCMjQzfccIPbz48fP17XX3+9Bg4cqLffflv/93//p+bNm6tPnz7nPBOqpj179ujSSy91vZBcdHS0PvzwQ40cOVK5ubmaMGGCZs+erdtvv13XXXed7rjjDuXl5emHH37Q119/rRtuuOGM69mMGTOUkpKiq666Sn5+fkpPT9e4cePkdDp16623us2zefNmDRo0SLfccouGDRumV155RQMGDFBGRoZ69uxZ7tO1fPlyDR48WN27d9eTTz4pSdq4caO++OIL3XHHHW6HPR/7MKoY6zzo16+fFRAQYG3ZssW1LTMz06pZs6Z12WWXWZZlWa+88oolyerUqZNVWFjoOlx+fr4VGRlptW3b1iooKHBtnzdvniXJ6tKli2tbYWGhlZ+fb1mWZX377beWJOvTTz+1YmNjrREjRrgOt23bNkuSFRkZae3fv9+1/f3337ckWenp6a5tkyZNsk7337J582YrNDTU6tmzp2vuk+coduDAAdccxbOtWLHCkmRNmjSpxPGe+nu/++47S5I1atQot8Pdc889liTrf//7n2tb3bp1LUnWZ5995tqWlZVlBQYGWnfffXeZp6WiFZ/Ob7/99oL9TniPp59+2pJkbdu2zW27JCsgIMD6/fffXdu+//57S5I1bdo017ajR4+WOM41a9ZYkqxXX33VtW3RokWWJGvlypUVfhoAy6qal5VDhw61fHx8rHXr1rltLz6txWtcjx49LKfT6fr+nXfeafn6+lo5OTmubWWtk3Xr1rWGDRvm+rqs6xE5OTlWzZo1rfbt21vHjh1zO46Tf3ebNm0sSdY///lP17b8/HwrLi7Ouvbaa8/6/8BTVcW/N7uMHDnSio+Pt7Kzs922X3/99VZoaKh19OhR6+qrr7ZSUlJOezxlrWeWVfpa1bt3b6tBgwZu24qv+73zzjuubQcPHrTi4+OtVq1aubatXLmyxJo2bNgwq27duq6v77jjDiskJMRtPzpV8f5Wnn0YZ68q7acV/rDYoqIiffzxx+rXr58aNGjg2h4fH68bbrhBn3/+uXJzc13bR48eLV9fX9fX33zzjfbt26fRo0fLz+//37F64403Kjw83O13+fr6KiAgQJLkdDolnXgo6SWXXKL169eXmG3QoEFux9G5c2dJJx4SUx5HjhzRNddco/DwcL3xxhuuuU+dY//+/aedozw++OADSdJdd93ltv3uu++WJC1btsxte3Jysuv0SCduAWvSpEm5TxtQmfXo0UMNGzZ0fd2iRQuFhIS4/f0HBQW5Pi8oKNC+ffuUmJiosLCwc95PAZxY99577z2lpqbqkksuOe1hx4wZ4/YUkM6dO6uoqEg7duw4599/6vWI5cuX69ChQ7r//vtLvJZBaW/59fe//931eUBAgNq1a8faiRIsy9I777yj1NRUWZal7Oxs10fv3r118OBBrV+/XmFhYfrzzz9LPO2qvE5eqw4ePKjs7Gx16dJFW7du1cGDB90Om5CQoGuuucb1dUhIiIYOHaoNGzZo9+7d5f6dYWFhOnLkiJYvX37Gw56PfRhVS4XH5d69e3X06FE1adKkxPeSkpLkdDr1xx9/uLbVr1/f7TDFf5yJiYlu2/38/Ep9T5758+erRYsW6tChg6QTVzKXLVtWYgeUpDp16rh9XRyaBw4cKMcpO7GAbdmyRe+++67roXanzlGtWjVFRkYqOjq6zDnKY8eOHfLx8Snx/xAXF6ewsLASO/Gpp006cfrKe9qAyqw8f//Hjh3TxIkTddFFFykwMFBRUVGKjo5WTk7OOe+nAE6s+7m5uWrWrNkZD2u6Dpfm1OsRW7ZskaRyzSOVDE7WTpRm7969ysnJ0UsvvaTo6Gi3j5tvvlmSlJWVpf/7v/9TjRo11K5dOzVq1Ei33nqrvvjii3L/ni+++EI9evRQ9erVFRYWpujoaD344IOSVGKtSkxMLPH327hxY0k6q1c8HzdunBo3bqw+ffqodu3aGjFiRInXLSh2PvZhVC22v1rsybfQnK3XXntNw4cPV8OGDTVx4kRJ0vTp09WtWzfXPZknO/mWzZNZlnXG3/X888/rjTfe0OzZs0s8l/PkOebOnauMjAwtX768zDnORmm3spbG5LQBlV15/v5vu+02Pfrooxo4cKDeeustffzxx1q+fLkiIyON91MA5WOyVhUVFZW63eR6RFlYO3Gq4nViyJAhWr58eakfHTt2VFJSkn777Te9+eab6tSpk9555x116tRJkyZNOuPv2LJli7p3767s7GxNnTpVy5Yt0/Lly3XnnXe6zVDRYmJi9N1332nJkiW66qqrtHLlSvXp00fDhg0rcViub+JMKvwFfaKjoxUcHFzq++f8+uuv8vHx0UUXXVTmwwXq1q0r6cQL1Fx++eWu7YWFhdq+fbvbC+C8/fbbatCggRYvXqwNGzZo4sSJat++fYkXEDC1evVq3XPPPZowYYJuvPHGEt8/eY6TY/DUC5LyhqJ04v/B6XRq8+bNbi8msmfPHuXk5Lj+nwBvcTb7T2nefvttDRs2TM8884xrW15eXon3GTP9PYC3iY6OVkhIiH766acKOb7w8PAS++Xx48e1a9eucv188UPkf/rppxKP/gHOVXR0tGrWrKmioqISL/R4qurVq2vQoEEaNGiQjh8/rv79++vRRx/VAw88oGrVqpW5zqSnpys/P19Llixxu4fw1HcfKPb777/Lsiy349u0aZMklfpov9MJCAhQamqqUlNT5XQ6NW7cOM2aNUuPPPII+xHOSoXfc+nr66tevXrp/fffd7tLfs+ePXr99dfVqVMnhYSElPnzl1xyiSIjIzV79mwVFha6ti9YsKDEXe7Ft56cfGvJjz/+qDVr1lTQqZF27dqlgQMHqlOnTnr66adLPUxpc3z99dcl5ih+7kd53jS3+Dkgzz33nNv2qVOnSpL69u1brvmBqqJ69eqSyrf/lMbX17fELavTpk0rcW+I6e8BvI2Pj4/69eun9PR0ffPNN8bH17BhQ3322Wdu21566aUy77k8Va9evVSzZk09/vjjysvLc/se967gXPn6+uraa6/VO++8U+oNKcVvx7Fv3z63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vvjiC40fP1533323evXqpb/++svusQAAqNKOHDmiW265RVdddZUuvfRS/fjjj6pfv77dY3ks4hIAKolq1arpmWee0YoVK/Trr7+qefPmmjx5svbs2WP3aAAAVClHjhzRzJkz1aJFC/33v//VrFmz9P777ysmJsbu0TwacQkAlUz37t31ww8/aPDgwXrqqadUp04dDR8+XBs2bLB7NAAAKrWdO3fq//7v/3TRRRfp1ltvVatWrbR+/XqNGTNGDofD7vE8HnEJAJVQRESEXnzxRf3555/617/+pf/9739q3bq1unTporfeekuHDx+2e0QAACqFgoICffLJJxo4cKAaNGigWbNmacSIEdqyZYvefvtt3nLkLBCXAFCJhYeH695779XWrVu1aNEiFRUVadCgQYqMjFSfPn00ffp0/fHHH3aPCQCARzlw4IBef/11DR48WNHR0erRo4e+++47Pf/88/rzzz/173//W/Xq1bN7zErHYVmWZfcQADxTWlqa5syZoz///NPuUXAWtmzZovT0dC1ZskSrV69WYWGhWrZsqdTUVF111VVq3bo1r3IHAPAqlmXp999/V3p6utLT07V69WoVFRWpdevWSk1NVWpqqlq3bs1DXw0RlwDKRFxWfjk5OcrIyFB6ero++OAD5eTkKCwsTO3bt1eHDh106aWXqn379goLC7N7VAAAKkxeXp6+/fZbrVmzRl999ZXWrFmjzMxMBQYGqnv37kpNTdWVV16p2rVr2z1qlUJcAigTcVm1FBQU6Msvv9Tq1atdi+3+/fvlcDiUlJSkSy+9VB06dFCHDh2UlJTEvZsAgErBsizt2LHDFZFr1qzRd999p4KCAgUFBalt27bq0KGDOnbsqG7duql69ep2j1xl+dk9AADgwvD391eXLl3UpUsXSScW482bN7sW4q+++krz5s2T0+lUjRo1lJSUpKZNm7o+kpKS1LBhQwUEBNh8SgAA3qioqEg7d+7Ur7/+qo0bN+rXX391fZ6dnS1JatiwoTp06KBhw4apQ4cOat68ufz9/W2e3HsQlwDgpRwOhxo3bqzGjRtr2LBhkqRDhw5p3bp1+uabb1yLdnp6unJyciRJvr6+atiwoSs2T45PHloLAKgIR48e1aZNm1zrUHFAbtq0SXl5eZKkoKAg1/rTvXt3tWrVSpdeeinvQ2kzHhYLoEw8LBbSiXs4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",
+                        "image/png": "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kZubqzlz5mjw4MHq3bu3Hn/8cR04cEC9e/fW2rVr1bJlS7e5Xn/9dR06dEhjx46Vw+HQU089pf79+2vr1q3y9/cv9bSMHTvWFYXFMjIytGDBAsXExJSYY/To0Tp06JDmzp3rmqPYAw88oMcff1zXXHON+vfvL0lq0aJFmf+Po0aN0vz583Xdddfp7rvv1tdff63HH39cGzdu1Lvvvut22N9//13XXXedRo4cqWHDhunll1/W8OHD1aZNG6WkpJT5O4DKoH///tq0aZPeeOMNPfvss4qKipIkRUdHS5I+//xzLV68WOPGjVPNmjX1wgsv6Nprr9XOnTsVGRkpSVq3bp2+/PJLXX/99apdu7a2b9+uGTNmqGvXrvrll18UHBysyy67TLfffrteeOEFPfjgg0pKSpIk178ASpeZmal27dopJydHY8aMUdOmTfXXX3/ptddeczvcbbfdpvDwcE2aNEnbt2/Xc889p/Hjx2vhwoXn/LtLux4xb948jRgxQikpKXrggQcUFhamDRs2KCMjQzfccIPbz48fP17XX3+9Bg4cqLffflv/93//p+bNm6tPnz7nPBOqpj179ujSSy91vZBcdHS0PvzwQ40cOVK5ubmaMGGCZs+erdtvv13XXXed7rjjDuXl5emHH37Q119/rRtuuOGM69mMGTOUkpKiq666Sn5+fkpPT9e4cePkdDp16623us2zefNmDRo0SLfccouGDRumV155RQMGDFBGRoZ69uxZ7tO1fPlyDR48WN27d9eTTz4pSdq4caO++OIL3XHHHW6HPR/7MKoY6zzo16+fFRAQYG3ZssW1LTMz06pZs6Z12WWXWZZlWa+88oolyerUqZNVWFjoOlx+fr4VGRlptW3b1iooKHBtnzdvniXJ6tKli2tbYWGhlZ+fb1mWZX377beWJOvTTz+1YmNjrREjRrgOt23bNkuSFRkZae3fv9+1/f3337ckWenp6a5tkyZNsk7337J582YrNDTU6tmzp2vuk+coduDAAdccxbOtWLHCkmRNmjSpxPGe+nu/++47S5I1atQot8Pdc889liTrf//7n2tb3bp1LUnWZ5995tqWlZVlBQYGWnfffXeZp6WiFZ/Ob7/99oL9TniPp59+2pJkbdu2zW27JCsgIMD6/fffXdu+//57S5I1bdo017ajR4+WOM41a9ZYkqxXX33VtW3RokWWJGvlypUVfhoAy6qal5VDhw61fHx8rHXr1rltLz6txWtcjx49LKfT6fr+nXfeafn6+lo5OTmubWWtk3Xr1rWGDRvm+rqs6xE5OTlWzZo1rfbt21vHjh1zO46Tf3ebNm0sSdY///lP17b8/HwrLi7Ouvbaa8/6/8BTVcW/N7uMHDnSio+Pt7Kzs922X3/99VZoaKh19OhR6+qrr7ZSUlJOezxlrWeWVfpa1bt3b6tBgwZu24qv+73zzjuubQcPHrTi4+OtVq1aubatXLmyxJo2bNgwq27duq6v77jjDiskJMRtPzpV8f5Wnn0YZ68q7acV/rDYoqIiffzxx+rXr58aNGjg2h4fH68bbrhBn3/+uXJzc13bR48eLV9fX9fX33zzjfbt26fRo0fLz+//37F64403Kjw83O13+fr6KiAgQJLkdDolnXgo6SWXXKL169eXmG3QoEFux9G5c2dJJx4SUx5HjhzRNddco/DwcL3xxhuuuU+dY//+/aedozw++OADSdJdd93ltv3uu++WJC1btsxte3Jysuv0SCduAWvSpEm5TxtQmfXo0UMNGzZ0fd2iRQuFhIS4/f0HBQW5Pi8oKNC+ffuUmJiosLCwc95PAZxY99577z2lpqbqkksuOe1hx4wZ4/YUkM6dO6uoqEg7duw4599/6vWI5cuX69ChQ7r//vtLvJZBaW/59fe//931eUBAgNq1a8faiRIsy9I777yj1NRUWZal7Oxs10fv3r118OBBrV+/XmFhYfrzzz9LPO2qvE5eqw4ePKjs7Gx16dJFW7du1cGDB90Om5CQoGuuucb1dUhIiIYOHaoNGzZo9+7d5f6dYWFhOnLkiJYvX37Gw56PfRhVS4XH5d69e3X06FE1adKkxPeSkpLkdDr1xx9/uLbVr1/f7TDFf5yJiYlu2/38/Ep9T5758+erRYsW6tChg6QTVzKXLVtWYgeUpDp16rh9XRyaBw4cKMcpO7GAbdmyRe+++67roXanzlGtWjVFRkYqOjq6zDnKY8eOHfLx8Snx/xAXF6ewsLASO/Gpp006cfrKe9qAyqw8f//Hjh3TxIkTddFFFykwMFBRUVGKjo5WTk7OOe+nAE6s+7m5uWrWrNkZD2u6Dpfm1OsRW7ZskaRyzSOVDE7WTpRm7969ysnJ0UsvvaTo6Gi3j5tvvlmSlJWVpf/7v/9TjRo11K5dOzVq1Ei33nqrvvjii3L/ni+++EI9evRQ9erVFRYWpujoaD344IOSVGKtSkxMLPH327hxY0k6q1c8HzdunBo3bqw+ffqodu3aGjFiRInXLSh2PvZhVC22v1rsybfQnK3XXntNw4cPV8OGDTVx4kRJ0vTp09WtWzfXPZknO/mWzZNZlnXG3/X888/rjTfe0OzZs0s8l/PkOebOnauMjAwtX768zDnORmm3spbG5LQBlV15/v5vu+02Pfrooxo4cKDeeustffzxx1q+fLkiIyON91MA5WOyVhUVFZW63eR6RFlYO3Gq4nViyJAhWr58eakfHTt2VFJSkn777Te9+eab6tSpk9555x116tRJkyZNOuPv2LJli7p3767s7GxNnTpVy5Yt0/Lly3XnnXe6zVDRYmJi9N1332nJkiW66qqrtHLlSvXp00fDhg0rcViub+JMKvwFfaKjoxUcHFzq++f8+uuv8vHx0UUXXVTmwwXq1q0r6cQL1Fx++eWu7YWFhdq+fbvbC+C8/fbbatCggRYvXqwNGzZo4sSJat++fYkXEDC1evVq3XPPPZowYYJuvPHGEt8/eY6TY/DUC5LyhqJ04v/B6XRq8+bNbi8msmfPHuXk5Lj+nwBvcTb7T2nefvttDRs2TM8884xrW15eXon3GTP9PYC3iY6OVkhIiH766acKOb7w8PAS++Xx48e1a9eucv188UPkf/rppxKP/gHOVXR0tGrWrKmioqISL/R4qurVq2vQoEEaNGiQjh8/rv79++vRRx/VAw88oGrVqpW5zqSnpys/P19Llixxu4fw1HcfKPb777/Lsiy349u0aZMklfpov9MJCAhQamqqUlNT5XQ6NW7cOM2aNUuPPPII+xHOSoXfc+nr66tevXrp/fffd7tLfs+ePXr99dfVqVMnhYSElPnzl1xyiSIjIzV79mwVFha6ti9YsKDEXe7Ft56cfGvJjz/+qDVr1lTQqZF27dqlgQMHqlOnTnr66adLPUxpc3z99dcl5ih+7kd53jS3+Dkgzz33nNv2qVOnSpL69u1brvmBqqJ69eqSyrf/lMbX17fELavTpk0rcW+I6e8BvI2Pj4/69eun9PR0ffPNN8bH17BhQ3322Wdu21566aUy77k8Va9evVSzZk09/vjjysvLc/se967gXPn6+uraa6/VO++8U+oNKcVvx7Fv3z63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vvjiC40fP1533323evXqpb/++svusQAAqNKOHDmiW265RVdddZUuvfRS/fjjj6pfv77dY3ks4hIAKolq1arpmWee0YoVK/Trr7+qefPmmjx5svbs2WP3aAAAVClHjhzRzJkz1aJFC/33v//VrFmz9P777ysmJsbu0TwacQkAlUz37t31ww8/aPDgwXrqqadUp04dDR8+XBs2bLB7NAAAKrWdO3fq//7v/3TRRRfp1ltvVatWrbR+/XqNGTNGDofD7vE8HnEJAJVQRESEXnzxRf3555/617/+pf/9739q3bq1unTporfeekuHDx+2e0QAACqFgoICffLJJxo4cKAaNGigWbNmacSIEdqyZYvefvtt3nLkLBCXAFCJhYeH695779XWrVu1aNEiFRUVadCgQYqMjFSfPn00ffp0/fHHH3aPCQCARzlw4IBef/11DR48WNHR0erRo4e+++47Pf/88/rzzz/173//W/Xq1bN7zErHYVmWZfcQADxTWlqa5syZoz///NPuUXAWtmzZovT0dC1ZskSrV69WYWGhWrZsqdTUVF111VVq3bo1r3IHAPAqlmXp999/V3p6utLT07V69WoVFRWpdevWSk1NVWpqqlq3bs1DXw0RlwDKRFxWfjk5OcrIyFB6ero++OAD5eTkKCwsTO3bt1eHDh106aWXqn379goLC7N7VAAAKkxeXp6+/fZbrVmzRl999ZXWrFmjzMxMBQYGqnv37kpNTdWVV16p2rVr2z1qlUJcAigTcVm1FBQU6Msvv9Tq1atdi+3+/fvlcDiUlJSkSy+9VB06dFCHDh2UlJTEvZsAgErBsizt2LHDFZFr1qzRd999p4KCAgUFBalt27bq0KGDOnbsqG7duql69ep2j1xl+dk9AADgwvD391eXLl3UpUsXSScW482bN7sW4q+++krz5s2T0+lUjRo1lJSUpKZNm7o+kpKS1LBhQwUEBNh8SgAA3qioqEg7d+7Ur7/+qo0bN+rXX391fZ6dnS1JatiwoTp06KBhw4apQ4cOat68ufz9/W2e3HsQlwDgpRwOhxo3bqzGjRtr2LBhkqRDhw5p3bp1+uabb1yLdnp6unJyciRJvr6+atiwoSs2T45PHloLAKgIR48e1aZNm1zrUHFAbtq0SXl5eZKkoKAg1/rTvXt3tWrVSpdeeinvQ2kzHhYLoEw8LBbSiXs4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",
                         "text/plain": [
                             "<Figure size 900x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -294,15 +294,15 @@
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5cAAAIHCAYAAAALhKgSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAAA7rUlEQVR4nO3dd5xUhb3w/++wNOkLgrCAVDGIAiJSDBo1JoAaLEE0ihVRY8V6rxoVTfHGciPgRVR8LKiJ4oMFo2C5ojEKEruisdCkqKGICNJ25/dHfuzjuqDAWTyzO+/368WL3dnZme/u2TnnfKacyWSz2WwAAABAAtXSHgAAAIDKT1wCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABIrHraA1Sk+fPnx5IlS9IeY5N23HHH2HnnndMeY7vL5WUAkCvyZZsQYbsAlUG+rJNyeX1UVZZBlYnL+fPnR+fOnWP16tVpj7JJderUiffee69K/NFsTq4vA4BckQ/bhAjbBags8mGdlOvro6qyDKpMXC5ZsiRWr14d9957b3Tu3Dntccp47733YujQobFkyZJK/wfzXXJ5GQDkinzZJkTYLkBlkC/rpFxeH1WlZVBl4nKjzp07R48ePdIeI69ZBgB8k+0CkCusj7YvB/QBAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5ffcNJJJ0Xbtm23+vvmzp0bmUwm7rrrrgqfCfhumUwmzj777LTHAMhpI0eOjEwmE0uWLKmQy7vrrrsik8nE3LlzS0/bf//9Y//99//e7502bVpkMpmYNm1ahcwC28tJJ50U9erVS+W6t/T2lGvyLi4XLVoUI0eOjDfeeGO7Xs8TTzwRI0eO3K7XAfnkpZdeipEjR8YXX3yxXa9n1qxZMXLkyDI7TAAAfL+8jMurr756k3F5++23xz//+c+tvsw2bdrE119/Hccff3zpaU888URcffXVSUYFvuGll16Kq6+++geJy6uvvlpcAnyH448/Pr7++uto06ZN2qMAOaR62gPkkho1amzT92Uymahdu3YFTwMAkJsKCgqioKAg7TGAHFMpHrmcN29enHnmmbHrrrvGDjvsEE2aNImjjjpqk48srFy5Ms4///xo27Zt1KpVK1q1ahUnnHBCLFmyJKZNmxZ77713REScfPLJkclkyrxW8puvuVy/fn00btw4Tj755HLX8eWXX0bt2rXjoosuiojyr7k86aST4n/+538i4t/huddee0VERDabjbZt28Zhhx1W7jLXrFkTDRs2jNNPPz3JrwqqpJEjR8bFF18cERHt2rUrve1+cx3wyCOPxO677x61atWKLl26xJQpU8pcxpasR+6666446qijIiLigAMOKL0erwsCqoolS5bEkCFDokGDBtGkSZM477zzYs2aNRHx3ceQyGQyZV7us6nXXG7KggUL4vDDD4+6detGs2bN4vzzz4+1a9dW4E8Em7Zy5coYMWJEaRMcdNBBERHx3nvvlZ5nxowZcfDBB0dhYWHUrVs3unbtGqNGjSp3WQsXLozDDz886tWrF02bNo2LLrooiouLy5xn1apVceGFF0br1q2jVq1aseuuu8YNN9wQ2Wy2zPk2bNgQv/3tb6NDhw5Rq1ataNu2bdx8883b4TeQjkrxyOXMmTPjpZdeimOOOSZatWoVc+fOjVtuuSX233//mDVrVtSpU6f0vMOGDYu5c+fGKaecEj169IglS5bEY489FgsWLIjOnTvHNddcE1deeWWcdtppse+++0ZExD777FPuOmvUqBFHHHFETJo0KW699daoWbNm6dceeeSRWLt2bRxzzDGbnPf000+PRYsWxdNPPx0TJkyIuXPnxhVXXBGZTCaGDh0a1113XSxbtiwaN25c+j2TJ0+OL7/8MoYOHVpRvzaoMo488sj44IMP4s9//nP86U9/ih133DEiIpo2bRoRES+++GJMmjQpzjzzzKhfv36MHj06fvnLX8b8+fOjSZMmEbFl65H99tsvzj333Bg9enRcdtll0blz54iI0v8BKrshQ4ZE27Zt49prr43p06fH6NGjY/ny5XHPPfdU+HV9/fXX8dOf/jTmz58f5557bhQVFcWECRPif//3fyv8uuDbzjjjjHjooYfi7LPPjt122y3eeuutGD16dMyZMyciIp5++uk49NBDo0WLFnHeeedF8+bN47333ovHH388zjvvvNLLKS4ujv79+0fv3r3jhhtuiGeeeSZuvPHG6NChQ/z617+OiH8/gDRo0KB47rnnYtiwYdG9e/eYOnVqXHzxxbFw4cL405/+VHp5p556atx9990xePDguPDCC2PGjBlx5513/rC/nO0pWwmsXr263Gkvv/xyNiKy99xzTzabzWZfffXVbERkIyI7adKkcucvKSnJZrPZ7MyZM7MRkb3zzjvLnefEE0/MtmnTpvTzqVOnZiMiO3ny5DLnO/jgg7Pt27cv/XzOnDnlLvOss87Kbvz1bpzt1Vdfzf7zn//MRkT2lltuKXOZgwYNyrZt27Z0zsromz8nVLTrr78+GxHZOXPmlDk9IrI1a9bMfvTRR6Wnvfnmm9mIyI4ZM6b0tC1Zj2Sz2ezEiROzEZF97rnnKvxngGw2v9aV+fSz5rqrrroqGxHZQYMGlTn9zDPPzEZE9s0339zk/sxGEZG96qqrSj+/8847y62Tf/KTn2R/8pOflH5+0003ZSMi++CDD5aetmrVqmzHjh2tZ3NIVb2dNmzYMHvWWWeVfv7Nn3PDhg3Zdu3aZdu0aZNdvnx5me/75r74iSeemI2I7DXXXFPmPHvuuWd2r732Kv38kUceyUZE9ne/+12Z8w0ePDibyWRK91HeeOONbERkTz311DLnO/7447MRkR03blzpad++PVUWleJpsTvssEPpx+vXr4+lS5dGx44do1GjRvHaa6+VOW+nTp3iiCOOKHcZmUxmq6/3wAMPjB133DEeeOCB0tOWL18eTz/9dBx99NFbfXkb5+vdu3fcd999pactW7YsnnzyyTjuuOO2aU7IdwcddFB06NCh9POuXbtGgwYNYvbs2aWnbc16BKCqOuuss8p8fs4550TEvw9EWNGeeOKJaNGiRQwePLj0tDp16sRpp51W4dcF39aoUaOYMWNGLFq0qNzXXn/99ZgzZ06MGDEiGjVqVOZrm9oXP+OMM8p8vu+++5bZx3jiiSeioKAgzj333DLnu/DCCyObzcaTTz5Zer6IiAsuuKDM+TY+c/HFF1/cwp8ud1WKuPz666/jyiuvLH0O84477hhNmzaNL774IlasWFHmvN/cwUyqevXq8ctf/jIeffTR0tcHTJo0KdavX7/NcRkRccIJJ8Tf//73mDdvXkRETJw4MdavX1/maLPAltt5553LnVZYWBjLly8v/Xxr1iMAVdUuu+xS5vMOHTpEtWrVtssRsufNmxcdO3Yst7O+6667Vvh1wbddd9118c4770Tr1q2jV69eceutt5Z+7eOPP46IiN133/17L6d27dqlL8PZ6Nv7GPPmzYuioqKoX79+mfNtfFnNxn3+efPmRbVq1aJjx45lzrfx5T6LFy/e0h8vZ1WKuDznnHPi97//fQwZMiQefPDBeOqpp+Lpp5+OJk2aRElJyXa97mOOOSZWrlxZeo/Dgw8+GD/60Y+iW7duiS6zRo0apY9e3nvvvdGzZ08rW9hGmztiYfYbL6JPcz0CkKu+GX6be/bUtw9cApXBkCFDYvbs2TFmzJgoKioqfV3x3//+9626nO1xVOSq/EzFShGXDz30UJx44olx4403xuDBg+NnP/tZ9OvXb5Pvd7fxnojN2dqFud9++0WLFi3igQceiCVLlsT//u//btGjlt91PY0bN45DDjkk7rvvvpg3b178/e9/96glfI+kK+ItXY9U5RU+wIcffljm848++ihKSkqibdu2UVhYGBFRbr248VGXrdWmTZv4+OOPyx0tc1veUxy2RYsWLeLMM8+MRx55JCZPnhwREXfccUfpMx3feeedCrmeNm3axKJFi2LlypVlTn///fdLv77x/5KSknK3w6VLl5bOW9lVirgsKCgot2IaM2bMJu9J++CDD+Lhhx8ud/rG769bt25ElF9xbk61atVi8ODBMXny5JgwYUJs2LBhi+Ly+67n+OOPj1mzZsXFF18cBQUFmz3yLPBvW3vb/bYtXY8kvR6AXLbxrdI2GjNmTEREDBw4MBo0aBA77rhjvPDCC2XOM3bs2G26roMPPjgWLVoUDz30UOlpq1evjttuu22bLg+2VHFxcbmXvGx8l4b169dHjx49ol27dnHTTTeV295/e19hSxx88MFRXFxc7i1F/vSnP0Umk4mBAweWni8i4qabbipzvo3PZuzXr99WX3euqRRvRXLooYfGhAkTomHDhrHbbrvFyy+/HM8880zpWwx8U/v27eOoo46KU045Jfbaa69YtmxZPPbYYzFu3Ljo1q1bdOjQIRo1ahTjxo2L+vXrR926daN3797Rrl27zV7/0UcfHWPGjImrrroq9thjjy16W4KN72157rnnRqdOncp9/ZBDDokmTZrExIkTY+DAgdGsWbOt+I1A/tl4m7r88stLn1r+i1/8You/f0vXI927d4+CgoL44x//GCtWrIhatWrFgQce6DYKVAlz5syJQYMGxYABA+Lll1+Oe++9N4499tjSl/uceuqp8V//9V9x6qmnRs+ePeOFF16IDz74YJuua/jw4XHzzTfHCSecEK+++mq0aNEiJkyYUOYt5GB7WLlyZbRq1SoGDx4c3bp1i3r16sXEiRMjIqJ///5RrVq1uOWWW+IXv/hFdO/ePU4++eRo0aJFvP/++/Huu+/G1KlTt+r6fvGLX8QBBxwQl19+ecydOze6desWTz31VDz66KMxYsSI0kdKu3XrFieeeGLcdttt8cUXX8RPfvKTeOWVV+Luu++OiIi99967Yn8RKagUcTlq1KgoKCiI++67L9asWRM//vGP45lnnon+/fuXO+/48eNj0qRJ8fDDD8fdd98dzZo1i5/+9KfRqlWriPj3+1fefffdcemll8YZZ5wRGzZsiDvvvPM743KfffaJ1q1bxyeffLLFB/I58sgj45xzzom//OUvce+995b7es2aNePoo4+OsWPHekosbIG99947fvvb38a4ceNiypQpUVJSUvpeVVtiS9cjzZs3j3HjxsW1114bw4YNi+Li4njuuefEJVAlPPDAA3HllVfGf/7nf0b16tXj7LPPjuuvv77061deeWX861//ioceeigefPDBGDhwYDz55JPbtA6sU6dOPPvss3HOOefEmDFjok6dOnHcccfFwIEDY8CAARX5Y0EZderUiTPPPDOeeuqpmDRpUpSUlETLli0j4v8dmbV///7x3HPPxdVXXx033nhjlJSURIcOHWL48OFbfX3VqlWLxx57LK688sp44IEH4s4774y2bdvG9ddfHxdeeGGZ844fPz7at28fd911Vzz88MPRvHnzOPnkk6vMe11mstvy2G8O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5ZxVq1bFiBEjol+/flFYWBhvvPFGXHzxxZ5Zt43EZUKdO3eOF198MW644YYYN25cdO3aNaZNm5b2WDnj/fffj3333TcuvPDCGD58eLz99ttx4IEHpj0WwHaRyWRi2LBh8e6778aee+4ZgwYNiuOOOy6WLl2a9mg5IZvNxp133hldunSJmTNnxiOPPBL3339/NG3aNO3RoEo68MAD46233orhw4fHBRdcEPvtt1+8//77aY+VM6ZNmxZdu3aNW2+9NW644YZ48cUXo3PnzmmPVamJywpQUFAQF1xwQbz11ltRVFQUBxxwQBx++OHxxBNP5OU9RNlsNqZPnx7Dhg2L7t27x9KlS+OFF16IUaNGeR9LIC+0atUqHn/88bjnnnviySefjF133TX+8z//Mz766KO0R0vF6tWr46677oq+ffvGKaecEocffnjMmjUrDjvssLRHgyqvXr16MWrUqHjhhRfiX//6V3Tv3j2GDRsW06dPz8v3xCwuLo6//vWvcfjhh8cBBxwQrVq1irfeeisuuOCCKCgoSHu8Sk9cVqBddtklpk2bFuPHj4+5c+fGIYccEu3atYuRI0fG/Pnz0x5vu1u2bFmMHj06unbtGn379o1nn302rrzyynjjjTeiX79+aY8H8IPKZDJx/PHHx6xZs+LYY4+NW2+9NXbZZZc48MAD489//nNeHAzu9ddfjzPPPDNatGgRJ598cjRo0CCmTp0ad911VxQWFqY9HuSVfv36xZtvvhlXXnll6Vsnde3aNUaPHh3Lli1Le7ztbv78+XHVVVdF27Zt49BDD4158+bF+PHj47nnnotddtkl7fGqDHFZwapVqxbDhg2L119/PV555ZUYMGBA3HjjjdG2bds4+OCD4+GHH47169enPWaFyWaz8fzzz8fQoUOjqKgoLrzwwth1111jypQpMXv27Ljssstihx12SHtMgNQ0b948Ro8eHYsWLYoJEybEhg0b4thjj42WLVvG+eefH7NmzUp7xAq1cuXKuO2226Jnz57Ro0ePeOSRR+Lss8+Ojz/+OJ566qn4+c9/nvaIkLd22GGHuOyyy+Ljjz+OKVOmxK677hoXXnhhFBUVxdChQ+P555+vUo9mrl+/PiZNmhQDBw6Mtm3bxn//93/HwIEDY+bMmfHaa6/FsGHDHFyygmWyVekvKEetXLkyHnjggbj99tvjlVdeiR133DH69esXffv2jT59+sRee+1VaZ4uun79+njzzTdj+vTpMX369HjxxRdj3rx50bFjxxg+fHiceOKJsdNOO6U9JhVk5MiRMX78+FiwYEHao+StxYsXR1FRUTz++OOOpFmFvP/++zF+/Pi4++67Y8mSJbHHHntE3759S7cLnTp1qjQ7PEuXLo0ZM2aUbhf+/ve/x5o1a2LgwIExfPjwOOSQQ6J69eppj0kFadWqVZx66qkxcuTItEehgnz22Wdx1113xfjx4+Ojjz6KNm3aRL9+/aJPnz7Rp0+f6NatW9SoUSPtMbfIqlWr4tVXX42XX365dD91yZIl0atXrxg+fHgcc8wxUa9evbTHrNLE5Q/szTffjAceeCCmT58er7zySqxatSoKCgpKn0q68YbcsWPHnDhK1cKFC0t3GF5++eV49dVXY82aNVGjRo3o0aNH9O7dOw4//PDYf//9c2JeKpa4TJ+4rNrWrl0bjz76aDz11FMxffr0mDVrVmSz2WjUqFH07t07+vTpE3379o1evXrlxNNIN2zYEG+//XaZ7cKHH34YERE77rhj9O3bN3784x/HscceG61bt055WrYHcVl1lZSUxPPPPx+PPPJITJ8+PV5//fVYv3591K5dO3r27Fm6j9qnT59o2bJl2uNGNpuNjz76qHRdNH369HjrrbeiuLg46tatG7169Yo+ffrE0UcfHd26dUt73LwhLlO0YcOGePfdd0s30tOnTy89gldhYWHsvPPO0bx583L/WrRoUfpxgwYNtinqVq1aFZ9++ukm/y1evDg+/fTTWLBgQXz22WcREbHzzjuXWansueeeUbt27Qr9fZB7xGX6xGV+WbFiRcycObN0R2n69Omlr4Vq06ZN6fr/m9uBb/7baaedtultnkpKSmLZsmVltgGb+jd37txYvXp1VK9ePbp3715mu9C+fXt3MuYBcZk/1qxZE6+//nqZ/dSNxxDZaaedolWrVt+5PmrevPk2PTMvm83Gl19++b3ro/nz55e+n/CPfvSj0jvj+vTpE126dHFwnpSIyxyzfPnyeOWVV+If//hHLFq0qFz0ff3112XOX7t27WjcuHHUrFkzatasGTVq1IgaNWpEzZo1o169erF8+fJYv359rF+/PtatWxfr16+PL774Ir766qsyl1OjRo1NRmz37t2jd+/eUVRU9EP+GsgR4jJ94jK/ffOe+VmzZpXbufr888+jpKSkzPcUFhZGvXr1SrcFG//v0KFDzJkzp3RbsPH/tWvXxpIlS2LDhg1lLqdhw4bltgs777xz9OrVK/baay+vp89T4jK/LVq0KGbMmBFvvPHGJsPv28cVqVevXjRq1KjM+qhGjRrRqFGjWLVqVel6aOM6ad26dbFs2bJyBzzbYYcdykVsUVFR9OzZM2ee2cG/eRFEjiksLIz+/ftH//79y30tm83GypUry92Qly1bVi4g161bF7Vr147i4uJyN+gGDRqUu4EWFha6xxkgx2Qymdhll102eyTD4uLiWLJkSbntwqpVq8psE9avXx8NGzaMhg0blgnOjf83bdq0XEiKR+DbioqK4ogjjogjjjii3Ney2WwsX7683AMjX375Zbn91IKCglizZk259VGNGjWicePG5dZH9evXt59aSYjLSiSTyUSDBg2iQYMG0alTp7THASBlBQUFsdNOO8VOO+3kNUVAqjKZTDRu3DgaN24cu+22W9rjkJLKcSg6AAAAcpq4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXADmsdu3a0aRJk1i9enXaowBEQUFBNGrUKO0xgBwlLgFyWMOGDWPZsmXxxRdfpD0KkOdKSkpiwYIFUbdu3bRHAXKUuATIYdWqVYtOnTrFzJkz0x4FyHOvvfZalJSURKdOndIeBchR4hIgxx166KHx+OOPR0lJSdqjAHls8uTJUVhYGD/+8Y/THgXIUeISIMcNGjQoFi9eHK+++mraowB57LHHHouDDz44qlevnvYoQI4SlwA5bp999onGjRvH/fffn/YoQJ5677334o033ohBgwalPQqQw8QlQI6rXr16nHvuuXHzzTfHm2++mfY4QJ4pKSmJ0047LTp06BCHHnpo2uMAOUxcAlQCl156afzoRz+KU045JTZs2JD2OEAeGTduXLz44osxfvz4qFOnTtrjADlMXAJUAjVr1ow77rgj3njjjbjhhhvSHgfIE/PmzYv/+I//iNNPPz3233//tMcBcpy4BKgkevXqFRdddFFcdtllcccdd6Q9DlDFzZs3Lw466KBo3Lhx/PGPf0x7HKAScLgvgErk2muvjS+//DJOPfXU+Oqrr+K8885LeySgCvrggw/ioIMOiurVq8e0adOiYcOGaY8EVALiEqASqVatWowdOzbq1asXI0aMiFWrVsVll12W9lhAFfL222/Hz372sygsLIxnnnkmWrZsmfZIQCXhabEAlUwmk4nrrrsurrnmmrj88svjqKOOis8++yztsYBKrqSkJMaNGxf77LNPtGjRIl544QVhCWwVcQlQCWUymbjiiiviL3/5S0ybNi26dOkS999/f2Sz2bRHAyqh2bNnx0EHHRS//vWv41e/+lU8//zz0bRp07THAioZcQlQiR199NExa9asOOigg+K4446Lww8/PBYtWpT2WEAlUVJSEqNHj4499tgj5syZE08//XTcdttt0aBBg7RHAyohcQlQyTVt2jT+8pe/xKRJk2LGjBmxyy67xAUXXCAygc3asGFD3HvvvbH77rvHeeedF6ecckq8/fbbcdBBB6U9GlCJiUuAKuKII46I9957Ly688ML4P//n/0S7du3i17/+dcydOzft0YAcsXbt2rjtttti1113jeOPPz46dOgQ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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5cAAAIHCAYAAAALhKgSAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA7rUlEQVR4nO3dd5xUhb3w/++wNOkLgrCAVDGIAiJSDBo1JoAaLEE0ihVRY8V6rxoVTfHGciPgRVR8LKiJ4oMFo2C5ojEKEruisdCkqKGICNJ25/dHfuzjuqDAWTyzO+/368WL3dnZme/u2TnnfKacyWSz2WwAAABAAtXSHgAAAIDKT1wCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABIrHraA1Sk+fPnx5IlS9IeY5N23HHH2HnnndMeY7vL5WUAkCvyZZsQYbsAlUG+rJNyeX1UVZZBlYnL+fPnR+fOnWP16tVpj7JJderUiffee69K/NFsTq4vA4BckQ/bhAjbBags8mGdlOvro6qyDKpMXC5ZsiRWr14d9957b3Tu3Dntccp47733YujQobFkyZJK/wfzXXJ5GQDkinzZJkTYLkBlkC/rpFxeH1WlZVBl4nKjzp07R48ePdIeI69ZBgB8k+0CkCusj7YvB/QBAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5ffcNJJJ0Xbtm23+vvmzp0bmUwm7rrrrgqfCfhumUwmzj777LTHAMhpI0eOjEwmE0uWLKmQy7vrrrsik8nE3LlzS0/bf//9Y//99//e7502bVpkMpmYNm1ahcwC28tJJ50U9erVS+W6t/T2lGvyLi4XLVoUI0eOjDfeeGO7Xs8TTzwRI0eO3K7XAfnkpZdeipEjR8YXX3yxXa9n1qxZMXLkyDI7TAAAfL+8jMurr756k3F5++23xz//+c+tvsw2bdrE119/Hccff3zpaU888URcffXVSUYFvuGll16Kq6+++geJy6uvvlpcAnyH448/Pr7++uto06ZN2qMAOaR62gPkkho1amzT92Uymahdu3YFTwMAkJsKCgqioKAg7TGAHFMpHrmcN29enHnmmbHrrrvGDjvsEE2aNImjjjpqk48srFy5Ms4///xo27Zt1KpVK1q1ahUnnHBCLFmyJKZNmxZ77713REScfPLJkclkyrxW8puvuVy/fn00btw4Tj755HLX8eWXX0bt2rXjoosuiojyr7k86aST4n/+538i4t/huddee0VERDabjbZt28Zhhx1W7jLXrFkTDRs2jNNPPz3JrwqqpJEjR8bFF18cERHt2rUrve1+cx3wyCOPxO677x61atWKLl26xJQpU8pcxpasR+6666446qijIiLigAMOKL0erwsCqoolS5bEkCFDokGDBtGkSZM477zzYs2aNRHx3ceQyGQyZV7us6nXXG7KggUL4vDDD4+6detGs2bN4vzzz4+1a9dW4E8Em7Zy5coYMWJEaRMcdNBBERHx3nvvlZ5nxowZcfDBB0dhYWHUrVs3unbtGqNGjSp3WQsXLozDDz886tWrF02bNo2LLrooiouLy5xn1apVceGFF0br1q2jVq1aseuuu8YNN9wQ2Wy2zPk2bNgQv/3tb6NDhw5Rq1ataNu2bdx8883b4TeQjkrxyOXMmTPjpZdeimOOOSZatWoVc+fOjVtuuSX233//mDVrVtSpU6f0vMOGDYu5c+fGKaecEj169IglS5bEY489FgsWLIjOnTvHNddcE1deeWWcdtppse+++0ZExD777FPuOmvUqBFHHHFETJo0KW699daoWbNm6dceeeSRWLt2bRxzzDGbnPf000+PRYsWxdNPPx0TJkyIuXPnxhVXXBGZTCaGDh0a1113XSxbtiwaN25c+j2TJ0+OL7/8MoYOHVpRvzaoMo488sj44IMP4s9//nP86U9/ih133DEiIpo2bRoRES+++GJMmjQpzjzzzKhfv36MHj06fvnLX8b8+fOjSZMmEbFl65H99tsvzj333Bg9enRcdtll0blz54iI0v8BKrshQ4ZE27Zt49prr43p06fH6NGjY/ny5XHPPfdU+HV9/fXX8dOf/jTmz58f5557bhQVFcWECRPif//3fyv8uuDbzjjjjHjooYfi7LPPjt122y3eeuutGD16dMyZMyciIp5++uk49NBDo0WLFnHeeedF8+bN47333ovHH388zjvvvNLLKS4ujv79+0fv3r3jhhtuiGeeeSZuvPHG6NChQ/z617+OiH8/gDRo0KB47rnnYtiwYdG9e/eYOnVqXHzxxbFw4cL405/+VHp5p556atx9990xePDguPDCC2PGjBlx5513/rC/nO0pWwmsXr263Gkvv/xyNiKy99xzTzabzWZfffXVbERkIyI7adKkcucvKSnJZrPZ7MyZM7MRkb3zzjvLnefEE0/MtmnTpvTzqVOnZiMiO3ny5DLnO/jgg7Pt27cv/XzOnDnlLvOss87Kbvz1bpzt1Vdfzf7zn//MRkT2lltuKXOZgwYNyrZt27Z0zsromz8nVLTrr78+GxHZOXPmlDk9IrI1a9bMfvTRR6Wnvfnmm9mIyI4ZM6b0tC1Zj2Sz2ezEiROzEZF97rnnKvxngGw2v9aV+fSz5rqrrroqGxHZQYMGlTn9zDPPzEZE9s0339zk/sxGEZG96qqrSj+/8847y62Tf/KTn2R/8pOflH5+0003ZSMi++CDD5aetmrVqmzHjh2tZ3NIVb2dNmzYMHvWWWeVfv7Nn3PDhg3Zdu3aZdu0aZNdvnx5me/75r74iSeemI2I7DXXXFPmPHvuuWd2r732Kv38kUceyUZE9ne/+12Z8w0ePDibyWRK91HeeOONbERkTz311DLnO/7447MRkR03blzpad++PVUWleJpsTvssEPpx+vXr4+lS5dGx44do1GjRvHaa6+VOW+nTp3iiCOOKHcZmUxmq6/3wAMPjB133DEeeOCB0tOWL18eTz/9dBx99NFbfXkb5+vdu3fcd999pactW7YsnnzyyTjuuOO2aU7IdwcddFB06NCh9POuXbtGgwYNYvbs2aWnbc16BKCqOuuss8p8fs4550TEvw9EWNGeeOKJaNGiRQwePLj0tDp16sRpp51W4dcF39aoUaOYMWNGLFq0qNzXXn/99ZgzZ06MGDEiGjVqVOZrm9oXP+OMM8p8vu+++5bZx3jiiSeioKAgzj333DLnu/DCCyObzcaTTz5Zer6IiAsuuKDM+TY+c/HFF1/cwp8ud1WKuPz666/jyiuvLH0O84477hhNmzaNL774IlasWFHmvN/cwUyqevXq8ctf/jIeffTR0tcHTJo0KdavX7/NcRkRccIJJ8Tf//73mDdvXkRETJw4MdavX1/maLPAltt5553LnVZYWBjLly8v/Xxr1iMAVdUuu+xS5vMOHTpEtWrVtssRsufNmxcdO3Yst7O+6667Vvh1wbddd9118c4770Tr1q2jV69eceutt5Z+7eOPP46IiN133/17L6d27dqlL8PZ6Nv7GPPmzYuioqKoX79+mfNtfFnNxn3+efPmRbVq1aJjx45lzrfx5T6LFy/e0h8vZ1WKuDznnHPi97//fQwZMiQefPDBeOqpp+Lpp5+OJk2aRElJyXa97mOOOSZWrlxZeo/Dgw8+GD/60Y+iW7duiS6zRo0apY9e3nvvvdGzZ08rW9hGmztiYfYbL6JPcz0CkKu+GX6be/bUtw9cApXBkCFDYvbs2TFmzJgoKioqfV3x3//+9626nO1xVOSq/EzFShGXDz30UJx44olx4403xuDBg+NnP/tZ9OvXb5Pvd7fxnojN2dqFud9++0WLFi3igQceiCVLlsT//u//btGjlt91PY0bN45DDjkk7rvvvpg3b178/e9/96glfI+kK+ItXY9U5RU+wIcffljm848++ihKSkqibdu2UVhYGBFRbr248VGXrdWmTZv4+OOPyx0tc1veUxy2RYsWLeLMM8+MRx55JCZPnhwREXfccUfpMx3feeedCrmeNm3axKJFi2LlypVlTn///fdLv77x/5KSknK3w6VLl5bOW9lVirgsKCgot2IaM2bMJu9J++CDD+Lhhx8ud/rG769bt25ElF9xbk61atVi8ODBMXny5JgwYUJs2LBhi+Ly+67n+OOPj1mzZsXFF18cBQUFmz3yLPBvW3vb/bYtXY8kvR6AXLbxrdI2GjNmTEREDBw4MBo0aBA77rhjvPDCC2XOM3bs2G26roMPPjgWLVoUDz30UOlpq1evjttuu22bLg+2VHFxcbmXvGx8l4b169dHjx49ol27dnHTTTeV295/e19hSxx88MFRXFxc7i1F/vSnP0Umk4mBAweWni8i4qabbipzvo3PZuzXr99WX3euqRRvRXLooYfGhAkTomHDhrHbbrvFyy+/HM8880zpWwx8U/v27eOoo46KU045Jfbaa69YtmxZPPbYYzFu3Ljo1q1bdOjQIRo1ahTjxo2L+vXrR926daN3797Rrl27zV7/0UcfHWPGjImrrroq9thjjy16W4KN72157rnnRqdOncp9/ZBDDokmTZrExIkTY+DAgdGsWbOt+I1A/tl4m7r88stLn1r+i1/8You/f0vXI927d4+CgoL44x//GCtWrIhatWrFgQce6DYKVAlz5syJQYMGxYABA+Lll1+Oe++9N4499tjSl/uceuqp8V//9V9x6qmnRs+ePeOFF16IDz74YJuua/jw4XHzzTfHCSecEK+++mq0aNEiJkyYUOYt5GB7WLlyZbRq1SoGDx4c3bp1i3r16sXEiRMjIqJ///5RrVq1uOWWW+IXv/hFdO/ePU4++eRo0aJFvP/++/Huu+/G1KlTt+r6fvGLX8QBBxwQl19+ecydOze6desWTz31VDz66KMxYsSI0kdKu3XrFieeeGLcdttt8cUXX8RPfvKTeOWVV+Luu++OiIi99967Yn8RKagUcTlq1KgoKCiI++67L9asWRM//vGP45lnnon+/fuXO+/48eNj0qRJ8fDDD8fdd98dzZo1i5/+9KfRqlWriPj3+1fefffdcemll8YZZ5wRGzZsiDvvvPM743KfffaJ1q1bxyeffLLFB/I58sgj45xzzom//OUvce+995b7es2aNePoo4+OsWPHekosbIG99947fvvb38a4ceNiypQpUVJSUvpeVVtiS9cjzZs3j3HjxsW1114bw4YNi+Li4njuuefEJVAlPPDAA3HllVfGf/7nf0b16tXj7LPPjuuvv77061deeWX861//ioceeigefPDBGDhwYDz55JPbtA6sU6dOPPvss3HOOefEmDFjok6dOnHcccfFwIEDY8CAARX5Y0EZderUiTPPPDOeeuqpmDRpUpSUlETLli0j4v8dmbV///7x3HPPxdVXXx033nhjlJSURIcOHWL48OFbfX3VqlWLxx57LK688sp44IEH4s4774y2bdvG9ddfHxdeeGGZ844fPz7at28fd911Vzz88MPRvHnzOPnkk6vMe11mstvy2G8O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5ZxVq1bFiBEjol+/flFYWBhvvPFGXHzxxZ5Zt43EZUKdO3eOF198MW644YYYN25cdO3aNaZNm5b2WDnj/fffj3333TcuvPDCGD58eLz99ttx4IEHpj0WwHaRyWRi2LBh8e6778aee+4ZgwYNiuOOOy6WLl2a9mg5IZvNxp133hldunSJmTNnxiOPPBL3339/NG3aNO3RoEo68MAD46233orhw4fHBRdcEPvtt1+8//77aY+VM6ZNmxZdu3aNW2+9NW644YZ48cUXo3PnzmmPVamJywpQUFAQF1xwQbz11ltRVFQUBxxwQBx++OHxxBNP5OU9RNlsNqZPnx7Dhg2L7t27x9KlS+OFF16IUaNGeR9LIC+0atUqHn/88bjnnnviySefjF133TX+8z//Mz766KO0R0vF6tWr46677oq+ffvGKaecEocffnjMmjUrDjvssLRHgyqvXr16MWrUqHjhhRfiX//6V3Tv3j2GDRsW06dPz8v3xCwuLo6//vWvcfjhh8cBBxwQrVq1irfeeisuuOCCKCgoSHu8Sk9cVqBddtklpk2bFuPHj4+5c+fGIYccEu3atYuRI0fG/Pnz0x5vu1u2bFmMHj06unbtGn379o1nn302rrzyynjjjTeiX79+aY8H8IPKZDJx/PHHx6xZs+LYY4+NW2+9NXbZZZc48MAD489//nNeHAzu9ddfjzPPPDNatGgRJ598cjRo0CCmTp0ad911VxQWFqY9HuSVfv36xZtvvhlXXnll6Vsnde3aNUaPHh3Lli1Le7ztbv78+XHVVVdF27Zt49BDD4158+bF+PHj47nnnotddtkl7fGqDHFZwapVqxbDhg2L119/PV555ZUYMGBA3HjjjdG2bds4+OCD4+GHH47169enPWaFyWaz8fzzz8fQoUOjqKgoLrzwwth1111jypQpMXv27Ljssstihx12SHtMgNQ0b948Ro8eHYsWLYoJEybEhg0b4thjj42WLVvG+eefH7NmzUp7xAq1cuXKuO2226Jnz57Ro0ePeOSRR+Lss8+Ojz/+OJ566qn4+c9/nvaIkLd22GGHuOyyy+Ljjz+OKVOmxK677hoXXnhhFBUVxdChQ+P555+vUo9mrl+/PiZNmhQDBw6Mtm3bxn//93/HwIEDY+bMmfHaa6/FsGHDHFyygmWyVekvKEetXLkyHnjggbj99tvjlVdeiR133DH69esXffv2jT59+sRee+1VaZ4uun79+njzzTdj+vTpMX369HjxxRdj3rx50bFjxxg+fHiceOKJsdNOO6U9JhVk5MiRMX78+FiwYEHao+StxYsXR1FRUTz++OOOpFmFvP/++zF+/Pi4++67Y8mSJbHHHntE3759S7cLnTp1qjQ7PEuXLo0ZM2aUbhf+/ve/x5o1a2LgwIExfPjwOOSQQ6J69eppj0kFadWqVZx66qkxcuTItEehgnz22Wdx1113xfjx4+Ojjz6KNm3aRL9+/aJPnz7Rp0+f6NatW9SoUSPtMbfIqlWr4tVXX42XX365dD91yZIl0atXrxg+fHgcc8wxUa9evbTHrNLE5Q/szTffjAceeCCmT58er7zySqxatSoKCgpKn0q68YbcsWPHnDhK1cKFC0t3GF5++eV49dVXY82aNVGjRo3o0aNH9O7dOw4//PDYf//9c2JeKpa4TJ+4rNrWrl0bjz76aDz11FMxffr0mDVrVmSz2WjUqFH07t07+vTpE3379o1evXrlxNNIN2zYEG+//XaZ7cKHH34YERE77rhj9O3bN3784x/HscceG61bt055WrYHcVl1lZSUxPPPPx+PPPJITJ8+PV5//fVYv3591K5dO3r27Fm6j9qnT59o2bJl2uNGNpuNjz76qHRdNH369HjrrbeiuLg46tatG7169Yo+ffrE0UcfHd26dUt73LwhLlO0YcOGePfdd0s30tOnTy89gldhYWHsvPPO0bx583L/WrRoUfpxgwYNtinqVq1aFZ9++ukm/y1evDg+/fTTWLBgQXz22WcREbHzzjuXWansueeeUbt27Qr9fZB7xGX6xGV+WbFiRcycObN0R2n69Omlr4Vq06ZN6fr/m9uBb/7baaedtultnkpKSmLZsmVltgGb+jd37txYvXp1VK9ePbp3715mu9C+fXt3MuYBcZk/1qxZE6+//nqZ/dSNxxDZaaedolWrVt+5PmrevPk2PTMvm83Gl19++b3ro/nz55e+n/CPfvSj0jvj+vTpE126dHFwnpSIyxyzfPnyeOWVV+If//hHLFq0qFz0ff3112XOX7t27WjcuHHUrFkzatasGTVq1IgaNWpEzZo1o169erF8+fJYv359rF+/PtatWxfr16+PL774Ir766qsyl1OjRo1NRmz37t2jd+/eUVRU9EP+GsgR4jJ94jK/ffOe+VmzZpXbufr888+jpKSkzPcUFhZGvXr1SrcFG//v0KFDzJkzp3RbsPH/tWvXxpIlS2LDhg1lLqdhw4bltgs777xz9OrVK/baay+vp89T4jK/LVq0KGbMmBFvvPHGJsPv28cVqVevXjRq1KjM+qhGjRrRqFGjWLVqVel6aOM6ad26dbFs2bJyBzzbYYcdykVsUVFR9OzZM2ee2cG/eRFEjiksLIz+/ftH//79y30tm83GypUry92Qly1bVi4g161bF7Vr147i4uJyN+gGDRqUu4EWFha6xxkgx2Qymdhll102eyTD4uLiWLJkSbntwqpVq8psE9avXx8NGzaMhg0blgnOjf83bdq0XEiKR+DbioqK4ogjjogjjjii3Ney2WwsX7683AMjX375Zbn91IKCglizZk259VGNGjWicePG5dZH9evXt59aSYjLSiSTyUSDBg2iQYMG0alTp7THASBlBQUFsdNOO8VOO+3kNUVAqjKZTDRu3DgaN24cu+22W9rjkJLKcSg6AAAAcpq4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXAAAAJCYuAQAASExcAgAAkJi4BAAAIDFxCQAAQGLiEgAAgMTEJQAAAImJSwAAABITlwAAACQmLgEAAEhMXAIAAJCYuAQAACAxcQkAAEBi4hIAAIDExCUAAACJiUsAAAASE5cAAAAkJi4BAABITFwCAACQmLgEAAAgMXEJAABAYuISAACAxMQlAAAAiYlLAAAAEhOXADmsdu3a0aRJk1i9enXaowBEQUFBNGrUKO0xgBwlLgFyWMOGDWPZsmXxxRdfpD0KkOdKSkpiwYIFUbdu3bRHAXKUuATIYdWqVYtOnTrFzJkz0x4FyHOvvfZalJSURKdOndIeBchR4hIgxx166KHx+OOPR0lJSdqjAHls8uTJUVhYGD/+8Y/THgXIUeISIMcNGjQoFi9eHK+++mraowB57LHHHouDDz44qlevnvYoQI4SlwA5bp999onGjRvH/fffn/YoQJ5677334o033ohBgwalPQqQw8QlQI6rXr16nHvuuXHzzTfHm2++mfY4QJ4pKSmJ0047LTp06BCHHnpo2uMAOUxcAlQCl156afzoRz+KU045JTZs2JD2OEAeGTduXLz44osxfvz4qFOnTtrjADlMXAJUAjVr1ow77rgj3njjjbjhhhvSHgfIE/PmzYv/+I//iNNPPz3233//tMcBcpy4BKgkevXqFRdddFFcdtllcccdd6Q9DlDFzZs3Lw466KBo3Lhx/PGPf0x7HKAScLgvgErk2muvjS+//DJOPfXU+Oqrr+K8885LeySgCvrggw/ioIMOiurVq8e0adOiYcOGaY8EVALiEqASqVatWowdOzbq1asXI0aMiFWrVsVll12W9lhAFfL222/Hz372sygsLIxnnnkmWrZsmfZIQCXhabEAlUwmk4nrrrsurrnmmrj88svjqKOOis8++yztsYBKrqSkJMaNGxf77LNPtGjRIl544QVhCWwVcQlQCWUymbjiiiviL3/5S0ybNi26dOkS999/f2Sz2bRHAyqh2bNnx0EHHRS//vWv41e/+lU8//zz0bRp07THAioZcQlQiR199NExa9asOOigg+K4446Lww8/PBYtWpT2WEAlUVJSEqNHj4499tgj5syZE08//XTcdttt0aBBg7RHAyohcQlQyTVt2jT+8pe/xKRJk2LGjBmxyy67xAUXXCAygc3asGFD3HvvvbH77rvHeeedF6ecckq8/fbbcdBBB6U9GlCJiUuAKuKII46I9957Ly688ML4P//n/0S7du3i17/+dcydOzft0YAcsXbt2rjtttti1113jeOPPz46dOgQ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",
                         "text/plain": [
                             "<Figure size 900x500 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -330,15 +330,15 @@
         {
             "cell_type": "code",
             "execution_count": 10,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5cAAAP7CAYAAADPo3rEAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAADba0lEQVR4nOzdeVhUdf//8dewKqK4oKImWa7kvitB4paauZR3qaWp2aKmZolmabfWnaWmaeWSFYmVaZu5VS6ZuORSobaJZpZahhYoLuACzOf3Rz/mK7nCGTgOPB/X5XXBmXM+5z1H3nPmNWcZhzHGCAAAAAAAC7zsLgAAAAAA4PkIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJfXiO+++06bN2+2uwwAubRgwQKdOHHC7jIA5MKJEye0YMECu8sAkEtfffWVvv/+e7vLgAiX14TNmzcrKipK7dq106pVq+wuB0AOGGM0duxY9enTR23atFFSUpLdJQHIgb///lutW7dWnz59NG7cOBlj7C4JQA6sXLlS7du3V6tWrbRlyxa7yyn0CJc2W7Nmjdq3b6969eqpTZs26tKliz766CO7ywJwFZxOp4YOHarnn39ejz/+uH7//XfdcsstOnTokN2lAbgKf/zxh2655Rb98ccfevzxxzVx4kQNGzZMTqfT7tIAXIUPP/xQXbt2Vdu2bVW3bl21a9dOa9assbusQo1waaOPP/5YnTt3VuvWrbVy5Up98sknuuuuu9SzZ0+99dZbdpcH4DLS09PVr18/zZkzR2+88YamTZumjRs3KjU1VREREfrll1/sLhHAZfzyyy+KiIhQWlqaNm3apGnTpun111/X7Nmz1a9fP6Wnp9tdIoDLiImJUa9evXTXXXdp8eLFWrlypaKionT77bdr8eLFdpdXeBnY4q233jJeXl6mV69e5ty5c67pmZmZZtCgQUaSeemll2ysEMClnD592nTt2tX4+vqa999/P9tjBw8eNDVr1jTly5c333//vU0VAric7777zpQvX97UrFnTHDx4MNtjixYtMj4+PqZr167m9OnTNlUI4HKmTZtmJJnBgwebzMxM1/SzZ8+anj17Gi8vLzNv3jz7CizECJc2mD59upFkHn74YZORkXHB406n0zz55JNGknn66aeN0+m0oUoAF3PixAnTunVrU7RoUfP5559fdJ4jR46Yhg0bmlKlSpktW7bkc4UALmfz5s2mZMmSplGjRuavv/666DyfffaZKVq0qGnTpo05ceJEPlcI4FKcTqcZN26ckWSefPLJi75HzsjIMA899JCRZGbMmGFDlYUb4TIfOZ1O89///tdIMk888cQVQ+OkSZOMJDNs2LBsn8oAsEdSUpJp2rSpKVGihNm4ceNl501JSTERERGmWLFiZs2aNflUIYDLWbNmjQkICDCRkZEmJSXlsvNu2LDBlChRwjRr1swkJyfnU4UALiUzM9MMHTrUSDKTJ0++7LxOp9OMHj3aSDLjx4/nQE0+Ilzmk8zMTDN8+HAjybzwwgtXvdxrr71mHA6Hue+++0x6enoeVgjgcg4dOmRq165typYta+Lj469qmdTUVNOxY0fj5+dnFi9enMcVAricxYsXGz8/P9OpUyeTmpp6VcvEx8eb4OBgU7t2bXPo0KE8rhDApaSnp5u+ffsah8Nh5s6de9XLvfDCC0aSefTRRzlQk08Il/kgPT3d9OvXzzgcDjNnzpwcL79w4ULj4+NjunfvzvUfgA327dtnbrjhBnPdddeZ3bt352jZs2fPmrvvvtt4e3ub+fPn51GFAC4nNjbWeHl5mZ49e5qzZ8/maNmEhARz3XXXmRtvvNH8+uuveVQhgEs5ffq06datm/Hx8TGLFi3K8fKzZ882DofD9O/fnwM1+YBwmcfOnDljunfvbnx8fMx7772X63FWrFhhihQpYtq2bWtOnjzpxgoBXM6PP/5oKlSoYKpXr27279+fqzEyMjLMAw88YCSZV155xc0VAricl19+2UgyDz744EXvc3A19u/fb6pVq2YqVKhgfvzxRzdXCOBSTpw4Ydq0aWOKFCliPv3001yPs2DBAuPt7W3uuOMOc+bMGTdWiH8jXOahkydPmnbt2pkiRYqY5cuXWx5v/fr1pnjx4qZ58+Zc/wHkg23btpnSpUub+vXrm8OHD1say+l0mujoaCPJPPPMM1z/AeQxp9NpJkyYYCSZUaNGWe65w4cPm3r16pnSpUubr7/+2k1VAriU5ORk06xZM1O8eHGzfv16y+MtW7bM+Pv7m/bt23OgJg85jDEm/78ApeA7evSoOnfurJ9++knLly9Xq1at3DJufHy8OnTooAoVKmj16tWqUKGCW8YFkN26devUtWtX1atXT59++qlKlixpeUxjjF544QWNHTtWjz32mKZNmyaHw2G9WADZOJ1OjRw5UjNmzNDzzz+vMWPGuKXXjh07ps6dO+uHH37QsmXL1Lp1azdUC+DfEhMTdeutt+rw4cNauXKlGjdu7JZx4+Li1KVLF9WpU0efffaZSpUq5ZZx8X8Il3ng8OHDuvXWW/Xnn39q5cqVatKkiVvHT0hIUPv27VWkSBGtWbNGN9xwg1vHBwq7ZcuW6e6771arVq20ePFiFStWzK3jz549W4888ogGDBig119/XT4+Pm4dHyjMMjIy9OCDDyo2NlazZs3SkCFD3Dp+amqq7rjjDm3YsEEffvihunTp4tbxgcLut99+U7t27XT27Fl98cUXqlWrllvH/+abb9SxY0ddd911WrVqlUJCQtw6fmHnZXcBBc3+/fsVERGh5ORkbdiwwe3BUpLCwsK0adMmSVJERIR27drl9nUAhdW7776rO++8U7fffruWLVvm9mApSUOGDNE777yjt99+W7169dLZs2fdvg6gMDp79qx69uypd955R++++67bg6UkFStWTMuXL1fnzp11xx13aMGCBW5fB1BY7dq1SxEREfLy8tKmTZvcHiwlqWnTptqwYYOSkpIUGRmpAwcOuH0dhRnh0o0SEhIUEREhSdq0aZNuuummPFtXlSpVtGnTJpUpU0a33HKLvv322zxbF1BYzJo1S3379tV9992nRYsWyd/fP8/W1adPHy1evFgrVqxQ165dlZqammfrAgqD1NRUdenSRZ9++qk++eQT3XvvvXm2Ln9/f73//vvq27ev+vbtq9mzZ+fZuoDC4ptvvtEtt9yi4OBgbdy4UVWqVMmzddWuXVubNm2S0+nUzTffrISEhDxbV2FDuHST+Ph4RUZGqlSpUtq4cWO+nKoaEhKiuLg4Va9eXW3atNH69evzfJ1AQWSM0fPPP6+hQ4fqscce05tvvpkvp6p27dpVn3/+uTZv3qxbb71VKSkpeb5OoCA6duyY2rdvry1btujzzz/Pl1NVfXx8FBMTo0cffVSPPPKIXnjhBXGlEZA7cXFxatOmjWrUqKG4uLh8OVX1hhtu0KZNm1SqVCndcsst2r59e56vszAgXLrBhg0b1Lp1a1WrVk3r16/P15vslC5dWmvWrFGzZs3UsWNHrVixIt/WDRQExhiNHj1aY8eO1bPPPqtp06bJyyv/Xhpbt26ttWvXavfu3YqKitKRI0fybd1AQXDkyBFFRUVpz549+vLLL/P1JjteXl566aWX9Mwzz+ipp57SE088QcAEcmj58uXq2LGjWrRoodWrV+frTXYqVKig9evXq2rVqmrdurU2bNiQb+susGy7T20Bca18/+SZM2fMHXfcYfn7NIHC5Fr6/kl3fJ8mUNhcS98/6Y7v0wQKm6zvn7zzzjtt/f7JkydPuuX7NGEMRy4tWLhwobp37+46YhgYGGhbLf7+/vrggw9077336t5779Vrr71mWy2AJzh37pzuuecezZs3T/Pnz9ewYcNsrSfr+o+MjAxFRERo9+7dttYDXOt2796tiIgIOZ1Obdq0SbVr17a1nuHDhys2NlYxMTG69957de7cOVvrAa51c+bMUZ8+fdS3b1+9//77eXqfgysJDAzUp59+qg4dOqhbt25atGiRbbV4PLvTrad67bXXjMPhMPfdd59JT0+3PN7MmTPN9ddfb/z9/U2zZs3Mtm3bcjVOZmamGT58uJFkXnjhBct1AQVRamqq6dixo/Hz8zOffPKJ5fHc1b/GGHPo0CFTu3ZtU7ZsWbN9+3bLtQEFUXx8vAkODja1a9c2f/75p+Xx3NnDixcvNn5+fqZTp04mNTXVcm1AQfT8888bSebRRx81mZmZlsZyZ/+mp6ebvn37GofDYebOnWuprsKKcJkLkyZNMpLMsGHDLDeEMcYsWrTI+Pn5mbfeesv89NNP5sEHHzQlS5Y0R44cydV4TqfTjB8/3kgyTzzxhHE6nZZrBAqKlJQUExERYYoVK2bWrFljeTx3968xxiQlJZmmTZuaEiVKmA0bNliuEShINmzYYEqUKGGaNWtmkpKSLI+XFz28Zs0aU6xYMRMZGWlSUlIs1wgUFE6n04wePdpIMhMmTLD8HjUv+jczM9MMHTrUSDKTJ0+2VF9hRLjMAafTacaMGWMkmf/+979uC23NmjUzjzzyiOv3zMxMU7FiRctHHqdPn24kmYcffpjrPwBjzJEjR0zDhg1NyZIlzZYtW9wyZl7174kTJ0zr1q1N0aJFzeeff261TKBA+Oyzz0yRIkVMmzZtzIkTJ9wyZl718ObNm03JkiVNw4YNzV9//WW1TMDjZWRkmIceeshIMjNmzHDLmHnVv06n0zz99NNGkhkzZgwHanKAcHmVMjMzzaBBg4wk89JLL7lt3LNnzxpvb+8LTs277777TNeuXS2P/9ZbbxkvLy/Tq1cvc+7cOcvjAZ7q4MGDpmbNmiYkJMR8//33bhkzr/v39OnTpmvXrsbX19e8//77lscDPNmiRYuMj4+P6datmzl9+rRbxszrHv7uu+9M+fLlTa1atczBgwctjwd4qrNnz5qePXsaLy8vM2/ePLeNmZf9a4wx06ZNM5LMoEGD3HK2YmHADX2uQnp6uvr06aPXX39dMTExeuyxx9w2dlJSkjIzM1W+fPls08uXL6/Dhw9bHn/AgAH64IMP9PHHH+uOO+7Q6dOnLY8JeJqff/5ZEREROnPmjDZu3Ki6deu6Zdy87t8iRYroo48+0t13361evXrpzTfftDwm4IneeOMN9e7dW7169dKHH36oIkWKuGXcvO7hevXqadOmTTp9+rQiIiK0d+9ey2MCniYtLU133HGHPvnkE3344Yfq37+/W8bN6/6VpMcff1xvvvmmXn/9dfXt21fp6eluGbcgI1xewenTp3XHHXfoo48+0vvvv6/777/f7pJyrEePHlqxYoXWrVunjh076sSJE3aXBOSb7777TpGRkSpWrJi++uorVatWze6ScsTX11dvv/22hgwZogcffFBTp061uyQgX7344ot66KGHNGTIEM2fP1++vr52l5Qj1apV06ZNmxQQEKDIyEh99913dpcE5Jvjx4+rY8eOiouL04oVK3TnnXfaXVKODRw4UO+//74+/PBD3XnnnRyouQLC5WWcOHFCnTp10pdffqnly5frP//5j9vXERwcLG9v7wu+OP3IkSMKCQlx23puvfVWrVmzRt99953atGmjpKQkt40NXKs2b96sVq1aqXLlytqwYYMqVark1vHzq3+9vLz06quvauzYsRo1apTGjRvHF7WjwDPGaOzYsRo9erTGjRunV199VV5e7n3bkl89fN1117leg6KiorR582a3jQ1cq/7++2+1adNGP/zwg9asWaP27du7dfz86l9J+s9//qPly5dr7dq16tSpEwdqLoNweQlJSUlq06aNdu7cqTVr1qhDhw55sh4/Pz81btxYa9eudU1zOp1au3atWrZs6dZ1hYeHa/369fr99991yy236I8//nDr+MC1ZPXq1Wrfvr3q16+vL7/8UsHBwW5fR372r8Ph0HPPPacXX3xREydO1LBhw+R0Ot26DuBa4XQ6NXToUD3//POaOnWq/ve//8nhcLh9PfnZw2XLltWXX36pevXqqX379lqzZo1bxweuJX/88YfrvWZcXJzCw8Pdvo787F9J6tChg1avXq2dO3eqbdu2HKi5FLsv+rwW/fHHHyYsLMyUK1fO7NixI8/Xt2jRIuPv729iY2PNrl27zEMPPWRKlixpDh8+nCfr27NnjwkNDTXXX3+92bt3b56sA7DTRx99ZHx9fU3nzp1NWlpanq4rv/vXGGNef/1143A4TJ8+fbhRFwqcc+fOmXvvvdc4HA7zxhtv5Pn68ruH09LSzG233Wb8/PzMxx9/nCfrAOz0888/m+uvv96Ehoaan3/+OU/XZcc+eMeOHaZs2bLmpptuMn/88UeercdTES7/Ze/evaZKlSqmcuXKZs+ePfm23ldffdWEhoYaPz8/06xZM7N169Y8XV/WnTPLly9vvvvuuzxdF5Cfsu6Q3Lt373wLXvndv8YY8/777xtfX1/TtWtXt905E7Db6dOnTZcuXYyvr6/54IMP8m29+d3DZ8+eNb169XLrnTOBa0HWHZJr1qyZb3dItmMfvHv3blO5cmVTpUoV88svv+T5+jyJwxgu3Mnyww8/qH379goKCtKaNWsUGhpqd0l56q+//lLHjh3122+/6fPPP1eLFi3sLgmwZMaMGXrsscc0aNAgzZw5U97e3naXlKc+//xz9ejRQy1atNDSpUtVvHhxu0sCcu3kyZPq1q2btm7dqsWLF6tjx452l5SnMjMz9cgjj2ju3LmaMWOGHn30UbtLAizZsmWLbrvtNt14441auXKlypYta3dJeergwYNq3769Tpw4odWrV7vtTvSejmsu/7+tW7eqVatWqlChgjZu3Fjgg6UklStXTuvWrVOdOnXUrl07ffHFF3aXBOSKMUbjx4/XY489pjFjxmj27NkFPlhKUqdOnbRq1SrFx8erXbt2Sk5OtrskIFeSk5PVtm1bxcfHa/Xq1QU+WEqSt7e35syZoyeeeEIjRozQhAkTuFEXPNaaNWvUrl071a1bV19++WWBD5aSFBoaqo0bNyokJEStWrXStm3b7C7pmkC4lPTFF1+oXbt2ql27ttatW6dy5crZXVK+CQoK0qpVqxQZGanOnTvrk08+sbskIEecTqdGjBihZ599VpMmTdILL7yQJzf+uFZFRkZq3bp1+u2339SqVSv9+eefdpcE5Miff/6pW265Rfv371dcXJwiIiLsLinfOBwO1+vWM888o8cee4wbdcHjfPLJJ7r99tvVqlUrrVy5UkFBQXaXlG+yDtTcdNNNatu2bbabCxVa9p6Va7/FixcbPz8/07FjR5Oammp3ObY5e/asufvuu42Xl5eJjY21uxzgqqSnp5t+/foZh8NhXnvtNbvLsdXu3bvNddddZ2688Uazb98+u8sBrsq+ffvMDTfcYCpXrmx2795tdzm2mjNnjnE4HKZ///4mPT3d7nKAqzJv3jzj5eVlevbsac6ePWt3ObZJTU01HTp0MH5+fuaTTz6xuxxbFepwOX/+fOPt7W3uuuuuQt0QWTIyMswDDzxgJJmXX37Z7nKAyzp9+rTp3r278fHxMe+9957d5VwT9u/fb6pXr24qVKhgfvzxR7vLAS7rhx9+MBUqVDA1atQwBw4csLuca8J7771nfHx8zB133GHOnDljdznAZc2YMcNIMg8++KDJyMiwuxzbnT171tx1113G29vbvP3223aXY5tCGy5feeUVI8k88MADNMR5nE6niY6ONpLMM888Y5xOp90lARc4efKkadu2rSlSpIhZsWKF3eVcUw4fPmzq169vSpcubbZt22Z3OcBFbdu2zZQqVcrUr18/T78ywBMtX77cFClSxLRr186cPHnS7nKACzidTjNhwgQjyYwaNYr3iufJyMgwAwcONJLMK6+8Ync5tih04dLpdJpnn33WSDLR0dE0xEU4nU4zceJEI8mMGDHCZGZm2l0S4JKcnGxatGhhihcvbuLi4uwu55p07NgxEx4ebgIDA82XX35pdzlANmvXrjWBgYHm5ptvNseOHbO7nGtSXFycKV68uGnRooU5evSo3eUALpmZmebRRx81kszzzz/P++iLcDqdZuTIkUaS+d///lfotlGhCpdOp9M89thjRpKZOHFiofvPzqlZs2YZSWbAgAFc/4FrQmJioqlbt64pU6aM+fbbb+0u55p26tQpc+uttxp/f3+zdOlSu8sBjDHGLFmyxPj7+5tbb73VnDp1yu5yrmnffPONKVOmjKlbt65JTEy0uxzApKenm/79+xtJZtasWXaXc01zOp3mueeeM5LM448/XqgyR6EJlxkZGeb+++83kszMmTPtLsdjvPPOO8bb29vceeedXP8BW/3222+matWqplKlSuann36yuxyPcObMGdOjRw/j7e1t3nnnHbvLQSGXtT/5z3/+w/7kKv3000+mYsWKplq1aua3336zuxwUYmfOnDF33nmn8fb2Nu+++67d5XiMV1991UgyAwcOLDSX4RWKcMkbLGuWLl1q/P39Tfv27fmkGbbYtWuXqVSpkqlatSpvsHIoPT3dDBgwgE+aYauZM2caSeb+++8vNG+w3OXXX391fbC2a9cuu8tBIXTq1CnTvn174+/vb5YtW2Z3OR7n7bffLlQfrBX4cHn+qWFLliyxuxyP9eWXX5rAwEATHh7O9R/IV+efGvbnn3/a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tevcuXOun1evXq0aNWrom2++UXR0tFavXq3Fixfr9ttv1//+9z916NAhV0fMnE6nhg0bpk6dOql8+fKaNWuWNmzYoNmzZyswMFARERGaNWuWO59WjsybN0/NmzeX0+nU1KlTtX79es2bN0833nijunbtqieffDLfannssce0fPlyffjhh1q/fr3+/PNP3XnnndnmGTBggObMmaOMjIx8qwsAPNnF3ivMnTv3qpa9lt4rpKen211Crp09e1Zly5bVuHHjVL9+/YvOExwcrA4dOmjOnDn5XJ1FBvmqadOmxsvLy0i66n9eXl6madOmdpeOa1y/fv1Mt27dsk278847TcOGDY0xxowfP/6if1/z5s0zxhjz4YcfmrJly7qW/e233y6Yt1+/fsYYY1q1amWGDRtmRo0aZUqVKmXKly9vxo8fn23d06ZNM3Xq1DEBAQHmuuuuM4MHDzYnT540xhizbt26C8Z+6KGHjCQTHx+fq+d//fXXm4kTJ5oBAwaYwMBAU7lyZTN37tzLLtOqVSvzyCOPmEcffdSUKVPGREVFGWOM+eabb0zp0qXNsmXLLrpcenq6GTBggOnSpcsF2+vjjz82UVFRpmjRoqZevXpm8+bN2ZaNjo42TZs2NYmJiRcd+5dffjE33HCD+fDDD13Txo8fb+rXr2/efvttc/3115sSJUqYnj17mhMnTlzyuc2bN88EBQVd8vGsenfs2GGMMSY+Pt5IMtddd53Zs2fPRZf566+/TMOGDc3UqVNd0/bv329uv/12U7JkSRMQEGBuuukm8+mnn15yvddff72ZPn36JR/PkpKSYnx9fbNth4SEBCPJbNmyxTXt7Nmzxt/f33zxxRdXHBO4lHnz5hlJJj093e5SgDx1qfcKNWvWzLYvvtr3Cll+/PFH07lzZ1O8eHETGBhoIiIizC+//JJtnS+++KIJCQkxpUuXNkOGDDHnzp1zLS/JfPLJJ9nGDAoKcq03a5+1aNEic8sttxh/f3/XYzExMeamm24yfn5+JiQkxDzyyCPZxn3jjTdM9+7dTdGiRU21atXM0qVLrW1E83/vY7744gvTuHFjU7RoUdOyZUuze/fuHI/VqlUr07t374u+B5o/f7657rrrLNebnzhymY927typb7755qqPWmZxOp365ptvuIsscuTHH3/U5s2b5efnJ+mf0ysSExNd/6ZOnaqAgAA1adJEkrRx40Y1btzYtXzlypX18ccfS5L27NmjxMREvfzyy67H58+fr2LFimnbtm2aMmWKnn32Wa1Zs8b1uJeXl1555RX99NNPmj9/vr788kuNHj1akhQeHq4ZM2aoRIkSrnr69u1r+TlPmzZNTZo00Y4dOzRkyBANHjxYe/bsuewy8+fPl5+fn7766iu99tprkqRhw4Zp4sSJ6tKli3bt2qVWrVqpbNmyuvvuu/X4449rypQpeu2117Rr1y6tW7cu23hjx45VdHS0du7cqRo1aqh3796uo2q7du1SbGyslixZopCQEM2ZM0fVq1dXlSpV9Oqrr6pmzZry9fXVG2+8oVGjRmU79Xbfvn1asmSJVqxYoRUrVmj9+vWaNGmS5W2W5dixY5KkqVOnqkaNGvrkk09Up04dVaxYUePGjVP79u21e/duLVy4UBMnTtTJkyclSY888ojOnj2rDRs26IcfftDkyZMVGBhouZ74+Hilp6erXbt2rmm1atVSaGhottNz/fz81KBBA23cuNHyOgGgsMl6r+Dr6ytJ6tu3b47eK0jSoUOHdMstt8jf319ffvml4uPjdf/992c7o2TdunXat2+f1q1bp/nz5ys2NlaxsbE5rnfMmDF69NFHlZCQ4Dqq98gjj+ihhx7SDz/8oGXLlqlatWrZlnnmmWd099136/vvv9dtt92me++9V0ePHs3xui9m7NixmjZtmr799lv5+Pjo/vvvd8u4WZo1a6Y//vjjqq9vvRb42F1AYfL1119bWv6BBx5Q1apV3VQNCpqvv/5aBw4ckK+vr5xOp5xOpxwOh2688Ub17Nkz27zJycmKi4tTs2bN9L///U+StGnTJvn7+2eb96+//pIkPfHEE66QKv0Tkvz8/LRr1y6NGzdOklSqVCkNHz5c9erVc813fggoXbq0YmJilJycLEn67bffdPr0aT366KOSpNq1a1veBrfddpuGDBniqnn69Olat26datasecllqlevrilTprh+37t3r/bv368HHnhAmZmZuuOOOxQVFaWXX35ZGzdu1OOPP66xY8fKz89PvXv31qpVq9S6dWvX8tHR0ercubOkf3ZotWvX1i+//KJatWppwYIF6tevnypWrKiNGzcqOjpab7zxhmrVqqXx48dr3759cjqdatu2rTIyMrRnzx7VqlVL0j8fMsXGxqp48eKS/nkDsHbtWk2cONHydpPkCsnVq1fXvn371Lt3b02bNk0333yzZs6cqXXr1mns2LGqWbOmateura+++kodO3bUwYMH1aNHD9WtW1eSdOONN7qlnsOHD8vPz++C63LLly+vw4cPZ5tWsWJFHThwwC3rBYCCbsWKFQoMDFRGRobOnj0rLy8vPf744xo9erQCAgIUEhIi6Z97A4wbN07z589XnTp1JEkHDhxQxYoVs403a9YsBQUFadGiRa6QWqNGjWzzlCpVSjNnzpS3t7dq1aqlzp07a+3atXrwwQdzVPuIESOyXR7x3HPPaeTIka73EpLUtGnTbMv0799fvXv3liQ9//zzeuWVV/T111+rY8eOOVr3xUycOFGtWrWS9E/w7dy5s86cOaMiRYpYHluSa1sfOHDAY65xJVzmo5MnT8rb2zvXN+c5ceKE2z5pQcFz9uxZlSpVSrVq1VJmZqYOHjwoh8OhgICAbH83Z86c0ddff63Q0FAVK1bM9diZM2fk5eWVbd4TJ05I+ueoVtYOQ/rnOofAwMBs83p5een48eOuacnJydq/f7/S0tKUkZEhY4ycTqf+/vtveXt7KzU1VcYY1/w5uZnApZwfbB0Oh0JCQlwB+VL+/QnsDz/8oKZNm8rHx0e7du3SoUOHNHPmTPn6+qpBgwZatmyZa94KFSrou+++u2QNFSpUkPRPSK9Vq5Z++OEH9e/fX5K0fPly3XvvvbrnnnskSa+99pquu+66bMtmHU2U/rnLalawzHr8Ss8tJ3755RfXz6tWrdItt9yiRx55RJI0e/bsbNd9n1/b8OHDNXjwYK1evVrt2rVTjx49sm2D/FC0aFGlpaXl6zoBwFO1bt1ac+bMUWpqqqZPny4fHx+1bds22zwHDx5U9+7dFR0drbvvvts1/fTp0xcEp507dyoyMjLb+4R/q127try9vV2/V6hQQT/88EOOa886gir9s2/9888/L6j9387fJxUrVkwlSpRw2/7zUvv80NBQt4xftGhRSfKofRzhMh8VL17c0l1fo6Oj9dBDD7mxIhQk/fv3V0pKiuuW206nU/Xr11evXr1cF96npqbq5ptv1m233abFixfL4XC4lr/33ntljNF7773nmhYXF6fWrVtryZIl2Y4gRUVFqUGDBtm+UqJ79+4qWbKkYmNjtX//ftWqVUuDBw9Wz549Vbp0aW3atEkDBw7U4sWLXfONGDHCdSrt9u3b9fzzz1vaBv/esTkcjiuehl6sWLFsv2dkZLhezM+dOydfX99s455/yuf27dsvOCp6/rxZ2zerhn+Pff66zx83NTVVe/fuzXamQm6eW06c/9r079r8/PxcR66dTqd27typUaNGSfrnjIoOHTro008/1erVq/XCCy9o2rRplm+fHhISonPnziklJSXb396RI0dcn6pnOXr0KGd1AMBVKlasmOvU0bfeekv169fPdjQyNTVVXbt2VcuWLfXss89mWzY4ODjbB5/S/wWgy7nSPszhcFxwF/aL3bDn/H3T1az3atZtxeX2+e6Q9QF82bJl3TZmXuOay3zUrFkzW5dH4eLl5aWnnnpK48aN0+nTp2WMUZ8+feR0OvXOO+9kC5aS1LBhQ+3atSvbtKxAkdMPReLj4+V0OjVt2jS1aNFCNWrU0J9//nnB2NfiV+xUq1bN9Wlq1jWQM2fOVGZmprZu3apVq1YpPT1d8+fP1+eff+46EpnTsSMiIrRo0SLt3r1b6enprtNb//77b91///3q1q2bypUr5/bndymVK1d2/RwREaHVq1dr69atyszM1MyZM5WSkqITJ05o5MiRqlSpUrbTjipXrqxBgwZp8eLFGjlypN544w3L9TRu3Fi+vr5au3ata9qePXt08OBBtWzZMtu8P/74oxo2bGh5nQBQ2GS9V5g9e7Yk5eq9Qr169bRx40ZLd28tW7asEhMTXb/v3bv3ikfrihcvripVqmTbTxQ0P/74o3x9fd1y6VB+IVzmowYNGqhp06by8srZZvfy8lLTpk3VoEGDvCkMBdZdd90lb29vzZo1SxMmTNAXX3yhuXPn6tSpUzp8+LAOHz6s06dPS5I6dOign376Kdsnktdff70cDodWrFihv//+W6dOnbqq9VarVk3p6el69dVX9euvv+qdd95x3SwnS5UqVXTq1CmtXbtWSUlJrjryUtu2bTVz5szLztOwYUOdPn1a69atU9GiRRUbG6v//ve/8vf314ABA9S9e3dNnjxZ8+bN0+rVq3P0aeIdd9yhN998U+np6erRo4e6du2qm266SQEBAUpJSVHFihXVrl07VapU6YLtdSUzZ8687KlBX3/9tWrVqqVDhw5d9PGsa0aOHz+uJk2aaMyYMYqMjJS/v79Wr16txo0bq1evXjp27Jg++eQT13IjRozQqlWr9Ntvv2n79u1at26dwsLCXI/XqlUr2/xXKygoSAMHDtTjjz+udevWKT4+XgMGDFDLli3VokUL13z79+/XoUOHst34BwBw9bLeK0jS3Llzc/xeYejQoTpx4oR69eqlb7/9Vnv37tU777xzxRvqna9NmzaaOXOmduzYoW+//VaDBg267Gm2WSZMmKBp06bplVde0d69e7V9+3a9+uqrOdwC9ti5c6d27typU6dOubbnv7/TcuPGjYqMjLzqo7TXAsJlPhs+fHiu7hY7fPjwPKoIBZmPj4+GDh2qKVOm6LPPPtOpU6cUHh6uChUquP69//77kqS6deuqUaNG+uCDD1zLV6pUSc8884zGjBmj8uXLa+jQoVe13vr16+ull17S5MmTVadOHS1YsEAvvPBCtnnCw8M1aNAg9ezZU2XLltXbb7/tvid+Cfv27VNSUtJl53E4HJo8ebL69eun/fv367bbbtPff/+tAwcOaNeuXZo9e7ZSUlIUFxeX408SW7durWrVqunBBx+U0+nU3Llzdfz4cR05ckSvv/66vv32Wx09elQvvfRSjm8GkJSUpH379l3y8bS0NO3Zs+eSnyxnHbl86qmnlJaWpqefflonTpzQn3/+qWXLlumzzz5TSkqKYmNjs52mmpmZqUceeURhYWHq2LGjatSo4foEXPrnaOPx48dz9FyyTJ8+Xbfffrt69OihW265RSEhIVq8eHG2eRYuXKhbb71V119/fa7WAQCFnY+Pj+u6yq+++irH7xXKlCmjL7/8UqdOnVKrVq3UuHFjvfHGG1cVDrNMmzZNlStXVmRkpO655x5FR0crICDgisv169dPM2bM0OzZs1W7dm3dfvvt2rt3bw63gD0aNmyohg0bKj4+XitXrpSkC97vL1q0KMc3PbKdjV+DUihlZGSY7t27X/V3XXp5eZk77rjDZGRk2F06CoEVK1aYsLAwk5mZme/rzvqexdx+z6W7TZw40ZQpU8ZMnTrV/P7778YYY86cOWNWrVplIiIizOLFi3M17tGjR02LFi1MixYtzPLly01qaqoxxpgjR46Yl156yTRo0MCcOnXKbc/jamVt/1atWpmwsDCzcOFCk5KSYowx5tixYyYmJsbUrl3btS2uBWfPnjWhoaFm06ZNdpcCD8f3XKKwy8k+2M73CgXVxbb/Z599ZsLCwjzudYkjl/nM29tb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f38NGDBA3bt31+TJkzVv3jytXr06R0fM7rjjDr355ptKT09Xjx491LVrV910000KCAhQSkqKKlasqHbt2qlSpUoXbK8rmTlz5mVP7/v6669Vq1Yt12nQF/PFF1/o6NGjatKkicaMGaPIyEj5+/tr9erVaty4sXr16qVjx45luzPriBEjtGrVKv3222/avn271q1bp7CwMNfjtWrVyvWdXA8fPqydO3e6Qu8PP/ygnTt3ZvvakbS0NMXHx+vWW2/N1TpgTdZrzAcffCBJevrppzV8+HB16tRJCxYs0Pvvv5/tzscdOnTQli1bsn2w9OSTT+qbb77RkCFD9P3332v37t2aM2eOkpKSrqqGokWLqkWLFq4b9axfv17jxo274nJFihTRE088odGjR+vtt9/Wvn37tHXrVsXExORwK+S/yZMn6+mnn9Zbb72lKlWquLbVv08P37hxo8f1BuESAHJg+PDhubpb7PDhw/OoIhRkPj4+Gjp0qKZMmaLPPvtMp06dUnh4uCpUqOD69/7770uS6tatq0aNGrneJEpSpUqV9Mwzz2jMmDEqX778BUchLqV+/fp66aWXNHnyZNWpU0cLFizQCy+8kG2e8PBwDRo0SD179lS7du3c96QvY9++fVd8w+pwODR58mT169dP+/fv12233aa///5bBw4c0K5duzR79mylpKQoLi7ugpuOXEnr1q1VrVo1Pfjgg3I6nZo7d66OHz+uI0eO6PXXX9e3336ro0eP6qWXXrrgurQrSUpK0r59+y75eFpamvbs2XPJ0wUlqV27durdu7fS0tL09NNP68SJE/rzzz+1bNkyffbZZ0pJSXF9hUKWzMxMPfLIIwoLC1PHjh1Vo0aNbDdm2bNnj44fP56j55LltddeU8OGDfXggw9Kkm655RY1bNgw23WvS5cuVWhoqCIjI3O1DliT9Rrz9ttvS/on6D3//POS/nlNef755/Xwww+7PtTo1KmTfHx89MUXX7jGqFGjhlavXq3vvvtOzZo1U8uWLbV06VL5+Fz91XdvvfWWMjIy1LhxY40YMULPPffcVS339NNPa+TIkfrvf/+rsLAw9ezZ0+3XMueFOXPm6Ny5c/rPf/6jChUquL5G6Z133nHNc+jQIW3evFkDBgywq8zcMQVEfHy8kWTi4+PtLqVQYvujsMjIyDDdu3c3Xl5eRtIV/3l5eZk7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Qzt37sw2/eWXX1ZsbKxb1vFvVapUybOxc8oYo//+97+qUKGCihYtqnbt2mnv3r2ux4ODg3Xfffdp/PjxNlaJwupSH/LExcXJ4XAoJSUl32sCcPXoYcBz0b/XJrcduezYsaMSExP166+/avr06Zo7d26O3vAfPHhQK1asUP/+/d1Vksu5c+fcPublhISEyN/fP0/XERQUpJIlS+bpOq4FU6ZM0SuvvKLXXntN27ZtU7FixdShQ4dsH1wMGDBACxYs0NGjR22sFAAAACjc3BYu/f39FRISosqVK6t79+5q166d1qxZI0l6++23FRgYmO2I05AhQ1SrVi2lpaVJkj744APVr19flSpVuuK61q9fr2bNmsnf318VKlTQmDFjlJGR4Xo8KipKQ4cO1YgRIxQcHKwOHTpIkpYtW6bq1aurSJEiat26tebPn5/tk43k5GT17t1blSpVUkBAgOrWrauFCxdmW3dUVJSGDx+u0aNHq3Tp0goJCdGECROyzXP+abETJkxwHdU9/1/WkcGVK1cqIiJCJUuWVJkyZXT77bdr3759rrFuuOEGSVLDhg3lcDgUFRUl6cJPa86ePavhw4erXLlyKlKkiCIiIvTNN9+4Hs/6FGft2rVq0qSJAgICFB4erj179kiSYmNjXbUdOHBAAwYMyLa+y+nfv78ef/xxSdKtt96qMmXK6JFHHlF6evoVl70cY4xmzJihcePGqVu3bqpXr57efvtt/fnnn9lOO65du7YqVqyoTz75xNL6AAAAAORenlxz+eOPP2rz5s3y8/OTJN1333267bbbdO+99yojI0Offvqp3nzzTS1YsEABAQGSpI0bN6pJkyZXHPvQoUO67bbb1LRpU3333XeaM2eOYmJiFBMTk22++fPny8/PT1999ZVee+01/fbbb/rPf/6j7t2767vvvtPDDz+ssWPHZlvmzJkzaty4sT799FP9+OOPeuihh9S3b199/fXXF4xdrFgxbdu2TVOmTNGzzz7rCtL/Fh0drcTERNe/qVOnKiAgwPVcU1NT9fjjj+vbb7/V2rVr5eXlpTvuuENOp1OSXOv+4osvlJiYqMWLF190PaNHj9bHH3+s+fPna/v27apWrZo6dOhwwdG8sWPHatq0afr222/l4+Oj+++/X5LUs2dPV43XXXedZsyYcdn1/du3334rSZo7d67mz5+v2NhYy6fW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55+XJD3zzDPy8PBQx44ddenSpXtuey/NmjXTf/7zH7Vt2/aO6zg6Oqp58+ZasmSJ6f4AAAAAZEyW3XO5f/9+ffvtt3JxcZH072WccXFx9q8JEybI1dVVTzzxhCQpKipKtWvXvme7iYmJCgkJUZEiRbR79259+eWX2rJliz744IM064WHh+vQoUPavHmz1q5dq4sXL6ply5aqVq2a9u7dq3fffVfDhg1Ls01qaqoeeughffnllzpw4IBGjBihN998U8uWLUuz3rZt23T06FFt27ZN8+fP17x58+wh+WahoaFp3vfixYvl5OSkevXqSZIuXbqk7t27Kzo6Wt9//70qVaqk5s2b24PZ7t27JUlz585VXFyc/eebffzxx5o4caImTJign3/+WSEhIWrVqpWOHDmSZr233npLYWFhiomJ0SOPPKLnn39eycnJ8vf3t9fo5+enIUOG3LW/m/3xxx+SpMmTJ2vt2rWKjIzUuHHj7mvbzPDkk08qKioq2/oDAAAAkJZTZja2du1aubm5KTk5Wf/8848cHBw0depUSf9exunm5iZJ+v777/X2229r/vz5qlq1qiTpxIkTKlmy5D37+OKLL3T16lV9/vnnKly4sCRp6tSpatmyZZr1ChcurE8//dQebmfMmCGbzabZs2erYMGCqlKlik6dOqXevXvbt3F2dtbo0aPtP5cvX17fffedli1bpueee86+vEiRIpo6daocHR316KOPqkWLFgoPD0/T1nWFChVSoUKFJElHjx7Vyy+/rPfee09NmjSRJDVq1CjN+rNmzZKnp6ciIyP1zDPPqFixYpIkT09P+fj43HG/TJgwQcOGDVPHjh0lSR988IG2bdumyZMnp7mkNCwsTC1atJAkjR49Wo899ph+/fVXPfroo/b2XVxc5Obmdtf+bnb9fseKFSuqVq1a6tq1q8LDwzV27Nj7bsOMkiVL6vfff1dqaqocHHLUPFUAgBzs+meXG6WkpFhUDQDkbpn6Kbxhw4aKiYnRzp071b17d/Xs2VPt27dPs87JkyfVpk0bhYWFpQlsV65cUcGCBdOs+9hjj9lDabNmzSRJsbGxql69uj1YSlK9evVumcylWrVq9mApSYcOHdLjjz+epo8nn3zylvcwbdo01a5dW8WKFZObm5tmzZqlkydP3lKXo6Oj/ecSJUro77//vuu+uXDhgp555hm1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pjlz5iglJUV+fn5ycXGxuqR0KVCggBo0aKA///zT6lLS7ffff9exY8d08uRJwiUybN26dVq0aJE8PT1VvXp1q8tJt8qVK0uS/vjjD4srSb8ffvhBiYmJCgwMJFwCAABUqFBBy5cvV2hoqDw8PLRixQq5urpaXVaet3fvXoWEhKhq1apaunSp1eUgF3v99dd16NAhLViwQB07dlTfvn2tLinPMwxD48aNU2RkpF599VX17t3b6pIyRe689gMAAOQobdq00bp16xQVFaWQkBBduHDB6pLytO3bt6thw4aqUKGCIiMjVaJECatLQi7m5OSkuXPnasCAAerXr5/GjRtndUl5mmEYGjZsmN58802NHj1aH330Ua69JP9meeNdAAAAyzVu3FhbtmzRL7/8ooYNG+rvv/+2uqQ8ad26dQoJCVGdOnW0ZcsWFS1a1OqSkAc4ODjo448/1ogRI/TGG29o+PDhMgzD6rLynJSUFPXp00fjx4/X5MmTNWLECNlsNqvLyjSESwAAkGmeeuopRUZGKi4uTvXr19fvv/9udUl5ytKlS9W6dWuFhIRo7dq1cnNzs7ok5CE2m81+Ju2DDz5Q//79lZKSYnVZeca1a9fUuXNnzZkzR/PmzdMrr7xidUmZjnAJAAAyVbVq1RQVFaV//vlHAQEBOnz4sNUl5QmzZs3S888/r06dOmn58uUqWLCg1SUhj3rttdc0Z84czZo1S127dlVSUpLVJeV6ly9fVps2bfTVV1/pyy+/zLMTcBEuAQBApqtYsaKio6NVuHBhBQYGKiYmxuqScrUPP/xQffr00YABAzR37lw5OTEnI7JWr169tGzZMi1fvlxt27bVlStXrC4p17pw4YJCQkIUGRmpb775Ru3atbO6pCxDuAQAAFmiVKlS2r59u0qXLq2goCDt2LHD6pJyHcMw9MYbb2jYsGF655139PHHH+eZiT+Q87Vv315ff/21tm3bpqZNm+rixYtWl5Tr/Pe//1XDhg21f/9+bdmyRcHBwVaXlKX47QQAALKMt7e3tm7dqho1aujpp5/Wpk2brC4p10hNTVX//v01btw4TZw4UWPGjMlTE38gdwgJCdHmzZv1008/qVGjRoqPj7e6pFzj999/V2BgoP78809FRkbKz8/P6pKyHOESAABkKXd3d61fv14NGzbUM888o+XLl1tdUo6XlJSkrl27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evLJJzV58mQlJiaqZ8+eGWrv/PnzeuaZZxQTE6P169erUaNGpuoD8pKHH35Y0dHRatKkierXr6+NGzeqZs2aGW4vs49fSdq+fbueeeYZValSRevWrVPRokUz3FZ+RLgEAAC5hoODgyZPnqwiRYrojTfe0Pnz5/X+++9n+F7G0NBQ/fe//9WIESN0+vRp1ahRQxs2bLhlkpD78ffffyskJEQnTpxQeHi46tatm6GagLysZMmS2r59u5o1a6agoCCtXbtWgYGBGWorM49fSfrmm2/UoUMH1atXT6tWrZKbm1uG2snPbIZhGFYXAQC5WXJyspydnTV37lz16NHD6nKAfGPy5Ml67bXX1LdvX02dOtXSx3ucPHlSTZo00aVLl7Rp0yZVrVrVslqA3ODSpUtq3bq1vv/+e61cuVJNmza1tJ4lS5aoa9euatGihZYsWaKCBQtaWk9uxT2XAAAgV3r11Vf12WefadasWeratauSkpIsqePQoUMKCAhQUlKSoqKiCJbAfXjggQe0bt06BQcHq1WrVlq2bJlltcycOVOdOnVSp06dtHz5coKlCYRLAACQa/Xs2VPLli3T8uXL1bZtW125ciVb+//xxx8VGBioBx54QFFRUapQoUK29g/kZgULFtSKFSv03HPPqWPHjvr000+zvYYPPvhAffv21YABAzR37lw5OXHXoBmESwAAkKu1b99ea9eu1bZt29S0aVNdvHgxW/rdsWOHGjZsqLJly2r79u0qVapUtvQL5CXOzs76/PPP1a9fP/Xu3VsTJkzIln4Nw9Abb7yh4cOH65133tHHH38sBweikVnsQQAAkOs9/fTT2rx5s3766Sc1atRI8fHxWdrfhg0b1KRJE9WsWVPh4eHy8vLK0v6AvMzBwUFTp07Vm2++qaFDh+rtt99WVk4Lk5qaqv79+2vcuHH66KOPNGbMmAxPCoa0CJcAACBP8Pf3V2RkpH7//XfVr19ff/zxR5b08+WXX6pVq1YKDg7WunXr5O7uniX9APmJzWbT2LFj9eGHH2rs2LEaOHCgUlNTM72fpKQkdenSRbNmzdKcOXP02muvZXof+RnhEgAA5BnVq1dXVFSUEhMTFRAQoF9//TVT258zZ446duyoZ599VitWrFChQoUytX0gvxs6dKhmzZqlTz75RN27d8/UibquXLmitm3bavny5Vq6dKl69eqV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CJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0/4fk4tDYlznoo8AAAAASUVORK5CYII=",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA5cAAAP7CAYAAADPo3rEAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAADba0lEQVR4nOzdeVhUdf//8dewKqK4oKImWa7kvitB4paauZR3qaWp2aKmZolmabfWnaWmaeWSFYmVaZu5VS6ZuORSobaJZpZahhYoLuACzOf3Rz/mK7nCGTgOPB/X5XXBmXM+5z1H3nPmNWcZhzHGCAAAAAAAC7zsLgAAAAAA4PkIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJcAAAAAAMsIlwAAAAAAywiXAAAAAADLCJfXiO+++06bN2+2uwwAubRgwQKdOHHC7jIA5MKJEye0YMECu8sAkEtfffWVvv/+e7vLgAiX14TNmzcrKipK7dq106pVq+wuB0AOGGM0duxY9enTR23atFFSUpLdJQHIgb///lutW7dWnz59NG7cOBlj7C4JQA6sXLlS7du3V6tWrbRlyxa7yyn0CJc2W7Nmjdq3b6969eqpTZs26tKliz766CO7ywJwFZxOp4YOHarnn39ejz/+uH7//XfdcsstOnTokN2lAbgKf/zxh2655Rb98ccfevzxxzVx4kQNGzZMTqfT7tIAXIUPP/xQXbt2Vdu2bVW3bl21a9dOa9assbusQo1waaOPP/5YnTt3VuvWrbVy5Up98sknuuuuu9SzZ0+99dZbdpcH4DLS09PVr18/zZkzR2+88YamTZumjRs3KjU1VREREfrll1/sLhHAZfzyyy+KiIhQWlqaNm3apGnTpun111/X7Nmz1a9fP6Wnp9tdIoDLiImJUa9evXTXXXdp8eLFWrlypaKionT77bdr8eLFdpdXeBnY4q233jJeXl6mV69e5ty5c67pmZmZZtCgQUaSeemll2ysEMClnD592nTt2tX4+vqa999/P9tjBw8eNDVr1jTly5c333//vU0VAric7777zpQvX97UrFnTHDx4MNtjixYtMj4+PqZr167m9OnTNlUI4HKmTZtmJJnBgwebzMxM1/SzZ8+anj17Gi8vLzNv3jz7CizECJc2mD59upFkHn74YZORkXHB406n0zz55JNGknn66aeN0+m0oUoAF3PixAnTunVrU7RoUfP5559fdJ4jR46Yhg0bmlKlSpktW7bkc4UALmfz5s2mZMmSplGjRuavv/666DyfffaZKVq0qGnTpo05ceJEPlcI4FKcTqcZN26ckWSefPLJi75HzsjIMA899JCRZGbMmGFDlYUb4TIfOZ1O89///tdIMk888cQVQ+OkSZOMJDNs2LBsn8oAsEdSUpJp2rSpKVGihNm4ceNl501JSTERERGmWLFiZs2aNflUIYDLWbNmjQkICDCRkZEmJSXlsvNu2LDBlChRwjRr1swkJyfnU4UALiUzM9MMHTrUSDKTJ0++7LxOp9OMHj3aSDLjx4/nQE0+Ilzmk8zMTDN8+HAjybzwwgtXvdxrr71mHA6Hue+++0x6enoeVgjgcg4dOmRq165typYta+Lj469qmdTUVNOxY0fj5+dnFi9enMcVAricxYsXGz8/P9OpUyeTmpp6VcvEx8eb4OBgU7t2bXPo0KE8rhDApaSnp5u+ffsah8Nh5s6de9XLvfDCC0aSefTRRzlQk08Il/kgPT3d9OvXzzgcDjNnzpwcL79w4ULj4+NjunfvzvUfgA327dtnbrjhBnPdddeZ3bt352jZs2fPmrvvvtt4e3ub+fPn51GFAC4nNjbWeHl5mZ49e5qzZ8/maNmEhARz3XXXmRtvvNH8+uuveVQhgEs5ffq06datm/Hx8TGLFi3K8fKzZ882DofD9O/fnwM1+YBwmcfOnDljunfvbnx8fMx7772X63FWrFhhihQpYtq2bWtOnjzpxgoBXM6PP/5oKlSoYKpXr27279+fqzEyMjLMAw88YCSZV155xc0VAricl19+2UgyDz744EXvc3A19u/fb6pVq2YqVKhgfvzxRzdXCOBSTpw4Ydq0aWOKFCliPv3001yPs2DBAuPt7W3uuOMOc+bMGTdWiH8jXOahkydPmnbt2pkiRYqY5cuXWx5v/fr1pnjx4qZ58+Zc/wHkg23btpnSpUub+vXrm8OHD1say+l0mujoaCPJPPPMM1z/AeQxp9NpJkyYYCSZUaNGWe65w4cPm3r16pnSpUubr7/+2k1VAriU5ORk06xZM1O8eHGzfv16y+MtW7bM+Pv7m/bt23OgJg85jDEm/78ApeA7evSoOnfurJ9++knLly9Xq1at3DJufHy8OnTooAoVKmj16tWqUKGCW8YFkN26devUtWtX1atXT59++qlKlixpeUxjjF544QWNHTtWjz32mKZNmyaHw2G9WADZOJ1OjRw5UjNmzNDzzz+vMWPGuKXXjh07ps6dO+uHH37QsmXL1Lp1azdUC+DfEhMTdeutt+rw4cNauXKlGjdu7JZx4+Li1KVLF9WpU0efffaZSpUq5ZZx8X8Il3ng8OHDuvXWW/Xnn39q5cqVatKkiVvHT0hIUPv27VWkSBGtWbNGN9xwg1vHBwq7ZcuW6e6771arVq20ePFiFStWzK3jz549W4888ogGDBig119/XT4+Pm4dHyjMMjIy9OCDDyo2NlazZs3SkCFD3Dp+amqq7rjjDm3YsEEffvihunTp4tbxgcLut99+U7t27XT27Fl98cUXqlWrllvH/+abb9SxY0ddd911WrVqlUJCQtw6fmHnZXcBBc3+/fsVERGh5ORkbdiwwe3BUpLCwsK0adMmSVJERIR27drl9nUAhdW7776rO++8U7fffruWLVvm9mApSUOGDNE777yjt99+W7169dLZs2fdvg6gMDp79qx69uypd955R++++67bg6UkFStWTMuXL1fnzp11xx13aMGCBW5fB1BY7dq1SxEREfLy8tKmTZvcHiwlqWnTptqwYYOSkpIUGRmpAwcOuH0dhRnh0o0SEhIUEREhSdq0aZNuuummPFtXlSpVtGnTJpUpU0a33HKLvv322zxbF1BYzJo1S3379tV9992nRYsWyd/fP8/W1adPHy1evFgrVqxQ165dlZqammfrAgqD1NRUdenSRZ9++qk++eQT3XvvvXm2Ln9/f73//vvq27ev+vbtq9mzZ+fZuoDC4ptvvtEtt9yi4OBgbdy4UVWqVMmzddWuXVubNm2S0+nUzTffrISEhDxbV2FDuHST+Ph4RUZGqlSpUtq4cWO+nKoaEhKiuLg4Va9eXW3atNH69evzfJ1AQWSM0fPPP6+hQ4fqscce05tvvpkvp6p27dpVn3/+uTZv3qxbb71VKSkpeb5OoCA6duyY2rdvry1btujzzz/Pl1NVfXx8FBMTo0cffVSPPPKIXnjhBXGlEZA7cXFxatOmjWrUqKG4uLh8OVX1hhtu0KZNm1SqVCndcsst2r59e56vszAgXLrBhg0b1Lp1a1WrVk3r16/P15vslC5dWmvWrFGzZs3UsWNHrVixIt/WDRQExhiNHj1aY8eO1bPPPqtp06bJyyv/Xhpbt26ttWvXavfu3YqKitKRI0fybd1AQXDkyBFFRUVpz549+vLLL/P1JjteXl566aWX9Mwzz+ipp57SE088QcAEcmj58uXq2LGjWrRoodWrV+frTXYqVKig9evXq2rVqmrdurU2bNiQb+susGy7T20Bca18/+SZM2fMHXfcYfn7NIHC5Fr6/kl3fJ8mUNhcS98/6Y7v0wQKm6zvn7zzzjtt/f7JkydPuuX7NGEMRy4tWLhwobp37+46YhgYGGhbLf7+/vrggw9077336t5779Vrr71mWy2AJzh37pzuuecezZs3T/Pnz9ewYcNsrSfr+o+MjAxFRERo9+7dttYDXOt2796tiIgIOZ1Obdq0SbVr17a1nuHDhys2NlYxMTG69957de7cOVvrAa51c+bMUZ8+fdS3b1+9//77eXqfgysJDAzUp59+qg4dOqhbt25atGiRbbV4PLvTrad67bXXjMPhMPfdd59JT0+3PN7MmTPN9ddfb/z9/U2zZs3Mtm3bcjVOZmamGT58uJFkXnjhBct1AQVRamqq6dixo/Hz8zOffPKJ5fHc1b/GGHPo0CFTu3ZtU7ZsWbN9+3bLtQEFUXx8vAkODja1a9c2f/75p+Xx3NnDixcvNn5+fqZTp04mNTXVcm1AQfT8888bSebRRx81mZmZlsZyZ/+mp6ebvn37GofDYebOnWuprsKKcJkLkyZNMpLMsGHDLDeEMcYsWrTI+Pn5mbfeesv89NNP5sEHHzQlS5Y0R44cydV4TqfTjB8/3kgyTzzxhHE6nZZrBAqKlJQUExERYYoVK2bWrFljeTx3968xxiQlJZmmTZuaEiVKmA0bNliuEShINmzYYEqUKGGaNWtmkpKSLI+XFz28Zs0aU6xYMRMZGWlSUlIs1wgUFE6n04wePdpIMhMmTLD8HjUv+jczM9MMHTrUSDKTJ0+2VF9hRLjMAafTacaMGWMkmf/+979uC23NmjUzjzzyiOv3zMxMU7FiRctHHqdPn24kmYcffpjrPwBjzJEjR0zDhg1NyZIlzZYtW9wyZl7174kTJ0zr1q1N0aJFzeeff261TKBA+Oyzz0yRIkVMmzZtzIkTJ9wyZl718ObNm03JkiVNw4YNzV9//WW1TMDjZWRkmIceeshIMjNmzHDLmHnVv06n0zz99NNGkhkzZgwHanKAcHmVMjMzzaBBg4wk89JLL7lt3LNnzxpvb+8LTs277777TNeuXS2P/9ZbbxkvLy/Tq1cvc+7cOcvjAZ7q4MGDpmbNmiYkJMR8//33bhkzr/v39OnTpmvXrsbX19e8//77lscDPNmiRYuMj4+P6datmzl9+rRbxszrHv7uu+9M+fLlTa1atczBgwctjwd4qrNnz5qePXsaLy8vM2/ePLeNmZf9a4wx06ZNM5LMoEGD3HK2YmHADX2uQnp6uvr06aPXX39dMTExeuyxx9w2dlJSkjIzM1W+fPls08uXL6/Dhw9bHn/AgAH64IMP9PHHH+uOO+7Q6dOnLY8JeJqff/5ZEREROnPmjDZu3Ki6deu6Zdy87t8iRYroo48+0t13361evXrpzTfftDwm4IneeOMN9e7dW7169dKHH36oIkWKuGXcvO7hevXqadOmTTp9+rQiIiK0d+9ey2MCniYtLU133HGHPvnkE3344Yfq37+/W8bN6/6VpMcff1xvvvmmXn/9dfXt21fp6eluGbcgI1xewenTp3XHHXfoo48+0vvvv6/777/f7pJyrEePHlqxYoXWrVunjh076sSJE3aXBOSb7777TpGRkSpWrJi++uorVatWze6ScsTX11dvv/22hgwZogcffFBTp061uyQgX7344ot66KGHNGTIEM2fP1++vr52l5Qj1apV06ZNmxQQEKDIyEh99913dpcE5Jvjx4+rY8eOiouL04oVK3TnnXfaXVKODRw4UO+//74+/PBD3XnnnRyouQLC5WWcOHFCnTp10pdffqnly5frP//5j9vXERwcLG9v7wu+OP3IkSMKCQlx23puvfVWrVmzRt99953atGmjpKQkt40NXKs2b96sVq1aqXLlytqwYYMqVark1vHzq3+9vLz06quvauzYsRo1apTGjRvHF7WjwDPGaOzYsRo9erTGjRunV199VV5e7n3bkl89fN1117leg6KiorR582a3jQ1cq/7++2+1adNGP/zwg9asWaP27du7dfz86l9J+s9//qPly5dr7dq16tSpEwdqLoNweQlJSUlq06aNdu7cqTVr1qhDhw55sh4/Pz81btxYa9eudU1zOp1au3atWrZs6dZ1hYeHa/369fr99991yy236I8//nDr+MC1ZPXq1Wrfvr3q16+vL7/8UsHBwW5fR372r8Ph0HPPPacXX3xREydO1LBhw+R0Ot26DuBa4XQ6NXToUD3//POaOnWq/ve//8nhcLh9PfnZw2XLltWXX36pevXqqX379lqzZo1bxweuJX/88YfrvWZcXJzCw8Pdvo787F9J6tChg1avXq2dO3eqbdu2HKi5FLsv+rwW/fHHHyYsLMyUK1fO7NixI8/Xt2jRIuPv729iY2PNrl27zEMPPWRKlixpDh8+nCfr27NnjwkNDTXXX3+92bt3b56sA7DTRx99ZHx9fU3nzp1NWlpanq4rv/vXGGNef/1143A4TJ8+fbhRFwqcc+fOmXvvvdc4HA7zxhtv5Pn68ruH09LSzG233Wb8/PzMxx9/nCfrAOz0888/m+uvv96Ehoaan3/+OU/XZcc+eMeOHaZs2bLmpptuMn/88UeercdTES7/Ze/evaZKlSqmcuXKZs+ePfm23ldffdWEhoYaPz8/06xZM7N169Y8XV/WnTPLly9vvvvuuzxdF5Cfsu6Q3Lt373wLXvndv8YY8/777xtfX1/TtWtXt905E7Db6dOnTZcuXYyvr6/54IMP8m29+d3DZ8+eNb169XLrnTOBa0HWHZJr1qyZb3dItmMfvHv3blO5cmVTpUoV88svv+T5+jyJwxgu3Mnyww8/qH379goKCtKaNWsUGhpqd0l56q+//lLHjh3122+/6fPPP1eLFi3sLgmwZMaMGXrsscc0aNAgzZw5U97e3naXlKc+//xz9ejRQy1atNDSpUtVvHhxu0sCcu3kyZPq1q2btm7dqsWLF6tjx452l5SnMjMz9cgjj2ju3LmaMWOGHn30UbtLAizZsmWLbrvtNt14441auXKlypYta3dJeergwYNq3769Tpw4odWrV7vtTvSejmsu/7+tW7eqVatWqlChgjZu3Fjgg6UklStXTuvWrVOdOnXUrl07ffHFF3aXBOSKMUbjx4/XY489pjFjxmj27NkFPlhKUqdOnbRq1SrFx8erXbt2Sk5OtrskIFeSk5PVtm1bxcfHa/Xq1QU+WEqSt7e35syZoyeeeEIjRozQhAkTuFEXPNaaNWvUrl071a1bV19++WWBD5aSFBoaqo0bNyokJEStWrXStm3b7C7pmkC4lPTFF1+oXbt2ql27ttatW6dy5crZXVK+CQoK0qpVqxQZGanOnTvrk08+sbskIEecTqdGjBihZ599VpMmTdILL7yQJzf+uFZFRkZq3bp1+u2339SqVSv9+eefdpcE5Miff/6pW265Rfv371dcXJwiIiLsLinfOBwO1+vWM888o8cee4wbdcHjfPLJJ7r99tvVqlUrrVy5UkFBQXaXlG+yDtTcdNNNatu2bbabCxVa9p6Va7/FixcbPz8/07FjR5Oammp3ObY5e/asufvuu42Xl5eJjY21uxzgqqSnp5t+/foZh8NhXnvtNbvLsdXu3bvNddddZ2688Uazb98+u8sBrsq+ffvMDTfcYCpXrmx2795tdzm2mjNnjnE4HKZ///4mPT3d7nKAqzJv3jzj5eVlevbsac6ePWt3ObZJTU01HTp0MH5+fuaTTz6xuxxbFepwOX/+fOPt7W3uuuuuQt0QWTIyMswDDzxgJJmXX37Z7nKAyzp9+rTp3r278fHxMe+9957d5VwT9u/fb6pXr24qVKhgfvzxR7vLAS7rhx9+MBUqVDA1atQwBw4csLuca8J7771nfHx8zB133GHOnDljdznAZc2YMcNIMg8++KDJyMiwuxzbnT171tx1113G29vbvP3223aXY5tCGy5feeUVI8k88MADNMR5nE6niY6ONpLMM888Y5xOp90lARc4efKkadu2rSlSpIhZsWKF3eVcUw4fPmzq169vSpcubbZt22Z3OcBFbdu2zZQqVcrUr18/T78ywBMtX77cFClSxLRr186cPHnS7nKACzidTjNhwgQjyYwaNYr3iufJyMgwAwcONJLMK6+8Ync5tih04dLpdJpnn33WSDLR0dE0xEU4nU4zceJEI8mMGDHCZGZm2l0S4JKcnGxatGhhihcvbuLi4uwu55p07NgxEx4ebgIDA82XX35pdzlANmvXrjWBgYHm5ptvNseOHbO7nGtSXFycKV68uGnRooU5evSo3eUALpmZmebRRx81kszzzz/P++iLcDqdZuTIkUaS+d///lfotlGhCpdOp9M89thjRpKZOHFiofvPzqlZs2YZSWbAgAFc/4FrQmJioqlbt64pU6aM+fbbb+0u55p26tQpc+uttxp/f3+zdOlSu8sBjDHGLFmyxPj7+5tbb73VnDp1yu5yrmnffPONKVOmjKlbt65JTEy0uxzApKenm/79+xtJZtasWXaXc01zOp3mueeeM5LM448/XqgyR6EJlxkZGeb+++83kszMmTPtLsdjvPPOO8bb29vceeedXP8BW/3222+matWqplKlSuann36yuxyPcObMGdOjRw/j7e1t3nnnHbvLQSGXtT/5z3/+w/7kKv3000+mYsWKplq1aua3336zuxwUYmfOnDF33nmn8fb2Nu+++67d5XiMV1991UgyAwcOLDSX4RWKcMkbLGuWLl1q/P39Tfv27fmkGbbYtWuXqVSpkqlatSpvsHIoPT3dDBgwgE+aYauZM2caSeb+++8vNG+w3OXXX391fbC2a9cuu8tBIXTq1CnTvn174+/vb5YtW2Z3OR7n7bffLlQfrBX4cHn+qWFLliyxuxyP9eWXX5rAwEATHh7O9R/IV+efGvbnn3/a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tevcuXOun1evXq0aNWrom2++UXR0tFavXq3Fixfr9ttv1//+9z916NAhV0fMnE6nhg0bpk6dOql8+fKaNWuWNmzYoNmzZyswMFARERGaNWuWO59WjsybN0/NmzeX0+nU1KlTtX79es2bN0833nijunbtqieffDLfannssce0fPlyffjhh1q/fr3+/PNP3XnnndnmGTBggObMmaOMjIx8qwsAPNnF3ivMnTv3qpa9lt4rpKen211Crp09e1Zly5bVuHHjVL9+/YvOExwcrA4dOmjOnDn5XJ1FBvmqadOmxsvLy0i66n9eXl6madOmdpeOa1y/fv1Mt27dsk278847TcOGDY0xxowfP/6if1/z5s0zxhjz4YcfmrJly7qW/e233y6Yt1+/fsYYY1q1amWGDRtmRo0aZUqVKmXKly9vxo8fn23d06ZNM3Xq1DEBAQHmuuuuM4MHDzYnT540xhizbt26C8Z+6KGHjCQTHx+fq+d//fXXm4kTJ5oBAwaYwMBAU7lyZTN37tzLLtOqVSvzyCOPmEcffdSUKVPGREVFGWOM+eabb0zp0qXNsmXLLrpcenq6GTBggOnSpcsF2+vjjz82UVFRpmjRoqZevXpm8+bN2ZaNjo42TZs2NYmJiRcd+5dffjE33HCD+fDDD13Txo8fb+rXr2/efvttc/3115sSJUqYnj17mhMnTlzyuc2bN88EBQVd8vGsenfs2GGMMSY+Pt5IMtddd53Zs2fPRZf566+/TMOGDc3UqVNd0/bv329uv/12U7JkSRMQEGBuuukm8+mnn15yvddff72ZPn36JR/PkpKSYnx9fbNth4SEBCPJbNmyxTXt7Nmzxt/f33zxxRdXHBO4lHnz5hlJJj093e5SgDx1qfcKNWvWzLYvvtr3Cll+/PFH07lzZ1O8eHETGBhoIiIizC+//JJtnS+++KIJCQkxpUuXNkOGDDHnzp1zLS/JfPLJJ9nGDAoKcq03a5+1aNEic8sttxh/f3/XYzExMeamm24yfn5+JiQkxDzyyCPZxn3jjTdM9+7dTdGiRU21atXM0qVLrW1E83/vY7744gvTuHFjU7RoUdOyZUuze/fuHI/VqlUr07t374u+B5o/f7657rrrLNebnzhymY927typb7755qqPWmZxOp365ptvuIsscuTHH3/U5s2b5efnJ+mf0ysSExNd/6ZOnaqAgAA1adJEkrRx40Y1btzYtXzlypX18ccfS5L27NmjxMREvfzyy67H58+fr2LFimnbtm2aMmWKnn32Wa1Zs8b1uJeXl1555RX99NNPmj9/vr788kuNHj1akhQeHq4ZM2aoRIkSrnr69u1r+TlPmzZNTZo00Y4dOzRkyBANHjxYe/bsuewy8+fPl5+fn7766iu99tprkqRhw4Zp4sSJ6tKli3bt2qVWrVqpbNmyuvvuu/X4449rypQpeu2117Rr1y6tW7cu23hjx45VdHS0du7cqRo1aqh3796uo2q7du1SbGyslixZopCQEM2ZM0fVq1dXlSpV9Oqrr6pmzZry9fXVG2+8oVGjRmU79Xbfvn1asmSJVqxYoRUrVmj9+vWaNGmS5W2W5dixY5KkqVOnqkaNGvrkk09Up04dVaxYUePGjVP79u21e/duLVy4UBMnTtTJkyclSY888ojOnj2rDRs26IcfftDkyZMVGBhouZ74+Hilp6erXbt2rmm1atVSaGhottNz/fz81KBBA23cuNHyOgGgsMl6r+Dr6ytJ6tu3b47eK0jSoUOHdMstt8jf319ffvml4uPjdf/992c7o2TdunXat2+f1q1bp/nz5ys2NlaxsbE5rnfMmDF69NFHlZCQ4Dqq98gjj+ihhx7SDz/8oGXLlqlatWrZlnnmmWd099136/vvv9dtt92me++9V0ePHs3xui9m7NixmjZtmr799lv5+Pjo/vvvd8u4WZo1a6Y//vjjqq9vvRb42F1AYfL1119bWv6BBx5Q1apV3VQNCpqvv/5aBw4ckK+vr5xOp5xOpxwOh2688Ub17Nkz27zJycmKi4tTs2bN9L///U+StGnTJvn7+2eb96+//pIkPfHEE66QKv0Tkvz8/LRr1y6NGzdOklSqVCkNHz5c9erVc813fggoXbq0YmJilJycLEn67bffdPr0aT366KOSpNq1a1veBrfddpuGDBniqnn69Olat26datasecllqlevrilTprh+37t3r/bv368HHnhAmZmZuuOOOxQVFaWXX35ZGzdu1OOPP66xY8fKz89PvXv31qpVq9S6dWvX8tHR0ercubOkf3ZotWvX1i+//KJatWppwYIF6tevnypWrKiNGzcqOjpab7zxhmrVqqXx48dr3759cjqdatu2rTIyMrRnzx7VqlVL0j8fMsXGxqp48eKS/nkDsHbtWk2cONHydpPkCsnVq1fXvn371Lt3b02bNk0333yzZs6cqXXr1mns2LGqWbOmateura+++kodO3bUwYMH1aNHD9WtW1eSdOONN7qlnsOHD8vPz++C63LLly+vw4cPZ5tWsWJFHThwwC3rBYCCbsWKFQoMDFRGRobOnj0rLy8vPf744xo9erQCAgIUEhIi6Z97A4wbN07z589XnTp1JEkHDhxQxYoVs403a9YsBQUFadGiRa6QWqNGjWzzlCpVSjNnzpS3t7dq1aqlzp07a+3atXrwwQdzVPuIESOyXR7x3HPPaeTIka73EpLUtGnTbMv0799fvXv3liQ9//zzeuWVV/T111+rY8eOOVr3xUycOFGtWrWS9E/w7dy5s86cOaMiRYpYHluSa1sfOHDAY65xJVzmo5MnT8rb2zvXN+c5ceKE2z5pQcFz9uxZlSpVSrVq1VJmZqYOHjwoh8OhgICAbH83Z86c0ddff63Q0FAVK1bM9diZM2fk5eWVbd4TJ05I+ueoVtYOQ/rnOofAwMBs83p5een48eOuacnJydq/f7/S0tKUkZEhY4ycTqf+/vtveXt7KzU1VcYY1/w5uZnApZwfbB0Oh0JCQlwB+VL+/QnsDz/8oKZNm8rHx0e7du3SoUOHNHPmTPn6+qpBgwZatmyZa94KFSrou+++u2QNFSpUkPRPSK9Vq5Z++OEH9e/fX5K0fPly3XvvvbrnnnskSa+99pquu+66bMtmHU2U/rnLalawzHr8Ss8tJ3755RfXz6tWrdItt9yiRx55RJI0e/bsbNd9n1/b8OHDNXjwYK1evVrt2rVTjx49sm2D/FC0aFGlpaXl6zoBwFO1bt1ac+bMUWpqqqZPny4fHx+1bds22zwHDx5U9+7dFR0drbvvvts1/fTp0xcEp507dyoyMjLb+4R/q127try9vV2/V6hQQT/88EOOa886gir9s2/9888/L6j9387fJxUrVkwlSpRw2/7zUvv80NBQt4xftGhRSfKofRzhMh8VL17c0l1fo6Oj9dBDD7mxIhQk/fv3V0pKiuuW206nU/Xr11evXr1cF96npqbq5ptv1m233abFixfL4XC4lr/33ntljNF7773nmhYXF6fWrVtryZIl2Y4gRUVFqUGDBtm+UqJ79+4qWbKkYmNjtX//ftWqVUuDBw9Wz549Vbp0aW3atEkDBw7U4sWLXfONGDHCdSrt9u3b9fzzz1vaBv/esTkcjiuehl6sWLFsv2dkZLhezM+dOydfX99s455/yuf27dsvOCp6/rxZ2zerhn+Pff66zx83NTVVe/fuzXamQm6eW06c/9r079r8/PxcR66dTqd27typUaNGSfrnjIoOHTro008/1erVq/XCCy9o2rRplm+fHhISonPnziklJSXb396RI0dcn6pnOXr0KGd1AMBVKlasmOvU0bfeekv169fPdjQyNTVVXbt2VcuWLfXss89mWzY4ODjbB5/S/wWgy7nSPszhcFxwF/aL3bDn/H3T1az3atZtxeX2+e6Q9QF82bJl3TZmXuOay3zUrFkzW5dH4eLl5aWnnnpK48aN0+nTp2WMUZ8+feR0OvXOO+9kC5aS1LBhQ+3atSvbtKxAkdMPReLj4+V0OjVt2jS1aNFCNWrU0J9//nnB2NfiV+xUq1bN9Wlq1jWQM2fOVGZmprZu3apVq1YpPT1d8+fP1+eff+46EpnTsSMiIrRo0SLt3r1b6enprtNb//77b91///3q1q2bypUr5/bndymVK1d2/RwREaHVq1dr69atyszM1MyZM5WSkqITJ05o5MiRqlSpUrbTjipXrqxBgwZp8eLFGjlypN544w3L9TRu3Fi+vr5au3ata9qePXt08OBBtWzZMtu8P/74oxo2bGh5nQBQ2GS9V5g9e7Yk5eq9Qr169bRx40ZLd28tW7asEhMTXb/v3bv3ikfrihcvripVqmTbTxQ0P/74o3x9fd1y6VB+IVzmowYNGqhp06by8srZZvfy8lLTpk3VoEGDvCkMBdZdd90lb29vzZo1SxMmTNAXX3yhuXPn6tSpUzp8+LAOHz6s06dPS5I6dOign376Kdsnktdff70cDodWrFihv//+W6dOnbqq9VarVk3p6el69dVX9euvv+qdd95x3SwnS5UqVXTq1CmtXbtWSUlJrjryUtu2bTVz5szLztOwYUOdPn1a69atU9GiRRUbG6v//ve/8vf314ABA9S9e3dNnjxZ8+bN0+rVq3P0aeIdd9yhN998U+np6erRo4e6du2qm266SQEBAUpJSVHFihXVrl07VapU6YLtdSUzZ8687KlBX3/9tWrVqqVDhw5d9PGsa0aOHz+uJk2aaMyYMYqMjJS/v79Wr16txo0bq1evXjp27Jg++eQT13IjRozQqlWr9Ntvv2n79u1at26dwsLCXI/XqlUr2/xXKygoSAMHDtTjjz+udevWKT4+XgMGDFDLli3VokUL13z79+/XoUOHst34BwBw9bLeK0jS3Llzc/xeYejQoTpx4oR69eqlb7/9Vnv37tU777xzxRvqna9NmzaaOXOmduzYoW+//VaDBg267Gm2WSZMmKBp06bplVde0d69e7V9+3a9+uqrOdwC9ti5c6d27typU6dOubbnv7/TcuPGjYqMjLzqo7TXAsJlPhs+fHiu7hY7fPjwPKoIBZmPj4+GDh2qKVOm6LPPPtOpU6cUHh6uChUquP69//77kqS6deuqUaNG+uCDD1zLV6pUSc8884zGjBmj8uXLa+jQoVe13vr16+ull17S5MmTVadOHS1YsEAvvPBCtnnCw8M1aNAg9ezZU2XLltXbb7/tvid+Cfv27VNSUtJl53E4HJo8ebL69eun/fv367bbbtPff/+tAwcOaNeuXZo9e7ZSUlIUFxeX408SW7durWrVqunBBx+U0+nU3Llzdfz4cR05ckSvv/66vv32Wx09elQvvfRSjm8GkJSUpH379l3y8bS0NO3Zs+eSnyxnHbl86qmnlJaWpqefflonTpzQn3/+qWXLlumzzz5TSkqKYmNjs52mmpmZqUceeURhYWHq2LGjatSo4foEXPrnaOPx48dz9FyyTJ8+Xbfffrt69OihW265RSEhIVq8eHG2eRYuXKhbb71V119/fa7WAQCFnY+Pj+u6yq+++irH7xXKlCmjL7/8UqdOnVKrVq3UuHFjvfHGG1cVDrNMmzZNlStXVmRkpO655x5FR0crICDgisv169dPM2bM0OzZs1W7dm3dfvvt2rt3bw63gD0aNmyohg0bKj4+XitXrpSkC97vL1q0KMc3PbKdjV+DUihlZGSY7t27X/V3XXp5eZk77rjDZGRk2F06CoEVK1aYsLAwk5mZme/rzvqexdx+z6W7TZw40ZQpU8ZMnTrV/P7778YYY86cOWNWrVplIiIizOLFi3M17tGjR02LFi1MixYtzPLly01qaqoxxpgjR46Yl156yTRo0MCcOnXKbc/jamVt/1atWpmwsDCzcOFCk5KSYowx5tixYyYmJsbUrl3btS2uBWfPnjWhoaFm06ZNdpcCD8f3XKKwy8k+2M73CgXVxbb/Z599ZsLCwjzudYkjl/nM29tb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f38NGDBA3bt31+TJkzVv3jytXr06R0fM7rjjDr355ptKT09Xjx491LVrV910000KCAhQSkqKKlasqHbt2qlSpUoXbK8rmTlz5mVP7/v6669Vq1Yt12nQF/PFF1/o6NGjatKkicaMGaPIyEj5+/tr9erVaty4sXr16qVjx45luzPriBEjtGrVKv3222/avn271q1bp7CwMNfjtWrVyvWdXA8fPqydO3e6Qu8PP/ygnTt3ZvvakbS0NMXHx+vWW2/N1TpgTdZrzAcffCBJevrppzV8+HB16tRJCxYs0Pvvv5/tzscdOnTQli1bsn2w9OSTT+qbb77RkCFD9P3332v37t2aM2eOkpKSrqqGokWLqkWLFq4b9axfv17jxo274nJFihTRE088odGjR+vtt9/Wvn37tHXrVsXExORwK+S/yZMn6+mnn9Zbb72lKlWquLbVv08P37hxo8f1BuESAHJg+PDhubpb7PDhw/OoIhRkPj4+Gjp0qKZMmaLPPvtMp06dUnh4uCpUqOD69/7770uS6tatq0aNGrneJEpSpUqV9Mwzz2jMmDEqX778BUchLqV+/fp66aWXNHnyZNWpU0cLFizQCy+8kG2e8PBwDRo0SD179lS7du3c96QvY9++fVd8w+pwODR58mT169dP+/fv12233aa///5bBw4c0K5duzR79mylpKQoLi7ugpuOXEnr1q1VrVo1Pfjgg3I6nZo7d66OHz+uI0eO6PXXX9e3336ro0eP6qWXXrrgurQrSUpK0r59+y75eFpamvbs2XPJ0wUlqV27durdu7fS0tL09NNP68SJE/rzzz+1bNkyffbZZ0pJSXF9hUKWzMxMPfLIIwoLC1PHjh1Vo0aNbDdm2bNnj44fP56j55LltddeU8OGDfXggw9Kkm655RY1bNgw23WvS5cuVWhoqCIjI3O1DliT9Rrz9ttvS/on6D3//POS/nlNef755/Xwww+7PtTo1KmTfHx89MUXX7jGqFGjhlavXq3vvvtOzZo1U8uWLbV06VL5+Fz91XdvvfWWMjIy1LhxY40YMULPPffcVS339NNPa+TIkfrvf/+rsLAw9ezZ0+3XMueFOXPm6Ny5c/rPf/6jChUquL5G6Z133nHNc+jQIW3evFkDBgywq8zcMQVEfHy8kWTi4+PtLqVQYvujsMjIyDDdu3c3Xl5eRtIV/3l5eZk7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Qzt37sw2/eWXX1ZsbKxb1vFvVapUybOxc8oYo//+97+qUKGCihYtqnbt2mnv3r2ux4ODg3Xfffdp/PjxNlaJwupSH/LExcXJ4XAoJSUl32sCcPXoYcBz0b/XJrcduezYsaMSExP166+/avr06Zo7d26O3vAfPHhQK1asUP/+/d1Vksu5c+fcPublhISEyN/fP0/XERQUpJIlS+bpOq4FU6ZM0SuvvKLXXntN27ZtU7FixdShQ4dsH1wMGDBACxYs0NGjR22sFAAAACjc3BYu/f39FRISosqVK6t79+5q166d1qxZI0l6++23FRgYmO2I05AhQ1SrVi2lpaVJkj744APVr19flSpVuuK61q9fr2bNmsnf318VKlTQmDFjlJGR4Xo8KipKQ4cO1YgRIxQcHKwOHTpIkpYtW6bq1aurSJEiat26tebPn5/tk43k5GT17t1blSpVUkBAgOrWrauFCxdmW3dUVJSGDx+u0aNHq3Tp0goJCdGECROyzXP+abETJkxwHdU9/1/WkcGVK1cqIiJCJUuWVJkyZXT77bdr3759rrFuuOEGSVLDhg3lcDgUFRUl6cJPa86ePavhw4erXLlyKlKkiCIiIvTNN9+4Hs/6FGft2rVq0qSJAgICFB4erj179kiSYmNjXbUdOHBAAwYMyLa+y+nfv78ef/xxSdKtt96qMmXK6JFHHlF6evoVl70cY4xmzJihcePGqVu3bqpXr57efvtt/fnnn9lOO65du7YqVqyoTz75xNL6AAAAAORenlxz+eOPP2rz5s3y8/OTJN1333267bbbdO+99yojI0Offvqp3nzzTS1YsEABAQGSpI0bN6pJkyZXHPvQoUO67bbb1LRpU3333XeaM2eOYmJiFBMTk22++fPny8/PT1999ZVee+01/fbbb/rPf/6j7t2767vvvtPDDz+ssWPHZlvmzJkzaty4sT799FP9+OOPeuihh9S3b199/fXXF4xdrFgxbdu2TVOmTNGzzz7rCtL/Fh0drcTERNe/qVOnKiAgwPVcU1NT9fjjj+vbb7/V2rVr5eXlpTvuuENOp1OSXOv+4osvlJiYqMWLF190PaNHj9bHH3+s+fPna/v27apWrZo6dOhwwdG8sWPHatq0afr222/l4+Oj+++/X5LUs2dPV43XXXedZsyYcdn1/du3334rSZo7d67mz5+v2NhYy6fW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55+XJD3zzDPy8PBQx44ddenSpXtuey/NmjXTf/7zH7Vt2/aO6zg6Oqp58+ZasmSJ6f4AAAAAZEyW3XO5f/9+ffvtt3JxcZH072WccXFx9q8JEybI1dVVTzzxhCQpKipKtWvXvme7iYmJCgkJUZEiRbR79259+eWX2rJliz744IM064WHh+vQoUPavHmz1q5dq4sXL6ply5aqVq2a9u7dq3fffVfDhg1Ls01qaqoeeughffnllzpw4IBGjBihN998U8uWLUuz3rZt23T06FFt27ZN8+fP17x58+wh+WahoaFp3vfixYvl5OSkevXqSZIuXbqk7t27Kzo6Wt9//70qVaqk5s2b24PZ7t27JUlz585VXFyc/eebffzxx5o4caImTJign3/+WSEhIWrVqpWOHDmSZr233npLYWFhiomJ0SOPPKLnn39eycnJ8vf3t9fo5+enIUOG3LW/m/3xxx+SpMmTJ2vt2rWKjIzUuHHj7mvbzPDkk08qKioq2/oDAAAAkJZTZja2du1aubm5KTk5Wf/8848cHBw0depUSf9exunm5iZJ+v777/X2229r/vz5qlq1qiTpxIkTKlmy5D37+OKLL3T16lV9/vnnKly4sCRp6tSpatmyZZr1ChcurE8//dQebmfMmCGbzabZs2erYMGCqlKlik6dOqXevXvbt3F2dtbo0aPtP5cvX17fffedli1bpueee86+vEiRIpo6daocHR316KOPqkWLFgoPD0/T1nWFChVSoUKFJElHjx7Vyy+/rPfee09NmjSRJDVq1CjN+rNmzZKnp6ciIyP1zDPPqFixYpIkT09P+fj43HG/TJgwQcOGDVPHjh0lSR988IG2bdumyZMnp7mkNCwsTC1atJAkjR49Wo899ph+/fVXPfroo/b2XVxc5Obmdtf+bnb9fseKFSuqVq1a6tq1q8LDwzV27Nj7bsOMkiVL6vfff1dqaqocHHLUPFUAgBzs+meXG6WkpFhUDQDkbpn6Kbxhw4aKiYnRzp071b17d/Xs2VPt27dPs87JkyfVpk0bhYWFpQlsV65cUcGCBdOs+9hjj9lDabNmzSRJsbGxql69uj1YSlK9evVumcylWrVq9mApSYcOHdLjjz+epo8nn3zylvcwbdo01a5dW8WKFZObm5tmzZqlkydP3lKXo6Oj/ecSJUro77//vuu+uXDhgp555hm1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pjlz5iglJUV+fn5ycXGxuqR0KVCggBo0aKA///zT6lLS7ffff9exY8d08uRJwiUybN26dVq0aJE8PT1VvXp1q8tJt8qVK0uS/vjjD4srSb8ffvhBiYmJCgwMJFwCAABUqFBBy5cvV2hoqDw8PLRixQq5urpaXVaet3fvXoWEhKhq1apaunSp1eUgF3v99dd16NAhLViwQB07dlTfvn2tLinPMwxD48aNU2RkpF599VX17t3b6pIyRe689gMAAOQobdq00bp16xQVFaWQkBBduHDB6pLytO3bt6thw4aqUKGCIiMjVaJECatLQi7m5OSkuXPnasCAAerXr5/GjRtndUl5mmEYGjZsmN58802NHj1aH330Ua69JP9meeNdAAAAyzVu3FhbtmzRL7/8ooYNG+rvv/+2uqQ8ad26dQoJCVGdOnW0ZcsWFS1a1OqSkAc4ODjo448/1ogRI/TGG29o+PDhMgzD6rLynJSUFPXp00fjx4/X5MmTNWLECNlsNqvLyjSESwAAkGmeeuopRUZGKi4uTvXr19fvv/9udUl5ytKlS9W6dWuFhIRo7dq1cnNzs7ok5CE2m81+Ju2DDz5Q//79lZKSYnVZeca1a9fUuXNnzZkzR/PmzdMrr7xidUmZjnAJAAAyVbVq1RQVFaV//vlHAQEBOnz4sNUl5QmzZs3S888/r06dOmn58uUqWLCg1SUhj3rttdc0Z84czZo1S127dlVSUpLVJeV6ly9fVps2bfTVV1/pyy+/zLMTcBEuAQBApqtYsaKio6NVuHBhBQYGKiYmxuqScrUPP/xQffr00YABAzR37lw5OTEnI7JWr169tGzZMi1fvlxt27bVlStXrC4p17pw4YJCQkIUGRmpb775Ru3atbO6pCxDuAQAAFmiVKlS2r59u0qXLq2goCDt2LHD6pJyHcMw9MYbb2jYsGF655139PHHH+eZiT+Q87Vv315ff/21tm3bpqZNm+rixYtWl5Tr/Pe//1XDhg21f/9+bdmyRcHBwVaXlKX47QQAALKMt7e3tm7dqho1aujpp5/Wpk2brC4p10hNTVX//v01btw4TZw4UWPGjMlTE38gdwgJCdHmzZv1008/qVGjRoqPj7e6pFzj999/V2BgoP78809FRkbKz8/P6pKyHOESAABkKXd3d61fv14NGzbUM888o+XLl1tdUo6XlJSkrl27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evLJJzV58mQlJiaqZ8+eGWrv/PnzeuaZZxQTE6P169erUaNGpuoD8pKHH35Y0dHRatKkierXr6+NGzeqZs2aGW4vs49fSdq+fbueeeYZValSRevWrVPRokUz3FZ+RLgEAAC5hoODgyZPnqwiRYrojTfe0Pnz5/X+++9n+F7G0NBQ/fe//9WIESN0+vRp1ahRQxs2bLhlkpD78ffffyskJEQnTpxQeHi46tatm6GagLysZMmS2r59u5o1a6agoCCtXbtWgYGBGWorM49fSfrmm2/UoUMH1atXT6tWrZKbm1uG2snPbIZhGFYXAQC5WXJyspydnTV37lz16NHD6nKAfGPy5Ml67bXX1LdvX02dOtXSx3ucPHlSTZo00aVLl7Rp0yZVrVrVslqA3ODSpUtq3bq1vv/+e61cuVJNmza1tJ4lS5aoa9euatGihZYsWaKCBQtaWk9uxT2XAAAgV3r11Vf12WefadasWeratauSkpIsqePQoUMKCAhQUlKSoqKiCJbAfXjggQe0bt06BQcHq1WrVlq2bJlltcycOVOdOnVSp06dtHz5coKlCYRLAACQa/Xs2VPLli3T8uXL1bZtW125ciVb+//xxx8VGBioBx54QFFRUapQoUK29g/kZgULFtSKFSv03HPPqWPHjvr000+zvYYPPvhAffv21YABAzR37lw5OXHXoBmESwAAkKu1b99ea9eu1bZt29S0aVNdvHgxW/rdsWOHGjZsqLJly2r79u0qVapUtvQL5CXOzs76/PPP1a9fP/Xu3VsTJkzIln4Nw9Abb7yh4cOH65133tHHH38sBweikVnsQQAAkOs9/fTT2rx5s3766Sc1atRI8fHxWdrfhg0b1KRJE9WsWVPh4eHy8vLK0v6AvMzBwUFTp07Vm2++qaFDh+rtt99WVk4Lk5qaqv79+2vcuHH66KOPNGbMmAxPCoa0CJcAACBP8Pf3V2RkpH7//XfVr19ff/zxR5b08+WXX6pVq1YKDg7WunXr5O7uniX9APmJzWbT2LFj9eGHH2rs2LEaOHCgUlNTM72fpKQkdenSRbNmzdKcOXP02muvZXof+RnhEgAA5BnVq1dXVFSUEhMTFRAQoF9//TVT258zZ446duyoZ599VitWrFChQoUytX0gvxs6dKhmzZqlTz75RN27d8/UibquXLmitm3bavny5Vq6dKl69eqV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CJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0wiXAAAAAADTCJcAAAAAANMIlwAAAAAA0/4fk4tDYlznoo8AAAAASUVORK5CYII=",
                         "text/plain": [
                             "<Figure size 900x1000 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
@@ -368,30 +368,30 @@
         {
             "cell_type": "code",
             "execution_count": 11,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAABfAAAADkCAYAAADXRQVdAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/SrBM8AAAACXBIWXMAAA9hAAAPYQGoP6dpAABVnUlEQVR4nO3deVwV9f7H8fdhB2MTwQ3FLU1QMte8iZJbi9l1z6zccMt9ya1riW2GZpaWu4mmWdcl08ytrpapuZY3c8sFzMwNBRcEBeb3R5fz4wgqKjAHeD0fj/OAMzNn5j0Mc+acz8x8vxbDMAwBAAAAAAAAAAC74mB2AAAAAAAAAAAAkBkFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7BAFfAAAAAAAAAAA7JCT2QHyo7i4OI0fP14pKSlmR8lR7dq1U4MGDcyOcc8uX76st99+W0lJSWZHAQBkUK1aNfXo0cPsGPfMMAx99NFHOnr0qNlRclSFChU0cOBAs2Pcl7lz5+rXX381OwYAk7i5uemtt96SkxNfawEAQMFlMQzDMDtEfjN27Fi98847qlKlitlRckRaWpoOHDigp59+WqtXrzY7zj374IMPNHToUAUHB5sdBQDwP8ePH5fFYtH58+fl5uZmdpx7cuDAAQUHB6t8+fLy8PAwO06OOHHihBITE3Xu3Dn5+vqaHeeenD59WiVLllTZsmXl6elpdhwAeezcuXM6e/asvvvuOzVu3NjsOAAAALmGSxXuQVpamkqXLq19+/aZHSVHREdHq1u3bhoxYoTZUe5LWlqaHnjggQKzXQAgvzt69KhCQkI0bNiwfFu8l/4+vkjSZ599pkcffdTkNPfv9OnTqlKlinr16pVvi/fS/2+X6dOn6+mnnzY5DYC8lJKSolq1aqlcuXIKDw83Ow4AAECuog18k0VGRspisZi23Pj4eI0YMUKdOnVSo0aN8jwHUJBZLBb179/f7BiAaQYPHqyAgAC9+uqrZkfJUdHR0bJYLNq1a5fZUazCw8NVrVq1bE07cuRIOTs766233srlVEDOKVeunJ555pk7Trdp0yZZLBZt2rTJOqxr164qV67cXS3PHvdz/L/p06fr119/1ccffywHB77SAgCAgo1POwVYYmKiIiMjbb7A3Oy1115TUlKSJk6cmHfBgAJm69atioyMVHx8fK4uZ//+/YqMjFRMTEyuLgfICatWrdLXX3+tDz74QEWKFDE7Dv5n8+bNWrBggaKiolS0aFGz46CQyKvjJAqHM2fOaMyYMerVq5dq165tdhwAAIBcRwHfZGPGjNG1a9dyZd6JiYkaN25clgX8MWPG6KefftK0adMUGRmpUqVK5UoGoDDYunWrxo0blycF/HHjxlHAh927du2aBg4cqCeeeEKtW7c2Ow7+JyUlRf369VO9evXUrVs3s+OgEMmr4+StzJ49W4cOHTJl2ch5I0aMkLOzs95++22zowAAAOSJQt0G/tWrV02/KtDJyUlOTnm/GRwcHDR06FBVrVpVAwYMyPPlAwAKrqioKP35559at26dKc3EFRQ5/Tll2rRp2rdvn3bu3EmTEyhUnJ2dzY6AHPLjjz9qwYIFmjVrlvz8/MyOAwAAkCcKzLe3n3/+WU899ZS8vLz0wAMPqEmTJvrpp5+s49Pbsfz+++/Vt29fBQQEKDAw0Dr+448/VoUKFeTu7q66detq8+bNCg8Pt+kU6fr163r99dc1Z84cnThxQkWKFFFYWJg2btxokyUmJkYWi0XvvfeeZs2apYoVK8rV1VV16tTRzp07baa9uQ38rl27ymKxZPmIjIy0yVGrVi15e3tnmSMmJkb+/v6SpHHjxmWaR5s2bbR161Z9/PHH1i81KSkpevPNN615y5Urp1dffVXJyck2mdPbIP3xxx9Vt25dubm5qUKFClqwYMFdbjUg/4uMjNTw4cMlSeXLl7fuaxmvkl+xYoWqVasmV1dXhYSEaO3atTbziI2NVd++fVWlShW5u7vLz89P7du3t5lHdHS02rdvL0l6/PHHrcu5XRNZgBmOHj2qd999V8OHD1flypXNjnPP/vzzT0VERKhUqVJ65JFHJEkTJkzQ9evXrdMkJydr6NCh8vf3V5EiRdS6dWudO3fOZj4Zj70ZlStXTl27drU+v9PnlDVr1qhRo0by9PSUl5eX6tSpo88++yzTfPfv36/HH39cHh4eKl26tCZMmCDp745rX3vtNfXp00e1atW6nz8NCpk///xT3bt3V/Hixa3HsU8++cRmmqlTpyokJEQeHh7y9fVV7dq1rf+fdzpOzps3T40bN1ZAQIBcXV0VHBys6dOn3zLP+vXrVaNGDbm5uSk4OFjLly+/4zpk1Qb+559/rlq1aln3qerVq+vDDz/M9Nrs7OfIG+l3EdWtW1cRERFmxwEAAMgzBeIK/N9++01hYWHy8vKy3lI5c+ZMhYeH6/vvv1e9evWs0/bt21f+/v56/fXXdfXqVUl/d4LUv39/hYWFaciQIYqJiVGrVq3k6+tr8+X50qVLmjNnjoKCgnT9+nWNGjVKc+fO1RNPPKEdO3aoRo0aNrk+++wzXb58Wb1795bFYtGECRPUpk0bHTt27JZXAvXu3VtNmza1GbZ27VotWrRIAQEBNjmef/559ezZU5cvX86Uw9/fX9OnT9fLL7+s1q1bq02bNpKk0NBQxcfHa8OGDZJk03Ftjx49NH/+fLVr107Dhg3T9u3bNX78eB04cEBffvmlTaYjR46oXbt2ioiIUJcuXfTJJ5+oa9euqlWrlkJCQu5m8wH5Wps2bXT48GEtXrxYkydPVrFixSTJegLtxx9/1PLly9W3b195enpqypQpatu2rU6cOGG9cmznzp3aunWrOnbsqMDAQMXExGj69OkKDw/X/v375eHhoYYNG2rgwIGaMmWKXn31VVWtWlWSrD8BezF48GAVL148X3dce+rUKdWtW1fx8fHq1auXvLy89MYbb+jnn39WYmKidboBAwbI19dXY8eOVUxMjD744AP1799fX3zxxT0vO6vPKdHR0erevbtCQkI0evRo+fj46Oeff9batWvVqVMn62svXryoJ598Um3atFGHDh20dOlSjRw5UtWrV9fnn39Ox7W4a2fOnNGjjz5q7ZTd399fa9asUUREhC5duqTBgwdr9uzZGjhwoNq1a6dBgwYpKSlJ//3vf7V9+3Z16tTpjsfJ6dOnKyQkRM8++6ycnJy0atUq9e3bV2lpaerXr59Nnt9//13PPfec+vTpoy5dumjevHlq37691q5dq2bNmmV7vTZs2KDnn39eTZo0UVRUlCTpwIED2rJliwYNGmQzbW7s57g36R3X7tixg7uIAABA4WIUAK1atTJcXFyMo0ePWoedOnXK8PT0NBo2bGgYhmHMmzfPkGQ0aNDASElJsU6XnJxs+Pn5GXXq1DFu3LhhHR4dHW1IMho1amQdlpKSYiQnJxtjxowxgoKCDMMwjIsXLxrFixc3unfvbp3u+PHjhiTDz8/PuHDhgnX4V199ZUgyVq1aZR02duxY43ab4ffffze8vb2NZs2aWXOn58goqxznzp0zJBljx461mbZ///6Gi4uLzXJ/+eUXQ5LRo0cPm2lfeeUVQ5Lxn//8xzosKCjIkGT88MMP1mFnz541XF1djWHDht1yXXLbpEmTDE9PT9OWj8Jr4sSJhiTj+PHjNsMlGS4uLsaRI0esw/bu3WtIMqZOnWodlpiYmGme27ZtMyQZCxYssA5bsmSJIcnYuHFjjq8DkBNWrlxpSDKWLVtmdpT70rlzZ8PBwcHYuXOnYRiGsW/fPkOSsW3bNiMtLc36maJp06ZGWlqa9XVDhgwxHB0djfj4eOuwrI7DhvH3sbRLly7W57f6nBIfH294enoa9erVM65du2Yzj4zLbtSoUab3jOTkZKNEiRLWcXPmzLnnv4k9+vPPPw1JxurVq82OUmBFREQYJUuWNM6fP28zvGPHjoa3t7eRmJho/POf/zRCQkJuO59bHScNI+tj4BNPPGFUqFDBZlj658+M7y8JCQlGyZIljUceecQ6bOPGjZmOlV26dLF+djcMwxg0aJDh5eVls6/d7G72c+S+06dPG15eXkbv3r3NjgIAAJDn8v2lC6mpqVq/fr1atWqlChUqWIeXLFlSnTp10o8//qhLly5Zh/fs2VOOjo7W57t27VJcXJx69uxp0xb9Cy+8IF9fX5tlOTo6ysXFRZJkGIYuXLiglJQU1a5dW3v27MmU7bnnnrOZR1hYmCTp2LFj2Vq3q1evqnXr1vL19dXixYutuTPmSEtLu2OOjH755RdNmzbNpmkgSfrmm28kSUOHDrUZPmzYMEnS6tWrbYYHBwdb10f6+yqqKlWqZHvdgMKiadOmqlixovV5aGiovLy8bPYVd3d36+83btxQXFycKlWqJB8fnzvu04C9KCgd16alpWnFihVq2bKlateunWl8xmbvevXqZfM8LCxMqampio2Nvefl3/w5ZcOGDbp8+bJGjRolNze3W2aRpAceeEAvvvii9bmLi4vq1Kmj7du303Et7pphGFq2bJlatmwpwzB0/vx56+OJJ55QQkKC9uzZIx8fH508eTJTM5HZlfEYmJCQoPPnz6tRo0Y6duyYEhISbKYtVaqUzfuLl5eXOnfurJ9//lmnT5/O9jJ9fHx09epV6x2pt5Mb+znuHh3XAgCAwizfF/DPnTunxMREValSJdO4qlWrKi0tTX/88Yd1WPny5W2mSf/wXalSJZvhTk5OmdrKlKT58+dr1qxZ1uYv/P39tXr16kxfMCSpbNmyNs/Ti/kXL17M1rr17NlTR48e1Zdffpmpk6b58+crNDRUbm5ud8yRLv1W5KpVq6pu3bo242JjY+Xg4JDp71CiRAn5+Phk+pJy87qlr1921w0oLLKzr1y7dk2vv/66ypQpI1dXVxUrVkz+/v6Kj4+/7T4N2JOoqCidOnVKU6dOzdcd1547d06XLl1StWrV7jjt/R7ns3Lz55SjR49KUrbyBAYGZvrbnzlzRklJSfr4449pcgJ35dy5c4qPj9esWbPk7+9v80g/GXT27FmNHDlSDzzwgOrWrasHH3xQ/fr105YtW7K9nC1btqhp06YqUqSIfHx85O/vb22C6+ZjYKVKlTL9j6f3tZGx35g76du3rypXrqynnnpKgYGB6t69e6b+adLlxn6Ou5Pece27775Lx7UAAKBQKhBt4N+NjFf53K2FCxeqa9euqlKlilJTU7Vo0SI5Ojpq/Pjx1i/YGWW8gi4jwzDuuKwPP/xQixcv1sKFCzO1rZ+eo1WrVho+fLgCAgJumyPdggULtHXrVm3atClTx7vpslt0uZ91AwqT7OwrAwYM0Lx58zR48GDVr19f3t7eslgs6tixo9LS0vIqKnDP0juufeWVV/Tggw+aHSfP3M+xMDU1Ncvh9/M55eY8p0+f1s8//yxPT086rsVdSz/+vPjii+rSpUuW04SGhiogIECHDh3S119/rbVr12rZsmWaNm2aXn/9dY0bN+62yzh69KiaNGmihx56SO+//77KlCkjFxcXffPNN5o8eXKuHQMDAgL0yy+/aN26dVqzZo3WrFmjefPmqXPnzpo/f77NtHzmNVfGjmu7d+9udhwAAABT5PsCvr+/vzw8PHTo0KFM4w4ePCgHBweVKVPmlrf1BgUFSfq7U9bHH3/cOjwlJUUxMTEKDQ21Dlu6dKkqVKigdu3aaeHChXriiSckSWPHjs3JVdLmzZv1yiuvaPDgwXrhhRcyjU/PsXz5cpuC+805Mo6Lj4/XiBEj1KlTJzVq1ChTAT8oKEhpaWn6/fffbTrFPHPmjOLj461/JwCZ3e/VxkuXLlWXLl00adIk67CkpCTFx8fn6HKA3FIQOq5N5+/vLy8vL+3bty9H5ufr65tpX75+/br++uuvbL0+vQmuffv2ZbpL7k5GjhwpBwcH+fj43NXrAOnvfcHT01Opqalq2rTpbactUqSInnvuOT333HO6fv262rRpo7ffflujR4+Wm5vbLY9fq1atUnJyslauXGlzpfutLjQ5cuSIDMOwmd/hw4clKcs7Z2/HxcVFLVu2VMuWLZWWlqa+fftq5syZeu211+56X0PuoeNaAACAAtCEjqOjo5o3b66vvvrK5tbZM2fO6LPPPlODBg3k5eV1y9fXrl1bfn5+mj17tlJSUqzDFy1alOnW2KyuwNm+fbu2bdt2/yvyP3/99Zc6dOigBg0aaOLEiVlOk54j45U/WeXw8PCQ9Hfx/rXXXlNSUtIt5/n0009Lkj744AOb4e+//74kqUWLFne/MkAhUaRIEUnKVKTLLkdHx0xX8k2dOjXTFbr3uxwgN6xatUpff/21Jk+ebP0fzc8cHBzUqlUrrVq1Srt27co0/m6vuq1YsaJ++OEHm2GzZs265RX4N2vevLk8PT01fvx4JSUlZTvL5s2btWDBAtWqVYuiF+6Jo6Oj2rZtq2XLlmV5QuvcuXOSpLi4OJvhLi4uCg4OlmEYunHjhqRbH7+y+kybkJCgefPmZZnp1KlT+vLLL63PL126pAULFqhGjRoqUaJEttft5swODg7Wi3aSk5OzPR/krjNnzmjMmDHq1atXln2SAAAAFBb5/gp8SXrrrbe0YcMGNWjQQH379pWTk5Nmzpyp5ORkTZgw4bavdXFxUWRkpAYMGKDGjRurQ4cOiomJUXR0tCpWrGhzhc8zzzyj5cuXa8mSJbp8+bJGjx6tGTNmKDg4WFeuXMmRdRk4cKDOnTunESNG6PPPP7cZFxoaqtDQUGuO1q1bq0WLFjp+/HiWOdzd3RUcHKxFixYpLi5OL7zwgi5cuKBSpUplWu7DDz+sLl26aNasWYqPj1ejRo20Y8cOzZ8/X61atbK5OwGArfSmKf71r3+pY8eOcnZ2VsuWLbP9+meeeUaffvqpvL29FRwcrG3btunbb7/N1M5rjRo15OjoqKioKCUkJMjV1VWNGzdWQEBAjq4PkF0FpePam73zzjtav369GjVqpF69esnb21vS3x3c7969+67m1aNHD/Xp00dt27ZVs2bNtHfvXq1bt07FihXL1uu9vLw0efJk9ejRQ3Xq1FGnTp3k6+urvXv3KjExMVNzH9L/NzlRr149VapUSX/++eddZQbSvfvuu9q4caPq1aunnj17Kjg4WBcuXNCePXv07bff6sKFC2revLlKlCihxx57TMWLF9eBAwf00UcfqUWLFvL09JR06+Nk8+bNrVfC9+7dW1euXNHs2bMVEBCQ5V0qlStXVkREhHbu3KnixYvrk08+0ZkzZ25Z8L+VHj166MKFC2rcuLECAwMVGxurqVOnqkaNGjZ3osJcdFwLAADwtwJRwA8JCdHmzZs1evRojR8/XmlpaapXr54WLlyoevXq3fH1/fv3l2EYmjRpkl555RU9/PDDWrlypQYOHCg3NzfrdF27dtXp06etxbN169Zp4cKFWrJkiTZt2pQj63Lu3DmlpqZq6NChmcaNHTtWoaGh1hwzZ87UunXrFBwcfMscs2bNsjb1s3DhQlWsWPGWHeHNmTNHFSpUUHR0tL788kuVKFFCo0ePzvEmgoCCpk6dOnrzzTc1Y8YMrV27VmlpaTp+/Hi2X//hhx/K0dFRixYtUlJSkh577DF9++231n03XYkSJTRjxgyNHz9eERERSk1N1caNGyngwzTpHdeuX7++QDXxVLp0aW3fvl2vvfaaFi1aZO1I85FHHrHe3ZZdPXv21PHjxzV37lytXbtWYWFh2rBhg5o0aZLteURERCggIEDvvvuu3nzzTTk7O+uhhx7SkCFDspx+2rRp2rdvn3bu3KmpU6feVV4go+LFi2vHjh164403tHz5ck2bNk1+fn4KCQlRVFSUJKl3795atGiR3n//fV25ckWBgYEaOHCgxowZY53PrY6TVapU0dKlSzVmzBi98sorKlGihF5++WX5+/tn2d75gw8+qKlTp2r48OE6dOiQypcvry+++CLT8fJOXnzxRc2aNUvTpk1TfHy8SpQooeeee06RkZHcsWIn0juunT17Nh3XAgCAQs9i0ANTltLS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AAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgAwAAAAAAAABghyjgA8h3OnTooMqVK5sdAwAAAAAAAMhVFsMwDLNDAAAAAAAAAAAAW1yBDwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHaKADwAAAAAAAACAHfo/VPDwENM59l8AAAAASUVORK5CYII=",
+                        "image/png": "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eZqbm8Pa2hr29vZo1KgRunbtivfee0+8kGVrawt9ff0y/iSIiKi0MLgkqoJkMhmcnZ3h7OxcYJr8/Hykp6cX2Brx+iMlJQXXr19HZmam0snoy5cvi1yu4ganenp6kEql0NXVVfpb2GUlmZ4tu5WLIAjIy8tDfn4+8vPzxf+Luqwk0ufm5hY5KFQ8srOzi7TdBgYGSt8xc3Nz8UKSg4OD2gtMb15skkqlpbRXiIioPGJwSURqSaVSWFlZwcrKqtjrkMvlyM7OFk9ui9Na8ubjzQBW8cjNzVU5ES+oNaW0SSQSjYNXdct0dHQgkUjEhyKvwv5fkul0dHQgCIL4APDO/0s7nVwuL5VAT5FPWdPR0VGpE3p6egVeYDE1NYWNjU2BrxsZGRWpJwEvkhARUVExuCSiUqOjoyOerGqDIAjFajEqrVYnTdchl8vFQOf1/4sSkBX1/4Je09HREYP34ga7JfW/ItjV09MrFy3XJbUOBndU0V2+fBnGxsbaLgYRlSEGl0RUaSlaEHV1eagjIiprNWrU0HYRiKiMcfQMIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDSyIiIiIiItIYg0siIiIiIiLSGINLIiIiIiIi0hiDS6rU9PT0MGzYMDg7O2u7KERERERElZpEEARB24UgIiIiIiKiio0tl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKQxBpdERERERESkMQaXREREREREpDEGl0RERERERKSx/wdDNB+Soczt6AAAAABJRU5ErkJggg==",
                         "text/plain": [
-                            "<Figure size 1500x600 with 1 Axes>"
+                            "<Figure size 900x600 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "from lambeq.backend import draw_equation\n",
                 "\n",
                 "original_diagram = train_diagrams[0]\n",
                 "removed_cups_diagram = remove_cups(original_diagram)\n",
                 "\n",
-                "draw_equation(original_diagram, removed_cups_diagram, symbol='-->', figsize=(15, 6), asymmetry=0.3, fontsize=12)"
+                "draw_equation(original_diagram, removed_cups_diagram, symbol='-->', figsize=(9, 6), asymmetry=0.3, fontsize=12)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Training\n",
@@ -554,48 +554,49 @@
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "raw_mimetype": "text/restructuredtext"
             },
             "source": [
-                "We can now pass the datasets to the :py:meth:`~lambeq.Trainer.fit` method of the trainer to start the training."
+                "We can now pass the datasets to the :py:meth:`~lambeq.Trainer.fit` method of the trainer to start the training. Here, we perform early stopping if the validation accuracy doesn't improve within the specified `early_stopping_interval` epochs."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Epoch 1:    train/loss: 1.6565   valid/loss: 2.5863   train/acc: 0.6000   valid/acc: 0.6129\n",
-                        "Epoch 2:    train/loss: 2.7489   valid/loss: 2.7984   train/acc: 0.6643   valid/acc: 0.3871\n",
-                        "Epoch 3:    train/loss: 0.2307   valid/loss: 1.0433   train/acc: 0.7214   valid/acc: 0.7903\n",
-                        "Epoch 4:    train/loss: 0.4410   valid/loss: 2.6108   train/acc: 0.7857   valid/acc: 0.6774\n",
-                        "Epoch 5:    train/loss: 1.4217   valid/loss: 2.0467   train/acc: 0.7143   valid/acc: 0.5968\n",
-                        "Epoch 6:    train/loss: 2.7733   valid/loss: 2.1691   train/acc: 0.6214   valid/acc: 0.4839\n",
-                        "Epoch 7:    train/loss: 0.7625   valid/loss: 1.2315   train/acc: 0.6571   valid/acc: 0.7742\n",
-                        "Epoch 8:    train/loss: 2.8028   valid/loss: 3.1985   train/acc: 0.5286   valid/acc: 0.6129\n",
-                        "Epoch 9:    train/loss: 0.7338   valid/loss: 1.4462   train/acc: 0.4857   valid/acc: 0.5161\n",
-                        "Epoch 10:   train/loss: 1.1405   valid/loss: 3.5565   train/acc: 0.3429   valid/acc: 0.3387\n",
-                        "Epoch 11:   train/loss: 2.2153   valid/loss: 2.9543   train/acc: 0.4143   valid/acc: 0.2258\n",
-                        "Epoch 12:   train/loss: 1.9657   valid/loss: 2.2286   train/acc: 0.3714   valid/acc: 0.3548\n",
-                        "Epoch 13:   train/loss: 0.7303   valid/loss: 1.3492   train/acc: 0.5143   valid/acc: 0.5806\n",
+                        "Epoch 1:    train/loss: 0.5620   valid/loss: 2.4878   train/acc: 0.6214   valid/acc: 0.6613\n",
+                        "Epoch 2:    train/loss: 0.7484   valid/loss: 2.3023   train/acc: 0.4786   valid/acc: 0.4355\n",
+                        "Epoch 3:    train/loss: 0.5687   valid/loss: 2.1669   train/acc: 0.5714   valid/acc: 0.4839\n",
+                        "Epoch 4:    train/loss: 0.5116   valid/loss: 1.7920   train/acc: 0.6071   valid/acc: 0.6935\n",
+                        "Epoch 5:    train/loss: 2.6042   valid/loss: 1.9361   train/acc: 0.7286   valid/acc: 0.7742\n",
+                        "Epoch 6:    train/loss: 0.6296   valid/loss: 1.4529   train/acc: 0.6000   valid/acc: 0.5000\n",
+                        "Epoch 7:    train/loss: 0.5425   valid/loss: 1.4265   train/acc: 0.5643   valid/acc: 0.5806\n",
+                        "Epoch 8:    train/loss: 2.1077   valid/loss: 2.3139   train/acc: 0.5000   valid/acc: 0.3871\n",
+                        "Epoch 9:    train/loss: 0.2571   valid/loss: 2.4732   train/acc: 0.6643   valid/acc: 0.6129\n",
+                        "Epoch 10:   train/loss: 1.7144   valid/loss: 2.9791   train/acc: 0.6929   valid/acc: 0.5000\n",
                         "Early stopping!\n",
-                        "Best model saved to RelPron/logs/best_model.lt\n",
+                        "Best model (epoch=5, step=35) saved to\n",
+                        "RelPron/logs/best_model.lt\n",
                         "\n",
                         "Training completed!\n"
                     ]
                 }
             ],
             "source": [
-                "trainer.fit(train_dataset, val_dataset, early_stopping_interval=10)"
+                "trainer.fit(train_dataset, val_dataset,\n",
+                "            early_stopping_criterion='acc',\n",
+                "            early_stopping_interval=5,\n",
+                "            minimize_criterion=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Results\n",
@@ -608,59 +609,59 @@
             "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Validation accuracy: 0.8225806451612904\n"
+                        "Validation accuracy: 0.7419354838709677\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "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",
+                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAA04AAAIjCAYAAAA0vUuxAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMCwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy81sbWrAAAACXBIWXMAAA9hAAAPYQGoP6dpAADN0klEQVR4nOzdd3QUVR/G8e9ueg89AQIEQidU6V2aVBFQFJUiWFFBwIK9Y+9dX0FFFAVERHqJ9N6l9wChBEjv2Xn/WLIaSQiBJJPyfM7Z4+7slCcjmclv5s69FsMwDERERERERCRbVrMDiIiIiIiIFHYqnERERERERHKgwklERERERCQHKpxERERERERyoMJJREREREQkByqcREREREREcqDCSUREREREJAcqnERERERERHKgwklERERERCQHKpxE8snw4cOpVq3aNS374osvYrFY8jaQiIiUKEePHsVisTBlyhSzo4gUCyqcpMSxWCxX9QoLCzM7apE3bdo0PvjgA7NjiIjkmSlTpmQ6V7i7u1OxYkV69OjBRx99RGxsrNkRBXj99deZPXt2gW/31KlTvPjii2zbtq3Aty35z2IYhmF2CJGCNHXq1Eyfv//+exYvXswPP/yQaXq3bt2oUKHCNW8nNTUVm82Gm5tbrpdNS0sjLS0Nd3f3a95+YdCnTx927drF0aNHzY4iIpInpkyZwogRI3j55ZcJDg4mNTWV06dPExYWxuLFi6lSpQpz5syhYcOGZkfl6NGjBAcHM3nyZIYPH252nALl7e3NoEGDCvxu26ZNm2jevHmJ3OclgbPZAUQK2l133ZXp87p161i8ePFl0/8rISEBT0/Pq96Oi4vLNeUDcHZ2xtlZv54iIoVVz549ueGGGxyfJ06cyLJly+jTpw/9+vVjz549eHh4mJhQRPKamuqJZKFTp040aNCAzZs306FDBzw9PXn66acB+P333+nduzcVK1bEzc2NGjVq8Morr5Cenp5pHf99ximjrfk777zDV199RY0aNXBzc6N58+Zs3Lgx07JZPeNksVh4+OGHmT17Ng0aNMDNzY369euzYMGCy/KHhYVxww034O7uTo0aNfjyyy+v+rmpAwcOMHDgQAICAnB3d6dy5crcfvvtREdHZ5pv6tSpNGvWDA8PD0qXLs3tt99OeHh4pn34559/cuzYMUeTlmt95ktEpCi48cYbee655zh27NhlrRv27t3LoEGDKF26NO7u7txwww3MmTPH8f2mTZuwWCx89913l6134cKFWCwW5s6d65h28uRJ7rnnHipUqOA4H3z77bdXlXPZsmW0b98eLy8v/P39ufnmm9mzZ0+meTLOGXv37uW2227D19eXMmXKMGbMGJKSkjLNm3F++vXXX6lXrx4eHh60bt2anTt3AvDll18SEhKCu7s7nTp1yrIVwvr167npppvw8/PD09OTjh07snr16iwzHTx4kOHDh+Pv74+fnx8jRowgISEhU574+Hi+++47x/knp7s/H3/8MfXr18fT05NSpUpxww03MG3atEzz5LTPw8LCaN68OQAjRoxwbFvPmBUfuqQtko3z58/Ts2dPbr/9du666y5Hs70pU6bg7e3NuHHj8Pb2ZtmyZTz//PPExMTw9ttv57jeadOmERsby/3334/FYuGtt95iwIABHD58OMe7VKtWrWLWrFk89NBD+Pj48NFHHzFw4ECOHz9OmTJlANi6dSs33XQTgYGBvPTSS6Snp/Pyyy9Trly5HLOlpKTQo0cPkpOTeeSRRwgICODkyZPMnTuXqKgo/Pz8AHjttdd47rnnuO222xg1ahTnzp3j448/pkOHDmzduhV/f3+eeeYZoqOjOXHiBO+//z5gbzohIlKc3X333Tz99NMsWrSIe++9F4C///6btm3bUqlSJZ566im8vLz45Zdf6N+/PzNnzuSWW27hhhtuoHr16vzyyy8MGzYs0zqnT59OqVKl6NGjBwBnzpyhVatWjoKlXLlyzJ8/n5EjRxITE8PYsWOzzbdkyRJ69uxJ9erVefHFF0lMTOTjjz+mbdu2bNmy5bILXLfddhvVqlVj0qRJrFu3jo8++oiLFy/y/fffZ5pv5cqVzJkzh9GjRwMwadIk+vTpwxNPPMFnn33GQw89xMWLF3nrrbe45557WLZsmWPZZcuW0bNnT5o1a8YLL7yA1Wpl8uTJ3HjjjaxcuZIWLVpclik4OJhJkyaxZcsWvvnmG8qXL8+bb74JwA8//MCoUaNo0aIF9913HwA1atTIdp98/fXXPProowwaNMhRGO7YsYP169czZMiQq97ndevW5eWXX+b555/nvvvuo3379gC0adMm221LEWOIlHCjR482/vur0LFjRwMwvvjii8vmT0hIuGza/fffb3h6ehpJSUmOacOG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ffRRLBYLP/zwQ542lbteL774IosWLaJt27Y8+OCDpKen88knn9CgQQO2bdt2xWWXLVvGww8/zK233kqtWrVIS0vjhx9+cJw0wH518NVXX2XixIkcPXqU/v374+Pjw5EjR/jtt9+47777mDBhAmA/IU6fPp1x48bRvHlzvL296du3b37vAhGRfDd//nz27t1LWloaZ86cYdmyZSxevJiqVasyZ84c3N3dHfN++umntGvXjtDQUO69916qV6/OmTNnWLt2LSdOnGD79u2Z1j148GCef/553N3dGTlyJFZr5uvcb7zxBsuXL6dly5bce++91KtXjwsXLrBlyxaWLFnChQsXss399ttv07NnT1q3bs3IkSMd3ZH7+fnx4osvXjb/kSNH6NevHzfddBNr165l6tSpDBkyhEaNGl3fDrzEarXyzTff0LNnT+rXr8+IESOoVKkSJ0+eZPny5fj6+vLHH3/ker3NmjVjyZIlvPfee1SsWJHg4GBHxxT/1b17dwICAmjbti0VKlRgz549fPLJJ/Tu3dvRscXV7vMaNWrg7+/PF198gY+PD15eXrRs2TLTXTspwgq+Iz+RwiW77siz65p09erVRqtWrQwPDw+jYsWKxhNPPGEsXLjQAIzly5c75suuO/K33377snUCxgsvvOD4nF135KNHj75s2apVq17W5erSpUuNJk2aGK6urkaNGjWMb775xhg/frzh7u6ezV6wO3z4sHHPPfcYNWrUMNzd3Y3SpUsbnTt3NpYsWXLZvDNnzjTatWtneHl5GV5eXkadOnWM0aNHG/v27XPMExcXZwwZMsTw9/c3AHVNLiJFXkZ35BkvV1dXIyAgwOjWrZvx4YcfZup6+98OHTpkDB061AgICDBcXFyMSpUqGX369DFmzJhx2bwHDhxwrH/VqlVZru/MmTPG6NGjjaCgIMPFxcUICAgwunTpYnz11VeOebLqjtwwDGPJkiVG27ZtDQ8PD8PX19fo27evsXv37kzzZJyHdu/ebQwaNMjw8fExSpUqZTz88MNGYmJipnmzOj9ld85bvnx5lsNebN261RgwYIBRpkwZw83Nzahatapx2223GUuXLr0s07lz5zItm/H/5N/doe/du9fo0KGD4eHhYQBX7Jr8yy+/NDp06ODYdo0aNYzHH3/ciI6OzjTf1exzw7APM1KvXj3HMCDqmrz4sBhG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EcmBCicREREREZEcqHASERERERHJgQonERERERGRHKhwEhERERERyYEKJxERERERkRyocBIREREREcmBCicREREREZEcqHASERERERHJgQonERERERGRHKhwEhERERERyYEKJxERERERkRyocBIREREREcmBCicREREREZEcqHASERERERHJgQonERERERGRHKhwEhERERERyYEKJxERERERkRyocBIREREREcmBCicREREREZEcqHASERERERHJgQonERERERGRHKhwEhERERERyYEKJxERERERkRyocBIREREREcmBCicREREREZEcqHASERERERHJgQonERERERGRHKhwEhERERERyYEKJxERERERkRw4mx2goNlsNk6dOoWPjw8Wi8XsOCIiJYphGMTGxlKxYkWsVl27y6Bzk4iIOXJzXipxhdOpU6cICgoyO4aISIkWHh5O5cqVzY5RaOjcJCJirqs5L5W4wsnHxwew7xxfX1+T04iIlCwxMTEEBQU5jsVip3OTiIg5cnNeKnGFU0YTCF9fX52cRERMouZomencJCJirqs5L6mBuYiIiIgUOtWqVeODDz4wO0a+ePHFF2ncuLHZMSSXVDiJiIiIlDDp6emEhYXx008/ERYWRnp6utmRClRYWBgWi4WoqChTtj9hwgSWLl1qyrbl2qlwEhERESlBZs2aRUhICJ07d2bIkCF07tyZkJAQZs2aZXY0AFJSUsyOkO+8vb0pU6aM2TEkl1Q4iYiIiJQQs2bNYtCgQYSGhrJ27VpiY2NZu3YtoaGhDBo0KNfFk81mY9KkSQQHB+Ph4UGjRo2YMWOG4/v09HRGjhzp+L527dp8+OGHmdYxfPhw+vfvz2uvvUbFihWpXbv2Zdu555576NOnT6ZpqamplC9fnv/9739ZZjt27Bh9+/alVKlSeHl5Ub9+febNm8fRo0fp3LkzAKVKlcJisTB8+HAAkpOTefTRRylfvjzu7u60a9eOjRs3OtaZcafqzz//pGHDhri7u9OqVSt27drlmGfKlCn4+/sze/Zsatasibu7Oz169CA8PNwxz3+b6mXsg3feeYfAwEDKlCnD6NGjSU1NdcwTERFB79698fDwIDg4mGnTphXr5oyFUYnrHEJERESkJEpPT2f8+PH06dOH2bNnO8asadWqFbNnz6Z///5MmDCBm2++GScnp6ta56RJk5g6dSpffPEFNWvWZMWKFdx1112UK1eOjh07YrPZqFy5Mr/++itlypRhzZo13HfffQQGBnLbbbc51rN06VJ8fX1ZvHhxltsZNWoUHTp0ICIigsDAQADmzp1LQkICgwcPznKZ0aNHk5KSwooVK/Dy8mL37t14e3sTFBTEzJkzGThwIPv27cPX1xcPDw8AnnjiCWbOnMl3331H1apVeeutt+jRowcHDx6kdOnSjnU//vjjfPjhhwQEBPD000/Tt29f9u/fj4uLCwAJCQm89tprfP/997i6uvLQQw9x++23s3r16mz35fLlywkMDGT58uUcPHiQwYMH07hxY+69914Ahg4dSmRkJGFhYbi4uDBu3DjOnj17Vf+fJI8YJUx0dLQBGNHR0WZHEREpcXQMzpr2ixSE5cuXG4Cxdu1awzAMI2bxYiP84YeN1HPnDMMwjDVr1hiAsXz58qtaX1JSkuHp6WmsWbMm0/SRI0cad9xxR7bLjR492hg4cKDj87Bhw4wKFSoYycnJmearWrWq8f777zs+16tXz3jzzTcdn/v27WsMHz482+2EhoYaL774YpbfZeyLixcvOqbFxcUZLi4uxo8//uiYlpKSYlSsWNF46623Mi33888/O+Y5f/684eHhYUyfPt0wDMOYPHmyARjr1q1zzLNnzx4DMNavX28YhmG88MILRqNGjTLtg6pVqxppaWmOabfeeqsxePDgTMtv3LjR8f2BAwcMINM+ktzLzfFXTfVERERESoCIiAgAGjRoQNzKlZwY+xixi5dw8ZdfHNP/PV9ODh48SEJCAt26dcPb29vx+v777zl06JBjvk8//ZRmzZpRrlw5vL29+eqrrzh+/HimdYWGhuLq6nrF7Y0aNYrJkycDcObMGebPn88999yT7fyPPvoor776Km3btuWFF15gx44dV1z/oUOHSE1NpW3bto5pLi4utGjRgj179mSat3Xr1o73pUuXpnbt2pnmcXZ2pnnz5o7PderUwd/f/7L1/Fv9+vUz3ekLDAx03FHat28fzs7ONG3a1PF9SEgIpUqVuuLPJHlLhZOIiIhICZDRxG3z7N85MWYspKUBkLB2HYDjOZ2M+XISFxcHwJ9//sm2bdscr927dzuec/r555+ZMGECI0eOZNGiRWzbto0RI0Zc1gGEl5dXjtsbOnQohw8fZu3atUydOpXg4GDa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",
                         "text/plain": [
                             "<Figure size 1000x600 with 4 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "fig, ((ax_tl, ax_tr), (ax_bl, ax_br)) = plt.subplots(2, 2, sharex=True, sharey='row', figsize=(10, 6))\n",
                 "ax_tl.set_title('Training set')\n",
                 "ax_tr.set_title('Development set')\n",
-                "ax_bl.set_xlabel('Iterations')\n",
-                "ax_br.set_xlabel('Iterations')\n",
+                "ax_bl.set_xlabel('Epochs')\n",
+                "ax_br.set_xlabel('Epochs')\n",
                 "ax_bl.set_ylabel('Accuracy')\n",
                 "ax_tl.set_ylabel('Loss')\n",
                 "\n",
                 "colours = iter(plt.rcParams['axes.prop_cycle'].by_key()['color'])\n",
                 "range_ = np.arange(1, len(trainer.train_epoch_costs)+1)\n",
                 "ax_tl.plot(range_, trainer.train_epoch_costs, color=next(colours))\n",
                 "ax_bl.plot(range_, trainer.train_eval_results['acc'], color=next(colours))\n",
                 "ax_tr.plot(range_, trainer.val_costs, color=next(colours))\n",
                 "ax_br.plot(range_, trainer.val_eval_results['acc'], color=next(colours))\n",
                 "\n",
                 "# mark best model as circle\n",
-                "best_epoch = np.argmin(trainer.val_costs)\n",
+                "best_epoch = np.argmax(trainer.val_eval_results['acc'])\n",
                 "ax_tl.plot(best_epoch + 1, trainer.train_epoch_costs[best_epoch], 'o', color='black', fillstyle='none')\n",
                 "ax_tr.plot(best_epoch + 1, trainer.val_costs[best_epoch], 'o', color='black', fillstyle='none')\n",
                 "ax_bl.plot(best_epoch + 1, trainer.train_eval_results['acc'][best_epoch], 'o', color='black', fillstyle='none')\n",
                 "ax_br.plot(best_epoch + 1, trainer.val_eval_results['acc'][best_epoch], 'o', color='black', fillstyle='none')\n",
                 "\n",
-                "ax_tr.text(best_epoch + 1.4, trainer.val_costs[best_epoch], 'early stopping', va='center')\n",
+                "ax_br.text(best_epoch + 1.4, trainer.val_eval_results['acc'][best_epoch], 'early stopping', va='center')\n",
                 "\n",
                 "# print test accuracy\n",
                 "model.load(trainer.log_dir + '/best_model.lt')\n",
-                "test_acc = acc(model(val_circuits), val_labels)\n",
-                "print('Validation accuracy:', test_acc.item())"
+                "val_acc = acc(model(val_circuits), val_labels)\n",
+                "print('Validation accuracy:', val_acc.item())"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "raw_mimetype": "text/restructuredtext"
             },
```

### Comparing `lambeq-0.4.0/docs/tutorials/training-symbols.ipynb` & `lambeq-0.4.1/docs/tutorials/training-symbols.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/tutorials/training-usecase.ipynb` & `lambeq-0.4.1/docs/tutorials/training-usecase.ipynb`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/uml-diagrams.rst` & `lambeq-0.4.1/docs/uml-diagrams.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/docs/use-cases.rst` & `lambeq-0.4.1/docs/use-cases.rst`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/__init__.py` & `lambeq-0.4.1/lambeq/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
         'BaseAnsatz',
         'CircuitAnsatz',
         'IQPAnsatz',
         'MPSAnsatz',
         'Sim14Ansatz',
         'Sim15Ansatz',
+        'Sim4Ansatz',
         'SpiderAnsatz',
         'StronglyEntanglingAnsatz',
         'Symbol',
         'TensorAnsatz',
 
         'CCGType',
         'CCGRule',
@@ -49,16 +50,14 @@
         'WebParseError',
         'WebParser',
 
         'AtomicType',
 
         'VerbosityLevel',
 
-        'diagram2str',
-
         'Reader',
         'LinearReader',
         'TreeReader',
         'TreeReaderMode',
         'bag_of_words_reader',
         'cups_reader',
         'spiders_reader',
@@ -103,19 +102,18 @@
         'CrossEntropyLoss',
         'LossFunction',
         'MSELoss',
 ]
 
 from lambeq import ansatz, core, rewrite, text2diagram, tokeniser, training
 from lambeq.ansatz import (BaseAnsatz, CircuitAnsatz, IQPAnsatz, MPSAnsatz,
-                           Sim14Ansatz, Sim15Ansatz, SpiderAnsatz,
+                           Sim14Ansatz, Sim15Ansatz, Sim4Ansatz, SpiderAnsatz,
                            StronglyEntanglingAnsatz, Symbol, TensorAnsatz)
 from lambeq.core.globals import VerbosityLevel
 from lambeq.core.types import AtomicType
-from lambeq.backend.drawing.text_printer import diagram2str
 from lambeq.rewrite import (CoordinationRewriteRule, CurryRewriteRule,
                             DiagramRewriter, RemoveCupsRewriter,
                             RemoveSwapsRewriter, Rewriter, RewriteRule,
                             SimpleRewriteRule, UnifyCodomainRewriter,
                             UnknownWordsRewriteRule)
 from lambeq.text2diagram import (
         CCGType, CCGRule, CCGRuleUseError, CCGTree,
```

### Comparing `lambeq-0.4.0/lambeq/ansatz/__init__.py` & `lambeq-0.4.1/lambeq/ansatz/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 __all__ = ['BaseAnsatz', 'CircuitAnsatz', 'IQPAnsatz', 'MPSAnsatz',
-           'Sim14Ansatz', 'Sim15Ansatz', 'SpiderAnsatz',
+           'Sim14Ansatz', 'Sim15Ansatz', 'Sim4Ansatz', 'SpiderAnsatz',
            'StronglyEntanglingAnsatz', 'Symbol', 'TensorAnsatz']
 
 from lambeq.ansatz.base import BaseAnsatz, Symbol
 from lambeq.ansatz.circuit import (CircuitAnsatz, IQPAnsatz,
-                                   Sim14Ansatz, Sim15Ansatz,
+                                   Sim14Ansatz, Sim15Ansatz, Sim4Ansatz,
                                    StronglyEntanglingAnsatz)
 from lambeq.ansatz.tensor import MPSAnsatz, SpiderAnsatz, TensorAnsatz
```

### Comparing `lambeq-0.4.0/lambeq/ansatz/base.py` & `lambeq-0.4.1/lambeq/ansatz/base.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/ansatz/circuit.py` & `lambeq-0.4.1/lambeq/ansatz/circuit.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 under the BSD 3-Clause "New" or "Revised" License.
 """
 
 from __future__ import annotations
 
 __all__ = ['CircuitAnsatz',
            'IQPAnsatz',
+           'Sim4Ansatz',
            'Sim14Ansatz',
            'Sim15Ansatz',
            'StronglyEntanglingAnsatz']
 
 from abc import abstractmethod
 from collections.abc import Callable, Mapping
 from itertools import cycle
@@ -73,14 +74,16 @@
         ob_map : dict
             A mapping from :py:class:`lambeq.backend.grammar.Ty` to
             the number of qubits it uses in a circuit.
         n_layers : int
             The number of layers used by the ansatz.
         n_single_qubit_params : int
             The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
         circuit : callable
             Circuit generator used by the ansatz. This is a function
             (or a class constructor) that takes a number of qubits and
             a numpy array of parameters, and returns the ansatz of that
             size, with parameterised boxes.
         discard : bool, default: False
             Discard open wires instead of post-selecting.
@@ -177,14 +180,16 @@
         ob_map : dict
             A mapping from :py:class:`lambeq.backend.grammar.Ty` to
             the number of qubits it uses in a circuit.
         n_layers : int
             The number of layers used by the ansatz.
         n_single_qubit_params : int, default: 3
             The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
         discard : bool, default: False
             Discard open wires instead of post-selecting.
 
         """
         super().__init__(ob_map,
                          n_layers,
                          n_single_qubit_params,
@@ -214,15 +219,15 @@
 
 class Sim14Ansatz(CircuitAnsatz):
     """Modification of circuit 14 from Sim et al.
 
     Replaces circuit-block construction with two rings of CRx gates, in
     opposite orientation.
 
-    Paper at: https://arxiv.org/pdf/1905.10876.pdf
+    Paper at: https://arxiv.org/abs/1905.10876
 
     Code adapted from DisCoPy.
 
     """
 
     def __init__(self,
                  ob_map: Mapping[Ty, int],
@@ -236,14 +241,16 @@
         ob_map : dict
             A mapping from :py:class:`lambeq.backend.grammar.Ty` to
             the number of qubits it uses in a circuit.
         n_layers : int
             The number of layers used by the ansatz.
         n_single_qubit_params : int, default: 3
             The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
         discard : bool, default: False
             Discard open wires instead of post-selecting.
 
         """
         super().__init__(ob_map,
                          n_layers,
                          n_single_qubit_params,
@@ -282,15 +289,15 @@
 
 class Sim15Ansatz(CircuitAnsatz):
     """Modification of circuit 15 from Sim et al.
 
     Replaces circuit-block construction with two rings of CNOT gates, in
     opposite orientation.
 
-    Paper at: https://arxiv.org/pdf/1905.10876.pdf
+    Paper at: https://arxiv.org/abs/1905.10876
 
     Code adapted from DisCoPy.
 
     """
 
     def __init__(self,
                  ob_map: Mapping[Ty, int],
@@ -304,14 +311,16 @@
         ob_map : dict
             A mapping from :py:class:`lambeq.backend.grammar.Ty` to
             the number of qubits it uses in a circuit.
         n_layers : int
             The number of layers used by the ansatz.
         n_single_qubit_params : int, default: 3
             The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
         discard : bool, default: False
             Discard open wires instead of post-selecting.
 
         """
         super().__init__(ob_map,
                          n_layers,
                          n_single_qubit_params,
@@ -344,14 +353,76 @@
                     sublayer2 = sublayer2.CX(src, tgt)
 
                 circuit >>= sublayer1 >> sublayer2
 
         return circuit  # type: ignore[return-value]
 
 
+class Sim4Ansatz(CircuitAnsatz):
+    """Circuit 4 from Sim et al.
+
+    Ansatz with a layer of Rx and Rz gates, followed by a
+    ladder of CRxs.
+
+    Paper at: https://arxiv.org/abs/1905.10876
+
+    """
+
+    def __init__(self,
+                 ob_map: Mapping[Ty, int],
+                 n_layers: int,
+                 n_single_qubit_params: int = 3,
+                 discard: bool = False) -> None:
+        """Instantiate a Sim 4 ansatz.
+
+        Parameters
+        ----------
+        ob_map : dict
+            A mapping from :py:class:`lambeq.backend.grammar.Ty` to
+            the number of qubits it uses in a circuit.
+        n_layers : int
+            The number of layers used by the ansatz.
+        n_single_qubit_params : int, default: 3
+            The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
+        discard : bool, default: False
+            Discard open wires instead of post-selecting.
+
+        """
+        super().__init__(ob_map,
+                         n_layers,
+                         n_single_qubit_params,
+                         self.circuit,
+                         discard,
+                         [Rx, Rz])
+
+    def params_shape(self, n_qubits: int) -> tuple[int, ...]:
+        return (self.n_layers, 3 * n_qubits - 1)
+
+    def circuit(self, n_qubits: int, params: np.ndarray) -> Circuit:
+        if n_qubits == 1:
+            circuit = Rx(params[0]) >> Rz(params[1]) >> Rx(params[2])
+        else:
+            circuit = Id(n_qubits)
+
+            for thetas in params:
+                circuit >>= Id().tensor(*map(Rx, thetas[:n_qubits]))
+                circuit >>= Id().tensor(*map(Rz,
+                                             thetas[n_qubits:2 * n_qubits]))
+
+                crxs = Id(n_qubits)
+                for i in range(n_qubits - 1):
+                    crxs = crxs.CRx(thetas[2 * n_qubits + i], i, i + 1)
+
+                circuit >>= crxs
+
+        return circuit  # type: ignore[return-value]
+
+
 class StronglyEntanglingAnsatz(CircuitAnsatz):
     """Strongly entangling ansatz.
 
     Ansatz using three single qubit rotations (RzRyRz) followed by a
     ladder of CNOT gates with different ranges per layer.
 
     This is adapted from the PennyLane implementation of the
@@ -376,14 +447,16 @@
         ob_map : dict
             A mapping from :py:class:`lambeq.backend.grammar.Ty` to
             the number of qubits it uses in a circuit.
         n_layers : int
             The number of circuit layers used by the ansatz.
         n_single_qubit_params : int, default: 3
             The number of single qubit rotations used by the ansatz.
+            It only affects wires that `ob_map` maps to a single
+            qubit.
         ranges : list of int, optional
             The range of the CNOT gate between wires in each layer. By
             default, the range starts at one (i.e. adjacent wires) and
             increases by one for each subsequent layer.
         discard : bool, default: False
             Discard open wires instead of post-selecting.
```

### Comparing `lambeq-0.4.0/lambeq/ansatz/tensor.py` & `lambeq-0.4.1/lambeq/ansatz/tensor.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/__init__.py` & `lambeq-0.4.1/lambeq/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/converters/discopy.py` & `lambeq-0.4.1/lambeq/backend/converters/discopy.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,43 @@
 under the BSD 3-Clause "New" or "Revised" License.
 
 """
 from __future__ import annotations
 
 from typing import cast, Type, TypeVar, Union
 
-try:
-    from discopy import quantum as dq
-    from discopy import tensor as dt
-    from discopy.grammar import pregroup as dg
-
-except ImportError:
-    raise ImportError('`import discopy` failed. Please install discopy by '
-                      'running `pip install discopy`.')
+from packaging import version
 
 from lambeq.backend import grammar as lg
 from lambeq.backend import quantum as lq
 from lambeq.backend import tensor as lt
 
 
+MIN_DISCOPY_VERSION = '1.1.0'
+
+try:
+    import discopy
+except ImportError as ie:
+    raise ImportError(
+        '`import discopy` failed. Please install discopy by '
+        f'running `pip install "discopy>={MIN_DISCOPY_VERSION}"`.'
+    ) from ie
+else:
+    if version.parse(discopy.__version__) < version.parse(MIN_DISCOPY_VERSION):
+        raise DeprecationWarning(
+            'Conversion from lambeq to discopy and vice versa '
+            f'requires discopy>={MIN_DISCOPY_VERSION}. Please update discopy '
+            f'by running `pip install "discopy>={MIN_DISCOPY_VERSION}"`.'
+        )
+
+from discopy import quantum as dq   # noqa: E402,I100
+from discopy import tensor as dt    # noqa: E402
+from discopy.grammar import pregroup as dg  # noqa: E402
+
+
 _LAMBEQ_QUANTUM_BOX_TY = Union[type[lq.Box], lq.Box]
 _DISCOPY_QUANTUM_BOX_TY = Union[type[dq.Box], dq.Box]
 _QUANTUM_MAP_L2D_TY = dict[_LAMBEQ_QUANTUM_BOX_TY, _DISCOPY_QUANTUM_BOX_TY]
 _QUANTUM_MAP_D2L_TY = dict[_DISCOPY_QUANTUM_BOX_TY, _LAMBEQ_QUANTUM_BOX_TY]
 QUANTUM_MAPPINGS_L2D: _QUANTUM_MAP_L2D_TY = {lq.Discard: dq.Discard,
                                              lq.Encode: dq.Encode,
                                              lq.Measure: dq.Measure,
@@ -64,15 +79,16 @@
     val: key for key, val in QUANTUM_MAPPINGS_L2D.items()
 }
 _LAMBEQ_DIAGRAM_TY = Union[lg.Diagram, lq.Diagram, lt.Diagram]
 _DISCOPY_DIAGRAM_TY = Union[dg.Diagram, dq.Circuit, dt.Diagram]
 _DISCOPY_TY_VAR = TypeVar('_DISCOPY_TY_VAR', dg.Ty, dq.Ty, dt.Dim)
 _LAMBEQ_TY_VAR = TypeVar('_LAMBEQ_TY_VAR', lg.Ty, lq.Ty, lt.Dim)
 _DISCOPY_BOX_VAR = TypeVar('_DISCOPY_BOX_VAR', dg.Box, dq.Box, dt.Box)
-_LAMBEQ_BOX_VAR = TypeVar('_LAMBEQ_BOX_VAR', lg.Box, lq.Box, lt.Box)
+_LAMBEQ_BOX_VAR = TypeVar('_LAMBEQ_BOX_VAR',
+                          lg.Box, lq.Box, lt.Box, lq.Diagram)
 _DISCOPY_ENTITY = TypeVar('_DISCOPY_ENTITY', dg.Ty, dq.Ty, dt.Dim, dg.Box,
                           dq.Box, dt.Box)
 
 
 def _unwind_discopy_entity(entity: _DISCOPY_ENTITY) -> _DISCOPY_ENTITY:
     """Unwind a discopy entity."""
     if entity.z in (None, 0):
@@ -184,34 +200,42 @@
                 op = op.rotate(box.z)
         except KeyError:  # pragma: no cover
             raise NotImplementedError(box)
 
     return op
 
 
-def convert_quantum_d2l(box: dq.Box) -> lq.Box:
+def convert_quantum_d2l(box: dq.Box) -> lq.Box | lq.Diagram:
     lq_box: _LAMBEQ_QUANTUM_BOX_TY
 
     if box.is_dagger:
         op = convert_quantum_d2l(box.dagger()).dagger()
 
     elif isinstance(box, dq.Controlled):
-        op = lq.Controlled(controlled=convert_quantum_d2l(box.controlled),
-                           distance=box.distance)
+        controlled = convert_quantum_d2l(box.controlled)
+        if isinstance(controlled, lq.Diagram):
+            op = controlled
+        else:
+            op = lq.Controlled(controlled=controlled,
+                               distance=box.distance)
 
     elif isinstance(box, (dq.Rx, dq.Ry, dq.Rz,
                           dq.gates.Scalar, dq.gates.Sqrt)):
         lq_box = cast(type[Union[lq.Rx, lq.Ry, lq.Rz, lq.Scalar, lq.Sqrt]],
                       QUANTUM_MAPPINGS_D2L[type(box)])
         op = lq_box(cast(float, box.data))
 
     elif isinstance(box, (dq.Bra, dq.Ket)):
-        lq_box = cast(type[Union[lq.Bra, lq.Ket]],
-                      QUANTUM_MAPPINGS_D2L[type(box)])
-        op = lq_box(*box.bitstring)
+        if box.bitstring:
+            lq_box = cast(type[Union[lq.Bra, lq.Ket]],
+                          QUANTUM_MAPPINGS_D2L[type(box)])
+
+            op = lq_box(*box.bitstring)
+        else:
+            op = lq.Id()
 
     elif isinstance(box, (dq.Discard, dq.Encode)):
         lq_box = cast(type[Union[lq.Discard, lq.Encode]],
                       QUANTUM_MAPPINGS_D2L[type(box)])
         op = lq_box()
 
     elif isinstance(box, dq.Measure):
@@ -411,15 +435,15 @@
             target: type[_LAMBEQ_BOX_VAR]) -> _LAMBEQ_BOX_VAR:
 
     if target == lg.Box:
         assert isinstance(box, dg.Box)
         return convert_grammar_d2l(box)  # type: ignore[return-value]
     elif target == lq.Box:
         assert isinstance(box, dq.Box)
-        return convert_quantum_d2l(box)
+        return convert_quantum_d2l(box)  # type: ignore[return-value]
     elif target == lt.Box:
         assert isinstance(box, dt.Box)
         return convert_tensor_d2l(box)  # type: ignore[return-value]
     else:
         raise NotImplementedError(target)
 
 
@@ -493,14 +517,20 @@
     :class:`lambeq.backend.grammar.Diagram` |
         :class:`lambeq.backend.quantum.Diagram` |
         :class:`lambeq.backend.tensor.Diagram`
         The converted diagram.
 
     """
 
+    if version.parse(discopy.__version__) < version.parse(MIN_DISCOPY_VERSION):
+        raise DeprecationWarning(
+            'Conversion from discopy to lambeq'
+            f'requires discopy>={MIN_DISCOPY_VERSION}.'
+        )
+
     if isinstance(diagram, dq.Circuit):
         from lambeq.backend.quantum import Box, Ty, Id
     elif isinstance(diagram, dt.Diagram):
         from lambeq.backend.tensor import (Box,  # type: ignore[assignment]
                                            Dim as Ty,
                                            Id)
     elif isinstance(diagram, dg.Diagram):
```

### Comparing `lambeq-0.4.0/lambeq/backend/converters/tk.py` & `lambeq-0.4.1/lambeq/backend/converters/tk.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/drawable.py` & `lambeq-0.4.1/lambeq/backend/drawing/drawable.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/drawing.py` & `lambeq-0.4.1/lambeq/backend/drawing/drawing.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
                                              LEDGE,
                                              WireEndpointType)
 from lambeq.backend.drawing.drawing_backend import (DEFAULT_ASPECT,
                                                     DEFAULT_MARGINS,
                                                     DrawingBackend)
 from lambeq.backend.drawing.helpers import drawn_as_spider, needs_asymmetry
 from lambeq.backend.drawing.mat_backend import MatBackend
+from lambeq.backend.drawing.text_printer import PregroupTextPrinter
 from lambeq.backend.drawing.tikz_backend import TikzBackend
 from lambeq.backend.grammar import Diagram
 
 
 if TYPE_CHECKING:
     from IPython.core.display import HTML as HTML_ty
 
@@ -197,14 +198,60 @@
         baseline=len(drawable.boxes) / 2 or .5,
         tikz_options=params.get('tikz_options', None),
         show=params.get('show', True),
         margins=params.get('margins', DEFAULT_MARGINS),
         aspect=params.get('aspect', DEFAULT_ASPECT))
 
 
+def render_as_str(diagram: Diagram,
+                  word_spacing: int = 2,
+                  use_at_separator: bool = False,
+                  compress_layers: bool = True,
+                  use_ascii: bool = False) -> str:
+    """Render a grammar diagram as text.
+
+    Presently only implemented for pregroup diagrams.
+
+    Parameters
+    ----------
+    diagram: Diagram
+        Diagram to draw.
+    word_spacing : int, default: 2
+        The number of spaces between the words of the diagrams.
+    use_at_separator : bool, default: False
+        Whether to represent types using @ as the monoidal product.
+        Otherwise, use the unicode dot character.
+    compress_layers : bool, default: True
+        Whether to draw boxes in the same layer when they can occur
+        simultaneously, otherwise, draw one box per layer.
+    use_ascii: bool, default: False
+        Whether to draw using ASCII characters only, for
+        compatibility reasons.
+
+    Returns
+    -------
+    str
+        Drawing of diagram in string format.
+
+    """
+
+    if diagram.is_pregroup:
+        text_printer = PregroupTextPrinter(word_spacing,
+                                           use_at_separator,
+                                           compress_layers,
+                                           use_ascii)
+    else:
+        # TODO: Add text/CLI drawing for non-pregroup diagrams.
+        raise NotImplementedError('Text drawing is only supported for'
+                                  ' pregroups. Provided diagram is not a'
+                                  ' pregroup diagram.')
+
+    return text_printer.diagram2str(diagram)
+
+
 def to_gif(diagrams: list[Diagram],
            path: str | None = None,
            timestep: int = 500,
            loop: bool = False,
            **params) -> str | HTML_ty:
     """Build a GIF stepping through the given diagrams.
```

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/drawing_backend.py` & `lambeq-0.4.1/lambeq/backend/drawing/drawing_backend.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/helpers.py` & `lambeq-0.4.1/lambeq/backend/drawing/helpers.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/mat_backend.py` & `lambeq-0.4.1/lambeq/backend/drawing/mat_backend.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/text_printer.py` & `lambeq-0.4.1/lambeq/backend/drawing/text_printer.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,36 +17,20 @@
 Module that allows printing of lambeq pregroup diagrams in text form,
 e.g. for the purpose of outputting them graphically in a terminal.
 
 """
 
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, InitVar
 from enum import Enum
 
 from lambeq.backend.grammar import Cup, Diagram, Word
 
 
-def diagram2str(diagram: Diagram,
-                word_spacing: int = 2,
-                use_at_separator: bool = False,
-                compress_layers: bool = True,
-                use_ascii: bool = False) -> str:
-    """Produces a string that graphically represents the input diagram
-    with text characters, without the need of first creating a printer.
-    For specific arguments, see the constructor of the
-    :py:class:`.TextDiagramPrinter` class."""
-    printer = TextDiagramPrinter(word_spacing,
-                                 use_at_separator,
-                                 compress_layers,
-                                 use_ascii)
-    return printer.diagram2str(diagram)
-
-
 class _MorphismType(Enum):
     """Enumeration for expected morphism types in a diagram."""
     ID = 0
     CUP = 1
     SWAP = 2
     START = -1
 
@@ -56,64 +40,71 @@
     """Represents a morphism. `start` and `end` refer to the original
     positions of the involved atomic types in the diagram."""
     morphism: _MorphismType
     start: int
     end: int
 
 
-class TextDiagramPrinter:
-    """A text printer for pregroup diagrams."""
+UNICODE_CHAR_SET: dict[str, str] = {
+    'BAR': '│',
+    'TOP_R_CORNER': '╮',
+    'TOP_L_CORNER': '╭',
+    'BOTTOM_L_CORNER': '╰',
+    'BOTTOM_R_CORNER': '╯',
+    'LINE': '─',
+    'DOT': '·'
+}
+
+ASCII_CHAR_SET: dict[str, str] = {
+    'BAR': '|',
+    'TOP_R_CORNER': chr(160),
+    'TOP_L_CORNER': chr(160),
+    'BOTTOM_L_CORNER': '\\',
+    'BOTTOM_R_CORNER': '/',
+    'LINE': '_',
+    'DOT': ' '
+}
 
-    UNICODE_CHAR_SET: dict[str, str] = {
-        'BAR': '│',
-        'TOP_R_CORNER': '╮',
-        'TOP_L_CORNER': '╭',
-        'BOTTOM_L_CORNER': '╰',
-        'BOTTOM_R_CORNER': '╯',
-        'LINE': '─',
-        'DOT': '·'
-    }
-
-    ASCII_CHAR_SET: dict[str, str] = {
-        'BAR': '|',
-        'TOP_R_CORNER': chr(160),
-        'TOP_L_CORNER': chr(160),
-        'BOTTOM_L_CORNER': '\\',
-        'BOTTOM_R_CORNER': '/',
-        'LINE': '_',
-        'DOT': ' '
-    }
-
-    def __init__(self,
-                 word_spacing: int = 2,
-                 use_at_separator: bool = False,
-                 compress_layers: bool = True,
-                 use_ascii: bool = False) -> None:
-        """Initialise a text diagram printer.
 
-        Parameters
-        ----------
-        word_spacing : int, default: 2
-            The number of spaces between the words of the diagrams.
-        use_at_separator : bool, default: False
-            Whether to represent types using @ as the monoidal product.
-            Otherwise, use the unicode dot character.
-        compress_layers : bool, default: True
-            Whether to draw boxes in the same layer when they can occur
-            simultaneously, otherwise, draw one box per layer.
-        use_ascii: bool, default: False
-            Whether to draw using ASCII characters only, for
-            compatibility reasons.
+@dataclass
+class DiagramTextPrinter:
+    """A text printer for all grammar diagrams.
 
-        """
-        self.word_spacing = word_spacing
-        self.use_at_separator = use_at_separator
-        self.compress_layers = compress_layers
-        self.chr_set = (self.UNICODE_CHAR_SET if not use_ascii
-                        else self.ASCII_CHAR_SET)
+    Parameters
+    ----------
+    word_spacing : int, default: 2
+        The number of spaces between the words of the diagrams.
+    use_at_separator : bool, default: False
+        Whether to represent types using @ as the monoidal product.
+        Otherwise, use the unicode dot character.
+    compress_layers : bool, default: True
+        Whether to draw boxes in the same layer when they can occur
+        simultaneously, otherwise, draw one box per layer.
+    use_ascii: bool, default: False
+        Whether to draw using ASCII characters only, for
+        compatibility reasons.
+
+    """
+
+    word_spacing: int = 2
+    use_at_separator: bool = False
+    compress_layers: bool = True
+    use_ascii: InitVar[bool] = False
+
+    def __post_init__(self, use_ascii: bool) -> None:
+        self.chr_set = (UNICODE_CHAR_SET if not use_ascii else ASCII_CHAR_SET)
+
+    def diagram2str(self, diagram: Diagram) -> str:
+        # TODO: Add text/CLI drawing for non-pregroup diagrams.
+        raise NotImplementedError()
+
+
+@dataclass
+class PregroupTextPrinter(DiagramTextPrinter):
+    """A text printer for pregroup diagrams."""
 
     def diagram2str(self, diagram: Diagram) -> str:
         """Produces a string that contains a graphical representation of
         the input diagram using text characters. The diagram is expected
         to be in pregroup form, i.e. all words must precede morphisms.
 
         Parameters
@@ -206,27 +197,27 @@
             if isinstance(box, Cup):
                 del scan[offset:offset + len(box.dom)]
 
         # draw layers
         print_rows = []
         wires = {i: n for i, n in enumerate(pos)}
         for layer in layers:
-            print_rows += self.draw_layer(layer, wires)
+            print_rows += self._draw_layer(layer, wires)
             for morphism in layer:
                 if morphism.morphism == _MorphismType.CUP:
                     del wires[morphism.start]
                     del wires[morphism.end]
 
         lines = [word_line.rstrip(), underlines, type_line.rstrip(),
                  *print_rows]
         return '\n'.join(lines)
 
-    def draw_layer(self,
-                   layer: list[_Morphism],
-                   wires: dict[int, int]) -> list[str]:
+    def _draw_layer(self,
+                    layer: list[_Morphism],
+                    wires: dict[int, int]) -> list[str]:
         # `wires` is a mapping from the index of the wire in the input
         # diagram to the location of the wire in the printed output, a
         # column index
 
         height = 1
         for morphism in layer:
             if morphism.morphism == _MorphismType.SWAP:
```

### Comparing `lambeq-0.4.0/lambeq/backend/drawing/tikz_backend.py` & `lambeq-0.4.1/lambeq/backend/drawing/tikz_backend.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/grammar.py` & `lambeq-0.4.1/lambeq/backend/grammar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1174,14 +1174,43 @@
         if draw_as_pregroup and self.is_pregroup:
             from lambeq.backend.drawing import draw_pregroup
             draw_pregroup(self, **kwargs)
         else:
             from lambeq.backend.drawing import draw
             draw(self, **kwargs)
 
+    def render_as_str(self, **kwargs: Any) -> str:
+        """Render the diagram as text.
+
+        Presently only implemented for pregroup diagrams.
+
+        Parameters
+        ----------
+        word_spacing : int, default: 2
+            The number of spaces between the words of the diagrams.
+        use_at_separator : bool, default: False
+            Whether to represent types using @ as the monoidal product.
+            Otherwise, use the unicode dot character.
+        compress_layers : bool, default: True
+            Whether to draw boxes in the same layer when they can occur
+            simultaneously, otherwise, draw one box per layer.
+        use_ascii: bool, default: False
+            Whether to draw using ASCII characters only, for
+            compatibility reasons.
+
+        Returns
+        -------
+        str
+            Drawing of diagram in string format.
+
+        """
+
+        from lambeq.backend.drawing import render_as_str
+        return render_as_str(self, **kwargs)
+
     def apply_functor(self, functor: Functor) -> Diagram:
         assert not self.is_id
         diagram = functor(self.id(self.dom))
         for layer in self.layers:
             left, box, right = layer.unpack()
             diagram >>= (functor(self.id(left))
                          @ functor(box).to_diagram()
```

### Comparing `lambeq-0.4.0/lambeq/backend/numerical_backend.py` & `lambeq-0.4.1/lambeq/backend/numerical_backend.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/pennylane.py` & `lambeq-0.4.1/lambeq/backend/pennylane.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/quantum.py` & `lambeq-0.4.1/lambeq/backend/quantum.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,15 +518,17 @@
                     for scan in (q_scan1, q_scan2):
                         (scan[q_offset],
                          scan[q_offset + 1]) = (scan[q_offset + 1],
                                                 scan[q_offset])
                 else:
                     utensor = box.array
                     node1 = tn.Node(utensor + 0j, 'q1_' + str(box))
-                    node2 = tn.Node(np.conj(utensor) + 0j, 'q2_' + str(box))
+                    with backend() as np:
+                        node2 = tn.Node(np.conj(utensor) + 0j,
+                                        'q2_' + str(box))
 
                     for i in range(len(box.dom)):
                         tn.connect(q_scan1[q_offset + i], node1[i])
                         tn.connect(q_scan2[q_offset + i], node2[i])
 
                     q_scan1[q_offset:q_offset
                             + len(box.dom)] = node1[len(box.dom):]
```

### Comparing `lambeq-0.4.0/lambeq/backend/snake_removal.py` & `lambeq-0.4.1/lambeq/backend/snake_removal.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/backend/tensor.py` & `lambeq-0.4.1/lambeq/backend/tensor.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/__init__.py` & `lambeq-0.4.1/lambeq/bobcat/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/fast_int_enum.py` & `lambeq-0.4.1/lambeq/bobcat/fast_int_enum.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/grammar.py` & `lambeq-0.4.1/lambeq/bobcat/grammar.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/lexicon.py` & `lambeq-0.4.1/lambeq/bobcat/lexicon.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/parser.py` & `lambeq-0.4.1/lambeq/bobcat/parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/rules.py` & `lambeq-0.4.1/lambeq/bobcat/rules.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/tagger.py` & `lambeq-0.4.1/lambeq/bobcat/tagger.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/bobcat/tree.py` & `lambeq-0.4.1/lambeq/bobcat/tree.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/cli.py` & `lambeq-0.4.1/lambeq/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 import yaml
 
 import lambeq
 from lambeq.ansatz import BaseAnsatz
 from lambeq.ansatz.circuit import CircuitAnsatz, IQPAnsatz
 from lambeq.ansatz.tensor import MPSAnsatz, SpiderAnsatz, TensorAnsatz
 from lambeq.backend import grammar, tensor
-from lambeq.backend.drawing import text_printer
 from lambeq.rewrite import RemoveSwapsRewriter
 from lambeq.text2diagram.base import Reader
 from lambeq.text2diagram.bobcat_parser import BobcatParser
 from lambeq.text2diagram.ccg_parser import CCGParser
 from lambeq.text2diagram.ccg_tree import CCGTree
 from lambeq.text2diagram.depccg_parser import DepCCGParser
 from lambeq.text2diagram.linear_reader import (cups_reader,
@@ -547,17 +546,19 @@
 
             # with open(cl_args.output_file, 'w') as f:
             #     json.dump([d.to_tree() for d in module_input], f)
 
             raise NotImplementedError('JSON output is currently disabled. '
                                       'Use option `pickle` instead.')
         elif cl_args.output_format in ['text-ascii', 'text-unicode']:
-            printer = text_printer.TextDiagramPrinter(use_ascii=(
-                                    cl_args.output_format == 'text-ascii'))
-            ascii_art = [printer.diagram2str(diag) for diag in module_input]
+            use_ascii = cl_args.output_format == 'text-ascii'
+            ascii_art = [
+                diag.render_as_str(use_ascii=use_ascii)
+                for diag in module_input
+            ]
             if cl_args.output_file is not None:
                 with open(cl_args.output_file, 'w') as f:
                     f.write('\n'.join(ascii_art))
             else:
                 print('\n'.join(ascii_art))
         elif cl_args.output_format == 'pickle':
             if cl_args.output_file is not None:
```

### Comparing `lambeq-0.4.0/lambeq/core/globals.py` & `lambeq-0.4.1/lambeq/core/globals.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     .. list-table:: Available Options
         :widths: 25 25 50
         :header-rows: 1
 
         * - Option
           - Value
           - Description
-        * - PROGESS
+        * - PROGRESS
           - :py:obj:`'progress'`
           - Use progress bar.
         * - TEXT
           - :py:obj:`'text'`
           - Give text report.
         * - SUPPRESS
           - :py:obj:`'suppress'`
```

### Comparing `lambeq-0.4.0/lambeq/core/types.py` & `lambeq-0.4.1/lambeq/core/types.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/core/utils.py` & `lambeq-0.4.1/lambeq/core/utils.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/rewrite/__init__.py` & `lambeq-0.4.1/lambeq/rewrite/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/rewrite/base.py` & `lambeq-0.4.1/lambeq/rewrite/base.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/rewrite/rewrite_diagram.py` & `lambeq-0.4.1/lambeq/rewrite/rewrite_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,18 +375,14 @@
 
         new_diag = Id(diagram.dom)
         for box, offset in zip(new_words+new_morphisms,
                                wrd_offsets+mor_offsets):
             new_diag = new_diag.then_at(box, offset)
 
         return new_diag
-        # return Diagram.decode(dom=diagram.dom,
-        #                       cod=diagram.cod,
-        #                       boxes=new_words+new_morphisms,
-        #                       offsets=wrd_offsets+mor_offsets)
 
     def rewrite(self, diagram: Diagram) -> Diagram:
         atomic_types = [ob for b in diagram.boxes
                         for ob in b.cod if isinstance(b, Word)]
         scan = list(range(len(atomic_types)))
 
         # Create lists with offset info for words and morphisms
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/__init__.py` & `lambeq-0.4.1/lambeq/text2diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/text2diagram/base.py` & `lambeq-0.4.1/lambeq/text2diagram/base.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/text2diagram/bobcat_parser.py` & `lambeq-0.4.1/lambeq/text2diagram/bobcat_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,16 +307,18 @@
         """Transform a Bobcat category into a biclosed type."""
 
         if cat.atomic:
             if cat.atom.is_punct:
                 return CCGType.PUNCTUATION
             else:
                 atom = str(cat.atom)
-                if atom in ('N', 'NP'):
+                if atom == 'N':
                     return CCGType.NOUN
+                elif atom == 'NP':
+                    return CCGType.NOUN_PHRASE
                 elif atom == 'S':
                     return CCGType.SENTENCE
                 elif atom == 'PP':
                     return CCGType.PREPOSITIONAL_PHRASE
                 elif atom == 'conj':
                     return CCGType.CONJUNCTION
             raise ValueError(f'Invalid atomic type: {cat.atom!r}')
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/ccg_parser.py` & `lambeq-0.4.1/lambeq/text2diagram/ccg_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,31 +120,36 @@
                             tokenised=tokenised,
                             verbose=VerbosityLevel.SUPPRESS.value)[0]
 
     def sentences2diagrams(self,
                            sentences: SentenceBatchType,
                            tokenised: bool = False,
                            planar: bool = False,
+                           collapse_noun_phrases: bool = True,
                            suppress_exceptions: bool = False,
                            verbose: str | None = None) -> list[Diagram | None]:
         """Parse multiple sentences into a list of lambeq diagrams.
 
         Parameters
         ----------
         sentences : list of str, or list of list of str
             The sentences to be parsed.
+        tokenised : bool, default: False
+            Whether each sentence has been passed as a list of tokens.
         planar : bool, default: False
             Force diagrams to be planar when they contain
             crossed composition.
+        collapse_noun_phrases : bool, default: True
+            If set, then before converting each tree to a diagram, any
+            noun phrase types in the tree are changed into nouns. This
+            includes sub-types, e.g. `S/NP` becomes `S/N`.
         suppress_exceptions : bool, default: False
             Whether to suppress exceptions. If :py:obj:`True`, then if a
             sentence fails to parse, instead of raising an exception,
             its return entry is :py:obj:`None`.
-        tokenised : bool, default: False
-            Whether each sentence has been passed as a list of tokens.
         verbose : str, optional
             See :py:class:`VerbosityLevel` for options. Not all parsers
             implement all three levels of progress reporting, see the
             respective documentation for each parser. If set, takes
             priority over the :py:attr:`verbose` attribute of the
             parser.
 
@@ -155,56 +160,66 @@
             exceptions are suppressed.
 
         """
         trees = self.sentences2trees(sentences,
                                      suppress_exceptions=suppress_exceptions,
                                      tokenised=tokenised,
                                      verbose=verbose)
-        diagrams = []
+        diagrams: list[Diagram | None] = []
         if verbose is None:
             verbose = self.verbose
         if verbose is VerbosityLevel.TEXT.value:
             print('Turning parse trees to diagrams.', file=sys.stderr)
         for tree in tqdm(
                 trees,
                 desc='Parse trees to diagrams',
                 leave=False,
                 disable=verbose != VerbosityLevel.PROGRESS.value):
             if tree is not None:
                 try:
-                    diagrams.append(tree.to_diagram(planar=planar))
+                    diagram = tree.to_diagram(
+                        planar=planar,
+                        collapse_noun_phrases=collapse_noun_phrases
+                    )
                 except Exception as e:
                     if suppress_exceptions:
                         diagrams.append(None)
                     else:
                         raise e
+                else:
+                    diagrams.append(diagram)
             else:
                 diagrams.append(None)
         return diagrams
 
     def sentence2diagram(self,
                          sentence: SentenceType,
                          tokenised: bool = False,
                          planar: bool = False,
+                         collapse_noun_phrases: bool = True,
                          suppress_exceptions: bool = False) -> Diagram | None:
         """Parse a sentence into a lambeq diagram.
 
         Parameters
         ----------
         sentence : str or list of str
             The sentence to be parsed.
+        tokenised : bool, default: False
+            Whether the sentence has been passed as a list of tokens.
         planar : bool, default: False
             Force diagrams to be planar when they contain
             crossed composition.
+        collapse_noun_phrases : bool, default: True
+            If set, then before converting the tree to a diagram, all
+            noun phrase types in the tree are changed into nouns. This
+            includes sub-types, e.g. `S/NP` becomes `S/N`.
         suppress_exceptions : bool, default: False
             Whether to suppress exceptions. If :py:obj:`True`, then if
             the sentence fails to parse, instead of raising an
             exception, returns :py:obj:`None`.
-        tokenised : bool, default: False
-            Whether the sentence has been passed as a list of tokens.
 
         Returns
         -------
         :py:class:`lambeq.backend.grammar.Diagram` or None
             The parsed diagram, or :py:obj:`None` on failure.
 
         """
@@ -213,20 +228,22 @@
                 raise ValueError('`tokenised` set to `True`, but variable '
                                  '`sentence` does not have type '
                                  '`list[str]`.')
             sent: list[str] = [str(token) for token in sentence]
             return self.sentences2diagrams(
                             [sent],
                             planar=planar,
+                            collapse_noun_phrases=collapse_noun_phrases,
                             suppress_exceptions=suppress_exceptions,
                             tokenised=tokenised,
                             verbose=VerbosityLevel.SUPPRESS.value)[0]
         else:
             if not isinstance(sentence, str):
                 raise ValueError('`tokenised` set to `False`, but variable '
                                  '`sentence` does not have type `str`.')
             return self.sentences2diagrams(
                             [sentence],
                             planar=planar,
+                            collapse_noun_phrases=collapse_noun_phrases,
                             suppress_exceptions=suppress_exceptions,
                             tokenised=tokenised,
                             verbose=VerbosityLevel.SUPPRESS.value)[0]
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/ccg_rule.py` & `lambeq-0.4.1/lambeq/text2diagram/ccg_rule.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/text2diagram/ccg_tree.py` & `lambeq-0.4.1/lambeq/text2diagram/ccg_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,14 +332,30 @@
 
         if not vertical:
             deriv = self._horiz_deriv(chr_set, word_spacing, use_slashes)
         else:
             deriv = self._vert_deriv(chr_set, use_slashes, '')
         return deriv
 
+    def collapse_noun_phrases(self) -> CCGTree:
+        """Change noun phrase types into noun types.
+
+        This includes sub-types, e.g. `S/NP` becomes `S/N`.
+
+        """
+        return type(self)(
+            text=self._text,
+            rule=self.rule,
+            biclosed_type=self.biclosed_type.replace(CCGType.NOUN_PHRASE,
+                                                     CCGType.NOUN),
+            children=[child.collapse_noun_phrases()
+                      for child in self.children],
+            metadata=self.metadata
+        )
+
     def _resolved(self, resolved_output: CCGType | None = None) -> CCGTree:
         """Perform type resolution on the tree.
 
         Actions:
         - unary rules (for the most part) are removed and the types are
         changed directly, resulting in changes in the lexical word
         types.
@@ -408,24 +424,29 @@
             for i, child in enumerate(self.children)
         ]
         if children == self.children and output == self.biclosed_type:
             return self
         else:
             return CCGTree(rule=rule, biclosed_type=output, children=children)
 
-    def to_diagram(self, planar: bool = False) -> Diagram:
+    def to_diagram(self,
+                   planar: bool = False,
+                   collapse_noun_phrases: bool = True) -> Diagram:
         """Convert tree to a DisCoCat diagram.
 
         Parameters
         ----------
         planar : bool, default: False
             Force the diagram to be planar. This only affects trees
             using cross composition.
 
         """
+        if collapse_noun_phrases:
+            self = self.collapse_noun_phrases()
+
         words, grammar = self._resolved()._to_diagram(planar)
         return words >> grammar
 
     def _to_diagram(self, planar: bool = False) -> tuple[Diagram, Diagram]:
         if self.rule == CCGRule.LEXICAL:
             if self.biclosed_type == CCGType.PUNCTUATION:
                 return Id(), Id()
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/ccg_type.py` & `lambeq-0.4.1/lambeq/text2diagram/ccg_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,14 +383,26 @@
                     f'input ended with unmatched "(" at index {start}'
                 )
             assert cat[end] == ')'
             end += 1
 
         return biclosed_type, end
 
+    def replace(self, original: CCGType, replacement: CCGType) -> CCGType:
+        """Replace all occurrences of a sub-type with a different type."""
+
+        if self == original:
+            return replacement
+        elif self.is_atomic:
+            return self
+        else:
+            new_result = self.result.replace(original, replacement)
+            new_argument = self.argument.replace(original, replacement)
+            return new_result.slash(self.direction, new_argument)
+
     def replace_result(self,
                        original: CCGType,
                        replacement: CCGType,
                        direction: str = '|') -> tuple[CCGType, CCGType | None]:
         r"""Replace the innermost category result with a new category.
 
         This performs a lenient replacement operation. This means that
@@ -545,12 +557,12 @@
             else:
                 left @= cat.left.to_grammar().r
                 cat = cat.right
         return left, cat.to_grammar(), right
 
 
 CCGType.NOUN = CCGType('n')
-CCGType.NOUN_PHRASE = CCGType('n')
+CCGType.NOUN_PHRASE = CCGType('np')
 CCGType.SENTENCE = CCGType('s')
 CCGType.PREPOSITIONAL_PHRASE = CCGType('p')
 CCGType.CONJUNCTION = CCGType('conj')
 CCGType.PUNCTUATION = CCGType('punc')
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/ccgbank_parser.py` & `lambeq-0.4.1/lambeq/text2diagram/ccgbank_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,16 +428,18 @@
 
     @staticmethod
     def _map_atomic_type(cat: str) -> str:
         match = CCGBankParser.ccg_type_regex.fullmatch(cat)
         if not match:
             raise CCGBankParseError(f'failed to parse atomic type {repr(cat)}')
         cat = match['bare_cat'] or cat
-        if cat in ('N', 'NP'):
+        if cat == 'N':
             return CCGType.NOUN.name
+        elif cat == 'NP':
+            return CCGType.NOUN_PHRASE.name
         elif cat == 'S':
             return CCGType.SENTENCE.name
         elif cat == 'PP':
             return CCGType.PREPOSITIONAL_PHRASE.name
         elif cat == 'conj':
             return CCGType.CONJUNCTION.name
         return CCGType.PUNCTUATION.name
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/depccg_parser.py` & `lambeq-0.4.1/lambeq/text2diagram/depccg_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -342,28 +342,33 @@
                             tokenised=tokenised,
                             verbose=VerbosityLevel.PROGRESS.value)[0]
 
     def sentence2diagram(self,
                          sentence: SentenceType,
                          tokenised: bool = False,
                          planar: bool = False,
+                         collapse_noun_phrases: bool = True,
                          suppress_exceptions: bool = False) -> Diagram | None:
         """Parse a sentence into a lambeq diagram.
 
         Parameters
         ----------
         sentence : str, list[str]
             The sentence to be parsed, passed either as a string, or as
             a list of tokens.
+        tokenised : bool, default: False
+            Whether the sentence has been passed as a list of tokens.
+        collapse_noun_phrases : bool, default: True
+            If set, then before converting each tree to a diagram, all
+            noun phrase types in the tree are changed into nouns. This
+            includes sub-types, e.g. `S/NP` becomes `S/N`.
         suppress_exceptions : bool, default: False
             Whether to suppress exceptions. If :py:obj:`True`, then if
             the sentence fails to parse, instead of raising an
             exception, returns :py:obj:`None`.
-        tokenised : bool, default: False
-            Whether the sentence has been passed as a list of tokens.
 
         Returns
         -------
         :py:class:`lambeq.backend.grammar.Diagram` or None
             The parsed diagram, or :py:obj:`None` on failure.
 
         Raises
@@ -377,24 +382,26 @@
                 raise ValueError('`tokenised` set to `True`, but variable '
                                  '`sentence` does not have type '
                                  '`list[str]`.')
             sent: list[str] = [str(token) for token in sentence]
             return self.sentences2diagrams(
                             [sent],
                             planar=planar,
+                            collapse_noun_phrases=collapse_noun_phrases,
                             suppress_exceptions=suppress_exceptions,
                             tokenised=tokenised,
                             verbose=VerbosityLevel.PROGRESS.value)[0]
         else:
             if not isinstance(sentence, str):
                 raise ValueError('`tokenised` set to `False`, but variable '
                                  '`sentence` does not have type `str`.')
             return self.sentences2diagrams(
                             [sentence],
                             planar=planar,
+                            collapse_noun_phrases=collapse_noun_phrases,
                             suppress_exceptions=suppress_exceptions,
                             tokenised=tokenised,
                             verbose=VerbosityLevel.PROGRESS.value)[0]
 
     def _depccg_parse(
             self,
             sentences: list[list[str]]) -> list[list[depccg.tree.ScoredTree]]:
@@ -419,16 +426,18 @@
         return ret
 
     @staticmethod
     def _to_biclosed(cat: Category) -> CCGType:
         """Transform a depccg category into a biclosed type."""
 
         if not cat.is_functor:
-            if cat.base in ('N', 'NP'):
+            if cat.base == 'N':
                 return CCGType.NOUN
+            elif cat.base == 'NP':
+                return CCGType.NOUN_PHRASE
             if cat.base == 'S':
                 return CCGType.SENTENCE
             if cat.base == 'PP':
                 return CCGType.PREPOSITIONAL_PHRASE
             if cat.base == 'conj':
                 return CCGType.CONJUNCTION
             if cat.base in ('LRB', 'RRB') or cat.base in ',.:;':
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/linear_reader.py` & `lambeq-0.4.1/lambeq/text2diagram/linear_reader.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/text2diagram/model_downloader.py` & `lambeq-0.4.1/lambeq/text2diagram/model_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from distutils.dir_util import copy_tree
 import hashlib
 import os
 from pathlib import Path
+from shutil import copytree
 import sys
 import tarfile
 import tempfile
 from typing import IO
 import warnings
 
 import requests
@@ -205,15 +205,17 @@
                 raise ModelDownloaderError(
                     'Failed to extract compressed model {self.model}'
                 ) from e
 
             model_file.close()
 
             # Copy extracted model to model_dir
-            copy_tree(extraction_target, str(self.model_dir))
+            copytree(extraction_target,
+                     str(self.model_dir),
+                     dirs_exist_ok=True)
 
         with open(self.model_dir / VERSION_FNAME, 'w') as w:
             w.write(self.remote_version)
 
     def get_latest_remote_version(self) -> str:
         """Retrieve the latest model version number from server."""
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/spiders_reader.py` & `lambeq-0.4.1/lambeq/text2diagram/spiders_reader.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/text2diagram/tree_reader.py` & `lambeq-0.4.1/lambeq/text2diagram/tree_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,26 +176,31 @@
             children = [TreeReader._tree2diagram(child, mode, word_type)
                         for child in tree.children]
             return Id().tensor(*children) >> Box(name, dom, cod)
 
     def sentence2diagram(self,
                          sentence: SentenceType,
                          tokenised: bool = False,
+                         collapse_noun_phrases: bool = True,
                          suppress_exceptions: bool = False) -> Diagram | None:
         """Parse a sentence into a lambeq diagram.
 
         This produces a tree-shaped diagram based on the output of the
         CCG parser.
 
         Parameters
         ----------
         sentence : str or list of str
             The sentence to be parsed.
         tokenised : bool, default: False
             Whether the sentence has been passed as a list of tokens.
+        collapse_noun_phrases : bool, default: True
+            If set, then before converting each tree to a diagram, any
+            noun phrase types in the tree are changed into nouns. This
+            includes sub-types, e.g. `S/NP` becomes `S/N`.
         suppress_exceptions : bool, default: False
             Whether to suppress exceptions. If :py:obj:`True`, then if a
             sentence fails to parse, instead of raising an exception,
             its return entry is :py:obj:`None`.
 
         Returns
         -------
@@ -207,11 +212,15 @@
         tree = self.ccg_parser.sentence2tree(
             sentence=sentence,
             tokenised=tokenised,
             suppress_exceptions=suppress_exceptions)
 
         if tree is None:
             return None
+
+        if collapse_noun_phrases:
+            tree = tree.collapse_noun_phrases()
+
         return self.tree2diagram(tree,
                                  mode=self.mode,
                                  word_type=self.word_type,
                                  suppress_exceptions=suppress_exceptions)
```

### Comparing `lambeq-0.4.0/lambeq/text2diagram/web_parser.py` & `lambeq-0.4.1/lambeq/text2diagram/web_parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/tokeniser/__init__.py` & `lambeq-0.4.1/lambeq/tokeniser/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/tokeniser/base.py` & `lambeq-0.4.1/lambeq/tokeniser/base.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/tokeniser/spacy_tokeniser.py` & `lambeq-0.4.1/lambeq/tokeniser/spacy_tokeniser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/__init__.py` & `lambeq-0.4.1/lambeq/training/__init__.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/checkpoint.py` & `lambeq-0.4.1/lambeq/training/checkpoint.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/dataset.py` & `lambeq-0.4.1/lambeq/training/dataset.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/loss.py` & `lambeq-0.4.1/lambeq/training/loss.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/model.py` & `lambeq-0.4.1/lambeq/training/model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/nelder_mead_optimizer.py` & `lambeq-0.4.1/lambeq/training/nelder_mead_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/numpy_model.py` & `lambeq-0.4.1/lambeq/training/numpy_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/optimizer.py` & `lambeq-0.4.1/lambeq/training/optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/pennylane_model.py` & `lambeq-0.4.1/lambeq/training/pennylane_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/pytorch_model.py` & `lambeq-0.4.1/lambeq/training/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/pytorch_trainer.py` & `lambeq-0.4.1/lambeq/training/pytorch_trainer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/quantum_model.py` & `lambeq-0.4.1/lambeq/training/quantum_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/quantum_trainer.py` & `lambeq-0.4.1/lambeq/training/quantum_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,19 +190,23 @@
 
     def fit(self,
             train_dataset: Dataset,
             val_dataset: Dataset | None = None,
             log_interval: int = 1,
             eval_interval: int = 1,
             eval_mode: str = EvalMode.EPOCH.value,
-            early_stopping_interval: int | None = None) -> None:
+            early_stopping_criterion: str | None = None,
+            early_stopping_interval: int | None = None,
+            minimize_criterion: bool = True) -> None:
 
         self.model._training = True
 
         super().fit(train_dataset,
                     val_dataset,
                     log_interval,
                     eval_interval,
                     eval_mode,
-                    early_stopping_interval)
+                    early_stopping_criterion,
+                    early_stopping_interval,
+                    minimize_criterion)
 
         self.model._training = False
```

### Comparing `lambeq-0.4.0/lambeq/training/rotosolve_optimizer.py` & `lambeq-0.4.1/lambeq/training/rotosolve_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/spsa_optimizer.py` & `lambeq-0.4.1/lambeq/training/spsa_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq/training/tket_model.py` & `lambeq-0.4.1/lambeq/training/tket_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,18 @@
 
         fields = ('backend', 'compilation', 'shots')
         missing_fields = [f for f in fields if f not in backend_config]
         if missing_fields:
             raise KeyError('Missing arguments in backend configuation. '
                            f'Missing arguments: {missing_fields}.')
         self.backend_config = backend_config
+        self.rng = np.random.default_rng()
 
     def _randint(self, low: int = -1 << 63, high: int = (1 << 63)-1) -> int:
-        return np.random.randint(low, high, dtype=np.int64)
+        return self.rng.integers(low, high, dtype=np.int64)
 
     def get_diagram_output(self, diagrams: list[Diagram]) -> np.ndarray:
         """Return the prediction for each diagram using t|ket>.
 
         Parameters
         ----------
         diagrams : list of :py:class:`~lambeq.backend.quantum.Diagram
```

### Comparing `lambeq-0.4.0/lambeq/training/trainer.py` & `lambeq-0.4.1/lambeq/training/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -370,21 +370,67 @@
                 self._generate_stat_report(
                     train_loss=(self.train_costs[-1] if self.train_costs
                                 else None),
                     val_loss=self.val_costs[-1] if self.val_costs else None
                 )
             )
 
+    def _check_early_stopping(self,
+                              early_stopping_criterion: str | None = None,
+                              early_stopping_interval: int | None = None,
+                              minimize_criterion: bool = True) -> bool:
+        """Determine if training should be stopped based on the specified
+        early stopping configuration.
+
+        Parameters
+        ----------
+        early_stopping_criterion : str, optional
+            If specified, the value of this on `val_dataset` (if provided)
+            will be used as the stopping criterion instead of
+            the (default) validation loss.
+        early_stopping_interval : int, optional
+            If specified, training is stopped if the validation loss does
+            not improve for `early_stopping_interval` validation cycles.
+        minimize_criterion: bool, default: True
+            Flag indicating if we should minimize or maximize the early
+            stopping criterion.
+
+        Returns
+        -------
+        Boolean
+            Flag if early stopping should be performed.
+        """
+        factor = 1 if minimize_criterion else -1
+        early_stopping = False
+        criterion_vals = self.val_costs
+        if early_stopping_criterion is not None:
+            criterion_vals = self.val_eval_results[
+                early_stopping_criterion
+            ]
+        if (early_stopping_interval is not None
+                and len(criterion_vals) > early_stopping_interval):
+
+            reference = factor * criterion_vals[-early_stopping_interval - 1]
+            latter_vals = [
+                factor * val for val in
+                criterion_vals[-early_stopping_interval:]
+            ]
+            early_stopping = reference < min(latter_vals)
+
+        return early_stopping
+
     def fit(self,
             train_dataset: Dataset,
             val_dataset: Dataset | None = None,
             log_interval: int = 1,
             eval_interval: int = 1,
             eval_mode: str = EvalMode.EPOCH.value,
-            early_stopping_interval: int | None = None) -> None:
+            early_stopping_criterion: str | None = None,
+            early_stopping_interval: int | None = None,
+            minimize_criterion: bool = True) -> None:
         """Fit the model on the training data and, optionally,
         evaluate it on the validation data.
 
         Parameters
         ----------
         train_dataset : :py:class:`Dataset`
             Dataset used for training.
@@ -400,17 +446,24 @@
             is performed at the end of each epoch.
         eval_mode : :py:class:`EvalMode`, default: 'epoch'
             Sets the evaluation mode. If `'epoch'`, the metrics are
             evaluated after multiples of `eval_interval` epochs. If
             `'step'`, the metrics are evaluated after multiples of
             `eval_interval` steps. Ignored if `val_dataset` is
             `None`.
+        early_stopping_criterion : str, optional
+            If specified, the value of this on `val_dataset` (if provided)
+            will be used as the stopping criterion instead of
+            the (default) validation loss.
         early_stopping_interval : int, optional
             If specified, training is stopped if the validation loss does
             not improve for `early_stopping_interval` validation cycles.
+        minimize_criterion: bool, default: True
+            Flag indicating if we should minimize or maximize the early
+            stopping criterion.
 
         Raises
         ------
         ValueError
             If `eval_mode` is not a valid :py:class:`EvalMode`.
 
         """
@@ -421,14 +474,28 @@
         if eval_mode == EvalMode.EPOCH.value:
             evaluation_step = eval_interval * train_dataset.batches_per_epoch
         elif eval_mode == EvalMode.STEP.value:
             evaluation_step = eval_interval
         else:
             raise ValueError(f'Invalid evaluation mode: {eval_mode}.')
 
+        # check that early stopping critera is in available list
+        if (early_stopping_criterion is not None
+                and self.evaluate_functions is not None
+                and early_stopping_criterion not in self.evaluate_functions):
+            raise ValueError('Invalid early stopping criterion: '
+                             f'{early_stopping_criterion}. '
+                             'Should be one of '
+                             f'{self.evaluate_functions.keys()}')
+
+        # Used for early stopping
+        factor = 1 if minimize_criterion else -1
+        best_epoch = 0
+        best_step = 0
+
         logging_step = log_interval * evaluation_step
         total_steps = self.epochs * train_dataset.batches_per_epoch
 
         # initialise progress bar
         step = self.start_step
         if val_dataset is not None:
             batches_per_validation = ceil(
@@ -441,15 +508,15 @@
                           disable=disable_tqdm,
                           leave=True,
                           position=0)
 
         # start training loop
         with backend(self.backend):
             early_stopping = False
-            best_val_loss = float('inf')
+            best_val_criterion = float('inf')
             for epoch in trange(self.start_epoch,
                                 self.epochs + 1,
                                 desc='Epoch',
                                 disable=disable_tqdm,
                                 leave=False,
                                 position=1):
 
@@ -526,16 +593,25 @@
 
                         self._summarize_metric(self._val_eval_running,
                                                self.val_eval_results,
                                                epoch,
                                                status_bar,
                                                mode='val')
                         # save best model
-                        if self.val_costs[-1] < best_val_loss:
-                            best_val_loss = self.val_costs[-1]
+                        criterion_vals = self.val_costs
+                        if early_stopping_criterion is not None:
+                            criterion_vals = self.val_eval_results[
+                                early_stopping_criterion
+                            ]
+
+                        criterion_val = factor * criterion_vals[-1]
+                        if criterion_val < best_val_criterion:
+                            best_val_criterion = criterion_val
+                            best_epoch = epoch
+                            best_step = step
                             self.save_checkpoint(
                                 {'epoch': epoch,
                                  'train_costs': self.train_costs,
                                  'train_epoch_costs': self.train_epoch_costs,
                                  'train_eval_results': self.train_eval_results,
                                  'val_costs': self.val_costs,
                                  'val_eval_results': self.val_eval_results,
@@ -564,20 +640,21 @@
                                     train_loss=(self.train_costs[-1]
                                                 if self.train_costs else None),
                                     val_loss=(self.val_costs[-1]
                                               if self.val_costs else None)),
                                   file=sys.stderr)
 
                     # check for early stopping
-                    if (early_stopping_interval is not None
-                        and len(self.val_costs) > early_stopping_interval
-                        and self.val_costs[-early_stopping_interval - 1] < min(
-                            self.val_costs[-early_stopping_interval:])):
-                        early_stopping = True
-                        break  # inner epoch loop
+                    early_stopping = self._check_early_stopping(
+                        early_stopping_criterion,
+                        early_stopping_interval,
+                        minimize_criterion
+                    )
+                    if early_stopping:
+                        break   # inner epoch loop
 
                 # calculate epoch loss
                 self.train_epoch_costs.append(
                     self._get_weighted_mean(train_losses))
                 self._to_tensorboard('train/epoch_loss',
                                      self.train_epoch_costs[-1],
                                      epoch)
@@ -593,15 +670,16 @@
                      'random_state': random.getstate(),
                      'step': step},
                     self.log_dir)
 
                 if early_stopping:
                     if self.verbose == VerbosityLevel.TEXT.value:
                         print('Early stopping!\n'
-                              'Best model saved to '
+                              f'Best model (epoch={best_epoch}, '
+                              f'step={best_step}) saved to\n'
                               f'{os.path.join(self.log_dir, "best_model.lt")}',
                               file=sys.stderr)
                     break  # break outer epoch loop
 
         status_bar.close()
         if self.verbose == VerbosityLevel.TEXT.value:
             print('\nTraining completed!', file=sys.stderr)
```

### Comparing `lambeq-0.4.0/lambeq/typing.py` & `lambeq-0.4.1/lambeq/typing.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/lambeq.egg-info/PKG-INFO` & `lambeq-0.4.1/lambeq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambeq
-Version: 0.4.0
+Version: 0.4.1
 Summary: A QNLP toolkit
 Home-page: https://cqcl.github.io/lambeq
 Download-URL: https://pypi.org/project/lambeq
 Author: Cambridge Quantum QNLP team
 Author-email: lambeq-support@cambridgequantum.com
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/CQCL/lambeq
@@ -15,27 +15,29 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib>=3.1.2
+Requires-Dist: packaging
 Requires-Dist: pillow>=6.2.1
 Requires-Dist: pytket>=0.19.2
 Requires-Dist: pyyaml
 Requires-Dist: spacy>=3.0
 Requires-Dist: tensornetwork
 Requires-Dist: torch>=1.12.1
 Requires-Dist: transformers
 Provides-Extra: extras
-Requires-Dist: discopy==1.1.4; extra == "extras"
+Requires-Dist: discopy>=1.1.7; extra == "extras"
 Requires-Dist: jax; extra == "extras"
 Requires-Dist: jaxlib; extra == "extras"
 Requires-Dist: pennylane>=0.29.1; extra == "extras"
 Requires-Dist: pennylane-honeywell; extra == "extras"
 Requires-Dist: pennylane-qiskit; extra == "extras"
 Requires-Dist: pytket-qiskit>=0.21.0; extra == "extras"
 Requires-Dist: tensorboard>=2.7.0; extra == "extras"
```

### Comparing `lambeq-0.4.0/lambeq.egg-info/SOURCES.txt` & `lambeq-0.4.1/lambeq.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 .github/workflows/build-docs
 .github/workflows/build_test.yml
 .github/workflows/clear-target-files
 .github/workflows/docs.yml
+contrib/convert_discopy_to_lambeq.py
 contrib/download_depccg_model.py
 docs/CONTRIBUTING.rst
 docs/Makefile
 docs/advanced.rst
 docs/bibliography.rst
 docs/cli.rst
 docs/conf.py
@@ -91,14 +92,15 @@
 docs/puml/text2diagram.puml
 docs/puml/tokeniser.puml
 docs/puml/training.puml
 docs/scripts/check_errors.py
 docs/scripts/clean_notebooks.py
 docs/scripts/compare_execution_times.py
 docs/scripts/track_execution_time.sh
+docs/tutorials/config.toml
 docs/tutorials/discocat.ipynb
 docs/tutorials/extend-lambeq.ipynb
 docs/tutorials/monoidal.ipynb
 docs/tutorials/parameterise.ipynb
 docs/tutorials/rewrite.ipynb
 docs/tutorials/sentence-input.ipynb
 docs/tutorials/trainer-classical.ipynb
@@ -192,29 +194,30 @@
 tests/test_bobcat.py
 tests/test_circuit.py
 tests/test_cli.py
 tests/test_pregroups.py
 tests/test_rewrite.py
 tests/test_symbol.py
 tests/test_tensor.py
-tests/test_text_printer.py
 tests/test_tokeniser.py
 tests/test_utils.py
 tests/backend/__init__.py
 tests/backend/test_circuit_drawing.py
 tests/backend/test_drawing.py
 tests/backend/test_grammar.py
 tests/backend/test_pennylane_interface.py
 tests/backend/test_quantum.py
 tests/backend/test_rewriting.py
 tests/backend/test_tensor.py
+tests/backend/test_text_printer.py
 tests/backend/converters/__init__.py
 tests/backend/converters/test_tket_conversion.py
 tests/backend/converters/discopy/__init__.py
 tests/backend/converters/discopy/test_grammar_conversion.py
+tests/backend/converters/discopy/test_old_discopy.py
 tests/backend/converters/discopy/test_quantum_conversion.py
 tests/backend/converters/discopy/test_tensor_conversion.py
 tests/src/alice-loves-bob.png
 tests/src/alice-loves-bob.tikz
 tests/src/gave-up.png
 tests/text2diagram/__init__.py
 tests/text2diagram/test_bobcat_parser.py
```

### Comparing `lambeq-0.4.0/pyproject.toml` & `lambeq-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/setup.cfg` & `lambeq-0.4.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 packages = 
 	lambeq
 	lambeq.ansatz
 	lambeq.text2diagram
@@ -51,26 +52,27 @@
 	lambeq.bobcat
 	lambeq.core
 	lambeq.rewrite
 	lambeq.tokeniser
 	lambeq.training
 install_requires = 
 	matplotlib >= 3.1.2
+	packaging
 	pillow >= 6.2.1
 	pytket >= 0.19.2
 	pyyaml
 	spacy >= 3.0
 	tensornetwork
 	torch >= 1.12.1
 	transformers
 python_requires = >=3.9
 
 [options.extras_require]
 extras = 
-	discopy == 1.1.4
+	discopy >= 1.1.7
 	jax
 	jaxlib
 	pennylane >= 0.29.1
 	pennylane-honeywell
 	pennylane-qiskit
 	pytket-qiskit >= 0.21.0
 	tensorboard >= 2.7.0
```

### Comparing `lambeq-0.4.0/tests/backend/converters/discopy/test_grammar_conversion.py` & `lambeq-0.4.1/tests/backend/converters/discopy/test_grammar_conversion.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/converters/discopy/test_quantum_conversion.py` & `lambeq-0.4.1/tests/backend/converters/discopy/test_quantum_conversion.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/converters/discopy/test_tensor_conversion.py` & `lambeq-0.4.1/tests/backend/converters/discopy/test_tensor_conversion.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/converters/test_tket_conversion.py` & `lambeq-0.4.1/tests/backend/converters/test_tket_conversion.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_circuit_drawing.py` & `lambeq-0.4.1/tests/backend/test_circuit_drawing.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_drawing.py` & `lambeq-0.4.1/tests/backend/test_drawing.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_grammar.py` & `lambeq-0.4.1/tests/backend/test_grammar.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_pennylane_interface.py` & `lambeq-0.4.1/tests/backend/test_pennylane_interface.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_quantum.py` & `lambeq-0.4.1/tests/backend/test_quantum.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_rewriting.py` & `lambeq-0.4.1/tests/backend/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/backend/test_tensor.py` & `lambeq-0.4.1/tests/backend/test_tensor.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/src/alice-loves-bob.png` & `lambeq-0.4.1/tests/src/alice-loves-bob.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/src/alice-loves-bob.tikz` & `lambeq-0.4.1/tests/src/alice-loves-bob.tikz`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/src/gave-up.png` & `lambeq-0.4.1/tests/src/gave-up.png`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_circuit.py` & `lambeq-0.4.1/tests/test_circuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from lambeq.backend.quantum import (Bra, Diagram as Circuit, Controlled, CRx,
                                     CRz, CX, Discard, H, Ket, qubit, Rx, Ry,
                                     Rz, Sqrt, X, Id)
 from lambeq.backend.converters.tk import from_tk
 from sympy import Symbol as sym
 
 from lambeq import (AtomicType, IQPAnsatz, Sim14Ansatz, Sim15Ansatz,
-                    StronglyEntanglingAnsatz)
+                    Sim4Ansatz, StronglyEntanglingAnsatz)
 
 N = AtomicType.NOUN
 S = AtomicType.SENTENCE
 
 
 def test_iqp_ansatz():
     diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
@@ -76,14 +76,35 @@
                         Id(1) @ CX >> Id(1) @ Controlled(X, distance=-1) >>
                         CX @ Id(1) >> H @ Sqrt(2) @ Id(2) >>
                         Bra(0, 0) @ Id(1))
 
     assert ansatz(diagram) == expected_circuit
 
 
+def test_sim4_ansatz():
+    diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
+               Cup(N, N.r) @ S)
+
+    ansatz = Sim4Ansatz({N: 1, S: 1}, n_layers=1)
+    expected_circuit = (Ket(0) >>
+                        Rx(sym('Alice__n_0')) >>
+                        Rz(sym('Alice__n_1')) >>
+                        Rx(sym('Alice__n_2')) >>
+                        Id(1) @ Ket(0, 0) >>
+                        Id(1) @ Rx(sym('runs__n.r@s_0')) @ Id(1) >>
+                        Id(2) @ Rx(sym('runs__n.r@s_1')) >>
+                        Id(1) @ Rz(sym('runs__n.r@s_2')) @ Id(1) >>
+                        Id(2) @ Rz(sym('runs__n.r@s_3')) >>
+                        Id(1) @ CRx(sym('runs__n.r@s_4')) >>
+                        CX @ Id(1) >> H @ Sqrt(2) @ Id(2) >>
+                        Bra(0, 0) @ Id(1))
+
+    assert ansatz(diagram) == expected_circuit
+
+
 def test_iqp_ansatz_inverted():
     d = Box("inverted", S, Ty())
     ansatz = IQPAnsatz({N: 0, S: 0}, n_layers=1)
     assert ansatz(d) == Id()
 
 
 def test_s14_ansatz_inverted():
@@ -94,48 +115,64 @@
 
 def test_s15_ansatz_inverted():
     d = Box("inverted", S, Ty())
     ansatz = Sim15Ansatz({N: 0, S: 0}, n_layers=1)
     assert ansatz(d) == Id()
 
 
+def test_s4_ansatz_inverted():
+    d = Box("inverted", S, Ty())
+    ansatz = Sim4Ansatz({N: 0, S: 0}, n_layers=1)
+    assert ansatz(d) == Id()
+
+
 def test_iqp_ansatz_empty():
     diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
                Cup(N, N.r) @ S)
     ansatz = IQPAnsatz({N: 0, S: 0}, n_layers=1)
     assert ansatz(diagram) == Id()
 
+
 def test_s14_ansatz_empty():
     diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
                Cup(N, N.r) @ S)
     ansatz = Sim14Ansatz({N: 0, S: 0}, n_layers=1)
     assert ansatz(diagram) == Id()
 
 
 def test_s15_ansatz_empty():
     diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
                Cup(N, N.r) @ S)
     ansatz = Sim15Ansatz({N: 0, S: 0}, n_layers=1)
     assert ansatz(diagram) == Id()
 
 
+def test_s4_ansatz_empty():
+    diagram = (Word('Alice', N) @ Word('runs', N >> S) >>
+               Cup(N, N.r) @ S)
+    ansatz = Sim4Ansatz({N: 0, S: 0}, n_layers=1)
+    assert ansatz(diagram) == Id()
+
 def test_discard():
     ansatz = IQPAnsatz({S: 2}, n_layers=0, discard=True)
     assert ansatz(Box('DISCARD', S, Ty())) == Discard() @ Discard()
 
 
 def test_s14_discard():
     ansatz = Sim14Ansatz({S: 2}, n_layers=0, discard=True)
     assert ansatz(Box('DISCARD', S, Ty())) == Discard() @ Discard()
 
 
 def test_s15_discard():
     ansatz = Sim15Ansatz({S: 2}, n_layers=0, discard=True)
     assert ansatz(Box('DISCARD', S, Ty())) == Discard() @ Discard()
 
+def test_s4_discard():
+    ansatz = Sim4Ansatz({S: 2}, n_layers=0, discard=True)
+    assert ansatz(Box('DISCARD', S, Ty())) == Discard() @ Discard()
 
 def test_postselection():
     ansatz_s15 = Sim15Ansatz({N: 1}, n_layers=1)
     ansatz_iqp = IQPAnsatz({N: 1}, n_layers=1)
 
     b = Box('something', N @ N @ N, N)
```

### Comparing `lambeq-0.4.0/tests/test_cli.py` & `lambeq-0.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_pregroups.py` & `lambeq-0.4.1/tests/test_pregroups.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_rewrite.py` & `lambeq-0.4.1/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_tensor.py` & `lambeq-0.4.1/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_text_printer.py` & `lambeq-0.4.1/tests/backend/test_text_printer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pytest
 
 from lambeq.backend.grammar import Cup, Id, Swap, Ty, Word
-from lambeq import AtomicType, diagram2str, cups_reader
+from lambeq.backend.quantum import CX, H, qubit
+from lambeq.backend.tensor import Box, Dim
+from lambeq import AtomicType, cups_reader
 
 
 n = AtomicType.NOUN
 s = AtomicType.SENTENCE
 
 
 @pytest.fixture(scope="module")
@@ -72,15 +74,15 @@
                       " n    n.r·s·n.l·n.l   n    n·n.l    n     s.r·n.r.r·n.r·s·s.l·n  n.r·s  s.r·n.r.r·n.r·s\n" \
                       " │     │  │  │   ╰────╯    │  ╰─────╯      │    │    │  │  │  │   │  ╰───╯    │    │  │\n" \
                       " │     │  │  ╰─────────────╯               │    │    │  │  │  │   ╰───────────╯    │  │\n" \
                       " │     │  ╰────────────────────────────────╯    │    │  │  │  ╰────────────────────╯  │\n" \
                       " │     ╰────────────────────────────────────────╯    │  │  ╰──────────────────────────╯\n" \
                       " ╰───────────────────────────────────────────────────╯  │"
 
-    assert diagram2str(diagram1) == expected_output
+    assert diagram1.render_as_str() == expected_output
 
 
 def test_diagram_with_cups_and_swaps(diagram2):
     expected_output = "Mary      does           not           like    John\n" \
                       "────  ───────────  ───────────────  ─────────  ────\n" \
                       " n    n.r·s·s.l·n  s.r·n.r.r·n.r·s  n.r·s·n.l   n\n" \
                       " │     │  │  │  ╰─╮─╯    │    │  │   │  │  ╰────╯\n" \
@@ -91,47 +93,57 @@
                       " │     │        ╭─╰─╮    ╭─╰──╮  │   │  │\n" \
                       " │     ╰────────╯   ╰─╮──╯    ╰╮─╯   │  │\n" \
                       " │                  ╭─╰──╮    ╭╰─╮   │  │\n" \
                       " ╰──────────────────╯    ╰─╮──╯  ╰───╯  │\n" \
                       "                         ╭─╰──╮         │\n" \
                       "                         │    ╰─────────╯"
 
-    assert diagram2str(diagram2) == expected_output
+    assert diagram2.render_as_str() == expected_output
 
 
 def test_diagram_from_cups_reader():
     expected_output = "START   John   gave   Mary    a    flower\n" \
                       "─────  ─────  ─────  ─────  ─────  ──────\n" \
                       "  s    s.r·s  s.r·s  s.r·s  s.r·s  s.r·s\n" \
                       "  ╰─────╯  ╰───╯  ╰───╯  ╰───╯  ╰───╯  │"
 
     diagram = cups_reader.sentence2diagram("John gave Mary a flower")
-    assert diagram2str(diagram) == expected_output
+    assert diagram.render_as_str() == expected_output
 
 
 def test_diagram_with_just_identities_1():
     n = Ty("n")
     diagram = Word("John", cod=n) >> Id(n)
 
     expected_output = "John\n" \
                       "────\n" \
                       " n\n" \
                       " │"
 
-    assert diagram2str(diagram) == expected_output
+    assert diagram.render_as_str() == expected_output
 
 
 def test_diagram_with_just_identities_2():
     n, s = Ty("n"), Ty("s")
     diagram = Word("runs", cod=n.r @ s) >> Id((n.r @ s))
 
     expected_output = " runs\n" \
                       "─────\n" \
                       "n.r·s\n" \
                       " │  │"
 
-    assert diagram2str(diagram) == expected_output
+    assert diagram.render_as_str() == expected_output
 
 
 def test_diagram_no_pregroup(diagram1):
-    with pytest.raises(ValueError):
-        diagram2str(diagram1.normal_form())
+    with pytest.raises(NotImplementedError):
+        diagram1.normal_form().render_as_str()
+
+
+def test_tensor():
+    with pytest.raises(NotImplementedError):
+        (Box("A", Dim(), Dim(3)) >> Box("A", Dim(3), Dim(4, 3))).render_as_str()
+
+
+def test_quantum():
+    with pytest.raises(NotImplementedError):
+        (H @ qubit >> CX).render_as_str()
```

### Comparing `lambeq-0.4.0/tests/test_tokeniser.py` & `lambeq-0.4.1/tests/test_tokeniser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/test_utils.py` & `lambeq-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_bobcat_parser.py` & `lambeq-0.4.1/tests/text2diagram/test_bobcat_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     with patch('sys.stderr', new=StringIO()) as fake_out:
         _=bobcat_parser.sentences2diagrams([sentence], verbose=VerbosityLevel.TEXT.value)
         assert fake_out.getvalue().rstrip() != ''
 
 
 def test_root_filtering(bobcat_parser):
     S = CCGType.SENTENCE
-    N = CCGType.NOUN
+    N = CCGType.NOUN_PHRASE
 
     sentence1 = 'do'
     sentence2 = 'I do'
     assert bobcat_parser.sentence2tree(sentence1).biclosed_type == N >> S
     assert bobcat_parser.sentence2tree(sentence2).biclosed_type == S
 
     bobcat_parser.parser.set_root_cats(['NP'])
```

### Comparing `lambeq-0.4.0/tests/text2diagram/test_ccg_parser.py` & `lambeq-0.4.1/tests/text2diagram/test_ccg_parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_ccg_rule.py` & `lambeq-0.4.1/tests/text2diagram/test_ccg_rule.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_ccg_tree.py` & `lambeq-0.4.1/tests/text2diagram/test_ccg_tree.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_ccg_type.py` & `lambeq-0.4.1/tests/text2diagram/test_ccg_type.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_ccgbank_parser.py` & `lambeq-0.4.1/tests/text2diagram/test_ccgbank_parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_depccg_parser.py` & `lambeq-0.4.1/tests/text2diagram/test_depccg_parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_model_download.py` & `lambeq-0.4.1/tests/text2diagram/test_model_download.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/text2diagram/test_reader.py` & `lambeq-0.4.1/tests/text2diagram/test_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     reader1 = TreeReader(ccg_parser=parser, mode=TreeReaderMode.RULE_ONLY)
     mode1_expect = the_words >> make_parse('FA', 'FA', 'BA')
     assert reader1.sentence2diagram(sentence) == mode1_expect
 
     reader2 = TreeReader(ccg_parser=parser, mode=TreeReaderMode.RULE_TYPE)
     mode2_expect = the_words >> make_parse('FA(n/n, n)', r'FA((s\n)/n, n)', r'BA(n, s\n)')
     assert reader2.sentence2diagram(sentence) == mode2_expect
+    mode2_expect_np = the_words >> make_parse('FA(np/n, n)', r'FA((s\np)/np, np)', r'BA(np, s\np)')
+    assert reader2.sentence2diagram(sentence, collapse_noun_phrases=False) == mode2_expect_np
 
     reader3 = TreeReader(ccg_parser=parser, mode=TreeReaderMode.HEIGHT)
     mode3_expect = the_words >> make_parse('layer_1', 'layer_2', 'layer_3')
     assert reader3.sentence2diagram(sentence) == mode3_expect
 
 def test_suppress_exceptions(sentence):
     bad_parser = WebParser()
```

### Comparing `lambeq-0.4.0/tests/text2diagram/test_web_parser.py` & `lambeq-0.4.1/tests/text2diagram/test_web_parser.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_chckpoint.py` & `lambeq-0.4.1/tests/training/test_chckpoint.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_dataset.py` & `lambeq-0.4.1/tests/training/test_dataset.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_loss.py` & `lambeq-0.4.1/tests/training/test_loss.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_model.py` & `lambeq-0.4.1/tests/training/test_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_nelder_mead_optimizer.py` & `lambeq-0.4.1/tests/training/test_nelder_mead_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_numpy_model.py` & `lambeq-0.4.1/tests/training/test_numpy_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pickle
 import pytest
 from copy import deepcopy
 from unittest.mock import mock_open, patch
 
 import numpy as np
 from lambeq.backend.grammar import Cup, Id, Word
-from lambeq.backend.quantum import CRz, CX, H, Ket, Measure, SWAP
+from lambeq.backend.quantum import CRz, CX, Discard, H, Ket, Measure, SWAP, qubit
 
 from lambeq import AtomicType, IQPAnsatz, NumpyModel, Symbol
 
 def test_init():
     N = AtomicType.NOUN
     S = AtomicType.SENTENCE
 
@@ -42,14 +42,28 @@
     diagrams = [ansatz((Word("Alice", N) @ Word("runs", N >> S) >> Cup(N, N.r) @ Id(S)))]
     model = NumpyModel.from_diagrams(diagrams, use_jit=True)
     model.initialise_weights()
     pred = model.forward(diagrams)
     assert pred.shape == (len(diagrams), s_dim)
 
 
+def test_jax_forward_mixed():
+    N = AtomicType.NOUN
+    S = AtomicType.SENTENCE
+
+    density_matrix_dim = (2, 2, 2, 2)
+    ansatz = IQPAnsatz({N: 1, S: 1}, n_layers=1)
+    diagrams = [ansatz((Word("Alice", N) @ Word("runs", N >> S))) >> (Discard() @ qubit @ qubit)]
+    model = NumpyModel.from_diagrams(diagrams, use_jit=True)
+    model.initialise_weights()
+    pred = model.forward(diagrams)
+
+    assert pred.shape == (len(diagrams), *density_matrix_dim)
+
+
 def test_lambda_error():
     N = AtomicType.NOUN
     S = AtomicType.SENTENCE
     ansatz = IQPAnsatz({N: 1, S: 1}, n_layers=1)
     diagram = ansatz((Word("Alice", N) @ Word("runs", N >> S) >> Cup(N, N.r) @ Id(S)))
     with pytest.raises(ValueError):
         model = NumpyModel()
```

### Comparing `lambeq-0.4.0/tests/training/test_pennylane_model.py` & `lambeq-0.4.1/tests/training/test_pennylane_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_pytorch_model.py` & `lambeq-0.4.1/tests/training/test_pytorch_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_pytorch_trainer.py` & `lambeq-0.4.1/tests/training/test_pytorch_trainer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from math import ceil
+import time
 
 import torch
 import numpy as np
 
 from lambeq.backend.grammar import Cup, Id, Word
 from lambeq.backend.tensor import Dim
 
@@ -58,14 +59,15 @@
     val_dataset = Dataset(dev_circuits, dev_targets)
 
     trainer.fit(train_dataset, val_dataset)
 
     assert len(trainer.train_costs) == EPOCHS
     assert len(trainer.val_eval_results["acc"]) == EPOCHS
 
+
 def test_restart_training(tmp_path):
     model = PytorchModel.from_diagrams(train_circuits + dev_circuits)
     log_dir = tmp_path / 'test_run'
     log_dir.mkdir()
     trainer = PytorchTrainer(
         model=model,
         loss_function=torch.nn.BCEWithLogitsLoss(),
@@ -124,14 +126,15 @@
     assert len(trainer_restarted.val_eval_results["acc"]) == EPOCHS+1
     assert len(trainer_restarted.train_eval_results["acc"]) == EPOCHS+1
     for a, b in zip(trainer_restarted.train_costs, trainer_uninterrupted.train_costs):
         assert np.isclose(a, b)
     for a, b in zip(model_new.weights, model_uninterrupted.weights):
         assert torch.allclose(a, b)
 
+
 def test_evaluation_skipping(tmp_path):
     model = PytorchModel.from_diagrams(train_circuits + dev_circuits)
     log_dir = tmp_path / 'test_run'
     epochs = 4
     eval_step = 2
     trainer = PytorchTrainer(
         model=model,
@@ -150,7 +153,76 @@
     train_dataset = Dataset(train_circuits, train_targets)
     val_dataset = Dataset(dev_circuits, dev_targets)
 
     trainer.fit(train_dataset, val_dataset, eval_interval=eval_step)
 
     assert len(trainer.train_costs) == epochs
     assert len(trainer.val_eval_results["acc"]) == ceil(epochs/eval_step)
+
+
+def test_early_stopping(tmp_path):
+    model = PytorchModel.from_diagrams(train_circuits + dev_circuits)
+    log_dir = tmp_path / 'test_run'
+    epochs = 100
+    inc_function = lambda _, __: time.time() * 1e-10
+    eval_step = 1
+    trainer = PytorchTrainer(
+        model=model,
+        loss_function=torch.nn.BCEWithLogitsLoss(),
+        optimizer=torch.optim.AdamW,
+        learning_rate=3e-3,
+        epochs=epochs,
+        evaluate_functions={"acc": inc_function},
+        evaluate_on_train=True,
+        use_tensorboard=True,
+        log_dir=log_dir,
+        verbose='suppress',
+        seed=0
+    )
+
+    train_dataset = Dataset(train_circuits, train_targets)
+    val_dataset = Dataset(dev_circuits, dev_targets)
+
+
+    trainer.fit(train_dataset, val_dataset,
+                eval_interval=eval_step,
+                early_stopping_criterion="acc",
+                early_stopping_interval=5)
+
+
+    assert len(trainer.val_eval_results["acc"]) == 6
+    assert len(trainer.train_costs) == 6
+
+
+def test_early_stopping_max(tmp_path):
+    model = PytorchModel.from_diagrams(train_circuits + dev_circuits)
+    log_dir = tmp_path / 'test_run'
+    epochs = 100
+    dec_function = lambda _, __: -time.time() * 1e-10
+    eval_step = 1
+    trainer = PytorchTrainer(
+        model=model,
+        loss_function=torch.nn.BCEWithLogitsLoss(),
+        optimizer=torch.optim.AdamW,
+        learning_rate=3e-3,
+        epochs=epochs,
+        evaluate_functions={"acc": dec_function},
+        evaluate_on_train=True,
+        use_tensorboard=True,
+        log_dir=log_dir,
+        verbose='suppress',
+        seed=0
+    )
+
+    train_dataset = Dataset(train_circuits, train_targets)
+    val_dataset = Dataset(dev_circuits, dev_targets)
+
+
+    trainer.fit(train_dataset, val_dataset,
+                eval_interval=eval_step,
+                early_stopping_criterion="acc",
+                early_stopping_interval=10,
+                minimize_criterion=False)
+
+
+    assert len(trainer.val_eval_results["acc"]) == 11
+    assert len(trainer.train_costs) == 11
```

### Comparing `lambeq-0.4.0/tests/training/test_quantum_trainer.py` & `lambeq-0.4.1/tests/training/test_quantum_trainer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_rotosolve_optimizer.py` & `lambeq-0.4.1/tests/training/test_rotosolve_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_spsa_optimizer.py` & `lambeq-0.4.1/tests/training/test_spsa_optimizer.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_tket_model.py` & `lambeq-0.4.1/tests/training/test_tket_model.py`

 * *Files identical despite different names*

### Comparing `lambeq-0.4.0/tests/training/test_trainer.py` & `lambeq-0.4.1/tests/training/test_trainer.py`

 * *Files identical despite different names*

