# Comparing `tmp/py_irt-0.6.1.tar.gz` & `tmp/py_irt-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_irt-0.6.1.tar", max compression
+gzip compressed data, was "py_irt-0.6.2.tar", max compression
```

## Comparing `py_irt-0.6.1.tar` & `py_irt-0.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1121 2024-03-13 22:49:12.851243 py_irt-0.6.1/LICENSE
--rw-r--r--   0        0        0     4902 2024-03-13 22:49:12.851243 py_irt-0.6.1/README.md
--rw-r--r--   0        0        0       16 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/__init__.py
--rw-r--r--   0        0        0    10500 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/cli.py
--rw-r--r--   0        0        0     1852 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/config.py
--rw-r--r--   0        0        0     5469 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/dataset.py
--rw-r--r--   0        0        0     3581 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/initializers.py
--rw-r--r--   0        0        0     3102 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/io.py
--rw-r--r--   0        0        0        0 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/__init__.py
--rw-r--r--   0        0        0     2770 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/abstract_model.py
--rw-r--r--   0        0        0    11158 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/amortized_1pl.py
--rw-r--r--   0        0        0     9746 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/four_param_logistic.py
--rw-r--r--   0        0        0     9457 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/multidim_2pl.py
--rw-r--r--   0        0        0    10941 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/one_param_logistic.py
--rw-r--r--   0        0        0    10151 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/three_param_logistic.py
--rw-r--r--   0        0        0     9961 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/tutorial_model.py
--rw-r--r--   0        0        0    12418 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/models/two_param_logistic.py
--rw-r--r--   0        0        0     2713 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/scoring.py
--rw-r--r--   0        0        0     8747 2024-03-13 22:49:12.851243 py_irt-0.6.1/py_irt/training.py
--rw-r--r--   0        0        0      996 2024-03-26 18:20:26.702494 py_irt-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 py_irt-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1142 2024-04-11 17:28:01.284874 py_irt-0.6.2/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-11 17:28:01.288878 py_irt-0.6.2/py_irt/__init__.py
+-rw-r--r--   0        0        0    10814 2024-04-11 17:28:01.288878 py_irt-0.6.2/py_irt/cli.py
+-rw-r--r--   0        0        0     1898 2024-04-11 17:28:01.289879 py_irt-0.6.2/py_irt/config.py
+-rw-r--r--   0        0        0    11542 2024-04-11 17:28:01.289879 py_irt-0.6.2/py_irt/dataset.py
+-rw-r--r--   0        0        0     3677 2024-04-11 17:28:01.289879 py_irt-0.6.2/py_irt/initializers.py
+-rw-r--r--   0        0        0     3201 2024-04-11 17:28:01.290878 py_irt-0.6.2/py_irt/io.py
+-rw-r--r--   0        0        0      395 2024-04-11 17:28:01.290878 py_irt-0.6.2/py_irt/models/__init__.py
+-rw-r--r--   0        0        0     3462 2024-04-11 17:28:01.290878 py_irt-0.6.2/py_irt/models/abstract_model.py
+-rw-r--r--   0        0        0    11422 2024-04-11 17:28:01.290878 py_irt-0.6.2/py_irt/models/amortized_1pl.py
+-rw-r--r--   0        0        0    10002 2024-04-11 17:28:01.291879 py_irt-0.6.2/py_irt/models/four_param_logistic.py
+-rw-r--r--   0        0        0     9709 2024-04-11 17:28:01.291879 py_irt-0.6.2/py_irt/models/multidim_2pl.py
+-rw-r--r--   0        0        0    11212 2024-04-11 17:28:01.291879 py_irt-0.6.2/py_irt/models/one_param_logistic.py
+-rw-r--r--   0        0        0    10425 2024-04-11 17:28:01.291879 py_irt-0.6.2/py_irt/models/three_param_logistic.py
+-rw-r--r--   0        0        0    10241 2024-04-11 17:28:01.292879 py_irt-0.6.2/py_irt/models/tutorial_model.py
+-rw-r--r--   0        0        0    12728 2024-04-11 17:28:01.292879 py_irt-0.6.2/py_irt/models/two_param_logistic.py
+-rw-r--r--   0        0        0     2786 2024-04-11 17:28:01.292879 py_irt-0.6.2/py_irt/scoring.py
+-rw-r--r--   0        0        0     8982 2024-04-11 17:28:01.292879 py_irt-0.6.2/py_irt/training.py
+-rw-r--r--   0        0        0     1045 2024-04-11 17:28:19.409635 py_irt-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5042 2024-04-11 17:28:01.284874 py_irt-0.6.2/README.md
+-rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 py_irt-0.6.2/PKG-INFO
```

### Comparing `py_irt-0.6.1/LICENSE` & `py_irt-0.6.2/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `py_irt-0.6.1/README.md` & `py_irt-0.6.2/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-[![Build Status](https://travis-ci.com/nd-ball/py-irt.svg?branch=master)](https://travis-ci.com/nd-ball/py-irt)
-[![codecov.io](https://codecov.io/gh/nd-ball/py-irt/coverage.svg?branch=master)](https://codecov.io/gh/nd-ball/py-irt)
-
-# py-irt
-
-Bayesian IRT models in Python
-
-## Overview
-
-This repository includes code for fitting Item Response Theory (IRT) models using variational inference.
-
-At present, the one parameter logistic (1PL) model, aka Rasch model, two parameter logistic model (2PL) and four parameter logistic model (4PL) have been implemented.
-The user can specify whether vague or hierarchical priors are used.
-The three-parameter logistic model is in the pipeline and will be added when available.
-
-## License
-
-py-irt is licensed under the [MIT license](https://opensource.org/licenses/MIT).
-
-## Installation
-
-py-irt is now available on PyPi!
-
-### Pre-reqs
-
-1. Install [PyTorch](https://pytorch.org/get-started/locally/).
-2. Install [Pyro](https://pyro.ai/)
-3. Install py-irt:
-
-```shell
-pip install py-irt
-```
-
-OR
-
-Install [Poetry](https://python-poetry.org/docs/#installation)
-
-```shell
-git clone https://github.com/nd-ball/py-irt.git
-cd py-irt
-poetry install
-```
-
-## Usage
-
-Once you install from PyPI, you can use the following command to fit an IRT
-model on the scored predictions of a dataset. For example, if you were to run py-irt with the 4PL model on the scored predictions of different transformer models on the SQuAD dataset, you'd do this:
-`py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`
-
-## FAQ
-
-1. What kind of output should I expect on running the command to train an IRT model?
-
-You should see something like this when you run the command given above:
-![image](https://user-images.githubusercontent.com/40918514/123986740-3eccd100-d9cf-11eb-8e58-ba5ad6c977ce.png)
-
-2. I tried installing py-irt using pip from PyPI. But when I try to run the command `py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`, I get an error that says `bash: py-irt: command not found`. How do I fix this?
-
-The CLI interface was implemented in PyPi version 0.2.1. If you are getting this error try updating py-irt:
-
-`pip install --upgrade py-irt`
-
-Alternatively, you can install the latest version from github:
-
-```shell
-git clone https://github.com/nd-ball/py-irt.git
-cd py-irt
-mv ~/py-irt/py_irt/cli.py ~/py-irt/
-python cli.py train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/
-```
-
-3. How do I evaluate a trained IRT model?
-
-If you have already trained an IRT model you can use the following command:
-
-`py-irt evaluate 4pl ~/path/to/data/best_parameters.json ~/path/to/data/test_pairs.jsonlines /path/to/output/eg/test-4pl/`
-
-Where `test_pairs.jsonlines` is a jsonlines file with the following format:
-
-```
-{"subject_id": "ken", "item_id": "q1"}
-{"subject_id": "ken", "item_id": "q2"}
-{"subject_id": "burt", "item_id": "q1"}
-{"subject_id": "burt", "item_id": "q3"}
-```
-
-If you would like to both train and evaluate a model you can use the following command:
-
-`py-irt train-and-evaluate 4pl ~/path/to/data/squad.jsonlines /path/to/output/eg/test-4pl/`
-
-By default this will train a model with 90% of the provided data and evaluate with the remaining 10%.
-To change this behavior you can add `--evaluation all` to the command above. 
-The model will train and evaluate against all of the data.
-
-## Citations
-
-If you use this code, please consider citing the following papers:
-
-```shell
-@inproceedings{lalor2019emnlp,
-  author    = {Lalor, John P and Wu, Hao and Yu, Hong},
-  title     = {Learning Latent Parameters without Human Response Patterns: Item Response Theory with Artificial Crowds},
-  year      = {2019},
-  booktitle = {Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing},
-}
-```
-
-```shell
-@inproceedings{rodriguez2021evaluation,
-  title={Evaluation Examples Are Not Equally Informative: How Should That Change NLP Leaderboards?},
-  author={Rodriguez, Pedro and Barrow, Joe and Hoyle, Alexander Miserlis and Lalor, John P and Jia, Robin and Boyd-Graber, Jordan},
-  booktitle={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},
-  pages={4486--4503},
-  year={2021}
-}
-```
-
-Implementation is based on the following paper:
-
-```shell
-@article{natesan2016bayesian,
-  title={Bayesian prior choice in IRT estimation using MCMC and variational Bayes},
-  author={Natesan, Prathiba and Nandakumar, Ratna and Minka, Tom and Rubright, Jonathan D},
-  journal={Frontiers in psychology},
-  volume={7},
-  pages={1422},
-  year={2016},
-  publisher={Frontiers}
-}
-```
-
-## Contributing
-
-This is research code. Pull requests and issues are welcome!
-
-## Questions?
-
-Let me know if you have any requests, bugs, etc.
-
-Email: john.lalor@nd.edu
+[![Build Status](https://travis-ci.com/nd-ball/py-irt.svg?branch=master)](https://travis-ci.com/nd-ball/py-irt)
+[![codecov.io](https://codecov.io/gh/nd-ball/py-irt/coverage.svg?branch=master)](https://codecov.io/gh/nd-ball/py-irt)
+
+# py-irt
+
+Bayesian IRT models in Python
+
+## Overview
+
+This repository includes code for fitting Item Response Theory (IRT) models using variational inference.
+
+At present, the one parameter logistic (1PL) model, aka Rasch model, two parameter logistic model (2PL) and four parameter logistic model (4PL) have been implemented.
+The user can specify whether vague or hierarchical priors are used.
+The three-parameter logistic model is in the pipeline and will be added when available.
+
+## License
+
+py-irt is licensed under the [MIT license](https://opensource.org/licenses/MIT).
+
+## Installation
+
+py-irt is now available on PyPi!
+
+### Pre-reqs
+
+1. Install [PyTorch](https://pytorch.org/get-started/locally/).
+2. Install [Pyro](https://pyro.ai/)
+3. Install py-irt:
+
+```shell
+pip install py-irt
+```
+
+OR
+
+Install [Poetry](https://python-poetry.org/docs/#installation)
+
+```shell
+git clone https://github.com/nd-ball/py-irt.git
+cd py-irt
+poetry install
+```
+
+## Usage
+
+Once you install from PyPI, you can use the following command to fit an IRT
+model on the scored predictions of a dataset. For example, if you were to run py-irt with the 4PL model on the scored predictions of different transformer models on the SQuAD dataset, you'd do this:
+`py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`
+
+## FAQ
+
+1. What kind of output should I expect on running the command to train an IRT model?
+
+You should see something like this when you run the command given above:
+![image](https://user-images.githubusercontent.com/40918514/123986740-3eccd100-d9cf-11eb-8e58-ba5ad6c977ce.png)
+
+2. I tried installing py-irt using pip from PyPI. But when I try to run the command `py-irt train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/`, I get an error that says `bash: py-irt: command not found`. How do I fix this?
+
+The CLI interface was implemented in PyPi version 0.2.1. If you are getting this error try updating py-irt:
+
+`pip install --upgrade py-irt`
+
+Alternatively, you can install the latest version from github:
+
+```shell
+git clone https://github.com/nd-ball/py-irt.git
+cd py-irt
+mv ~/py-irt/py_irt/cli.py ~/py-irt/
+python cli.py train 4pl ~/path/to/dataset/eg/squad.jsonlines /path/to/output/eg/test-4pl/
+```
+
+3. How do I evaluate a trained IRT model?
+
+If you have already trained an IRT model you can use the following command:
+
+`py-irt evaluate 4pl ~/path/to/data/best_parameters.json ~/path/to/data/test_pairs.jsonlines /path/to/output/eg/test-4pl/`
+
+Where `test_pairs.jsonlines` is a jsonlines file with the following format:
+
+```
+{"subject_id": "ken", "item_id": "q1"}
+{"subject_id": "ken", "item_id": "q2"}
+{"subject_id": "burt", "item_id": "q1"}
+{"subject_id": "burt", "item_id": "q3"}
+```
+
+If you would like to both train and evaluate a model you can use the following command:
+
+`py-irt train-and-evaluate 4pl ~/path/to/data/squad.jsonlines /path/to/output/eg/test-4pl/`
+
+By default this will train a model with 90% of the provided data and evaluate with the remaining 10%.
+To change this behavior you can add `--evaluation all` to the command above. 
+The model will train and evaluate against all of the data.
+
+## Citations
+
+If you use this code, please consider citing the following papers:
+
+```shell
+@inproceedings{lalor2019emnlp,
+  author    = {Lalor, John P and Wu, Hao and Yu, Hong},
+  title     = {Learning Latent Parameters without Human Response Patterns: Item Response Theory with Artificial Crowds},
+  year      = {2019},
+  booktitle = {Proceedings of the 2019 Conference on Empirical Methods in Natural Language Processing},
+}
+```
+
+```shell
+@inproceedings{rodriguez2021evaluation,
+  title={Evaluation Examples Are Not Equally Informative: How Should That Change NLP Leaderboards?},
+  author={Rodriguez, Pedro and Barrow, Joe and Hoyle, Alexander Miserlis and Lalor, John P and Jia, Robin and Boyd-Graber, Jordan},
+  booktitle={Proceedings of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing (Volume 1: Long Papers)},
+  pages={4486--4503},
+  year={2021}
+}
+```
+
+Implementation is based on the following paper:
+
+```shell
+@article{natesan2016bayesian,
+  title={Bayesian prior choice in IRT estimation using MCMC and variational Bayes},
+  author={Natesan, Prathiba and Nandakumar, Ratna and Minka, Tom and Rubright, Jonathan D},
+  journal={Frontiers in psychology},
+  volume={7},
+  pages={1422},
+  year={2016},
+  publisher={Frontiers}
+}
+```
+
+## Contributing
+
+This is research code. Pull requests and issues are welcome!
+
+## Questions?
+
+Let me know if you have any requests, bugs, etc.
+
+Email: john.lalor@nd.edu
```

