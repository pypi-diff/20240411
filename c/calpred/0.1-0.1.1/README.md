# Comparing `tmp/calpred-0.1.tar.gz` & `tmp/calpred-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calpred-0.1.tar", last modified: Sat Nov 18 00:06:27 2023, max compression
+gzip compressed data, was "calpred-0.1.1.tar", last modified: Thu Apr 11 18:07:17 2024, max compression
```

## Comparing `calpred-0.1.tar` & `calpred-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2023-11-18 00:06:27.786345 calpred-0.1/
--rw-r--r--   0 kangchenghou (38218510) 855425921     1852 2023-11-18 00:06:27.784018 calpred-0.1/PKG-INFO
--rw-r--r--   0 kangchenghou (38218510) 855425921     1706 2023-11-18 00:06:22.000000 calpred-0.1/README.md
-drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2023-11-18 00:06:27.759186 calpred-0.1/calpred/
--rw-r--r--   0 kangchenghou (38218510) 855425921      138 2023-11-10 23:54:47.000000 calpred-0.1/calpred/__init__.py
--rw-r--r--   0 kangchenghou (38218510) 855425921     6476 2023-11-04 19:38:41.000000 calpred-0.1/calpred/calpred.cli.R
--rw-r--r--   0 kangchenghou (38218510) 855425921     4963 2023-11-09 04:36:07.000000 calpred-0.1/calpred/cli.py
--rw-r--r--   0 kangchenghou (38218510) 855425921     2445 2023-11-17 05:38:38.000000 calpred-0.1/calpred/method.py
--rw-r--r--   0 kangchenghou (38218510) 855425921    10276 2023-11-13 16:46:45.000000 calpred-0.1/calpred/plot.py
--rw-r--r--   0 kangchenghou (38218510) 855425921     4652 2023-11-10 22:01:27.000000 calpred-0.1/calpred/simulate.py
--rw-r--r--   0 kangchenghou (38218510) 855425921     5578 2023-11-04 21:47:19.000000 calpred-0.1/calpred/utils.py
-drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2023-11-18 00:06:27.776747 calpred-0.1/calpred.egg-info/
--rw-r--r--   0 kangchenghou (38218510) 855425921     1852 2023-11-18 00:06:27.000000 calpred-0.1/calpred.egg-info/PKG-INFO
--rw-r--r--   0 kangchenghou (38218510) 855425921      334 2023-11-18 00:06:27.000000 calpred-0.1/calpred.egg-info/SOURCES.txt
--rw-r--r--   0 kangchenghou (38218510) 855425921        1 2023-11-18 00:06:27.000000 calpred-0.1/calpred.egg-info/dependency_links.txt
--rw-r--r--   0 kangchenghou (38218510) 855425921       44 2023-11-18 00:06:27.000000 calpred-0.1/calpred.egg-info/entry_points.txt
--rw-r--r--   0 kangchenghou (38218510) 855425921        1 2023-11-09 04:35:19.000000 calpred-0.1/calpred.egg-info/not-zip-safe
--rw-r--r--   0 kangchenghou (38218510) 855425921        8 2023-11-18 00:06:27.000000 calpred-0.1/calpred.egg-info/top_level.txt
--rw-r--r--   0 kangchenghou (38218510) 855425921       38 2023-11-18 00:06:27.786680 calpred-0.1/setup.cfg
--rw-r--r--   0 kangchenghou (38218510) 855425921      541 2023-11-18 00:05:48.000000 calpred-0.1/setup.py
+drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2024-04-11 18:07:17.688348 calpred-0.1.1/
+-rw-r--r--   0 kangchenghou (38218510) 855425921     2203 2024-04-11 18:07:17.687595 calpred-0.1.1/PKG-INFO
+-rw-r--r--   0 kangchenghou (38218510) 855425921     2056 2024-04-11 18:06:52.000000 calpred-0.1.1/README.md
+drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2024-04-11 18:07:17.675450 calpred-0.1.1/calpred/
+-rw-r--r--   0 kangchenghou (38218510) 855425921      156 2023-11-28 19:35:14.000000 calpred-0.1.1/calpred/__init__.py
+-rw-r--r--   0 kangchenghou (38218510) 855425921     6442 2023-11-28 19:12:11.000000 calpred-0.1.1/calpred/calpred.cli.R
+-rw-r--r--   0 kangchenghou (38218510) 855425921     4963 2023-11-09 04:36:07.000000 calpred-0.1.1/calpred/cli.py
+-rw-r--r--   0 kangchenghou (38218510) 855425921     8944 2023-12-06 20:24:09.000000 calpred-0.1.1/calpred/method.py
+-rw-r--r--   0 kangchenghou (38218510) 855425921    20318 2024-01-14 19:03:53.000000 calpred-0.1.1/calpred/plot.py
+-rw-r--r--   0 kangchenghou (38218510) 855425921     8966 2024-01-14 02:47:58.000000 calpred-0.1.1/calpred/simulate.py
+-rw-r--r--   0 kangchenghou (38218510) 855425921     5578 2023-11-04 21:47:19.000000 calpred-0.1.1/calpred/utils.py
+drwxr-xr-x   0 kangchenghou (38218510) 855425921        0 2024-04-11 18:07:17.685447 calpred-0.1.1/calpred.egg-info/
+-rw-r--r--   0 kangchenghou (38218510) 855425921     2203 2024-04-11 18:07:17.000000 calpred-0.1.1/calpred.egg-info/PKG-INFO
+-rw-r--r--   0 kangchenghou (38218510) 855425921      334 2024-04-11 18:07:17.000000 calpred-0.1.1/calpred.egg-info/SOURCES.txt
+-rw-r--r--   0 kangchenghou (38218510) 855425921        1 2024-04-11 18:07:17.000000 calpred-0.1.1/calpred.egg-info/dependency_links.txt
+-rw-r--r--   0 kangchenghou (38218510) 855425921       44 2024-04-11 18:07:17.000000 calpred-0.1.1/calpred.egg-info/entry_points.txt
+-rw-r--r--   0 kangchenghou (38218510) 855425921        1 2023-11-09 04:35:19.000000 calpred-0.1.1/calpred.egg-info/not-zip-safe
+-rw-r--r--   0 kangchenghou (38218510) 855425921        8 2024-04-11 18:07:17.000000 calpred-0.1.1/calpred.egg-info/top_level.txt
+-rw-r--r--   0 kangchenghou (38218510) 855425921       38 2024-04-11 18:07:17.688524 calpred-0.1.1/setup.cfg
+-rw-r--r--   0 kangchenghou (38218510) 855425921      543 2024-04-11 18:06:16.000000 calpred-0.1.1/setup.py
```

### Comparing `calpred-0.1/calpred/calpred.cli.R` & `calpred-0.1.1/calpred/calpred.cli.R`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 #!/usr/bin/env Rscript
 
 # Load required libraries
-library(optparse)
-library(logger)
 suppressPackageStartupMessages(library(statmod))
 suppressPackageStartupMessages(library(Rchoice))
 
 
 #' @rdname train
 #'
 #' @title Train CalPred model
```

