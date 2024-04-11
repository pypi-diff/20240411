# Comparing `tmp/phasegen-0.0.5b0.tar.gz` & `tmp/phasegen-0.0.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasegen-0.0.5b0.tar", max compression
+gzip compressed data, was "phasegen-0.0.6b0.tar", max compression
```

## Comparing `phasegen-0.0.5b0.tar` & `phasegen-0.0.6b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      725 2024-04-06 17:40:09.560423 phasegen-0.0.5b0/README.md
--rw-r--r--   0        0        0     4631 2024-04-06 17:40:09.568423 phasegen-0.0.5b0/phasegen/__init__.py
--rw-r--r--   0        0        0    15046 2024-04-06 17:40:09.568423 phasegen-0.0.5b0/phasegen/coalescent_models.py
--rw-r--r--   0        0        0    14599 2024-04-06 17:40:09.568423 phasegen-0.0.5b0/phasegen/comparison.py
--rw-r--r--   0        0        0    37008 2024-04-06 17:40:09.568423 phasegen-0.0.5b0/phasegen/demography.py
--rw-r--r--   0        0        0    93421 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/distributions.py
--rw-r--r--   0        0        0     1652 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/expm.py
--rw-r--r--   0        0        0    25126 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/inference.py
--rw-r--r--   0        0        0     2378 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/lineage.py
--rw-r--r--   0        0        0     2745 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/locus.py
--rw-r--r--   0        0        0     2653 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/norms.py
--rw-r--r--   0        0        0    16983 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/rewards.py
--rw-r--r--   0        0        0     1121 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/serialization.py
--rw-r--r--   0        0        0    11098 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/spectrum.py
--rw-r--r--   0        0        0    29122 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/state_space.py
--rw-r--r--   0        0        0    53272 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/state_space_old.py
--rw-r--r--   0        0        0     1230 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/utils.py
--rw-r--r--   0        0        0     4478 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/phasegen/visualization.py
--rw-r--r--   0        0        0      931 2024-04-06 17:40:09.572423 phasegen-0.0.5b0/pyproject.toml
--rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.5b0/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-04-11 08:07:49.318896 phasegen-0.0.6b0/README.md
+-rw-r--r--   0        0        0     4599 2024-04-11 08:07:49.330896 phasegen-0.0.6b0/phasegen/__init__.py
+-rw-r--r--   0        0        0    15044 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/coalescent_models.py
+-rw-r--r--   0        0        0    14462 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/comparison.py
+-rw-r--r--   0        0        0    36975 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/demography.py
+-rw-r--r--   0        0        0    80702 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/distributions.py
+-rw-r--r--   0        0        0     1722 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/expm.py
+-rw-r--r--   0        0        0    27043 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/inference.py
+-rw-r--r--   0        0        0     2378 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/lineage.py
+-rw-r--r--   0        0        0     2751 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/locus.py
+-rw-r--r--   0        0        0     2653 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/norms.py
+-rw-r--r--   0        0        0    16757 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/rewards.py
+-rw-r--r--   0        0        0     1121 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/serialization.py
+-rw-r--r--   0        0        0    11106 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/spectrum.py
+-rw-r--r--   0        0        0    29433 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/state_space.py
+-rw-r--r--   0        0        0    53110 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/state_space_old.py
+-rw-r--r--   0        0        0     1230 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/utils.py
+-rw-r--r--   0        0        0     4478 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/phasegen/visualization.py
+-rw-r--r--   0        0        0      931 2024-04-11 08:07:49.334896 phasegen-0.0.6b0/pyproject.toml
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.6b0/PKG-INFO
```

### Comparing `phasegen-0.0.5b0/README.md` & `phasegen-0.0.6b0/README.md`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/phasegen/__init__.py` & `phasegen-0.0.6b0/phasegen/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PhaseGen package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-04-09"
 
-__version__ = '0.0.5-beta'
+__version__ = '0.0.6-beta'
 
 import logging
 import os
 import sys
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 from tqdm import tqdm
@@ -135,16 +135,14 @@
     StateSpace,
     DefaultStateSpace,
     BlockCountingStateSpace
 )
 
 from .rewards import (
     Reward,
-    DefaultReward,
-    NonDefaultReward,
     TreeHeightReward,
     TotalTreeHeightReward,
     TotalBranchLengthReward,
     UnfoldedSFSReward,
     FoldedSFSReward,
     CustomReward,
     ProductReward,
@@ -171,14 +169,16 @@
     L2Norm,
     LInfNorm,
     PoissonLikelihood
 )
 
 from .state_space_old import StateSpace as OldStateSpace
 
+from .expm import Backend, SciPyExpm, TensorFlowExpm
+
 __all__ = [
     'PhaseTypeDistribution',
     'Coalescent',
     'Demography',
     'Epoch',
     'PopSizeChanges',
     'PopSizeChange',
@@ -209,16 +209,14 @@
     'TotalBranchLengthReward',
     'UnfoldedSFSReward',
     'FoldedSFSReward',
     'CustomReward',
     'ProductReward',
     'SumReward',
     'DemeReward',
-    'DefaultReward',
-    'NonDefaultReward',
     'CombinedReward',
     'StateSpace',
     'DefaultStateSpace',
     'BlockCountingStateSpace',
     'CoalescentModel',
     'LineageConfig',
     'LocusConfig',
```

### Comparing `phasegen-0.0.5b0/phasegen/coalescent_models.py` & `phasegen-0.0.6b0/phasegen/coalescent_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,15 @@
         """
         Initialize the Dirac coalescent model.
 
         :param psi: The fraction of the population replaced by offspring in one large reproduction event
         :param c: The rate of potential multiple merger events.
         :param scale_time: Whether to scale coalescence time as described in
             `Msprime docs <https://tskit.dev/msprime/docs/stable/api.html?
-            highlight=dirac+coalescent#msprime.DiracCoalescent>`__. If ``False``, the timescale is set to N.
+            highlight=dirac+coalescent#msprime.DiracCoalescent>`__. If `False`, the timescale is set to N.
         """
         super().__init__()
 
         if not 0 < psi < 1:
             raise ValueError("Psi must be between 0 and 1.")
 
         #: The fraction of the population replaced by offspring in one large reproduction event
```

### Comparing `phasegen-0.0.5b0/phasegen/comparison.py` & `phasegen-0.0.6b0/phasegen/comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,17 @@
 
         :param n: Either a single integer if only one population, or a list of integers
             or a dictionary with population names as keys and number of lineages as values.
         :param pop_sizes: Population sizes. Either a dictionary of the form ``{pop_i: {time1: size1, time2: size2}}``,
             indexed by population name, or a list of dictionaries of the form ``{time1: size1, time2: size2}`` ordered
             by population index, or a single dictionary of the form ``{time1: size1, time2: size2}`` for a single
             population. Note that the first time must always be 0.
-        :param migration_rates: Migration matrix. Use ``None`` for no migration.
+        :param migration_rates: Migration matrix. Use ```None``` for no migration.
             A dictionary of the form ``{(pop_i, pop_j): {time1: rate1, time2: rate2}}`` where ``m_ij`` is the
-            migration rate from population ``pop_i`` to population ``pop_j`` at time ``time1`` and ``time2`` etc.
+            migration rate from population ``pop_i`` to population ``pop_j`` at time ``time1`` and `time2` etc.
             Alternatively, a dictionary of 2-dimensional numpy arrays where the rows correspond to the source
             population and the columns to the destination. Note that migration rates for which the source and
             destination population are the same are ignored and that the first time must always be 0.
         :param n_loci: Number of loci.
         :param recombination_rate: Recombination rate.
         :param num_replicates: Number of replicates to use.
         :param record_migration: Whether to record migrations.
@@ -71,16 +71,14 @@
         :param parallelize: Whether to parallelize the msprime simulations.
         :param alpha: Initial distribution of the phase-type coalescent.
         :param comparisons: Dictionary specifying which comparisons to make.
         :param model: Coalescent model to use.
         :param alpha: Alpha parameter of the beta coalescent.
         :param psi: Psi parameter of the Dirac coalescent.
         :param c: C parameter of the Dirac coalescent.
-        :param max_epochs: Maximum number of epochs.
-        :param precision: Precision of the phase-type coalescent.
         """
         if migration_rates is None:
             migration_rates = {}
 
         self.logger = logging.getLogger('phasegen').getChild(self.__class__.__name__)
 
         self.comparisons = comparisons
@@ -154,29 +152,29 @@
             return DiracCoalescent(psi=self.psi, c=self.c)
 
         raise ValueError(f"Unknown coalescent model {name}.")
 
     @cached_property
     def ph(self):
         """
-        Get the phase-type coalescent.
+        PhaseGen coalescent.
         """
         return Coalescent(
             n=self.n,
             demography=self.get_demography(),
             loci=self.get_locus_config(),
             parallelize=self.parallelize,
             end_time=self.end_time,
             model=self.model
         )
 
     @cached_property
     def ms(self):
         """
-        Get the msprime coalescent.
+        Msprime coalescent.
         """
         return MsprimeCoalescent(
             n=self.n,
             demography=self.get_demography(),
             loci=self.get_locus_config(),
             num_replicates=self.num_replicates,
             record_migration=self.record_migration,
```

### Comparing `phasegen-0.0.5b0/phasegen/demography.py` & `phasegen-0.0.6b0/phasegen/demography.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,15 +432,15 @@
             migration_rates: Dict[Tuple[str, str], float] = None
     ):
         """
         Initialize the epoch.
 
         :param start_time: Start time of the epoch.
         :param end_time: End time of the epoch.
-        :param pop_sizes: Population sizes. By default, we have ``{'pop_0': 1}``.
+        :param pop_sizes: Population sizes. By default, we have ``{'pop_0': 1}`.
         :param migration_rates: Migration rates. By default, we have zero migration rates between all populations.
         """
         if pop_sizes is None:
             pop_sizes = {'pop_0': 1}
 
         if migration_rates is None:
             migration_rates = {}
@@ -593,20 +593,20 @@
             self,
             pop_sizes: Dict[str, Dict[float, float]] = None,
             migration_rates: Dict[Tuple[str, str], Dict[float, float]] = None
     ):
         """
         Initialize the population size change.
 
-        :param pop_sizes: Population sizes. Either a dictionary of the form ``{pop_i: {time1: size1, time2: size2}}``,
-            indexed by population name, or a list of dictionaries of the form ``{time1: size1, time2: size2}`` ordered
-            by population index, or a single dictionary of the form ``{time1: size1, time2: size2}`` for a single
+        :param pop_sizes: Population sizes. Either a dictionary of the form `{pop_i: {time1: size1, time2: size2}}`,
+            indexed by population name, or a list of dictionaries of the form `{time1: size1, time2: size2}` ordered
+            by population index, or a single dictionary of the form `{time1: size1, time2: size2}` for a single
             population.
-        :param migration_rates: Migration rates. A dictionary of the form ``{(pop_i, pop_j): {time1: rate1, time2:
-            rate2}}`` of migration from population ``pop_i`` to population ``pop_j`` at time ``time1`` etc.
+        :param migration_rates: Migration rates. A dictionary of the form `{(pop_i, pop_j): {time1: rate1, time2:
+            rate2}}` of migration from population `pop_i` to population `pop_j` at time `time1` etc.
         """
         if pop_sizes is None:
             pop_sizes = {}
 
         if migration_rates is None:
             migration_rates = {}
 
@@ -681,15 +681,15 @@
     Demographic event for changes in population size.
     """
 
     def __init__(self, pop_sizes: Dict[str, Dict[float, float]]):
         """
         Initialize the population size change.
 
-        :param pop_sizes: Population sizes. A dictionary of the form ``{pop_i: {time1: size1, time2: size2}}``.
+        :param pop_sizes: Population sizes. A dictionary of the form `{pop_i: {time1: size1, time2: size2}}`.
         """
         super().__init__(pop_sizes=pop_sizes)
 
 
 class PopSizeChange(PopSizeChanges):
     """
     Demographic event for a single change in population size.
@@ -712,16 +712,16 @@
     """
 
     def __init__(self, rates: Dict[Tuple[str, str], Dict[float, float]]):
         """
         Initialize the (backwards-time) migration rate change.
 
         :param rates: Migration rates. A dictionary of the form
-            ``{(pop_i, pop_j): {time1: rate1, time2: rate2}}`` of migration from population ``pop_i`` to population
-            ``pop_j`` at time ``time1`` etc.
+            `{(pop_i, pop_j): {time1: rate1, time2: rate2}}` of migration from population `pop_i` to population
+            `pop_j` at time `time1` etc.
         """
         super().__init__(migration_rates=rates)
 
 
 class MigrationRateChange(MigrationRateChanges):
     """
     Demographic event for a single change in migration rate.
@@ -745,16 +745,16 @@
     """
 
     def __init__(self, pops: Iterable[str], rate: Dict[float, float] | float):
         """
         Initialize the (backwards-time) migration rate change.
 
         :param pops: Population names across which the migration rates change uniformly.
-        :param rate: Migration rates. A dictionary of the form ``{time1: rate1, time2: rate2}`` of migration
-            from population ``pop_i`` to population ``pop_j`` at time ``time1`` etc. or alternatively a single float
+        :param rate: Migration rates. A dictionary of the form `{time1: rate1, time2: rate2}` of migration
+            from population `pop_i` to population `pop_j` at time `time1` etc. or alternatively a single float
             if the migration rate is constant over time.
         """
         if isinstance(rate, (float, int)):
             rate = {0: rate}
 
         rate = {(p, q): rate for p in pops for q in pops if p != q}
```

