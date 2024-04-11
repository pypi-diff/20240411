# Comparing `tmp/flowMC-0.3.0.tar.gz` & `tmp/flowMC-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.3.0.tar", last modified: Fri Apr  5 21:30:46 2024, max compression
+gzip compressed data, was "flowMC-0.3.1.tar", last modified: Thu Apr 11 20:08:33 2024, max compression
```

## Comparing `flowMC-0.3.0.tar` & `flowMC-0.3.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-05 21:30:39.000000 flowMC-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-05 21:30:46.194362 flowMC-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-05 21:30:39.000000 flowMC-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-05 21:30:39.000000 flowMC-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-05 21:30:46.194362 flowMC-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.190362 flowMC-0.3.0/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/nfmodel/rqSpline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/proposal/
--rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/HMC.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/MALA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/proposal/flowHMC.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/global_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/strategy/importance_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/EvolutionaryOptimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-05 21:30:39.000000 flowMC-0.3.0/src/flowMC/utils/postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 21:30:46.194362 flowMC-0.3.0/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 21:30:46.000000 flowMC-0.3.0/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-11 20:08:29.000000 flowMC-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-11 20:08:33.527804 flowMC-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-11 20:08:29.000000 flowMC-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-11 20:08:29.000000 flowMC-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-11 20:08:33.527804 flowMC-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (127)    12800 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.523804 flowMC-0.3.1/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19506 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/nfmodel/rqSpline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/proposal/
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8563 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/proposal/flowHMC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9889 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/global_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/strategy/importance_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-11 20:08:29.000000 flowMC-0.3.1/src/flowMC/utils/postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:08:33.527804 flowMC-0.3.1/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:08:33.000000 flowMC-0.3.1/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowMC-0.3.0/LICENSE` & `flowMC-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.0/PKG-INFO` & `flowMC-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.0
+Version: 0.3.1
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.0 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.1 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowMC-0.3.0/README.md` & `flowMC-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flowMC-0.3.0/setup.cfg` & `flowMC-0.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flowMC
-version = 0.3.0
+version = 0.3.1
 author = Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 author_email = kazewong.physics@gmail.com
 url = https://github.com/kazewong/flowMC
 description = Normalizing flow exhanced sampler in jax
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = sampling, inference, machine learning, normalizing, autodiff, jax
```

### Comparing `flowMC-0.3.0/src/flowMC/Sampler.py` & `flowMC-0.3.1/src/flowMC/Sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pickle
-import jax
-import jax.numpy as jnp
-from jaxtyping import Array, Int, Float, PRNGKeyArray
-from tqdm import tqdm
+
 import equinox as eqx
+import jax.numpy as jnp
 import optax
-from flowMC.proposal.NF_proposal import NFProposal
-from flowMC.proposal.base import ProposalBase
+from jaxtyping import Array, Float, Int, PRNGKeyArray
+
 from flowMC.nfmodel.base import NFModel
+from flowMC.proposal.base import ProposalBase
+from flowMC.proposal.NF_proposal import NFProposal
 from flowMC.strategy.base import Strategy
-from flowMC.strategy.global_tuning import GlobalTuning, GlobalSampling
+from flowMC.strategy.global_tuning import GlobalSampling, GlobalTuning
 
 
 class Sampler:
     """
     Sampler class that host configuration parameters, NF model, and local sampler
 
     Args:
```

### Comparing `flowMC-0.3.0/src/flowMC/nfmodel/base.py` & `flowMC-0.3.1/src/flowMC/nfmodel/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from abc import abstractmethod
 import copy
+from abc import abstractmethod
+from typing import Optional, overload
+
 import equinox as eqx
-from typing import overload, Optional
-from typing_extensions import Self
-from jaxtyping import Array, PRNGKeyArray, Float
-import optax
-from tqdm import trange, tqdm
-import jax.numpy as jnp
 import jax
+import jax.numpy as jnp
+import optax
+from jaxtyping import Array, Float, PRNGKeyArray
+from tqdm import tqdm, trange
+from typing_extensions import Self
 
 
 class NFModel(eqx.Module):
     """
     Base class for normalizing flow models.
 
     This is an abstract template that should not be directly used.
