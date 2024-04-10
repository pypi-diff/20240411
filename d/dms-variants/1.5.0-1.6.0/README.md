# Comparing `tmp/dms_variants-1.5.0.tar.gz` & `tmp/dms_variants-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dms_variants-1.5.0.tar", last modified: Tue Feb  6 23:53:04 2024, max compression
+gzip compressed data, was "dms_variants-1.6.0.tar", last modified: Wed Apr 10 22:59:33 2024, max compression
```

## Comparing `dms_variants-1.5.0.tar` & `dms_variants-1.6.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:04.185556 dms_variants-1.5.0/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      259 2022-08-04 00:15:21.000000 dms_variants-1.5.0/.flake8
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      148 2024-02-06 23:52:29.000000 dms_variants-1.5.0/.gitignore
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    10805 2024-02-06 23:52:29.000000 dms_variants-1.5.0/CHANGELOG.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7343 2021-12-29 17:41:37.000000 dms_variants-1.5.0/CONTRIBUTING.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1615 2019-06-21 15:41:54.000000 dms_variants-1.5.0/LICENSE.txt
--rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     1993 2024-02-06 23:53:04.181618 dms_variants-1.5.0/PKG-INFO
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1321 2024-02-06 23:52:29.000000 dms_variants-1.5.0/README.rst
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.150331 dms_variants-1.5.0/dms_variants/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      361 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/__init__.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1724 2019-08-08 13:40:53.000000 dms_variants-1.5.0/dms_variants/_cutils.c
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6515 2021-12-29 17:41:37.000000 dms_variants-1.5.0/dms_variants/barcodes.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     8054 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/bottlenecks.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   142384 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/codonvarianttable.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3019 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/constants.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    10612 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/fastq.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   121007 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/globalepistasis.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    13649 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/illuminabarcodeparser.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    39927 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/ispline.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7282 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/pdb_utils.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1978 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/plotnine_themes.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    35620 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/simulate.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    24968 2024-02-06 23:52:29.000000 dms_variants-1.5.0/dms_variants/utils.py
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.173821 dms_variants-1.5.0/dms_variants.egg-info/
--rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     1993 2024-02-06 23:53:02.000000 dms_variants-1.5.0/dms_variants.egg-info/PKG-INFO
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2840 2024-02-06 23:53:02.000000 dms_variants-1.5.0/dms_variants.egg-info/SOURCES.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)        1 2024-02-06 23:53:02.000000 dms_variants-1.5.0/dms_variants.egg-info/dependency_links.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      119 2024-02-06 23:53:02.000000 dms_variants-1.5.0/dms_variants.egg-info/requires.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       13 2024-02-06 23:53:02.000000 dms_variants-1.5.0/dms_variants.egg-info/top_level.txt
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.476263 dms_variants-1.5.0/docs/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)        0 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/.nojekyll
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      729 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/Makefile
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3613 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/README.rst
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.497873 dms_variants-1.5.0/docs/_static/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   172664 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/_static/BloomLogo.jpg
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      229 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/acknowledgments.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2020-01-20 16:49:17.000000 dms_variants-1.5.0/docs/bottleneck_likelihood.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       66 2019-11-01 04:46:22.000000 dms_variants-1.5.0/docs/codonvariant_plot_formatting.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2019-06-25 13:56:05.000000 dms_variants-1.5.0/docs/codonvariant_sim_data.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       73 2020-04-30 13:10:13.000000 dms_variants-1.5.0/docs/codonvariant_sim_data_multi_targets.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       66 2021-12-28 21:22:43.000000 dms_variants-1.5.0/docs/codonvariant_sim_data_w_gaps.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6827 2024-02-06 23:52:29.000000 dms_variants-1.5.0/docs/conf.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      129 2019-06-25 13:56:05.000000 dms_variants-1.5.0/docs/doc_requirements.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1356 2022-03-04 02:18:14.000000 dms_variants-1.5.0/docs/examples.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      546 2019-11-01 04:46:22.000000 dms_variants-1.5.0/docs/index.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      337 2024-02-06 19:24:37.000000 dms_variants-1.5.0/docs/installation.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       55 2019-11-10 02:51:54.000000 dms_variants-1.5.0/docs/narrow_bottleneck.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       65 2019-06-21 15:41:54.000000 dms_variants-1.5.0/docs/package_index.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       60 2019-08-16 16:47:32.000000 dms_variants-1.5.0/docs/parsebarcodes_sim_data.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       49 2022-03-04 02:18:14.000000 dms_variants-1.5.0/docs/prob_escape.nblink
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      282 2021-03-11 17:23:36.000000 dms_variants-1.5.0/environment.yml
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      332 2020-01-29 04:00:43.000000 dms_variants-1.5.0/nbval_sanitize.cfg
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.725927 dms_variants-1.5.0/notebooks/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      274 2019-11-01 04:46:22.000000 dms_variants-1.5.0/notebooks/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   323628 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/bottleneck_likelihood.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   359368 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/codonvariant_plot_formatting.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)  1972288 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/codonvariant_sim_data.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)  2502119 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/codonvariant_sim_data_multi_targets.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   709442 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/codonvariant_sim_data_w_gaps.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   397577 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/multi_latent_phenos.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   652450 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/narrow_bottleneck.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    51628 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/parsebarcodes_sim_data.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   924393 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/predict_variants.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   264475 2024-02-06 23:52:29.000000 dms_variants-1.5.0/notebooks/prob_escape.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188) 10191948 2022-03-04 02:18:14.000000 dms_variants-1.5.0/notebooks/prob_escape_codon_variant_table.csv
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3754 2022-03-04 02:18:14.000000 dms_variants-1.5.0/notebooks/spike.txt
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      523 2021-12-29 17:41:37.000000 dms_variants-1.5.0/pytest.ini
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       38 2024-02-06 23:53:04.186825 dms_variants-1.5.0/setup.cfg
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2062 2024-02-06 23:52:29.000000 dms_variants-1.5.0/setup.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       68 2024-02-06 23:52:29.000000 dms_variants-1.5.0/test_requirements.txt
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:03.795110 dms_variants-1.5.0/tests/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)       13 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/.gitignore
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      122 2019-06-21 15:41:54.000000 dms_variants-1.5.0/tests/README.rst
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    11930 2023-03-19 20:30:35.000000 dms_variants-1.5.0/tests/bottleneck_likelihood_deriv_equations.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    82507 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/codonvarianttable_toy_example.ipynb
-drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-02-06 23:53:04.173394 dms_variants-1.5.0/tests/count_codonvariant_files/
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2762 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/PacBio_amplicon.gb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    57804 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/barcode_variant_table.csv
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      730 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/fates.csv
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394529 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-1_plasmid_R1.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394529 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-1_plasmid_R2.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394540 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-1_uninduced_R1.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394540 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-1_uninduced_R2.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394542 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-2_plasmid_R1.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394542 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/library-2_plasmid_R2.fastq
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)      121 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/n_variants.csv
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   108174 2019-08-08 13:40:54.000000 dms_variants-1.5.0/tests/count_codonvariant_files/variant_counts.csv
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    26285 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/epistasis_model_preferences.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    11360 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/illuminabarcodeparser_toy_example.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    40077 2024-02-06 23:52:29.000000 dms_variants-1.5.0/tests/monotonicsplineepistasisbottlenecklikelihood_model.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   279040 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/monotonicsplineepistasiscauchylikelihood_model.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   329986 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/monotonicsplineepistasisgaussianlikelihood_model.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   177372 2024-02-06 23:52:29.000000 dms_variants-1.5.0/tests/noepistasisbottlenecklikelihood_model.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)   195617 2024-02-06 23:52:29.000000 dms_variants-1.5.0/tests/noepistasisgaussianlikelihood_model.ipynb
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7654 2024-02-06 23:52:29.000000 dms_variants-1.5.0/tests/test_count_codonvariants.py
--rw-r-----   0 jbloom   (46188) g_jbloom (46188)    62901 2021-12-29 17:41:37.000000 dms_variants-1.5.0/tests/test_escape_scores.ipynb
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:33.540252 dms_variants-1.6.0/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      259 2022-08-04 00:15:21.000000 dms_variants-1.6.0/.flake8
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      148 2024-02-06 23:52:29.000000 dms_variants-1.6.0/.gitignore
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    11675 2024-04-10 22:58:57.000000 dms_variants-1.6.0/CHANGELOG.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7343 2021-12-29 17:41:37.000000 dms_variants-1.6.0/CONTRIBUTING.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1615 2019-06-21 15:41:54.000000 dms_variants-1.6.0/LICENSE.txt
+-rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     1993 2024-04-10 22:59:33.537317 dms_variants-1.6.0/PKG-INFO
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1321 2024-02-06 23:52:29.000000 dms_variants-1.6.0/README.rst
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:32.242525 dms_variants-1.6.0/dms_variants/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      361 2024-04-10 22:58:57.000000 dms_variants-1.6.0/dms_variants/__init__.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1724 2019-08-08 13:40:53.000000 dms_variants-1.6.0/dms_variants/_cutils.c
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6515 2021-12-29 17:41:37.000000 dms_variants-1.6.0/dms_variants/barcodes.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     8054 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/bottlenecks.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   142356 2024-04-10 22:58:57.000000 dms_variants-1.6.0/dms_variants/codonvarianttable.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3019 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/constants.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    10612 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/fastq.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   121007 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/globalepistasis.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    16414 2024-04-10 22:58:57.000000 dms_variants-1.6.0/dms_variants/illuminabarcodeparser.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    39927 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/ispline.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7282 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/pdb_utils.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1978 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/plotnine_themes.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    35620 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/simulate.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    24968 2024-02-06 23:52:29.000000 dms_variants-1.6.0/dms_variants/utils.py
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:32.265893 dms_variants-1.6.0/dms_variants.egg-info/
+-rw-r--r--   0 jbloom   (46188) g_jbloom (46188)     1993 2024-04-10 22:59:31.000000 dms_variants-1.6.0/dms_variants.egg-info/PKG-INFO
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2840 2024-04-10 22:59:31.000000 dms_variants-1.6.0/dms_variants.egg-info/SOURCES.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)        1 2024-04-10 22:59:31.000000 dms_variants-1.6.0/dms_variants.egg-info/dependency_links.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      119 2024-04-10 22:59:31.000000 dms_variants-1.6.0/dms_variants.egg-info/requires.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       13 2024-04-10 22:59:31.000000 dms_variants-1.6.0/dms_variants.egg-info/top_level.txt
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:32.545321 dms_variants-1.6.0/docs/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)        0 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/.nojekyll
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      729 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/Makefile
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3613 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/README.rst
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:32.569886 dms_variants-1.6.0/docs/_static/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   172664 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/_static/BloomLogo.jpg
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      229 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/acknowledgments.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2020-01-20 16:49:17.000000 dms_variants-1.6.0/docs/bottleneck_likelihood.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       66 2019-11-01 04:46:22.000000 dms_variants-1.6.0/docs/codonvariant_plot_formatting.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       59 2019-06-25 13:56:05.000000 dms_variants-1.6.0/docs/codonvariant_sim_data.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       73 2020-04-30 13:10:13.000000 dms_variants-1.6.0/docs/codonvariant_sim_data_multi_targets.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       66 2021-12-28 21:22:43.000000 dms_variants-1.6.0/docs/codonvariant_sim_data_w_gaps.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     6827 2024-02-06 23:52:29.000000 dms_variants-1.6.0/docs/conf.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      129 2019-06-25 13:56:05.000000 dms_variants-1.6.0/docs/doc_requirements.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     1356 2022-03-04 02:18:14.000000 dms_variants-1.6.0/docs/examples.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      546 2019-11-01 04:46:22.000000 dms_variants-1.6.0/docs/index.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      337 2024-02-06 19:24:37.000000 dms_variants-1.6.0/docs/installation.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       55 2019-11-10 02:51:54.000000 dms_variants-1.6.0/docs/narrow_bottleneck.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       65 2019-06-21 15:41:54.000000 dms_variants-1.6.0/docs/package_index.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       60 2019-08-16 16:47:32.000000 dms_variants-1.6.0/docs/parsebarcodes_sim_data.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       49 2022-03-04 02:18:14.000000 dms_variants-1.6.0/docs/prob_escape.nblink
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      282 2021-03-11 17:23:36.000000 dms_variants-1.6.0/environment.yml
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      332 2020-01-29 04:00:43.000000 dms_variants-1.6.0/nbval_sanitize.cfg
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:33.008880 dms_variants-1.6.0/notebooks/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      274 2019-11-01 04:46:22.000000 dms_variants-1.6.0/notebooks/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   323628 2024-02-06 23:52:29.000000 dms_variants-1.6.0/notebooks/bottleneck_likelihood.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   359368 2024-02-06 23:52:29.000000 dms_variants-1.6.0/notebooks/codonvariant_plot_formatting.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)  1972275 2024-04-10 22:58:57.000000 dms_variants-1.6.0/notebooks/codonvariant_sim_data.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)  2502106 2024-04-10 22:58:57.000000 dms_variants-1.6.0/notebooks/codonvariant_sim_data_multi_targets.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   709442 2024-02-06 23:52:29.000000 dms_variants-1.6.0/notebooks/codonvariant_sim_data_w_gaps.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   397564 2024-04-10 22:58:57.000000 dms_variants-1.6.0/notebooks/multi_latent_phenos.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   652437 2024-04-10 22:58:57.000000 dms_variants-1.6.0/notebooks/narrow_bottleneck.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    98567 2024-04-10 22:58:57.000000 dms_variants-1.6.0/notebooks/parsebarcodes_sim_data.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   924393 2024-02-06 23:52:29.000000 dms_variants-1.6.0/notebooks/predict_variants.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   264475 2024-02-06 23:52:29.000000 dms_variants-1.6.0/notebooks/prob_escape.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188) 10191948 2022-03-04 02:18:14.000000 dms_variants-1.6.0/notebooks/prob_escape_codon_variant_table.csv
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     3754 2022-03-04 02:18:14.000000 dms_variants-1.6.0/notebooks/spike.txt
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      523 2024-04-10 18:45:31.000000 dms_variants-1.6.0/pytest.ini
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       38 2024-04-10 22:59:33.541263 dms_variants-1.6.0/setup.cfg
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2062 2024-02-06 23:52:29.000000 dms_variants-1.6.0/setup.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       68 2024-02-06 23:52:29.000000 dms_variants-1.6.0/test_requirements.txt
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:33.115511 dms_variants-1.6.0/tests/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)       13 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/.gitignore
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      122 2019-06-21 15:41:54.000000 dms_variants-1.6.0/tests/README.rst
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    11930 2023-03-19 20:30:35.000000 dms_variants-1.6.0/tests/bottleneck_likelihood_deriv_equations.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    82507 2021-12-29 17:41:37.000000 dms_variants-1.6.0/tests/codonvarianttable_toy_example.ipynb
+drwxr-x---   0 jbloom   (46188) g_jbloom (46188)        0 2024-04-10 22:59:33.514895 dms_variants-1.6.0/tests/count_codonvariant_files/
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     2762 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/PacBio_amplicon.gb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    57804 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/barcode_variant_table.csv
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      855 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/count_codonvariant_files/fates.csv
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394529 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-1_plasmid_R1.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394529 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-1_plasmid_R2.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394540 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-1_uninduced_R1.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394540 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-1_uninduced_R2.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394542 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-2_plasmid_R1.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   394542 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/library-2_plasmid_R2.fastq
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)      121 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/n_variants.csv
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   108174 2019-08-08 13:40:54.000000 dms_variants-1.6.0/tests/count_codonvariant_files/variant_counts.csv
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    26285 2021-12-29 17:41:37.000000 dms_variants-1.6.0/tests/epistasis_model_preferences.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    14551 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/illuminabarcodeparser_toy_example.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    40064 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/monotonicsplineepistasisbottlenecklikelihood_model.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   279027 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/monotonicsplineepistasiscauchylikelihood_model.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   329973 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/monotonicsplineepistasisgaussianlikelihood_model.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   177359 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/noepistasisbottlenecklikelihood_model.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)   195604 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/noepistasisgaussianlikelihood_model.ipynb
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)     7675 2024-04-10 22:58:58.000000 dms_variants-1.6.0/tests/test_count_codonvariants.py
+-rw-r-----   0 jbloom   (46188) g_jbloom (46188)    62901 2021-12-29 17:41:37.000000 dms_variants-1.6.0/tests/test_escape_scores.ipynb
```

### Comparing `dms_variants-1.5.0/CHANGELOG.rst` & `dms_variants-1.6.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com>`_.
 
+1.6.0
+-----
+- Added ability to parse second upstream / downstream region in ``IlluminaBarcodeParser`` by adding ``upstream2`` and ``downstream2`` parameters. Also modified ``IlluminaBarcodeParser`` so that reads will only be parsed if they are long enough to fully cover the region containing the barcodes and specified upstream / downstream sequences. Based on docs, this is how it was supposed to function before but did not. Additionally, this adds another row ("reads too short") to the fates from the barcode parser, as well as the ``outer_flank_fates`` option to report just failing the additional upstream and downstream regions.
+- Change default color of heatmaps made by ``CodonVariantTable`` due to current one being obsolete.
+- Remove obsolete ``guide=False`` from some ``plotnine`` plots in examples / tests (this was removed in ``plotnine`` version 0.13).
+
 1.5.0
 -----
 - Remove use of deprecated ``scipy`` functions like ``flip`` to use ``numpy`` alternatives instead (fixes [this issue](https://github.com/jbloomlab/dms_variants/issues/86)).
 - Re-format code with latest version of ``black``.
 - Lint with ``ruff`` rather than ``flake8``
 - Add ``pyarrow`` as dependency as required by ``pandas``.
 - Tweaks to work with new versions of ``pandas`` and ``plotnine``
```