### Comparing `phasegen-0.0.5b0/phasegen/distributions.py` & `phasegen-0.0.6b0/phasegen/distributions.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,30 +8,27 @@
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from functools import cached_property, cache
 from math import factorial
 from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator
 
 import numpy as np
-from numpy.polynomial.hermite_e import HermiteE
-from scipy import special
 from scipy.ndimage import gaussian_filter1d
-from scipy.stats import norm
 
 from .coalescent_models import StandardCoalescent, CoalescentModel, BetaCoalescent, DiracCoalescent
 from .demography import Demography, PopSizeChanges
+from .expm import Backend
 from .lineage import LineageConfig
 from .locus import LocusConfig
 from .rewards import Reward, TreeHeightReward, TotalBranchLengthReward, UnfoldedSFSReward, DemeReward, UnitReward, \
     LocusReward, CombinedReward, FoldedSFSReward, SFSReward
 from .serialization import Serializable
 from .spectrum import SFS, SFS2
 from .state_space import BlockCountingStateSpace, DefaultStateSpace, StateSpace
 from .utils import parallelize
-from .expm import Backend
 
 expm = Backend.expm
 
 logger = logging.getLogger('phasegen')
 
 
 class ProbabilityDistribution(ABC):
@@ -61,65 +58,53 @@
     Abstract base class for probability distributions for which moments can be calculated.
     """
 
     @abstractmethod
     @cached_property
     def mean(self) -> float:
         """
-        Get the mean absorption time.
-
-        :return: The mean absorption time.
+        First moment / mean.
         """
         pass
 
     @abstractmethod
     @cached_property
     def var(self) -> float:
         """
-        Get the variance in the absorption time.
-
-        :return: The variance in the absorption time.
+        Second central moment / variance.
         """
         pass
 
     @abstractmethod
     @cached_property
     def m2(self) -> float:
         """
-        Get the second (non-central) moment of the absorption time.
-
-        :return: The variance in the absorption time.
+        Second (non-central) moment.
         """
         pass
 
 
 class MarginalDistributions(Mapping, ABC):
     """
     Base class for marginal distributions.
-
-    TODO remove marginal properties from sub-distributions
     """
 
     @abstractmethod
     @cached_property
     def cov(self) -> np.ndarray:
         """
-        Get the covariance matrix.
-
-        :return: covariance matrix
+        Covariance matrix.
         """
         pass
 
     @abstractmethod
     @cached_property
     def corr(self) -> np.ndarray:
         """
-        Get the correlation matrix.
-
-        :return: correlation matrix
+        Correlation matrix.
         """
         pass
 
     @abstractmethod
     def get_cov(self, d1, d2) -> float:
         """
         Get the covariance between two marginal distributions.
@@ -179,17 +164,15 @@
         :return: Number of distributions.
         """
         return len(self.loci)
 
     @cached_property
     def loci(self) -> Dict[int, 'PhaseTypeDistribution']:
         """
-        Get the distribution for each locus.
-
-        :return: List of distributions.
+        Distributions marginalized over loci.
         """
         # get class of distribution but use PhaseTypeDistribution
         # if this is a TreeHeightDistribution as TreeHeightDistribution
         # only works with default rewards
         cls = self.dist.__class__ if not isinstance(self.dist, TreeHeightDistribution) else PhaseTypeDistribution
 
         loci = {}
@@ -220,17 +203,15 @@
         ))
 
         return xy - self.loci[locus1].mean * self.loci[locus2].mean
 
     @cached_property
     def cov(self) -> np.ndarray:
         """
-        The covariance matrix for the loci under the distribution in question.
-
-        :return: covariance matrix
+        Covariance matrix across loci.
         """
         n_loci = self.dist.locus_config.n
 
         return np.array([[self.get_cov(i, j) for i in range(n_loci)] for j in range(n_loci)])
 
     def get_corr(self, locus1: int, locus2: int) -> float:
         """
@@ -241,17 +222,15 @@
         :return: The correlation coefficient.
         """
         return self.get_cov(locus1, locus2) / (self.loci[locus1].std * self.loci[locus2].std)
 
     @cached_property
     def corr(self) -> np.ndarray:
         """
-        The correlation matrix for the loci under the distribution in question.
-
-        :return: correlation matrix
+        Correlation matrix across loci.
         """
         n_loci = self.dist.locus_config.n
 
         return np.array([[self.get_corr(i, j) for i in range(n_loci)] for j in range(n_loci)])
 
 
 class MarginalDemeDistributions(MarginalDistributions):
@@ -291,25 +270,23 @@
         :return: Number of distributions.
         """
         return len(self.demes)
 
     @cached_property
     def demes(self) -> Dict[str, 'PhaseTypeDistribution']:
         """
-        Get the distribution for each deme.
-
-        :return: List of distributions.
+        Distributions marginalized over demes.
         """
         # get class of distribution but use PhaseTypeDistribution
         # if this is a TreeHeightDistribution as TreeHeightDistribution
         # only works with default rewards
         cls = self.dist.__class__ if not isinstance(self.dist, TreeHeightDistribution) else PhaseTypeDistribution
 
         demes = {}
-        for pop in self.dist.pop_config.pop_names:
+        for pop in self.dist.lineage_config.pop_names:
             demes[pop] = cls(
                 state_space=self.dist.state_space,
                 tree_height=self.dist.tree_height,
                 demography=self.dist.demography,
                 reward=CombinedReward([self.dist.reward, DemeReward(pop)])
             )
 
@@ -319,32 +296,30 @@
         """
         Get the covariance between two demes.
 
         :param pop1: The first deme.
         :param pop2: The second deme.
         :return: The covariance.
         """
-        if pop1 not in self.dist.pop_config.pop_names or pop2 not in self.dist.pop_config.pop_names:
+        if pop1 not in self.dist.lineage_config.pop_names or pop2 not in self.dist.lineage_config.pop_names:
             raise ValueError(f"Population {pop1} or {pop2} does not exist.")
 
         xy = self.dist.moment(k=2, rewards=(
             CombinedReward([self.dist.reward, DemeReward(pop1)]),
             CombinedReward([self.dist.reward, DemeReward(pop2)])
         ))
 
         return xy - self.demes[pop1].mean * self.demes[pop2].mean
 
     @cached_property
     def cov(self) -> np.ndarray:
         """
-        The covariance matrix for the demes under the distribution in question.
-
-        :return: covariance matrix
+        Covariance matrix across demes.
         """
-        pops = self.dist.pop_config.pop_names
+        pops = self.dist.lineage_config.pop_names
 
         return np.array([[self.get_cov(p1, p2) for p1 in pops] for p2 in pops])
 
     def get_corr(self, pop1: str, pop2: str) -> float:
         """
         Get the correlation coefficient between two demes.
 
@@ -353,19 +328,17 @@
         :return: The correlation coefficient.
         """
         return self.get_cov(pop1, pop2) / (self.demes[pop1].std * self.demes[pop2].std)
 
     @cached_property
     def corr(self) -> np.ndarray:
         """
-        The correlation matrix for the demes under the distribution in question.
-
-        :return: correlation matrix
+        Correlation matrix across demes.
         """
-        pops = self.dist.pop_config.pop_names
+        pops = self.dist.lineage_config.pop_names
 
         return np.array([[self.get_corr(p1, p2) for p1 in pops] for p2 in pops])
 
 
 class DensityAwareDistribution(MomentAwareDistribution, ABC):
     """
     Abstract base class for probability distributions for which moments and densities can be calculated.
@@ -480,16 +453,14 @@
         )
 
 
 class PhaseTypeDistribution(MomentAwareDistribution):
     """
     Phase-type distribution for a piecewise time-homogeneous process.
     """
-    #: Number of decimals to round moments to.
-    n_decimals: int = 12
 
     def __init__(
             self,
             state_space: StateSpace,
             tree_height: 'TreeHeightDistribution',
             demography: Demography = None,
             reward: Reward = None
@@ -507,30 +478,30 @@
 
         if reward is None:
             reward = TreeHeightReward()
 
         super().__init__()
 
         #: Population configuration
-        self.pop_config: LineageConfig = state_space.pop_config
+        self.lineage_config: LineageConfig = state_space.lineage_config
 
         #: Locus configuration
         self.locus_config: LocusConfig = state_space.locus_config
 
         #: Reward
         self.reward: Reward = reward
 
         #: State space
         self.state_space: StateSpace = state_space
 
         #: Demography
         self.demography: Demography = demography
 
         #: Tree height distribution
-        self.tree_height = tree_height
+        self.tree_height: TreeHeightDistribution = tree_height
 
     @staticmethod
     def _get_van_loan_matrix(R: List[np.ndarray], S: np.ndarray, k: int = 1) -> np.ndarray:
         """
         Get the block matrix for the given reward matrices and transition matrix.
 
         :param R: List of length k of reward matrices
@@ -543,149 +514,54 @@
 
         # create compound matrix
         return np.block([[S if i == j else R[i] if i == j - 1 else O for j in range(k + 1)] for i in range(k + 1)])
 
     @cached_property
     def mean(self) -> float | SFS:
         """
-        Get the mean absorption time.
-
-        :return: The mean absorption time.
+        First moment / mean.
         """
         return self.moment(k=1)
 
     @cached_property
     def var(self) -> float | SFS:
         """
-        Get the variance in the absorption time.
-
-        :return: The variance in the absorption time.
+        Second central moment / variance.
         """
         return self.moment(k=2) - self.moment(k=1) ** 2
 
     @cached_property
     def std(self) -> float | SFS:
         """
-        Get the standard deviation in the absorption time.
-
-        :return: The standard deviation in the absorption time.
+        Standard deviation.
         """
         return self.var ** 0.5
 
     @cached_property
     def m2(self) -> float | SFS:
         """
-        Get the (non-central) second moment.
-
-        :return: The second moment.
+        Second (non-central) moment.
         """
         return self.moment(k=2)
 
     @cached_property
     def demes(self) -> MarginalDemeDistributions:
         """
-        Get marginal distributions for each deme.
-
-        :return: Marginal distributions.
+        Marginal distributions over each deme.
         """
         return MarginalDemeDistributions(self)
 
     @cached_property
     def loci(self) -> MarginalLocusDistributions:
         """
-        Get marginal distributions for each locus.
-
-        :return: Marginal distributions.
+        Marginal distributions over each locus.
         """
         return MarginalLocusDistributions(self)
 
     @cache