### Comparing `py_irt-0.6.1/py_irt/cli.py` & `py_irt-0.6.2/py_irt/cli.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,314 +1,314 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-import random
-from typing import Optional, List
-import time
-import json
-import copy
-from pathlib import Path
-
-import torch
-import pyro
-import numpy as np
-import typer
-import toml
-from rich.console import Console
-from sklearn.model_selection import train_test_split
-
-from py_irt.training import IrtModelTrainer
-from py_irt.config import IrtConfig
-from py_irt.dataset import Dataset
-from py_irt.models.abstract_model import IrtModel
-from py_irt.io import write_json, write_jsonlines, read_jsonlines, read_json
-
-console = Console()
-app = typer.Typer()
-
-
-@app.command()
-def train(
-    model_type: str,
-    data_path: str,
-    output_dir: str,
-    epochs: Optional[int] = None,
-    priors: Optional[str] = None,
-    dims: Optional[int] = None,
-    lr: Optional[float] = None,
-    lr_decay: Optional[float] = None,
-    device: str = "cpu",
-    initializers: Optional[List[str]] = None,
-    config_path: Optional[str] = None,
-    dropout: Optional[float] = 0.5,
-    hidden: Optional[int] = 100,
-    seed: Optional[int] = None,
-    deterministic: bool = False,
-    log_every: int = 100,
-):
-    if config_path is None:
-        parsed_config = {}
-    else:
-        if config_path.endswith(".toml"):
-            with open(config_path) as f:
-                parsed_config = toml.load(f)
-        else:
-            parsed_config = read_json(config_path)
-
-    args_config = {
-        "priors": priors,
-        "dims": dims,
-        "lr": lr,
-        "lr_decay": lr_decay,
-        "epochs": epochs,
-        "initializers": initializers,
-        "model_type": model_type,
-        "dropout": dropout,
-        "hidden": hidden,
-        "log_every": log_every,
-        "deterministic": deterministic,
-        "seed": seed,
-    }
-    for key, value in args_config.items():
-        if value is not None:
-            parsed_config[key] = value
-
-    if seed is not None:
-        random.seed(seed)
-        np.random.seed(seed)
-        torch.manual_seed(seed)
-        pyro.set_rng_seed(seed)
-    if deterministic:
-        torch.backends.cudnn.deterministic = True
-        torch.backends.cudnn.benchmark = True
-        torch.use_deterministic_algorithms(True)
-
-    if model_type != parsed_config["model_type"]:
-        raise ValueError("Mismatching model types in args and config")
-
-    config = IrtConfig(**parsed_config)
-    console.log(f"config: {config}")
-
-    console.log(f"data_path: {data_path}")
-    console.log(f"output directory: {output_dir}")
-    start_time = time.time()
-    trainer = IrtModelTrainer(config=config, data_path=data_path)
-    output_dir = Path(output_dir)
-    console.log("Training Model...")
-    trainer.train(device=device)
-    trainer.save(output_dir / "parameters.json")
-    write_json(output_dir / "best_parameters.json", trainer.best_params)
-    end_time = time.time()
-    elapsed_time = end_time - start_time
-    console.log("Train time:", elapsed_time)
-
-
-@app.command()
-def train_and_evaluate(
-    model_type: str,
-    data_path: str,
-    output_dir: str,
-    epochs: int = 2000,
-    priors: Optional[str] = None,
-    dims: Optional[int] = None,
-    device: str = "cpu",
-    lr: Optional[float] = None,
-    lr_decay: Optional[float] = None,
-    initializers: Optional[List[str]] = None,
-    evaluation: str = "heldout",
-    seed: int = 42,
-    train_size: float = 0.9,
-    config_path: Optional[str] = None,
-    dropout: Optional[float] = 0.5,
-    hidden: Optional[int] = 100
-):
-    if config_path is None:
-        parsed_config = {}
-    else:
-        if config_path.endswith(".toml"):
-            with open(config_path) as f:
-                parsed_config = toml.load(f)
-        else:
-            parsed_config = read_json(config_path)
-
-    args_config = {
-        "priors": priors,
-        "dims": dims,
-        "lr": lr,
-        "lr_decay": lr_decay,
-        "epochs": epochs,
-        "initializers": initializers,
-        "model_type": model_type,
-        "dropout": dropout,
-        "hidden": hidden,
-    }
-    for key, value in args_config.items():
-        if value is not None:
-            parsed_config[key] = value
-    if 'amortized' in model_type:
-        amortized = True
-    else:
-        amortized = False
-
-    if model_type != parsed_config["model_type"]:
-        raise ValueError("Mismatching model types in args and config")
-    start_time = time.time()
-    config = IrtConfig(**parsed_config)
-    console.log(f"config: {config}")
-
-    console.log(f"data_path: {data_path}")
-    console.log(f"output directory: {output_dir}")
-
-#    config = IrtConfig(model_type=model_type, epochs=epochs, initializers=initializers)
-    if evaluation == "heldout":
-        with open(data_path) as f:
-            items = []
-            for line in f:
-                submission = json.loads(line)
-                model_id = submission["subject_id"]
-                for example_id in submission["responses"].keys():
-                    items.append((model_id, example_id))
-            train, test = train_test_split(
-                items, train_size=train_size, random_state=seed)
-            training_dict = {}
-            for model_id, example_id in train:
-                training_dict.setdefault(model_id, dict())
-                training_dict[model_id][example_id] = True
-            for model_id, example_id in test:
-                training_dict.setdefault(model_id, dict())
-                training_dict[model_id][example_id] = False
-        dataset = Dataset.from_jsonlines(
-            data_path, train_items=training_dict, amortized=amortized)
-    else:
-        dataset = Dataset.from_jsonlines(data_path, amortized=amortized)
-
-    # deep copy for training
-    training_data = copy.deepcopy(dataset)
-    trainer = IrtModelTrainer(
-        config=config, dataset=training_data, data_path=data_path)
-    output_dir = Path(output_dir)
-    console.log("Training Model...")
-    trainer.train(device=device)
-    trainer.save(output_dir / "parameters.json")
-    write_json(output_dir / "best_parameters.json", trainer.best_params)
-
-    # get validation data
-    # filter out test data
-    console.log("Evaluating Model...")
-    testing_idx = [
-        i for i in range(len(dataset.training_example)) if not dataset.training_example[i]
-    ]
-    if len(testing_idx) > 0:
-        dataset.observation_subjects = [
-            dataset.observation_subjects[i] for i in testing_idx]
-        dataset.observation_items = [
-            dataset.observation_items[i] for i in testing_idx]
-        dataset.observations = [dataset.observations[i] for i in testing_idx]
-        dataset.training_example = [
-            dataset.training_example[i] for i in testing_idx]
-
-    preds = trainer.irt_model.predict(
-        dataset.observation_subjects, dataset.observation_items)
-    outputs = []
-    for i in range(len(preds)):
-        outputs.append(
-            {
-                "subject_id": dataset.observation_subjects[i],
-                "example_id": dataset.observation_items[i],
-                "response": dataset.observations[i],
-                "prediction": preds[i],
-            }
-        )
-    write_jsonlines(f"{output_dir}/model_predictions.jsonlines", outputs)
-    end_time = time.time()
-    elapsed_time = end_time - start_time
-    console.log("Evaluation time:", elapsed_time)
-
-
-@app.command()
-def evaluate(
-    model_type: str,
-    parameter_path: str,
-    test_pairs_path: str,
-    output_dir: str,
-    epochs: int = 2000,
-    device: str = "cpu",
-    initializers: Optional[List[str]] = None,
-    evaluation: str = "heldout",
-    seed: int = 42,
-    train_size: float = 0.9,
-):
-    console.log(
-        f"model_type: {model_type}, parameter_path: {parameter_path}, test_pairs_path: {test_pairs_path}"
-    )
-    console.log(f"output directory: {output_dir}")
-    start_time = time.time()
-    console.log("Evaluating Model...")
-    # load saved params
-    irt_params = read_json(parameter_path)
-
-    # reverse dict for lookup
-    subjectIDX = {}
-    for (key, item) in irt_params["subject_ids"].items():
-        subjectIDX[item] = int(key)
-
-    itemIDX = {}
-    for (key, item) in irt_params["item_ids"].items():
-        itemIDX[item] = int(key)
-
-    # load subject, item pairs we want to test
-    subject_item_pairs = read_jsonlines(test_pairs_path)
-
-    # calculate predictions and write them to disk
-    config = IrtConfig(model_type=model_type, epochs=epochs,
-                       initializers=initializers)
-    
-    observation_subjects = [subjectIDX[entry["subject_id"]]
-                            for entry in subject_item_pairs]
-    observation_items = [itemIDX[entry["item_id"]] for entry in subject_item_pairs]
-
-    irt_model = IrtModel.from_name(model_type)(
-        priors="vague",
-        device=device,
-        num_items=len(set(observation_items)),
-        num_subjects=len(set(observation_subjects)),
-    )
-
-    preds = irt_model.predict(observation_subjects,
-                              observation_items, irt_params)
-    outputs = []
-    for i in range(len(preds)):
-        outputs.append(
-            {
-                "subject_id": observation_subjects[i],
-                "example_id": observation_items[i],
-                "prediction": preds[i],
-            }
-        )
-    write_jsonlines(f"{output_dir}/model_predictions.jsonlines", outputs)
-    end_time = time.time()
-    elapsed_time = end_time - start_time
-    console.log("Evaluation time:", elapsed_time)
-
-
-if __name__ == "__main__":
-    app()
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+import random
+from typing import Optional, List
+import time
+import json
+import copy
+from pathlib import Path
+
+import torch
+import pyro
+import numpy as np
+import typer
+import toml
+from rich.console import Console
+from sklearn.model_selection import train_test_split
+
+from py_irt.training import IrtModelTrainer
+from py_irt.config import IrtConfig
+from py_irt.dataset import Dataset
+from py_irt.models.abstract_model import IrtModel
+from py_irt.io import write_json, write_jsonlines, read_jsonlines, read_json
+
+console = Console()
+app = typer.Typer()
+
+
+@app.command()
+def train(
+    model_type: str,
+    data_path: str,
+    output_dir: str,
+    epochs: Optional[int] = None,
+    priors: Optional[str] = None,
+    dims: Optional[int] = None,
+    lr: Optional[float] = None,
+    lr_decay: Optional[float] = None,
+    device: str = "cpu",
+    initializers: Optional[List[str]] = None,
+    config_path: Optional[str] = None,
+    dropout: Optional[float] = 0.5,
+    hidden: Optional[int] = 100,
+    seed: Optional[int] = None,
+    deterministic: bool = False,
+    log_every: int = 100,
+):
+    if config_path is None:
+        parsed_config = {}
+    else:
+        if config_path.endswith(".toml"):
+            with open(config_path) as f:
+                parsed_config = toml.load(f)
+        else:
+            parsed_config = read_json(config_path)
+
+    args_config = {
+        "priors": priors,
+        "dims": dims,
+        "lr": lr,
+        "lr_decay": lr_decay,
+        "epochs": epochs,
+        "initializers": initializers,
+        "model_type": model_type,
+        "dropout": dropout,
+        "hidden": hidden,
+        "log_every": log_every,
+        "deterministic": deterministic,
+        "seed": seed,
+    }
+    for key, value in args_config.items():
+        if value is not None:
+            parsed_config[key] = value
+
+    if seed is not None:
+        random.seed(seed)
+        np.random.seed(seed)
+        torch.manual_seed(seed)
+        pyro.set_rng_seed(seed)
+    if deterministic:
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = True
+        torch.use_deterministic_algorithms(True)
+
+    if model_type != parsed_config["model_type"]:
+        raise ValueError("Mismatching model types in args and config")
+
+    config = IrtConfig(**parsed_config)
+    console.log(f"config: {config}")
+
+    console.log(f"data_path: {data_path}")
+    console.log(f"output directory: {output_dir}")
+    start_time = time.time()
+    trainer = IrtModelTrainer(config=config, data_path=data_path)
+    output_dir = Path(output_dir)
+    console.log("Training Model...")
+    trainer.train(device=device)
+    trainer.save(output_dir / "parameters.json")
+    write_json(output_dir / "best_parameters.json", trainer.best_params)
+    end_time = time.time()
+    elapsed_time = end_time - start_time
+    console.log("Train time:", elapsed_time)
+
+
+@app.command()
+def train_and_evaluate(
+    model_type: str,
+    data_path: str,
+    output_dir: str,
+    epochs: int = 2000,
+    priors: Optional[str] = None,
+    dims: Optional[int] = None,
+    device: str = "cpu",
+    lr: Optional[float] = None,
+    lr_decay: Optional[float] = None,
+    initializers: Optional[List[str]] = None,
+    evaluation: str = "heldout",
+    seed: int = 42,
+    train_size: float = 0.9,
+    config_path: Optional[str] = None,
+    dropout: Optional[float] = 0.5,
+    hidden: Optional[int] = 100
+):
+    if config_path is None:
+        parsed_config = {}
+    else:
+        if config_path.endswith(".toml"):
+            with open(config_path) as f:
+                parsed_config = toml.load(f)
+        else:
+            parsed_config = read_json(config_path)
+
+    args_config = {
+        "priors": priors,
+        "dims": dims,
+        "lr": lr,
+        "lr_decay": lr_decay,
+        "epochs": epochs,
+        "initializers": initializers,
+        "model_type": model_type,
+        "dropout": dropout,
+        "hidden": hidden,
+    }
+    for key, value in args_config.items():
+        if value is not None:
+            parsed_config[key] = value
+    if 'amortized' in model_type:
+        amortized = True
+    else:
+        amortized = False
+
+    if model_type != parsed_config["model_type"]:
+        raise ValueError("Mismatching model types in args and config")
+    start_time = time.time()
+    config = IrtConfig(**parsed_config)
+    console.log(f"config: {config}")
+
+    console.log(f"data_path: {data_path}")
+    console.log(f"output directory: {output_dir}")
+
+#    config = IrtConfig(model_type=model_type, epochs=epochs, initializers=initializers)
+    if evaluation == "heldout":
+        with open(data_path) as f:
+            items = []
+            for line in f:
+                submission = json.loads(line)
+                model_id = submission["subject_id"]
+                for example_id in submission["responses"].keys():
+                    items.append((model_id, example_id))
+            train, test = train_test_split(
+                items, train_size=train_size, random_state=seed)
+            training_dict = {}
+            for model_id, example_id in train:
+                training_dict.setdefault(model_id, dict())
+                training_dict[model_id][example_id] = True
+            for model_id, example_id in test:
+                training_dict.setdefault(model_id, dict())
+                training_dict[model_id][example_id] = False
+        dataset = Dataset.from_jsonlines(
+            data_path, train_items=training_dict, amortized=amortized)
+    else:
+        dataset = Dataset.from_jsonlines(data_path, amortized=amortized)
+
+    # deep copy for training
+    training_data = copy.deepcopy(dataset)
+    trainer = IrtModelTrainer(
+        config=config, dataset=training_data, data_path=data_path)
+    output_dir = Path(output_dir)
+    console.log("Training Model...")
+    trainer.train(device=device)
+    trainer.save(output_dir / "parameters.json")
+    write_json(output_dir / "best_parameters.json", trainer.best_params)
+
+    # get validation data
+    # filter out test data
+    console.log("Evaluating Model...")
+    testing_idx = [
+        i for i in range(len(dataset.training_example)) if not dataset.training_example[i]
+    ]
+    if len(testing_idx) > 0:
+        dataset.observation_subjects = [
+            dataset.observation_subjects[i] for i in testing_idx]
+        dataset.observation_items = [
+            dataset.observation_items[i] for i in testing_idx]
+        dataset.observations = [dataset.observations[i] for i in testing_idx]
+        dataset.training_example = [
+            dataset.training_example[i] for i in testing_idx]
+
+    preds = trainer.irt_model.predict(
+        dataset.observation_subjects, dataset.observation_items)
+    outputs = []
+    for i in range(len(preds)):
+        outputs.append(
+            {
+                "subject_id": dataset.observation_subjects[i],
+                "example_id": dataset.observation_items[i],
+                "response": dataset.observations[i],
+                "prediction": preds[i],
+            }
+        )
+    write_jsonlines(f"{output_dir}/model_predictions.jsonlines", outputs)
+    end_time = time.time()
+    elapsed_time = end_time - start_time
+    console.log("Evaluation time:", elapsed_time)
+
+
+@app.command()
+def evaluate(
+    model_type: str,
+    parameter_path: str,
+    test_pairs_path: str,
+    output_dir: str,
+    epochs: int = 2000,
+    device: str = "cpu",
+    initializers: Optional[List[str]] = None,
+    evaluation: str = "heldout",
+    seed: int = 42,
+    train_size: float = 0.9,
+):
+    console.log(
+        f"model_type: {model_type}, parameter_path: {parameter_path}, test_pairs_path: {test_pairs_path}"
+    )
+    console.log(f"output directory: {output_dir}")
+    start_time = time.time()
+    console.log("Evaluating Model...")
+    # load saved params
+    irt_params = read_json(parameter_path)
+
+    # reverse dict for lookup
+    subjectIDX = {}
+    for (key, item) in irt_params["subject_ids"].items():
+        subjectIDX[item] = int(key)
+
+    itemIDX = {}
+    for (key, item) in irt_params["item_ids"].items():
+        itemIDX[item] = int(key)
+
+    # load subject, item pairs we want to test
+    subject_item_pairs = read_jsonlines(test_pairs_path)
+
+    # calculate predictions and write them to disk
+    config = IrtConfig(model_type=model_type, epochs=epochs,
+                       initializers=initializers)
+    
+    observation_subjects = [subjectIDX[entry["subject_id"]]
+                            for entry in subject_item_pairs]
+    observation_items = [itemIDX[entry["item_id"]] for entry in subject_item_pairs]
+
+    irt_model = IrtModel.from_name(model_type)(
+        priors="vague",
+        device=device,
+        num_items=len(set(observation_items)),
+        num_subjects=len(set(observation_subjects)),
+    )
+
+    preds = irt_model.predict(observation_subjects,
+                              observation_items, irt_params)
+    outputs = []
+    for i in range(len(preds)):
+        outputs.append(
+            {
+                "subject_id": observation_subjects[i],
+                "example_id": observation_items[i],
+                "prediction": preds[i],
+            }
+        )
+    write_jsonlines(f"{output_dir}/model_predictions.jsonlines", outputs)
+    end_time = time.time()
+    elapsed_time = end_time - start_time
+    console.log("Evaluation time:", elapsed_time)
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `py_irt-0.6.1/py_irt/config.py` & `py_irt-0.6.2/py_irt/config.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-from typing import List, Dict, Union, Optional, Callable
-from pydantic import BaseModel, ConfigDict
-
-# This registers all models with the registry
-# pylint: disable=unused-import
-from py_irt.models import *
-
-
-class IrtConfig(BaseModel):
-    model_type: Union[str, Callable]
-    epochs: int = 2000
-    priors: Optional[str] = None
-    initializers: Optional[List[Union[str, Dict]]] = None
-    dims: Optional[int] = None
-    lr: float = 0.1
-    lr_decay: float = 0.9999
-    dropout: float = 0.5
-    hidden: int = 100
-    vocab_size: Optional[int] = None
-    log_every: int = 100
-    seed: Optional[int] = None
-    deterministic: bool = False
-    model_config = ConfigDict(protected_namespaces=())
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+from typing import List, Dict, Union, Optional, Callable
+from pydantic import BaseModel, ConfigDict
+
+# This registers all models with the registry
+# pylint: disable=unused-import
+from py_irt.models import *
+
+
+class IrtConfig(BaseModel):
+    model_type: Union[str, Callable]
+    epochs: int = 2000
+    priors: Optional[str] = None
+    initializers: Optional[List[Union[str, Dict]]] = None
+    dims: Optional[int] = None
+    lr: float = 0.1
+    lr_decay: float = 0.9999
+    dropout: float = 0.5
+    hidden: int = 100
+    vocab_size: Optional[int] = None
+    log_every: int = 100
+    seed: Optional[int] = None
+    deterministic: bool = False
+    model_config = ConfigDict(protected_namespaces=())
```