### Comparing `dms_variants-1.5.0/CONTRIBUTING.rst` & `dms_variants-1.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/LICENSE.txt` & `dms_variants-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/PKG-INFO` & `dms_variants-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dms_variants
-Version: 1.5.0
+Version: 1.6.0
 Summary: Analyze deep mutational scanning of barcoded variants.
 Home-page: https://github.com/jbloomlab/dms_variants
-Download-URL: https://github.com/jbloomlab/dms_variants/tarball/1.5.0
+Download-URL: https://github.com/jbloomlab/dms_variants/tarball/1.6.0
 Author: `the Bloom lab <https://research.fhcrc.org/bloom/en.html>`_
 Author-email: jbloom@fredhutch.org
 License: GPLv3
 Platform: Linux and Mac OS X.
 License-File: LICENSE.txt
 Requires-Dist: binarymap>=0.1
 Requires-Dist: biopython>=1.73
```

### Comparing `dms_variants-1.5.0/README.rst` & `dms_variants-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/_cutils.c` & `dms_variants-1.6.0/dms_variants/_cutils.c`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/barcodes.py` & `dms_variants-1.6.0/dms_variants/barcodes.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/bottlenecks.py` & `dms_variants-1.6.0/dms_variants/bottlenecks.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/codonvarianttable.py` & `dms_variants-1.6.0/dms_variants/codonvarianttable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1930,15 +1930,14 @@
             )
             + p9.scale_x_continuous(
                 name=f"{mut_desc} site",
                 limits=(min(self.sites) - 1, max(self.sites) + 1),
                 expand=(0, 0),
             )
             + p9.ylab(mut_desc)
-            + p9.scale_fill_cmap("gnuplot")
         )
 
         if samples is None:
             if nlibraries > 1 or one_lib_facet:
                 p = p + p9.facet_wrap(
                     "~ library", nrow={"h": 1, "v": nlibraries}[orientation]
                 )
@@ -1995,15 +1994,15 @@
             sample_rename=sample_rename,
             primary_target_only=True,
         ).rename(columns={"count": "nseqs"})
 
         assert "target" not in set(df.columns).union(set(n_variants.columns))
 
         df = (
-            df.groupby(["library", "sample", "mutation_type", "site"])
+            df.groupby(["library", "sample", "mutation_type", "site"], observed=False)
             .aggregate({"count": "sum"})
             .reset_index()
             .merge(n_variants, on=["library", "sample"])
             .assign(freq=lambda x: x["count"] / x["nseqs"])
         )
 
         nlibraries = len(df["library"].unique())
```