-    def moment_deprecated(
-            self,
-            k: int,
-            rewards: Tuple[Reward, ...] = None,
-            start_time: float = None,
-            end_time: float = None
-    ) -> float:
-        """
-        Get the kth (non-central) moment.
-
-        TODO remove later
-
-        :param k: The order of the moment.
-        :param rewards: Tuple of k rewards
-        :param start_time: Time when to start accumulation of moments. By default, the start time specified when
-            initializing the distribution.
-        :param end_time: Time when to end accumulation of moments. By default, either the end time specified when
-            initializing the distribution or the time until almost sure absorption.
-        :return: The kth moment
-        """
-        # use default reward if not specified
-        if rewards is None:
-            rewards = (self.reward,) * k
-        else:
-            if len(rewards) != k:
-                raise ValueError(f"Number of rewards must be {k}.")
-
-        if start_time is None:
-            start_time = self.tree_height.start_time
-
-        if end_time is None:
-            end_time = self.tree_height.t_max
-
-        # get reward matrix
-        R = [np.diag(r._get(state_space=self.state_space)) for r in rewards]
-
-        # number of states
-        n_states = self.state_space.k
-
-        # initialize Van Loan matrix holding (rewarded) moments
-        Q = np.eye(n_states * (k + 1))
-
-        # iterate through epochs and compute initial values
-        for i, epoch in enumerate(self.demography.epochs):
-
-            # get state space for this epoch
-            self.state_space.update_epoch(epoch)
-
-            # get Van Loan matrix
-            V = self._get_van_loan_matrix(S=self.state_space.S, R=R, k=k)
-
-            # compute tau
-            tau = min(epoch.end_time, end_time) - epoch.start_time
-
-            # compute matrix exponential
-            Q_curr = expm(V * tau)
-
-            # update by accumulated reward
-            Q = Q @ Q_curr
-
-            # break if we have reached the end time
-            if epoch.end_time >= end_time:
-                break
-
-        # calculate moment
-        m = factorial(k) * self.state_space.alpha @ Q[:n_states, -n_states:] @ self.state_space.e
-
-        # subtract accumulated moment up to start time if greater than 0
-        if start_time > 0:
-            # call on PhaseTypeDistribution to make possible SFS moment calculation
-            m -= PhaseTypeDistribution.moment(
-                self,
-                k=k,
-                rewards=rewards,
-                start_time=0,
-                end_time=self.tree_height.start_time
-            )
-
-        # TODO round to avoid numerical errors?
-        # return np.round(m, self.n_decimals)
-        return m
-
-    @cache
     def moment(
             self,
             k: int,
             rewards: Tuple[Reward, ...] = None,
             start_time: float = None,
             end_time: float = None
     ) -> float:
@@ -735,22 +611,21 @@
 
         # rewards in the Van Loan matrix are of order 1
         return 10 ** - np.log10(rates).mean()
 
     def _check_numerical_stability(self, S: np.ndarray, epoch: int):
         """
         Warn about potential numerical instability with very small or very large rates.
-        TODO this is a good approach but often there are not precision problem so this might confuse the user
 
         :param S: (Regularized) intensity matrix.
         :param epoch: Epoch number.
         """
         rates = S[S > 0]
 