@@ -98,17 +99,18 @@
             opt_state (optax.OptState): Optimizer state.
 
         Returns:
             loss (Array): Loss value.
             model (eqx.Model): Updated model.
             opt_state (optax.OptState): Updated optimizer state.
         """
-        loss, grads = self.loss_fn(x)
+        model = self
+        loss, grads = model.loss_fn(x)
         updates, state = optim.update(grads, state)
-        model = eqx.apply_updates(self, updates)
+        model = eqx.apply_updates(model, updates)
         return loss, model, state
 
     def train_epoch(
         self: Self,
         rng: PRNGKeyArray,
         optim: optax.GradientTransformation,
         state: optax.OptState,
@@ -158,35 +160,39 @@
             loss_values (Array): Loss values.
         """
         loss_values = jnp.zeros(num_epochs)
         if verbose:
             pbar = trange(num_epochs, desc="Training NF", miniters=int(num_epochs / 10))
         else:
             pbar = range(num_epochs)
+
         best_model = model = self
         best_loss = 1e9
         for epoch in pbar:
             # Use a separate PRNG key to permute image data during shuffling
             rng, input_rng = jax.random.split(rng)
             # Run an optimization step over a training batch
-            value, model, state = model.train_epoch(input_rng, optim, state, data, batch_size)
+            value, model, state = model.train_epoch(
+                input_rng, optim, state, data, batch_size
+            )
             loss_values = loss_values.at[epoch].set(value)
             if loss_values[epoch] < best_loss:
                 best_model = model
+                best_state = state
                 best_loss = loss_values[epoch]
             if verbose:
                 assert isinstance(pbar, tqdm)
                 if num_epochs > 10:
                     if epoch % int(num_epochs / 10) == 0:
                         pbar.set_description(f"Training NF, current loss: {value:.3f}")
                 else:
                     if epoch == num_epochs:
                         pbar.set_description(f"Training NF, current loss: {value:.3f}")
 
-        return rng, best_model, state, loss_values
+        return rng, best_model, best_state, loss_values
 
 
 class Bijection(eqx.Module):
     """
     Base class for bijective transformations.
 
     This is an abstract template that should not be directly used."""
```

### Comparing `flowMC-0.3.0/src/flowMC/nfmodel/common.py` & `flowMC-0.3.1/src/flowMC/nfmodel/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from typing import Callable, List, Tuple
 
-import jax
-import jax.numpy as jnp
-from jaxtyping import Array
 import equinox as eqx
-
-from flowMC.nfmodel.base import Bijection, Distribution
-
 import jax
 import jax.numpy as jnp
-import equinox as eqx
 from jaxtyping import Array, Float, PRNGKeyArray
 
