# Comparing `tmp/dflow_galaxy-0.1.5.post5.tar.gz` & `tmp/dflow_galaxy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dflow_galaxy-0.1.5.post5.tar", max compression
+gzip compressed data, was "dflow_galaxy-0.1.6.tar", max compression
```

## Comparing `dflow_galaxy-0.1.5.post5.tar` & `dflow_galaxy-0.1.6.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.5.post5/LICENSE
--rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.5.post5/README.md
--rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.5.post5/dflow_galaxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/__init__.py
--rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/common.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/cp2k_lightning/__init__.py
--rw-r--r--   0        0        0     2086 2024-04-10 06:27:32.443692 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/cp2k_lightning/dflow.py
--rw-r--r--   0        0        0     6456 2024-04-07 14:10:40.795458 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/cp2k_lightning/main.py
--rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_md/__init__.py
--rw-r--r--   0        0        0     1945 2024-04-10 06:27:50.843692 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_md/dflow.py
--rw-r--r--   0        0        0     4338 2024-04-10 01:12:26.524183 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_md/main.py
--rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_tesla/__init__.py
--rw-r--r--   0        0        0    14744 2024-04-10 06:30:21.403689 dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_tesla/main.py
--rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/__init__.py
--rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/dflow.py
--rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/dispatcher.py
--rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/log.py
--rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/pydantic.py
--rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/types.py
--rw-r--r--   0        0        0     5765 2024-04-10 05:28:39.453780 dflow_galaxy-0.1.5.post5/dflow_galaxy/core/util.py
--rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post5/dflow_galaxy/main.py
--rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/__init__.py
--rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
--rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
--rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
--rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM
--rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
--rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
--rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
--rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
--rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
--rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MINIX
--rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
--rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
--rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
--rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
--rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
--rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
--rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
--rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
--rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_SET
--rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
--rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
--rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
--rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_pob
--rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
--rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
--rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
--rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
--rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
--rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
--rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/HFX_BASIS
--rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
--rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
--rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
--rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
--rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
--rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/POTENTIAL
--rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
--rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/README.md
--rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
--rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/xTB_parameters
--rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post5/dflow_galaxy/res/dynacat/tesla_template.yml
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/config.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/abacus.py
--rw-r--r--   0        0        0     6339 2024-04-10 05:02:53.113820 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/cp2k.py
--rw-r--r--   0        0        0     9775 2024-04-09 14:05:23.796450 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/deepmd.py
--rw-r--r--   0        0        0     8057 2024-04-10 05:03:29.533819 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/lammps.py
--rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/lib.py
--rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/model_devi.py
--rw-r--r--   0        0        0     8185 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/main.py
--rw-r--r--   0        0        0      547 2024-04-10 06:37:19.483673 dflow_galaxy-0.1.5.post5/pyproject.toml
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.5.post5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-02-19 03:12:58.574253 dflow_galaxy-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1834 2024-04-09 15:45:18.275720 dflow_galaxy-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-01-30 01:22:58.649023 dflow_galaxy-0.1.6/dflow_galaxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/__init__.py
+-rw-r--r--   0        0        0     2499 2024-04-09 15:45:01.375722 dflow_galaxy-0.1.6/dflow_galaxy/app/common.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/__init__.py
+-rw-r--r--   0        0        0     2167 2024-04-10 12:51:32.469597 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/dflow.py
+-rw-r--r--   0        0        0     7015 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/main.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:32:16.436174 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/__init__.py
+-rw-r--r--   0        0        0     2006 2024-04-10 13:00:43.009583 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/dflow.py
+-rw-r--r--   0        0        0     4853 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/main.py
+-rw-r--r--   0        0        0     2493 2024-04-11 08:26:42.339456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/report.py
+-rw-r--r--   0        0        0        0 2024-04-02 03:42:50.450085 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/__init__.py
+-rw-r--r--   0        0        0    15556 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/main.py
+-rw-r--r--   0        0        0     5892 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/report.py
+-rw-r--r--   0        0        0        0 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.6/dflow_galaxy/core/__init__.py
+-rw-r--r--   0        0        0    28431 2024-04-09 03:02:40.485846 dflow_galaxy-0.1.6/dflow_galaxy/core/dflow.py
+-rw-r--r--   0        0        0     4687 2024-04-10 06:26:03.273692 dflow_galaxy-0.1.6/dflow_galaxy/core/dispatcher.py
+-rw-r--r--   0        0        0      163 2024-02-06 03:07:45.063120 dflow_galaxy-0.1.6/dflow_galaxy/core/log.py
+-rw-r--r--   0        0        0       97 2024-04-01 07:14:05.895738 dflow_galaxy-0.1.6/dflow_galaxy/core/pydantic.py
+-rw-r--r--   0        0        0      541 2024-04-03 16:22:36.889294 dflow_galaxy-0.1.6/dflow_galaxy/core/types.py
+-rw-r--r--   0        0        0     6065 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/core/util.py
+-rw-r--r--   0        0        0      335 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/main.py
+-rw-r--r--   0        0        0      146 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/res/__init__.py
+-rw-r--r--   0        0        0   189331 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS
+-rw-r--r--   0        0        0     2717 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS
+-rw-r--r--   0        0        0    15836 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS
+-rw-r--r--   0        0        0    57524 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM
+-rw-r--r--   0        0        0   189911 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT
+-rw-r--r--   0        0        0   133011 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH
+-rw-r--r--   0        0        0    66934 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae
+-rw-r--r--   0        0        0    17509 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT
+-rw-r--r--   0        0        0   244853 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINBAS
+-rw-r--r--   0        0        0    49588 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINIX
+-rw-r--r--   0        0        0   127679 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT
+-rw-r--r--   0        0        0    55644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1
+-rw-r--r--   0        0        0    23527 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1
+-rw-r--r--   0        0        0    65485 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2
+-rw-r--r--   0        0        0   179850 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL
+-rw-r--r--   0        0        0  1574370 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH
+-rw-r--r--   0        0        0     6644 2024-04-02 03:42:50.460085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW
+-rw-r--r--   0        0        0    37261 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ
+-rw-r--r--   0        0        0   195109 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_SET
+-rw-r--r--   0        0        0     5526 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA
+-rw-r--r--   0        0        0   324291 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH
+-rw-r--r--   0        0        0   258169 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL
+-rw-r--r--   0        0        0   191314 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_pob
+-rw-r--r--   0        0        0   223481 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS
+-rw-r--r--   0        0        0    23668 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2
+-rw-r--r--   0        0        0  1713484 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS
+-rw-r--r--   0        0        0   119403 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS
+-rw-r--r--   0        0        0   167483 2024-04-02 03:42:50.470085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS
+-rw-r--r--   0        0        0   253677 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS
+-rw-r--r--   0        0        0    17275 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HFX_BASIS
+-rw-r--r--   0        0        0     2106 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HF_POTENTIALS
+-rw-r--r--   0        0        0     5486 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS
+-rw-r--r--   0        0        0     7829 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS
+-rw-r--r--   0        0        0      447 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/MM_POTENTIAL
+-rw-r--r--   0        0        0     5498 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS
+-rw-r--r--   0        0        0   177804 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL
+-rw-r--r--   0        0        0   385325 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH
+-rw-r--r--   0        0        0      125 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/README.md
+-rw-r--r--   0        0        0    91811 2024-04-02 03:42:50.480085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/nm12_parameters.xml
+-rw-r--r--   0        0        0    32194 2024-04-02 03:42:50.640085 dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/xTB_parameters
+-rw-r--r--   0        0        0     1171 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/res/dynacat/tesla_template.yml
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.6/dflow_galaxy/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 08:30:41.445577 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/__init__.py
+-rw-r--r--   0        0        0     1702 2024-04-09 15:45:01.385722 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/config.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/abacus.py
+-rw-r--r--   0        0        0     6339 2024-04-10 05:02:53.113820 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/cp2k.py
+-rw-r--r--   0        0        0     9692 2024-04-11 08:26:42.349456 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/deepmd.py
+-rw-r--r--   0        0        0     8057 2024-04-11 02:42:29.459986 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lammps.py
+-rw-r--r--   0        0        0     1261 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lib.py
+-rw-r--r--   0        0        0     6334 2024-02-25 16:19:13.409582 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/model_devi.py
+-rw-r--r--   0        0        0     8185 2024-04-11 01:41:14.700081 dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/main.py
+-rw-r--r--   0        0        0      561 2024-04-11 08:27:34.919457 dflow_galaxy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 dflow_galaxy-0.1.6/PKG-INFO
```

### Comparing `dflow_galaxy-0.1.5.post5/LICENSE` & `dflow_galaxy-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/README.md` & `dflow_galaxy-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/common.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/common.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/cp2k_lightning/dflow.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/dflow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from dflow_galaxy.core import dflow, types, dispatcher
 import shutil