### Comparing `calpred-0.1/calpred/cli.py` & `calpred-0.1.1/calpred/cli.py`

 * *Files identical despite different names*

### Comparing `calpred-0.1/calpred/simulate.py` & `calpred-0.1.1/calpred/simulate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,60 @@
 import numpy as np
+import pandas as pd
 from tqdm import tqdm
 
 
+def simulate_toy_quant_data(
+    n,
+    sd_coef=pd.Series(
+        {"intercept": np.log(7 / 3), "ancestry": 0.2, "age": -0.15, "sex": 0.2}
+    ),
+):
+    # Simulate contexts
+    data = pd.DataFrame(
+        {
+            "yhat": np.random.normal(size=n),
+            "intercept": 1,
+            "ancestry": np.random.uniform(size=n),
+            "age": np.random.normal(loc=40, scale=10, size=n),
+            "sex": np.random.binomial(n=1, p=0.5, size=n),
+        }
+    )
+
+    # Create categorical labels
+    data["ancestry_label"] = pd.cut(data["ancestry"], bins=5, labels=False)
+    data["age_label"] = pd.cut(data["age"], bins=5, labels=False)
+    data["sex_label"] = np.where(data["sex"] > 0, "Female", "Male")
+
+    # Standardize numerical features
+    data[["ancestry", "age", "sex"]] = (
+        data[["ancestry", "age", "sex"]] - data[["ancestry", "age", "sex"]].mean()
+    ) / data[["ancestry", "age", "sex"]].std()
+
+    # Simulate phenotype mean
+    y_mean = data["yhat"]
+
+    # Calculate standard deviation
+    sd_mat = data[["intercept", "ancestry", "age", "sex"]].values
+    y_sd = np.sqrt(np.exp(sd_mat.dot(sd_coef)))
+
+    # Simulate phenotype
+    data["y"] = np.random.normal(loc=y_mean, scale=y_sd)
+
+    # quantile -> real phenotype
+    # pheno = sorted(poisson.rvs(mu=120, size=n, loc=10))
+    # data["pheno"] = pheno[data["y"].rank(method="first")]
+
+    return data
+
+
 def simulate_gxe(
     scenario: int,
     n_rep: int = 100,
-    n_indiv: int = 10000,
+    n_indiv: int = 40000,
     n_gwas: int = 20000,
     n_snp=10000,
     hsq: float = None,
     rg: float = None,
     hsq1: float = None,
     hsq2: float = None,
     prop_amp: float = None,
@@ -76,15 +121,15 @@
     if hsq1 is None:
         hsq1 = hsq
     beta = np.zeros((n_snp, 2, n_rep))
     betaprs = np.zeros((n_snp, n_rep))
     emat = np.zeros([n_indiv, 2, n_rep])
 
     for i in tqdm(range(n_rep)):
-        beta_i = np.random.multivariate_normal(mean=[0, 0], cov=beta_cov, size=n_indiv)
+        beta_i = np.random.multivariate_normal(mean=[0, 0], cov=beta_cov, size=n_snp)
 
         # generate betahat and betaprs using pop1
         betahat_i = beta_i[:, 0] + np.random.normal(
             0, scale=np.sqrt((1 - hsq1 / n_snp) / n_gwas), size=n_snp
         )
         betaprs_i = betahat_i * hsq1 / (hsq1 + n_snp / n_gwas)
         beta[:, :, i] = beta_i
@@ -141,7 +186,102 @@
         e = np.random.normal(scale=np.sqrt(e_var), size=(n_indiv, 2))
         emat[:, :, i] = e
     ymat = gmat + emat
 
     if scenario == 3:
         ymat[:, 1, :] *= prop_amp
     return ymat, gmat, emat
+
+
+def simulate_gxe3(
+    n_rep: int = 100,
+    n_indiv: int = 10000,
+    n_gwas: int = 20000,
+    n_snp: int = 10000,
+    var_g1: float = 0.5,
+    var_g2: float = 0.5,
+    rg: float = 1,
+    var_e1: float = 0.5,
+    var_e2: float = 0.5,
+):
+    """Simulate three modes of GxE as in Durvasula & Price 2023
+
+    Parameters
+    ----------
+    scenario : int
+        which scenario, 1,2,3
+    n_rep : int, optional
+        number of replicates, by default 100
+    n_indiv : int, optional
+        number of individuals, by default 10000
+    n_gwas : int, optional
+        number of GWAS individuals, used to simulate GWAS noise, by default 20000
+    n_snp : int, optional
+        number of SNPs to simulate, by default 10000
+    hsq : float, optional
+        heritability, by default None
+    rg : float, optional
+        genetic correlation, by default None
+    hsq1 : float, optional
+        heritability in pop1, by default None
+    hsq2 : float, optional
+        heritability in pop2, by default None
+    prop_amp : float, optional
+        proportional amplification magnitude, by default None
+
+    Returns
+    -------
+    ymat (n_indiv, 2, n_rep)
+    prsmat (n_indiv, 2, n_rep), using PRS from pop1
+    gmat (n_indiv, 2, n_rep)
+    emat (n_indiv, 2, n_rep)
+    beta (n_snp, 2, n_rep)
+    betaprs (n_snp, n_rep)
+    """
+    beta_cov = (
+        np.array(
+            [
+                [var_g1, rg * np.sqrt(var_g1 * var_g2)],
+                [rg * np.sqrt(var_g1 * var_g2), var_g2],
+            ]
+        )
+        / n_snp
+    )
+
+    e_var = [var_e1, var_e2]
+
+    hsq1 = var_g1 / (var_g1 + var_e1)
+    hsq2 = var_g2 / (var_g2 + var_e2)
+
+    # generate standardized genotypes
+    xmat1 = np.random.binomial(n=2, p=0.5, size=(n_indiv, n_snp))
+    xmat2 = np.random.binomial(n=2, p=0.5, size=(n_indiv, n_snp))
+    xmat1 = (xmat1 - xmat1.mean(axis=0)) / xmat1.std(axis=0)
+    xmat2 = (xmat2 - xmat2.mean(axis=0)) / xmat2.std(axis=0)
+
+    # simulate effect sizes
+    beta = np.zeros((n_snp, 2, n_rep))
+    betaprs = np.zeros((n_snp, n_rep))
+    emat = np.zeros([n_indiv, 2, n_rep])
+
+    for i in tqdm(range(n_rep)):
+        beta_i = np.random.multivariate_normal(mean=[0, 0], cov=beta_cov, size=n_indiv)
+
+        # generate betahat and betaprs using pop1
+        betahat_i = beta_i[:, 0] + np.random.normal(
+            0, scale=np.sqrt((1 - hsq1 / n_snp) / n_gwas), size=n_snp
+        )
+        betaprs_i = betahat_i * hsq1 / (hsq1 + n_snp / n_gwas)
+        beta[:, :, i] = beta_i
+        betaprs[:, i] = betaprs_i
+        emat[:, :, i] = np.random.normal(scale=np.sqrt(e_var), size=(n_indiv, 2))
+
+    gmat = np.zeros([n_indiv, 2, n_rep])
+    prsmat = np.zeros([n_indiv, 2, n_rep])
+
+    gmat[:, 0, :] = xmat1 @ beta[:, 0, :]
+    gmat[:, 1, :] = xmat2 @ beta[:, 1, :]
+    prsmat[:, 0, :] = xmat1 @ betaprs
+    prsmat[:, 1, :] = xmat2 @ betaprs
+    ymat = gmat + emat
+
+    return ymat, prsmat, gmat, emat, beta, betaprs
```

### Comparing `calpred-0.1/calpred/utils.py` & `calpred-0.1.1/calpred/utils.py`

 * *Files identical despite different names*

### Comparing `calpred-0.1/setup.py` & `calpred-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import open
 
 import setuptools
 from setuptools import setup
 
 setup(
     name="calpred",
-    version="0.1",
+    version="0.1.1",
     description="calibrated prediction across diverse contexts",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=["calpred"],
     setup_requires=["numpy>=1.10"],
     entry_points={"console_scripts": ["calpred=calpred.cli:cli"]},
     package_data={
```