-        if rates.min() / rates.max() < 1e-6:
+        if rates.min() / rates.max() < 1e-10:
             self._logger.warning(
                 f"Intensity matrix in epoch {epoch} contains rates that differ by more than 6 orders of magnitude: "
                 f"min: {rates.min()}, max: {rates.max()}. "
                 f"This may potentially lead to numerical instability, despite matrix regularization."
             )
 
     def accumulate(
@@ -1098,18 +973,16 @@
         x2 = x1 + dx
 
         return (self.cdf(x2) - self.cdf(x1)) / dx
 
     @cached_property
     def t_max(self) -> float:
         """
-        Get the time until which computations are performed. This is either the end time specified when initializing
+        Time until which computations are performed. This is either the end time specified when initializing
         the distribution or the time until almost sure absorption.
-
-        :return: The maximum time.
         """
         if self.end_time is not None:
             return self.end_time
 
         t_abs = self._get_absorption_time()
 
         if t_abs < self.start_time:
@@ -1147,16 +1020,16 @@
             # update state space
             self.state_space.update_epoch(epoch)
 
             if i > self.max_epochs:
                 self._logger.warning(
                     f"Reached maximum number of epochs ({self.max_epochs}) when determining "
                     "time of almost sure absorption. This may be due to an ill-defined demography. "
-                    "You can also increase the maximum number of epochs (`TreeHeightDistribution.max_epochs`) or "
-                    "set the end time manually (`Coalescent.end_time`)."
+                    "You can also increase the maximum number of epochs (TreeHeightDistribution.max_epochs) or "
+                    "set the end time manually (Coalescent.end_time)."
                 )
                 return t
 
             # make sure we are not in last epoch
             if epoch.tau < np.inf:
                 # update transition matrix
                 T_curr = expm(self.state_space.S * epoch.tau) @ T_curr
@@ -1221,15 +1094,15 @@
 
         return t
 
     def _warn_p_is_nan(self, t: float) -> float:
         """
         Warn if the probability of absorption is nan.
 
-        :param p: The probability of absorption.
+        :param t: The absorption time.
         :return: The time.
         """
         self._logger.critical(
             "Could not reliably find time of almost sure absorption "
             "as probability of absorption is NaN. "
             "This is likely due to an ill-conditioned rate matrix. "
             f"Using time {t:.1f}. "
@@ -1325,15 +1198,15 @@
             func=lambda x: self._moment(*x),
             data=[[k, i, rewards, start_time, end_time] for i in self._get_indices()],
             desc=f"Calculating {k}-moments",
             pbar=self.pbar,
             parallelize=self.parallelize
         )
 
-        return SFS([0] + list(moments) + [0] * (self.pop_config.n - len(moments)))
+        return SFS([0] + list(moments) + [0] * (self.lineage_config.n - len(moments)))
 
     def _moment(
             self,
             k: int,
             i: int,
             rewards: Tuple[SFSReward, ...] = None,
             start_time: float = None,
@@ -1386,15 +1259,15 @@
             parallelize=self.parallelize
         )
 
         # pad with zeros
         return np.concatenate([
             np.zeros((1, len(end_times))),
             accumulation,
-            np.zeros((self.pop_config.n - len(indices), len(end_times)))
+            np.zeros((self.lineage_config.n - len(indices), len(end_times)))
         ])
 
     def plot_accumulation(
             self,
             k: int = 1,
             end_times: Iterable[float] = None,
             rewards: Tuple[Reward, ...] = None,
@@ -1482,15 +1355,15 @@
             end_times=end_times,
             rewards=tuple([CombinedReward([r, self._get_sfs_reward(i)]) for r in rewards])
         )
 
     @cached_property
     def cov(self) -> SFS2:
         """
-        The 2-SFS, i.e. the (central) covariance matrix of the site-frequencies.
+        Covariance matrix across site-frequency counts.
         """
         # create list of arguments for each combination of i, j
         indices = [(i, j) for i in self._get_indices() for j in self._get_indices()]
 
         # get sfs using parallelized function
         sfs_results = parallelize(
             func=lambda x: (
@@ -1502,15 +1375,15 @@
             data=indices,
             desc="Calculating covariance",
             pbar=self.pbar,
             parallelize=self.parallelize
         )
 
         # re-structure the results to a matrix form
-        sfs = np.zeros((self.pop_config.n + 1, self.pop_config.n + 1))
+        sfs = np.zeros((self.lineage_config.n + 1, self.lineage_config.n + 1))
         for ((i, j), result) in zip(indices, sfs_results):
             sfs[i, j] = result
 
         # get matrix of marginal moments
         m2 = np.outer(self.mean.data, self.mean.data)
 
         # calculate covariances
@@ -1522,35 +1395,32 @@
         """
         Get the covariance between the ith and jth site-frequency.
 
         :param i: The ith frequency count
         :param j: The jth frequency count
         :return: covariance
         """
-        if i in (0, self.pop_config.n) or j in (0, self.pop_config.n):
+        if i in (0, self.lineage_config.n) or j in (0, self.lineage_config.n):
             return 0
 
         reward_i = CombinedReward([self.reward, self._get_sfs_reward(i)])
         reward_j = CombinedReward([self.reward, self._get_sfs_reward(j)])
 
         xy = super().moment(k=2, rewards=(reward_i, reward_j))
         yx = super().moment(k=2, rewards=(reward_j, reward_i))
 
         x = super().moment(k=1, rewards=(reward_i,))
         y = super().moment(k=1, rewards=(reward_j,))
 
-        # TODO check why covariance is not symmetric
         return (xy + yx) / 2 - x * y
 
     @cached_property
     def corr(self) -> SFS2:
         """
-        The correlation coefficient matrix of the site-frequencies.
-
-        :return: The correlation coefficient matrix
+        Correlation matrix across site-frequency counts.
         """
         # get standard deviations
         std = np.sqrt(self.var.data)
 
         sfs = SFS2(self.cov.data / np.outer(std, std))
 
         # replace NaNs with zeros
@@ -1562,15 +1432,15 @@
         """
         Get the correlation coefficient between the ith and jth site-frequency.
 
         :param i: The ith frequency count
         :param j: The jth frequency count
         :return: Correlation coefficient
         """
-        if i in (0, self.pop_config.n) or j in (0, self.pop_config.n):
+        if i in (0, self.lineage_config.n) or j in (0, self.lineage_config.n):
             return 0
 
         return self.get_cov(i, j) / (np.sqrt(self.get_cov(i, i)) * np.sqrt(self.get_cov(j, j)))
 
 
 class UnfoldedSFSDistribution(SFSDistribution):
     """
@@ -1588,15 +1458,15 @@
 
     def _get_indices(self) -> np.ndarray:
         """
         Get the indices for the site-frequency spectrum.
 
         :return: The indices.
         """
-        return np.arange(1, self.pop_config.n)
+        return np.arange(1, self.lineage_config.n)
 
 
 class FoldedSFSDistribution(SFSDistribution):
     """
     Folded site-frequency spectrum distribution.
     """
 
@@ -1611,15 +1481,15 @@
 
     def _get_indices(self) -> np.ndarray:
         """
         Get the indices for the site-frequency spectrum.
 
         :return: The indices.
         """
-        return np.arange(1, self.pop_config.n // 2 + 1)
+        return np.arange(1, self.lineage_config.n // 2 + 1)
 
 
 class EmpiricalDistribution(DensityAwareDistribution):
     """
     Probability distribution based on realisations.
     """
 
@@ -1654,71 +1524,57 @@
         Drop all cached properties.
         """
         self.samples = None
 
     @cached_property
     def mean(self) -> float | np.ndarray:
         """
-        Get the mean absorption time.
-
-        :return: Mean absorption time.
+        First moment / mean.
         """
         return np.mean(self.samples, axis=0)
 
     @cached_property
     def var(self) -> float | np.ndarray:
         """
-        Get the variance in the absorption time.
-
-        :return: Variance in the absorption time.
+        Second central moment / variance.
         """
         return np.var(self.samples, axis=0)
 
     @cached_property
     def m2(self) -> float | np.ndarray:
         """
-        Get the second moment.
-
-        :return: Second moment.
+        Second non-central moment.
         """
         return np.mean(self.samples ** 2, axis=0)
 
     @cached_property
     def m3(self) -> float | np.ndarray:
         """
-        Get the third moment.
-
-        :return: Third moment.
+        Third non-central moment.
         """
         return np.mean(self.samples ** 3, axis=0)
 
     @cached_property
     def m4(self) -> float | np.ndarray:
         """
-        Get the fourth moment.
-
-        :return: Fourth moment.
+        Fourth non-central moment.
         """
         return np.mean(self.samples ** 4, axis=0)
 
     @cached_property
     def cov(self) -> float | np.ndarray:
         """
-        Get the covariance matrix.
-
-        :return: Second moment.
+        Covariance matrix.
         """
         return np.nan_to_num(np.cov(self.samples, rowvar=False))
 
     @cached_property
     def corr(self) -> float | np.ndarray:
         """
-        Get the correlation matrix.
-
-        :return: Second moment.
+        Correlation matrix.
         """
         return np.nan_to_num(np.corrcoef(self.samples, rowvar=False))
 
     def moment(self, k: int) -> float | np.ndarray:
         """
         Get the kth moment.
 
@@ -1802,53 +1658,43 @@
         :param samples: 2-D array of samples.
         """
         super().__init__(samples)
 
     @cached_property
     def mean(self) -> SFS:
         """
-        Get the mean absorption time.
-
-        :return: Mean absorption time.
+        First moment / mean.
         """
         return SFS(super().mean)
 
     @cached_property
     def var(self) -> SFS:
         """
-        Get the variance in the absorption time.
-
-        :return: Variance in the absorption time.
+        Second central moment / variance.
         """
         return SFS(super().var)
 
     @cached_property
     def m2(self) -> SFS:
         """
-        Get the second moment.
-
-        :return: Second moment.
+        Second non-central moment.
         """
         return SFS(super().m2)
 
     @cached_property
     def cov(self) -> SFS2:
         """
-        Get the covariance matrix.
-
-        :return: Second moment.
+        Covariance matrix.
         """
         return SFS2(np.nan_to_num(np.cov(self.samples, rowvar=False)))
 
     @cached_property
     def corr(self) -> SFS2:
         """
-        Get the correlation matrix.
-
-        :return: Second moment.
+        Correlation matrix.
         """
         return SFS2(np.nan_to_num(np.corrcoef(self.samples, rowvar=False)))
 
 
 class DictContainer(dict):
     """
     Dictionary container.
@@ -2033,15 +1879,15 @@
             end_time: float = None
     ):
         """
         Create object.
 
         :param n: n: Number of lineages. Either a single integer if only one population, or a list of integers
             or a dictionary with population names as keys and number of lineages as values. Alternatively, a
-            :class:`PopulationConfig` object can be passed.
+            :class:`LineageConfig` object can be passed.
         :param model: Coalescent model. By default, the standard coalescent is used.
         :param loci: Number of loci or locus configuration.
         :param recombination_rate: Recombination rate.
         :param demography: Demography.
         :param end_time: Time when to end the computation. If ``None``, the end time is end time is taken to be the
             time of almost sure absorption. Note that unnecessarily large end times can lead to numerical errors.
         """
@@ -2051,18 +1897,18 @@
             model = StandardCoalescent()
 
         if demography is None:
             demography = Demography()
 
         if not isinstance(n, LineageConfig):
             #: Population configuration
-            self.pop_config: LineageConfig = LineageConfig(n)
+            self.lineage_config: LineageConfig = LineageConfig(n)
         else:
             #: Population configuration
-            self.pop_config: LineageConfig = n
+            self.lineage_config: LineageConfig = n
 
         # set up locus configuration
         if isinstance(loci, int):
             #: Locus configuration
             self.locus_config: LocusConfig = LocusConfig(
                 n=loci,
                 recombination_rate=recombination_rate if recombination_rate is not None else 0
@@ -2071,25 +1917,25 @@
             #: Locus configuration
             self.locus_config: LocusConfig = loci
 
             if recombination_rate is not None:
                 self.locus_config.recombination_rate = recombination_rate
 
         # population names present in the population configuration but not in the demography
-        initial_sizes = {p: {0: 1} for p in self.pop_config.pop_names if p not in demography.pop_names}
+        initial_sizes = {p: {0: 1} for p in self.lineage_config.pop_names if p not in demography.pop_names}
 
         # add missing population sizes to demography
         if len(initial_sizes) > 0:
             demography.add_event(
                 PopSizeChanges(initial_sizes)
             )
 
         # add zero lineage counts to lineage configuration for populations only present in the demography
-        unspecified_lineages = set(demography.pop_names) - set(self.pop_config.pop_names)
-        self.pop_config = LineageConfig(self.pop_config.lineage_dict | {p: 0 for p in unspecified_lineages})
+        unspecified_lineages = set(demography.pop_names) - set(self.lineage_config.pop_names)
+        self.lineage_config = LineageConfig(self.lineage_config.lineage_dict | {p: 0 for p in unspecified_lineages})
 
         #: Coalescent model
         self.model: CoalescentModel = model
 
         #: Demography
         self.demography: Demography = demography
 
@@ -2139,15 +1985,15 @@
             end_time: float = None
     ):
         """
         Create object.
 
         :param :param n: n: Number of lineages. Either a single integer if only one population, or a list of integers
             or a dictionary with population names as keys and number of lineages as values. Alternatively, a
-            :class:`PopulationConfig` object can be passed.
+            :class:`LineageConfig` object can be passed.
         :param model: Coalescent model. Default is the standard coalescent.
         :param demography: Demography.
         :param loci: Number of loci or locus configuration.
         :param recombination_rate: Recombination rate.
         :param pbar: Whether to show a progress bar.
         :param parallelize: Whether to parallelize computations.
         :param start_time: Time when to start accumulating moments. By default, this is 0.
@@ -2174,27 +2020,27 @@
 
     @cached_property
     def default_state_space(self) -> DefaultStateSpace:
         """
         The default state space.
         """
         return DefaultStateSpace(
-            pop_config=self.pop_config,
+            lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
             epoch=self.demography.get_epochs(0)
         )
 
     @cached_property
     def block_counting_state_space(self) -> BlockCountingStateSpace:
         """
         The block counting state space.
         """
         return BlockCountingStateSpace(
-            pop_config=self.pop_config,
+            lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
             epoch=self.demography.get_epochs(0)
         )
 
     @cached_property
     def tree_height(self) -> TreeHeightDistribution:
@@ -2337,15 +2183,15 @@
         :param record_migration: Whether to record migrations which is necessary to calculate statistics per deme.
         :return: msprime coalescent.
         """
         if self.start_time != 0:
             self._logger.warning("Non-zero start times are not supported by MsprimeCoalescent.")
 
         return MsprimeCoalescent(
-            n=self.pop_config,
+            n=self.lineage_config,
             demography=self.demography,
             model=self.model,
             loci=self.locus_config,
             recombination_rate=self.locus_config.recombination_rate,
             end_time=self.end_time,
             num_replicates=num_replicates,
             n_threads=n_threads,
@@ -2425,20 +2271,20 @@
     @cache
     def simulate(self):
         """
         Simulate data using msprime.
         """
         # number of replicates for one thread
         num_replicates = self.num_replicates // self.n_threads
-        samples = self.pop_config.lineage_dict
+        samples = self.lineage_config.lineage_dict
         demography = self.demography.to_msprime()
         model = self.get_coalescent_model()
         end_time = self.end_time
         n_pops = self.demography.n_pops
-        sample_size = self.pop_config.n
+        sample_size = self.lineage_config.n
 
         def simulate_batch(_) -> (np.ndarray, np.ndarray, np.ndarray):
             """
             Simulate statistics.
 
             :param _:
             :return: Statistics.
@@ -2648,15 +2494,15 @@
     @cached_property
     def fsfs(self) -> EmpiricalPhaseTypeSFSDistribution:
         """
         Folded site frequency spectrum distribution.
         """
         self.simulate()
 
-        mid = (self.pop_config.n + 1) // 2
+        mid = (self.lineage_config.n + 1) // 2
 
         counts = self.sfs_counts.copy().T
 
         counts[:mid] += counts[-mid:][::-1]
         counts[-mid:] = 0
 
         return EmpiricalPhaseTypeSFSDistribution(counts.T, pops=self.demography.pop_names)
@@ -2664,265 +2510,14 @@
     def to_phasegen(self) -> Coalescent:
         """
         Convert to native phasegen coalescent.
 
         :return: phasegen coalescent.
         """
         return Coalescent(
-            n=self.pop_config,
+            n=self.lineage_config,
             model=self.model,
             demography=self.demography,
             loci=self.locus_config,
             recombination_rate=self.locus_config.recombination_rate,
             end_time=self.end_time
         )
-
-
-class _GramCharlierExpansion:
-    """
-    Probability density function approximated from its moments using Hermite polynomials.
-
-    .. note::
-        Does not work reliably at all. We get negative values for the density function which seems to be a problem
-        with the method in general. Trying some other statsmodels implementation provides similarly cumbersome results.
-    """
-
-    @classmethod
-    def pdf(cls, x: np.ndarray, moments: np.ndarray[float], mu: float = 0, sigma: float = 1) -> np.ndarray:
-        """
-        Approximate the distribution using its moments and Hermite polynomials.
-
-        :param x: Array of standard normal values.
-        :param moments: List of moments of the distribution.
-        :param mu: Mean of the normal distribution.
-        :param sigma: Standard deviation of the normal distribution.
-        :return: Approximated probability density function values.
-        """
-        y = np.ones_like(x)
-
-        # d = [cls.d(n, moments, mu, sigma) for n in range(0, len(moments) + 1)]
-
-        for n in range(3, len(moments) + 1):
-            y += cls.d(n, moments, mu, sigma) * cls.H(n, (x - mu) / sigma)
-
-        return norm.pdf(x, loc=mu, scale=sigma) * y
-
-    @classmethod
-    def H(cls, n: int, x: np.ndarray[float]) -> np.ndarray[float]:
-        """
-        Probabilist's Hermite polynomial of order n.
-
-        :param n: Order of the polynomial.
-        :param x: Values to evaluate the polynomial at.
-        :return: Hermite polynomial of order n evaluated at x.
-        """
-        y = np.zeros_like(x)
-
-        for j in range(int(n / 2) + 1):
-            y += (((-1) ** j * factorial(n) * x ** (n - 2 * j) / (2 ** j * factorial(n - 2 * j) * factorial(j)))
-                  .astype(float))
-
-        return y
-
-    @classmethod
-    def d(cls, n: int, moments: np.ndarray[float], mu: float, sigma: float) -> float:
-        """
-        Coefficient of the Hermite series.
-
-        :param n: Order of the coefficient.
-        :param moments: Moments of the distribution.
-        :param mu: Mean of the distribution.
-        :param sigma: Standard deviation of the distribution.
-        :return: Coefficients of the Hermite polynomial of order n.
-        """
-        y = np.zeros(int(n / 2) + 1)
-
-        for j in range(len(y)):
-            y[j] = (-1) ** j / 2 ** j / factorial(j) * cls.E(n - 2 * j, moments, mu, sigma)
-
-        return y.sum()
-
-    @classmethod
-    def E(cls, n: int, moments: np.ndarray[float], mu: float, sigma: float) -> float:
-        """
-        Expectation of the nth standard normal moment.
-
-        :param n: Order of the polynomial.
-        :param moments: Moments of the distribution.
-        :param mu: Mean of the distribution.
-        :param sigma: Standard deviation of the distribution.
-        :return: Expectation of the Hermite polynomial of order n.
-        """
-        # add zeroth moment
-        all_moments = np.concatenate((np.array([1]), moments))
-
-        # return all_moments[n] / factorial(n)
-
-        y = np.zeros(n + 1)
-
-        for k in range(len(y)):
-            y[k] = (-1) ** k * mu ** (n - k) * all_moments[k] / factorial(n - k) / factorial(k)
-
-        return y.sum() / sigma ** n
-
-
-class _EdgeworthExpansion:
-    """
-    Probability density function approximated from its moments using Edgeworth expansion.
-
-    Adapted from statsmodels.distributions.edgeworth.
-
-    .. note::
-        Only works well for values for which the normal distribution is not close to zero, so it is unsuitable for
-        approximating long-tailed distributions.
-    """
-
-    @staticmethod
-    def _norm_pdf(x: np.ndarray | float) -> np.ndarray | float:
-        """
-        Standard normal probability density function.
-
-        :param x: Value or values to evaluate the PDF at.
-        :return: PDF.
-        """
-        return np.exp(-x ** 2 / 2.0) / np.sqrt(2 * np.pi)
-
-    @staticmethod
-    def _norm_cdf(x: np.ndarray | float) -> np.ndarray | float:
-        """
-        Standard normal cumulative distribution function.
-
-        :param x: Value or values to evaluate the CDF at.
-        :return: CDF.
-        """
-        return special.ndtr(x)
-
-    def __init__(self, cum: List[float]):
-        """
-        Initialize object.
-
-        :param cum: Cumulants.
-        """
-
-        self._logger = logger.getChild(self.__class__.__name__)
-
-        self._coef, self._mu, self._sigma = self._compute_coefficients(cum)
-
-        self._herm_pdf = HermiteE(self._coef)
-
-        if self._coef.size > 2:
-            self._herm_cdf = HermiteE(-self._coef[1:])
-        else:
-            self._herm_cdf = lambda x: 0
-
-        # warn if pdf(x) < 0 for some values of x within 4 sigma
-        r = np.real_if_close(self._herm_pdf.roots())
-        r = (r - self._mu) / self._sigma
-
-        if r[(np.imag(r) == 0) & (np.abs(r) < 4)].any():
-            self._logger.warning(f'PDF has zeros at {r}')
-
-    def _pdf(self, x: np.ndarray | float) -> np.ndarray | float:
-        """
-        Probability density function.
-
-        :param x: Value or values to evaluate the PDF at.
-        :return: PDF.
-        """
-        y = (x - self._mu) / self._sigma
-
-        return self._herm_pdf(y) * self._norm_pdf(y) / self._sigma
-
-    def _cdf(self, x: np.ndarray | float) -> np.ndarray | float:
-        """
-        Cumulative distribution function.
-
-        :param x: Value or values to evaluate the CDF at.
-        :return: CDF.
-        """
-        y = (x - self._mu) / self._sigma
-
-        return self._norm_cdf(y) + self._herm_cdf(y) * self._norm_pdf(y)
-
-    def _compute_coefficients(self, cum: List[float]) -> (np.ndarray, float, float):
-        """
-        Compute coefficients of the Edgeworth expansion for the PDF.
-
-        :param cum: Cumulants.
-        :return: Coefficients, mean and standard deviation.
-        """
-        # scale cumulants by \sigma
-        mu, sigma = cum[0], np.sqrt(cum[1])
-        lam = np.asarray(cum)
-        for j, l in enumerate(lam):
-            lam[j] /= cum[1] ** j
-
-        coef = np.zeros(lam.size * 3 - 5)
-        coef[0] = 1
-
-        for s in range(lam.size - 2):
-            for p in self._generate_partitions(s + 1):
-                term = sigma ** (s + 1)
-
-                for (m, k) in p:
-                    term *= np.power(lam[m + 1] / factorial(m + 2), k) / factorial(k)
-
-                r = sum(k for (m, k) in p)
-                coef[s + 1 + 2 * r] += term
-
-        return coef, mu, sigma
-
-    @classmethod
-    def cumulant_from_moments(cls, moments: List[float], n: int) -> float:
-        """
-        Compute n-th cumulant from moments.
-
-        :param moments: The moments, raw or central
-        :param n: The order of the cumulant to compute
-        :return: The cumulant
-        """
-        kappa = 0
-
-        for p in cls._generate_partitions(n):
-            r = sum(k for (m, k) in p)
-            term = (-1) ** (r - 1) * factorial(r - 1)
-
-            for (m, k) in p:
-                term *= np.power(moments[m - 1] / factorial(m), k) / factorial(k)
-
-            kappa += term
-
-        kappa *= factorial(n)
-
-        return kappa
-
-    @classmethod
-    def cumulants_from_moments(cls, moments: List[float]) -> List[float]:
-        """
-        Compute cumulants from moments.
-
-        The mnc2cum implementation which provides more accurate results
-
-        :param moments: The moments, raw or central
-        :return: The cumulants
-        """
-        return [cls.cumulant_from_moments(moments, k) for k in range(1, len(moments) + 1)]
-
-    @classmethod
-    def _generate_partitions(cls, n: int):
-        """
-        Generate partitions of an integer.
-
-        :param n: Integer to partition.
-        :return: Partitions formatted as a list of tuples where the first element is the partition and the second
-            element is the number of times the partition is repeated.
-        """
-        x = BlockCountingStateSpace._find_sample_configs(n, n)
-
-        for v in x:
-
-            m = []
-            for i in range(0, n):
-                if v[i] > 0:
-                    m.append((i + 1, v[i]))
-
-            yield m
```

### Comparing `phasegen-0.0.5b0/phasegen/expm.py` & `phasegen-0.0.6b0/phasegen/expm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Matrix exponential computation.
 """
 from abc import ABC, abstractmethod
+from typing import Type
 
 import numpy as np
 import scipy
 
 
 class MatrixExponentiation(ABC):
     """
     Base class for matrix exponentiation.
+
+    :meta private:
     """
 
     @staticmethod
     @abstractmethod
     def compute(m: np.ndarray) -> np.ndarray:
         """
         Compute the matrix exponential.
@@ -53,26 +56,26 @@
         :return: Matrix exponential
         """
         return scipy.linalg.expm(m)
 
 
 class Backend(ABC):
     """
-    Backend for matrix exponentiation.
+    Configure the backend for matrix exponentiation.
     """
     #: Backend for matrix exponentiation
-    backend: MatrixExponentiation = SciPyExpm
+    backend: Type[MatrixExponentiation] = SciPyExpm
 
     @classmethod
     @abstractmethod
     def expm(cls, m: np.ndarray) -> np.ndarray:
         """
         Compute the matrix exponential.
         """
         return cls.backend.compute(m)
 
     @classmethod
-    def register(cls, backend: MatrixExponentiation):
+    def register(cls, backend: Type[MatrixExponentiation]):
         """
         Register a backend.
         """
         cls.backend = backend
```

### Comparing `phasegen-0.0.5b0/phasegen/inference.py` & `phasegen-0.0.6b0/phasegen/inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,16 +168,14 @@
         if not all([self.bounds[key][0] <= value <= self.bounds[key][1] for key, value in self.x0.items()]):
             raise ValueError('Initial parameters must be within the specified bounds.')
 
     @cached_property
     def x0(self) -> Dict[str, float]:
         """
         Initial parameters.
-
-        :return: Initial parameters.
         """
         return self._x0 if self._x0 is not None else self._sample()
 
     def __getstate__(self) -> dict:
         """
         Get the state of the object for serialization.
 
@@ -205,15 +203,15 @@
 
     def get_coal(self, **kwargs) -> Coalescent:
         """
         Get the (possibly cached) coalescent distribution.
 
         TODO test state space caching by comparing cached und uncached results.
 
-        :param kwargs: Keyword arguments passed to the callback specified as ``dist``.
+        :param kwargs: Keyword arguments passed to the callback specified as ``dist`.
         :return: Coalescent distribution.
         """
         coal = self.coal(**kwargs)
 
         # disable parallelization to avoid problematic double parallelization
         coal.parallelize = False
 
@@ -227,26 +225,22 @@
                 coal.__dict__['block_counting_state_space'] = self.block_counting_state_space
 
         return coal
 
     @cached_property
     def default_state_space(self) -> DefaultStateSpace:
         """
-        Default state space.
-
-        :return: Default state space.
+        Default state space which only keeps track of the number of lineages present.
         """
         return self.coal(**self.x0).default_state_space
 
     @cached_property
     def block_counting_state_space(self) -> BlockCountingStateSpace:
         """
-        Block counting state space.
-
-        :return: Block counting state space.
+        Block counting state space which keeps track for the number of lineages that subtend `i` lineages.
         """
         return self.coal(**self.x0).block_counting_state_space
 
     @staticmethod
     def _get_loss_function(
             observation: Any,
             x0: Dict[str, float],
@@ -697,14 +691,61 @@
             for dist in self.bootstrap_dists:
                 plot(dist.demography, {'color': 'C0', 'alpha': 0.3})
 
         Visualization.show_and_save(show=show, file=file)
 
         return ax
 
+    def create_run(self, x0: Dict[str, float] = None) -> 'Inference':
+        """
+        Create a new Inference object which can be run independently. This is useful when parallelizing runs on a
+        cluster. You can add performed runs by using the `add_run` method.
+
+        :param x0: Initial parameters.
+        :return: Inference object.
+        """
+        other = copy.deepcopy(self)
+
+        other._x0 = x0
+        other._check_x0_within_bounds()
+
+        # generate a new random seed if seeded
+        if other.seed is not None:
+            other.seed = self._rng.integers(0, 2 ** 32 - 1)
+            other._rng = np.random.default_rng(other.seed)
+
+        return other
+
+    def add_run(self, inference: 'Inference'):
+        """
+        Merge the main optimization result from another Inference object into the current Inference object. We only
+        store the result of the run with the lowest loss.
+
+        :param inference: Inference object.
+        :raises RuntimeError: If the main optimization has not been run yet.
+        """
+        if inference.loss_inferred is None:
+            raise RuntimeError('The provided Inference object must be run first (call the `run` method).')
+
+        if self.loss_inferred is None or inference.loss_inferred < self.loss_inferred:
+            self.result = inference.result
+            self.params_inferred = inference.params_inferred
+            self.loss_inferred = inference.loss_inferred
+            self.dist_inferred = inference.dist_inferred
+
+    def add_runs(self, inferences: Iterable['Inference']):
+        """
+        Merge the main optimization results from an iterable of Inference objects with the current Inference object. We
+        only store the result of the run with the lowest loss.
+
+        :param inferences: Iterable of Inference objects.
+        """
+        for inference in inferences:
+            self.add_run(inference)
+
     def create_bootstrap(self, n_runs: int = 1) -> 'Inference':
         """
         Resample the observation and return a new Inference object with the resampled observation.
         This is useful when parallelizing bootstraps on a cluster. You can add performed bootstraps
         by using the `add_bootstrap` method.
 
         :return: Resampled observation.
@@ -719,16 +760,16 @@
     def add_bootstrap(self, inference: 'Inference'):
         """
         Add main optimization result from another Inference object as a bootstrap to the current Inference object.
 
         :param inference: Inference object with bootstraps.
         :return: Inference object with bootstraps.
         """
-        if inference.params_inferred is None:
-            raise RuntimeError('The main optimization must be run first (call the `run` method).')
+        if inference.loss_inferred is None:
+            raise RuntimeError('The provided Inference object must be run first (call the `run` method).')
 
         self.bootstrap_results.append(inference.result.x)
         self.bootstrap_dists.append(inference.dist_inferred)
         self.bootstraps = pd.DataFrame(self.bootstrap_results, columns=list(self.x0.keys()))
 
     def add_bootstraps(self, inferences: Iterable['Inference']):
         """
```

### Comparing `phasegen-0.0.5b0/phasegen/lineage.py` & `phasegen-0.0.6b0/phasegen/lineage.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/phasegen/locus.py` & `phasegen-0.0.6b0/phasegen/locus.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
         :return: Initial state vector
         """
         if self.n == 1:
             # every lineage is on the same locus
             return np.ones(s.k)
 
         # number of lineages linked between loci
-        n_linked = max(s.pop_config.n - self.n_unlinked, 0)
+        n_linked = max(s.lineage_config.n - self.n_unlinked, 0)
 
-        # sum over demes and lineage blocks, and require all loci to have `n_linked` linked lineages
+        # sum over demes and lineage blocks, and require all loci to have ``n_linked`` linked lineages
         return (s.linked.sum(axis=(2, 3)) == n_linked).all(axis=1).astype(int)
 
     def __eq__(self, other):
         """
         Check if two locus configurations are equal.
 
         :param other: Other locus configuration
```

### Comparing `phasegen-0.0.5b0/phasegen/norms.py` & `phasegen-0.0.6b0/phasegen/norms.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/phasegen/rewards.py` & `phasegen-0.0.6b0/phasegen/rewards.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,35 +87,17 @@
 class BlockCountingReward(Reward, ABC):
     """
     Base class for rewards that count blocks. Such rewards are compatible with :class:`BlockCountingStateSpace`.
     """
     pass
 
 
-class DefaultReward(Reward, ABC):
+class TreeHeightReward(LineageCountingReward, BlockCountingReward):
     """
-    Default reward where all non-absorbing states have a reward of 1.
-
-    :meta private:
-    """
-    pass
-
-
-class NonDefaultReward(Reward, ABC):
-    """
-    Non-default reward where not all non-absorbing states have a reward of 1.
-
-    :meta private:
-    """
-    pass
-
-
-class TreeHeightReward(DefaultReward, LineageCountingReward, BlockCountingReward):
-    """
-    Reward based on tree height. Note that when using multiple loci, this will provide the
+    Reward for tree height. Note that when using multiple loci, this will provide the
     height of the locus with the highest tree.
     """
 
     def _get(self, state_space: StateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
@@ -128,18 +110,18 @@
             return np.any(state_space.states.sum(axis=(2, 3)) > 1, axis=1).astype(int)
 
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
-class TotalTreeHeightReward(NonDefaultReward, LineageCountingReward, BlockCountingReward):
+class TotalTreeHeightReward(LineageCountingReward, BlockCountingReward):
     """
-    Reward based on tree height. When using multiple loci, this will provide the sum of the
-    heights of all loci, regardless of whether they are linked or not.
+    Reward based on tree height. When using multiple loci, this will provide the sum of the tree 
+    heights over all loci, regardless of whether they are linked or not.
     """
 
     def _get(self, state_space: StateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
         :param state_space: state space
@@ -150,18 +132,18 @@
             return np.sum([LocusReward(i)._get(state_space) for i in range(state_space.locus_config.n)], axis=0)
 
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
-class TotalBranchLengthReward(NonDefaultReward, LineageCountingReward, BlockCountingReward):
+class TotalBranchLengthReward(LineageCountingReward, BlockCountingReward):
     """
-    Reward based on total branch length. When using multiple loci, this will provide the sum of the
-    total branch lengths of all loci, regardless of whether they are linked or not. Note that due to
+    Reward for total branch length. When using multiple loci, this will provide the sum of the
+    total branch lengths over all loci, regardless of whether they are linked or not. Note that due to
     inherent limitation to rewards, we cannot determine the total branch length of the tree with
     the largest total branch length as done in :class:`TreeHeightReward`.
     """
 
     def _get(self, state_space: StateSpace) -> np.ndarray:
         """
         Get the reward vector.
@@ -183,17 +165,17 @@
             return weights
 
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
-class SFSReward(NonDefaultReward, BlockCountingReward, ABC):
+class SFSReward(BlockCountingReward, ABC):
     """
-    Reward based on site frequency spectrum (SFS).
+    Base class for site frequency spectrum (SFS) rewards.
 
     :meta private:
     """
 
     def __init__(self, index: int = None):
         """
         Initialize the reward.
@@ -209,15 +191,15 @@
         :return: hash
         """
         return hash(self.__class__.__name__ + str(self.index))
 
 
 class UnfoldedSFSReward(SFSReward, BlockCountingReward):
     """
-    Reward based on unfolded site frequency spectrum (SFS).
+    Reward for unfolded site frequency spectrum (SFS).
     """
 
     def _get(self, state_space: BlockCountingStateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
         :param state_space: state space
@@ -231,28 +213,28 @@
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
 class FoldedSFSReward(SFSReward, BlockCountingReward):
     """
-    Reward based on folded site frequency spectrum (SFS).
+    Reward for folded site frequency spectrum (SFS).
     """
 
     def _get_indices(self, state_space: BlockCountingStateSpace) -> np.ndarray:
         """
         Get the indices of the blocks that make up the folded SFS bin.
 
         :param state_space: state space
         :return: indices
         """
-        if self.index == state_space.pop_config.n - self.index:
+        if self.index == state_space.lineage_config.n - self.index:
             return np.array([self.index - 1])
 
-        return np.array([self.index - 1, state_space.pop_config.n - self.index - 1])
+        return np.array([self.index - 1, state_space.lineage_config.n - self.index - 1])
 
     def _get(self, state_space: BlockCountingStateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
         :param state_space: state space
         :return: reward vector
@@ -265,18 +247,19 @@
             return state_space.states[:, :, :, blocks].sum(axis=(1, 2, 3))
 
         raise NotImplementedError(
             f'Unsupported state space type for reward {self.__class__.__name__}: {state_space.__class__.__name__}'
         )
 
 
-class DemeReward(NonDefaultReward, LineageCountingReward, BlockCountingReward):
+class DemeReward(LineageCountingReward, BlockCountingReward):
     """
-    Reward based on fraction of lineages in a specific deme. Taking the product of this reward with another reward
-    will result in a reward that only considers the specified deme.
+    Reward fraction of lineages in a specific deme. Taking the product of this reward with another reward
+    will result in a reward that only considers the specified deme. Use :class:`SumReward` to marginalize over
+    several demes.
     """
 
     def __init__(self, pop: str):
         """
         Initialize the reward.
 
         :param pop: The population id to use.
@@ -309,17 +292,17 @@
         Calculate the hash of the class name and the population name.
 
         :return: hash
         """
         return hash(self.__class__.__name__ + str(self.pop))
 
 
-class LocusReward(NonDefaultReward, LineageCountingReward):
+class LocusReward(LineageCountingReward):
     """
-    Reward based on fraction of lineages in a specific locus. Taking the product of this reward with another reward
+    Reward fraction of lineages in a specific locus. Taking the product of this reward with another reward
     will result in a reward that only considers the specified locus.
     """
 
     def __init__(self, locus: int):
         """
         Initialize the reward.
 
@@ -347,32 +330,34 @@
         Calculate the hash of the class name and the population name.
 
         :return: hash
         """
         return hash(self.__class__.__name__ + str(self.locus))
 
 
-class UnitReward(NonDefaultReward, LineageCountingReward, BlockCountingReward):
+class UnitReward(LineageCountingReward, BlockCountingReward):
     """
-    Rewards all states with 1 (including absorbing states).
+    Reward all states with 1 (including absorbing states).
     """
 
     def _get(self, state_space: StateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
         :param state_space: state space
         :return: reward vector
         """
         return np.ones(state_space.k)
 
 
 class TotalBranchLengthLocusReward(LocusReward, LineageCountingReward):
     """
-    Reward based on total branch length per locus.
+    Reward for total branch length per locus. This is needed as the taking the product of
+    :class:`TotalBranchLengthReward` and :class:`LocusReward` will not work as expected (see
+    :class:`CombinedReward`).
     """
 
     def _get(self, state_space: StateSpace) -> np.ndarray:
         """
         Get the reward vector.
 
         :param state_space: state space
```

### Comparing `phasegen-0.0.5b0/phasegen/serialization.py` & `phasegen-0.0.6b0/phasegen/serialization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/phasegen/spectrum.py` & `phasegen-0.0.6b0/phasegen/spectrum.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         :param power: exponent
         :return: Spectrum
         """
         return SFS2(self.data ** power)
 
     def fold(self) -> 'SFS2':
         """
-        Fold 2-SFS by adding up `i` and `n - i` for both axes.
+        Fold 2-SFS by adding up ``i`` and ``n - i`` for both axes.
         Node that this only make sense for counts or frequencies.
 
         :return: Folded 2-SFS.
         """
         data = self.data.copy()
 
         for _ in range(2):
@@ -179,15 +179,15 @@
 
         :return: Deep copy.
         """
         return copy.deepcopy(self)
 
     def symmetrize(self) -> 'SFS2':
         """
-        Symmetric SFS so that `i, j` and `j, i` are the same.
+        Symmetric SFS so that ``i, j`` and ``j, i`` are the same.
 
         :return: Symmetric 2-SFS.
         """
         return SFS2((self.data + self.data.T) / 2)
 
     def fill_monomorphic(self, fill_value=np.nan) -> 'SFS2':
         """
```

### Comparing `phasegen-0.0.5b0/phasegen/state_space.py` & `phasegen-0.0.6b0/phasegen/state_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 class StateSpace(ABC):
     """
     State space.
     """
 
     def __init__(
             self,
-            pop_config: LineageConfig,
+            lineage_config: LineageConfig,
             locus_config: LocusConfig = None,
             model: CoalescentModel = None,
             epoch: Epoch = None,
             cache: bool = True
     ):
         """
         Create a rate matrix.
 
-        :param pop_config: Population configuration.
+        :param lineage_config: Population configuration.
         :param locus_config: Locus configuration. One locus is used by default.
         :param model: Coalescent model. By default, the standard coalescent is used.
         :param epoch: Epoch.
         :param cache: Whether to cache the rate matrix for different epochs.
         """
         if locus_config is None:
             locus_config = LocusConfig()
@@ -55,15 +55,15 @@
         #: Logger
         self._logger = logger.getChild(self.__class__.__name__)
 
         #: Coalescent model
         self.model: CoalescentModel = model
 
         #: Population configuration
-        self.pop_config: LineageConfig = pop_config
+        self.lineage_config: LineageConfig = lineage_config
 
         #: Locus configuration
         self.locus_config: LocusConfig = locus_config
 
         #: Epoch
         self.epoch: Epoch = epoch
 
@@ -84,16 +84,17 @@
 
         # time in seconds to compute original rate matrix
         self.time: float | None = None
 
     @cached_property
     def states(self) -> np.ndarray:
         """
-        Get the states. Each state describes the lineage configuration per deme and locus, i.e.
-        one state has the structure [[[a_ijk]]] where i is the lineage configuration, j is the deme and k is the locus.
+        The states. Each state describes the lineage configuration per deme and locus, i.e.,
+        one state has the structure ``[[[a_ijk]]]`` where ``i`` is the lineage configuration, ``j`` is the deme
+        and ``k`` is the locus.
         """
         start = time.time()
 
         # get all possible transitions
         transitions, states = self.get_transitions()
 
         # record time to compute rate matrix
@@ -109,15 +110,15 @@
 
         # indices of non-zero rates
         return np.array([s.lineages for s in states])
 
     @cached_property
     def _states(self) -> List['State']:
         """
-        Get the (ordered) list of states.
+        Ordered list of states.
         """
         _ = self.states
         return self.__states
 
     @abstractmethod
     def _get_old(self) -> OldStateSpace:
         """
@@ -156,54 +157,52 @@
         Vector with ones of size ``k``.
         """
         return np.ones(self.k)
 
     @cached_property
     def S(self) -> np.ndarray:
         """
-        Get full intensity matrix.
+        Intensity matrix.
         """
         return self._get_rate_matrix()
 
     @cached_property
     def alpha(self) -> np.ndarray:
         """
         Initial state vector.
         """
-        pops = self.pop_config._get_initial_states(self)
+        pops = self.lineage_config._get_initial_states(self)
         loci = self.locus_config._get_initial_states(self)
 
         # combine initial states
         alpha = pops * loci
 
         # return normalized vector
         # normalization ensures that the initial state vector is a probability distribution
         # as we may have multiple initial states
         return alpha / alpha.sum()
 
     @cached_property
     def k(self) -> int:
         """
-        Get number of states.
-
-        :return: The number of states.
+        Number of states.
         """
         k = len(self.states)
 
         # warn if state space is large
         if k > 400:
             self._logger.warning(f'State space is large ({k} states). Note that the computation time '
                                  f'increases exponentially with the number of states.')
 
         return k
 
     @cached_property
     def transition(self) -> 'Transition':
         """
-        Get Transition.
+        Transition.
         """
         return Transition(self)
 
     def update_epoch(self, epoch: Epoch):
         """
         Update the epoch.
 
@@ -222,15 +221,15 @@
         update the epoch of a state space.
 
         :param other: Other state space
         :return: Whether the two state spaces are equal
         """
         return (
                 self.__class__ == other.__class__ and
-                self.pop_config == other.pop_config and
+                self.lineage_config == other.lineage_config and
                 self.locus_config == other.locus_config and
                 self.model == other.model
         )
 
     def drop_S(self):
         """
         Drop the current rate matrix.
@@ -363,33 +362,35 @@
             return '#f1807e'
 
         if self.alpha[i] > 0:
             return 'lightgreen'
 
         return 'lightblue'
 
-    def _plot_rates(
+    def plot_rates(
             self,
             file: str,
             view: bool = True,
             cleanup: bool = False,
             dpi: int = 400,
             ratio: float = 0.6,
+            background_color: str = 'white',
             extension: str = 'png',
             format_state: Callable[[np.array], str] = None,
             format_transition: Callable[['Transition'], str] = None
     ):
         """
-        Plot the rate matrix using graphviz.
+        Plot the rate matrix using graphviz. Note that graphviz must be installed which is an external dependency.
 
         :param file: File to save plot to.
         :param view: Whether to view the plot.
         :param cleanup: Whether to remove the source file.
         :param dpi: Dots per inch.
         :param ratio: Aspect ratio.
+        :param background_color: Background color.
         :param extension: File format.
         :param format_state: Function to format state with state array as argument.
         :param format_transition: Function to format transition with transition as argument.
         """
         import graphviz
 
         if format_state is None:
@@ -434,14 +435,15 @@
                     label=format_transition(*transition),
                     color=Transition._colors[transition[1]],
                     fontcolor=Transition._colors[transition[1]]
                 )
 
         graph.graph_attr['dpi'] = str(dpi)
         graph.graph_attr['ratio'] = str(ratio)
+        graph.graph_attr['bgcolor'] = background_color
 
         graph.render(
             filename=file,
             view=view,
             cleanup=cleanup,
             format=extension
         )
@@ -452,25 +454,25 @@
     Default rate matrix where there is one state per number of lineages for each deme and locus.
     """
 
     def _get_initial(self):
         """
         Get the initial state.
         """
-        data = tuple(np.zeros((self.locus_config.n, self.pop_config.n_pops, 1), dtype=int) for _ in range(2))
-        data[0][:, 0, 0] = self.pop_config.n
+        data = tuple(np.zeros((self.locus_config.n, self.lineage_config.n_pops, 1), dtype=int) for _ in range(2))
+        data[0][:, 0, 0] = self.lineage_config.n
 
         return State(data)
 
     def _get_old(self) -> OldDefaultStateSpace:
         """
         Get the old state space.
         """
         return OldDefaultStateSpace(
-            pop_config=self.pop_config,
+            lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
             epoch=self.epoch
         )
 
 
 class BlockCountingStateSpace(StateSpace):
@@ -480,51 +482,52 @@
 
     per deme and per locus. This state space can distinguish between different tree topologies
     and is thus used when computing statistics based on the SFS.
     """
 
     def __init__(
             self,
-            pop_config: LineageConfig,
+            lineage_config: LineageConfig,
             locus_config: LocusConfig = None,
             model: CoalescentModel = None,
             epoch: Epoch = None
     ):
         """
         Create a rate matrix.
 
-        :param pop_config: Population configuration.
+        :param lineage_config: Population configuration.
         :param locus_config: Locus configuration. One locus is used by default.
         :param model: Coalescent model. By default, the standard coalescent is used.
         :param epoch: Epoch.
         """
         # currently only one locus is supported, due to a very complex state space for multiple loci
         if locus_config is not None and locus_config.n > 1:
             raise NotImplementedError('Block counting state space only supports one locus.')
 
-        super().__init__(pop_config=pop_config, locus_config=locus_config, model=model, epoch=epoch)
+        super().__init__(lineage_config=lineage_config, locus_config=locus_config, model=model, epoch=epoch)
 
     def _get_initial(self):
         """
         Get the initial state.
         """
         data = tuple(
-            np.zeros((self.locus_config.n, self.pop_config.n_pops, self.pop_config.n), dtype=int) for _ in range(2)
+            np.zeros((self.locus_config.n, self.lineage_config.n_pops, self.lineage_config.n), dtype=int)
+            for _ in range(2)
         )
 
-        data[0][:, 0, 0] = self.pop_config.n
+        data[0][:, 0, 0] = self.lineage_config.n
 
         return State(data)
 
     def _get_old(self) -> OldBlockCountingStateSpace:
         """
         Get the old state space.
         """
         return OldBlockCountingStateSpace(
-            pop_config=self.pop_config,
+            lineage_config=self.lineage_config,
             locus_config=self.locus_config,
             model=self.model,
             epoch=self.epoch
         )
 
 
 class Transition:
@@ -540,14 +543,15 @@
         'linked_coalescence': 'darkgreen',
         'unlinked_coalescence': 'darkgreen',
         'mixed_coalescence': 'darkgreen',
         'unlinked_coalescence+mixed_coalescence': 'darkgreen',
         'mixed_coalescence+unlinked_coalescence': 'darkgreen',
         'linked_migration': 'blue',
         'unlinked_migration': 'blue',
+        'migration': 'blue',
         'invalid': 'red'
     }
 
     def __init__(
             self,
             state_space: StateSpace
     ):
@@ -599,22 +603,22 @@
         """
         Get all possible coalescent transitions from the given state.
 
         :param source: Source state.
         :return: All possible coalescent transitions from the given state.
         """
         targets: Dict['State', Tuple[float, str]] = {}
-        pop_sizes = [self.state_space.epoch.pop_sizes[pop] for pop in self.state_space.pop_config.pop_names]
+        pop_sizes = [self.state_space.epoch.pop_sizes[pop] for pop in self.state_space.lineage_config.pop_names]
 
         if source.n_loci == 1:
             locus = 0
             for deme in range(source.n_demes):
 
                 blocks = self.state_space.model.coalesce(
-                    self.state_space.pop_config.n,
+                    self.state_space.lineage_config.n,
                     source.lineages[locus, deme]
                 )
 
                 for block, rate in blocks:
                     target = source.copy()
                     target.lineages[locus, deme] = block
 
@@ -712,15 +716,15 @@
         Get all possible unlinked migration transitions from the given state.
         Note that we also consider migration to unlinked when there is only one locus.
 
         :param source: Source state.
         :return: All possible migration transitions from the given state.
         """
         targets: Dict['State', Tuple[float, str]] = {}
-        pop_names = self.state_space.pop_config.pop_names
+        pop_names = self.state_space.lineage_config.pop_names
         kind = 'migration' if source.n_loci == 1 else 'unlinked_migration'
 
         for locus in range(source.n_loci):
             for d1, d2 in filter(lambda x: x[0] != x[1], product(range(source.n_demes), repeat=2)):
 
                 for block in range(source.n_blocks):
 
@@ -749,15 +753,15 @@
         """
         targets: Dict['State', Tuple[float, str]] = {}
 
         # no linked migration if there is only one locus
         if source.n_loci == 1:
             return targets
 
-        pop_names = self.state_space.pop_config.pop_names
+        pop_names = self.state_space.lineage_config.pop_names
 
         for d1, d2 in filter(lambda x: x[0] != x[1], product(range(source.n_demes), repeat=2)):
 
             for block in range(source.n_blocks):
 
                 # skip if no lineages to migrate
                 if np.all(source.lineages[:, d1, block]) > 0 and np.all(source.linked[:, d1, block] > 0):
```

### Comparing `phasegen-0.0.5b0/phasegen/state_space_old.py` & `phasegen-0.0.6b0/phasegen/state_space_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 class StateSpace(ABC):
     """
     State space.
     """
 
     def __init__(
             self,
-            pop_config: LineageConfig,
+            lineage_config: LineageConfig,
             locus_config: LocusConfig = None,
             model: CoalescentModel = None,
             epoch: Epoch = None,
             cache: bool = True
     ):
         """
         Create a rate matrix.
 
-        :param pop_config: Population configuration.
+        :param lineage_config: Population configuration.
         :param locus_config: Locus configuration. One locus is used by default.
         :param model: Coalescent model. By default, the standard coalescent is used.
         :param epoch: Epoch.
         :param cache: Whether to cache the rate matrix for different epochs.
         """
         if locus_config is None:
             locus_config = LocusConfig()
@@ -55,15 +55,15 @@
         #: Logger
         self._logger = logger.getChild(self.__class__.__name__)
 
         #: Coalescent model
         self.model: CoalescentModel = model
 
         #: Population configuration
-        self.pop_config: LineageConfig = pop_config
+        self.lineage_config: LineageConfig = lineage_config
 
         #: Locus configuration
         self.locus_config: LocusConfig = locus_config
 
         #: Epoch
         self.epoch: Epoch = epoch
 
@@ -78,18 +78,15 @@
 
         # time in seconds to compute original rate matrix
         self.time: float | None = None
 
     @cached_property
     def _non_zero_states(self) -> Tuple[np.ndarray, ...]:
         """
-        Get the indices of non-zero rates. This improves performance when computing the rate matrix
-        for different epochs
-
-        :return: Indices of non-zero rates.
+        Indices of non-zero rates.
         """
         # cache the current epoch
         epoch = self.epoch
 
         # we first determine the non-zero states by using default values for the demography
         self.epoch = Epoch(
             pop_sizes={p: 1 for p in epoch.pop_names},
@@ -115,40 +112,41 @@
         # this improves performance when recomputing the rate matrix for different epochs
         return np.where(default_rate_matrix != 0)
 
     @cached_property
     @abstractmethod
     def states(self) -> np.ndarray:
         """
-        Get the states. Each state describes the lineage configuration per deme and locus, i.e.
-        one state has the structure [[[a_ijk]]] where i is the lineage configuration, j is the deme and k is the locus.
+        The states. Each state describes the lineage configuration per deme and locus, i.e.,
+        one state has the structure ``[[[a_ijk]]]`` where ``i`` is the lineage configuration, ``j`` is the deme
+        and ``k`` is the locus.
         """
         pass
 
     @cached_property
     def e(self) -> np.ndarray:
         """
-        Vector with ones of size ``n``.
+        Vector with ones of size `k`.
         """
         return np.ones(self.k)
 
     @cached_property
     def S(self) -> np.ndarray:
         """
-        Get full intensity matrix.
+        Intensity matrix.
         """
         # obtain intensity matrix
         return self._get_rate_matrix()
 
     @cached_property
     def alpha(self) -> np.ndarray:
         """
         Initial state vector.
         """
-        pops = self.pop_config._get_initial_states(self)
+        pops = self.lineage_config._get_initial_states(self)
         loci = self.locus_config._get_initial_states(self)
 
         # combine initial states
         alpha = pops * loci
 
         # return normalized vector
         # normalization ensures that the initial state vector is a probability distribution
@@ -174,41 +172,37 @@
         update the epoch of a state space.
 
         :param other: Other state space
         :return: Whether the two state spaces are equal
         """
         return (
                 self.__class__ == other.__class__ and
-                self.pop_config == other.pop_config and
+                self.lineage_config == other.lineage_config and
                 self.locus_config == other.locus_config and
                 self.model == other.model
         )
 
     @cached_property
     def k(self) -> int:
         """
-        Get number of states.
-
-        :return: The number of states.
+        Number of states.
         """
         k = len(self.states)
 
         # warn if state space is large
         if k > 400:
             self._logger.warning(f'State space is large ({k} states). Note that the computation time '
                                  f'increases exponentially with the number of states.')
 
         return k
 
     @cached_property
     def m(self) -> int:
         """
-        Length of the state vector for a single deme.
-
-        :return: The length
+        Length of state vector for a single deme.
         """
         return self.states.shape[2]
 
     def drop_S(self):
         """
         Drop the current rate matrix.
         """
@@ -267,20 +261,20 @@
         :return: The sparsity.
         """
         return 1 - np.count_nonzero(self.S) / self.S.size
 
     @abstractmethod
     def _get_coalescent_rate(self, n: int, s1: np.ndarray, s2: np.ndarray) -> float:
         """
-        Get the coalescent rate from state ``s1`` to state ``s2``.
+        Get the coalescent rate from state `s1` to state `s2`.
 
         :param n: Number of lineages.
         :param s1: Block configuration of state 1.
         :param s2: Block configuration of state 2.
-        :return: The coalescent rate from state ``s1`` to state ``s2``.
+        :return: The coalescent rate from state `s1` to state `s2`.
         """
         pass
 
     def _get_rate(self, i: int, j: int) -> float:
         """
         Get the rate from the state indexed by i to the state indexed by j.
 
@@ -396,19 +390,19 @@
             cleanup=cleanup,
             format=extension
         )
 
     @staticmethod
     def _find_vectors(n: int, k: int) -> List[List[int]]:
         """
-        Find all vectors of length ``k`` with non-negative integers that sum to ``n``.
+        Find all vectors of length `k` with non-negative integers that sum to `n`.
 
         :param n: The sum.
         :param k: The length of the vectors.
-        :return: All vectors of length ``k`` with non-negative integers that sum to ``n``.
+        :return: All vectors of length `k` with non-negative integers that sum to `n`.
         """
         if k == 0:
             return [[]]
 
         if k == 1:
             return [[n]]
 
@@ -418,30 +412,30 @@
                 vectors.append(vector + [i])
 
         return vectors
 
     @staticmethod
     def p(n: int, k: int) -> int:
         """
-        Partition function. Get number of ways to partition ``n`` into ``k`` positive integers.
+        Partition function. Get number of ways to partition `n` into `k` positive integers.
 
         :param n: Number to partition.
         :param k: Number of parts.
-        :return: Number of ways to partition ``n`` into ``k`` positive integers.
+        :return: Number of ways to partition `n` into `k` positive integers.
         """
         return comb(n - 1, k - 1, exact=True)
 
     @classmethod
     def p0(cls, n: int, k: int) -> int:
         """
-        Partition function. Get number of ways to partition ``n`` into ``k`` non-negative integers.
+        Partition function. Get number of ways to partition `n` into `k` non-negative integers.
 
         :param n: Number to partition.
         :param k: Number of parts.
-        :return: Number of ways to partition ``n`` into ``k`` non-negative integers.
+        :return: Number of ways to partition `n` into `k` non-negative integers.
         """
         return cls.p(n + k, k)
 
     @staticmethod
     def P(n: int) -> int:
         """
         Calculate the number of partitions of a non-negative integer.
@@ -486,20 +480,20 @@
 class DefaultStateSpace(StateSpace):
     """
     Default rate matrix where there is one state per number of lineages for each deme and locus.
     """
 
     def _get_coalescent_rate(self, n: int, s1: np.ndarray, s2: np.ndarray) -> float:
         """
-        Get the coalescent rate from state ``s1`` to state ``s2``.
+        Get the coalescent rate from state `s1` to state `s2`.
 
         :param n: Number of lineages.
         :param s1: Block configuration of state 1.
         :param s2: Block configuration of state 2.
-        :return: The coalescent rate from state ``s1`` to state ``s2``.
+        :return: The coalescent rate from state `s1` to state `s2`.
         """
         return self.model.get_rate(s1=s1[0], s2=s2[0])
 
     def _expand_loci(self, states: np.ndarray) -> np.ndarray:
         """
         Expand the given states to include all possible combinations of locus configurations.
 
@@ -511,19 +505,19 @@
 
             # no lineages are linked
             self.linked = np.zeros_like(states, dtype=int)
 
             return states
 
         if self.locus_config.n == 2:
-            n_pops = self.pop_config.n_pops
+            n_pops = self.lineage_config.n_pops
 
             # determine number of linked lineage configurations irrespective of states
-            linked_locus = np.array(list(itertools.product(range(self.pop_config.n + 1), repeat=n_pops)))
-            linked_locus = linked_locus[linked_locus.sum(axis=1) <= self.pop_config.n]
+            linked_locus = np.array(list(itertools.product(range(self.lineage_config.n + 1), repeat=n_pops)))
+            linked_locus = linked_locus[linked_locus.sum(axis=1) <= self.lineage_config.n]
 
             # expand loci, each deme needs to have the same number of linked lineages
             linked = np.repeat(linked_locus[:, np.newaxis], 2, axis=1)
 
             # add extra dimension for lineage blocks
             linked = linked[..., np.newaxis]
 
@@ -538,19 +532,20 @@
             return states_new[:, 1, :, :]
 
         raise NotImplementedError("Only 1 or 2 loci are currently supported.")
 
     @cached_property
     def states(self) -> np.ndarray:
         """
-        Get the states. Each state describes the lineage configuration per deme and locus, i.e.
-        one state has the structure [[[a_ijk]]] where i is the lineage configuration, j is the deme and k is the locus.
+        The states. Each state describes the lineage configuration per deme and locus, i.e.,
+        one state has the structure `[[[a_ijk]]]` where `i` is the lineage configuration, `j` is the deme and `k` is
+        the locus.
         """
         # the number of lineages
-        lineages = np.arange(1, self.pop_config.n + 1)[::-1]
+        lineages = np.arange(1, self.lineage_config.n + 1)[::-1]
 
         # iterate lineage configurations and find all possible deme configurations
         states = []
         for i in lineages:
             states += self._find_vectors(n=i, k=self.epoch.n_pops)
 
         # convert to numpy array
@@ -567,16 +562,16 @@
     def get_k(self) -> int:
         """
         Get number of states.
         TODO currently no support for multiple loci.
 
         :return: The number of states.
         """
-        n = self.pop_config.n
-        d = self.pop_config.n_pops
+        n = self.lineage_config.n
+        d = self.lineage_config.n_pops
 
         i = np.arange(1, n + 1)[::-1]
 
         k = np.sum([self.p0(j, d) for j in i])
 
         return k
 
@@ -588,41 +583,41 @@
 
     per deme and per locus. This state space can distinguish between different tree topologies
     and is thus used when computing statistics based on the SFS.
     """
 
     def __init__(
             self,
-            pop_config: LineageConfig,
+            lineage_config: LineageConfig,
             locus_config: LocusConfig = None,
             model: CoalescentModel = None,
             epoch: Epoch = None
     ):
         """
         Create a rate matrix.
 
-        :param pop_config: Population configuration.
+        :param lineage_config: Population configuration.
         :param locus_config: Locus configuration. One locus is used by default.
         :param model: Coalescent model. By default, the standard coalescent is used.
         :param epoch: Epoch.
         """
         # currently only one locus is supported, due to a very complex state space for multiple loci
         if locus_config is not None and locus_config.n > 1:
             raise NotImplementedError('Block counting state space only supports one locus.')
 
-        super().__init__(pop_config=pop_config, locus_config=locus_config, model=model, epoch=epoch)
+        super().__init__(lineage_config=lineage_config, locus_config=locus_config, model=model, epoch=epoch)
 
     def _get_coalescent_rate(self, n: int, s1: np.ndarray, s2: np.ndarray) -> float:
         """
-        Get the coalescent rate from state ``s1`` to state ``s2``.
+        Get the coalescent rate from state `s1` to state `s2`.
 
         :param n: Number of lineages.
         :param s1: Block configuration of state 1.
         :param s2: Block configuration of state 2.
-        :return: The coalescent rate from state ``s1`` to state ``s2``.
+        :return: The coalescent rate from state `s1` to state `s2`.
         """
         return self.model.get_rate_block_counting(n=n, s1=s1, s2=s2)
 
     def _expand_loci(self, states: np.ndarray) -> np.ndarray:
         """
         Expand the given states to include all possible combinations of locus configurations.
         TODO two-locus state space not sufficient for computing SFS as lineages are not longer
@@ -669,21 +664,20 @@
             self.linked = expanded[:, :, 1]
 
             return expanded[:, :, 0]
 
     @cached_property
     def states(self) -> np.ndarray:
         """
-        Get the states. Each state describes the lineage configuration per deme and locus, i.e.
-        one state has the structure [[[a_ijk]]] where i is the lineage configuration, j is the deme and k is the locus.
-
-        :return: The states.
+        The states. Each state describes the lineage configuration per deme and locus, i.e.,
+        one state has the structure `[[[a_ijk]]]` where `i` is the lineage configuration, `j` is the deme and `k` is
+        the locus.
         """
         # the possible allele configurations
-        lineage_configs = np.array(self._find_sample_configs(m=self.pop_config.n, n=self.pop_config.n))
+        lineage_configs = np.array(self._find_sample_configs(m=self.lineage_config.n, n=self.lineage_config.n))
 
         # iterate over possible allele configurations and find all possible deme configurations
         states = []
         for config in lineage_configs:
 
             # iterate over possible number of lineages with multiplicity k and
             # find all possible deme configurations
@@ -728,16 +722,16 @@
 
     def get_k(self) -> int:
         """
         Get number of states.
 
         :return: The number of states.
         """
-        n = self.pop_config.n
-        d = self.pop_config.n_pops
+        n = self.lineage_config.n
+        d = self.lineage_config.n_pops
 
         # len(i) == self.P(n)
         i = np.array(self._find_sample_configs(m=n, n=n))
 
         k = np.sum([np.prod([self.p0(l, d) for l in j]) for j in i])
 
         return k
@@ -1431,44 +1425,44 @@
         unlinked coalescence event in each locus, and subsequently n - 1 locus coalescence events. Now the state looks
         identical to the first scenario but it should be allowed to have a linked coalescence event where one of the
         lineages is a doubleton in one locus and a singleton in the other locus, given that an unlinked doubleton
         coalesced with an unlinked singleton. We thus need to keep track of the associations between lineages, which
         means they are no longer exchangeable.
         """
         return self.state_space._get_coalescent_rate(
-            n=self.state_space.pop_config.n,
+            n=self.state_space.lineage_config.n,
             s1=self.linked1[0, self.deme_coal],
             s2=self.linked2[0, self.deme_coal]
         ) / self.get_scaled_pop_size_coalescence()
 
         # if (
         #        np.all(self.linked1[:, self.deme_coal] == self.linked1[0, self.deme_coal]) and
         #        np.any(self.linked2[:, self.deme_coal] != self.linked2[0, self.deme_coal])
         # ):
         #    return 0
 
         # rates = np.zeros(self.n_loci)
         # for i in range(self.n_loci):
         #    rates[i] = self.state_space._get_coalescent_rate(
-        #        n=self.state_space.pop_config.n,
+        #        n=self.state_space.lineage_config.n,
         #        s1=self.linked1[i, self.deme_coal],
         #        s2=self.linked2[i, self.deme_coal]
         #    )
 
         # return rates.min() / self.get_scaled_pop_size_coalescence()
 
     def get_rate_unlinked_coalescence(self) -> float:
         """
         Get the rate of an unlinked coalescence event.
         """
         unlinked1 = self.unlinked1[self.locus_coal_unlinked, self.deme_coal]
         unlinked2 = self.unlinked2[self.locus_coal_unlinked, self.deme_coal]
 
         rate = self.state_space._get_coalescent_rate(
-            n=self.state_space.pop_config.n,
+            n=self.state_space.lineage_config.n,
             s1=unlinked1,
             s2=unlinked2
         )
 
         return rate / self.get_scaled_pop_size_coalescence()
 
     def get_rate_mixed_coalescence(self) -> float:
```

### Comparing `phasegen-0.0.5b0/phasegen/utils.py` & `phasegen-0.0.6b0/phasegen/utils.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/phasegen/visualization.py` & `phasegen-0.0.6b0/phasegen/visualization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.5b0/pyproject.toml` & `phasegen-0.0.6b0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phasegen"
-version = "0.0.5-beta"
+version = "0.0.6-beta"
 description = "Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `phasegen-0.0.5b0/PKG-INFO` & `phasegen-0.0.6b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasegen
-Version: 0.0.5b0
+Version: 0.0.6b0
 Summary: Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