+import os
 
 
 @dataclass(frozen=True)
 class RunCp2kArgs:
     input_dir : types.InputArtifact
     output_dir: types.OutputArtifact
 
@@ -15,15 +16,15 @@
 
     def __call__(self, args: RunCp2kArgs):
         """
         bash step to run cp2k aimd task
         """
         script = [
             # guess cp2k data dir
-            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k)")/../../data" || true',
+            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k || which cp2k.psmp)")/../../data" || true',
             f'cd {args.input_dir}',
             self.cp2k_script,
             f'mkdir -p {args.output_dir}',
             f'mv * {args.output_dir}',
         ]
         return script
 
@@ -60,8 +61,9 @@
     dflow_builder.add_step(cp2k_step)
 
     # run workflow
     dflow_builder.run()
 
     # download artifacts to out_dir
     dflow_builder.s3_download('cp2k_output')
-    shutil.move('cp2k_output', f'{out_dir}/cp2k_output.tgz')
+    shutil.unpack_archive('cp2k_output', out_dir, format='gztar')
+    return os.path.join(out_dir, 'output_dir')
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/cp2k_lightning/main.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/cp2k_lightning/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 from dp.launching.typing import Int, String, Enum, Float, Boolean
 from dp.launching.cli import to_runner, default_minimal_exception_handler
 
 from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context
 from dflow_galaxy.res import get_cp2k_data_dir
 from dflow_galaxy.core.log import get_logger
 from ai2_kit.feat import catalysis as ai2cat