### Comparing `py_irt-0.6.1/py_irt/initializers.py` & `py_irt-0.6.2/py_irt/initializers.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-"""
-A set of initializers to modify how IRT models are initialized.
-
-For example, the expression disc * (skill - diff) permits two equivalent
-solutions, one where disc/skill/diff are "normal", and another one where the
-sign on each is flipped. Initializing difficulty helps push towards the intuitive
-solution.
-"""
-import abc
-import torch
-import pyro
-from rich.console import Console
-from py_irt.dataset import Dataset, ItemAccuracy
-
-
-console = Console()
-INITIALIZERS = {}
-
-
-def register(name: str):
-    def decorator(class_):
-        INITIALIZERS[name] = class_
-        return class_
-
-    return decorator
-
-
-class IrtInitializer(abc.ABC):
-    def __init__(self, dataset: Dataset):
-        self._dataset = dataset
-
-    def initialize(self) -> None:
-        pass
-
-
-@register("difficulty_sign")
-class DifficultySignInitializer(IrtInitializer):
-    def __init__(self, dataset: Dataset, magnitude: float = 3.0, n_to_init: int = 4):
-        super().__init__(dataset)
-        self._magnitude = magnitude
-        self._n_to_init = n_to_init
-
-    def initialize(self) -> None:
-        """
-        Initialize the hardest and easiest (by accuracy) n_to_init item difficulties.
-        Set to magnitude.
-        """
-        item_accuracies = {}
-        for item_ix, response in zip(self._dataset.observation_items, self._dataset.observations):
-            if item_ix not in item_accuracies:
-                item_accuracies[item_ix] = ItemAccuracy()
-
-            item_accuracies[item_ix].correct += response
-            item_accuracies[item_ix].total += 1
-
-        sorted_item_accuracies = sorted(
-            list(item_accuracies.items()), key=lambda kv: kv[1].accuracy
-        )
-
-        diff = pyro.param("loc_diff")
-        for item_ix, accuracy in sorted_item_accuracies[: self._n_to_init]:
-            item_id = self._dataset.ix_to_item_id[item_ix]
-            console.log(f"Low Accuracy: {accuracy}, ix={item_ix} id={item_id}")
-            diff.data[item_ix] = torch.tensor(
-                self._magnitude, dtype=diff.data.dtype, device=diff.data.device
-            )
-
-        for item_ix, accuracy in sorted_item_accuracies[-self._n_to_init :]:
-            item_id = self._dataset.ix_to_item_id[item_ix]
-            console.log(f"High Accuracy: {accuracy}, ix={item_ix} id={item_id}")
-            diff.data[item_ix] = torch.tensor(
-                -self._magnitude, dtype=diff.data.dtype, device=diff.data.device
-            )
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+"""
+A set of initializers to modify how IRT models are initialized.
+
+For example, the expression disc * (skill - diff) permits two equivalent
+solutions, one where disc/skill/diff are "normal", and another one where the
+sign on each is flipped. Initializing difficulty helps push towards the intuitive
+solution.
+"""
+import abc
+import torch
+import pyro
+from rich.console import Console
+from py_irt.dataset import Dataset, ItemAccuracy
+
+
+console = Console()
+INITIALIZERS = {}
+
+
+def register(name: str):
+    def decorator(class_):
+        INITIALIZERS[name] = class_
+        return class_
+
+    return decorator
+
+
+class IrtInitializer(abc.ABC):
+    def __init__(self, dataset: Dataset):
+        self._dataset = dataset
+
+    def initialize(self) -> None:
+        pass
+
+
+@register("difficulty_sign")
+class DifficultySignInitializer(IrtInitializer):
+    def __init__(self, dataset: Dataset, magnitude: float = 3.0, n_to_init: int = 4):
+        super().__init__(dataset)
+        self._magnitude = magnitude
+        self._n_to_init = n_to_init
+
+    def initialize(self) -> None:
+        """
+        Initialize the hardest and easiest (by accuracy) n_to_init item difficulties.
+        Set to magnitude.
+        """
+        item_accuracies = {}
+        for item_ix, response in zip(self._dataset.observation_items, self._dataset.observations):
+            if item_ix not in item_accuracies:
+                item_accuracies[item_ix] = ItemAccuracy()
+
+            item_accuracies[item_ix].correct += response
+            item_accuracies[item_ix].total += 1
+
+        sorted_item_accuracies = sorted(
+            list(item_accuracies.items()), key=lambda kv: kv[1].accuracy
+        )
+
+        diff = pyro.param("loc_diff")
+        for item_ix, accuracy in sorted_item_accuracies[: self._n_to_init]:
+            item_id = self._dataset.ix_to_item_id[item_ix]
+            console.log(f"Low Accuracy: {accuracy}, ix={item_ix} id={item_id}")
+            diff.data[item_ix] = torch.tensor(
+                self._magnitude, dtype=diff.data.dtype, device=diff.data.device
+            )
+
+        for item_ix, accuracy in sorted_item_accuracies[-self._n_to_init :]:
+            item_id = self._dataset.ix_to_item_id[item_ix]
+            console.log(f"High Accuracy: {accuracy}, ix={item_ix} id={item_id}")
+            diff.data[item_ix] = torch.tensor(
+                -self._magnitude, dtype=diff.data.dtype, device=diff.data.device
+            )
```

### Comparing `py_irt-0.6.1/py_irt/io.py` & `py_irt-0.6.2/py_irt/io.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-from typing import Any, Union, List
-from pathlib import Path
-import os
-import json
-from pydantic import BaseModel
-
-
-def read_json(path: Union[str, Path]):
-    """
-    Read a json file from a string path
-    """
-    with open(path) as f:
-        return json.load(f)
-
-
-def write_json(path: Union[str, Path], obj: Any):
-    """
-    Write an object to a string path as json.
-    If the object is a pydantic model, export it to json
-    """
-    if isinstance(obj, BaseModel):
-        with open(path, "w") as f:
-            f.write(obj.json())
-    else:
-        with open(path, "w") as f:
-            json.dump(obj, f)
-
-
-def _read_jsonlines_list(path: Union[str, Path]):
-    """
-    Read a jsonlines file into memory all at once
-    """
-    out = []
-    with open(path) as f:
-        for line in f:
-            out.append(json.loads(line))
-    return out
-
-
-def _read_jsonlines_lazy(path: Union[str, Path]):
-    """
-    Lazily return the contents of a jsonlines file
-    """
-    with open(path) as f:
-        for line in f:
-            yield json.loads(line)
-
-
-def read_jsonlines(path: Union[str, Path], lazy: bool = False):
-    """
-    Read a jsonlines file as a list/iterator of json objects
-    """
-    if lazy:
-        return _read_jsonlines_lazy(path)
-    else:
-        return _read_jsonlines_list(path)
-
-
-def write_jsonlines(path: Union[str, Path], elements: List[Any]):
-    """
-    Write a list of json serialiazable objects to the path given
-    """
-    with open(path, "w") as f:
-        for e in elements:
-            f.write(json.dumps(e))
-            f.write("\n")
-
-
-def safe_file(path: Union[str, Path]) -> Union[str, Path]:
-    """
-    Ensure that the path to the file exists, then return the path.
-    For example, if the path passed in is /home/entilzha/stuff/stuff/test.txt,
-    this function will run the equivalent of mkdir -p /home/entilzha/stuff/stuff/
-    """
-    os.makedirs(os.path.dirname(path), exist_ok=True)
-    return path
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+from typing import Any, Union, List
+from pathlib import Path
+import os
+import json
+from pydantic import BaseModel
+
+
+def read_json(path: Union[str, Path]):
+    """
+    Read a json file from a string path
+    """
+    with open(path) as f:
+        return json.load(f)
+
+
+def write_json(path: Union[str, Path], obj: Any):
+    """
+    Write an object to a string path as json.
+    If the object is a pydantic model, export it to json
+    """
+    if isinstance(obj, BaseModel):
+        with open(path, "w") as f:
+            f.write(obj.json())
+    else:
+        with open(path, "w") as f:
+            json.dump(obj, f)
+
+
+def _read_jsonlines_list(path: Union[str, Path]):
+    """
+    Read a jsonlines file into memory all at once
+    """
+    out = []
+    with open(path) as f:
+        for line in f:
+            out.append(json.loads(line))
+    return out
+
+
+def _read_jsonlines_lazy(path: Union[str, Path]):
+    """
+    Lazily return the contents of a jsonlines file
+    """
+    with open(path) as f:
+        for line in f:
+            yield json.loads(line)
+
+
+def read_jsonlines(path: Union[str, Path], lazy: bool = False):
+    """
+    Read a jsonlines file as a list/iterator of json objects
+    """
+    if lazy:
+        return _read_jsonlines_lazy(path)
+    else:
+        return _read_jsonlines_list(path)
+
+
+def write_jsonlines(path: Union[str, Path], elements: List[Any]):
+    """
+    Write a list of json serialiazable objects to the path given
+    """
+    with open(path, "w") as f:
+        for e in elements:
+            f.write(json.dumps(e))
+            f.write("\n")
+
+
+def safe_file(path: Union[str, Path]) -> Union[str, Path]:
+    """
+    Ensure that the path to the file exists, then return the path.
+    For example, if the path passed in is /home/entilzha/stuff/stuff/test.txt,
+    this function will run the equivalent of mkdir -p /home/entilzha/stuff/stuff/
+    """
+    os.makedirs(os.path.dirname(path), exist_ok=True)
+    return path
```

### Comparing `py_irt-0.6.1/py_irt/models/abstract_model.py` & `py_irt-0.6.2/py_irt/models/abstract_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,96 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-import abc
-from typing import Dict, Any
-
-
-_IRT_REGISTRY = {}
-
-
-class IrtModel(abc.ABC):
-    def __init__(
-        self, *, num_items: int, num_subjects: int, verbose: bool = False, device: str = "cpu"
-    ) -> None:
-        super().__init__()
-        if device not in ["cpu", "cuda"]:
-            raise ValueError("Options for device are cpu and cuda")
-        if num_items <= 0:
-            raise ValueError("Number of items must be greater than 0")
-        if num_subjects <= 0:
-            raise ValueError("Number of subjects must be greater than 0")
-        self.device = device
-        self.num_items = num_items
-        self.num_subjects = num_subjects
-        self.verbose = verbose
-
-    @classmethod
-    def register(cls, name: str):
-        def add_to_registry(class_):
-            if class_ in _IRT_REGISTRY:
-                raise ValueError(f"Model name already in registry: {class_}")
-            _IRT_REGISTRY[name] = class_
-            return class_
-
-        return add_to_registry
-
-    @classmethod
-    def from_name(cls, name: str):
-        if name not in _IRT_REGISTRY:
-            raise ValueError(f"Unknown model name: {name}, Registry:\n{_IRT_REGISTRY}")
-        return _IRT_REGISTRY[name]
-
-    @classmethod
-    def validate_name(cls, name: str):
-        if name not in _IRT_REGISTRY:
-            raise ValueError(f"Unknown model name: {name}, Registry:\n{_IRT_REGISTRY}")
-        return
-
-    @abc.abstractmethod
-    def get_model(self):
-        pass
-
-    @abc.abstractmethod
-    def get_guide(self):
-        pass
-
-    @abc.abstractmethod
-    def export(self) -> Dict[str, Any]:
-        pass
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+import abc
+from typing import Dict, Any
+
+_IRT_REGISTRY = {}
+
+
+class IrtModel(abc.ABC):
+    def __init__(
+        self, *, num_items: int, num_subjects: int, verbose: bool = False, device: str = "cpu"
+    ) -> None:
+        super().__init__()
+        if device not in ["cpu", "cuda"]:
+            raise ValueError("Options for device are cpu and cuda")
+        if num_items <= 0:
+            raise ValueError("Number of items must be greater than 0")
+        if num_subjects <= 0:
+            raise ValueError("Number of subjects must be greater than 0")
+        self.device = device
+        self.num_items = num_items
+        self.num_subjects = num_subjects
+        self.verbose = verbose
+
+    @classmethod
+    def register(cls, name: str):
+        def add_to_registry(class_):
+            if class_ in _IRT_REGISTRY:
+                raise ValueError(f"Model name already in registry: {class_}")
+            _IRT_REGISTRY[name] = class_
+            return class_
+
+        return add_to_registry
+
+    @classmethod
+    def from_name(cls, name: str):
+        if name not in _IRT_REGISTRY:
+            raise ValueError(f"Unknown model name: {name}, Registry:\n{_IRT_REGISTRY}")
+        return _IRT_REGISTRY[name]
+
+    @classmethod
+    def validate_name(cls, name: str):
+        if name not in _IRT_REGISTRY:
+            raise ValueError(f"Unknown model name: {name}, Registry:\n{_IRT_REGISTRY}")
+        return
+
+    @abc.abstractmethod
+    def get_model(self):
+        pass
+
+    @abc.abstractmethod
+    def get_guide(self):
+        pass
+
+    @abc.abstractmethod
+    def export(self) -> Dict[str, Any]:
+        pass
+
+    @classmethod
+    def train(cls, dataset, **kw):
+        # import here to avoid circular import
+        from py_irt.config import IrtConfig
+        from py_irt.training import IrtModelTrainer
+
+        inv_irt_registry = {v: k for k, v in _IRT_REGISTRY.items()}
+        try:
+            my_name = inv_irt_registry[cls]
+        except KeyError:
+            raise KeyError("model not found in registry")
+
+        config = IrtConfig(model_type=my_name, **kw)
+        trainer = IrtModelTrainer(dataset=dataset, data_path=None, config=config)
+        trainer.train()
+        
+        return trainer
```

### Comparing `py_irt-0.6.1/py_irt/models/amortized_1pl.py` & `py_irt-0.6.2/py_irt/models/amortized_1pl.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,264 +1,264 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-from py_irt.models import abstract_model
-import pyro
-import pyro.distributions as dist
-import torch
-
-import torch.distributions.constraints as constraints
-
-from pyro.infer import SVI, Trace_ELBO, EmpiricalMarginal, TraceEnum_ELBO
-from pyro.infer.mcmc import MCMC, NUTS
-from pyro.optim import Adam, SGD
-
-import pyro.contrib.autoguide as autoguide
-
-import pandas as pd
-
-from functools import partial
-
-import numpy as np
-
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-
-# building off of ProdLDA model for amortization (text only for now) 
-# https://pyro.ai/examples/prodlda.html
-class Encoder(nn.Module):
-    # Base class for the encoder net, used in the guide
-    def __init__(self, vocab_size, num_dimensions, hidden, dropout):
-        super().__init__()
-        self.drop = nn.Dropout(dropout)  # to avoid component collapse
-        self.fc1 = nn.Linear(vocab_size, hidden)
-        self.fc2 = nn.Linear(hidden, hidden)
-        self.fcmu = nn.Linear(hidden, num_dimensions)
-        self.fclv = nn.Linear(hidden, num_dimensions)
-        # NB: here we set `affine=False` to reduce the number of learning parameters
-        # See https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
-        # for the effect of this flag in BatchNorm1d
-        self.bnmu = nn.BatchNorm1d(num_dimensions, affine=False)  # to avoid component collapse
-        self.bnlv = nn.BatchNorm1d(num_dimensions, affine=False)  # to avoid component collapse
-
-    def forward(self, inputs):
-        h = F.softplus(self.fc1(inputs))
-        h = F.softplus(self.fc2(h))
-        h = self.drop(h)
-        # μ and Σ are the outputs
-        logtheta_loc = self.bnmu(self.fcmu(h))
-        logtheta_logvar = self.bnlv(self.fclv(h))
-        logtheta_scale = (0.5 * logtheta_logvar).exp()  # Enforces positivity
-        return logtheta_loc, logtheta_scale
-
-
-class Decoder(nn.Module):
-    # Base class for the decoder net, used in the model
-    def __init__(self, vocab_size, num_dimensions, dropout):
-        super().__init__()
-        self.beta = nn.Linear(num_dimensions, vocab_size, bias=False)
-        self.bn = nn.BatchNorm1d(vocab_size, affine=False)
-        self.drop = nn.Dropout(dropout)
-
-    def forward(self, inputs):
-        inputs = self.drop(inputs)
-        # the output is σ(βθ)
-        return F.softmax(self.bn(self.beta(inputs)), dim=1)
-
-
-@abstract_model.IrtModel.register("amortized_1pl")
-class Amortized1PL(abstract_model.IrtModel):
-    
-    def __init__(
-        self, *, 
-        priors: str, 
-        num_items: int, 
-        num_subjects: int, 
-        verbose: bool = False, 
-        device: str = "cpu",
-        vocab_size: int,
-        dropout: float,
-        hidden: int,
-        **kwargs
-    ):
-        super().__init__(
-            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
-        )
-
-        # initialize the class with all arguments provided to the constructor
-        self.num_dimensions = 1
-        self.device = torch.device(device)
-        self.drop = dropout
-        self.hidden = hidden
-        self.num_items = num_items
-
-        self.vocab_size = vocab_size
-        self.encoder = Encoder(vocab_size, self.num_dimensions, self.hidden, self.drop)
-        self.decoder = Decoder(vocab_size, self.num_dimensions, self.drop)
-    
-
-    def model_irt(self, models, items, obs):
-        num_items = len(items)
-        options = dict(dtype=torch.float64, device=self.device)
-        #xs = torch.flatten(items, start_dim=1)
-        xs = items
-        models = torch.tensor(models, dtype=torch.long, device=items.device)
-        items = torch.tensor(items, dtype=torch.long, device=items.device)
-        obs = torch.tensor(obs, dtype=torch.float, device=items.device)
-
-        with pyro.plate("thetas"):
-            ability = pyro.sample('theta', dist.Normal(torch.zeros(self.num_subjects, **options),
-                torch.ones(self.num_subjects, **options)))
-        with pyro.plate("diffs", num_items):
-            # sample the item difficulty from the prior distribution
-            diff_prior_loc = torch.zeros(num_items, **options).unsqueeze(1).float()
-            diff_prior_scale = torch.ones(num_items, **options).fill_(1.e3).unsqueeze(1).float()
-            diff = pyro.sample('b', dist.Normal(diff_prior_loc, diff_prior_scale).to_event(1))
-            loc = self.decoder.forward(diff)
-            total_count = int(xs.sum(-1).max())
-            pyro.sample(
-                'items',
-                dist.Multinomial(total_count, loc),
-                obs=items
-            )
-            #diff = pyro.sample('b', dist.Normal(torch.zeros(num_items, **options),
-            #    torch.tensor(num_items, **options).fill_(1.e-3)))
-
-        with pyro.plate("data", len(obs)):
-            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff).to_event(1), obs=obs)
-        
-    def guide_irt(self, models, items, obs):
-        num_items = len(items)
-        options = dict(dtype=torch.float64, device=self.device)
-        #xs = torch.flatten(items, start_dim=1)
-        xs = items
-        # vectorize
-        models = torch.tensor(models, dtype=torch.long, device=self.device)
-        items = torch.tensor(items, dtype=torch.float, device=self.device)
-        obs = torch.tensor(obs, dtype=torch.float, device=self.device)
-
-
-        # register learnable params in the param store
-        with pyro.plate("thetas"):
-            m_theta_param = pyro.param("loc_ability", torch.zeros(self.num_subjects, **options))
-            s_theta_param = pyro.param("scale_ability", torch.ones(self.num_subjects, **options),
-                            constraint=constraints.positive)
-            dist_theta = dist.Normal(m_theta_param, s_theta_param)
-            pyro.sample("theta", dist_theta)
-
-        # items 
-        with pyro.plate("diffs", num_items):
-            irt_batch_size = 256
-            loc_diffs_all, scale_diffs_all = [], []
-            for i in range(0, len(items), irt_batch_size):
-                if len(items[i:]) < irt_batch_size:
-                    batch_xs = items[i:]
-                    loc_diffs, scale_diffs = self.encoder.forward(batch_xs)
-                    loc_diffs_all.extend(loc_diffs)
-                    scale_diffs_all.extend(scale_diffs) 
-                else:
-                    # pick out the appropriate images from xs based on items idx
-                    batch_xs = items[i:i+irt_batch_size]
-                    loc_diffs, scale_diffs = self.encoder.forward(batch_xs)            
-                    loc_diffs_all.extend(loc_diffs)
-                    scale_diffs_all.extend(scale_diffs)
-            loc_diffs_all = torch.tensor(loc_diffs_all, **options).unsqueeze(1).float()
-            scale_diffs_all = torch.tensor(scale_diffs_all, **options).unsqueeze(1).float()
-            dist_b = dist.Normal(loc_diffs_all, scale_diffs_all)
-            pyro.sample('b', dist_b.to_event(1))
-
-    def get_model(self):
-        return self.model_irt
-
-    def get_guide(self):
-        return self.guide_irt
-
-    def fit(self, models, items, responses, num_epochs):
-        """Fit the IRT model with variational inference"""
-        # need to step with IRT loss and with reconstruction loss
-
-        optim = Adam({"lr": 0.1})
-        svi = SVI(self.model_irt, self.guide_irt, optim, loss=Trace_ELBO())
-        #svi_diff = SVI(self.model, self.guide, optim, loss=Trace_ELBO())
-
-        pyro.clear_param_store()
-        for j in range(num_epochs):
-            loss = svi.step(models, items, responses)
-            #loss_diff = svi_diff.step(items)
-            if j % 100 == 0 and self.verbose:
-                print("[epoch %04d] irt loss: %.4f" % (j + 1, loss))
-                #print("[epoch %04d] recon loss: %.4f" % (j + 1, loss_diff))
-
-        print("[epoch %04d] loss: %.4f" % (j + 1, loss))
-        #print("[epoch %04d] loss: %.4f" % (j + 1, loss_diff))
-        values = ["loc_diff", "scale_diff", "loc_ability", "scale_ability"]
-
-    def export(self, items):
-        items = torch.tensor(items, dtype=torch.float)
-        diffs, _ = self.encoder.forward(items)
-        diffs = diffs.squeeze().detach().numpy()
-
-        return {
-            "ability": pyro.param("loc_ability").data.tolist(),
-            "diff": diffs.tolist()
-        }
-
-    def fit_MCMC(self, models, items, responses, num_epochs):
-        """Fit the IRT model with MCMC"""
-        sites = ["theta", "b"]
-        nuts_kernel = NUTS(self.model_vague, adapt_step_size=True)
-        hmc_posterior = MCMC(nuts_kernel, num_samples=1000, warmup_steps=100).run(
-            models, items, responses
-        )
-        theta_sum = self.summary(hmc_posterior, ["theta"]).items()
-        b_sum = self.summary(hmc_posterior, ["b"]).items()
-        
-    def predict(self, subjects, items, params_from_file=None):
-        """predict p(correct | params) for a specified list of model, item pairs"""
-        if params_from_file is not None:
-            model_params = params_from_file
-        else:
-            model_params = self.export(items)
-        abilities = np.array([model_params["ability"][i] for i in subjects])
-        diffs = np.array(model_params["diff"])
-        #items = torch.tensor(items, dtype=torch.float)
-        #diffs, _ = self.encoder.forward(items)
-        #diffs = diffs.squeeze().detach().numpy()
-        return 1 / (1 + np.exp(-(abilities - diffs)))
-
-    def summary(self, traces, sites):
-        """Aggregate marginals for MCM"""
-        marginal = (
-            EmpiricalMarginal(traces, sites)._get_samples_and_weights()[0].detach().cpu().numpy()
-        )
-        print(marginal)
-        site_stats = {}
-        for i in range(marginal.shape[1]):
-            site_name = sites[i]
-            marginal_site = pd.DataFrame(marginal[:, i]).transpose()
-            describe = partial(pd.Series.describe, percentiles=[0.05, 0.25, 0.5, 0.75, 0.95])
-            site_stats[site_name] = marginal_site.apply(describe, axis=1)[
-                ["mean", "std", "5%", "25%", "50%", "75%", "95%"]
-            ]
-        return site_stats
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+from py_irt.models import abstract_model
+import pyro
+import pyro.distributions as dist
+import torch
+
+import torch.distributions.constraints as constraints
+
+from pyro.infer import SVI, Trace_ELBO, EmpiricalMarginal, TraceEnum_ELBO
+from pyro.infer.mcmc import MCMC, NUTS
+from pyro.optim import Adam, SGD
+
+import pyro.contrib.autoguide as autoguide
+
+import pandas as pd
+
+from functools import partial
+
+import numpy as np
+
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+
+# building off of ProdLDA model for amortization (text only for now) 
+# https://pyro.ai/examples/prodlda.html
+class Encoder(nn.Module):
+    # Base class for the encoder net, used in the guide
+    def __init__(self, vocab_size, num_dimensions, hidden, dropout):
+        super().__init__()
+        self.drop = nn.Dropout(dropout)  # to avoid component collapse
+        self.fc1 = nn.Linear(vocab_size, hidden)
+        self.fc2 = nn.Linear(hidden, hidden)
+        self.fcmu = nn.Linear(hidden, num_dimensions)
+        self.fclv = nn.Linear(hidden, num_dimensions)
+        # NB: here we set `affine=False` to reduce the number of learning parameters
+        # See https://pytorch.org/docs/stable/generated/torch.nn.BatchNorm1d.html
+        # for the effect of this flag in BatchNorm1d
+        self.bnmu = nn.BatchNorm1d(num_dimensions, affine=False)  # to avoid component collapse
+        self.bnlv = nn.BatchNorm1d(num_dimensions, affine=False)  # to avoid component collapse
+
+    def forward(self, inputs):
+        h = F.softplus(self.fc1(inputs))
+        h = F.softplus(self.fc2(h))
+        h = self.drop(h)
+        # μ and Σ are the outputs
+        logtheta_loc = self.bnmu(self.fcmu(h))
+        logtheta_logvar = self.bnlv(self.fclv(h))
+        logtheta_scale = (0.5 * logtheta_logvar).exp()  # Enforces positivity
+        return logtheta_loc, logtheta_scale
+
+
+class Decoder(nn.Module):
+    # Base class for the decoder net, used in the model
+    def __init__(self, vocab_size, num_dimensions, dropout):
+        super().__init__()
+        self.beta = nn.Linear(num_dimensions, vocab_size, bias=False)
+        self.bn = nn.BatchNorm1d(vocab_size, affine=False)
+        self.drop = nn.Dropout(dropout)
+
+    def forward(self, inputs):
+        inputs = self.drop(inputs)
+        # the output is σ(βθ)
+        return F.softmax(self.bn(self.beta(inputs)), dim=1)
+
+
+@abstract_model.IrtModel.register("amortized_1pl")
+class Amortized1PL(abstract_model.IrtModel):
+    
+    def __init__(
+        self, *, 
+        priors: str, 
+        num_items: int, 
+        num_subjects: int, 
+        verbose: bool = False, 
+        device: str = "cpu",
+        vocab_size: int,
+        dropout: float,
+        hidden: int,
+        **kwargs
+    ):
+        super().__init__(
+            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
+        )
+
+        # initialize the class with all arguments provided to the constructor
+        self.num_dimensions = 1
+        self.device = torch.device(device)
+        self.drop = dropout
+        self.hidden = hidden
+        self.num_items = num_items
+
+        self.vocab_size = vocab_size
+        self.encoder = Encoder(vocab_size, self.num_dimensions, self.hidden, self.drop)
+        self.decoder = Decoder(vocab_size, self.num_dimensions, self.drop)
+    
+
+    def model_irt(self, models, items, obs):
+        num_items = len(items)
+        options = dict(dtype=torch.float64, device=self.device)
+        #xs = torch.flatten(items, start_dim=1)
+        xs = items
+        models = torch.tensor(models, dtype=torch.long, device=items.device)
+        items = torch.tensor(items, dtype=torch.long, device=items.device)
+        obs = torch.tensor(obs, dtype=torch.float, device=items.device)
+
+        with pyro.plate("thetas"):
+            ability = pyro.sample('theta', dist.Normal(torch.zeros(self.num_subjects, **options),
+                torch.ones(self.num_subjects, **options)))
+        with pyro.plate("diffs", num_items):
+            # sample the item difficulty from the prior distribution
+            diff_prior_loc = torch.zeros(num_items, **options).unsqueeze(1).float()
+            diff_prior_scale = torch.ones(num_items, **options).fill_(1.e3).unsqueeze(1).float()
+            diff = pyro.sample('b', dist.Normal(diff_prior_loc, diff_prior_scale).to_event(1))
+            loc = self.decoder.forward(diff)
+            total_count = int(xs.sum(-1).max())
+            pyro.sample(
+                'items',
+                dist.Multinomial(total_count, loc),
+                obs=items
+            )
+            #diff = pyro.sample('b', dist.Normal(torch.zeros(num_items, **options),
+            #    torch.tensor(num_items, **options).fill_(1.e-3)))
+
+        with pyro.plate("data", len(obs)):
+            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff).to_event(1), obs=obs)
+        
+    def guide_irt(self, models, items, obs):
+        num_items = len(items)
+        options = dict(dtype=torch.float64, device=self.device)
+        #xs = torch.flatten(items, start_dim=1)
+        xs = items
+        # vectorize
+        models = torch.tensor(models, dtype=torch.long, device=self.device)
+        items = torch.tensor(items, dtype=torch.float, device=self.device)
+        obs = torch.tensor(obs, dtype=torch.float, device=self.device)
+
+
+        # register learnable params in the param store
+        with pyro.plate("thetas"):
+            m_theta_param = pyro.param("loc_ability", torch.zeros(self.num_subjects, **options))
+            s_theta_param = pyro.param("scale_ability", torch.ones(self.num_subjects, **options),
+                            constraint=constraints.positive)
+            dist_theta = dist.Normal(m_theta_param, s_theta_param)
+            pyro.sample("theta", dist_theta)
+
+        # items 
+        with pyro.plate("diffs", num_items):
+            irt_batch_size = 256
+            loc_diffs_all, scale_diffs_all = [], []
+            for i in range(0, len(items), irt_batch_size):
+                if len(items[i:]) < irt_batch_size:
+                    batch_xs = items[i:]
+                    loc_diffs, scale_diffs = self.encoder.forward(batch_xs)
+                    loc_diffs_all.extend(loc_diffs)
+                    scale_diffs_all.extend(scale_diffs) 
+                else:
+                    # pick out the appropriate images from xs based on items idx
+                    batch_xs = items[i:i+irt_batch_size]
+                    loc_diffs, scale_diffs = self.encoder.forward(batch_xs)            
+                    loc_diffs_all.extend(loc_diffs)
+                    scale_diffs_all.extend(scale_diffs)
+            loc_diffs_all = torch.tensor(loc_diffs_all, **options).unsqueeze(1).float()
+            scale_diffs_all = torch.tensor(scale_diffs_all, **options).unsqueeze(1).float()
+            dist_b = dist.Normal(loc_diffs_all, scale_diffs_all)
+            pyro.sample('b', dist_b.to_event(1))
+
+    def get_model(self):
+        return self.model_irt
+
+    def get_guide(self):
+        return self.guide_irt
+
+    def fit(self, models, items, responses, num_epochs):
+        """Fit the IRT model with variational inference"""
+        # need to step with IRT loss and with reconstruction loss
+
+        optim = Adam({"lr": 0.1})
+        svi = SVI(self.model_irt, self.guide_irt, optim, loss=Trace_ELBO())
+        #svi_diff = SVI(self.model, self.guide, optim, loss=Trace_ELBO())
+
+        pyro.clear_param_store()
+        for j in range(num_epochs):
+            loss = svi.step(models, items, responses)
+            #loss_diff = svi_diff.step(items)
+            if j % 100 == 0 and self.verbose:
+                print("[epoch %04d] irt loss: %.4f" % (j + 1, loss))
+                #print("[epoch %04d] recon loss: %.4f" % (j + 1, loss_diff))
+
+        print("[epoch %04d] loss: %.4f" % (j + 1, loss))
+        #print("[epoch %04d] loss: %.4f" % (j + 1, loss_diff))
+        values = ["loc_diff", "scale_diff", "loc_ability", "scale_ability"]
+
+    def export(self, items):
+        items = torch.tensor(items, dtype=torch.float)
+        diffs, _ = self.encoder.forward(items)
+        diffs = diffs.squeeze().detach().numpy()
+
+        return {
+            "ability": pyro.param("loc_ability").data.tolist(),
+            "diff": diffs.tolist()
+        }
+
+    def fit_MCMC(self, models, items, responses, num_epochs):
+        """Fit the IRT model with MCMC"""
+        sites = ["theta", "b"]
+        nuts_kernel = NUTS(self.model_vague, adapt_step_size=True)
+        hmc_posterior = MCMC(nuts_kernel, num_samples=1000, warmup_steps=100).run(
+            models, items, responses
+        )
+        theta_sum = self.summary(hmc_posterior, ["theta"]).items()
+        b_sum = self.summary(hmc_posterior, ["b"]).items()
+        
+    def predict(self, subjects, items, params_from_file=None):
+        """predict p(correct | params) for a specified list of model, item pairs"""
+        if params_from_file is not None:
+            model_params = params_from_file
+        else:
+            model_params = self.export(items)
+        abilities = np.array([model_params["ability"][i] for i in subjects])
+        diffs = np.array(model_params["diff"])
+        #items = torch.tensor(items, dtype=torch.float)
+        #diffs, _ = self.encoder.forward(items)
+        #diffs = diffs.squeeze().detach().numpy()
+        return 1 / (1 + np.exp(-(abilities - diffs)))
+
+    def summary(self, traces, sites):
+        """Aggregate marginals for MCM"""
+        marginal = (
+            EmpiricalMarginal(traces, sites)._get_samples_and_weights()[0].detach().cpu().numpy()
+        )
+        print(marginal)
+        site_stats = {}
+        for i in range(marginal.shape[1]):
+            site_name = sites[i]
+            marginal_site = pd.DataFrame(marginal[:, i]).transpose()
+            describe = partial(pd.Series.describe, percentiles=[0.05, 0.25, 0.5, 0.75, 0.95])
+            site_stats[site_name] = marginal_site.apply(describe, axis=1)[
+                ["mean", "std", "5%", "25%", "50%", "75%", "95%"]
+            ]
+        return site_stats
```

### Comparing `py_irt-0.6.1/py_irt/models/multidim_2pl.py` & `py_irt-0.6.2/py_irt/models/multidim_2pl.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,252 +1,252 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-import pyro
-import pyro.distributions as dist
-import torch
-import torch.distributions.constraints as constraints
-from rich.console import Console
-
-from py_irt.models.abstract_model import IrtModel
-
-console = Console()
-
-
-@IrtModel.register("multidim_2pl")
-class Multidim2PL(IrtModel):
-    def __init__(
-        self,
-        *,
-        num_items: int,
-        num_subjects: int,
-        dims: int = 2,
-        verbose=False,
-        device: str = "cpu",
-        **kwargs
-    ):
-        super().__init__(
-            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
-        )
-        self.dims = dims
-
-    def export(self):
-        return {
-            "ability": pyro.param("loc_ability").data.tolist(),
-            "diff": pyro.param("loc_diff").data.tolist(),
-            "disc": pyro.param("loc_disc").data.tolist(),
-        }
-
-    def get_model(self):
-        return self.model_hierarchical
-
-    def get_guide(self):
-        return self.guide_hierarchical
-
-    def model_hierarchical(self, subjects, items, obs):
-        with pyro.plate("mu_b_plate", self.dims):
-            mu_b = pyro.sample(
-                "mu_b",
-                dist.Normal(
-                    torch.tensor(0.0, device=self.device),
-                    torch.tensor(1.0e6, device=self.device),
-                ),
-            )
-
-        with pyro.plate("u_b_plate", self.dims):
-            u_b = pyro.sample(
-                "u_b",
-                dist.Gamma(
-                    torch.tensor(1.0, device=self.device),
-                    torch.tensor(1.0, device=self.device),
-                ),
-            )
-
-        with pyro.plate("mu_theta_plate", self.dims):
-            mu_theta = pyro.sample(
-                "mu_theta",
-                dist.Normal(
-                    torch.tensor(0.0, device=self.device),
-                    torch.tensor(1.0e6, device=self.device),
-                ),
-            )
-
-        with pyro.plate("u_theta_plate", self.dims):
-            u_theta = pyro.sample(
-                "u_theta",
-                dist.Gamma(
-                    torch.tensor(1.0, device=self.device),
-                    torch.tensor(1.0, device=self.device),
-                ),
-            )
-
-        with pyro.plate("mu_gamma_plate", self.dims):
-            mu_gamma = pyro.sample(
-                "mu_gamma",
-                dist.Normal(
-                    torch.tensor(0.0, device=self.device),
-                    torch.tensor(1.0e6, device=self.device),
-                ),
-            )
-
-        with pyro.plate("u_gamma_plate", self.dims):
-            u_gamma = pyro.sample(
-                "u_gamma",
-                dist.Gamma(
-                    torch.tensor(1.0, device=self.device),
-                    torch.tensor(1.0, device=self.device),
-                ),
-            )
-
-        with pyro.plate("thetas", self.num_subjects, dim=-2, device=self.device):
-            with pyro.plate("theta_dims", self.dims, dim=-1):
-                ability = pyro.sample("theta", dist.Normal(mu_theta, 1.0 / u_theta))
-
-        with pyro.plate("bs", self.num_items, dim=-2, device=self.device):
-            with pyro.plate("bs_dims", self.dims, dim=-1):
-                diff = pyro.sample("b", dist.Normal(mu_b, 1.0 / u_b))
-
-        with pyro.plate("gammas", self.num_items, dim=-2, device=self.device):
-            with pyro.plate("gamma_dims", self.dims, dim=-1):
-                disc = pyro.sample("gamma", dist.Normal(mu_gamma, 1.0 / u_gamma))
-
-        with pyro.plate("observe_data", obs.size(0)):
-            multidim_logits = disc[items] * (ability[subjects] - diff[items])
-            logits = multidim_logits.sum(axis=-1)
-
-            pyro.sample("obs", dist.Bernoulli(logits=logits), obs=obs)
-
-    def guide_hierarchical(self, subjects, items, obs):
-        loc_mu_b_param = pyro.param("loc_mu_b", torch.zeros(self.dims, device=self.device))
-        scale_mu_b_param = pyro.param(
-            "scale_mu_b",
-            1e2 * torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        loc_mu_theta_param = pyro.param("loc_mu_theta", torch.zeros(self.dims, device=self.device))
-        scale_mu_theta_param = pyro.param(
-            "scale_mu_theta",
-            1e2 * torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        loc_mu_gamma_param = pyro.param("loc_mu_gamma", torch.zeros(self.dims, device=self.device))
-        scale_mu_gamma_param = pyro.param(
-            "scale_mu_gamma",
-            1.0e2 * torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        alpha_b_param = pyro.param(
-            "alpha_b",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-        beta_b_param = pyro.param(
-            "beta_b",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        alpha_theta_param = pyro.param(
-            "alpha_theta",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-        beta_theta_param = pyro.param(
-            "beta_theta",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        alpha_gamma_param = pyro.param(
-            "alpha_gamma",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-        beta_gamma_param = pyro.param(
-            "beta_gamma",
-            torch.ones(self.dims, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        m_theta_param = pyro.param(
-            "loc_ability", torch.zeros([self.num_subjects, self.dims], device=self.device)
-        )
-        s_theta_param = pyro.param(
-            "scale_ability",
-            torch.ones([self.num_subjects, self.dims], device=self.device),
-            constraint=constraints.positive,
-        )
-
-        m_b_param = pyro.param(
-            "loc_diff", torch.zeros([self.num_items, self.dims], device=self.device)
-        )
-        s_b_param = pyro.param(
-            "scale_diff",
-            torch.ones([self.num_items, self.dims], device=self.device),
-            constraint=constraints.positive,
-        )
-
-        m_gamma_param = pyro.param(
-            "loc_disc", torch.zeros([self.num_items, self.dims], device=self.device)
-        )
-        s_gamma_param = pyro.param(
-            "scale_disc",
-            torch.ones([self.num_items, self.dims], device=self.device),
-            constraint=constraints.positive,
-        )
-
-        # sample statements
-        with pyro.plate("mu_b_plate", self.dims):
-            mu_b = pyro.sample("mu_b", dist.Normal(loc_mu_b_param, scale_mu_b_param))
-
-        with pyro.plate("u_b_plate", self.dims):
-            u_b = pyro.sample("u_b", dist.Gamma(alpha_b_param, beta_b_param))
-
-        with pyro.plate("mu_theta_plate", self.dims):
-            mu_theta = pyro.sample(
-                "mu_theta", dist.Normal(loc_mu_theta_param, scale_mu_theta_param)
-            )
-        with pyro.plate("u_theta_plate", self.dims):
-            u_theta = pyro.sample("u_theta", dist.Gamma(alpha_theta_param, beta_theta_param))
-
-        with pyro.plate("mu_gamma_plate", self.dims):
-            mu_gamma = pyro.sample(
-                "mu_gamma", dist.Normal(loc_mu_gamma_param, scale_mu_gamma_param)
-            )
-
-        with pyro.plate("u_gamma_plate", self.dims):
-            u_gamma = pyro.sample("u_gamma", dist.Gamma(alpha_gamma_param, beta_gamma_param))
-
-        with pyro.plate("thetas", self.num_subjects, dim=-2, device=self.device):
-            with pyro.plate("theta_dims", self.dims, dim=-1):
-                theta = pyro.sample("theta", dist.Normal(m_theta_param, s_theta_param))
-
-        with pyro.plate("bs", self.num_items, dim=-2, device=self.device):
-            with pyro.plate("bs_dims", self.dims, dim=-1):
-                b = pyro.sample("b", dist.Normal(m_b_param, s_b_param))
-
-        with pyro.plate("gammas", self.num_items, dim=-2, device=self.device):
-            with pyro.plate("gamma_dims", self.dims, dim=-1, device=self.device):
-                gamma = pyro.sample("gamma", dist.Normal(m_gamma_param, s_gamma_param))
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+import pyro
+import pyro.distributions as dist
+import torch
+import torch.distributions.constraints as constraints
+from rich.console import Console
+
+from py_irt.models.abstract_model import IrtModel
+
+console = Console()
+
+
+@IrtModel.register("multidim_2pl")
+class Multidim2PL(IrtModel):
+    def __init__(
+        self,
+        *,
+        num_items: int,
+        num_subjects: int,
+        dims: int = 2,
+        verbose=False,
+        device: str = "cpu",
+        **kwargs
+    ):
+        super().__init__(
+            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
+        )
+        self.dims = dims
+
+    def export(self):
+        return {
+            "ability": pyro.param("loc_ability").data.tolist(),
+            "diff": pyro.param("loc_diff").data.tolist(),
+            "disc": pyro.param("loc_disc").data.tolist(),
+        }
+
+    def get_model(self):
+        return self.model_hierarchical
+
+    def get_guide(self):
+        return self.guide_hierarchical
+
+    def model_hierarchical(self, subjects, items, obs):
+        with pyro.plate("mu_b_plate", self.dims):
+            mu_b = pyro.sample(
+                "mu_b",
+                dist.Normal(
+                    torch.tensor(0.0, device=self.device),
+                    torch.tensor(1.0e6, device=self.device),
+                ),
+            )
+
+        with pyro.plate("u_b_plate", self.dims):
+            u_b = pyro.sample(
+                "u_b",
+                dist.Gamma(
+                    torch.tensor(1.0, device=self.device),
+                    torch.tensor(1.0, device=self.device),
+                ),
+            )
+
+        with pyro.plate("mu_theta_plate", self.dims):
+            mu_theta = pyro.sample(
+                "mu_theta",
+                dist.Normal(
+                    torch.tensor(0.0, device=self.device),
+                    torch.tensor(1.0e6, device=self.device),
+                ),
+            )
+
+        with pyro.plate("u_theta_plate", self.dims):
+            u_theta = pyro.sample(
+                "u_theta",
+                dist.Gamma(
+                    torch.tensor(1.0, device=self.device),
+                    torch.tensor(1.0, device=self.device),
+                ),
+            )
+
+        with pyro.plate("mu_gamma_plate", self.dims):
+            mu_gamma = pyro.sample(
+                "mu_gamma",
+                dist.Normal(
+                    torch.tensor(0.0, device=self.device),
+                    torch.tensor(1.0e6, device=self.device),
+                ),
+            )
+
+        with pyro.plate("u_gamma_plate", self.dims):
+            u_gamma = pyro.sample(
+                "u_gamma",
+                dist.Gamma(
+                    torch.tensor(1.0, device=self.device),
+                    torch.tensor(1.0, device=self.device),
+                ),
+            )
+
+        with pyro.plate("thetas", self.num_subjects, dim=-2, device=self.device):
+            with pyro.plate("theta_dims", self.dims, dim=-1):
+                ability = pyro.sample("theta", dist.Normal(mu_theta, 1.0 / u_theta))
+
+        with pyro.plate("bs", self.num_items, dim=-2, device=self.device):
+            with pyro.plate("bs_dims", self.dims, dim=-1):
+                diff = pyro.sample("b", dist.Normal(mu_b, 1.0 / u_b))
+
+        with pyro.plate("gammas", self.num_items, dim=-2, device=self.device):
+            with pyro.plate("gamma_dims", self.dims, dim=-1):
+                disc = pyro.sample("gamma", dist.Normal(mu_gamma, 1.0 / u_gamma))
+
+        with pyro.plate("observe_data", obs.size(0)):
+            multidim_logits = disc[items] * (ability[subjects] - diff[items])
+            logits = multidim_logits.sum(axis=-1)
+
+            pyro.sample("obs", dist.Bernoulli(logits=logits), obs=obs)
+
+    def guide_hierarchical(self, subjects, items, obs):
+        loc_mu_b_param = pyro.param("loc_mu_b", torch.zeros(self.dims, device=self.device))
+        scale_mu_b_param = pyro.param(
+            "scale_mu_b",
+            1e2 * torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        loc_mu_theta_param = pyro.param("loc_mu_theta", torch.zeros(self.dims, device=self.device))
+        scale_mu_theta_param = pyro.param(
+            "scale_mu_theta",
+            1e2 * torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        loc_mu_gamma_param = pyro.param("loc_mu_gamma", torch.zeros(self.dims, device=self.device))
+        scale_mu_gamma_param = pyro.param(
+            "scale_mu_gamma",
+            1.0e2 * torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        alpha_b_param = pyro.param(
+            "alpha_b",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+        beta_b_param = pyro.param(
+            "beta_b",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        alpha_theta_param = pyro.param(
+            "alpha_theta",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+        beta_theta_param = pyro.param(
+            "beta_theta",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        alpha_gamma_param = pyro.param(
+            "alpha_gamma",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+        beta_gamma_param = pyro.param(
+            "beta_gamma",
+            torch.ones(self.dims, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        m_theta_param = pyro.param(
+            "loc_ability", torch.zeros([self.num_subjects, self.dims], device=self.device)
+        )
+        s_theta_param = pyro.param(
+            "scale_ability",
+            torch.ones([self.num_subjects, self.dims], device=self.device),
+            constraint=constraints.positive,
+        )
+
+        m_b_param = pyro.param(
+            "loc_diff", torch.zeros([self.num_items, self.dims], device=self.device)
+        )
+        s_b_param = pyro.param(
+            "scale_diff",
+            torch.ones([self.num_items, self.dims], device=self.device),
+            constraint=constraints.positive,
+        )
+
+        m_gamma_param = pyro.param(
+            "loc_disc", torch.zeros([self.num_items, self.dims], device=self.device)
+        )
+        s_gamma_param = pyro.param(
+            "scale_disc",
+            torch.ones([self.num_items, self.dims], device=self.device),
+            constraint=constraints.positive,
+        )
+
+        # sample statements
+        with pyro.plate("mu_b_plate", self.dims):
+            mu_b = pyro.sample("mu_b", dist.Normal(loc_mu_b_param, scale_mu_b_param))
+
+        with pyro.plate("u_b_plate", self.dims):
+            u_b = pyro.sample("u_b", dist.Gamma(alpha_b_param, beta_b_param))
+
+        with pyro.plate("mu_theta_plate", self.dims):
+            mu_theta = pyro.sample(
+                "mu_theta", dist.Normal(loc_mu_theta_param, scale_mu_theta_param)
+            )
+        with pyro.plate("u_theta_plate", self.dims):
+            u_theta = pyro.sample("u_theta", dist.Gamma(alpha_theta_param, beta_theta_param))
+
+        with pyro.plate("mu_gamma_plate", self.dims):
+            mu_gamma = pyro.sample(
+                "mu_gamma", dist.Normal(loc_mu_gamma_param, scale_mu_gamma_param)
+            )
+
+        with pyro.plate("u_gamma_plate", self.dims):
+            u_gamma = pyro.sample("u_gamma", dist.Gamma(alpha_gamma_param, beta_gamma_param))
+
+        with pyro.plate("thetas", self.num_subjects, dim=-2, device=self.device):
+            with pyro.plate("theta_dims", self.dims, dim=-1):
+                theta = pyro.sample("theta", dist.Normal(m_theta_param, s_theta_param))
+
+        with pyro.plate("bs", self.num_items, dim=-2, device=self.device):
+            with pyro.plate("bs_dims", self.dims, dim=-1):
+                b = pyro.sample("b", dist.Normal(m_b_param, s_b_param))
+
+        with pyro.plate("gammas", self.num_items, dim=-2, device=self.device):
+            with pyro.plate("gamma_dims", self.dims, dim=-1, device=self.device):
+                gamma = pyro.sample("gamma", dist.Normal(m_gamma_param, s_gamma_param))
```

### Comparing `py_irt-0.6.1/py_irt/models/one_param_logistic.py` & `py_irt-0.6.2/py_irt/models/one_param_logistic.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,271 +1,271 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-from py_irt.models import abstract_model
-import pyro
-import pyro.distributions as dist
-import torch
-
-import torch.distributions.constraints as constraints
-
-from pyro.infer import SVI, Trace_ELBO, EmpiricalMarginal, TraceEnum_ELBO
-from pyro.infer.mcmc import MCMC, NUTS
-from pyro.optim import Adam, SGD
-
-import pyro.contrib.autoguide as autoguide
-
-import pandas as pd
-
-from functools import partial
-
-import numpy as np
-
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-@abstract_model.IrtModel.register("1pl")
-class OneParamLog(abstract_model.IrtModel):
-    """1PL IRT model"""
-
-    def __init__(
-            self, *,
-            priors: str,
-            num_items: int,
-            num_subjects: int,
-            verbose: bool = False,
-            device: str = "cpu",
-            vocab_size: int = None,
-            dropout: float = None,
-            hidden: int = None,
-            **kwargs
-    ):
-        super().__init__(
-            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
-        )
-        if priors not in ["vague", "hierarchical"]:
-            raise ValueError("Options for priors are vague and hierarchical")
-        self.priors = priors
-
-    def model_vague(self, models, items, obs):
-        """Initialize a 1PL model with vague priors"""
-        with pyro.plate("thetas", self.num_subjects, device=self.device):
-            ability = pyro.sample(
-                "theta",
-                dist.Normal(
-                    torch.tensor(0.0, device=self.device), torch.tensor(1.0, device=self.device)
-                ),
-            )
-
-        with pyro.plate("bs", self.num_items, device=self.device):
-            diff = pyro.sample(
-                "b",
-                dist.Normal(
-                    torch.tensor(0.0, device=self.device), torch.tensor(1.0e3, device=self.device)
-                ),
-            )
-
-        with pyro.plate("observe_data", obs.size(0), device=self.device):
-            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff[items]), obs=obs)
-
-    def guide_vague(self, models, items, obs):
-        """Initialize a 1PL guide with vague priors"""
-        # register learnable params in the param store
-        m_theta_param = pyro.param(
-            "loc_ability", torch.zeros(self.num_subjects, device=self.device)
-        )
-        s_theta_param = pyro.param(
-            "scale_ability",
-            torch.ones(self.num_subjects, device=self.device),
-            constraint=constraints.positive,
-        )
-        m_b_param = pyro.param("loc_diff", torch.zeros(self.num_items, device=self.device))
-        s_b_param = pyro.param(
-            "scale_diff",
-            torch.empty(self.num_items, device=self.device).fill_(1.0e3),
-            constraint=constraints.positive,
-        )
-
-        # guide distributions
-        with pyro.plate("thetas", self.num_subjects, device=self.device):
-            dist_theta = dist.Normal(m_theta_param, s_theta_param)
-            pyro.sample("theta", dist_theta)
-        with pyro.plate("bs", self.num_items, device=self.device):
-            dist_b = dist.Normal(m_b_param, s_b_param)
-            pyro.sample("b", dist_b)
-
-    def model_hierarchical(self, models, items, obs):
-        """Initialize a 1PL model with hierarchical priors"""
-        mu_b = pyro.sample(
-            "mu_b",
-            dist.Normal(
-                torch.tensor(0.0, device=self.device), torch.tensor(1.0e6, device=self.device)
-            ),
-        )
-        u_b = pyro.sample(
-            "u_b",
-            dist.Gamma(
-                torch.tensor(1.0, device=self.device), torch.tensor(1.0, device=self.device)
-            ),
-        )
-        mu_theta = pyro.sample(
-            "mu_theta",
-            dist.Normal(
-                torch.tensor(0.0, device=self.device), torch.tensor(1.0e6, device=self.device)
-            ),
-        )
-        u_theta = pyro.sample(
-            "u_theta",
-            dist.Gamma(
-                torch.tensor(1.0, device=self.device), torch.tensor(1.0, device=self.device)
-            ),
-        )
-        with pyro.plate("thetas", self.num_subjects, device=self.device):
-            ability = pyro.sample("theta", dist.Normal(mu_theta, 1.0 / u_theta))
-        with pyro.plate("bs", self.num_items, device=self.device):
-            diff = pyro.sample("b", dist.Normal(mu_b, 1.0 / u_b))
-        with pyro.plate("observe_data", obs.size(0)):
-            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff[items]), obs=obs)
-
-    def guide_hierarchical(self, models, items, obs):
-        """Initialize a 1PL guide with hierarchical priors"""
-        loc_mu_b_param = pyro.param("loc_mu_b", torch.tensor(0.0, device=self.device))
-        scale_mu_b_param = pyro.param(
-            "scale_mu_b", torch.tensor(1.0e2, device=self.device), constraint=constraints.positive
-        )
-        loc_mu_theta_param = pyro.param("loc_mu_theta", torch.tensor(0.0, device=self.device))
-        scale_mu_theta_param = pyro.param(
-            "scale_mu_theta",
-            torch.tensor(1.0e2, device=self.device),
-            constraint=constraints.positive,
-        )
-        alpha_b_param = pyro.param(
-            "alpha_b", torch.tensor(1.0, device=self.device), constraint=constraints.positive
-        )
-        beta_b_param = pyro.param(
-            "beta_b", torch.tensor(1.0, device=self.device), constraint=constraints.positive
-        )
-        alpha_theta_param = pyro.param(
-            "alpha_theta", torch.tensor(1.0, device=self.device), constraint=constraints.positive
-        )
-        beta_theta_param = pyro.param(
-            "beta_theta", torch.tensor(1.0, device=self.device), constraint=constraints.positive
-        )
-        m_theta_param = pyro.param(
-            "loc_ability", torch.zeros(self.num_subjects, device=self.device)
-        )
-        s_theta_param = pyro.param(
-            "scale_ability",
-            torch.ones(self.num_subjects, device=self.device),
-            constraint=constraints.positive,
-        )
-        m_b_param = pyro.param("loc_diff", torch.zeros(self.num_items, device=self.device))
-        s_b_param = pyro.param(
-            "scale_diff",
-            torch.ones(self.num_items, device=self.device),
-            constraint=constraints.positive,
-        )
-
-        # sample statements
-        pyro.sample("mu_b", dist.Normal(loc_mu_b_param, scale_mu_b_param))
-        pyro.sample("u_b", dist.Gamma(alpha_b_param, beta_b_param))
-        pyro.sample("mu_theta", dist.Normal(loc_mu_theta_param, scale_mu_theta_param))
-        pyro.sample("u_theta", dist.Gamma(alpha_theta_param, beta_theta_param))
-
-        with pyro.plate("thetas", self.num_subjects, device=self.device):
-            pyro.sample("theta", dist.Normal(m_theta_param, s_theta_param))
-        with pyro.plate("bs", self.num_items, device=self.device):
-            pyro.sample("b", dist.Normal(m_b_param, s_b_param))
-
-    def get_model(self):
-        if self.priors == "vague":
-            return self.model_vague
-        else:
-            return self.model_hierarchical
-
-    def get_guide(self):
-        if self.priors == "vague":
-            return self.guide_vague
-        else:
-            return self.guide_hierarchical
-
-    def fit(self, models, items, responses, num_epochs):
-        """Fit the IRT model with variational inference"""
-        optim = Adam({"lr": 0.1})
-        if self.priors == "vague":
-            svi = SVI(self.model_vague, self.guide_vague, optim, loss=Trace_ELBO())
-        else:
-            svi = SVI(self.model_hierarchical, self.guide_hierarchical, optim, loss=Trace_ELBO())
-
-        pyro.clear_param_store()
-        for j in range(num_epochs):
-            loss = svi.step(models, items, responses)
-            if j % 100 == 0 and self.verbose:
-                print("[epoch %04d] loss: %.4f" % (j + 1, loss))
-
-        print("[epoch %04d] loss: %.4f" % (j + 1, loss))
-        values = ["loc_diff", "scale_diff", "loc_ability", "scale_ability"]
-
-    def export(self):
-        return {
-            "ability": pyro.param("loc_ability").data.tolist(),
-            "diff": pyro.param("loc_diff").data.tolist(),
-        }
-
-    def fit_MCMC(self, models, items, responses, num_epochs):
-        """Fit the IRT model with MCMC"""
-        sites = ["theta", "b"]
-        nuts_kernel = NUTS(self.model_vague, adapt_step_size=True)
-        hmc_posterior = MCMC(nuts_kernel, num_samples=1000, warmup_steps=100).run(
-            models, items, responses
-        )
-        theta_sum = self.summary(hmc_posterior, ["theta"]).items()
-        b_sum = self.summary(hmc_posterior, ["b"]).items()
-        print(theta_sum)
-        print(b_sum)
-
-    def predict(self, subjects, items, params_from_file=None):
-        """predict p(correct | params) for a specified list of model, item pairs"""
-        if params_from_file is not None:
-            model_params = params_from_file
-        else:
-            model_params = self.export()
-        abilities = np.array([model_params["ability"][i] for i in subjects])
-        diffs = np.array([model_params["diff"][i] for i in items])
-        return 1 / (1 + np.exp(-(abilities - diffs)))
-
-    def summary(self, traces, sites):
-        """Aggregate marginals for MCM"""
-        marginal = (
-            EmpiricalMarginal(traces, sites)._get_samples_and_weights()[0].detach().cpu().numpy()
-        )
-        print(marginal)
-        site_stats = {}
-        for i in range(marginal.shape[1]):
-            site_name = sites[i]
-            marginal_site = pd.DataFrame(marginal[:, i]).transpose()
-            describe = partial(pd.Series.describe, percentiles=[0.05, 0.25, 0.5, 0.75, 0.95])
-            site_stats[site_name] = marginal_site.apply(describe, axis=1)[
-                ["mean", "std", "5%", "25%", "50%", "75%", "95%"]
-            ]
-        return site_stats
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+from py_irt.models import abstract_model
+import pyro
+import pyro.distributions as dist
+import torch
+
+import torch.distributions.constraints as constraints
+
+from pyro.infer import SVI, Trace_ELBO, EmpiricalMarginal, TraceEnum_ELBO
+from pyro.infer.mcmc import MCMC, NUTS
+from pyro.optim import Adam, SGD
+
+import pyro.contrib.autoguide as autoguide
+
+import pandas as pd
+
+from functools import partial
+
+import numpy as np
+
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+@abstract_model.IrtModel.register("1pl")
+class OneParamLog(abstract_model.IrtModel):
+    """1PL IRT model"""
+
+    def __init__(
+            self, *,
+            priors: str,
+            num_items: int,
+            num_subjects: int,
+            verbose: bool = False,
+            device: str = "cpu",
+            vocab_size: int = None,
+            dropout: float = None,
+            hidden: int = None,
+            **kwargs
+    ):
+        super().__init__(
+            device=device, num_items=num_items, num_subjects=num_subjects, verbose=verbose
+        )
+        if priors not in ["vague", "hierarchical"]:
+            raise ValueError("Options for priors are vague and hierarchical")
+        self.priors = priors
+
+    def model_vague(self, models, items, obs):
+        """Initialize a 1PL model with vague priors"""
+        with pyro.plate("thetas", self.num_subjects, device=self.device):
+            ability = pyro.sample(
+                "theta",
+                dist.Normal(
+                    torch.tensor(0.0, device=self.device), torch.tensor(1.0, device=self.device)
+                ),
+            )
+
+        with pyro.plate("bs", self.num_items, device=self.device):
+            diff = pyro.sample(
+                "b",
+                dist.Normal(
+                    torch.tensor(0.0, device=self.device), torch.tensor(1.0e3, device=self.device)
+                ),
+            )
+
+        with pyro.plate("observe_data", obs.size(0), device=self.device):
+            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff[items]), obs=obs)
+
+    def guide_vague(self, models, items, obs):
+        """Initialize a 1PL guide with vague priors"""
+        # register learnable params in the param store
+        m_theta_param = pyro.param(
+            "loc_ability", torch.zeros(self.num_subjects, device=self.device)
+        )
+        s_theta_param = pyro.param(
+            "scale_ability",
+            torch.ones(self.num_subjects, device=self.device),
+            constraint=constraints.positive,
+        )
+        m_b_param = pyro.param("loc_diff", torch.zeros(self.num_items, device=self.device))
+        s_b_param = pyro.param(
+            "scale_diff",
+            torch.empty(self.num_items, device=self.device).fill_(1.0e3),
+            constraint=constraints.positive,
+        )
+
+        # guide distributions
+        with pyro.plate("thetas", self.num_subjects, device=self.device):
+            dist_theta = dist.Normal(m_theta_param, s_theta_param)
+            pyro.sample("theta", dist_theta)
+        with pyro.plate("bs", self.num_items, device=self.device):
+            dist_b = dist.Normal(m_b_param, s_b_param)
+            pyro.sample("b", dist_b)
+
+    def model_hierarchical(self, models, items, obs):
+        """Initialize a 1PL model with hierarchical priors"""
+        mu_b = pyro.sample(
+            "mu_b",
+            dist.Normal(
+                torch.tensor(0.0, device=self.device), torch.tensor(1.0e6, device=self.device)
+            ),
+        )
+        u_b = pyro.sample(
+            "u_b",
+            dist.Gamma(
+                torch.tensor(1.0, device=self.device), torch.tensor(1.0, device=self.device)
+            ),
+        )
+        mu_theta = pyro.sample(
+            "mu_theta",
+            dist.Normal(
+                torch.tensor(0.0, device=self.device), torch.tensor(1.0e6, device=self.device)
+            ),
+        )
+        u_theta = pyro.sample(
+            "u_theta",
+            dist.Gamma(
+                torch.tensor(1.0, device=self.device), torch.tensor(1.0, device=self.device)
+            ),
+        )
+        with pyro.plate("thetas", self.num_subjects, device=self.device):
+            ability = pyro.sample("theta", dist.Normal(mu_theta, 1.0 / u_theta))
+        with pyro.plate("bs", self.num_items, device=self.device):
+            diff = pyro.sample("b", dist.Normal(mu_b, 1.0 / u_b))
+        with pyro.plate("observe_data", obs.size(0)):
+            pyro.sample("obs", dist.Bernoulli(logits=ability[models] - diff[items]), obs=obs)
+
+    def guide_hierarchical(self, models, items, obs):
+        """Initialize a 1PL guide with hierarchical priors"""
+        loc_mu_b_param = pyro.param("loc_mu_b", torch.tensor(0.0, device=self.device))
+        scale_mu_b_param = pyro.param(
+            "scale_mu_b", torch.tensor(1.0e2, device=self.device), constraint=constraints.positive
+        )
+        loc_mu_theta_param = pyro.param("loc_mu_theta", torch.tensor(0.0, device=self.device))
+        scale_mu_theta_param = pyro.param(
+            "scale_mu_theta",
+            torch.tensor(1.0e2, device=self.device),
+            constraint=constraints.positive,
+        )
+        alpha_b_param = pyro.param(
+            "alpha_b", torch.tensor(1.0, device=self.device), constraint=constraints.positive
+        )
+        beta_b_param = pyro.param(
+            "beta_b", torch.tensor(1.0, device=self.device), constraint=constraints.positive
+        )
+        alpha_theta_param = pyro.param(
+            "alpha_theta", torch.tensor(1.0, device=self.device), constraint=constraints.positive
+        )
+        beta_theta_param = pyro.param(
+            "beta_theta", torch.tensor(1.0, device=self.device), constraint=constraints.positive
+        )
+        m_theta_param = pyro.param(
+            "loc_ability", torch.zeros(self.num_subjects, device=self.device)
+        )
+        s_theta_param = pyro.param(
+            "scale_ability",
+            torch.ones(self.num_subjects, device=self.device),
+            constraint=constraints.positive,
+        )
+        m_b_param = pyro.param("loc_diff", torch.zeros(self.num_items, device=self.device))
+        s_b_param = pyro.param(
+            "scale_diff",
+            torch.ones(self.num_items, device=self.device),
+            constraint=constraints.positive,
+        )
+
+        # sample statements
+        pyro.sample("mu_b", dist.Normal(loc_mu_b_param, scale_mu_b_param))
+        pyro.sample("u_b", dist.Gamma(alpha_b_param, beta_b_param))
+        pyro.sample("mu_theta", dist.Normal(loc_mu_theta_param, scale_mu_theta_param))
+        pyro.sample("u_theta", dist.Gamma(alpha_theta_param, beta_theta_param))
+
+        with pyro.plate("thetas", self.num_subjects, device=self.device):
+            pyro.sample("theta", dist.Normal(m_theta_param, s_theta_param))
+        with pyro.plate("bs", self.num_items, device=self.device):
+            pyro.sample("b", dist.Normal(m_b_param, s_b_param))
+
+    def get_model(self):
+        if self.priors == "vague":
+            return self.model_vague
+        else:
+            return self.model_hierarchical
+
+    def get_guide(self):
+        if self.priors == "vague":
+            return self.guide_vague
+        else:
+            return self.guide_hierarchical
+
+    def fit(self, models, items, responses, num_epochs):
+        """Fit the IRT model with variational inference"""
+        optim = Adam({"lr": 0.1})
+        if self.priors == "vague":
+            svi = SVI(self.model_vague, self.guide_vague, optim, loss=Trace_ELBO())
+        else:
+            svi = SVI(self.model_hierarchical, self.guide_hierarchical, optim, loss=Trace_ELBO())
+
+        pyro.clear_param_store()
+        for j in range(num_epochs):
+            loss = svi.step(models, items, responses)
+            if j % 100 == 0 and self.verbose:
+                print("[epoch %04d] loss: %.4f" % (j + 1, loss))
+
+        print("[epoch %04d] loss: %.4f" % (j + 1, loss))
+        values = ["loc_diff", "scale_diff", "loc_ability", "scale_ability"]
+
+    def export(self):
+        return {
+            "ability": pyro.param("loc_ability").data.tolist(),
+            "diff": pyro.param("loc_diff").data.tolist(),
+        }
+
+    def fit_MCMC(self, models, items, responses, num_epochs):
+        """Fit the IRT model with MCMC"""
+        sites = ["theta", "b"]
+        nuts_kernel = NUTS(self.model_vague, adapt_step_size=True)
+        hmc_posterior = MCMC(nuts_kernel, num_samples=1000, warmup_steps=100).run(
+            models, items, responses
+        )
+        theta_sum = self.summary(hmc_posterior, ["theta"]).items()
+        b_sum = self.summary(hmc_posterior, ["b"]).items()
+        print(theta_sum)
+        print(b_sum)
+
+    def predict(self, subjects, items, params_from_file=None):
+        """predict p(correct | params) for a specified list of model, item pairs"""
+        if params_from_file is not None:
+            model_params = params_from_file
+        else:
+            model_params = self.export()
+        abilities = np.array([model_params["ability"][i] for i in subjects])
+        diffs = np.array([model_params["diff"][i] for i in items])
+        return 1 / (1 + np.exp(-(abilities - diffs)))
+
+    def summary(self, traces, sites):
+        """Aggregate marginals for MCM"""
+        marginal = (
+            EmpiricalMarginal(traces, sites)._get_samples_and_weights()[0].detach().cpu().numpy()
+        )
+        print(marginal)
+        site_stats = {}
+        for i in range(marginal.shape[1]):
+            site_name = sites[i]
+            marginal_site = pd.DataFrame(marginal[:, i]).transpose()
+            describe = partial(pd.Series.describe, percentiles=[0.05, 0.25, 0.5, 0.75, 0.95])
+            site_stats[site_name] = marginal_site.apply(describe, axis=1)[
+                ["mean", "std", "5%", "25%", "50%", "75%", "95%"]
+            ]
+        return site_stats
```

### Comparing `py_irt-0.6.1/py_irt/scoring.py` & `py_irt-0.6.2/py_irt/scoring.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-
-"""
-Functions to facilitate theta estimation
-"""
-
-import numpy as np
-from scipy.optimize import minimize
-from scipy.stats import lognorm, norm
-from scipy.special import expit
-
-
-def theta_fn(difficulties, response_pattern):
-    """Estimate theta for a given response pattern"""
-
-    def fn(theta):
-        theta = theta[0]
-        probabilities = expit(theta - difficulties)
-        log_likelihood = 0
-        for i, rp in enumerate(response_pattern):
-            if rp == 0:
-                log_likelihood += np.log(1-probabilities[i])
-            else:
-                log_likelihood += np.log(probabilities[i])
-        return -log_likelihood
-
-    return fn
-
-
-def calculate_theta(difficulties, response_pattern, num_obs=-1):
-    """
-    Given learned item difficulties and a model response pattern, estimate theta
-    if num_obs > 0, then sample from the observed values for a computational speedup
-    """
-
-    if num_obs > 0:
-        samples = np.random.choice(len(difficulties), num_obs)
-        difficulties = [difficulties[s] for s in samples]
-        response_pattern = [response_pattern[s] for s in samples]
-
-    fn = theta_fn(difficulties, response_pattern)
-    result = minimize(fn, [0.1], method="BFGS")
-    return result["x"]
-
-
-def calculate_diff_threshold(p_correct, theta):
-    """
-    Calculate the difficulty threshold where the probability correct given theta is equal to p_correct
-    p_correct: the desired probability threshold
-    theta: estimated model ability at current timestep
-    """
-    return np.log(1 / p_correct - 1) + theta
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+
+"""
+Functions to facilitate theta estimation
+"""
+
+import numpy as np
+from scipy.optimize import minimize
+from scipy.stats import lognorm, norm
+from scipy.special import expit
+
+
+def theta_fn(difficulties, response_pattern):
+    """Estimate theta for a given response pattern"""
+
+    def fn(theta):
+        theta = theta[0]
+        probabilities = expit(theta - difficulties)
+        log_likelihood = 0
+        for i, rp in enumerate(response_pattern):
+            if rp == 0:
+                log_likelihood += np.log(1-probabilities[i])
+            else:
+                log_likelihood += np.log(probabilities[i])
+        return -log_likelihood
+
+    return fn
+
+
+def calculate_theta(difficulties, response_pattern, num_obs=-1):
+    """
+    Given learned item difficulties and a model response pattern, estimate theta
+    if num_obs > 0, then sample from the observed values for a computational speedup
+    """
+
+    if num_obs > 0:
+        samples = np.random.choice(len(difficulties), num_obs)
+        difficulties = [difficulties[s] for s in samples]
+        response_pattern = [response_pattern[s] for s in samples]
+
+    fn = theta_fn(difficulties, response_pattern)
+    result = minimize(fn, [0.1], method="BFGS")
+    return result["x"]
+
+
+def calculate_diff_threshold(p_correct, theta):
+    """
+    Calculate the difficulty threshold where the probability correct given theta is equal to p_correct
+    p_correct: the desired probability threshold
+    theta: estimated model ability at current timestep
+    """
+    return np.log(1 / p_correct - 1) + theta
```

### Comparing `py_irt-0.6.1/py_irt/training.py` & `py_irt-0.6.2/py_irt/training.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-# MIT License
-
-# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-from typing import Optional, Union, Dict
-from pathlib import Path
-
-import typer
-import torch
-
-from pyro.infer import SVI, Trace_ELBO
-import pyro
-
-from rich.console import Console
-from rich.live import Live
-from rich.table import Table
-
-from sklearn.feature_extraction.text import CountVectorizer
-
-
-# These imports are necessary to have @register run
-# pylint: disable=unused-import
-from py_irt.models import (
-    abstract_model,
-    one_param_logistic,
-    two_param_logistic,
-    three_param_logistic,
-    four_param_logistic,
-    multidim_2pl,
-    amortized_1pl,
-)
-from py_irt.io import safe_file, write_json
-from py_irt.dataset import Dataset
-from py_irt.initializers import INITIALIZERS, IrtInitializer
-from py_irt.config import IrtConfig
-from py_irt.models.abstract_model import IrtModel
-
-
-training_app = typer.Typer()
-console = Console()
-
-
-class IrtModelTrainer:
-    def __init__(
-        self,
-        *,
-        data_path: Path,
-        config: IrtConfig,
-        dataset: Optional[Dataset] = None,
-        verbose: bool = True,
-    ) -> None:
-        self._data_path = data_path
-        self._config = config
-        if isinstance(config.model_type, str):
-            IrtModel.validate_name(config.model_type)
-            self.amortized = "amortized" in self._config.model_type
-        else:
-            self.amortized = False
-        self._priors = None
-        self._device = None
-        self._epochs = None
-        self.irt_model: Optional[abstract_model.IrtModel] = None
-        self._pyro_model = None
-        self._pyro_guide = None
-        self._verbose = verbose
-        self.best_params = None
-        if dataset is None:
-            self._dataset = Dataset.from_jsonlines(data_path, amortized=self.amortized)
-        else:
-            self._dataset = dataset
-
-        if self.amortized:
-            self._config.vocab_size = len(self._dataset.observation_items[0])
-        console.log(f"Vocab size: {self._config.vocab_size}")
-
-        # filter out test data
-        training_idx = [
-            i
-            for i in range(len(self._dataset.training_example))
-            if self._dataset.training_example[i]
-        ]
-        self._dataset.observation_subjects = [
-            self._dataset.observation_subjects[i] for i in training_idx
-        ]
-        self._dataset.observation_items = [
-            self._dataset.observation_items[i] for i in training_idx
-        ]
-        self._dataset.observations = [
-            self._dataset.observations[i] for i in training_idx
-        ]
-        self._dataset.training_example = [
-            self._dataset.training_example[i] for i in training_idx
-        ]
-
-        if config.initializers is None:
-            initializers = []
-        else:
-            initializers = config.initializers
-
-        self._initializers = []
-        for init in initializers:
-            if isinstance(init, IrtInitializer):
-                self._initializers.append(init)
-            elif isinstance(init, str):
-                self._initializers.append(INITIALIZERS[init](self._dataset))
-            elif isinstance(init, Dict):
-                name = init.pop("name")
-                self._initializers.append(INITIALIZERS[name](self._dataset, **init))
-            else:
-                raise TypeError("invalid initializer type")
-
-    def train(self, *, epochs: Optional[int] = None, device: str = "cpu") -> None:
-        model_type = self._config.model_type
-        if epochs is None:
-            epochs = self._config.epochs
-        self._device = device
-        self._priors = self._config.priors
-        self._epochs = epochs
-        args = {
-            "device": device,
-            "num_items": len(self._dataset.ix_to_item_id),
-            "num_subjects": len(self._dataset.ix_to_subject_id),
-        }
-        console.log(f"args: {args}")
-        # TODO: Find a better solution to this
-        if self._config.priors is not None:
-            args["priors"] = self._config.priors
-        else:
-            args["priors"] = "vague"
-
-        if self._config.dims is not None:
-            args["dims"] = self._config.dims
-        args["dropout"] = self._config.dropout
-        args["hidden"] = self._config.hidden
-        args["vocab_size"] = self._config.vocab_size
-
-        console.log(f"Parsed Model Args: {args}")
-        if isinstance(model_type, str):
-            self.irt_model = IrtModel.from_name(model_type)(**args)
-        else:
-            self.irt_model = model_type(**args)
-            assert isinstance(self.irt_model, IrtModel)
-        pyro.clear_param_store()
-        self._pyro_model = self.irt_model.get_model()
-        self._pyro_guide = self.irt_model.get_guide()
-        device = torch.device(device)
-        scheduler = pyro.optim.ExponentialLR(
-            {
-                "optimizer": torch.optim.Adam,
-                "optim_args": {"lr": self._config.lr},
-                "gamma": self._config.lr_decay,
-            }
-        )
-        svi = SVI(self._pyro_model, self._pyro_guide, scheduler, loss=Trace_ELBO())
-        subjects = torch.tensor(
-            self._dataset.observation_subjects, dtype=torch.long, device=device
-        )
-        items = torch.tensor(
-            self._dataset.observation_items, dtype=torch.long, device=device
-        )
-        responses = torch.tensor(
-            self._dataset.observations, dtype=torch.float, device=device
-        )
-        print(subjects.size(), items.size())
-        # Don't take a step here, just make sure params are initialized
-        # so that initializers can modify the params
-        _ = self._pyro_model(subjects, items, responses)
-        _ = self._pyro_guide(subjects, items, responses)
-        for init in self._initializers:
-            init.initialize()
-
-        table = Table()
-        table.add_column("Epoch")
-        table.add_column("Loss")
-        table.add_column("Best Loss")
-        table.add_column("New LR")
-        loss = float("inf")
-        best_loss = loss
-        current_lr = self._config.lr
-        with Live(table) as live:
-            live.console.print(f"Training Pyro IRT Model for {epochs} epochs")
-            for epoch in range(epochs):
-                loss = svi.step(subjects, items, responses)
-                if loss < best_loss:
-                    best_loss = loss
-                    self.best_params = self.export(items)
-                scheduler.step()
-                current_lr = current_lr * self._config.lr_decay
-                if epoch % self._config.log_every == 0:
-                    table.add_row(
-                        f"{epoch + 1}",
-                        "%.4f" % loss,
-                        "%.4f" % best_loss,
-                        "%.4f" % current_lr,
-                    )
-
-            table.add_row(
-                f"{epoch + 1}", "%.4f" % loss, "%.4f" % best_loss, "%.4f" % current_lr
-            )
-            self.last_params = self.export(items)
-
-    def export(self, items):
-        if self.amortized:
-            vectorizer = CountVectorizer(max_df=0.5, min_df=20, stop_words="english")
-            inputs = list(self._dataset.item_ids)
-            vectorizer.fit(inputs)
-            inputs = vectorizer.transform(inputs).todense().tolist()
-            results = self.irt_model.export(inputs)
-        else:
-            results = self.irt_model.export()
-        results["irt_model"] = self._config.model_type
-        results["item_ids"] = self._dataset.ix_to_item_id
-        results["subject_ids"] = self._dataset.ix_to_subject_id
-        return results
-
-    def save(self, output_path: Union[str, Path]):
-        write_json(safe_file(output_path), self.last_params)
+# MIT License
+
+# Copyright (c) 2019 John Lalor <john.lalor@nd.edu> and Pedro Rodriguez <me@pedro.ai>
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+from typing import Optional, Union, Dict
+from pathlib import Path
+
+import typer
+import torch
+
+from pyro.infer import SVI, Trace_ELBO
+import pyro
+
+from rich.console import Console
+from rich.live import Live
+from rich.table import Table
+
+from sklearn.feature_extraction.text import CountVectorizer
+
+
+# These imports are necessary to have @register run
+# pylint: disable=unused-import
+from py_irt.models import (
+    abstract_model,
+    one_param_logistic,
+    two_param_logistic,
+    three_param_logistic,
+    four_param_logistic,
+    multidim_2pl,
+    amortized_1pl,
+)
+from py_irt.io import safe_file, write_json
+from py_irt.dataset import Dataset
+from py_irt.initializers import INITIALIZERS, IrtInitializer
+from py_irt.config import IrtConfig
+from py_irt.models.abstract_model import IrtModel
+
+
+training_app = typer.Typer()
+console = Console()
+
+
+class IrtModelTrainer:
+    def __init__(
+        self,
+        *,
+        data_path: Path,
+        config: IrtConfig,
+        dataset: Optional[Dataset] = None,
+        verbose: bool = True,
+    ) -> None:
+        self._data_path = data_path
+        self._config = config
+        if isinstance(config.model_type, str):
+            IrtModel.validate_name(config.model_type)
+            self.amortized = "amortized" in self._config.model_type
+        else:
+            self.amortized = False
+        self._priors = None
+        self._device = None
+        self._epochs = None
+        self.irt_model: Optional[abstract_model.IrtModel] = None
+        self._pyro_model = None
+        self._pyro_guide = None
+        self._verbose = verbose
+        self.best_params = None
+        if dataset is None:
+            self._dataset = Dataset.from_jsonlines(data_path, amortized=self.amortized)
+        else:
+            self._dataset = dataset
+
+        if self.amortized:
+            self._config.vocab_size = len(self._dataset.observation_items[0])
+        console.log(f"Vocab size: {self._config.vocab_size}")
+
+        # filter out test data
+        training_idx = [
+            i
+            for i in range(len(self._dataset.training_example))
+            if self._dataset.training_example[i]
+        ]
+        self._dataset.observation_subjects = [
+            self._dataset.observation_subjects[i] for i in training_idx
+        ]
+        self._dataset.observation_items = [
+            self._dataset.observation_items[i] for i in training_idx
+        ]
+        self._dataset.observations = [
+            self._dataset.observations[i] for i in training_idx
+        ]
+        self._dataset.training_example = [
+            self._dataset.training_example[i] for i in training_idx
+        ]
+
+        if config.initializers is None:
+            initializers = []
+        else:
+            initializers = config.initializers
+
+        self._initializers = []
+        for init in initializers:
+            if isinstance(init, IrtInitializer):
+                self._initializers.append(init)
+            elif isinstance(init, str):
+                self._initializers.append(INITIALIZERS[init](self._dataset))
+            elif isinstance(init, Dict):
+                name = init.pop("name")
+                self._initializers.append(INITIALIZERS[name](self._dataset, **init))
+            else:
+                raise TypeError("invalid initializer type")
+
+    def train(self, *, epochs: Optional[int] = None, device: str = "cpu") -> None:
+        model_type = self._config.model_type
+        if epochs is None:
+            epochs = self._config.epochs
+        self._device = device
+        self._priors = self._config.priors
+        self._epochs = epochs
+        args = {
+            "device": device,
+            "num_items": len(self._dataset.ix_to_item_id),
+            "num_subjects": len(self._dataset.ix_to_subject_id),
+        }
+        console.log(f"args: {args}")
+        # TODO: Find a better solution to this
+        if self._config.priors is not None:
+            args["priors"] = self._config.priors
+        else:
+            args["priors"] = "vague"
+
+        if self._config.dims is not None:
+            args["dims"] = self._config.dims
+        args["dropout"] = self._config.dropout
+        args["hidden"] = self._config.hidden
+        args["vocab_size"] = self._config.vocab_size
+
+        console.log(f"Parsed Model Args: {args}")
+        if isinstance(model_type, str):
+            self.irt_model = IrtModel.from_name(model_type)(**args)
+        else:
+            self.irt_model = model_type(**args)
+            assert isinstance(self.irt_model, IrtModel)
+        pyro.clear_param_store()
+        self._pyro_model = self.irt_model.get_model()
+        self._pyro_guide = self.irt_model.get_guide()
+        device = torch.device(device)
+        scheduler = pyro.optim.ExponentialLR(
+            {
+                "optimizer": torch.optim.Adam,
+                "optim_args": {"lr": self._config.lr},
+                "gamma": self._config.lr_decay,
+            }
+        )
+        svi = SVI(self._pyro_model, self._pyro_guide, scheduler, loss=Trace_ELBO())
+        subjects = torch.tensor(
+            self._dataset.observation_subjects, dtype=torch.long, device=device
+        )
+        items = torch.tensor(
+            self._dataset.observation_items, dtype=torch.long, device=device
+        )
+        responses = torch.tensor(
+            self._dataset.observations, dtype=torch.float, device=device
+        )
+        print(subjects.size(), items.size())
+        # Don't take a step here, just make sure params are initialized
+        # so that initializers can modify the params
+        _ = self._pyro_model(subjects, items, responses)
+        _ = self._pyro_guide(subjects, items, responses)
+        for init in self._initializers:
+            init.initialize()
+
+        table = Table()
+        table.add_column("Epoch")
+        table.add_column("Loss")
+        table.add_column("Best Loss")
+        table.add_column("New LR")
+        loss = float("inf")
+        best_loss = loss
+        current_lr = self._config.lr
+        with Live(table) as live:
+            live.console.print(f"Training Pyro IRT Model for {epochs} epochs")
+            for epoch in range(epochs):
+                loss = svi.step(subjects, items, responses)
+                if loss < best_loss:
+                    best_loss = loss
+                    self.best_params = self.export(items)
+                scheduler.step()
+                current_lr = current_lr * self._config.lr_decay
+                if epoch % self._config.log_every == 0:
+                    table.add_row(
+                        f"{epoch + 1}",
+                        "%.4f" % loss,
+                        "%.4f" % best_loss,
+                        "%.4f" % current_lr,
+                    )
+
+            table.add_row(
+                f"{epoch + 1}", "%.4f" % loss, "%.4f" % best_loss, "%.4f" % current_lr
+            )
+            self.last_params = self.export(items)
+
+    def export(self, items):
+        if self.amortized:
+            vectorizer = CountVectorizer(max_df=0.5, min_df=20, stop_words="english")
+            inputs = list(self._dataset.item_ids)
+            vectorizer.fit(inputs)
+            inputs = vectorizer.transform(inputs).todense().tolist()
+            results = self.irt_model.export(inputs)
+        else:
+            results = self.irt_model.export()
+        results["irt_model"] = self._config.model_type
+        results["item_ids"] = self._dataset.ix_to_item_id
+        results["subject_ids"] = self._dataset.ix_to_subject_id
+        return results
+
+    def save(self, output_path: Union[str, Path]):
+        write_json(safe_file(output_path), self.last_params)
```

### Comparing `py_irt-0.6.1/PKG-INFO` & `py_irt-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-irt
-Version: 0.6.1
+Version: 0.6.2
 Summary: Bayesian IRT models in Python
 Home-page: https://github.com/nd-ball/py-irt/
 License: MIT
 Author: John P. Lalor
 Author-email: john.lalor@nd.edu
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