### Comparing `dms_variants-1.5.0/dms_variants/constants.py` & `dms_variants-1.6.0/dms_variants/constants.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/fastq.py` & `dms_variants-1.6.0/dms_variants/fastq.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/globalepistasis.py` & `dms_variants-1.6.0/dms_variants/globalepistasis.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/illuminabarcodeparser.py` & `dms_variants-1.6.0/dms_variants/illuminabarcodeparser.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 class IlluminaBarcodeParser:
     """Parser for Illumina barcodes.
 
     Note
     ----
     Barcodes should be read by R1 and optionally R2. Expected arrangement is
 
-        5'-[R2_start]-upstream-barcode-downstream-[R1_start]-3'
+        5'-[R2_start]-upstream2-upstream-barcode-downstream-downstream2-[R1_start]-3'
 
     R1 anneals downstream of barcode and reads backwards. If R2 is used,
     it anneals upstream of barcode and reads forward. There can be sequences
     (`upstream` and `downstream`) on either side of the barcode: `downstream`
     must fully cover region between R1 start and barcode, and if using R2
     then `upstream` must fully cover region between R2 start and barcode.
     However, it is fine if R1 reads backwards past `upstream`, and if `R2`
-    reads forward past `downstream`.
+    reads forward past `downstream`. The `upstream2` and `downstream2`
+    can be used to require additional flanking sequences. Normally these
+    would just be rolled into `upstream` and `downstream`, but you might
+    specify separately if you are actually using these to parse additional
+    indices that you might want to set different mismatch criteria for.
 
     Parameters
     ----------
     bclen : int or `None`
         Barcode length; `None` if length determined from `valid_barcodes`.
     upstream : str
         Sequence upstream of the barcode; empty str if no such sequence.
@@ -68,20 +72,28 @@
 
     Attributes
     ----------
     bclen : int
         Length of barcodes.
     upstream : str
         Sequence upstream of barcode.
+    upstream2 : str
+        Second sequence upstream of barcode.
     downstream : str
         Sequence downstream of barcode.
+    downstream2 : str
+        Second sequence downstream of barcode
     upstream_mismatch : int
         Max number of mismatches allowed in `upstream`.
+    upstream2_mismatch : int
+        Max number of mismatches allowed in `upstream2`.
     downstream_mismatch : int
         Max number of mismatches allowed in `downstream`.
+    downstream2_mismatch : int
+        Max number of mismatches allowed in `downstream2`.
     valid_barcodes : None or set
         If not `None`, set of barcodes to retain.
     bc_orientation : {'R1', 'R2'}
         Is the barcode defined in the orientation read by R1 or R2?
     minq : int
         Require >= this Q score for all bases in barcode for at least one read.
     chastity_filter : bool
@@ -97,35 +109,43 @@
     """str : Valid nucleotide characters in FASTQ files."""
 
     def __init__(
         self,
         *,
         bclen=None,
         upstream="",
+        upstream2="",
         downstream="",
+        downstream2="",
         upstream_mismatch=0,
+        upstream2_mismatch=0,
         downstream_mismatch=0,
+        downstream2_mismatch=0,
         valid_barcodes=None,
         bc_orientation="R1",
         minq=20,
         chastity_filter=True,
         list_all_valid_barcodes=True,
     ):
         """See main class doc string."""
         self.bclen = bclen
-        if regex.match(f"^[{self.VALID_NTS}]*$", upstream):
-            self.upstream = upstream
-        else:
-            raise ValueError(f"invalid chars in upstream {upstream}")
-        if regex.match(f"^[{self.VALID_NTS}]*$", downstream):
-            self.downstream = downstream
-        else:
-            raise ValueError(f"invalid chars in downstream {downstream}")
+        for param_name, param_val in [
+            ("upstream", upstream),
+            ("downstream", downstream),
+            ("upstream2", upstream2),
+            ("downstream2", downstream2),
+        ]:
+            if regex.match(f"^[{self.VALID_NTS}]*$", param_val):
+                setattr(self, param_name, param_val)
+            else:
+                raise ValueError(f"invalid chars in {param_name} {param_val}")
         self.upstream_mismatch = upstream_mismatch
         self.downstream_mismatch = downstream_mismatch
+        self.upstream2_mismatch = upstream2_mismatch
+        self.downstream2_mismatch = downstream2_mismatch
         self.valid_barcodes = valid_barcodes
         if self.valid_barcodes is not None:
             self.valid_barcodes = set(self.valid_barcodes)
             if len(self.valid_barcodes) < 1:
                 raise ValueError("empty list for `valid_barcodes`")
             if self.bclen is None:
                 self.bclen = len(list(self.valid_barcodes)[0])
@@ -138,34 +158,85 @@
             self.bc_orientation = bc_orientation
         else:
             raise ValueError(f"invalid `bc_orientation` {bc_orientation}")
         self.chastity_filter = chastity_filter
         self.list_all_valid_barcodes = list_all_valid_barcodes
 
         # specify information about R1 / R2 matches
-        self._bcend = {
-            "R1": self.bclen + len(self.downstream),
-            "R2": self.bclen + len(self.upstream),
-        }
         self._rcdownstream = reverse_complement(self.downstream)
         self._rcupstream = reverse_complement(self.upstream)
-        self._matches = {"R1": {}, "R2": {}}  # match objects by read length
+        self._rcdownstream2 = reverse_complement(self.downstream2)
+        self._rcupstream2 = reverse_complement(self.upstream2)
+
+        # build the regex read matches
+        self._matchers = {
+            "R1": regex.compile(
+                f"({self._rcdownstream2})"
+                + f"{{s<={self.downstream2_mismatch}}}"
+                + f"({self._rcdownstream})"
+                + f"{{s<={self.downstream_mismatch}}}"
+                + f"(?P<bc>[ACTG]{{{self.bclen}}})"
+                + f"({self._rcupstream})"
+                + f"{{s<={self.upstream_mismatch}}}"
+                + f"({self._rcupstream2})"
+                + f"{{s<={self.upstream2_mismatch}}}"
+            ),
+            "R2": regex.compile(
+                f"({self.upstream2})"
+                + f"{{s<={self.upstream2_mismatch}}}"
+                + f"({self.upstream})"
+                + f"{{s<={self.upstream_mismatch}}}"
+                + f"(?P<bc>[ACTG]{{{self.bclen}}})"
+                + f"({self.downstream})"
+                + f"{{s<={self.downstream_mismatch}}}"
+                + f"({self.downstream2})"
+                + f"{{s<={self.downstream2_mismatch}}}"
+            ),
+        }
+
+        # build matchers that do not have upstream2 or downstream2 if needed
+        self._has_flank2 = (len(self.upstream2) > 0) or (len(self.downstream2) > 0)
+        self._matchers_no_flank2 = {
+            "R1": regex.compile(
+                f"[{self.VALID_NTS}]{{{len(self.downstream2)}}}"
+                + f"({self._rcdownstream})"
+                + f"{{s<={self.downstream_mismatch}}}"
+                + f"(?P<bc>[ACTG]{{{self.bclen}}})"
+                + f"({self._rcupstream})"
+                + f"{{s<={self.upstream_mismatch}}}"
+                + f"[{self.VALID_NTS}]{{{len(self.upstream2)}}}"
+            ),
+            "R2": regex.compile(
+                f"[{self.VALID_NTS}]{{{len(self.upstream2)}}}"
+                + f"^({self.upstream})"
+                + f"{{s<={self.upstream_mismatch}}}"
+                + f"(?P<bc>[ACTG]{{{self.bclen}}})"
+                + f"({self.downstream})"
+                + f"{{s<={self.downstream_mismatch}}}"
+                + f"[{self.VALID_NTS}]{{{len(self.downstream2)}}}"
+            ),
+        }
 
-    def parse(self, r1files, *, r2files=None, add_cols=None):
+    def parse(self, r1files, *, r2files=None, add_cols=None, outer_flank_fates=False):
         """Parse barcodes from files.
 
         Parameters
         ----------
         r1files : str or list
             Name of R1 FASTQ file, or list of such files. Can be gzipped.
         r2files : None, str, or list
             `None` or empty list if not using R2, or like `r1files` for R2.
         add_cols : None or dict
             If dict, specify names and values (i.e., sample or library names)
             to be aded to returned data frames.