+from ai2_kit.tool.ase import AseHelper
+from ai2_kit.tool.dpdata import DpdataHelper
 
 from pathlib import Path
 import shutil
 import sys
+import os
 
 from .dflow import run_cp2k_workflow
 
 logger = get_logger(__name__)
 
 
 def get_cp2k_data_file(name: str):
@@ -75,15 +78,15 @@
 class Cp2kLightningArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
-        description="A system file as the initial structure of AIMD simulation")
+        description="A system file as the initial structure of AIMD simulation, can be xyz, cif, POSCAR format")
 
     system_type: SystemTypeOptions = Field(
         default=SystemTypeOptions.metal,
         description="Type of the system, semi for semi-conductor, metal for metal")
 
     accuracy: AccuracyOptions = Field(
         default=AccuracyOptions.medium,
@@ -138,19 +141,20 @@
     # stage 1: generate cp2k input file
     basis_set_file = get_cp2k_data_file(args.basis_set.value)
     potential_file = get_cp2k_data_file(args.potential.value)
     # copy data file to cwd
     # don't use absolute path as the config file will be use in docker
     shutil.copy(basis_set_file, '.')
     shutil.copy(potential_file, '.')
+    system_file = args.system_file.get_full_path()
 
     # create a closure to generate cp2k input file
     def _gen_cp2k_input(out_dir: str, aimd: bool):
         config_builder = ai2cat.ConfigBuilder()
-        config_builder.load_system(args.system_file.get_full_path()).gen_cp2k_input(
+        config_builder.load_system(system_file).gen_cp2k_input(
             out_dir=out_dir,
             aimd=aimd,
             # common options
             style=args.system_type.value,
             temp=args.temperature,
             steps=args.steps,
             timestep=args.timestep,
@@ -169,21 +173,34 @@
 
     if args.dry_run:
         logger.info('skip dflow run due to dry_run is set to True')
         return 0
 
     # stage 2: run cp2k with dflow
     setup_dflow_context(args)
-    run_cp2k_workflow(
+    cp2k_output_dir = run_cp2k_workflow(
         input_dir=str(args.output_dir),
         out_dir=str(args.output_dir),
         cp2k_device_model=str(args.cp2k_device_model),
         cp2k_image=str(args.cp2k_image),
         cp2k_script=str(args.cp2k_script),
     )
+
+    # stage 3: post-process cp2k output
+    # convert cp2k output to xyz file and dpdata set
+    AseHelper().read(
+        os.path.join(cp2k_output_dir, '*-pos-1.xyz')
+    ).set_by_ref(
+        system_file
+    ).write(str(out_dir / 'aimd.xyz' ))
+
+    DpdataHelper().read(
+        cp2k_output_dir, fmt='cp2kdata/md', cp2k_output_name='output'
+    ).write(str(out_dir / 'dp-dataset'))
+
     return 0
 
 def main():
     to_runner(
         Cp2kLightningArgs,
         launch_app,
         version="0.1.0",
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_md/dflow.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/dflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from dflow_galaxy.core import dflow, types, dispatcher
 import shutil
+import os
 
 
 @dataclass(frozen=True)
 class RunLammpsArgs:
     input_dir : types.InputArtifact
     output_dir: types.OutputArtifact
 
@@ -55,8 +56,10 @@
     dflow_builder.add_step(lammps_step)
 
     # run workflow
     dflow_builder.run()
 
     # download artifacts to out_dir
     dflow_builder.s3_download('lammps_output')
-    shutil.move('lammps_output', f'{out_dir}/lammps_output.tgz')
+    shutil.unpack_archive('lammps_output', out_dir, format='gztar')
+    return os.path.join(out_dir, 'output_dir')
+
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_md/main.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_md/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,27 @@
 
 from pathlib import Path
 import shutil
 import sys
 import os
 
 from .dflow import run_lammps_workflow
+from .report import gen_report
 
 logger = get_logger(__name__)
 
 
 class DynaCatMdArgs(DFlowOptions):
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     system_file: InputFilePath = Field(
-        description="A system file as the initial structure of LAMMPS simulation")
+        description="A system file as the initial structure of LAMMPS simulation, can be xyz, cif, POSCAR, etc.")
 
     # TODO: support multiple deepmd models
     deepmd_model: InputFilePath = Field(
         description="Deepmd model file for LAMMPS simulation")
 
     ensemble: EnsembleOptions = Field(
         default=EnsembleOptions.csvr,
@@ -83,23 +84,28 @@
         description="Device model for LAMMPS simulation")
 
     lammps_script: String = Field(
         default= '\n'.join([
             '# LAMMPS input can be referenced as lammps.inp',
             '# Note that different container may have different setup',
             'lmp -in lammps.inp &> lammps.out',
+            '# Run plumed to calculate free energy surface',
+            'plumed sum_hills --hills HILLS --mintozero --outfile fes.dat'
         ]),
         format='multi-line',
         description="Script to run LAMMPS simulation, note that it depends on the docker image")
 
 
 def launch_app(args: DynaCatMdArgs) -> int:
     config_builder = ai2cat.ConfigBuilder()
 
     shutil.copy(args.deepmd_model, 'dp-model.pb')
+    if not args.plumed_config:
+        raise ValueError('plumed_config is required for metadynamics simulation')
+
     dump_text(args.plumed_config, 'plumed.inp')
 
     logger.info(f'type of system_file: {type(args.system_file)}')
     config_builder.load_system(args.system_file.get_full_path()).gen_lammps_input(
         out_dir=args.output_dir,
         nsteps=args.steps,
         temp=args.temperature,
@@ -113,22 +119,27 @@
     shutil.move('plumed.inp', args.output_dir)
     shutil.move('dp-model.pb', args.output_dir)
 
     if args.dry_run:
         return 0
 
     setup_dflow_context(args)
-    run_lammps_workflow(
+    lammps_output_dir = run_lammps_workflow(
         input_dir=str(args.output_dir),
         out_dir=str(args.output_dir),
         lammps_image=str(args.lammps_image),
         lammps_device_model=str(args.lammps_device_model),
         lammps_script=str(args.lammps_script),
     )
 
+    try:
+        gen_report(lammps_output_dir=lammps_output_dir,
+                   output_dir=str(args.output_dir))
+    except:
+        logger.exception('Failed to generate report')
     return 0
 
 
 def main():
     to_runner(
         DynaCatMdArgs,
         launch_app,
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/app/dynacat_tesla/main.py` & `dflow_galaxy-0.1.6/dflow_galaxy/app/dynacat_tesla/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from dp.launching.typing import BaseModel, Field, OutputDirectory, InputFilePath
 from dp.launching.typing import Int, String, Enum, Float, Boolean, List, Optional, Dict
 from dp.launching.cli import to_runner, default_minimal_exception_handler
+from dp.launching.report import Report, ReportSection, ChartReportElement
 
 from dflow_galaxy.app.common import DFlowOptions, setup_dflow_context, EnsembleOptions
 from dflow_galaxy.res import get_res_path
 from dflow_galaxy.core.log import get_logger
+from dflow_galaxy.core.util import parse_string_array, str_or_none
 
 from dflow_galaxy.workflow.tesla.main import build_tesla_workflow
 
 from ai2_kit.core.util import dump_json, load_text, load_json
 from ai2_kit.feat import catalysis as ai2cat
 
 import ase.io
+import fire
 
 from pathlib import Path
 from uuid import uuid4
 import shutil
 import glob
 import sys
 import os
 
+from .report import gen_report
 
 logger = get_logger(__name__)
 
 
 BH_DEEPMD_DEFAULT = {
     'image_name': 'registry.dp.tech/dptech/dpmd:2.2.8-cuda12.0',
     'scass_type': 'c8_m32_1 * NVIDIA V100',
@@ -56,21 +60,14 @@
         description="Value of the item, multiple value should be separated by comma")
     broadcast: Boolean = Field(
         default=False,
         description="Use broadcast instead of full combination")
 
 
 class DeepmdSettings(BaseModel):
-    dataset : InputFilePath = Field(
-        title='DeepMD Dataset',
-        description="DeepMD in zip or tgz format")
-
-    input_template: InputFilePath = Field(
-        title='DeepMD Input Template',
-        description="Input template file for DeepMD training")
 
     compress_model: Boolean = Field(
         default=True,
         description="Compress the model after training")
 
     concurrency: Int = Field(
         default=4,
@@ -83,17 +80,14 @@
     setup_script: String = Field(
         default='',
         format='multi-line',
         description="Setup script for DeepMD simulation, note that it depends on the docker image you used")
 
 
 class LammpsSetting(BaseModel):
-    system_file: InputFilePath = Field(
-        description="Structure file in xyz format use for LAMMPS simulation")
-
     ensemble: EnsembleOptions = Field(
         default=EnsembleOptions.csvr,
         description='Ensemble of LAMMPS simulation')
 
     plumed_config: Optional[String] = Field(
         format='multi-line',
         description='Plumed configuration file for metadynamics simulation')
@@ -158,16 +152,14 @@
 
     metric: String = Field(
         default='max_devi_f',
         description="Metric to measure the deviation")
 
 
 class Cp2kSettings(BaseModel):
-    input_template: InputFilePath = Field(
-        description="Input template file for CP2K simulation")
 
     limit: Int = Field(
         default=50,
         description="Limit of the number of structures to be labeled for each iteration")
 
     concurrency: Int = Field(
         default=5,
@@ -176,22 +168,35 @@
     cmd: String = Field(
         default='mpirun -np 32 cp2k.popt',
         description="Script to run CP2K simulation, note that it depends on the docker image")
 
     setup_script: String = Field(
         default = '\n'.join([
             '# guess cp2k data dir',
-            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k)")/../../data" || true',
+            '[[ -z "${CP2K_DATA_DIR}" ]] && export CP2K_DATA_DIR="$(dirname "$(which cp2k || which cp2k.psmp)")/../../data" || true',
             'source /opt/cp2k-toolchain/install/setup',
         ]),
         format='multi-line',
         description="Setup script for CP2K simulation, note that it depends on the docker image you used")
 
 
 class DynacatTeslaArgs(DFlowOptions):
+    deepmd_dataset : InputFilePath = Field(
+        title='DeepMD Dataset',
+        description="DeepMD in zip or tgz format, for example: deepmd-dataset.tgz")
+
+    deepmd_input_template: InputFilePath = Field(
+        title='DeepMD Input Template',
+        description="Input template file for DeepMD training, in json format, for example: deepmd.json")
+
+    lammps_system_file: InputFilePath = Field(
+        description="Structure file in xyz format use for LAMMPS simulation, for example h2o.xyz")
+
+    cp2k_input_template: InputFilePath = Field(
+        description="Input template file for CP2K simulation, for example: cp2k.inp")
 
     dry_run: Boolean = Field(
         default = True,
         description="Generate configuration file without running the simulation")
 
     max_iters: Int = Field(
         default = 7,
@@ -234,15 +239,15 @@
 
 
 def launch_app(args: DynacatTeslaArgs) -> int:
     s3_prefix = args.s3_prefix or f'dynacat-{uuid4()}'
     logger.info(f'using s3 prefix: {s3_prefix}')
     tesla_template = get_res_path() / 'dynacat' / 'tesla_template.yml'
     # handle deepmd dataset
-    dp_dataset_file = args.deepmd.dataset.get_full_path()
+    dp_dataset_file = args.deepmd_dataset.get_full_path()
     dp_dataset = _unpack_dpdata(dp_dataset_file, 'init-dataset')
     dp_dataset_config = {}
     for i, d in enumerate(dp_dataset):
         dp_dataset_config[f'dpdata-{i}'] = {
             'url': d,
         }
     logger.info(f'Unpacked dpdata to {dp_dataset}')
@@ -272,18 +277,28 @@
     except:
         logger.exception('Failed to run workflow')
         return 1
     finally:
         # reclaim useful data
         dp_dataset_dir = os.path.join(args.output_dir, 'dp-dataset')
         dp_models_dir = os.path.join(args.output_dir, 'dp-models')
+        model_devi_dir = os.path.join(args.output_dir, 'model-devi')
         os.makedirs(dp_dataset_dir, exist_ok=True)
         os.makedirs(dp_models_dir, exist_ok=True)
+        os.makedirs(model_devi_dir, exist_ok=True)
         workflow.s3_download('iter-dataset', dp_dataset_dir)
         workflow.s3_download('train-deepmd', dp_models_dir)
+        workflow.s3_download('screen-model-devi', model_devi_dir)
+        try:
+            gen_report(dp_models_dir=dp_models_dir,
+                    model_devi_dir=model_devi_dir,
+                    max_iters=args.max_iters,
+                    output_dir=str(args.output_dir))
+        except:
+            logger.exception('Failed to generate report')
     return 0
 
 
 def _get_executor_config(args: DynacatTeslaArgs):
     return {
         'executors': {
             'bohrium': {
@@ -328,21 +343,21 @@
             'cp2k': 'bohrium'
         },
     }
 
 
 def _get_workflow_config(args: DynacatTeslaArgs, dp_dataset_config: dict):
     # process system file
-    explore_data_file = args.lammps.system_file.get_full_path()
+    explore_data_file = args.lammps_system_file.get_full_path()
     explore_data_key = os.path.basename(explore_data_file)
     atoms = ase.io.read(explore_data_file, index=0)
     type_map, mass_map = ai2cat.get_type_map(atoms)  # type: ignore
 
-    cp2k_input_template = load_text(args.cp2k.input_template.get_full_path())
-    deepmd_template = load_json(args.deepmd.input_template.get_full_path())
+    cp2k_input_template = load_text(args.cp2k_input_template.get_full_path())
+    deepmd_template = load_json(args.deepmd_input_template.get_full_path())
     product_vars, broadcast_vars = _get_lammps_vars(args.lammps.explore_vars)
 
     return {
         'datasets': {
             **dp_dataset_config,
             explore_data_key: {  # data key must be a normal file name or else ase cannot detect the format
                 'url': explore_data_file,
@@ -364,15 +379,15 @@
                 'lammps': {
                     'systems': [explore_data_key],
                     'nsteps': args.lammps.nsteps,
                     'ensemble': args.lammps.ensemble.value,
                     'timestep': args.lammps.timestep,
                     'sample_freq': args.lammps.sample_freq,
                     'no_pbc': args.lammps.no_pbc,
-                    'plumed_config': args.lammps.plumed_config or None,
+                    'plumed_config': str_or_none(args.lammps.plumed_config),
                     'product_vars': product_vars,
                     'broadcast_vars': broadcast_vars,
                     'template_vars': dict((item.key, item.value) for item in args.lammps.template_vars),
                 }
             },
             'screen':{
                 'model_devi': {
@@ -391,24 +406,20 @@
 
 
 def _get_lammps_vars(explore_vars: List[ExploreItem]):
     broadcast_vars = {}
     product_vars = {}
     for item in explore_vars:
         if item.broadcast:
-            broadcast_vars[item.key] = _parse_string_array(item.value, dtype=float)
+            broadcast_vars[item.key] = parse_string_array(item.value, dtype=float, delimiter=',')
         else:
-            product_vars[item.key] = _parse_string_array(item.value, dtype=float)
+            product_vars[item.key] = parse_string_array(item.value, dtype=float, delimiter=',')
     return product_vars, broadcast_vars
 
 
-def _parse_string_array(s: str, dtype=float, delimiter=','):
-    return [dtype(x) for x in s.split(delimiter)]
-
-
 def _unpack_dpdata(file: str, extract_dir: str):
     extract_dir = os.path.normpath(extract_dir)
     os.makedirs(extract_dir, exist_ok=True)
     shutil.unpack_archive(file, extract_dir=extract_dir)
     # use type.raw to locate the dpdata folder
     paths = glob.glob(f'{extract_dir}/**/type.raw', recursive=True)
     return [ os.path.dirname(p) for p in paths]
@@ -419,8 +430,11 @@
         DynacatTeslaArgs,
         launch_app,
         version="0.1.0",
     )(sys.argv[1:])
 
 
 if __name__ == "__main__":
-    main()
+    fire.Fire({
+        'main': main,
+        'gen_report': gen_report,
+    })
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/core/dflow.py` & `dflow_galaxy-0.1.6/dflow_galaxy/core/dflow.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/core/dispatcher.py` & `dflow_galaxy-0.1.6/dflow_galaxy/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/core/types.py` & `dflow_galaxy-0.1.6/dflow_galaxy/core/types.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/core/util.py` & `dflow_galaxy-0.1.6/dflow_galaxy/core/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,7 +173,22 @@
         for root, dirs, files in os.walk(path):
             for file in files:
                 file_path = os.path.join(root, file)
                 resolve_ln(file_path, mv=mv)
             for dir in dirs:
                 dir_path = os.path.join(root, dir)
                 resolve_ln(dir_path, mv=mv)
+
+
+def parse_string_array(s: str, dtype=None, delimiter=None):
+    arr = [x.strip() for x in s.split(delimiter)]
+    if dtype:
+        arr = [dtype(x) for x in arr]
+    return arr
+
+def str_or_none(s):
+    """
+    return None if s is empty string
+    """
+    if not s:
+        return None
+    return s
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/AcPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ADMM_ae`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_LRIGPW_AUXMOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MINBAS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINBAS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MINIX` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MINIX`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_AcPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP1`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_LnPP2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UCL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_MOLOPT_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_PERIODIC_GW`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_RI_cc-TZ`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_SET` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_SET`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ZIJLSTRA`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_ccGRB_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_def2_QZVP_RI_ALL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/BASIS_pob` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/BASIS_pob`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/ECP_POTENTIALS_pob-TZVP-rev2`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/EMSL_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_BASIS_SETS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/GTH_SOC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/HFX_BASIS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HFX_BASIS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/HF_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/HF_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP1_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/LnPP2_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/NLCC_POTENTIALS`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/POTENTIAL` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/POTENTIAL_UZH`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/nm12_parameters.xml` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/nm12_parameters.xml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/cp2k_data/xTB_parameters` & `dflow_galaxy-0.1.6/dflow_galaxy/res/cp2k_data/xTB_parameters`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/res/dynacat/tesla_template.yml` & `dflow_galaxy-0.1.6/dflow_galaxy/res/dynacat/tesla_template.yml`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/config.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/config.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/cp2k.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/cp2k.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/deepmd.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/deepmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,17 +159,16 @@
                     bash_ln_cmd(args.iter_dataset_dir, ITER_DATASET_DIR),
                     '',
                     self._build_dp_train_script(),
                     '',
                     '# persist result',
                     f'PERSIST_DIR={args.persist_dir}/$ITEM/persist/',
                     'mkdir -p $PERSIST_DIR',
-                    'mv *.done $PERSIST_DIR',
-                    f'mv {DP_FROZEN_MODEL} $PERSIST_DIR',
-                    f'mv {DP_ORIGINAL_MODEL} $PERSIST_DIR || true',
+                    'rm model.ckpt* || true',
+                    'mv *.* $PERSIST_DIR',
                     'popd',
                 ]
             ),
             'popd',
         ]
         return script
```

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/lammps.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lammps.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/lib.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/lib.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/domain/model_devi.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/domain/model_devi.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/dflow_galaxy/workflow/tesla/main.py` & `dflow_galaxy-0.1.6/dflow_galaxy/workflow/tesla/main.py`

 * *Files identical despite different names*

### Comparing `dflow_galaxy-0.1.5.post5/pyproject.toml` & `dflow_galaxy-0.1.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "dflow-galaxy"
-version = "0.1.5.post5"
+version = "0.1.6"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 include = ["dflow_galaxy/res/*"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydflow = "1.8.60"
 dpdispatcher = "^0.6.4"
 ai2-kit= "0.15.10"
 dp-launching-sdk = "^0.12.0"
 lbg = "^1.2.24"
+cp2kdata = "^0.6.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.0"
 sphinx = "^7.2.6"
 
 [build-system]
```

### Comparing `dflow_galaxy-0.1.5.post5/PKG-INFO` & `dflow_galaxy-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dflow-galaxy
-Version: 0.1.5.post5
+Version: 0.1.6
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ai2-kit (==0.15.10)
+Requires-Dist: cp2kdata (>=0.6.6,<0.7.0)
 Requires-Dist: dp-launching-sdk (>=0.12.0,<0.13.0)
 Requires-Dist: dpdispatcher (>=0.6.4,<0.7.0)
 Requires-Dist: lbg (>=1.2.24,<2.0.0)
 Requires-Dist: pydflow (==1.8.60)
 Description-Content-Type: text/markdown
 
 # DFlow Galaxy
```