+from flowMC.nfmodel.base import Bijection, Distribution
+
 
 class MLP(eqx.Module):
     r"""Multilayer perceptron.
 
     Args:
         shape (List[int]): Shape of the MLP. The first element is the input dimension, the last element is the output dimension.
         key (PRNGKeyArray): Random key.
```

### Comparing `flowMC-0.3.0/src/flowMC/nfmodel/realNVP.py` & `flowMC-0.3.1/src/flowMC/nfmodel/realNVP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from functools import partial
 from typing import List, Tuple
+
+import equinox as eqx
 import jax
 import jax.numpy as jnp
 import numpy as np
-import equinox as eqx
-from flowMC.nfmodel.base import NFModel, Distribution
-from flowMC.nfmodel.common import MLP, MaskedCouplingLayer, MLPAffine, Gaussian
-from jaxtyping import Array, Float, PRNGKeyArray
-from functools import partial
 import optax
+from jaxtyping import Array, Float, PRNGKeyArray
+
+from flowMC.nfmodel.base import Distribution, NFModel
+from flowMC.nfmodel.common import MLP, Gaussian, MaskedCouplingLayer, MLPAffine
 
 
 class AffineCoupling(eqx.Module):
     """
     Affine coupling layer.
     (Defined in the RealNVP paper https://arxiv.org/abs/1605.08803)
     We use tanh as the default activation function.
```

### Comparing `flowMC-0.3.0/src/flowMC/nfmodel/rqSpline.py` & `flowMC-0.3.1/src/flowMC/nfmodel/rqSpline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from functools import partial
+
+import equinox as eqx
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array, PRNGKeyArray, Float
-import equinox as eqx
+from jaxtyping import Array, Float, PRNGKeyArray
 
-from flowMC.nfmodel.base import NFModel, Bijection, Distribution
-from flowMC.nfmodel.common import MaskedCouplingLayer, ScalarAffine, MLP, Gaussian
-from functools import partial
+from flowMC.nfmodel.base import Bijection, Distribution, NFModel
+from flowMC.nfmodel.common import (MLP, Gaussian, MaskedCouplingLayer,
+                                   ScalarAffine)
 
 
 @partial(jax.vmap, in_axes=(0, None, None))
 def _normalize_bin_sizes(
     unnormalized_bin_sizes: Array, total_size: float, min_bin_size: float
 ) -> Array:
     """Make bin sizes sum to `total_size` and be no less than `min_bin_size`."""
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/Gaussian_random_walk.py` & `flowMC-0.3.1/src/flowMC/proposal/Gaussian_random_walk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Callable
+
 import jax
 import jax.numpy as jnp
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
 from tqdm import tqdm
+
 from flowMC.proposal.base import ProposalBase
-from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray
 
 
 class GaussianRandomWalk(ProposalBase):
     """
     Gaussian random walk sampler class builiding the rw_sampler method
 
     Args:
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/HMC.py` & `flowMC-0.3.1/src/flowMC/proposal/HMC.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Callable
+
 import jax
 import jax.numpy as jnp
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
 from tqdm import tqdm
+
 from flowMC.proposal.base import ProposalBase
-from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray
 
 
 class HMC(ProposalBase):
     """
     Hamiltonian Monte Carlo sampler class builiding the hmc_sampler method
     from target logpdf.
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/MALA.py` & `flowMC-0.3.1/src/flowMC/proposal/MALA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from functools import partialmethod
 from typing import Callable
+
 import jax
 import jax.numpy as jnp
 from jax.scipy.stats import multivariate_normal
+from jaxtyping import Array, Bool, Float, Int, PRNGKeyArray, PyTree
 from tqdm import tqdm
+
 from flowMC.proposal.base import ProposalBase
-from functools import partialmethod
-from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray, Bool
 
 
 class MALA(ProposalBase):
     """
     Metropolis-adjusted Langevin algorithm sampler clas
     builiding the mala_sampler method
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/NF_proposal.py` & `flowMC-0.3.1/src/flowMC/proposal/NF_proposal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from math import ceil
+from typing import Callable
+
 import jax
 import jax.numpy as jnp
 from jax import random
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
 from tqdm import tqdm
+
 from flowMC.nfmodel.base import NFModel
-from typing import Callable
 from flowMC.proposal.base import ProposalBase
-from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
-from math import ceil
 
 
 @jax.tree_util.register_pytree_node_class
 class NFProposal(ProposalBase):
     model: NFModel
 
     def __init__(
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/base.py` & `flowMC-0.3.1/src/flowMC/proposal/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import abstractmethod
 from typing import Callable
+
 import jax
 import jax.numpy as jnp
-from jaxtyping import PyTree, Array, Float, Int, PRNGKeyArray
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
 
 
 @jax.tree_util.register_pytree_node_class
 class ProposalBase:
     def __init__(
         self,
         logpdf: Callable[[Float[Array, " n_dim"], PyTree], Float],
```

### Comparing `flowMC-0.3.0/src/flowMC/proposal/flowHMC.py` & `flowMC-0.3.1/src/flowMC/proposal/flowHMC.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from math import ceil
+from typing import Callable
+
 import jax
 import jax.numpy as jnp
+from jax import random
+from jaxtyping import Array, Float, Int, PRNGKeyArray, PyTree
+from tqdm import tqdm
+
 from flowMC.nfmodel.base import NFModel
-from jaxtyping import Array, PRNGKeyArray, PyTree
-from typing import Callable
 from flowMC.proposal.HMC import HMC
 from flowMC.proposal.NF_proposal import NFProposal
-from jaxtyping import Array, Float, Int, PRNGKeyArray
-from math import ceil
-from jax import random
-from tqdm import tqdm
 
 ###################################
 # This is not in production yet
 ###################################
 
 
 # Note that the inverse metric needs float64 precision
```

### Comparing `flowMC-0.3.0/src/flowMC/strategy/base.py` & `flowMC-0.3.1/src/flowMC/strategy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from abc import abstractmethod
+
+from jaxtyping import Array, Float, PRNGKeyArray, PyTree
+
 from flowMC.proposal.base import ProposalBase
 from flowMC.proposal.NF_proposal import NFProposal
-from jaxtyping import Array, Float, PRNGKeyArray, PyTree
+
+
 class Strategy:
     """
     Base class for strategies, which are basically wrapper blocks that modify the state of the sampler
 
     This is an abstract template that should not be directly used.
     
     """
```

### Comparing `flowMC-0.3.0/src/flowMC/strategy/global_tuning.py` & `flowMC-0.3.1/src/flowMC/strategy/global_tuning.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from flowMC.proposal.base import ProposalBase
-from flowMC.proposal.NF_proposal import NFProposal
-from flowMC.strategy.base import Strategy
+import equinox as eqx
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array, Float, PRNGKeyArray, PyTree
 import optax
-import equinox as eqx
+from jaxtyping import Array, Float, PRNGKeyArray, PyTree
 from tqdm import tqdm
 
+from flowMC.proposal.base import ProposalBase
+from flowMC.proposal.NF_proposal import NFProposal
+from flowMC.strategy.base import Strategy
+
 
 class GlobalTuning(Strategy):
 
     optim: optax.GradientTransformation
     optim_state: optax.OptState
 
     n_dim: int
@@ -72,29 +73,30 @@
 
         summary = {}
         summary["chains"] = jnp.empty((self.n_chains, 0, self.n_dim))
         summary["log_prob"] = jnp.empty((self.n_chains, 0))
         summary["local_accs"] = jnp.empty((self.n_chains, 0))
         summary["global_accs"] = jnp.empty((self.n_chains, 0))
         summary["loss_vals"] = jnp.empty((0, self.n_epochs))
+        current_position = initial_position
         for _ in tqdm(
             range(self.n_loop),
             desc="Global Tuning",
         ):
             rng_key, rng_keys_mcmc = jax.random.split(rng_key)
             rng_keys_mcmc = jax.random.split(rng_keys_mcmc, self.n_chains)
             (
                 rng_keys_mcmc,
                 positions,
                 log_prob,
                 local_acceptance,
             ) = local_sampler.sample(
                 rng_keys_mcmc,
                 self.n_local_steps,
-                initial_position,
+                current_position,
                 data,
                 verbose=self.verbose,
             )
 
             summary["chains"] = jnp.append(
                 summary["chains"],
                 positions[:, :: self.output_thinning],
@@ -108,14 +110,16 @@
 
             summary["local_accs"] = jnp.append(
                 summary["local_accs"],
                 local_acceptance[:, 1 :: self.output_thinning],
                 axis=1,
             )
 
+            current_position = summary["chains"][:, -1]
+
             rng_key, rng_keys_nf = jax.random.split(rng_key)
             positions = summary["chains"][:, :: self.train_thinning]
             chain_size = positions.shape[0] * positions.shape[1]
             if chain_size > self.n_max_examples:
                 flat_chain = positions[
                     :, -int(self.n_max_examples / self.n_chains) :
                 ].reshape(-1, self.n_dim)
@@ -138,41 +142,43 @@
             )
             global_sampler.model = eqx.tree_at(
                 lambda m: m._data_cov, global_sampler.model, data_cov
             )
 
             (
                 rng_keys_nf,
-                global_sampler.model,
-                self.optim_state,
+                model,
+                optim_state,
                 loss_values,
             ) = global_sampler.model.train(
                 rng_keys_nf,
                 flat_chain,
                 self.optim,
                 self.optim_state,
                 self.n_epochs,
                 self.batch_size,
                 self.verbose,
             )
+            global_sampler.model = model
+            self.optim_state = optim_state
             summary["loss_vals"] = jnp.append(
                 summary["loss_vals"],
                 loss_values.reshape(1, -1),
                 axis=0,
             )
 
             (
                 rng_keys_nf,
                 nf_chain,
                 log_prob,
                 global_acceptance,
             ) = global_sampler.sample(
                 rng_keys_nf,
                 self.n_global_steps,
-                positions[:, -1],
+                current_position,
                 data,
                 verbose=self.verbose,
             )
 
             summary["chains"] = jnp.append(
                 summary["chains"],
                 nf_chain[:, :: self.output_thinning],
@@ -186,15 +192,17 @@
 
             summary["global_accs"] = jnp.append(
                 summary["global_accs"],
                 global_acceptance[:, 1 :: self.output_thinning],
                 axis=1,
             )
 
-        return rng_key, summary['chains'][:, -1], local_sampler, global_sampler, summary
+            current_position = summary["chains"][:, -1]
+
+        return rng_key, current_position, local_sampler, global_sampler, summary
 
 
 class GlobalSampling(Strategy):
 
     n_dim: int
     n_chains: int
     n_local_steps: int
@@ -235,29 +243,30 @@
 
         summary = {}
         summary["chains"] = jnp.empty((self.n_chains, 0, self.n_dim))
         summary["log_prob"] = jnp.empty((self.n_chains, 0))
         summary["local_accs"] = jnp.empty((self.n_chains, 0))
         summary["global_accs"] = jnp.empty((self.n_chains, 0))
 
+        current_position = initial_position
         for _ in tqdm(
             range(self.n_loop),
             desc="Global Sampling",
         ):
             rng_key, rng_keys_mcmc = jax.random.split(rng_key)
             rng_keys_mcmc = jax.random.split(rng_keys_mcmc, self.n_chains)
             (
                 rng_keys_mcmc,
                 positions,
                 log_prob,
                 local_acceptance,
             ) = local_sampler.sample(
                 rng_keys_mcmc,
                 self.n_local_steps,
-                initial_position,
+                current_position,
                 data,
                 verbose=self.verbose,
             )
 
             summary["chains"] = jnp.append(
                 summary["chains"],
                 positions[:, :: self.output_thinning],
@@ -271,14 +280,16 @@
 
             summary["local_accs"] = jnp.append(
                 summary["local_accs"],
                 local_acceptance[:, 1 :: self.output_thinning],
                 axis=1,
             )
 
+            current_position = summary["chains"][:, -1]
+
             rng_key, rng_keys_nf = jax.random.split(rng_key)
             (
                 rng_keys_nf,
                 nf_chain,
                 log_prob,
                 global_acceptance,
             ) = global_sampler.sample(
@@ -302,8 +313,10 @@
 
             summary["global_accs"] = jnp.append(
                 summary["global_accs"],
                 global_acceptance[:, 1 :: self.output_thinning],
                 axis=1,
             )
 
+            current_position = summary["chains"][:, -1]
+
         return rng_key, summary['chains'][:, -1], local_sampler, global_sampler, summary
```

### Comparing `flowMC-0.3.0/src/flowMC/utils/EvolutionaryOptimizer.py` & `flowMC-0.3.1/src/flowMC/utils/EvolutionaryOptimizer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from evosax import CMA_ES
 import jax
 import jax.numpy as jnp
-from jaxtyping import PRNGKeyArray
 import tqdm
+from evosax import CMA_ES
+from jaxtyping import PRNGKeyArray
 
 
 class EvolutionaryOptimizer:
     """
     A wrapper class for the evosax package.
     Note that we do not aim to solve any generic optimization problem,
     especially in a high dimension space.
```

### Comparing `flowMC-0.3.0/src/flowMC/utils/PythonFunctionWrap.py` & `flowMC-0.3.1/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 from functools import wraps
-from typing import Any, List, Dict, Callable, Iterable, Tuple, NamedTuple, Union
+from typing import (Any, Callable, Dict, Iterable, List, NamedTuple, Tuple,
+                    Union)
 
 Array = Any
 PyTree = Union[Array, Iterable[Array], Dict[Any, Array], NamedTuple]
 SampleStats = Dict[str, Array]
 Extras = PyTree
 
 import jax
```

### Comparing `flowMC-0.3.0/src/flowMC/utils/postprocessing.py` & `flowMC-0.3.1/src/flowMC/utils/postprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import matplotlib.pyplot as plt
 import jax.numpy as jnp
+import matplotlib.pyplot as plt
 # from flowMC.sampler.Sampler import Sampler
-from jaxtyping import Float, Array
+from jaxtyping import Array, Float
+
 
 def plot_summary(sampler: object, training: bool = False, **plotkwargs) -> None:
     """
     Create plots of the most important quantities in the summary.
 
     Args:
         training (bool, optional): If True, plot training quantities. If False, plot production quantities. Defaults to False.
```

### Comparing `flowMC-0.3.0/src/flowMC.egg-info/PKG-INFO` & `flowMC-0.3.1/src/flowMC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.3.0
+Version: 0.3.1
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
 Requires-Python: >=3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.3.0 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.3.1 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
 learning,normalizing,autodiff,jax Requires-Python: >=3.10 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: jax>=0.4.12 Requires-
 Dist: jaxlib>=0.4.12 Requires-Dist: equinox>=0.10.6 Requires-Dist: optax>=0.1.5
 Requires-Dist: evosax>=0.1.4 Requires-Dist: tqdm Requires-Dist: corner # flowMC
```

### Comparing `flowMC-0.3.0/src/flowMC.egg-info/SOURCES.txt` & `flowMC-0.3.1/src/flowMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

