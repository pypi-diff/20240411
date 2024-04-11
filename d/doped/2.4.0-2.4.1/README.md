# Comparing `tmp/doped-2.4.0.tar.gz` & `tmp/doped-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doped-2.4.0.tar", last modified: Sun Mar 31 05:27:44 2024, max compression
+gzip compressed data, was "doped-2.4.1.tar", last modified: Thu Apr 11 05:54:42 2024, max compression
```

## Comparing `doped-2.4.0.tar` & `doped-2.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.432201 doped-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-31 05:26:22.000000 doped-2.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13819 2024-03-31 05:27:44.432201 doped-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-03-31 05:26:22.000000 doped-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.424201 doped-2.4.0/doped/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.428201 doped-2.4.0/doped/VASP_sets/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-31 05:26:22.000000 doped-2.4.0/doped/VASP_sets/DefectSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-31 05:26:22.000000 doped-2.4.0/doped/VASP_sets/HSESet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-31 05:26:22.000000 doped-2.4.0/doped/VASP_sets/PBEsol_ConvergenceSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-31 05:26:22.000000 doped-2.4.0/doped/VASP_sets/PotcarSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-31 05:26:22.000000 doped-2.4.0/doped/VASP_sets/RelaxSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-03-31 05:26:22.000000 doped-2.4.0/doped/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   113093 2024-03-31 05:26:22.000000 doped-2.4.0/doped/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    88639 2024-03-31 05:26:22.000000 doped-2.4.0/doped/chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    85980 2024-03-31 05:26:22.000000 doped-2.4.0/doped/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-03-31 05:26:22.000000 doped-2.4.0/doped/corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)   108002 2024-03-31 05:26:22.000000 doped-2.4.0/doped/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)   147246 2024-03-31 05:26:22.000000 doped-2.4.0/doped/thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.428201 doped-2.4.0/doped/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/displacement.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    24728 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/doped.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)    30936 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/eigenvalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/legacy_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)    62379 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    39141 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/supercells.py
--rw-r--r--   0 runner    (1001) docker     (127)    69846 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)   148776 2024-03-31 05:26:22.000000 doped-2.4.0/doped/utils/wyckpos.dat
--rw-r--r--   0 runner    (1001) docker     (127)   117892 2024-03-31 05:26:22.000000 doped-2.4.0/doped/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.432201 doped-2.4.0/doped.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13819 2024-03-31 05:27:44.000000 doped-2.4.0/doped.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-31 05:27:44.000000 doped-2.4.0/doped.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 05:27:44.000000 doped-2.4.0/doped.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-31 05:27:44.000000 doped-2.4.0/doped.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-31 05:27:44.000000 doped-2.4.0/doped.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-31 05:26:25.000000 doped-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 05:27:44.432201 doped-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 05:27:44.432201 doped-2.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)   150889 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    34638 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_chemical_potentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_displacements.py
--rw-r--r--   0 runner    (1001) docker     (127)   165562 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    96396 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)    81920 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-31 05:26:27.000000 doped-2.4.0/tests/test_wyckoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.649243 doped-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-11 05:53:24.000000 doped-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-04-11 05:54:42.649243 doped-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-04-11 05:53:24.000000 doped-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.641243 doped-2.4.1/doped/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.641243 doped-2.4.1/doped/VASP_sets/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-11 05:53:25.000000 doped-2.4.1/doped/VASP_sets/DefectSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-11 05:53:25.000000 doped-2.4.1/doped/VASP_sets/HSESet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-11 05:53:25.000000 doped-2.4.1/doped/VASP_sets/PBEsol_ConvergenceSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-11 05:53:25.000000 doped-2.4.1/doped/VASP_sets/PotcarSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-11 05:53:25.000000 doped-2.4.1/doped/VASP_sets/RelaxSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-11 05:53:25.000000 doped-2.4.1/doped/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116875 2024-04-11 05:53:25.000000 doped-2.4.1/doped/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90125 2024-04-11 05:53:25.000000 doped-2.4.1/doped/chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88148 2024-04-11 05:53:25.000000 doped-2.4.1/doped/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28951 2024-04-11 05:53:25.000000 doped-2.4.1/doped/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108002 2024-04-11 05:53:25.000000 doped-2.4.1/doped/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147387 2024-04-11 05:53:25.000000 doped-2.4.1/doped/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.645243 doped-2.4.1/doped/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/displacement.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    24728 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/doped.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)    30685 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/eigenvalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/legacy_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62103 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39178 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69846 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148776 2024-04-11 05:53:25.000000 doped-2.4.1/doped/utils/wyckpos.dat
+-rw-r--r--   0 runner    (1001) docker     (127)   117811 2024-04-11 05:53:25.000000 doped-2.4.1/doped/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.649243 doped-2.4.1/doped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13942 2024-04-11 05:54:42.000000 doped-2.4.1/doped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 05:54:42.000000 doped-2.4.1/doped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:54:42.000000 doped-2.4.1/doped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-11 05:54:42.000000 doped-2.4.1/doped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 05:54:42.000000 doped-2.4.1/doped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-11 05:53:27.000000 doped-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:54:42.649243 doped-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:54:42.649243 doped-2.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)   152828 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36321 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_chemical_potentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165562 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97854 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82287 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-11 05:53:30.000000 doped-2.4.1/tests/test_wyckoff.py
```

### Comparing `doped-2.4.0/LICENSE` & `doped-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/PKG-INFO` & `doped-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <skavanagh@seas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -91,15 +91,16 @@
 - **Thermodynamic Analysis**: Compute (non-)equilibrium Fermi levels, defect/carrier concentrations etc. as functions of annealing/cooling temperature, chemical potentials etc.
 - **Plotting**: Generate publication-quality plots of defect formation energies, chemical potential limits, defect/carrier concentrations, Fermi levels, charge corrections, etc.
 - **`Python` Interface**: Fully-customisable, modular `Python` API. Plug-and-play w/[`ShakeNBreak`](https://shakenbreak.readthedocs.io) – [defect structure-searching](https://www.nature.com/articles/s41524-023-00973-1), [`easyunfold`](https://smtg-bham.github.io/easyunfold/) – band unfolding, [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/[`nonrad`](https://nonrad.readthedocs.io/en/latest/) – non-radiative recombination etc.
 - Reproducibility, tabulation, automated compatibility/sanity checking, strain/displacement analysis, shallow defect analysis, high-throughput compatibility, Wyckoff analysis...
 
 ### Performance and Example Outputs
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
-**a.** Optimal supercell generation comparison. **b.** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
+**(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
+displacements from DFT supercell calculations. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
 <!-- Update this link!! -->
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doped Version: 2.4.0 Summary: Python package to
+Metadata-Version: 2.1 Name: doped Version: 2.4.1 Summary: Python package to
 setup, process and analyse solid-state defect calculations with VASP Author-
 email: SeÃ¡n Kavanagh
 seas.harvard.edu> License: MIT License Copyright (c) 2021 SeÃ¡n Kavanagh
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -76,32 +76,34 @@
 (https://smtg-bham.github.io/easyunfold/) â band unfolding,
 [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/
 [`nonrad`](https://nonrad.readthedocs.io/en/latest/) â non-radiative
 recombination etc. - Reproducibility, tabulation, automated compatibility/
 sanity checking, strain/displacement analysis, shallow defect analysis, high-
 throughput compatibility, Wyckoff analysis... ### Performance and Example
 Outputs ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/
-doped_JOSS_figure.png) **a.** Optimal supercell generation comparison. **b.**
+doped_JOSS_figure.png) **(a)** Optimal supercell generation comparison. **(b)**
 Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-
 size correction plot, **(d)** defect formation energy diagram, **(e)** chemical
 potential / stability region, **(f)** Fermi level vs. annealing temperature, **
 (g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi
-level / carrier concentration heatmap plots from `doped`. See the [JOSS paper]
-(https://github.com/openjournals/joss-reviews/issues/6433) for more details. ##
-Installation ```bash pip install doped # install doped and dependencies ```
-Alternatively if desired, `doped` can also be installed from `conda` with:
-```bash conda install -c conda-forge doped pip install pydefect # pydefect not
-available on conda, so needs to be installed with pip or otherwise, if using
-the eFNV correction ``` If you haven't done so already, you will need to set up
-your VASP `POTCAR` files and `Materials Project` API with `pymatgen` using the
-`.pmgrc.yaml` file, in order for `doped` to automatically generate VASP input
-files for defect calculations and determine competing phases for chemical
-potentials. See the docs [Installation](https://doped.readthedocs.io/en/latest/
-Installation.html) page for details on this. ## `ShakeNBreak` As shown in the
-`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+level / carrier concentration heatmap plots from `doped`. Automated plots of **
+(i,j)** single-particle eigenvalues and **(k)** site displacements from DFT
+supercell calculations. See the [JOSS paper](https://github.com/openjournals/
+joss-reviews/issues/6433) for more details. ## Installation ```bash pip install
+doped # install doped and dependencies ``` Alternatively if desired, `doped`
+can also be installed from `conda` with: ```bash conda install -c conda-forge
+doped pip install pydefect # pydefect not available on conda, so needs to be
+installed with pip or otherwise, if using the eFNV correction ``` If you
+haven't done so already, you will need to set up your VASP `POTCAR` files and
+`Materials Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order
+for `doped` to automatically generate VASP input files for defect calculations
+and determine competing phases for chemical potentials. See the docs
+[Installation](https://doped.readthedocs.io/en/latest/Installation.html) page
+for details on this. ## `ShakeNBreak` As shown in the `doped` tutorials, it is
+highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.0/README.md` & `doped-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 - **Thermodynamic Analysis**: Compute (non-)equilibrium Fermi levels, defect/carrier concentrations etc. as functions of annealing/cooling temperature, chemical potentials etc.
 - **Plotting**: Generate publication-quality plots of defect formation energies, chemical potential limits, defect/carrier concentrations, Fermi levels, charge corrections, etc.
 - **`Python` Interface**: Fully-customisable, modular `Python` API. Plug-and-play w/[`ShakeNBreak`](https://shakenbreak.readthedocs.io) – [defect structure-searching](https://www.nature.com/articles/s41524-023-00973-1), [`easyunfold`](https://smtg-bham.github.io/easyunfold/) – band unfolding, [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/[`nonrad`](https://nonrad.readthedocs.io/en/latest/) – non-radiative recombination etc.
 - Reproducibility, tabulation, automated compatibility/sanity checking, strain/displacement analysis, shallow defect analysis, high-throughput compatibility, Wyckoff analysis...
 
 ### Performance and Example Outputs
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
-**a.** Optimal supercell generation comparison. **b.** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
+**(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
+displacements from DFT supercell calculations. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
 <!-- Update this link!! -->
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
 ```
```

#### html2text {}

```diff
@@ -36,32 +36,34 @@
 (https://smtg-bham.github.io/easyunfold/) â band unfolding,
 [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/
 [`nonrad`](https://nonrad.readthedocs.io/en/latest/) â non-radiative
 recombination etc. - Reproducibility, tabulation, automated compatibility/
 sanity checking, strain/displacement analysis, shallow defect analysis, high-
 throughput compatibility, Wyckoff analysis... ### Performance and Example
 Outputs ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/
-doped_JOSS_figure.png) **a.** Optimal supercell generation comparison. **b.**
+doped_JOSS_figure.png) **(a)** Optimal supercell generation comparison. **(b)**
 Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-
 size correction plot, **(d)** defect formation energy diagram, **(e)** chemical
 potential / stability region, **(f)** Fermi level vs. annealing temperature, **
 (g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi
-level / carrier concentration heatmap plots from `doped`. See the [JOSS paper]
-(https://github.com/openjournals/joss-reviews/issues/6433) for more details. ##
-Installation ```bash pip install doped # install doped and dependencies ```
-Alternatively if desired, `doped` can also be installed from `conda` with:
-```bash conda install -c conda-forge doped pip install pydefect # pydefect not
-available on conda, so needs to be installed with pip or otherwise, if using
-the eFNV correction ``` If you haven't done so already, you will need to set up
-your VASP `POTCAR` files and `Materials Project` API with `pymatgen` using the
-`.pmgrc.yaml` file, in order for `doped` to automatically generate VASP input
-files for defect calculations and determine competing phases for chemical
-potentials. See the docs [Installation](https://doped.readthedocs.io/en/latest/
-Installation.html) page for details on this. ## `ShakeNBreak` As shown in the
-`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+level / carrier concentration heatmap plots from `doped`. Automated plots of **
+(i,j)** single-particle eigenvalues and **(k)** site displacements from DFT
+supercell calculations. See the [JOSS paper](https://github.com/openjournals/
+joss-reviews/issues/6433) for more details. ## Installation ```bash pip install
+doped # install doped and dependencies ``` Alternatively if desired, `doped`
+can also be installed from `conda` with: ```bash conda install -c conda-forge
+doped pip install pydefect # pydefect not available on conda, so needs to be
+installed with pip or otherwise, if using the eFNV correction ``` If you
+haven't done so already, you will need to set up your VASP `POTCAR` files and
+`Materials Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order
+for `doped` to automatically generate VASP input files for defect calculations
+and determine competing phases for chemical potentials. See the docs
+[Installation](https://doped.readthedocs.io/en/latest/Installation.html) page
+for details on this. ## `ShakeNBreak` As shown in the `doped` tutorials, it is
+highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.0/doped/VASP_sets/DefectSet.yaml` & `doped-2.4.1/doped/VASP_sets/DefectSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/VASP_sets/HSESet.yaml` & `doped-2.4.1/doped/VASP_sets/HSESet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/VASP_sets/PotcarSet.yaml` & `doped-2.4.1/doped/VASP_sets/PotcarSet.yaml`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/VASP_sets/RelaxSet.yaml` & `doped-2.4.1/doped/VASP_sets/RelaxSet.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 INCAR:
   '# May want to change NCORE, KPAR, AEXX, ENCUT, IBRION, LREAL, NUPDOWN, ISPIN, MAGMOM': 'Typical variable parameters'
-  ALGO: "Normal  # Change to All if ZHEGV, FEXCP/F or ZBRENT errors encountered"
+  ALGO: "Normal  # Change to All if ZHEGV, FEXCP/F or ZBRENT errors encountered, or poor electronic convergence"
   EDIFF_PER_ATOM: 2.0e-07  # capped at a max EDIFF of 1e-4 for large supercells (N(atoms) > 500)
   EDIFFG: -0.01
   ENCUT: 300
   GGA: PS  # switched to PE (PBE) for hybrid DFT (HSE/PBE0) calculations
   IBRION: '2  # Typically more stable/reliable than "1" (RMM-DIIS), but change if ionic convergence is poor'
   ICHARG: 1
   ISIF: 3  # changed to 2 (fixed cell) for defect calculations, see DefectSet.yaml
```

### Comparing `doped-2.4.0/doped/__init__.py` & `doped-2.4.1/doped/__init__.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/analysis.py` & `doped-2.4.1/doped/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -399,16 +399,17 @@
             if structure matching with the relaxed defect structure(s) fails (rare).
             Default is None.
         skip_corrections (bool):
             Whether to skip the calculation and application of finite-size charge
             corrections to the defect energy (not recommended in most cases).
             Default = False.
         error_tolerance (float):
-            If the estimated error in the defect charge correction is greater
-            than this value (in eV), then a warning is raised. (default: 0.05 eV)
+            If the estimated error in the defect charge correction, based on the
+            variance of the potential in the sampling region is greater than this
+            value (in eV), then a warning is raised. (default: 0.05 eV)
         bulk_band_gap_path (str):
             Path to bulk OUTCAR file for determining the band gap. If the VBM/CBM
             occur at reciprocal space points not included in the bulk supercell
             calculation, you should use this tag to point to a bulk bandstructure
             calculation instead. Alternatively, you can edit/add the "gap" and "vbm"
             entries in self.defect_entry.calculation_metadata to match the correct
             (eigen)values.
@@ -507,15 +508,16 @@
                 ``output_path`` directory (matching the default ``doped`` name for
                 the bulk supercell reference folder).
             skip_corrections (bool):
                 Whether to skip the calculation & application of finite-size charge
                 corrections to the defect energies (not recommended in most cases).
                 Default = False.
             error_tolerance (float):
-                If the estimated error in any charge correction is greater than
+                If the estimated error in any charge correction, based on the
+                variance of the potential in the sampling region, is greater than
                 this value (in eV), then a warning is raised. (default: 0.05 eV)
             bulk_band_gap_path (str):
                 Path to bulk OUTCAR file for determining the band gap. If the
                 VBM/CBM occur at reciprocal space points not included in the bulk
                 supercell calculation, you should use this tag to point to a bulk
                 band structure calculation instead. Alternatively, you can edit/add
                 the "gap" and "vbm" entries in
@@ -583,14 +585,35 @@
                 "vasprun" in file and ".xml" in file
                 for file_list in [tup[2] for tup in os.walk(os.path.join(self.output_path, dir))]
                 for file in file_list
             )
             and dir not in (self.bulk_path.split("/") if self.bulk_path else [])
         ]
 
+        if not possible_defect_folders:  # user may have specified the defect folder directly, so check
+            # if we can dynamically determine the defect folder:
+            possible_defect_folders = [
+                dir
+                for dir in os.listdir(os.path.join(self.output_path, os.pardir))
+                if any(
+                    "vasprun" in file and ".xml" in file
+                    for file_list in [
+                        tup[2] for tup in os.walk(os.path.join(self.output_path, os.pardir, dir))
+                    ]
+                    for file in file_list
+                )
+                and (
+                    os.path.basename(self.output_path) in dir  # only that defect directory
+                    or "bulk" in str(dir).lower()  # or a bulk directory, for later
+                )
+                and dir not in (self.bulk_path.split("/") if self.bulk_path else [])
+            ]
+            if possible_defect_folders:  # update output path (otherwise will crash with informative error)
+                self.output_path = os.path.join(self.output_path, os.pardir)
+
         if self.subfolder is None:  # determine subfolder to use
             vasp_subfolders = [
                 subdir
                 for possible_defect_folder in possible_defect_folders
                 for subdir in os.listdir(os.path.join(self.output_path, possible_defect_folder))
                 if os.path.isdir(os.path.join(self.output_path, possible_defect_folder, subdir))
                 and "vasp_" in subdir
@@ -662,44 +685,24 @@
             _multiple_files_warning(
                 "vasprun.xml",
                 self.bulk_path,
                 bulk_vr_path,
                 dir_type="bulk",
             )
 
-        self.bulk_procar = None
-        bulk_vr_exc = None
-
-        try:
-            self.bulk_vr = get_vasprun(
-                bulk_vr_path, parse_projected_eigen=parse_projected_eigen is not False
-            )
-        except Exception as exc:
-            bulk_vr_exc = exc  # don't throw unless PROCAR also fails
-            self.bulk_vr = get_vasprun(bulk_vr_path, parse_projected_eigen=False)
-
-        if parse_projected_eigen is not False and self.bulk_vr.projected_eigenvalues is None:
-            # Checking if PROCAR available:
-            bulk_procar_path, multiple = _get_output_files_and_check_if_multiple("PROCAR", self.bulk_path)
-            if "PROCAR" in bulk_procar_path:
-                try:
-                    self.bulk_procar = get_procar(bulk_procar_path)
-
-                except Exception as procar_exc:
-                    if parse_projected_eigen is not None:  # otherwise no warning
-                        warning_message = (
-                            f"Could not parse vasprun.xml.gz files in bulk folder at {self.bulk_path}, "
-                            f"got error:\n{bulk_vr_exc}\nThen got "
-                            if bulk_vr_exc
-                            else "Got "
-                        )
-                        warnings.warn(
-                            f"{warning_message}the following error when attempting to parse projected "
-                            f"eigenvalues from the bulk PROCAR(.gz):\n{procar_exc}"
-                        )
+        self.bulk_vr, self.bulk_procar = _parse_vr_and_poss_procar(
+            bulk_vr_path,
+            parse_projected_eigen=self.parse_projected_eigen,
+            output_path=self.bulk_path,
+            label="bulk",
+            parse_procar=True,
+        )
+        self.parse_projected_eigen = (
+            self.bulk_vr.projected_eigenvalues is not None or self.bulk_procar is not None
+        )
 
         # try parsing the bulk oxidation states first, for later assigning defect "oxi_state"s (i.e.
         # fully ionised charge states):
         if _rough_oxi_state_cost_from_comp(self.bulk_vr.final_structure.composition) > 1e6:
             self._bulk_oxi_states: Union[dict, bool] = False  # will take very long to guess oxi_state
         else:
             queue: Queue = Queue()
@@ -1013,20 +1016,28 @@
             ):
                 eFNV_correction_errors.append(
                     (name, defect_entry.corrections_metadata["kumagai_charge_correction_error"])
                 )
 
         def _call_multiple_corrections_tolerance_warning(correction_errors, type="FNV"):
             long_name = "Freysoldt" if type == "FNV" else "Kumagai"
-            correction_errors_string = "\n".join(
-                f"{name}: {error:.3f} eV" for name, error in correction_errors
-            )
+            if error_tolerance >= 0.01:  # if greater than 10 meV, round energy values to meV:
+                error_tol_string = f"{error_tolerance:.3f}"
+                correction_errors_string = "\n".join(
+                    f"{name}: {error:.3f} eV" for name, error in correction_errors
+                )
+            else:  # else give in scientific notation:
+                error_tol_string = f"{error_tolerance:.2e}"
+                correction_errors_string = "\n".join(
+                    f"{name}: {error:.2e} eV" for name, error in correction_errors
+                )
+
             warnings.warn(
                 f"Estimated error in the {long_name} ({type}) charge correction for certain "
-                f"defects is greater than the `error_tolerance` (= {error_tolerance:.3f} eV):"
+                f"defects is greater than the `error_tolerance` (= {error_tol_string} eV):"
                 f"\n{correction_errors_string}\n"
                 f"You may want to check the accuracy of the corrections by plotting the site "
                 f"potential differences (using `defect_entry.get_{long_name.lower()}_correction()`"
                 f" with `plot=True`). Large errors are often due to unstable or shallow defect "
                 f"charge states (which can't be accurately modelled with the supercell "
                 f"approach). If these errors are not acceptable, you may need to use a larger "
                 f"supercell for more accurate energies."
@@ -1324,46 +1335,100 @@
         return (
             f"doped DefectsParser for bulk composition {formula}, with {len(self.defect_dict)} parsed "
             f"defect entries in self.defect_dict. Available attributes:\n{properties}\n\n"
             f"Available methods:\n{methods}"
         )
 
 
+def _parse_vr_and_poss_procar(
+    vr_path: str,
+    parse_projected_eigen: Optional[bool] = None,
+    output_path: Optional[str] = None,
+    label: str = "bulk",
+    parse_procar: bool = True,
+):
+    procar = None
+
+    failed_eig_parsing_warning_message = (
+        f"Could not parse eigenvalue data from vasprun.xml.gz files in {label} folder at {output_path}"
+    )
+
+    try:
+        vr = get_vasprun(
+            vr_path,
+            parse_projected_eigen=parse_projected_eigen is not False,
+            parse_eigen=(parse_projected_eigen is not False or label == "bulk"),
+        )  # vr.eigenvalues not needed for defects except for vr-only eigenvalue analysis
+    except Exception as vr_exc:
+        vr = get_vasprun(vr_path, parse_projected_eigen=False, parse_eigen=label == "bulk")
+        failed_eig_parsing_warning_message += f", got error:\n{vr_exc}"
+
+        if parse_procar:
+            procar_path, multiple = _get_output_files_and_check_if_multiple("PROCAR", output_path)
+            if "PROCAR" in procar_path and parse_projected_eigen is not False:
+                try:
+                    procar = get_procar(procar_path)
+
+                except Exception as procar_exc:
+                    failed_eig_parsing_warning_message += (
+                        f"\nThen got the following error when attempting to parse projected eigenvalues "
+                        f"from the defect PROCAR(.gz):\n{procar_exc}"
+                    )
+
+    if vr.projected_eigenvalues is None and procar is None and parse_projected_eigen is True:
+        # only warn if parse_projected_eigen is set to True (not None)
+        warnings.warn(failed_eig_parsing_warning_message)
+
+    return vr, procar if parse_procar else vr
+
+
 class DefectParser:
     def __init__(
         self,
         defect_entry: DefectEntry,
         defect_vr: Optional[Vasprun] = None,
         bulk_vr: Optional[Vasprun] = None,
         skip_corrections: bool = False,
         error_tolerance: float = 0.05,
+        parse_projected_eigen: Optional[bool] = None,
         **kwargs,
     ):
         """
-        Create a DefectParser object, which has methods for parsing the results
-        of defect supercell calculations.
+        Create a ``DefectParser`` object, which has methods for parsing the
+        results of defect supercell calculations.
 
-        Direct initiation with DefectParser() is typically not recommended. Rather
-        DefectParser.from_paths() or defect_entry_from_paths() are preferred as
+        Direct initiation with ``DefectParser()`` is typically not recommended. Rather
+        ``DefectParser.from_paths()`` or ``defect_entry_from_paths()`` are preferred as
         shown in the doped parsing tutorials.
 
         Args:
             defect_entry (DefectEntry):
-                doped DefectEntry
+                doped ``DefectEntry``
             defect_vr (Vasprun):
-                pymatgen Vasprun object for the defect supercell calculation
+                ``pymatgen`` ``Vasprun`` object for the defect supercell calculation
             bulk_vr (Vasprun):
-                pymatgen Vasprun object for the reference bulk supercell calculation
+                ``pymatgen`` ``Vasprun`` object for the reference bulk supercell calculation
             skip_corrections (bool):
                 Whether to skip calculation and application of finite-size charge
                 corrections to the defect energy (not recommended in most cases).
                 Default = False.
             error_tolerance (float):
-                If the estimated error in the defect charge correction is greater
-                than this value (in eV), then a warning is raised. (default: 0.05 eV)
+                If the estimated error in the defect charge correction, based on the
+                variance of the potential in the sampling region is greater than this
+                value (in eV), then a warning is raised. (default: 0.05 eV)
+            parse_projected_eigen (bool):
+                Whether to parse the projected eigenvalues & orbitals from the bulk and
+                defect calculations (so ``DefectEntry.get_eigenvalue_analysis()`` can
+                then be used with no further parsing). Will initially try to load orbital
+                projections from ``vasprun.xml(.gz)`` files (slightly slower but more
+                accurate), or failing that from ``PROCAR(.gz)`` files if present in the
+                bulk/defect directories. Parsing this data can increase total parsing time
+                by anywhere from ~5-25%, so set to ``False`` if parsing speed is crucial.
+                Default is ``None``, which will attempt to load this data but with no
+                warning if it fails (otherwise if ``True`` a warning will be printed).
             **kwargs:
                 Keyword arguments to pass to ``DefectParser()`` methods
                 (``load_FNV_data()``, ``load_eFNV_data()``, ``load_bulk_gap_data()``)
                 ``point_symmetry_from_defect_entry()`` or ``defect_from_structures``,
                 including ``bulk_locpot_dict``, ``bulk_site_potentials``, ``use_MP``,
                 ``mpid``, ``api_key``, ``symprec`` or ``oxi_state``. Primarily used by
                 ``DefectsParser`` to expedite parsing by avoiding reloading bulk data
@@ -1371,14 +1436,15 @@
         """
         self.defect_entry: DefectEntry = defect_entry
         self.defect_vr = defect_vr
         self.bulk_vr = bulk_vr
         self.skip_corrections = skip_corrections
         self.error_tolerance = error_tolerance
         self.kwargs = kwargs or {}
+        self.parse_projected_eigen = parse_projected_eigen
 
     @classmethod
     def from_paths(
         cls,
         defect_path: str,
         bulk_path: Optional[str] = None,
         bulk_vr: Optional[Vasprun] = None,
@@ -1431,16 +1497,17 @@
                 if structure matching with the relaxed defect structure(s) fails (rare).
                 Default is ``None``.
             skip_corrections (bool):
                 Whether to skip the calculation and application of finite-size charge
                 corrections to the defect energy (not recommended in most cases).
                 Default = ``False``.
             error_tolerance (float):
-                If the estimated error in the defect charge correction is greater
-                than this value (in eV), then a warning is raised. (default: 0.05 eV)
+                If the estimated error in the defect charge correction, based on the
+                variance of the potential in the sampling region, is greater than this
+                value (in eV), then a warning is raised. (default: 0.05 eV)
             bulk_band_gap_path (str):
                 Path to bulk ``OUTCAR`` file for determining the band gap. If the
                 VBM/CBM occur at reciprocal space points not included in the bulk
                 supercell calculation, you should use this tag to point to a bulk
                 band structure calculation instead. Alternatively, you can edit/add the
                 "gap"/"vbm" entries in ``DefectParser.defect_entry.calculation_metadata``
                 to match the correct eigenvalues.
@@ -1481,15 +1548,24 @@
             if multiple:
                 _multiple_files_warning(
                     "vasprun.xml",
                     bulk_path,
                     bulk_vr_path,
                     dir_type="bulk",
                 )
-            bulk_vr = get_vasprun(bulk_vr_path)
+            bulk_vr, reparsed_bulk_procar = _parse_vr_and_poss_procar(
+                bulk_vr_path,
+                parse_projected_eigen,
+                bulk_path,
+                label="bulk",
+                parse_procar=bulk_procar is None,
+            )
+            if bulk_procar is None and reparsed_bulk_procar is not None:
+                bulk_procar = reparsed_bulk_procar
+            parse_projected_eigen = bulk_vr.projected_eigenvalues is not None or bulk_procar is not None
 
         elif bulk_vr is None:
             raise ValueError("Either `bulk_path` or `bulk_vr` must be provided!")
         bulk_supercell = bulk_vr.final_structure.copy()
 
         # add defect simple properties
         (
@@ -1500,49 +1576,29 @@
             _multiple_files_warning(
                 "vasprun.xml",
                 defect_path,
                 defect_vr_path,
                 dir_type="defect",
             )
 
-        defect_procar = None
-        try:
-            defect_vr = get_vasprun(
-                defect_vr_path,
-                parse_projected_eigen=parse_projected_eigen is not False,
-                parse_eigen=parse_projected_eigen is not False,
-            )  # vr.eigenvalues not needed for defects except for vr-only eigenvalue analysis
-        except Exception as defect_vr_exc:
-            defect_vr = get_vasprun(defect_vr_path, parse_projected_eigen=False, parse_eigen=False)
-            defect_procar_path, multiple = _get_output_files_and_check_if_multiple("PROCAR", defect_path)
-            if "PROCAR" in defect_procar_path and parse_projected_eigen is not False:
-                try:
-                    defect_procar = get_procar(defect_procar_path)
-
-                except Exception as procar_exc:
-                    if parse_projected_eigen is not None:  # otherwise no warning
-                        warning_message = (
-                            f"Could not parse vasprun.xml.gz files in defect folder at {defect_path}, "
-                            f"got error:\n{defect_vr_exc}\nThen got "
-                        )
-                        warnings.warn(
-                            f"{warning_message}the following error when attempting to parse projected "
-                            f"eigenvalues from the defect PROCAR(.gz):\n{procar_exc}"
-                        )
+        defect_vr, defect_procar = _parse_vr_and_poss_procar(
+            defect_vr_path, parse_projected_eigen, defect_path, label="defect"
+        )
+        parse_projected_eigen = defect_procar is not None or defect_vr.projected_eigenvalues is not None
 
         possible_defect_name = os.path.basename(
             defect_path.rstrip("/.").rstrip("/")  # remove any trailing slashes to ensure correct name
         )  # set equal to folder name
         if "vasp" in possible_defect_name:  # get parent directory name:
             possible_defect_name = os.path.basename(os.path.dirname(defect_path))
 
         try:
             parsed_charge_state: int = _defect_charge_from_vasprun(bulk_vr, defect_vr, charge_state)
         except RuntimeError as orig_exc:  # auto charge guessing failed and charge_state not provided,
-            # try determine from folder name - must have "-" or "+" at end of name for this
+            # try to determine from folder name - must have "-" or "+" at end of name for this
             try:
                 charge_state_suffix = possible_defect_name.rsplit("_", 1)[-1]
                 if charge_state_suffix[0] not in ["-", "+"]:
                     raise ValueError(
                         f"Could not guess charge state from folder name ({possible_defect_name}), must "
                         f"end in '_+X' or '_-X' where +/-X is the charge state."
                     )
@@ -1746,27 +1802,28 @@
 
         dp = cls(
             defect_entry,
             defect_vr=defect_vr,
             bulk_vr=bulk_vr,
             skip_corrections=skip_corrections,
             error_tolerance=error_tolerance,
+            parse_projected_eigen=parse_projected_eigen,
             **kwargs,
         )
 
         if parse_projected_eigen is not False:
             try:
                 dp.defect_entry._load_and_parse_eigenvalue_data(
-                    bulk_vr,
-                    bulk_procar,
+                    bulk_vr=bulk_vr,
+                    bulk_procar=bulk_procar,
                     defect_vr=defect_vr,
                     defect_procar=defect_procar,
                 )
             except Exception as exc:
-                if parse_projected_eigen is not None:  # otherwise no warning
+                if parse_projected_eigen is True:  # otherwise no warning
                     warnings.warn(f"Projected eigenvalues/orbitals parsing failed with error: {exc!r}")
 
         defect_vr.projected_eigenvalues = None  # no longer needed, delete to reduce memory demand
         defect_vr.eigenvalues = None  # no longer needed, delete to reduce memory demand
         dp.load_and_check_calculation_metadata()  # Load standard defect metadata
         dp.load_bulk_gap_data(bulk_band_gap_path=bulk_band_gap_path)  # Load band gap data
 
@@ -2062,52 +2119,69 @@
             if multiple:
                 _multiple_files_warning(
                     "vasprun.xml",
                     self.defect_entry.calculation_metadata["bulk_path"],
                     bulk_vr_path,
                     dir_type="bulk",
                 )
-            self.bulk_vr = get_vasprun(bulk_vr_path)
+            self.bulk_vr = _parse_vr_and_poss_procar(
+                bulk_vr_path,
+                parse_projected_eigen=False,  # not needed for DefectEntry metadata
+                label="bulk",
+                parse_procar=False,
+            )
 
         if not self.defect_vr:
             defect_vr_path, multiple = _get_output_files_and_check_if_multiple(
                 "vasprun.xml", self.defect_entry.calculation_metadata["defect_path"]
             )
             if multiple:
                 _multiple_files_warning(
                     "vasprun.xml",
                     self.defect_entry.calculation_metadata["defect_path"],
                     defect_vr_path,
                     dir_type="defect",
                 )
-            self.defect_vr = get_vasprun(defect_vr_path)
+            self.defect_vr = _parse_vr_and_poss_procar(
+                defect_vr_path,
+                parse_projected_eigen=False,  # not needed for DefectEntry metadata
+                label="defect",
+                parse_procar=False,
+            )
+
+        def _get_vr_dict_without_proj_eigenvalues(vr):
+            proj_eigen = vr.projected_eigenvalues
+            vr.projected_eigenvalues = None
+            vr_dict = vr.as_dict()  # only call once
+            vr_dict_wout_proj = {  # projected eigenvalue data might be present, but not needed (v slow
+                # and data-heavy)
+                **{k: v for k, v in vr_dict.items() if k != "output"},
+                "output": {
+                    k: v
+                    for k, v in vr_dict["output"].items()
+                    if k != "projected_eigenvalues"  # reduce memory demand
+                },
+            }
+            vr_dict_wout_proj["output"]["projected_eigenvalues"] = None
+            vr.projected_eigenvalues = proj_eigen  # reset to original value
+            return vr_dict_wout_proj
 
         run_metadata = {
             # incars need to be as dict without module keys otherwise not JSONable:
             "defect_incar": {k: v for k, v in self.defect_vr.incar.as_dict().items() if "@" not in k},
             "bulk_incar": {k: v for k, v in self.bulk_vr.incar.as_dict().items() if "@" not in k},
             "defect_kpoints": self.defect_vr.kpoints,
             "bulk_kpoints": self.bulk_vr.kpoints,
             "defect_actual_kpoints": self.defect_vr.actual_kpoints,
             "bulk_actual_kpoints": self.bulk_vr.actual_kpoints,
             "defect_potcar_symbols": self.defect_vr.potcar_spec,
             "bulk_potcar_symbols": self.bulk_vr.potcar_spec,
-            "defect_vasprun_dict": self.defect_vr.as_dict(),  # projected_eigenvalues already removed
-            "bulk_vasprun_dict": {
-                **{  # projected_eigenvalues may not yet be removed
-                    k: v for k, v in self.bulk_vr.as_dict().items() if k != "output"
-                },
-                "output": {
-                    k: v
-                    for k, v in self.bulk_vr.as_dict()["output"].items()
-                    if k != "projected_eigenvalues"
-                },
-            },
+            "defect_vasprun_dict": _get_vr_dict_without_proj_eigenvalues(self.defect_vr),
+            "bulk_vasprun_dict": _get_vr_dict_without_proj_eigenvalues(self.bulk_vr),
         }
-        run_metadata["bulk_vasprun_dict"]["output"]["projected_eigenvalues"] = None  # reduce memory demand
 
         self.defect_entry.calculation_metadata["mismatching_INCAR_tags"] = _compare_incar_tags(
             run_metadata["bulk_incar"], run_metadata["defect_incar"]
         )
         self.defect_entry.calculation_metadata["mismatching_POTCAR_symbols"] = _compare_potcar_symbols(
             run_metadata["bulk_potcar_symbols"], run_metadata["defect_potcar_symbols"]
         )
@@ -2118,49 +2192,55 @@
             run_metadata["defect_kpoints"],
         )
 
         self.defect_entry.calculation_metadata.update({"run_metadata": run_metadata.copy()})
 
     def load_bulk_gap_data(self, bulk_band_gap_path=None, use_MP=False, mpid=None, api_key=None):
         """
-        Get bulk band gap data from bulk OUTCAR file, or OUTCAR located at
-        ``actual_bulk_path``.
+        Get bulk band gap data from a bulk ``vasprun.xml(.gz)`` file located
+        in/at ``bulk_band_gap_path``.
 
         Alternatively, one can specify query the Materials Project (MP) database
         for the bulk gap data, using ``use_MP = True``, in which case the MP entry
         with the lowest number ID and composition matching the bulk will be used,
         or the MP ID (mpid) of the bulk material to use can be specified. This is
         not recommended as it will correspond to a severely-underestimated GGA DFT
         bandgap!
 
         Args:
             bulk_band_gap_path (str):
-                Path to bulk OUTCAR file for determining the band gap. If the VBM/CBM
-                occur at reciprocal space points not included in the bulk supercell
-                calculation, you should use this tag to point to a bulk bandstructure
-                calculation instead. If None, will use
-                self.defect_entry.calculation_metadata["bulk_path"].
+                Path to bulk ``vasprun.xml(.gz)`` file for determining the band gap.
+                If the VBM/CBM occur at reciprocal space points not included in the bulk
+                supercell calculation, you should use this tag to point to a bulk
+                band-structure calculation instead. If None, will use
+                ``self.defect_entry.calculation_metadata["bulk_path"]``.
             use_MP (bool):
                 If True, will query the Materials Project database for the bulk gap data.
             mpid (str):
                 If provided, will query the Materials Project database for the bulk gap
                 data, using this Materials Project ID.
-            api_key (str): Materials API key to access database.
+            api_key (str):
+                Materials API key to access database.
         """
         if not self.bulk_vr:
             bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
                 "vasprun.xml", self.defect_entry.calculation_metadata["bulk_path"]
             )
             if multiple:
                 warnings.warn(
                     f"Multiple `vasprun.xml` files found in bulk directory: "
                     f"{self.defect_entry.calculation_metadata['bulk_path']}. Using "
                     f"{os.path.basename(bulk_vr_path)} to {_vasp_file_parsing_action_dict['vasprun.xml']}."
                 )
-            self.bulk_vr = get_vasprun(bulk_vr_path)
+            self.bulk_vr = _parse_vr_and_poss_procar(
+                bulk_vr_path,
+                parse_projected_eigen=self.parse_projected_eigen,
+                label="bulk",
+                parse_procar=False,
+            )
 
         bulk_sc_structure = self.bulk_vr.initial_structure
 
         band_gap, cbm, vbm, _ = self.bulk_vr.eigenvalue_band_properties
         gap_calculation_metadata = {}
 
         use_MP = use_MP or self.kwargs.get("use_MP", False)
@@ -2229,26 +2309,25 @@
             warnings.warn(
                 f"MPID {mpid} was provided, but no bandstructure entry currently exists for it. "
                 f"Reverting to use of bulk supercell calculation for band edge extrema."
             )
             gap_calculation_metadata["MP_gga_BScalc_data"] = None  # to signal no MP BS is used
 
         if bulk_band_gap_path:
-            print(f"Using actual bulk path: {bulk_band_gap_path}")
-            actual_bulk_vr_path, multiple = _get_output_files_and_check_if_multiple(
+            bulk_gap_vr_path, multiple = _get_output_files_and_check_if_multiple(
                 "vasprun.xml", bulk_band_gap_path
             )
             if multiple:
                 warnings.warn(
                     f"Multiple `vasprun.xml` files found in specified directory: "
-                    f"{bulk_band_gap_path}. Using {os.path.basename(actual_bulk_vr_path)} to "
+                    f"{bulk_band_gap_path}. Using {os.path.basename(bulk_gap_vr_path)} to "
                     f"{_vasp_file_parsing_action_dict['vasprun.xml']}."
                 )
-            actual_bulk_vr = get_vasprun(actual_bulk_vr_path)
-            band_gap, cbm, vbm, _ = actual_bulk_vr.eigenvalue_band_properties
+            bulk_gap_vr = get_vasprun(bulk_gap_vr_path, parse_projected_eigen=False)
+            band_gap, cbm, vbm, _ = bulk_gap_vr.eigenvalue_band_properties
 
         gap_calculation_metadata = {
             "mpid": mpid,
             "cbm": cbm,
             "vbm": vbm,
             "gap": band_gap,
         }
```

### Comparing `doped-2.4.0/doped/chemical_potentials.py` & `doped-2.4.1/doped/chemical_potentials.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,55 +172,58 @@
         elemental (dict): Dictionary of elemental reference energies.
 
     Returns:
         pd.DataFrame: DataFrame formation energies of the input phases.
     """
     for d in data:
         for el in elemental:
-            d[el] = Composition(d["formula"]).as_dict().get(el, 0)
+            d[el] = Composition(d["Formula"]).as_dict().get(el, 0)
 
     formation_energy_df = pd.DataFrame(data)
-    formation_energy_df["num_atoms_in_fu"] = formation_energy_df["formula"].apply(
+    formation_energy_df["num_atoms_in_fu"] = formation_energy_df["Formula"].apply(
         lambda x: Composition(x).num_atoms
     )
-    formation_energy_df["num_species"] = formation_energy_df["formula"].apply(
+    formation_energy_df["num_species"] = formation_energy_df["Formula"].apply(
         lambda x: len(Composition(x).as_dict())
     )
 
     # get energy per fu then subtract elemental energies later, to get formation energies
-    if "energy_per_fu" in formation_energy_df.columns:
-        formation_energy_df["formation_energy_calc"] = formation_energy_df["energy_per_fu"]
-        if "energy_per_atom" not in formation_energy_df.columns:
-            formation_energy_df["energy_per_atom"] = formation_energy_df["energy_per_fu"] / (
+    if "DFT Energy (eV/fu)" in formation_energy_df.columns:
+        formation_energy_df["formation_energy_calc"] = formation_energy_df["DFT Energy (eV/fu)"]
+        if "DFT Energy (eV/atom)" not in formation_energy_df.columns:
+            formation_energy_df["DFT Energy (eV/atom)"] = formation_energy_df["DFT Energy (eV/fu)"] / (
                 formation_energy_df["num_atoms_in_fu"]
             )
 
-    elif "energy_per_atom" in formation_energy_df.columns:
+    elif "DFT Energy (eV/atom)" in formation_energy_df.columns:
         formation_energy_df["formation_energy_calc"] = (
-            formation_energy_df["energy_per_atom"] * formation_energy_df["num_atoms_in_fu"]
+            formation_energy_df["DFT Energy (eV/atom)"] * formation_energy_df["num_atoms_in_fu"]
         )
-        formation_energy_df["energy_per_fu"] = formation_energy_df["energy_per_atom"] * (
+        formation_energy_df["DFT Energy (eV/fu)"] = formation_energy_df["DFT Energy (eV/atom)"] * (
             formation_energy_df["num_atoms_in_fu"]
         )
 
     else:
         raise ValueError(
-            "No energy data (energy_per_atom or energy_per_fu) found in input data to calculate "
-            "formation energies!"
+            "No energy data (DFT Energy (eV/atom) or per Formula Unit (eV/fu)) found in input "
+            "data to calculate formation energies!"
         )
 
     for k, v in elemental.items():
         formation_energy_df["formation_energy_calc"] -= formation_energy_df[k] * v
 
-    formation_energy_df["formation_energy"] = formation_energy_df["formation_energy_calc"]
+    formation_energy_df["Formation Energy (eV/fu)"] = formation_energy_df["formation_energy_calc"]
+    formation_energy_df["Formation Energy (eV/atom)"] = (
+        formation_energy_df["formation_energy_calc"] / formation_energy_df["num_atoms_in_fu"]
+    )
     formation_energy_df = formation_energy_df.drop(columns=["formation_energy_calc"])
 
     # sort by num_species, then alphabetically, then by num_atoms_in_fu, then by formation_energy
     formation_energy_df = formation_energy_df.sort_values(
-        by=["num_species", "formula", "num_atoms_in_fu", "formation_energy"],
+        by=["num_species", "Formula", "num_atoms_in_fu", "Formation Energy (eV/fu)"],
     )
     # drop num_atoms_in_fu and num_species
     return formation_energy_df.drop(columns=["num_atoms_in_fu", "num_species"])
 
 
 def _renormalise_entry(entry, renormalisation_energy_per_atom):
     """
@@ -547,15 +550,16 @@
                 dict_set.user_kpoints_settings = {"reciprocal_density": kpoint}
                 kname = (
                     "k"
                     + ("_" * (dict_set.kpoints.kpts[0][0] // 10))
                     + ",".join(str(k) for k in dict_set.kpoints.kpts[0])
                 )
                 fname = f"competing_phases/{self._competing_phase_name(e)}/kpoint_converge/{kname}"
-                # TODO: competing_phases folder name should be an optional parameter
+                # TODO: competing_phases folder name should be an optional parameter, and rename default
+                #  to something that isn't so ugly? CompetingPhases?
                 # TODO: Naming should be done in __init__ to ensure consistency and efficiency. Watch
                 #  out for cases where rounding can give same name (e.g. Te!) - should use
                 #  {formula}_MP_{mpid}_EaH_{round(e_above_hull,4)} as naming convention, to prevent any
                 #  rare cases of overwriting
                 dict_set.write_input(fname, **kwargs)
 
         for e in self.metals:
@@ -1260,81 +1264,91 @@
                         self.elemental.append(el)
 
                 elif v["output"]["final_energy_per_atom"] < self.elemental_energies[el]:
                     # only include lowest energy elemental polymorph
                     self.elemental_energies[el] = v["output"]["final_energy_per_atom"]
 
             d = {
-                "formula": v["pretty_formula"],
-                "kpoints": kpoints,
-                "energy_per_fu": final_energy / formulas_per_unit,
-                "energy_per_atom": v["output"]["final_energy_per_atom"],
-                "energy": final_energy,
+                "Formula": v["pretty_formula"],
+                "k-points": kpoints,
+                "DFT Energy (eV/fu)": final_energy / formulas_per_unit,
+                "DFT Energy (eV/atom)": v["output"]["final_energy_per_atom"],
+                "DFT Energy (eV)": final_energy,
             }
             temp_data.append(d)
 
         formation_energy_df = _calculate_formation_energies(temp_data, self.elemental_energies)
         self.data = formation_energy_df.to_dict(orient="records")
         self.formation_energy_df = pd.DataFrame(self._get_and_sort_formation_energy_data())  # sort data
+        self.formation_energy_df.set_index("Formula")
 
         if csv_path is not None:
             self.to_csv(csv_path)
 
     def _get_and_sort_formation_energy_data(self, sort_by_energy=False, prune_polymorphs=False):
         data = copy.deepcopy(self.data)
 
         if prune_polymorphs:  # only keep the lowest energy polymorphs
             formation_energy_df = _calculate_formation_energies(data, self.elemental_energies)
-            indices = formation_energy_df.groupby("formula")["energy_per_atom"].idxmin()
+            indices = formation_energy_df.groupby("Formula")["DFT Energy (eV/atom)"].idxmin()
             pruned_df = formation_energy_df.loc[indices]
             data = pruned_df.to_dict(orient="records")
 
         if sort_by_energy:
-            data = sorted(data, key=lambda x: x["formation_energy"], reverse=True)
+            data = sorted(data, key=lambda x: x["Formation Energy (eV/fu)"], reverse=True)
 
         # moves the bulk composition to the top of the list
-        _move_dict_to_start(data, "formula", self.bulk_composition.reduced_formula)
+        _move_dict_to_start(data, "Formula", self.bulk_composition.reduced_formula)
 
         # for each dict in data list, sort the keys as formula, formation_energy, energy_per_atom,
         # energy_per_fu, energy, kpoints, then by order of appearance in bulk_composition dict,
         # then alphabetically for any remaining:
-        data = [
+        copied_data = copy.deepcopy(data)
+        formation_energy_data = [
             {
-                "formula": d["formula"],
-                "formation_energy": d["formation_energy"],
-                "energy_per_atom": d["energy_per_atom"],
-                "energy_per_fu": d["energy_per_fu"],
-                "energy": d.get("energy"),
-                "kpoints": d.get("kpoints"),
+                **{
+                    k: d.pop(k, None)
+                    for k in [
+                        "Formula",
+                        "Formation Energy (eV/fu)",
+                        "Formation Energy (eV/atom)",
+                        "DFT Energy (eV/atom)",
+                        "DFT Energy (eV/fu)",
+                        "DFT Energy (eV)",
+                        "k-points",
+                    ]
+                },
                 **{  # num elts columns, sorted by order of occurrence in bulk composition:
-                    str(elt): d.get(str(elt))
+                    str(elt): d.pop(str(elt), None)
                     for elt in sorted(
                         self.bulk_composition.elements,
                         key=lambda x: self.bulk_composition.reduced_formula.index(str(x)),
                     )
                 },
                 **{
                     k: v
                     for k, v in d.items()
-                    if k
-                    not in [
-                        "formula",
-                        "formation_energy",
-                        "energy_per_atom",
-                        "energy_per_fu",
-                        "energy",
-                        "kpoints",
-                    ]
+                    if not any(
+                        i in k
+                        for i in [
+                            "Formula",
+                            "Formation Energy",
+                            "DFT Energy",
+                            "k-points",
+                        ]
+                    )
                 },
             }
-            for d in data
+            for d in copied_data
         ]
         # if all values are None for a certain key, remove that key from all dicts in list:
-        keys_to_remove = [k for k in data[0] if all(d[k] is None for d in data)]
-        return [{k: v for k, v in d.items() if k not in keys_to_remove} for d in data]
+        keys_to_remove = [
+            k for k in formation_energy_data[0] if all(d[k] is None for d in formation_energy_data)
+        ]
+        return [{k: v for k, v in d.items() if k not in keys_to_remove} for d in formation_energy_data]
 
     def to_csv(self, csv_path, sort_by_energy=False, prune_polymorphs=False):
         """
         Write parsed competing phases data to ``csv``. Can be re-loaded with
         ``CompetingPhasesAnalyzer.from_csv()``.
 
         Args:
@@ -1345,56 +1359,61 @@
             prune_polymorphs (bool):
                 Whether to only write the lowest energy polymorphs for each composition.
                 Doesn't affect chemical potential limits (only the ground-state
                 polymorphs matter for this).
                 Default is False.
         """
         formation_energy_data = self._get_and_sort_formation_energy_data(sort_by_energy, prune_polymorphs)
-        pd.DataFrame(formation_energy_data).to_csv(csv_path, index=False)
-        print(f"Competing phase formation energies have been saved to {csv_path}.")
+        pd.DataFrame(formation_energy_data).set_index("Formula").to_csv(csv_path)
+        print(f"Competing phase formation energies have been saved to {csv_path}")
 
     def from_csv(self, csv_path):
         """
-        Read in data from csv.
+        Read in data from a previously parsed formation energies csv file.
 
         Args:
-            csv_path (str): Path to csv file. Must have columns 'formula',
-                'energy_per_fu', 'energy' and 'formation_energy'
+            csv_path (str): Path to csv file. Must have columns 'Formula',
+            and 'DFT Energy per Formula Unit (ev/fu)' or
+            'DFT Energy per Atom (ev/atom)'
         Returns:
-            None, sets self.data and self.elemental_energies.
+            None, sets ``self.data`` and ``self.elemental_energies``.
         """
         formation_energy_df = pd.read_csv(csv_path)
-        if "formula" not in list(formation_energy_df.columns) or all(
-            x not in list(formation_energy_df.columns) for x in ["energy_per_fu", "energy_per_atom"]
+        if "Formula" not in list(formation_energy_df.columns) or all(
+            x not in list(formation_energy_df.columns)
+            for x in [
+                "DFT Energy (eV/fu)",
+                "DFT Energy (eV/atom)",
+            ]
         ):
             raise ValueError(
-                "Supplied csv does not contain the minimal columns required ('formula', "
-                "and 'energy_per_fu' or 'energy_per_atom'!"
+                "Supplied csv does not contain the minimal columns required ('Formula', and "
+                "'DFT Energy (eV/fu)' or 'DFT Energy (eV/atom)')"
             )
 
         self.data = formation_energy_df.to_dict(orient="records")
-
         self.elemental_energies = {}
         for i in self.data:
-            c = Composition(i["formula"])
+            c = Composition(i["Formula"])
             if len(c.elements) == 1:
                 el = c.chemical_system
-                if "energy_per_atom" in list(formation_energy_df.columns):
-                    el_energy_per_atom = i["energy_per_atom"]
+                if "DFT Energy (eV/atom)" in list(formation_energy_df.columns):
+                    el_energy_per_atom = i["DFT Energy (eV/atom)"]
                 else:
-                    el_energy_per_atom = i["energy_per_fu"] / c.num_atoms
+                    el_energy_per_atom = i["DFT Energy (eV/fu)"] / c.num_atoms
 
                 if el not in self.elemental_energies or el_energy_per_atom < self.elemental_energies[el]:
                     self.elemental_energies[el] = el_energy_per_atom
 
-        if "formation_energy" not in list(formation_energy_df.columns):
+        if "Formation Energy (eV/fu)" not in list(formation_energy_df.columns):
             formation_energy_df = _calculate_formation_energies(self.data, self.elemental_energies)
             self.data = formation_energy_df.to_dict(orient="records")
 
         self.formation_energy_df = pd.DataFrame(self._get_and_sort_formation_energy_data())  # sort data
+        self.formation_energy_df.set_index("Formula")
 
     def calculate_chempots(self, csv_path=None, verbose=True, sort_by=None):
         """
         Calculates chemical potential limits. For dopant species, it calculates
         the limiting potential based on the intrinsic chemical potentials (i.e.
         same as ``full_sub_approach=False`` in pycdt).
 
@@ -1408,23 +1427,23 @@
         Returns:
             Pandas DataFrame, optionally saved to csv.
         """
         intrinsic_phase_diagram_entries = []
         extrinsic_formation_energies = []
         bulk_pde_list = []
         for d in self.data:
-            e = PDEntry(d["formula"], d["energy_per_fu"])
+            e = PDEntry(d["Formula"], d["DFT Energy (eV/fu)"])
             # checks if the phase is intrinsic
-            if set(Composition(d["formula"]).elements).issubset(self.bulk_composition.elements):
+            if set(Composition(d["Formula"]).elements).issubset(self.bulk_composition.elements):
                 intrinsic_phase_diagram_entries.append(e)
                 if e.composition == self.bulk_composition:  # bulk phase
                     bulk_pde_list.append(e)
             else:
                 extrinsic_formation_energies.append(
-                    {"formula": d["formula"], "formation_energy": d["formation_energy"]}
+                    {k: v for k, v in d.items() if k in ["Formula", "Formation Energy (eV/fu)"]}
                 )
 
         if not bulk_pde_list:
             intrinsic_phase_diagram_compositions = (
                 {e.composition.reduced_formula for e in intrinsic_phase_diagram_entries}
                 if intrinsic_phase_diagram_entries
                 else None
@@ -1479,68 +1498,73 @@
         # get chemical potentials as pandas dataframe
         chemical_potentials = []
         for _, chempot_dict in self._intrinsic_chempots["limits_wrt_el_refs"].items():
             phase_energy_list = []
             phase_name_columns = []
             for k, v in chempot_dict.items():
                 phase_name_columns.append(str(k))
-                phase_energy_list.append(v)
+                phase_energy_list.append(round(v, 4))
             chemical_potentials.append(phase_energy_list)
 
         # make df, will need it in next step
-        chempots_df = pd.DataFrame(chemical_potentials, columns=phase_name_columns)
+        chempots_df = pd.DataFrame(
+            chemical_potentials,
+            index=list(self._intrinsic_chempots["limits_wrt_el_refs"].keys()),
+            columns=phase_name_columns,
+        )
+        chempots_df.index.name = "Limit"
 
         if self.extrinsic_species is not None:
             self._calculate_extrinsic_chempot_lims(  # updates self._chempots
                 extrinsic_formation_energies=extrinsic_formation_energies,
                 chempots_df=chempots_df,
                 verbose=verbose,
             )
         else:  # intrinsic only
             self._chempots = self._intrinsic_chempots
 
         # save and print
         if csv_path is not None:
-            chempots_df.to_csv(csv_path, index=False)
+            chempots_df.to_csv(csv_path)
             if verbose:
                 print("Saved chemical potential limits to csv file: ", csv_path)
 
         if verbose:
-            print("Calculated chemical potential limits: \n")
+            print("Calculated chemical potential limits (in eV wrt elemental reference phases): \n")
             print(chempots_df)
 
         return chempots_df
 
     def _calculate_extrinsic_chempot_lims(self, extrinsic_formation_energies, chempots_df, verbose=False):
         if verbose:
             print(f"Calculating chempots for {self.extrinsic_species}")
         for e in extrinsic_formation_energies:
             for el in self.elemental:  # TODO: This code (in all this module) should be rewritten to
                 # be more readable (re-used and uninformative variable names, missing informative
                 # comments...)
-                e[el] = Composition(e["formula"]).as_dict().get(el, 0)
+                e[el] = Composition(e["Formula"]).as_dict().get(el, 0)
 
         # gets the df into a slightly more convenient dict
         cpd = chempots_df.to_dict(orient="records")
         mins = []
         mins_formulas = []
         df3 = pd.DataFrame(extrinsic_formation_energies)
         # print(f"df3: {df3}")  # debugging
         for i, c in enumerate(cpd):
             name = f"mu_{self.extrinsic_species}_{i}"
-            df3[name] = df3["formation_energy"]
+            df3[name] = df3["Formation Energy (eV/fu)"]
             for k, v in c.items():
                 df3[name] -= df3[k] * v
             df3[name] /= df3[self.extrinsic_species]
             # find min at that chempot
             mins.append(df3[name].min())
-            mins_formulas.append(df3.iloc[df3[name].idxmin()]["formula"])
+            mins_formulas.append(df3.iloc[df3[name].idxmin()]["Formula"])
 
         chempots_df[self.extrinsic_species] = mins
-        col_name = f"{self.extrinsic_species}_limiting_phase"
+        col_name = f"{self.extrinsic_species}-Limiting Phase"
         chempots_df[col_name] = mins_formulas
 
         # 1. work out the formation energies of all dopant competing
         #    phases using the elemental energies
         # 2. for each of the chempots already calculated work out what
         #    the chemical potential of the dopant would be from
         #       mu_dopant = Hf(dopant competing phase) - sum(mu_elements)
@@ -1617,53 +1641,57 @@
 
         with open(filename, "w", encoding="utf-8") as f, contextlib.redirect_stdout(f):
             # get lowest energy bulk phase
             bulk_entries = [
                 sub_dict
                 for sub_dict in self.data
                 if self.bulk_composition.reduced_composition
-                == Composition(sub_dict["formula"]).reduced_composition
+                == Composition(sub_dict["Formula"]).reduced_composition
             ]
-            bulk_entry = min(bulk_entries, key=lambda x: x["formation_energy"])
+            bulk_entry = min(bulk_entries, key=lambda x: x["Formation Energy (eV/fu)"])
             print(f"{len(self.bulk_composition.as_dict())}  # number of elements in bulk")
             for k, v in self.bulk_composition.as_dict().items():
                 print(int(v), k, end=" ")
-            print(f"{bulk_entry['formation_energy']}  # num_atoms, element, formation_energy (bulk)")
+            print(
+                f"{bulk_entry['Formation Energy (eV/fu)']}  # number of atoms, element, formation "
+                f"energy (bulk)"
+            )
 
             if dependent_variable is not None:
                 print(f"{dependent_variable}  # dependent variable (element)")
             else:
                 print(f"{self.elemental[0]}  # dependent variable (element)")
 
             # get only the lowest energy entries of compositions in self.data which are on a
             # limit in self._intrinsic_chempots
             bordering_phases = {phase for limit in self._chempots["limits"] for phase in limit.split("-")}
             entries_for_cplap = [
                 entry_dict
                 for entry_dict in self.data
-                if entry_dict["formula"] in bordering_phases
-                and Composition(entry_dict["formula"]).reduced_composition
+                if entry_dict["Formula"] in bordering_phases
+                and Composition(entry_dict["Formula"]).reduced_composition
                 != self.bulk_composition.reduced_composition
             ]
             # cull to only the lowest energy entries of each composition
             culled_cplap_entries = {}
             for entry in entries_for_cplap:
-                reduced_comp = Composition(entry["formula"]).reduced_composition
+                reduced_comp = Composition(entry["Formula"]).reduced_composition
                 if (
                     reduced_comp not in culled_cplap_entries
-                    or entry["formation_energy"] < culled_cplap_entries[reduced_comp]["formation_energy"]
+                    or entry["Formation Energy (eV/fu)"]
+                    < culled_cplap_entries[reduced_comp]["Formation Energy (eV/fu)"]
                 ):
                     culled_cplap_entries[reduced_comp] = entry
 
             print(f"{len(culled_cplap_entries)}  # number of bordering phases")
             for i in culled_cplap_entries.values():
-                print(f"{len(Composition(i['formula']).as_dict())}  # number of elements in phase:")
-                for k, v in Composition(i["formula"]).as_dict().items():
+                print(f"{len(Composition(i['Formula']).as_dict())}  # number of elements in phase:")
+                for k, v in Composition(i["Formula"]).as_dict().items():
                     print(int(v), k, end=" ")
-                print(f"{i['formation_energy']}  # num_atoms, element, formation_energy")
+                print(f"{i['Formation Energy (eV/fu)']}  # number of atoms, element, formation energy")
 
     def to_LaTeX_table(self, splits=1, sort_by_energy=False, prune_polymorphs=True):
         """
         A very simple function to print out the competing phase formation
         energies in a LaTeX table format, showing the formula, kpoints (if
         present in the parsed data) and formation energy.
 
@@ -1687,75 +1715,78 @@
             str: LaTeX table string
         """
         if splits not in [1, 2]:
             raise ValueError("`splits` must be either 1 or 2")
         # done in the pyscfermi report style
         formation_energy_data = self._get_and_sort_formation_energy_data(sort_by_energy, prune_polymorphs)
 
-        if any("kpoints" not in item for item in formation_energy_data):  # TODO: this is bad,
-            # should just not have the kpoints column if it's not present, and warn user
-            raise (
-                ValueError(
-                    "kpoints need to be present in data; run CompetingPhasesAnalyzer.from_vaspruns "
-                    "instead of from_csv"
-                )
-            )
+        kpoints_col = any("k-points" in item for item in formation_energy_data)
 
         string = "\\begin{table}[h]\n\\centering\n"
         string += (
-            "\\caption{Formation energies ($\\Delta E_f$) per formula unit of \\ce{"
+            "\\caption{Formation energies per formula unit ($\\Delta E_f$) of \\ce{"
             + self.bulk_composition.reduced_formula
-            + "} and all competing phases, with k-meshes used in calculations."
-            + ("}\n" if not prune_polymorphs else " Only the lowest energy polymorphs are included}\n")
+            + "} and all competing phases"
+            + (", with k-meshes used in calculations." if kpoints_col else ".")
+            + (" Only the lowest energy polymorphs are included}\n" if prune_polymorphs else "}\n")
         )
         string += "\\label{tab:competing_phase_formation_energies}\n"
+        column_names_string = "Formula" + (" & k-mesh" if kpoints_col else "") + " & $\\Delta E_f$ (eV/fu)"
+
         if splits == 1:
-            string += "\\begin{tabular}{ccc}\n"
+            string += "\\begin{tabular}" + ("{ccc}" if kpoints_col else "{cc}") + "\n"
             string += "\\hline\n"
-            string += "Formula & k-mesh & $\\Delta E_f$ (eV) \\\\ \\hline \n"
+            string += column_names_string + " \\\\ \\hline \n"
             for i in formation_energy_data:
-                kpoints = i["kpoints"].split("x")
-                fe = i["formation_energy"]
+                kpoints = i.get("k-points", "0x0x0").split("x")
+                fe = i["Formation Energy (eV/fu)"]
                 string += (
                     "\\ce{"
-                    + i["formula"]
-                    + "} & "
-                    + f"{kpoints[0]}$\\times${kpoints[1]}$\\times${kpoints[2]}"
-                    " & " + f"{fe:.3f} \\\\ \n"
+                    + i["Formula"]
+                    + "}"
+                    + (f" & {kpoints[0]}$\\times${kpoints[1]}$\\times${kpoints[2]}" if kpoints_col else "")
+                    + " & "
+                    + f"{fe:.3f} \\\\ \n"
                 )
 
         elif splits == 2:
-            string += "\\begin{tabular}{ccc|ccc}\n"
+            string += "\\begin{tabular}" + ("{ccc|ccc}" if kpoints_col else "{cc|cc}") + "\n"
             string += "\\hline\n"
-            string += (
-                "Formula & k-mesh & $\\Delta E_f$ (eV) & Formula & k-mesh & $\\Delta E_f$ (eV)\\\\ "
-                "\\hline \n"
-            )
+            string += column_names_string + " & " + column_names_string + " \\\\ \\hline \n"
 
             mid = len(formation_energy_data) // 2
             first_half = formation_energy_data[:mid]
             last_half = formation_energy_data[mid:]
 
             for i, j in zip(first_half, last_half):
-                kpoints = i["kpoints"].split("x")
-                fe = i["formation_energy"]
-                kpoints2 = j["kpoints"].split("x")
-                fe2 = j["formation_energy"]
+                kpoints1 = i.get("k-points", "0x0x0").split("x")
+                fe1 = i["Formation Energy (eV/fu)"]
+                kpoints2 = j.get("k-points", "0x0x0").split("x")
+                fe2 = j["Formation Energy (eV/fu)"]
                 string += (
                     "\\ce{"
-                    + i["formula"]
-                    + "} & "
-                    + f"{kpoints[0]}$\\times${kpoints[1]}$\\times${kpoints[2]}"
-                    " & "
-                    + f"{fe:.3f} & "
+                    + i["Formula"]
+                    + "}"
+                    + (
+                        f" & {kpoints1[0]}$\\times${kpoints1[1]}$\\times${kpoints1[2]}"
+                        if kpoints_col
+                        else ""
+                    )
+                    + " & "
+                    + f"{fe1:.3f} & "
                     + "\\ce{"
-                    + j["formula"]
-                    + "} & "
-                    + f"{kpoints2[0]}$\\times${kpoints2[1]}$\\times${kpoints2[2]}"
-                    " & " + f"{fe2:.3f} \\\\ \n"
+                    + j["Formula"]
+                    + "}"
+                    + (
+                        f" & {kpoints2[0]}$\\times${kpoints2[1]}$\\times${kpoints2[2]}"
+                        if kpoints_col
+                        else ""
+                    )
+                    + " & "
+                    + f"{fe2:.3f} \\\\ \n"
                 )
 
         string += "\\hline\n"
         string += "\\end{tabular}\n"
         string += "\\end{table}"
 
         return string
```

### Comparing `doped-2.4.0/doped/core.py` & `doped-2.4.1/doped/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,21 +247,23 @@
         Args:
             d (dict):
                 Dictionary representation of the ``DefectEntry`` object.
 
         Returns:
             ``DefectEntry`` object
         """
-        from doped.utils.parsing import _reset_warnings, suppress_logging
+        orig_simplefilter = warnings.simplefilter
+        warnings.simplefilter = lambda *args, **kwargs: None  # avoid vise warning suppression
+
+        from doped.utils.parsing import suppress_logging
 
         with suppress_logging():
             obj = super().from_dict(d)
 
-        _reset_warnings()  # vise suppresses ``UserWarning``s (and this initialises ``vise``
-        # ``BandEdgeStates`` objects) so need to reset
+        warnings.simplefilter = orig_simplefilter  # reset to original
 
         return obj
 
     def _check_correction_error_and_return_output(
         self,
         correction_output,
         correction_error,
@@ -273,18 +275,25 @@
             if isinstance(correction_output, tuple):  # correction_output may be a tuple, so amalgamate:
                 return (*correction_output, correction_error)
             return correction_output, correction_error
 
         if (
             correction_error > error_tolerance
         ):  # greater than 50 meV error in charge correction, warn the user
+            if error_tolerance >= 0.01:  # if greater than 10 meV, round energy values to meV:
+                error_val_string = f"{correction_error:.3f}"
+                error_tol_string = f"{error_tolerance:.3f}"
+            else:  # else give in scientific notation:
+                error_val_string = f"{correction_error:.2e}"
+                error_tol_string = f"{error_tolerance:.2e}"
+
             warnings.warn(
                 f"Estimated error in the {'Freysoldt (FNV)' if type == 'FNV' else 'Kumagai (eFNV)'} "
-                f"charge correction for defect {self.name} is {correction_error:.3f} eV (i.e. which is "
-                f"greater than the `error_tolerance`: {error_tolerance:.3f} eV). You may want to check "
+                f"charge correction for defect {self.name} is {error_val_string} eV (i.e. which is "
+                f"greater than the `error_tolerance`: {error_tol_string} eV). You may want to check "
                 f"the accuracy of the correction by plotting the site potential differences (using "
                 f"`defect_entry.get_{'freysoldt' if type == 'FNV' else 'kumagai'}_correction()` with "
                 f"`plot=True`). Large errors are often due to unstable or shallow defect charge states ("
                 f"which can't be accurately modelled with the supercell approach; see "
                 f"https://doped.readthedocs.io/en/latest/Tips.html#perturbed-host-states). "
                 f"If this error is not acceptable, you may need to use a larger supercell for more "
                 f"accurate energies."
@@ -310,14 +319,19 @@
         defect_entry.
 
         The correction is added to the ``defect_entry.corrections`` dictionary
         (to be used in following formation energy calculations).
         If this correction is used, please cite Freysoldt's
         original paper; 10.1103/PhysRevLett.102.016402.
 
+        The charge correction error is estimated by computing the average
+        standard deviation of the planar-averaged potential difference in the
+        sampling region, and multiplying by the defect charge. This is expected
+        to be a lower bound estimate of the true charge correction error.
+
         Args:
             dielectric (float or int or 3x1 matrix or 3x3 matrix):
                 Total dielectric constant of the host compound (including both
                 ionic and (high-frequency) electronic contributions), in the
                 same xyz Cartesian basis as the supercell calculations. If None,
                 then the dielectric constant is taken from the ``defect_entry``
                 ``calculation_metadata`` if available.
@@ -348,15 +362,16 @@
                 If None, then all three axes are plotted.
             return_correction_error (bool):
                 If True, also returns the average standard deviation of the
                 planar-averaged potential difference times the defect charge
                 (which gives an estimate of the error range of the correction
                 energy). Default is False.
             error_tolerance (float):
-                If the estimated error in the charge correction is greater than
+                If the estimated error in the charge correction, based on the
+                variance of the potential in the sampling region, is greater than
                 this value (in eV), then a warning is raised. (default: 0.05 eV)
             style_file (str):
                 Path to a ``.mplstyle`` file to use for the plot. If ``None``
                 (default), uses the default doped style
                 (from ``doped/utils/doped.mplstyle``).
             **kwargs:
                 Additional kwargs to pass to
@@ -443,15 +458,20 @@
         at small/intermediate supercell sizes, you may want to adjust this (and/or
         ``excluded_indices``) to ensure the best sampling of the plateau region away
         from the defect position - ``doped`` should throw a warning in these cases
         (about the correction error being above the default tolerance (50 meV)).
         For example, with layered materials, the defect charge is often localised
         to one layer, so we may want to adjust ``defect_region_radius`` and/or
         ``excluded_indices`` to ensure that only sites in other layers are used for
-        the sampling region (plateau) - see example on doped docs Tips page.
+        the sampling region (plateau) - see example on doped docs ``Tips`` page.
+
+        The correction error is estimated by computing the standard error of the mean
+        of the sampled site potential differences, multiplied by the defect charge.
+        This is expected to be a lower bound estimate of the true charge correction
+        error.
 
         Args:
             dielectric (float or int or 3x1 matrix or 3x3 matrix):
                 Total dielectric constant of the host compound (including both
                 ionic and (high-frequency) electronic contributions), in the
                 same xyz Cartesian basis as the supercell calculations. If None,
                 then the dielectric constant is taken from the ``defect_entry``
@@ -483,15 +503,16 @@
                 If None, plots are not saved.
             return_correction_error (bool):
                 If True, also returns the standard error of the mean of the
                 sampled site potential differences times the defect charge
                 (which gives an estimate of the error range of the correction
                 energy). Default is False.
             error_tolerance (float):
-                If the estimated error in the charge correction is greater than
+                If the estimated error in the charge correction, based on the
+                variance of the potential in the sampling region, is greater than
                 this value (in eV), then a warning is raised. (default: 0.05 eV)
             style_file (str):
                 Path to a ``.mplstyle`` file to use for the plot. If ``None``
                 (default), uses the default doped style
                 (from ``doped/utils/doped.mplstyle``).
             **kwargs:
                 Additional kwargs to pass to
@@ -599,21 +620,18 @@
         if self.calculation_metadata.get("eigenvalue_data") is not None and not force_reparse:
             return
 
         from doped.utils.eigenvalues import _parse_procar, get_band_edge_info
         from doped.utils.parsing import (
             _get_output_files_and_check_if_multiple,
             _multiple_files_warning,
-            _reset_warnings,
             get_procar,
             get_vasprun,
         )
 
-        _reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
-
         parsed_vr_procar_dict = {}
         for vr, procar, label in [(bulk_vr, bulk_procar, "bulk"), (defect_vr, defect_procar, "defect")]:
             path = self.calculation_metadata.get(f"{label}_path")
             if vr is not None and not isinstance(vr, Vasprun):  # just try loading from vasprun first
                 with contextlib.suppress(Exception):
                     vr = get_vasprun(vr, parse_projected_eigen=True)  # noqa: PLW2901
 
@@ -676,14 +694,15 @@
         defect_vr, defect_procar = parsed_vr_procar_dict["defect"]
 
         band_orb, vbm_info, cbm_info = get_band_edge_info(
             bulk_vr=bulk_vr,
             defect_vr=defect_vr,
             bulk_procar=bulk_procar,  # may be None, in which case Vasprun.projected_eigenvalues used
             defect_procar=defect_procar,  # may be None, in which case Vasprun.projected_eigenvalues used
+            defect_supercell_site=self.defect_supercell_site,
         )
 
         self.calculation_metadata["eigenvalue_data"] = {
             "band_orb": band_orb,
             "vbm_info": vbm_info,
             "cbm_info": cbm_info,
         }
@@ -786,17 +805,14 @@
                 ``similar_energy_criterion``.
 
         Returns:
             ``pydefect`` ``BandEdgeStates`` object and ``matplotlib``
             ``Figure`` object (if ``plot=True``).
         """
         from doped.utils.eigenvalues import get_eigenvalue_analysis
-        from doped.utils.parsing import _reset_warnings
-
-        _reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
 
         self._load_and_parse_eigenvalue_data(
             bulk_vr=bulk_vr,
             bulk_procar=bulk_procar,
             defect_vr=defect_vr,
             defect_procar=defect_procar,
             force_reparse=force_reparse,
@@ -1735,14 +1751,44 @@
                 Filename of json file to load ``Defect`` from.
 
         Returns:
             ``Defect`` object
         """
         return loadfn(filename)
 
+    def get_charge_states(self, padding: int = 1) -> list[int]:
+        """
+        Refactored version of ``pymatgen-analysis-defects``'s
+        ``get_charge_states`` to not break when ``oxi_state`` is not set.
+        """
+        if self.user_charges:
+            return self.user_charges
+
+        if self.oxi_state is None or not isinstance(self.oxi_state, (int, float)):
+            self._set_oxi_state()  # try guessing
+
+        if self.oxi_state is None or not isinstance(self.oxi_state, (int, float)):  # still not set
+            warnings.warn(
+                f"Defect oxidation state not set and couldn't be guessed, returning charge"
+                f"state range from -{padding} to +{padding}"
+            )
+            return [*range(-padding, padding + 1)]
+
+        if isinstance(self.oxi_state, int) or self.oxi_state.is_integer():
+            oxi_state = int(self.oxi_state)
+        else:
+            raise ValueError("Oxidation state must be an integer")
+
+        if oxi_state >= 0:
+            charges = [*range(-padding, oxi_state + padding + 1)]
+        else:
+            charges = [*range(oxi_state - padding, padding + 1)]
+
+        return charges
+
 
 def doped_defect_from_pmg_defect(defect: core.Defect, bulk_oxi_states=False, **doped_kwargs):
     """
     Create the corresponding ``doped`` ``Defect`` (``Vacancy``,
     ``Interstitial``, ``Substitution``) from an input ``pymatgen`` ``Defect``
     object.
```

### Comparing `doped-2.4.0/doped/corrections.py` & `doped-2.4.1/doped/corrections.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 resulting quantitative error in the correction is negligible. However, in cases where we have large
 finite-size correction values, this can be significant. If some efficient methods for determining the
 centroid of charge difference between bulk/defect LOCPOTs (for FNV) or bulk/defect site potentials (for
 eFNV) were developed, they should be used here.
 """
 
 import os
+import warnings
 from typing import Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.lines import Line2D
 from monty.json import MontyDecoder
 from pymatgen.analysis.defects.corrections import freysoldt
@@ -49,22 +50,19 @@
 from shakenbreak.plotting import _install_custom_font
 
 from doped.analysis import _convert_dielectric_to_tensor
 from doped.utils.parsing import (
     _get_bulk_supercell,
     _get_defect_supercell,
     _get_defect_supercell_bulk_site_coords,
-    _reset_warnings,
     get_locpot,
     get_outcar,
 )
 from doped.utils.plotting import _get_backend, format_defect_name
 
-_reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
-
 
 def _monty_decode_nested_dicts(d):
     """
     Recursively find any dictionaries in defect_entry.calculation_metadata,
     which may be nested in dicts or in lists of dicts, and decode them.
     """
     for key, value in d.items():
@@ -388,14 +386,17 @@
             pydefect.corrections.efnv_correction.ExtendedFnvCorrection
             (e.g. charge, defect_region_radius, defect_coords).
 
     Returns:
         CorrectionResults (summary of the corrections applied and metadata), and
         the matplotlib figure object if ``plot`` is True.
     """
+    orig_simplefilter = warnings.simplefilter
+    warnings.simplefilter = lambda *args, **kwargs: None  # monkey-patch to avoid vise warning suppression
+
     # suppress pydefect INFO messages
     import logging
 
     try:
         from vise import user_settings
 
         user_settings.logger.setLevel(logging.CRITICAL)
@@ -410,15 +411,15 @@
 
     except ImportError as exc:
         raise ImportError(
             "To use the Kumagai (eFNV) charge correction, you need to install pydefect. "
             "You can do this by running `pip install pydefect`."
         ) from exc
 
-    _reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
+    warnings.simplefilter = orig_simplefilter  # reset to original
 
     def doped_make_efnv_correction(
         charge: float,
         calc_results: CalcResults,
         perfect_calc_results: CalcResults,
         dielectric_tensor: np.array,
         defect_region_radius: Optional[float] = None,
```

### Comparing `doped-2.4.0/doped/generation.py` & `doped-2.4.1/doped/generation.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/thermodynamics.py` & `doped-2.4.1/doped/thermodynamics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1306,15 +1306,15 @@
         )
 
     def _parse_fermi_dos(self, bulk_dos_vr: Union[str, Vasprun, FermiDos]):
         if isinstance(bulk_dos_vr, FermiDos):
             return bulk_dos_vr
 
         if isinstance(bulk_dos_vr, str):
-            bulk_dos_vr = get_vasprun(bulk_dos_vr)
+            bulk_dos_vr = get_vasprun(bulk_dos_vr, parse_dos=True)
 
         fermi_dos_band_gap, _cbm, fermi_dos_vbm, _ = bulk_dos_vr.eigenvalue_band_properties
         if abs(fermi_dos_vbm - self.vbm) > 0.1:
             warnings.warn(
                 f"The VBM eigenvalue of the bulk DOS calculation ({fermi_dos_vbm:.2f} eV, with band "
                 f"gap of {fermi_dos_band_gap:.2f} eV) differs from that of the bulk supercell "
                 f"calculations ({self.vbm:.2f} eV, with band gap of {self.band_gap:.2f} eV) by more "
@@ -2860,15 +2860,16 @@
             f"{properties}\n\nAvailable methods:\n{methods}"
         )
 
 
 def get_e_h_concs(fermi_dos: FermiDos, fermi_level: float, temperature: float) -> tuple[float, float]:
     """
     Get the corresponding electron and hole concentrations (in cm^-3) for a
-    given Fermi level (in eV) and temperature (in K), for a FermiDos object.
+    given Fermi level (in eV) and temperature (in K), for a ``FermiDos``
+    object.
 
     Note that the Fermi level here is NOT referenced to the VBM! So the Fermi
     level should be the corresponding eigenvalue within the calculation (or in
     other words, the Fermi level relative to the VBM plus the VBM eigenvalue).
     """
     # code for obtaining the electron and hole concentrations here is taken from
     # FermiDos.get_doping():
@@ -2892,15 +2893,15 @@
         * fermi_dos.de[: fermi_dos.idx_vbm + 1],
         axis=0,
     ) / (fermi_dos.volume * fermi_dos.A_to_cm**3)
 
     return e_conc, h_conc
 
 
-def scissor_dos(delta_gap: float, dos: Dos, tol=1e-8, verbose=True):
+def scissor_dos(delta_gap: float, dos: Union[Dos, FermiDos], tol: float = 1e-8, verbose: bool = True):
     """
     Given an input Dos/FermiDos object, rigidly shifts the valence and
     conduction bands of the DOS object to give a band gap that is now
     increased/decreased by ``delta_gap`` eV, where this rigid scissor shift is
     applied symmetrically around the original gap (i.e. the VBM is downshifted
     by ``delta_gap/2`` and the CBM is upshifted by ``delta_gap/2``).
 
@@ -2985,8 +2986,10 @@
     scissored_dos_dict["energies"] = np.array(scissored_dos_dict["energies"])
     scissored_dos_dict["energies"] -= np.float64(delta_gap / 2)
     scissored_dos_dict["efermi"] -= np.float64(delta_gap / 2)
 
     if verbose:
         print(f"Orig gap: {dos.get_gap(tol=tol)}, new gap:{dos.get_gap(tol=tol) + delta_gap}")
     scissored_dos_dict["structure"] = dos.structure.as_dict()
-    return FermiDos.from_dict(scissored_dos_dict)
+    if isinstance(dos, FermiDos):
+        return FermiDos.from_dict(scissored_dos_dict)
+    return Dos.from_dict(scissored_dos_dict)
```

### Comparing `doped-2.4.0/doped/utils/displacement.mplstyle` & `doped-2.4.1/doped/utils/displacement.mplstyle`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/displacements.py` & `doped-2.4.1/doped/utils/displacements.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/doped.mplstyle` & `doped-2.4.1/doped/utils/doped.mplstyle`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/eigenvalues.py` & `doped-2.4.1/doped/utils/eigenvalues.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,93 +12,51 @@
 from collections import defaultdict
 from itertools import zip_longest
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Optional, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
-from pymatgen.core import Element, Species
+from pymatgen.core.structure import PeriodicSite
 from pymatgen.electronic_structure.core import Spin
 from pymatgen.entries.computed_entries import ComputedStructureEntry
 from pymatgen.io.vasp.outputs import Procar, Vasprun
 from shakenbreak.plotting import _install_custom_font
 
+from doped.analysis import defect_from_structures
 from doped.core import DefectEntry
-from doped.utils.parsing import (
-    _reset_warnings,
-    get_magnetization_from_vasprun,
-    get_nelect_from_vasprun,
-    get_procar,
-)
+from doped.utils.parsing import get_magnetization_from_vasprun, get_nelect_from_vasprun, get_procar
 from doped.utils.plotting import _get_backend
 
+orig_simplefilter = warnings.simplefilter
+warnings.simplefilter = lambda *args, **kwargs: None  # monkey-patch to avoid vise warning suppression
+
 if TYPE_CHECKING:
     from easyunfold.procar import Procar as EasyunfoldProcar
-    from pydefect.analyzer.make_defect_structure_info import DefectStructureInfo
 
 try:
     from vise import user_settings
 
     user_settings.logger.setLevel(logging.CRITICAL)
     import pydefect.analyzer.make_band_edge_states
     import pydefect.cli.vasp.make_band_edge_orbital_infos as make_bes
     from pydefect.analyzer.band_edge_states import BandEdgeOrbitalInfos, OrbitalInfo, PerfectBandEdgeState
     from pydefect.analyzer.eigenvalue_plotter import EigenvalueMplPlotter
     from pydefect.analyzer.make_band_edge_states import make_band_edge_states
-    from pydefect.analyzer.make_defect_structure_info import MakeDefectStructureInfo
     from pydefect.cli.vasp.make_perfect_band_edge_state import get_edge_info
     from pydefect.defaults import defaults
-    from pydefect.util.structure_tools import Coordination, Distances
     from vise.analyzer.vasp.band_edge_properties import BandEdgeProperties, eigenvalues_from_vasprun
 
 except ImportError as exc:
     raise ImportError(
         "To perform eigenvalue & orbital analysis, you need to install pydefect. "
         "You can do this by running `pip install pydefect`."
     ) from exc
 
-_reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
-
-
-def _coordination(self, include_on_site=True, cutoff_factor=None) -> "Coordination":
-    cutoff_factor = cutoff_factor or defaults.cutoff_distance_factor
-    cutoff = self.shortest_distance * cutoff_factor
-    elements = [element.specie.name for element in self.structure]
-    e_d = zip(elements, self.distances(remove_self=False))
-
-    unsorted_distances = defaultdict(list)
-    neighboring_atom_indices = []
-    for i, (element, distance) in enumerate(e_d):
-        if distance < cutoff and include_on_site:
-            unsorted_distances[element].append(round(distance, 2))
-            neighboring_atom_indices.append(i)
-
-    distance_dict = {element: sorted(distances) for element, distances in unsorted_distances.items()}
-    return Coordination(distance_dict, round(cutoff, 3), neighboring_atom_indices)
-
-
-def _distances(self, remove_self=True, specie=None) -> list[float]:
-    result = []
-    lattice = self.structure.lattice
-    if isinstance(specie, Element):
-        el = specie.symbol
-    elif specie is None:
-        el = None
-    elif isinstance(specie, Species):
-        el = specie.element
-    for site in self.structure:
-        site_specie = site.specie.element if isinstance(site.specie, Species) else site.specie
-        if el and Element(el) != site_specie:
-            result.append(float("inf"))
-            continue
-        distance, _ = lattice.get_distance_and_image(site.frac_coords, self.coord)
-        if remove_self and distance < 1e-5:
-            continue
-        result.append(distance)
-    return result
+warnings.simplefilter = orig_simplefilter  # reset to original
 
 
 def band_edge_properties_from_vasprun(
     vasprun: Vasprun, integer_criterion: float = 0.1
 ) -> BandEdgeProperties:
     """
     Create a ``pydefect`` ``BandEdgeProperties`` object from a ``Vasprun``
@@ -152,102 +110,116 @@
     band_edge_prop = band_edge_properties_from_vasprun(vasprun, integer_criterion)
     orbs, s = procar.data, vasprun.final_structure
     vbm_info = get_edge_info(band_edge_prop.vbm_info, orbs, s, vasprun)
     cbm_info = get_edge_info(band_edge_prop.cbm_info, orbs, s, vasprun)
     return PerfectBandEdgeState(vbm_info, cbm_info)
 
 
-def _make_band_edge_orbital_infos_vr(
-    defect_vr: Vasprun, vbm: float, cbm: float, str_info: "DefectStructureInfo", eigval_shift: float = 0.0
+def make_band_edge_orbital_infos(
+    defect_vr: Vasprun,
+    vbm: float,
+    cbm: float,
+    eigval_shift: float = 0.0,
+    neighbor_indices: Optional[list[int]] = None,
+    defect_procar: Optional[Union["EasyunfoldProcar", Procar]] = None,
 ):
     """
     Make ``BandEdgeOrbitalInfos`` from a ``Vasprun`` object.
 
     Modified from ``pydefect`` to use projected orbitals
     stored in the ``Vasprun`` object.
 
     Args:
         defect_vr (Vasprun): Defect ``Vasprun`` object.
         vbm (float): VBM eigenvalue in eV.
         cbm (float): CBM eigenvalue in eV.
-        str_info (DefectStructureInfo): ``pydefect`` ``DefectStructureInfo``.
-        eigval_shift (float): Shift eigenvalues down by this value (to set VBM at 0 eV).
+        eigval_shift (float):
+            Shift eigenvalues down by this value (to set VBM at 0 eV).
+            Default is 0.0.
+        neighbor_indices (list[int]):
+            Indices of neighboring atoms to the defect site, for localisation analysis.
+            Default is ``None``.
+        defect_procar (EasyunfoldProcar, Procar):
+            ``EasyunfoldProcar`` or ``Procar`` object, for the defect supercell,
+            if projected eigenvalue/orbitals data is not provided in ``defect_vr``.
 
     Returns:
         ``BandEdgeOrbitalInfos `` object
     """
     eigval_range = defaults.eigval_range
     kpt_coords = [tuple(coord) for coord in defect_vr.actual_kpoints]
     max_energy_by_spin, min_energy_by_spin = [], []
-    neighbors = str_info.neighbor_atom_indices
 
     for e in defect_vr.eigenvalues.values():
         max_energy_by_spin.append(np.amax(e[:, :, 0], axis=0))
         min_energy_by_spin.append(np.amin(e[:, :, 0], axis=0))
 
     max_energy_by_band = np.amax(np.vstack(max_energy_by_spin), axis=0)
     min_energy_by_band = np.amin(np.vstack(min_energy_by_spin), axis=0)
 
     lower_idx = np.argwhere(max_energy_by_band > vbm - eigval_range)[0][0]
     upper_idx = np.argwhere(min_energy_by_band < cbm + eigval_range)[-1][-1]
 
-    orbs, s = defect_vr.projected_eigenvalues, defect_vr.final_structure
+    orbs = defect_vr.projected_eigenvalues if defect_procar is None else defect_procar.data
+    s = defect_vr.final_structure
     orb_infos: list[Any] = []
     for spin, eigvals in defect_vr.eigenvalues.items():
         orb_infos.append([])
         for k_idx in range(len(kpt_coords)):
             orb_infos[-1].append([])
             for b_idx in range(lower_idx, upper_idx + 1):
                 e, occ = eigvals[k_idx, b_idx, :]
                 orbitals = make_bes.calc_orbital_character(orbs, s, spin, k_idx, b_idx)
-                if neighbors:
-                    p_ratio = make_bes.calc_participation_ratio(orbs, spin, k_idx, b_idx, neighbors)
+                if neighbor_indices:
+                    p_ratio = make_bes.calc_participation_ratio(orbs, spin, k_idx, b_idx, neighbor_indices)
                 else:
                     p_ratio = None
                 orb_infos[-1][-1].append(OrbitalInfo(e, orbitals, occ, p_ratio))
 
     return BandEdgeOrbitalInfos(
         orbital_infos=orb_infos,
         kpt_coords=kpt_coords,
         kpt_weights=defect_vr.actual_kpoints_weights,
         lowest_band_index=int(lower_idx),
         fermi_level=defect_vr.efermi,
         eigval_shift=eigval_shift,
     )
 
 
-def _parse_procar(procar: Union[str, "Path", "EasyunfoldProcar", Procar]):
+def _parse_procar(procar: Optional[Union[str, Path, "EasyunfoldProcar", Procar]] = None):
     """
     Parse a ``procar`` input to a ``Procar`` object in the correct format.
 
     Args:
         procar (str, Path, EasyunfoldProcar, Procar):
             Either a path to the ``VASP`` ``PROCAR``` output file (with
             ``LORBIT > 10`` in the ``INCAR``) or an ``easyunfold``/``pymatgen``
             ``Procar`` object.
     """
     if not hasattr(procar, "data"):  # not a parsed Procar object
-        if hasattr(procar, "proj_data") and not isinstance(procar, (str, Path, Procar)):
+        if procar and hasattr(procar, "proj_data") and not isinstance(procar, (str, Path, Procar)):
             if procar._is_soc:
                 procar.data = {Spin.up: procar.proj_data[0]}
             else:
                 procar.data = {Spin.up: procar.proj_data[0], Spin.down: procar.proj_data[1]}
             del procar.proj_data
 
-        else:  # path to PROCAR file
+        elif isinstance(procar, (str, Path)):  # path to PROCAR file
             procar = get_procar(procar)
 
     return procar
 
 
 def get_band_edge_info(
     bulk_vr: Vasprun,
     defect_vr: Vasprun,
-    bulk_procar: Optional[Union[str, "Path", "EasyunfoldProcar", Procar]] = None,
-    defect_procar: Optional[Union[str, "Path", "EasyunfoldProcar", Procar]] = None,
+    bulk_procar: Optional[Union[str, Path, "EasyunfoldProcar", Procar]] = None,
+    defect_procar: Optional[Union[str, Path, "EasyunfoldProcar", Procar]] = None,
+    defect_supercell_site: Optional[PeriodicSite] = None,
+    neighbor_cutoff_factor: float = 1.3,
 ):
     """
     Generate metadata required for performing eigenvalue & orbital analysis,
     specifically ``pydefect`` ``BandEdgeOrbitalInfos``, and ``EdgeInfo``
     objects for the bulk VBM and CBM.
 
     See https://doped.readthedocs.io/en/latest/Tips.html#perturbed-host-states.
@@ -275,73 +247,85 @@
         defect_procar (str, Path, EasyunfoldProcar, Procar):
             Either a path to the ``VASP`` ``PROCAR`` output file (with
             ``LORBIT > 10`` in the ``INCAR``) or an ``easyunfold``/
             ``pymatgen`` ``Procar`` object, for the defect supercell
             calculation. Not required if the supplied ``bulk_vr`` was
             parsed with ``parse_projected_eigen = True``.
             Default is ``None``.
+        defect_supercell_site (PeriodicSite):
+            ``PeriodicSite`` object of the defect site in the defect
+            supercell, from which the defect neighbours are determined
+            for localisation analysis. If ``None`` (default), then the
+            defect site is determined automatically from the defect
+            and bulk supercell structures.
+        neighbor_cutoff_factor (float):
+            Sites within ``min_distance * neighbor_cutoff_factor`` of
+            the defect site in the `relaxed` defect supercell are
+            considered neighbors for localisation analysis, where
+            ``min_distance`` is the minimum distance between sites in
+            the defect supercell. Default is 1.3 (matching the ``pydefect``
+            default).
 
     Returns:
         ``pydefect`` ``BandEdgeOrbitalInfos``, and ``EdgeInfo`` objects
         for the bulk VBM and CBM.
     """
     band_edge_prop = band_edge_properties_from_vasprun(bulk_vr)
 
     if bulk_procar is not None:
         bulk_procar = _parse_procar(bulk_procar)
         pbes = make_perfect_band_edge_state_from_vasp(vasprun=bulk_vr, procar=bulk_procar)
 
-    _orig_method_coor = Distances.coordination
-    Distances.coordination = _coordination
-    _orig_method_dist = Distances.distances
-    Distances.distances = _distances
-
-    dsinfo = MakeDefectStructureInfo(  # Using default values suggested by pydefect
-        bulk_vr.final_structure,
-        defect_vr.final_structure,
-        defect_vr.final_structure,
-        symprec=0.1,
-        dist_tol=1.0,
-        neighbor_cutoff_factor=1.3,  # Neighbors are sites within min_dist * neighbor_cutoff_factor
-    )
+    # get defect neighbour indices
+    sorted_distances = np.sort(defect_vr.final_structure.distance_matrix.flatten())
+    min_distance = sorted_distances[sorted_distances > 0.5][0]
+
+    if defect_supercell_site is None:
+        (
+            _defect,
+            defect_site,  # _relaxed_ defect site in supercell (if substitution/interstitial)
+            defect_site_in_bulk,  # vacancy site
+            _defect_site_index,
+            _bulk_site_index,
+            _guessed_initial_defect_structure,
+            _unrelaxed_defect_structure,
+            _bulk_voronoi_node_dict,
+        ) = defect_from_structures(
+            bulk_vr.final_structure,
+            defect_vr.final_structure.copy(),
+            return_all_info=True,
+            oxi_state="Undetermined",
+        )
+        defect_supercell_site = defect_site or defect_site_in_bulk
 
-    # Undo monkey patch in case used in other parts of the code:
-    Distances.coordination = _orig_method_coor
-    Distances.distances = _orig_method_dist
+    neighbor_indices = [
+        i
+        for i, site in enumerate(defect_vr.final_structure.sites)
+        if defect_supercell_site.distance(site) <= min_distance * neighbor_cutoff_factor
+    ]
 
     from pydefect.analyzer.band_edge_states import logger
 
     logger.setLevel(logging.CRITICAL)  # quieten unnecessary eigenvalue shift INFO message
 
     if bulk_procar is not None:
         vbm_info, cbm_info = pbes.vbm_info, pbes.cbm_info
     else:
         orbs, s = bulk_vr.projected_eigenvalues, bulk_vr.final_structure
         vbm_info = get_edge_info(band_edge_prop.vbm_info, orbs, s, bulk_vr)
         cbm_info = get_edge_info(band_edge_prop.cbm_info, orbs, s, bulk_vr)
 
-    if defect_procar is not None:
-        defect_procar = _parse_procar(defect_procar)
-        band_orb = make_bes.make_band_edge_orbital_infos(
-            defect_procar,
-            defect_vr,
-            vbm_info.orbital_info.energy,
-            cbm_info.orbital_info.energy,
-            eigval_shift=-vbm_info.orbital_info.energy,
-            str_info=dsinfo.defect_structure_info,
-        )
-
-    else:
-        band_orb = _make_band_edge_orbital_infos_vr(
-            defect_vr,
-            vbm_info.orbital_info.energy,
-            cbm_info.orbital_info.energy,
-            eigval_shift=-vbm_info.orbital_info.energy,
-            str_info=dsinfo.defect_structure_info,
-        )
+    band_orb = make_band_edge_orbital_infos(
+        defect_vr,
+        vbm_info.orbital_info.energy,
+        cbm_info.orbital_info.energy,
+        eigval_shift=-vbm_info.orbital_info.energy,
+        neighbor_indices=neighbor_indices,
+        defect_procar=_parse_procar(defect_procar),
+    )
 
     return band_orb, vbm_info, cbm_info
 
 
 def _add_eigenvalues(
     self,
     occupied_color=(0.22, 0.325, 0.643),
@@ -395,18 +379,18 @@
 
 def get_eigenvalue_analysis(
     defect_entry: Optional[DefectEntry] = None,
     plot: bool = True,
     filename: Optional[str] = None,
     ks_labels: bool = False,
     style_file: Optional[str] = None,
-    bulk_vr: Optional[Union[str, "Path", Vasprun]] = None,
-    bulk_procar: Optional[Union[str, "Path", "EasyunfoldProcar", Procar]] = None,
-    defect_vr: Optional[Union[str, "Path", Vasprun]] = None,
-    defect_procar: Optional[Union[str, "Path", "EasyunfoldProcar", Procar]] = None,
+    bulk_vr: Optional[Union[str, Path, Vasprun]] = None,
+    bulk_procar: Optional[Union[str, Path, "EasyunfoldProcar", Procar]] = None,
+    defect_vr: Optional[Union[str, Path, Vasprun]] = None,
+    defect_procar: Optional[Union[str, Path, "EasyunfoldProcar", Procar]] = None,
     force_reparse: bool = False,
     ylims: Optional[tuple[float, float]] = None,
     legend_kwargs: Optional[dict] = None,
     similar_orb_criterion: Optional[float] = None,
     similar_energy_criterion: Optional[float] = None,
 ):
     r"""
@@ -643,16 +627,16 @@
                 if hasattr(child, "get_facecolor"):
                     partial = partial or any(
                         np.array_equal(child.get_facecolor()[i], [0, 0.5, 0, 1])
                         for i in range(len(child.get_facecolor()))
                     )
 
         if len(emp.axs) > 1:
-            emp.axs[0].set_title("Spin Down")
-            emp.axs[1].set_title("Spin Up")
+            emp.axs[0].set_title("Spin Up")
+            emp.axs[1].set_title("Spin Down")
         else:
             emp.axs[0].set_title("KS levels")
 
         gamma_check = "\N{GREEK CAPITAL LETTER GAMMA}"
         for ax in emp.axs:
             labels = ax.get_xticklabels()
             labels = [label.get_text() for label in labels]
```

### Comparing `doped-2.4.0/doped/utils/legacy_corrections.py` & `doped-2.4.1/doped/utils/legacy_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/parsing.py` & `doped-2.4.1/doped/utils/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,37 +17,25 @@
 from pymatgen.core.periodic_table import Element
 from pymatgen.core.structure import PeriodicSite, Structure
 from pymatgen.electronic_structure.core import Spin
 from pymatgen.io.vasp.inputs import POTCAR_STATS_PATH, UnknownPotcarWarning
 from pymatgen.io.vasp.outputs import Locpot, Outcar, Procar, Vasprun, _parse_vasp_array
 from pymatgen.util.coord import pbc_diff
 
-from doped import _ignore_pmg_warnings
 from doped.core import DefectEntry
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @lru_cache(maxsize=1000)  # cache POTCAR generation to speed up generation and writing
 def _get_potcar_summary_stats() -> dict:
     return loadfn(POTCAR_STATS_PATH)
 
 
-def _reset_warnings():
-    """
-    When importing ``vise``/``pydefect``, ``UserWarning``s are suppressed, so
-    we need to reset.
-    """
-    warnings.simplefilter("default")
-    warnings.filterwarnings("ignore", message="`np.int` is a deprecated alias for the builtin `int`")
-    warnings.filterwarnings("ignore", message="Use get_magnetic_symmetry()")
-    _ignore_pmg_warnings()
-
-
 @contextlib.contextmanager
 def suppress_logging(level=logging.CRITICAL):
     """
     Context manager to catch and suppress logging messages.
     """
     previous_level = logging.root.manager.disable  # store the current logging level
     logging.disable(level)  # disable logging at the specified level
@@ -537,27 +525,30 @@
 
 def check_atom_mapping_far_from_defect(bulk, defect, defect_coords):
     """
     Check the displacement of atoms far from the determined defect site, and
     warn the user if they are large (often indicates a mismatch between the
     bulk and defect supercell definitions).
     """
+    orig_simplefilter = warnings.simplefilter
+    warnings.simplefilter = lambda *args, **kwargs: None  # monkey-patch to avoid vise warning suppression
+
     # suppress pydefect INFO messages
     import logging
 
     try:
         from vise import user_settings
 
         user_settings.logger.setLevel(logging.CRITICAL)
         from pydefect.cli.vasp.make_efnv_correction import calc_max_sphere_radius
 
     except ImportError:  # can't check as vise/pydefect not installed. Not critical so just return
         return
 
-    _reset_warnings()  # vise suppresses `UserWarning`s, so need to reset
+    warnings.simplefilter = orig_simplefilter  # reset to original
 
     far_from_defect_disps = {site.specie.symbol: [] for site in bulk}
 
     wigner_seitz_radius = calc_max_sphere_radius(bulk.lattice.matrix)
 
     bulk_sites_outside_or_at_wigner_radius = [
         site
```

### Comparing `doped-2.4.0/doped/utils/plotting.py` & `doped-2.4.1/doped/utils/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,15 +623,15 @@
                 defect_name = f"{defect_name}$_{{-{chr(96 + 2)}}}$"  # b
 
             else:
                 defect_name = f"{defect_name}$_{{-{chr(96 + i)}}}$"  # c
 
             while defect_name in legends_txt:
                 i += 1
-                defect_name = f"{defect_name}$_{{-{chr(96 + i)}}}$"  # d, e, f etc
+                defect_name = f"{defect_name.rsplit('$_', 1)[0]}$_{{-{chr(96 + i)}}}$"  # d, e, f etc
 
         legends_txt.append(defect_name)
 
     return legends_txt
 
 
 def _rename_key_and_dicts(
@@ -659,15 +659,15 @@
             key = f"{key}_{chr(96 + 2)}"  # b
 
         else:
             key = f"{key}_{chr(96 + i)}"  # c
 
         while key in output_dict:
             i += 1
-            key = f"{key}_{chr(96 + i)}"  # d, e, f etc
+            key = f"{key.rsplit('_', 1)[0]}_{chr(96 + i)}"  # d, e, f etc
 
     return key, output_dicts
 
 
 def _get_formation_energy_lines(defect_thermodynamics, dft_chempots, xlim):
     xy, all_lines_xy = {}, {}  # dict of {defect_name: [[x_vals],[y_vals]]}
     y_range_vals, all_entries_y_range_vals = (
```

### Comparing `doped-2.4.0/doped/utils/supercells.py` & `doped-2.4.1/doped/utils/supercells.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/symmetry.py` & `doped-2.4.1/doped/utils/symmetry.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/utils/wyckpos.dat` & `doped-2.4.1/doped/utils/wyckpos.dat`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/doped/vasp.py` & `doped-2.4.1/doped/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,14 @@
             poscar_comment (str):
                 Comment line to use for ``POSCAR`` files. Default is defect name,
                 fractional coordinates of initial site and charge state.
             **kwargs: Additional kwargs to pass to ``DictSet``.
         """
         _ignore_pmg_warnings()
         self.charge_state = charge_state
-        self.potcars = self._check_user_potcars(unperturbed_poscar=True, snb=False)
         self.poscar_comment = (
             poscar_comment
             or f"{structure.formula} {'+' if self.charge_state > 0 else ''}{self.charge_state}"
         )
         custom_user_incar_settings = user_incar_settings or {}
 
         # get base config and set EDIFF
@@ -513,35 +512,38 @@
                 the specific POTCAR file can be re-generated using pymatgen with the
                 "generate_potcar" function in the pymatgen CLI. (default: False)
             zip_output (bool): Whether to zip each VASP input file written to the
                 output directory. (default: False)
             snb (bool): If input structures are from ShakeNBreak (so POSCARs aren't
                 'unperturbed'). (default: False)
         """
-        if not potcar_spec:
-            potcars = self._check_user_potcars(unperturbed_poscar=unperturbed_poscar, snb=snb)
-        else:
+        if potcar_spec:
             potcars = True
 
+        else:
+            potcars = self._check_user_potcars(unperturbed_poscar=unperturbed_poscar, snb=snb)
+
         if unperturbed_poscar and potcars:  # write everything, use DictSet.write_input()
             try:
                 super().write_input(
                     output_path,
                     make_dir_if_not_present=make_dir_if_not_present,
                     include_cif=include_cif,
                     potcar_spec=potcar_spec,
                     zip_output=zip_output,
                 )
             except ValueError as e:
-                if str(e).startswith("NELECT") and potcar_spec:
-                    with zopen(os.path.join(output_path, "POTCAR.spec"), "wt") as pot_spec_file:
-                        pot_spec_file.write("\n".join(self.potcar_symbols))
+                if not str(e).startswith("NELECT") or not potcar_spec:
+                    raise e
 
-                    self.kpoints.write_file(f"{output_path}/KPOINTS")
-                    self.poscar.write_file(f"{output_path}/POSCAR")
+                with zopen(os.path.join(output_path, "POTCAR.spec"), "wt") as pot_spec_file:
+                    pot_spec_file.write("\n".join(self.potcar_symbols))
+
+                self.kpoints.write_file(f"{output_path}/KPOINTS")
+                self.poscar.write_file(f"{output_path}/POSCAR")
 
         else:  # use `write_file()`s rather than `write_input()` to avoid writing POSCARs/POTCARs
             os.makedirs(output_path, exist_ok=True)
 
             # if not POTCARs and charge_state not 0, but unperturbed POSCAR is true, then skip INCAR
             # write attempt (unperturbed POSCARs and KPOINTS will be written, and user already warned):
             if potcars or self.charge_state == 0 or not unperturbed_poscar:
@@ -1178,15 +1180,15 @@
 
         # check NKRED by running through ``vasp_nkred_std``:
         nkred_defect_dict_set = self.vasp_nkred_std
 
         if nkred_defect_dict_set is None:
             return None
 
-        if nkred_defect_dict_set._check_user_potcars(unperturbed_poscar=True, snb=False):
+        if any("VASP_PSP_DIR" in i for i in SETTINGS):  # POTCARs available
             user_incar_settings = copy.deepcopy(self.user_incar_settings)
             user_incar_settings.update(singleshot_incar_settings)
             user_incar_settings.update(  # add NKRED settings
                 {k: v for k, v in nkred_defect_dict_set.incar.as_dict().items() if "NKRED" in k}
             )
         else:
             user_incar_settings = {}
```

### Comparing `doped-2.4.0/doped.egg-info/PKG-INFO` & `doped-2.4.1/doped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doped
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python package to setup, process and analyse solid-state defect calculations with VASP
 Author-email: Seán Kavanagh <skavanagh@seas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2021 Seán Kavanagh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -91,15 +91,16 @@
 - **Thermodynamic Analysis**: Compute (non-)equilibrium Fermi levels, defect/carrier concentrations etc. as functions of annealing/cooling temperature, chemical potentials etc.
 - **Plotting**: Generate publication-quality plots of defect formation energies, chemical potential limits, defect/carrier concentrations, Fermi levels, charge corrections, etc.
 - **`Python` Interface**: Fully-customisable, modular `Python` API. Plug-and-play w/[`ShakeNBreak`](https://shakenbreak.readthedocs.io) – [defect structure-searching](https://www.nature.com/articles/s41524-023-00973-1), [`easyunfold`](https://smtg-bham.github.io/easyunfold/) – band unfolding, [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/[`nonrad`](https://nonrad.readthedocs.io/en/latest/) – non-radiative recombination etc.
 - Reproducibility, tabulation, automated compatibility/sanity checking, strain/displacement analysis, shallow defect analysis, high-throughput compatibility, Wyckoff analysis...
 
 ### Performance and Example Outputs
 ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/doped_JOSS_figure.png)
-**a.** Optimal supercell generation comparison. **b.** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
+**(a)** Optimal supercell generation comparison. **(b)** Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-size correction plot, **(d)** defect formation energy diagram, **(e)** chemical potential / stability region, **(f)** Fermi level vs. annealing temperature, **(g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi level / carrier concentration heatmap plots from `doped`. Automated plots of **(i,j)** single-particle eigenvalues and **(k)** site
+displacements from DFT supercell calculations. See the [JOSS paper](https://github.com/openjournals/joss-reviews/issues/6433) for more details.
 <!-- Update this link!! -->
 
 ## Installation
 ```bash
 pip install doped  # install doped and dependencies
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: doped Version: 2.4.0 Summary: Python package to
+Metadata-Version: 2.1 Name: doped Version: 2.4.1 Summary: Python package to
 setup, process and analyse solid-state defect calculations with VASP Author-
 email: SeÃ¡n Kavanagh
 seas.harvard.edu> License: MIT License Copyright (c) 2021 SeÃ¡n Kavanagh
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -76,32 +76,34 @@
 (https://smtg-bham.github.io/easyunfold/) â band unfolding,
 [`CarrierCapture.jl`](https://github.com/WMD-group/CarrierCapture.jl)/
 [`nonrad`](https://nonrad.readthedocs.io/en/latest/) â non-radiative
 recombination etc. - Reproducibility, tabulation, automated compatibility/
 sanity checking, strain/displacement analysis, shallow defect analysis, high-
 throughput compatibility, Wyckoff analysis... ### Performance and Example
 Outputs ![https://github.com/openjournals/joss-reviews/issues/6433](docs/JOSS/
-doped_JOSS_figure.png) **a.** Optimal supercell generation comparison. **b.**
+doped_JOSS_figure.png) **(a)** Optimal supercell generation comparison. **(b)**
 Charge state estimation comparison. Example **(c)** Kumagai-Oba (eFNV) finite-
 size correction plot, **(d)** defect formation energy diagram, **(e)** chemical
 potential / stability region, **(f)** Fermi level vs. annealing temperature, **
 (g)** defect/carrier concentrations vs. annealing temperature and **(h)** Fermi
-level / carrier concentration heatmap plots from `doped`. See the [JOSS paper]
-(https://github.com/openjournals/joss-reviews/issues/6433) for more details. ##
-Installation ```bash pip install doped # install doped and dependencies ```
-Alternatively if desired, `doped` can also be installed from `conda` with:
-```bash conda install -c conda-forge doped pip install pydefect # pydefect not
-available on conda, so needs to be installed with pip or otherwise, if using
-the eFNV correction ``` If you haven't done so already, you will need to set up
-your VASP `POTCAR` files and `Materials Project` API with `pymatgen` using the
-`.pmgrc.yaml` file, in order for `doped` to automatically generate VASP input
-files for defect calculations and determine competing phases for chemical
-potentials. See the docs [Installation](https://doped.readthedocs.io/en/latest/
-Installation.html) page for details on this. ## `ShakeNBreak` As shown in the
-`doped` tutorials, it is highly recommended to use the [`ShakeNBreak`](https://
+level / carrier concentration heatmap plots from `doped`. Automated plots of **
+(i,j)** single-particle eigenvalues and **(k)** site displacements from DFT
+supercell calculations. See the [JOSS paper](https://github.com/openjournals/
+joss-reviews/issues/6433) for more details. ## Installation ```bash pip install
+doped # install doped and dependencies ``` Alternatively if desired, `doped`
+can also be installed from `conda` with: ```bash conda install -c conda-forge
+doped pip install pydefect # pydefect not available on conda, so needs to be
+installed with pip or otherwise, if using the eFNV correction ``` If you
+haven't done so already, you will need to set up your VASP `POTCAR` files and
+`Materials Project` API with `pymatgen` using the `.pmgrc.yaml` file, in order
+for `doped` to automatically generate VASP input files for defect calculations
+and determine competing phases for chemical potentials. See the docs
+[Installation](https://doped.readthedocs.io/en/latest/Installation.html) page
+for details on this. ## `ShakeNBreak` As shown in the `doped` tutorials, it is
+highly recommended to use the [`ShakeNBreak`](https://
 shakenbreak.readthedocs.io/en/latest/) approach when calculating point defects
 in solids, to ensure you have identified the groundstate structures of your
 defects. As detailed in the [theory paper](https://doi.org/10.1038/s41524-023-
 00973-1), skipping this step can result in drastically incorrect formation
 energies, transition levels, carrier capture (basically any property associated
 with defects). This approach is followed in the [doped example notebook](https:
 //github.com/SMTG-Bham/doped/blob/main/dope_workflow_example.ipynb), with a
```

### Comparing `doped-2.4.0/doped.egg-info/SOURCES.txt` & `doped-2.4.1/doped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/pyproject.toml` & `doped-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doped"
-version = "2.4.0"
+version = "2.4.1"
 description = "Python package to setup, process and analyse solid-state defect calculations with VASP"
 authors = [{name = "Seán Kavanagh", email = "skavanagh@seas.harvard.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `doped-2.4.0/tests/test_analysis.py` & `doped-2.4.1/tests/test_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from unittest.mock import patch
 
 import matplotlib as mpl
 import numpy as np
 import pytest
 from monty.serialization import dumpfn, loadfn
 from pymatgen.core.structure import Structure
-from test_generation import _potcars_available
 from test_thermodynamics import custom_mpl_image_compare
 
 from doped.analysis import (
     DefectParser,
     DefectsParser,
     defect_entry_from_paths,
     defect_from_structures,
@@ -607,21 +606,21 @@
 
         assert all(
             any(i in str(warn.message) for warn in w)
             for i in [
                 "Estimated error in the Freysoldt (FNV) ",
                 "Estimated error in the Kumagai (eFNV) ",
                 "charge correction for certain defects is greater than the `error_tolerance` (= "
-                "0.001 eV):",
-                "v_Cd_-2: 0.011 eV",
-                "v_Cd_-1: 0.008 eV",
-                "Int_Te_3_1: 0.003 eV",
-                "Te_Cd_+1: 0.002 eV",
-                "Int_Te_3_Unperturbed_1: 0.005 eV",
-                "Int_Te_3_2: 0.012 eV",
+                "1.00e-03 eV):",
+                "v_Cd_-2: 1.13e-02 eV",
+                "v_Cd_-1: 7.91e-03 eV",
+                "Int_Te_3_1: 3.10e-03 eV",
+                "Te_Cd_+1: 2.02e-03 eV",
+                "Int_Te_3_Unperturbed_1: 4.91e-03 eV",
+                "Int_Te_3_2: 1.24e-02 eV",
                 "You may want to check the accuracy of the corrections by",
                 "(using `defect_entry.get_freysoldt_correction()` with `plot=True`)",
                 "(using `defect_entry.get_kumagai_correction()` with `plot=True`)",
             ]
         )  # correction errors warnings
 
     @custom_mpl_image_compare(filename="YTOS_example_defects_plot.png")
@@ -768,16 +767,35 @@
                     "The calculated finite-size charge corrections for defect at",
                     "sum to a _negative_ value of -0.144.",
                 ]
             )
             for warn in w
         )
 
+        # spot check:
+        assert np.isclose(Sb2Se3_O_thermo.get_formation_energy("O_Se_Cs_Sb2.02_-2"), -1.84684, atol=1e-3)
+
         return Sb2Se3_O_thermo.plot(chempots={"O": -8.9052, "Se": -5})  # example chempots
 
+    def test_extrinsic_Sb2Se3_parsing_with_single_defect_dir(self):
+        with warnings.catch_warnings(record=True) as w:  # no warning about negative corrections with
+            # strong anisotropic dielectric:
+            Sb2Se3_O_dp = DefectsParser(
+                output_path=f"{self.Sb2Se3_DATA_DIR}/defect/O_-2",
+                bulk_path=f"{self.Sb2Se3_DATA_DIR}/bulk",
+                dielectric=self.Sb2Se3_dielectric,
+            )
+        print([warn.message for warn in w])  # for debugging
+        assert not w  # no warnings
+        self._check_DefectsParser(Sb2Se3_O_dp)
+        Sb2Se3_O_thermo = Sb2Se3_O_dp.get_defect_thermodynamics()
+        assert np.isclose(Sb2Se3_O_thermo.get_formation_energy("O_Se_Cs_Sb2.02_-2"), -1.84684, atol=1e-3)
+
+        assert len(Sb2Se3_O_thermo.defect_entries) == 1  # only the one specified defect parsed
+
     @custom_mpl_image_compare(filename="Sb2Si2Te6_v_Sb_-3_eFNV_plot_no_intralayer.png")
     def test_sb2si2te6_eFNV(self):
         with warnings.catch_warnings(record=True) as w:
             dp = DefectsParser(
                 self.Sb2Si2Te6_DATA_DIR,
                 dielectric=self.Sb2Si2Te6_dielectric,
                 json_filename="Sb2Si2Te6_example_defect_dict.json",  # testing in test_thermodynamics.py
@@ -1047,16 +1065,15 @@
         relaxed symmetry determination scheme with old default of
         ``symprec=0.2``).
         """
         with warnings.catch_warnings(record=True) as w:
             dp = DefectsParser(
                 output_path=self.CaO_DATA_DIR,
                 skip_corrections=True,
-                parse_projected_eigen=bool(_potcars_available()),
-            )  # only test projected eigenvalues if POTCARs available (i.e. locally) to save time
+            )
 
         print([str(warning.message) for warning in w])  # for debugging
         assert not w
         assert len(dp.defect_dict) == 4
         self._check_DefectsParser(dp, skip_corrections=True)
 
         # some hardcoded symmetry tests with default `symprec = 0.1` for relaxed structures:
@@ -1911,16 +1928,16 @@
                 defect_path=defect_path,
                 bulk_path=f"{self.YTOS_EXAMPLE_DIR}/Bulk/",
                 dielectric=self.ytos_dielectric,
                 error_tolerance=0.001,
             )
         assert (
             f"Estimated error in the Kumagai (eFNV) charge correction for defect "
-            f"{int_F_minus1_ent.name} is 0.003 eV (i.e. which is greater than the `error_tolerance`: "
-            f"0.001 eV). You may want to check the accuracy of the correction by plotting the site "
+            f"{int_F_minus1_ent.name} is 2.58e-03 eV (i.e. which is greater than the `error_tolerance`: "
+            f"1.00e-03 eV). You may want to check the accuracy of the correction by plotting the site "
             f"potential differences (using `defect_entry.get_kumagai_correction()` with "
             f"`plot=True`). Large errors are often due to unstable or shallow defect charge states ("
             f"which can't be accurately modelled with the supercell approach; see "
             f"https://doped.readthedocs.io/en/latest/Tips.html#perturbed-host-states). If this error is "
             f"not acceptable, you may need to use a larger supercell for more accurate energies."
             in str(w[0].message)
         )
@@ -2006,16 +2023,16 @@
                 dielectric=self.ytos_dielectric,
                 error_tolerance=0.00001,
                 parse_projected_eigen=False,
             )  # check no correction error warning with default tolerance:
         print([str(warn.message) for warn in w])
         assert any(
             f"Estimated error in the Freysoldt (FNV) charge correction for defect {F_O_1_ent.name} is "
-            f"0.000 eV (i.e. which is greater than the `error_tolerance`: 0.000 eV). You may want to "
-            f"check the accuracy of the correction by plotting the site potential differences (using "
+            f"3.54e-04 eV (i.e. which is greater than the `error_tolerance`: 1.00e-05 eV). You may want "
+            f"to check the accuracy of the correction by plotting the site potential differences (using "
             f"`defect_entry.get_freysoldt_correction()` with `plot=True`). Large errors are often due "
             f"to unstable or shallow defect charge states (which can't be accurately modelled with "
             f"the supercell approach; see "
             f"https://doped.readthedocs.io/en/latest/Tips.html#perturbed-host-states). "
             f"If this error is not acceptable, you may need to use a larger supercell for more "
             f"accurate energies." in str(warning.message)
             for warning in w
@@ -2250,61 +2267,14 @@
                     d[key][i] = _remove_metadata_keys_from_dict(item)
         elif isinstance(d[key], dict):
             d[key] = _remove_metadata_keys_from_dict(d[key])
 
     return d
 
 
-def _compare_band_edge_states_dicts(d1, d2, orb_diff_tol: float = 0.1):
-    """
-    Compare two dictionaries of band edge states, removing metadata keys and
-    allowing a slight difference in the ``vbm/cbm_orbital_diff`` values to
-    account for rounding errors with ``PROCAR``s.
-    """
-    if isinstance(d1, str):
-        d1 = loadfn(d1)
-    if isinstance(d2, str):
-        d2 = loadfn(d2)
-
-    d1 = d1.as_dict()
-    d2 = d2.as_dict()
-
-    cbm_orbital_diffs1 = [subdict.pop("cbm_orbital_diff") for subdict in d1["states"]]
-    cbm_orbital_diffs2 = [subdict.pop("cbm_orbital_diff") for subdict in d2["states"]]
-    for i, j in zip(cbm_orbital_diffs1, cbm_orbital_diffs2):
-        print(f"cbm_orbital_diffs: {i:.3f} vs {j:.3f}")
-        assert np.isclose(i, j, atol=orb_diff_tol)
-    vbm_orbital_diffs1 = [subdict.pop("vbm_orbital_diff") for subdict in d1["states"]]
-    vbm_orbital_diffs2 = [subdict.pop("vbm_orbital_diff") for subdict in d2["states"]]
-    for i, j in zip(vbm_orbital_diffs1, vbm_orbital_diffs2):
-        print(f"vbm_orbital_diffs: {i:.3f} vs {j:.3f}")
-        assert np.isclose(i, j, atol=orb_diff_tol)
-
-    orb_infos_orbitals1 = [
-        subdict["vbm_info"]["orbital_info"].pop("orbitals") for subdict in d1["states"]
-    ] + [subdict["cbm_info"]["orbital_info"].pop("orbitals") for subdict in d1["states"]]
-    orb_infos_orbitals2 = [
-        subdict["vbm_info"]["orbital_info"].pop("orbitals") for subdict in d2["states"]
-    ] + [subdict["cbm_info"]["orbital_info"].pop("orbitals") for subdict in d2["states"]]
-    for i, j in zip(orb_infos_orbitals1, orb_infos_orbitals2):
-        print(f"orbital_info_orbitals: {i} vs {j}")
-        for k, v in i.items():
-            assert np.allclose(v, j[k], atol=orb_diff_tol)
-
-    participation_ratio1 = [
-        subdict["vbm_info"]["orbital_info"].pop("participation_ratio") for subdict in d1["states"]
-    ] + [subdict["cbm_info"]["orbital_info"].pop("participation_ratio") for subdict in d1["states"]]
-    participation_ratio2 = [
-        subdict["vbm_info"]["orbital_info"].pop("participation_ratio") for subdict in d2["states"]
-    ] + [subdict["cbm_info"]["orbital_info"].pop("participation_ratio") for subdict in d2["states"]]
-    assert np.allclose(participation_ratio1, participation_ratio2, atol=orb_diff_tol)
-
-    assert _remove_metadata_keys_from_dict(d1) == _remove_metadata_keys_from_dict(d2)
-
-
 class DopedParsingFunctionsTestCase(unittest.TestCase):
     def setUp(self):
         DopedParsingTestCase.setUp(self)  # get attributes from DopedParsingTestCase
         self.data_dir = os.path.join(os.path.dirname(__file__), "data")
         self.prim_cdte = Structure.from_file(f"{self.EXAMPLE_DIR}/CdTe/relaxed_primitive_POSCAR")
         self.ytos_bulk_supercell = Structure.from_file(f"{self.EXAMPLE_DIR}/YTOS/Bulk/POSCAR")
         self.lmno_primitive = Structure.from_file(f"{self.data_dir}/Li2Mn3NiO8_POSCAR")
@@ -2719,27 +2689,101 @@
     def test_eigenvalues_parsing_and_warnings(self):
         """
         Test eigenvalues functions.
 
         Print statements added because dict comparison doesn't give verbose
         output on exact location of failure.
         """
+
+        def _compare_band_edge_states_dicts(d1, d2, orb_diff_tol: float = 0.1):
+            """
+            Compare two dictionaries of band edge states, removing metadata
+            keys and allowing a slight difference in the
+            ``vbm/cbm_orbital_diff`` values to account for rounding errors with
+            ``PROCAR``s.
+            """
+            if isinstance(d1, str):
+                d1 = loadfn(d1)
+            if isinstance(d2, str):
+                d2 = loadfn(d2)
+
+            d1 = d1.as_dict()
+            d2 = d2.as_dict()
+
+            cbm_orbital_diffs1 = [subdict.pop("cbm_orbital_diff") for subdict in d1["states"]]
+            cbm_orbital_diffs2 = [subdict.pop("cbm_orbital_diff") for subdict in d2["states"]]
+            for i, j in zip(cbm_orbital_diffs1, cbm_orbital_diffs2):
+                print(f"cbm_orbital_diffs: {i:.3f} vs {j:.3f}")
+                assert np.isclose(i, j, atol=orb_diff_tol)
+            vbm_orbital_diffs1 = [subdict.pop("vbm_orbital_diff") for subdict in d1["states"]]
+            vbm_orbital_diffs2 = [subdict.pop("vbm_orbital_diff") for subdict in d2["states"]]
+            for i, j in zip(vbm_orbital_diffs1, vbm_orbital_diffs2):
+                print(f"vbm_orbital_diffs: {i:.3f} vs {j:.3f}")
+                assert np.isclose(i, j, atol=orb_diff_tol)
+
+            orb_infos_orbitals1 = [
+                subdict["vbm_info"]["orbital_info"].pop("orbitals") for subdict in d1["states"]
+            ] + [subdict["cbm_info"]["orbital_info"].pop("orbitals") for subdict in d1["states"]]
+            orb_infos_orbitals2 = [
+                subdict["vbm_info"]["orbital_info"].pop("orbitals") for subdict in d2["states"]
+            ] + [subdict["cbm_info"]["orbital_info"].pop("orbitals") for subdict in d2["states"]]
+            for i, j in zip(orb_infos_orbitals1, orb_infos_orbitals2):
+                print(f"orbital_info_orbitals: {i} vs {j}")
+                for k, v in i.items():
+                    assert np.allclose(v, j[k], atol=orb_diff_tol)
+
+            participation_ratio1 = (
+                [
+                    subdict["vbm_info"]["orbital_info"].pop("participation_ratio")
+                    for subdict in d1["states"]
+                ]
+                + [
+                    subdict["cbm_info"]["orbital_info"].pop("participation_ratio")
+                    for subdict in d1["states"]
+                ]
+                + [
+                    subsubdict.pop("participation_ratio")
+                    for subdict in d1["states"]
+                    for subsubdict in subdict["localized_orbitals"]
+                ]
+            )
+
+            participation_ratio2 = (
+                [
+                    subdict["vbm_info"]["orbital_info"].pop("participation_ratio")
+                    for subdict in d2["states"]
+                ]
+                + [
+                    subdict["cbm_info"]["orbital_info"].pop("participation_ratio")
+                    for subdict in d2["states"]
+                ]
+                + [
+                    subsubdict.pop("participation_ratio")
+                    for subdict in d2["states"]
+                    for subsubdict in subdict["localized_orbitals"]
+                ]
+            )
+            print(f"participation_ratio: {participation_ratio1} vs {participation_ratio2}")
+            assert np.allclose(participation_ratio1, participation_ratio2, atol=orb_diff_tol)
+
+            assert _remove_metadata_keys_from_dict(d1) == _remove_metadata_keys_from_dict(d2)
+
         # Test loading of MgO using vasprun.xml
         defect_entry = DefectParser.from_paths(
             f"{self.MgO_EXAMPLE_DIR}/Defects/Mg_O_+1/vasp_std",
             f"{self.MgO_EXAMPLE_DIR}/Defects/MgO_bulk/vasp_std",
             skip_corrections=True,
             parse_projected_eigen=True,
         ).defect_entry
 
         print("Testing MgO eigenvalue analysis")
         bes, fig = defect_entry.get_eigenvalue_analysis()  # Test plotting KS
         Mg_O_1_bes_path = f"{self.MgO_EXAMPLE_DIR}/Defects/Mg_O_1_band_edge_states.json"
         # dumpfn(bes, Mg_O_1_bes_path)  # for saving test data
-        _compare_band_edge_states_dicts(bes, Mg_O_1_bes_path, orb_diff_tol=0.001)
+        _compare_band_edge_states_dicts(bes, Mg_O_1_bes_path, orb_diff_tol=0.01)
         assert bes.has_occupied_localized_state
         assert not any(
             [bes.has_acceptor_phs, bes.has_donor_phs, bes.has_unoccupied_localized_state, bes.is_shallow]
         )
 
         # Test loading using ``DefectsParser``
         print("Testing Cu2SiSe3 eigenvalue analysis default, with vaspruns (& PROCARs)")
@@ -2767,15 +2811,15 @@
             [bes.has_donor_phs, bes.has_occupied_localized_state, bes.has_unoccupied_localized_state]
         )
 
         print("Testing Si_i_-1 with plot = True")
         bes = dp.defect_dict["Si_i_-1"].get_eigenvalue_analysis(plot=False)
         Si_i_m1_bes_path = f"{self.Cu2SiSe3_EXAMPLE_DIR}/Cu2SiSe3_int_band_edge_states.json"
         # dumpfn(bes, Si_i_m1_bes_path)  # for saving test data
-        _compare_band_edge_states_dicts(bes, Si_i_m1_bes_path, orb_diff_tol=0.001)
+        _compare_band_edge_states_dicts(bes, Si_i_m1_bes_path, orb_diff_tol=0.01)
         assert bes.has_occupied_localized_state
         assert not any(
             [bes.has_acceptor_phs, bes.has_donor_phs, bes.has_unoccupied_localized_state, bes.is_shallow]
         )
 
         # test parses fine without projected eigenvalues from vaspruns:
         print("Testing Cu2SiSe3 parsing and eigenvalue analysis with bulk vr, no projected eigenvalues")
@@ -2849,15 +2893,15 @@
             parse_projected_eigen=True,
         ).defect_entry
 
         print("Testing Int_Te_3_1 with plot = True")
         bes = defect_entry.get_eigenvalue_analysis(plot=False)
         Te_i_1_SOC_bes_path = f"{self.CdTe_EXAMPLE_DIR}/CdTe_test_soc_band_edge_states.json"
         # dumpfn(bes, Te_i_1_SOC_bes_path)  # for saving test data
-        _compare_band_edge_states_dicts(bes, Te_i_1_SOC_bes_path, orb_diff_tol=0.001)
+        _compare_band_edge_states_dicts(bes, Te_i_1_SOC_bes_path, orb_diff_tol=0.02)
         assert bes.has_unoccupied_localized_state
         assert not any(
             [bes.has_acceptor_phs, bes.has_donor_phs, bes.has_occupied_localized_state, bes.is_shallow]
         )
 
         # Test warning for no projected orbitals: Sb2Se3 data
         print("Testing Sb2Se3 parsing and warning; no projected orbital data")
@@ -2866,15 +2910,15 @@
                 f"{self.Sb2Se3_DATA_DIR}/defect/O_1",
                 f"{self.Sb2Se3_DATA_DIR}/bulk",
                 skip_corrections=True,
                 parse_projected_eigen=True,
             )
 
         print([str(warning.message) for warning in w])  # for debugging
-        assert any("with projected orbitals in path" in str(warning.message) for warning in w)
+        assert any("Could not parse eigenvalue data" in str(warning.message) for warning in w)
 
         # Test no warning for no projected orbitals with default ``parse_projected_eigen=None`` (attempt
         # but don't warn): Sb2Se3 data
         print("Testing Sb2Se3 parsing and warning; no warning with default settings")
         with warnings.catch_warnings(record=True) as w:
             DefectParser.from_paths(
                 f"{self.Sb2Se3_DATA_DIR}/defect/O_1",
```

### Comparing `doped-2.4.0/tests/test_chemical_potentials.py` & `doped-2.4.1/tests/test_chemical_potentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,17 +59,21 @@
         self.ext_cpa = chemical_potentials.CompetingPhasesAnalyzer(
             self.stable_system, self.extrinsic_species
         )
         self.ext_cpa.from_csv(self.csv_path_ext)
 
         assert len(stable_cpa.elemental) == 2
         assert len(self.ext_cpa.elemental) == 3
-        assert any(entry["formula"] == "O2" for entry in stable_cpa.data)
+        assert any(entry["Formula"] == "O2" for entry in stable_cpa.data)
         assert np.isclose(
-            next(entry["energy_per_fu"] for entry in self.ext_cpa.data if entry["formula"] == "La2Zr2O7"),
+            next(
+                entry["DFT Energy (eV/fu)"]
+                for entry in self.ext_cpa.data
+                if entry["Formula"] == "La2Zr2O7"
+            ),
             -119.619571095,
         )
 
     # test chempots
     def test_cpa_chempots(self):
         stable_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         stable_cpa.from_csv(self.csv_path)
@@ -84,15 +88,15 @@
             self.unstable_cpa.calculate_chempots()
 
         self.ext_cpa = chemical_potentials.CompetingPhasesAnalyzer(
             self.stable_system, self.extrinsic_species
         )
         self.ext_cpa.from_csv(self.csv_path_ext)
         chempot_df = self.ext_cpa.calculate_chempots()
-        assert next(iter(chempot_df["La_limiting_phase"])) == "La2Zr2O7"
+        assert next(iter(chempot_df["La-Limiting Phase"])) == "La2Zr2O7"
         assert np.isclose(next(iter(chempot_df["La"])), -9.46298748)
 
     def test_ext_cpa_chempots(self):
         # test accessing cpa.chempots without previously calling cpa.calculate_chempots()
         stable_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         stable_cpa.from_csv(self.csv_path)
         _compare_chempot_dicts(stable_cpa.chempots, self.parsed_chempots)
@@ -103,42 +107,42 @@
         self.ext_cpa.from_csv(self.csv_path_ext)
         assert self.ext_cpa.chempots["elemental_refs"] == self.parsed_ext_chempots["elemental_refs"]
 
     def test_sort_by(self):
         stable_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         stable_cpa.from_csv(self.csv_path)
         chempot_df = stable_cpa.calculate_chempots(sort_by="Zr")
-        assert np.isclose(next(iter(chempot_df["Zr"])), -0.199544)
-        assert np.isclose(list(chempot_df["Zr"])[1], -10.975428439999998)
+        assert np.isclose(next(iter(chempot_df["Zr"])), -0.199544, atol=1e-4)
+        assert np.isclose(list(chempot_df["Zr"])[1], -10.975428439999998, atol=1e-4)
 
         with pytest.raises(KeyError):
             stable_cpa.calculate_chempots(sort_by="M")
 
     # test vaspruns
     def test_vaspruns(self):
         cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         path = self.path / "ZrO2"
         cpa.from_vaspruns(path=path, folder="relax", csv_path=self.csv_path)
         assert len(cpa.elemental) == 2
-        assert cpa.data[0]["formula"] == "O2"
+        assert cpa.data[0]["Formula"] == "O2"
 
         cpa_no = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         with pytest.raises(FileNotFoundError):
             cpa_no.from_vaspruns(path="path")
 
         with pytest.raises(ValueError):
             cpa_no.from_vaspruns(path=0)
 
         ext_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system, self.extrinsic_species)
         path2 = self.path / "La_ZrO2"
         ext_cpa.from_vaspruns(path=path2, folder="relax", csv_path=self.csv_path_ext)
         assert len(ext_cpa.elemental) == 3
         # sorted by num_species, then alphabetically, then by num_atoms_in_fu, then by
         # formation_energy
-        assert [entry["formula"] for entry in ext_cpa.data] == [
+        assert [entry["Formula"] for entry in ext_cpa.data] == [
             "La",
             "O2",
             "Zr",
             "Zr",
             "La2O3",
             "Zr2O",
             "Zr3O",
@@ -167,26 +171,29 @@
         # 'formation_energy': -5.935114089999992}, {'formula': 'ZrO2', 'kpoints': '3x3x3',
         # 'energy_per_fu': -34.83230881, 'energy_per_atom': -11.610769603333333, 'energy':
         # -139.32923524, 'formation_energy': -10.975428440000002}, {'formula': 'ZrO2', 'kpoints':
         # '3x3x1', 'energy_per_fu': -34.807990365, 'energy_per_atom': -11.602663455, 'energy':
         # -278.46392292, 'formation_energy': -10.951109995000003}, {'formula': 'La2Zr2O7',
         # 'kpoints': '3x3x3', 'energy_per_fu': -119.619571095, 'energy_per_atom':
         # -10.874506463181818, 'energy': -239.23914219, 'formation_energy': -40.87683184}]
-        assert np.isclose(ext_cpa.data[0]["energy_per_fu"], -5.00458616)
-        assert np.isclose(ext_cpa.data[0]["energy_per_atom"], -5.00458616)
-        assert np.isclose(ext_cpa.data[0]["energy"], -20.01834464)
-        assert np.isclose(ext_cpa.data[0]["formation_energy"], 0.0)
-        assert np.isclose(ext_cpa.data[-1]["energy_per_fu"], -119.619571095)
-        assert np.isclose(ext_cpa.data[-1]["energy_per_atom"], -10.874506463181818)
-        assert np.isclose(ext_cpa.data[-1]["energy"], -239.23914219)
-        assert np.isclose(ext_cpa.data[-1]["formation_energy"], -40.87683184)
-        assert np.isclose(ext_cpa.data[6]["energy_per_fu"], -42.524204305)
-        assert np.isclose(ext_cpa.data[6]["energy_per_atom"], -10.63105107625)
-        assert np.isclose(ext_cpa.data[6]["energy"], -85.04840861)
-        assert np.isclose(ext_cpa.data[6]["formation_energy"], -5.986573519999993)
+        assert np.isclose(ext_cpa.data[0]["DFT Energy (eV/fu)"], -5.00458616)
+        assert np.isclose(ext_cpa.data[0]["DFT Energy (eV/atom)"], -5.00458616)
+        assert np.isclose(ext_cpa.data[0]["DFT Energy (eV)"], -20.01834464)
+        assert np.isclose(ext_cpa.data[0]["Formation Energy (eV/fu)"], 0.0)
+        assert np.isclose(ext_cpa.data[0]["Formation Energy (eV/atom)"], 0.0)
+        assert np.isclose(ext_cpa.data[-1]["DFT Energy (eV/fu)"], -119.619571095)
+        assert np.isclose(ext_cpa.data[-1]["DFT Energy (eV/atom)"], -10.874506463181818)
+        assert np.isclose(ext_cpa.data[-1]["DFT Energy (eV)"], -239.23914219)
+        assert np.isclose(ext_cpa.data[-1]["Formation Energy (eV/fu)"], -40.87683184)
+        assert np.isclose(ext_cpa.data[-1]["Formation Energy (eV/atom)"], -40.87683184 / 11)
+        assert np.isclose(ext_cpa.data[6]["DFT Energy (eV/fu)"], -42.524204305)
+        assert np.isclose(ext_cpa.data[6]["DFT Energy (eV/atom)"], -10.63105107625)
+        assert np.isclose(ext_cpa.data[6]["DFT Energy (eV)"], -85.04840861)
+        assert np.isclose(ext_cpa.data[6]["Formation Energy (eV/fu)"], -5.986573519999993)
+        assert np.isclose(ext_cpa.data[6]["Formation Energy (eV/atom)"], -5.986573519999993 / 4)
 
         # check if it works from a list
         all_paths = []
         for p in path.iterdir():
             if not p.name.startswith("."):
                 pp = p / "relax" / "vasprun.xml"
                 ppgz = p / "relax" / "vasprun.xml.gz"
@@ -243,21 +250,21 @@
 
         with open("input.dat", encoding="utf-8") as file:
             contents = file.readlines()
 
         # assert these lines are in the file:
         for i in [
             "2  # number of elements in bulk\n",
-            "1 Zr 2 O -10.975428440000002  # num_atoms, element, formation_energy (bulk)\n",
+            "1 Zr 2 O -10.975428440000002  # number of atoms, element, formation energy (bulk)\n",
             "O  # dependent variable (element)\n",
             "2  # number of bordering phases\n",
             "1  # number of elements in phase:\n",
-            "2 O 0.0  # num_atoms, element, formation_energy\n",
+            "2 O 0.0  # number of atoms, element, formation energy\n",
             "2  # number of elements in phase:\n",
-            "3 Zr 1 O -5.986573519999993  # num_atoms, element, formation_energy\n",
+            "3 Zr 1 O -5.986573519999993  # number of atoms, element, formation energy\n",
         ]:
             assert i in contents
 
         assert (
             "1 Zr 2 O -10.951109995000005\n" not in contents
         )  # shouldn't be included as is a higher energy polymorph of the bulk phase
         assert all("2 Zr 1 O" not in i for i in contents)  # non-bordering phase
@@ -266,36 +273,50 @@
         cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         path = self.path / "ZrO2"
         cpa.from_vaspruns(path=path, folder="relax", csv_path=self.csv_path)
 
         string = cpa.to_LaTeX_table(splits=1)
         assert (
             string[28:209]
-            == "\\caption{Formation energies ($\\Delta E_f$) per formula unit of \\ce{ZrO2} and all "
+            == "\\caption{Formation energies per formula unit ($\\Delta E_f$) of \\ce{ZrO2} and all "
             "competing phases, with k-meshes used in calculations. Only the lowest energy polymorphs "
             "are included"
         )
-        assert len(string) == 586
-        assert string.split("hline")[1] == "\nFormula & k-mesh & $\\Delta E_f$ (eV) \\\\ \\"
+        assert len(string) == 589
+        assert string.split("hline")[1] == "\nFormula & k-mesh & $\\Delta E_f$ (eV/fu) \\\\ \\"
         assert string.split("hline")[2][2:45] == "\\ce{ZrO2} & 3$\\times$3$\\times$3 & -10.975 \\"
 
         string = cpa.to_LaTeX_table(splits=2)
         assert (
             string[28:209]
-            == "\\caption{Formation energies ($\\Delta E_f$) per formula unit of \\ce{ZrO2} and all "
+            == "\\caption{Formation energies per formula unit ($\\Delta E_f$) of \\ce{ZrO2} and all "
             "competing phases, with k-meshes used in calculations. Only the lowest energy polymorphs "
             "are included"
         )
         assert (
             string.split("hline")[1]
-            == "\nFormula & k-mesh & $\\Delta E_f$ (eV) & Formula & k-mesh & $\\Delta E_f$ (eV)\\\\ \\"
+            == "\nFormula & k-mesh & $\\Delta E_f$ (eV/fu) & Formula & k-mesh & $\\Delta E_f$ ("
+            "eV/fu) \\\\ \\"
         )
 
         assert string.split("hline")[2][2:45] == "\\ce{ZrO2} & 3$\\times$3$\\times$3 & -10.975 &"
-        assert len(string) == 579
+        assert len(string) == 586
+
+        # test without kpoints:
+        for entry_dict in cpa.data:
+            entry_dict.pop("k-points")
+        string = cpa.to_LaTeX_table(splits=1)
+        assert (
+            string[28:173]
+            == "\\caption{Formation energies per formula unit ($\\Delta E_f$) of \\ce{ZrO2} and all "
+            "competing phases. Only the lowest energy polymorphs are included"
+        )
+        assert len(string) == 433
+        assert string.split("hline")[1] == "\nFormula & $\\Delta E_f$ (eV/fu) \\\\ \\"
+        assert string.split("hline")[2][2:23] == "\\ce{ZrO2} & -10.975 \\"
 
         cpa_csv = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         cpa_csv.from_csv(self.csv_path)
         with pytest.raises(ValueError):
             cpa_csv.to_LaTeX_table(splits=3)
 
     def test_to_csv(self):
@@ -304,15 +325,18 @@
         stable_cpa.from_csv(self.csv_path)
         stable_cpa_data = stable_cpa._get_and_sort_formation_energy_data()
 
         stable_cpa.to_csv("competing_phases.csv")
         reloaded_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         reloaded_cpa.from_csv("competing_phases.csv")
         reloaded_cpa_data = reloaded_cpa._get_and_sort_formation_energy_data()
-        assert pd.DataFrame(stable_cpa_data).equals(pd.DataFrame(reloaded_cpa_data))
+        print(
+            pd.DataFrame(stable_cpa_data).to_dict(), pd.DataFrame(reloaded_cpa_data).to_dict()
+        )  # for debugging
+        assert pd.DataFrame(stable_cpa_data).round(4).equals(pd.DataFrame(reloaded_cpa_data).round(4))
 
         # check chem limits the same:
         _compare_chempot_dicts(stable_cpa.chempots, reloaded_cpa.chempots)
 
         self.ext_cpa = chemical_potentials.CompetingPhasesAnalyzer(
             self.stable_system, self.extrinsic_species
         )
@@ -320,23 +344,25 @@
         self.ext_cpa.to_csv("competing_phases.csv")
         reloaded_ext_cpa = chemical_potentials.CompetingPhasesAnalyzer(
             self.stable_system, self.extrinsic_species
         )
         reloaded_ext_cpa.from_csv("competing_phases.csv")
         reloaded_ext_cpa._get_and_sort_formation_energy_data()
 
-        assert reloaded_ext_cpa.formation_energy_df.equals(self.ext_cpa.formation_energy_df)
+        assert reloaded_ext_cpa.formation_energy_df.round(4).equals(
+            self.ext_cpa.formation_energy_df.round(4)
+        )
 
         # test pruning:
         self.ext_cpa.to_csv("competing_phases.csv", prune_polymorphs=True)
         reloaded_ext_cpa.from_csv("competing_phases.csv")
         assert len(reloaded_ext_cpa.data) == 8  # polymorphs pruned
         assert len(self.ext_cpa.data) == 11
 
-        formulas = [i["formula"] for i in reloaded_ext_cpa.data]
+        formulas = [i["Formula"] for i in reloaded_ext_cpa.data]
         assert len(formulas) == len(set(formulas))  # no polymorphs
 
         reloaded_cpa.to_csv("competing_phases.csv", prune_polymorphs=True)
         reloaded_cpa.from_csv("competing_phases.csv")
 
         # check chem limits the same:
         _compare_chempot_dicts(reloaded_cpa.chempots, stable_cpa.chempots)
@@ -352,17 +378,19 @@
         reloaded_ext_cpa_energy_sorted = chemical_potentials.CompetingPhasesAnalyzer(
             self.stable_system, self.extrinsic_species
         )
         reloaded_ext_cpa_energy_sorted.from_csv("competing_phases.csv")
         assert len(reloaded_ext_cpa.data) == 8  # polymorphs pruned
 
         assert reloaded_ext_cpa_energy_sorted.data != reloaded_ext_cpa.data  # different order
-        sorted_data = sorted(reloaded_ext_cpa.data, key=lambda x: x["formation_energy"], reverse=True)
+        sorted_data = sorted(
+            reloaded_ext_cpa.data, key=lambda x: x["Formation Energy (eV/fu)"], reverse=True
+        )
         chemical_potentials._move_dict_to_start(
-            sorted_data, "formula", self.ext_cpa.bulk_composition.reduced_formula
+            sorted_data, "Formula", self.ext_cpa.bulk_composition.reduced_formula
         )
         assert reloaded_ext_cpa_energy_sorted.data == sorted_data  # energy sorted data
 
     def test_from_csv_minimal(self):
         """
         Test that CompetingPhasesAnalyzer.from_csv() works with minimal data.
         """
@@ -370,46 +398,49 @@
         cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         path = self.path / "ZrO2"
         cpa.from_vaspruns(path=path, folder="relax")
         formation_energy_data = cpa._get_and_sort_formation_energy_data()
         formation_energy_df = pd.DataFrame(formation_energy_data)
 
         # drop all but the formula and energy_per_fu columns:
-        for i in ["energy_per_fu", "energy_per_atom"]:
-            minimal_formation_energy_df = formation_energy_df[["formula", i]]
+        for i in ["DFT Energy (eV/fu)", "DFT Energy (eV/atom)"]:
+            minimal_formation_energy_df = formation_energy_df[["Formula", i]]
             minimal_formation_energy_df.to_csv("competing_phases.csv", index=False)
 
             reloaded_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
             reloaded_cpa.from_csv("competing_phases.csv")
-            assert not cpa.formation_energy_df.equals(
-                reloaded_cpa.formation_energy_df
+            assert not cpa.formation_energy_df.round(4).equals(
+                reloaded_cpa.formation_energy_df.round(4)
             )  # no kpoints or raw energy, but should have formula, energy_per_fu, energy_per_atom,
             # elemental amounts (i.e. Zr and O here) and formation_energy:
             minimal_columns = [
-                "formula",
-                "energy_per_fu",
-                "energy_per_atom",
-                "formation_energy",
+                "Formula",
+                "DFT Energy (eV/fu)",
+                "DFT Energy (eV/atom)",
+                "Formation Energy (eV/fu)",
+                "Formation Energy (eV/atom)",
                 "Zr",  # ordered by appearance in bulk composition
                 "O",
             ]
             trimmed_df = cpa.formation_energy_df[
                 [column for column in cpa.formation_energy_df.columns if column in minimal_columns]
             ]
             # trimmed_df is formation_energy_df with min columns but in same order as original
 
             trimmed_df = trimmed_df.round(5)  # round to avoid slight numerical differences
             reloaded_cpa.formation_energy_df = reloaded_cpa.formation_energy_df.round(5)
-            assert trimmed_df.equals(reloaded_cpa.formation_energy_df)
+            print(trimmed_df, reloaded_cpa.formation_energy_df)
+            print(trimmed_df.columns, reloaded_cpa.formation_energy_df.columns)
+            assert trimmed_df.round(4).equals(reloaded_cpa.formation_energy_df.round(4))
 
             # check chem limits the same:
             _compare_chempot_dicts(cpa.chempots, reloaded_cpa.chempots)
 
         # test ValueError without energy_per_fu/energy_per_atom column:
-        too_minimal_formation_energy_df = formation_energy_df[["formula"]]
+        too_minimal_formation_energy_df = formation_energy_df[["Formula"]]
         too_minimal_formation_energy_df.to_csv("competing_phases.csv", index=False)
         reloaded_cpa = chemical_potentials.CompetingPhasesAnalyzer(self.stable_system)
         with pytest.raises(ValueError) as exc:
             reloaded_cpa.from_csv("competing_phases.csv")
         assert "Supplied csv does not contain the minimal columns required" in str(exc.value)
 
 
@@ -425,58 +456,58 @@
 
 
 class FormationEnergyTestCase(unittest.TestCase):
     def test_fe(self):
         elemental = {"O": -7.006602065, "Zr": -9.84367624}
         data = [
             {
-                "formula": "O2",
-                "energy_per_fu": -14.01320413,
-                "energy_per_atom": -7.006602065,
-                "energy": -14.01320413,
+                "Formula": "O2",
+                "DFT Energy (eV/fu)": -14.01320413,
+                "DFT Energy (eV/atom)": -7.006602065,
+                "DFT Energy (eV)": -14.01320413,
             },
             {
-                "formula": "Zr",
-                "energy_per_fu": -9.84367624,
-                "energy_per_atom": -9.84367624,
-                "energy": -19.68735248,
+                "Formula": "Zr",
+                "DFT Energy (eV/fu)": -9.84367624,
+                "DFT Energy (eV/atom)": -9.84367624,
+                "DFT Energy (eV)": -19.68735248,
             },
             {
-                "formula": "Zr3O",
-                "energy_per_fu": -42.524204305,
-                "energy_per_atom": -10.63105107625,
-                "energy": -85.04840861,
+                "Formula": "Zr3O",
+                "DFT Energy (eV/fu)": -42.524204305,
+                "DFT Energy (eV/atom)": -10.63105107625,
+                "DFT Energy (eV)": -85.04840861,
             },
             {
-                "formula": "ZrO2",
-                "energy_per_fu": -34.5391058,
-                "energy_per_atom": -11.5130352,
-                "energy": -138.156423,
+                "Formula": "ZrO2",
+                "DFT Energy (eV/fu)": -34.5391058,
+                "DFT Energy (eV/atom)": -11.5130352,
+                "DFT Energy (eV)": -138.156423,
             },
             {
-                "formula": "ZrO2",
-                "energy_per_fu": -34.83230881,
-                "energy_per_atom": -11.610769603333331,
-                "energy": -139.32923524,
+                "Formula": "ZrO2",
+                "DFT Energy (eV/fu)": -34.83230881,
+                "DFT Energy (eV/atom)": -11.610769603333331,
+                "DFT Energy (eV)": -139.32923524,
             },
             {
-                "formula": "Zr2O",
-                "energy_per_fu": -32.42291351666667,
-                "energy_per_atom": -10.807637838888889,
-                "energy": -194.5374811,
+                "Formula": "Zr2O",
+                "DFT Energy (eV/fu)": -32.42291351666667,
+                "DFT Energy (eV/atom)": -10.807637838888889,
+                "DFT Energy (eV)": -194.5374811,
             },
         ]
 
         formation_energy_df = chemical_potentials._calculate_formation_energies(data, elemental)
-        assert formation_energy_df["formula"][0] == "O2"  # definite order
-        assert formation_energy_df["formation_energy"][0] == 0
-        assert formation_energy_df["formula"][1] == "Zr"
-        assert formation_energy_df["formation_energy"][1] == 0
+        assert formation_energy_df["Formula"][0] == "O2"  # definite order
+        assert formation_energy_df["Formation Energy (eV/fu)"][0] == 0
+        assert formation_energy_df["Formula"][1] == "Zr"
+        assert formation_energy_df["Formation Energy (eV/fu)"][1] == 0
         # lowest energy ZrO2:
-        assert np.isclose(formation_energy_df["formation_energy"][4], -10.975428440000002)
+        assert np.isclose(formation_energy_df["Formation Energy (eV/fu)"][4], -10.975428440000002)
 
 
 class CombineExtrinsicTestCase(unittest.TestCase):
     def setUp(self) -> None:
         self.path = Path(__file__).parents[1].joinpath("examples/competing_phases")
         first = self.path / "zro2_la_chempots.json"
         second = self.path / "zro2_y_chempots.json"
```

### Comparing `doped-2.4.0/tests/test_corrections.py` & `doped-2.4.1/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/tests/test_displacements.py` & `doped-2.4.1/tests/test_displacements.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/tests/test_generation.py` & `doped-2.4.1/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/tests/test_plotting.py` & `doped-2.4.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `doped-2.4.0/tests/test_thermodynamics.py` & `doped-2.4.1/tests/test_thermodynamics.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 from monty.serialization import dumpfn, loadfn
 
 from doped.generation import _sort_defect_entries
 from doped.thermodynamics import DefectThermodynamics, scissor_dos
+from doped.utils.parsing import get_vasprun
 from doped.utils.symmetry import _get_sga, point_symmetry
 
 # for pytest-mpl:
 module_path = os.path.dirname(os.path.abspath(__file__))
 data_dir = os.path.join(module_path, "data")
 
 # Define paths for baseline_dir and style as constants
@@ -2074,14 +2075,44 @@
             rasterized=True,
             aspect="auto",
         )
         ax.set_ylim(-0.2, 1.7)
 
         return f
 
+    def test_calculated_fermi_level_k10(self):
+        """
+        Test calculating the Fermi level using a 10x10x10 k-point mesh DOS
+        calculation for primitive CdTe; specifying just the path to the DOS
+        vasprun.xml.
+        """
+        k10_dos_vr_path = os.path.join(self.module_path, "data/CdTe/CdTe_prim_k101010_dos_vr.xml.gz")
+
+        for i, bulk_dos_vr in enumerate([k10_dos_vr_path, get_vasprun(k10_dos_vr_path, parse_dos=True)]):
+            print(f"Testing k10 DOS with thermo for {'str input' if i == 0 else 'DOS object input'}")
+            quenched_fermi_levels = []
+            for anneal_temp in self.anneal_temperatures:
+                gap_shift = belas_linear_fit(anneal_temp) - 1.5
+                (
+                    fermi_level,
+                    e_conc,
+                    h_conc,
+                    conc_df,
+                ) = self.defect_thermo.get_quenched_fermi_level_and_concentrations(
+                    # quenching to 300K (default)
+                    bulk_dos_vr=bulk_dos_vr,
+                    limit="Te-rich",
+                    annealing_temperature=anneal_temp,
+                    delta_gap=gap_shift,
+                )
+                quenched_fermi_levels += [fermi_level]
+
+            # (approx) same result as with k181818 NKRED=2 (0.319104 eV with this dos)
+            assert np.isclose(np.mean(quenched_fermi_levels[12:16]), 0.318674, atol=1e-3)
+
     @custom_mpl_image_compare(filename="CdTe_LZ_Te_rich_concentrations.png")
     def test_calculated_concentrations(self):
         annealing_n = np.array(
             [self.annealing_dict[k]["annealing_e_conc"] for k in self.anneal_temperatures]
         )
         annealing_p = np.array(
             [self.annealing_dict[k]["annealing_h_conc"] for k in self.anneal_temperatures]
```

### Comparing `doped-2.4.0/tests/test_vasp.py` & `doped-2.4.1/tests/test_vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
 
             potcar_settings = default_potcar_dict.copy()
             potcar_settings.update(dds.user_potcar_settings or {})
             assert set(dds.potcar.as_dict()["symbols"]) == {
                 potcar_settings[el_symbol] for el_symbol in dds.structure.symbol_set
             }
         else:
-            assert not dds.potcars
             with pytest.raises(ValueError) as e:
                 _test_pop = dds.potcar
             assert _check_no_potcar_available_warning_error(dds.potcar_symbols[0], e.value)
 
             if dds.charge_state != 0:
                 with pytest.raises(ValueError) as e:
                     _test_pop = dds.incar
@@ -188,14 +187,15 @@
                 "incar",
                 "Available methods",
                 "write_input",
             ]
         )
 
     def _check_potcar_nupdown_dds_warnings(self, w, dds):
+        print("Testing:", [str(warning.message) for warning in w])  # for debugging
         assert any(_check_potcar_dir_not_setup_warning_error(dds, warning.message) for warning in w)
         assert any(_check_nupdown_neutral_cell_warning(warning.message) for warning in w)
         assert any(
             _check_no_potcar_available_warning_error(dds.potcar_symbols[0], warning.message)
             for warning in w
         )
 
@@ -285,28 +285,28 @@
                     )
                 _check_nelect_nupdown_error(e.value)
             self._general_defect_dict_set_check(  # also tests dds.charge_state
                 dds, struct, incar_check=kwargs.pop("incar_check", False), **kwargs
             )
 
     def _generate_and_check_dds(self, struct, incar_check=True, **dds_kwargs):
-        dds = DefectDictSet(struct, **dds_kwargs)  # fine for bulk prim input as well
+        with warnings.catch_warnings(record=True) as w:
+            dds = DefectDictSet(struct, **dds_kwargs)  # fine for bulk prim input as well
+        print([str(warning.message) for warning in w])  # for debugging
         self._check_dds(dds, struct, incar_check=incar_check, **dds_kwargs)
         return dds
 
     def kpts_nelect_nupdown_check(self, dds, kpt, nelect, nupdown):
         if isinstance(kpt, int):
             assert dds.kpoints.kpts == [[kpt, kpt, kpt]]
         else:
             assert dds.kpoints.kpts == kpt
         if _potcars_available():
             assert dds.incar["NELECT"] == nelect
             assert dds.incar["NUPDOWN"] == nupdown
-        else:
-            assert not dds.potcars
 
     def test_neutral_defect_dict_set(self):
         dds = self._generate_and_check_dds(self.prim_cdte.copy())  # fine for bulk prim input as well
         # reciprocal_density = 100/Å⁻³ for prim CdTe:
         self.kpts_nelect_nupdown_check(dds, 7, 18, 0)
         self._write_and_check_dds_files(dds)
         self._write_and_check_dds_files(dds, unperturbed_poscar=False)
@@ -512,15 +512,18 @@
                 "# May want to change NCORE, KPAR, AEXX, ENCUT",
                 "needed if using the kumagai-oba",
                 "symmetry breaking extremely likely",
             ]:
                 assert any(comment_string in line for line in incar_lines)
 
             if dds.incar.get("ALGO", "normal").lower() == "normal":  # ALGO = Normal default, has comment
-                assert any("change to all if zhegv, fexcp/f or zbrent" in line for line in incar_lines)
+                assert any(
+                    "change to all if zhegv, fexcp/f or zbrent, or poor electronic convergence" in line
+                    for line in incar_lines
+                )
 
         else:
             assert not os.path.exists(f"{output_path}/INCAR")
 
         if _potcars_available() and not kwargs.get("potcar_spec", False):
             written_potcar = Potcar.from_file(f"{output_path}/POTCAR")
             # assert dicts equal, as Potcar __eq__ fails due to hashing I believe
@@ -586,15 +589,18 @@
 
     def tearDown(self):
         self.dds_test.tearDown()  # use tearDown from DefectDictSetTest
         if_present_rm("test_dir")
         if_present_rm("CdTe_bulk")
 
         for i in os.listdir():
-            if os.path.isdir(i) and any(j in i for j in ["Mg_", "O_", "v_", "MgO"]):
+            if os.path.isdir(i) and (
+                "MgO" in i
+                or any("vasp_" in j and os.path.isdir(os.path.join(i, j)) for j in os.listdir(i))
+            ):
                 if_present_rm(i)
 
         if_present_rm("MgO_defects_generator.json")
 
     def _general_defect_relax_set_check(self, defect_relax_set, **kwargs):
         dds_test_list = [
             (defect_relax_set.vasp_gam, "vasp_gam"),
@@ -1240,15 +1246,16 @@
         if _potcars_available():
             defects_set.write_files(potcar_spec=True)  # unperturbed_poscar=False by default
 
             # test no (unperturbed) POSCAR files written:
             for folder in os.listdir("."):
                 if os.path.isdir(folder) and "bulk" not in folder:
                     for subfolder in os.listdir(folder):
-                        assert not os.path.exists(f"{folder}/{subfolder}/POSCAR")
+                        if "vasp" in subfolder:
+                            assert not os.path.exists(f"{folder}/{subfolder}/POSCAR")
 
         else:
             with pytest.raises(ValueError):
                 defects_set.write_files(
                     potcar_spec=True
                 )  # INCAR ValueError for charged defects if POTCARs not
                 # available and unperturbed_poscar=False
```

### Comparing `doped-2.4.0/tests/test_wyckoff.py` & `doped-2.4.1/tests/test_wyckoff.py`

 * *Files identical despite different names*