+        outer_flank_fates : bool
+            If `True`, if using outer flanking regions then in the output fates
+            specify reads that fail just the outer flanking regions (`upstream2` or
+            `downstream2`). Otherwise, such failures will be grouped with the
+            "unparseable barcode" fate.
 
         Returns
         -------
         tuple
             The 2-tuple `(barcodes, fates)`, where:
                 - `barcodes` is pandas DataFrame giving number of observations
                   of each barcode (columns are "barcode" and "count").
@@ -173,14 +244,17 @@
                   each fate (columns "fate" and "count"). Possible fates:
                   - "failed chastity filter"
                   - "valid barcode"
                   - "invalid barcode": not in barcode whitelist
                   - "R1 / R2 disagree" (if using `r2files`)
                   - "low quality barcode": sequencing quality low
                   - "unparseable barcode": invalid flank sequence, N in barcode
+                  - "read too short": read is too short to cover specified region
+                  - "invalid outer flank" : if using `outer_flank_fates` and
+                    `upstream2` or `downstream2` fails.
 
             Note that these data frames also include any columns specified by
             `add_cols`.
 
         """
         if isinstance(r1files, str):
             r1files = [r1files]
@@ -206,29 +280,38 @@
 
         fates = {
             "failed chastity filter": 0,
             "unparseable barcode": 0,
             "low quality barcode": 0,
             "invalid barcode": 0,
             "valid barcode": 0,
+            "read too short": 0,
         }
         if not r1only:
             fates["R1 / R2 disagree"] = 0
+        if outer_flank_fates and self._has_flank2:
+            fates["invalid outer flank"] = 0
 
-        # max length of interest for reads
-        max_len = self.bclen + len(self.upstream) + len(self.downstream)
+        # min length of interest for reads
+        minlen = (
+            self.bclen
+            + len(self.upstream)
+            + len(self.downstream)
+            + len(self.upstream2)
+            + len(self.downstream2)
+        )
 
         for filetup in zip(*fileslist):
             if r1only:
                 assert len(filetup) == 1
-                iterator = iterate_fastq(filetup[0], check_pair=1, trim=max_len)
+                iterator = iterate_fastq(filetup[0], check_pair=1, trim=minlen)
             else:
                 assert len(filetup) == 2, f"{filetup}\n{fileslist}"
                 iterator = iterate_fastq_pair(
-                    filetup[0], filetup[1], r1trim=max_len, r2trim=max_len
+                    filetup[0], filetup[1], r1trim=minlen, r2trim=minlen
                 )
 
             for entry in iterator:
                 if r1only:
                     readlist = [entry[1]]
                     qlist = [entry[2]]
                     fail = entry[3]
@@ -238,52 +321,26 @@
                     qlist = [entry[3], entry[4]]
                     fail = entry[5]
 
                 if fail and self.chastity_filter:
                     fates["failed chastity filter"] += 1
                     continue
 
-                matches = {}
-                for read, r in zip(reads, readlist):
-                    rlen = len(r)
-
-                    # get or build matcher for read of this length
-                    len_past_bc = rlen - self._bcend[read]
-                    if len_past_bc < 0:
-                        raise ValueError(f"{read} too short: {rlen}")
-                    elif rlen in self._matches[read]:
-                        matcher = self._matches[read][rlen]
-                    else:
-                        if read == "R1":
-                            match_str = (
-                                f"^({self._rcdownstream})"
-                                f"{{s<={self.downstream_mismatch}}}"
-                                f"(?P<bc>[ACTG]{{{self.bclen}}})"
-                                f"({self._rcupstream[: len_past_bc]})"
-                                f"{{s<={self.upstream_mismatch}}}"
-                            )
-                        else:
-                            assert read == "R2"
-                            match_str = (
-                                f"^({self.upstream})"
-                                f"{{s<={self.upstream_mismatch}}}"
-                                f"(?P<bc>[ACTG]{{{self.bclen}}})"
-                                f"({self.downstream[: len_past_bc]})"
-                                f"{{s<={self.downstream_mismatch}}}"
-                            )
-                        matcher = regex.compile(match_str, flags=regex.BESTMATCH)
-                        self._matches[read][rlen] = matcher
-
-                    m = matcher.match(r)
-                    if m:
-                        matches[read] = m
-                    else:
-                        break
+                if any(len(r) < minlen for r in readlist):
+                    fates["read too short"] += 1
+                    continue
+
+                assert all(len(r) == minlen for r in readlist)
+
+                matches = {
+                    read: self._matchers[read].fullmatch(r)
+                    for (read, r) in zip(reads, readlist)
+                }
 
-                if len(matches) == len(reads):
+                if all(m is not None for m in matches.values()):
                     bc = {}
                     bc_q = {}
                     for read, q in zip(reads, qlist):
                         bc[read] = matches[read].group("bc")
                         bc_q[read] = qual_str_to_array(
                             q[matches[read].start("bc") : matches[read].end("bc")]
                         )
@@ -317,14 +374,23 @@
                             ).all():
                                 barcodes[bc["R1"]] += 1
                                 fates["valid barcode"] += 1
                             else:
                                 fates["low quality barcode"] += 1
                         else:
                             fates["R1 / R2 disagree"] += 1
+                elif (
+                    outer_flank_fates
+                    and self._has_flank2
+                    and all(
+                        self._matchers_no_flank2[read].fullmatch(r) is not None
+                        for (read, r) in zip(reads, readlist)
+                    )
+                ):
+                    fates["invalid outer flank"] += 1
                 else:
                     # invalid flanking sequence or N in barcode
                     fates["unparseable barcode"] += 1
 
         if add_cols is None:
             add_cols = {}
         existing_cols = {"barcode", "count", "fate"}
```

### Comparing `dms_variants-1.5.0/dms_variants/ispline.py` & `dms_variants-1.6.0/dms_variants/ispline.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/pdb_utils.py` & `dms_variants-1.6.0/dms_variants/pdb_utils.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/plotnine_themes.py` & `dms_variants-1.6.0/dms_variants/plotnine_themes.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/simulate.py` & `dms_variants-1.6.0/dms_variants/simulate.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants/utils.py` & `dms_variants-1.6.0/dms_variants/utils.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/dms_variants.egg-info/PKG-INFO` & `dms_variants-1.6.0/dms_variants.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dms-variants
-Version: 1.5.0
+Version: 1.6.0
 Summary: Analyze deep mutational scanning of barcoded variants.
 Home-page: https://github.com/jbloomlab/dms_variants
-Download-URL: https://github.com/jbloomlab/dms_variants/tarball/1.5.0
+Download-URL: https://github.com/jbloomlab/dms_variants/tarball/1.6.0
 Author: `the Bloom lab <https://research.fhcrc.org/bloom/en.html>`_
 Author-email: jbloom@fredhutch.org
 License: GPLv3
 Platform: Linux and Mac OS X.
 License-File: LICENSE.txt
 Requires-Dist: binarymap>=0.1
 Requires-Dist: biopython>=1.73
```

### Comparing `dms_variants-1.5.0/dms_variants.egg-info/SOURCES.txt` & `dms_variants-1.6.0/dms_variants.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/Makefile` & `dms_variants-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/README.rst` & `dms_variants-1.6.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/_static/BloomLogo.jpg` & `dms_variants-1.6.0/docs/_static/BloomLogo.jpg`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/conf.py` & `dms_variants-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/examples.rst` & `dms_variants-1.6.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/docs/index.rst` & `dms_variants-1.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/bottleneck_likelihood.ipynb` & `dms_variants-1.6.0/notebooks/bottleneck_likelihood.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/codonvariant_plot_formatting.ipynb` & `dms_variants-1.6.0/notebooks/codonvariant_plot_formatting.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/codonvariant_sim_data.ipynb` & `dms_variants-1.6.0/notebooks/codonvariant_sim_data.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999900635930048%*

 * *Differences: {"'cells'": "{96: {'source': {insert: [(13, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [13]}}}'}*

```diff
@@ -3580,15 +3580,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw(show=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/notebooks/codonvariant_sim_data_multi_targets.ipynb` & `dms_variants-1.6.0/notebooks/codonvariant_sim_data_multi_targets.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999880268199234%*

 * *Differences: {"'cells'": "{114: {'source': {insert: [(13, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [13]}}}'}*

```diff
@@ -5426,15 +5426,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "\n",
                 "_ = p.draw(show=True)"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `dms_variants-1.5.0/notebooks/codonvariant_sim_data_w_gaps.ipynb` & `dms_variants-1.6.0/notebooks/codonvariant_sim_data_w_gaps.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/multi_latent_phenos.ipynb` & `dms_variants-1.6.0/notebooks/multi_latent_phenos.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999780701754386%*

 * *Differences: {"'cells'": "{41: {'source': {insert: [(11, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [11]}}}'}*

```diff
@@ -764,15 +764,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_wrap(\"~ library\", nrow=1)\n",
                 "    + theme(\n",
                 "        figure_size=(2.25 * len(variants.libraries), 2),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw(show=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/notebooks/narrow_bottleneck.ipynb` & `dms_variants-1.6.0/notebooks/narrow_bottleneck.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999789029535865%*

 * *Differences: {"'cells'": "{46: {'source': {insert: [(11, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [11]}}}'}*

```diff
@@ -831,15 +831,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_wrap(\"~ post_sample\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(bottlenecks), 2 * len(libs)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw(show=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/notebooks/predict_variants.ipynb` & `dms_variants-1.6.0/notebooks/predict_variants.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/prob_escape.ipynb` & `dms_variants-1.6.0/notebooks/prob_escape.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/prob_escape_codon_variant_table.csv` & `dms_variants-1.6.0/notebooks/prob_escape_codon_variant_table.csv`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/notebooks/spike.txt` & `dms_variants-1.6.0/notebooks/spike.txt`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/pytest.ini` & `dms_variants-1.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/setup.py` & `dms_variants-1.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/bottleneck_likelihood_deriv_equations.ipynb` & `dms_variants-1.6.0/tests/bottleneck_likelihood_deriv_equations.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/codonvarianttable_toy_example.ipynb` & `dms_variants-1.6.0/tests/codonvarianttable_toy_example.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/PacBio_amplicon.gb` & `dms_variants-1.6.0/tests/count_codonvariant_files/PacBio_amplicon.gb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/barcode_variant_table.csv` & `dms_variants-1.6.0/tests/count_codonvariant_files/barcode_variant_table.csv`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/fates.csv` & `dms_variants-1.6.0/tests/count_codonvariant_files/fates.csv`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 fate,count,library,sample,run
 invalid barcode,1739,library-1,plasmid,run-1
 low quality barcode,480,library-1,plasmid,run-1
 unparseable barcode,281,library-1,plasmid,run-1
 failed chastity filter,0,library-1,plasmid,run-1
+read too short,0,library-1,plasmid,run-1
 valid barcode,0,library-1,plasmid,run-1
 invalid barcode,1761,library-1,uninduced,run-1
 low quality barcode,374,library-1,uninduced,run-1
 unparseable barcode,362,library-1,uninduced,run-1
 valid barcode,3,library-1,uninduced,run-1
 failed chastity filter,0,library-1,uninduced,run-1
+read too short,0,library-1,uninduced,run-1
 invalid barcode,1844,library-2,plasmid,run-1
 low quality barcode,435,library-2,plasmid,run-1
 unparseable barcode,220,library-2,plasmid,run-1
 valid barcode,1,library-2,plasmid,run-1
 failed chastity filter,0,library-2,plasmid,run-1
+read too short,0,library-2,plasmid,run-1
```

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-1_plasmid_R1.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-1_plasmid_R1.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-1_plasmid_R2.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-1_plasmid_R2.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-1_uninduced_R1.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-1_uninduced_R1.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-1_uninduced_R2.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-1_uninduced_R2.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-2_plasmid_R1.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-2_plasmid_R1.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/library-2_plasmid_R2.fastq` & `dms_variants-1.6.0/tests/count_codonvariant_files/library-2_plasmid_R2.fastq`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/count_codonvariant_files/variant_counts.csv` & `dms_variants-1.6.0/tests/count_codonvariant_files/variant_counts.csv`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/epistasis_model_preferences.ipynb` & `dms_variants-1.6.0/tests/epistasis_model_preferences.ipynb`

 * *Files identical despite different names*

### Comparing `dms_variants-1.5.0/tests/monotonicsplineepistasisbottlenecklikelihood_model.ipynb` & `dms_variants-1.6.0/tests/monotonicsplineepistasisbottlenecklikelihood_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999806501547988%*

 * *Differences: {"'cells'": "{32: {'source': {insert: [(13, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [13]}}}'}*

```diff
@@ -486,15 +486,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/tests/monotonicsplineepistasiscauchylikelihood_model.ipynb` & `dms_variants-1.6.0/tests/monotonicsplineepistasiscauchylikelihood_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999803921568627%*

 * *Differences: {"'cells'": "{36: {'source': {insert: [(11, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [11]}}}'}*

```diff
@@ -741,15 +741,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/tests/monotonicsplineepistasisgaussianlikelihood_model.ipynb` & `dms_variants-1.6.0/tests/monotonicsplineepistasisgaussianlikelihood_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999861111111111%*

 * *Differences: {"'cells'": "{36: {'source': {insert: [(11, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [11]}}}'}*

```diff
@@ -601,15 +601,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/tests/noepistasisbottlenecklikelihood_model.ipynb` & `dms_variants-1.6.0/tests/noepistasisbottlenecklikelihood_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999762808349146%*

 * *Differences: {"'cells'": "{32: {'source': {insert: [(13, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [13]}}}'}*

```diff
@@ -399,15 +399,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/tests/noepistasisgaussianlikelihood_model.ipynb` & `dms_variants-1.6.0/tests/noepistasisgaussianlikelihood_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999985294117647%*

 * *Differences: {"'cells'": "{36: {'source': {insert: [(13, '    + scale_fill_manual(values=CBPALETTE[1:])\\n')], "*

 * *            'delete: [13]}}}'}*

```diff
@@ -701,15 +701,15 @@
                 "    + xlab(\"\")\n",
                 "    + facet_grid(\"post_sample ~ library\")\n",
                 "    + theme(\n",
                 "        figure_size=(2.75 * len(libs), 2 * len(bottlenecks)),\n",
                 "        axis_text_x=element_text(angle=90),\n",
                 "        panel_grid_major_x=element_blank(),  # no vertical grid lines\n",
                 "    )\n",
-                "    + scale_fill_manual(values=CBPALETTE[1:], guide=False)\n",
+                "    + scale_fill_manual(values=CBPALETTE[1:])\n",
                 ")\n",
                 "_ = p.draw()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `dms_variants-1.5.0/tests/test_count_codonvariants.py` & `dms_variants-1.6.0/tests/test_count_codonvariants.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,14 +151,15 @@
 
         # concatenate read fates into one data frame
         fates = pd.concat(fates, ignore_index=True, sort=False).assign(
             count=lambda x: x["count"].fillna(0).astype("int")
         )
 
         fatesfile = os.path.join(indir, "fates.csv")
+        print(fates)
         assert_frame_equal(fates, pd.read_csv(fatesfile))
 
         libs_to_analyze = ["library-1"]
 
         for mut_type in ["aa", "codon"]:
             _ = variants.plotNumMutsHistogram(
                 mut_type, libraries=libs_to_analyze, max_muts=7, orientation="v"
```

### Comparing `dms_variants-1.5.0/tests/test_escape_scores.ipynb` & `dms_variants-1.6.0/tests/test_escape_scores.ipynb`

 * *Files identical despite different names*

