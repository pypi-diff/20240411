# Comparing `tmp/multiqc_sgr-1.21.0.tar.gz` & `tmp/multiqc_sgr-1.22.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiqc_sgr-1.21.0.tar", last modified: Thu Apr 11 08:14:07 2024, max compression
+gzip compressed data, was "multiqc_sgr-1.22.post0.tar", last modified: Fri Mar 22 05:36:04 2024, max compression
```

## Comparing `multiqc_sgr-1.21.0.tar` & `multiqc_sgr-1.22.post0.tar`

### file list

```diff
@@ -1,739 +1,711 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.384896 multiqc_sgr-1.21.0/
--rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44731 2024-04-11 08:14:07.384896 multiqc_sgr-1.21.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.268895 multiqc_sgr-1.21.0/multiqc/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      711 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.268895 multiqc_sgr-1.21.0/multiqc/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/adapterRemoval/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/adapterRemoval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/adapterRemoval/adapterRemoval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/afterqc/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/afterqc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5639 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/afterqc/afterqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/anglerfish/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/anglerfish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/anglerfish/anglerfish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/bakta/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bakta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bakta/bakta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/bamdst/
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bamdst/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17969 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bamdst/bamdst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/bamtools/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bamtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bamtools/bamtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bamtools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27482 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/base_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.272895 multiqc_sgr-1.21.0/multiqc/modules/bbduk/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbduk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6823 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbduk/bbduk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/bbmap/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/bbmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/bbmap_filetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_aqhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_basic_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_bhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_bqhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_covhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_idhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_ihist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_indelhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_mhist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_qahist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_qchist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_qhist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/bcftools/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bcftools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bcftools/bcftools.py
--rw-r--r--   0 runner    (1001) docker     (127)    21499 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bcftools/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/bcl2fastq/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bcl2fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23115 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bcl2fastq/bcl2fastq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/bclconvert/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bclconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40023 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bclconvert/bclconvert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/biobambam2/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biobambam2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biobambam2/biobambam2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.276895 multiqc_sgr-1.21.0/multiqc/modules/biobloomtools/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biobloomtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biobloomtools/biobloomtools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/biscuit/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biscuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46465 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/biscuit/biscuit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/bismark/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bismark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22267 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bismark/bismark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/bowtie1/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bowtie1/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5868 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bowtie1/bowtie1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/bowtie2/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bowtie2/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13231 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bowtie2/bowtie2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/bracken/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bracken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bracken/bracken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/busco/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/busco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/busco/busco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/bustools/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bustools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/bustools/bustools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/ccs/
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ccs/ccs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.280895 multiqc_sgr-1.21.0/multiqc/modules/cellranger/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cellranger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cellranger/cellranger.py
--rw-r--r--   0 runner    (1001) docker     (127)    21274 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cellranger/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cellranger/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cellranger/vdj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/checkqc/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/checkqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23236 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/checkqc/checkqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/clipandmerge/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/clipandmerge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/clipandmerge/clipandmerge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/clusterflow/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/clusterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14928 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/clusterflow/clusterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/conpair/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/conpair/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/conpair/conpair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/custom_content/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/custom_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/custom_content/custom_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/cutadapt/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cutadapt/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19133 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/cutadapt/cutadapt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/damageprofiler/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/damageprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/damageprofiler/damageprofiler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.284895 multiqc_sgr-1.21.0/multiqc/modules/dedup/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dedup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dedup/dedup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.288895 multiqc_sgr-1.21.0/multiqc/modules/deeptools/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/bamPEFragmentSizeDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/bamPEFragmentSizeTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/deeptools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/estimateReadFiltering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotCorrelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotCoverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotEnrichment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotFingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotPCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.288895 multiqc_sgr-1.21.0/multiqc/modules/diamond/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/diamond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/diamond/diamond.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.288895 multiqc_sgr-1.21.0/multiqc/modules/disambiguate/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/disambiguate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/disambiguate/disambiguate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/dragen/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)    76479 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_per_contig.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5382 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/dragen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/dragen_gc_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/fragment_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    34589 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/mapping_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/overall_mean_cov.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/ploidy_estimation_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/rna_quant_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/rna_transcript_cov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/sc_atac_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/sc_rna_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/time_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/trimmer_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen/vc_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.252895 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    24776 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/assets/js/multiqc_dragen_fastqc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/base_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/content_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4288 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/dragen_fastqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/gc_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/read_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/eigenstratdatabasetools/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/eigenstratdatabasetools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3399 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/eigenstratdatabasetools/eigenstratdatabasetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/fastp/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20455 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastp/fastp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/fastq_screen/
--rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastq_screen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11366 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastq_screen/fastq_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/fastqc/
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.252895 multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/css/multiqc_fastqc.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.292895 multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)    24501 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/js/multiqc_fastqc.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    55955 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_genome.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_txome.txt
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_genome.txt
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_txome.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/featureCounts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/featureCounts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/featureCounts/feature_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/fgbio/
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fgbio/ErrorRateByReadPosition.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fgbio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fgbio/fgbio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/fgbio/groupreadsbyumi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/filtlong/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/filtlong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/filtlong/filtlong.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/flash/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/flash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9487 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/flash/flash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/flexbar/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/flexbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/flexbar/flexbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/freyja/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/freyja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/freyja/freyja.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.296895 multiqc_sgr-1.21.0/multiqc/modules/gatk/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gatk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gatk/analyze_saturation_mutagenesis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gatk/base_recalibrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gatk/gatk.py
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gatk/varianteval.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/gffcompare/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gffcompare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gffcompare/gffcompare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/goleft_indexcov/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/goleft_indexcov/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/goleft_indexcov/goleft_indexcov.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/gopeaks/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gopeaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/gopeaks/gopeaks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/happy/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/happy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/happy/happy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hicexplorer/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicexplorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicexplorer/hicexplorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hicpro/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicpro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicpro/hicpro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hicup/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hicup/hicup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hifiasm/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hifiasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hifiasm/hifiasm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hisat2/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hisat2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hisat2/hisat2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/homer/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/homer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/homer/findpeaks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/homer/homer.py
--rw-r--r--   0 runner    (1001) docker     (127)    20173 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/homer/tagdirectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.300896 multiqc_sgr-1.21.0/multiqc/modules/hops/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/hops/hops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/htseq/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/htseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/htseq/htseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/humid/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/counts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/humid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/neighbours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/humid/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/interop/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/interop/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19184 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/interop/interop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/isoseq/
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/isoseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/isoseq/isoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/ivar/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ivar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ivar/ivar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/jcvi/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/jcvi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/jcvi/jcvi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/jellyfish/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/jellyfish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/jellyfish/jellyfish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/kaiju/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kaiju/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kaiju/kaiju.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.304895 multiqc_sgr-1.21.0/multiqc/modules/kallisto/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kallisto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kallisto/kallisto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/kat/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kat/kat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/kraken/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kraken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20481 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/kraken/kraken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/leehom/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/leehom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/leehom/leehom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/librarian/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/librarian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/librarian/librarian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/lima/
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/lima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13723 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/lima/lima.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/longranger/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/longranger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18595 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/longranger/longranger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/macs2/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/macs2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/macs2/macs2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/malt/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/malt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/malt/malt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/mapdamage/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mapdamage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mapdamage/mapdamage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/megahit/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/megahit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/megahit/megahit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/metaphlan/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/metaphlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/metaphlan/metaphlan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.308895 multiqc_sgr-1.21.0/multiqc/modules/methylqa/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/methylqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/methylqa/methylqa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/minionqc/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/minionqc/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/minionqc/minionqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/mirtop/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mirtop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mirtop/mirtop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/mirtrace/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mirtrace/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13829 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mirtrace/mirtrace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/mosdepth/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mosdepth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24592 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mosdepth/mosdepth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/motus/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/motus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/motus/motus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/mtnucratio/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mtnucratio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/mtnucratio/mtnucratio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/multivcfanalyzer/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/multivcfanalyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/multivcfanalyzer/multivcfanalyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/nanostat/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nanostat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nanostat/nanostat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/nextclade/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nextclade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nextclade/nextclade.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/ngsderive/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ngsderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/ngsderive/ngsderive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.312896 multiqc_sgr-1.21.0/multiqc/modules/nonpareil/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nonpareil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15590 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/nonpareil/nonpareil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/odgi/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/odgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/odgi/odgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/optitype/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/optitype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/optitype/optitype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/pangolin/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pangolin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pangolin/pangolin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/pbmarkdup/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pbmarkdup/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5209 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pbmarkdup/pbmarkdup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/peddy/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/peddy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/peddy/peddy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.316896 multiqc_sgr-1.21.0/multiqc/modules/phantompeakqualtools/
--rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/phantompeakqualtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/phantompeakqualtools/phantompeakqualtools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/picard/
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/AlignmentSummaryMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/BaseDistributionByCycleMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15256 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/CrosscheckFingerprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/ExtractIlluminaBarcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/GcBiasMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20365 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/HsMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/IlluminaBasecallingMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/IlluminaLaneMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/InsertSizeMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/MarkDuplicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/MarkIlluminaAdapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/OxoGMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/QualityByCycleMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/QualityScoreDistributionMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/QualityYieldMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/RnaSeqMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/RrbsSummaryMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/TargetedPcrMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/ValidateSamFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/VariantCallingMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/WgsMetrics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3212 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/picard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/picard/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/porechop/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/porechop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/porechop/porechop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/preseq/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/preseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/preseq/preseq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/prinseqplusplus/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/prinseqplusplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/prinseqplusplus/prinseqplusplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/profile_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/prokka/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/prokka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/prokka/prokka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.320896 multiqc_sgr-1.21.0/multiqc/modules/purple/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/purple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/purple/purple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/pychopper/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pychopper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pychopper/pychopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/pycoqc/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pycoqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/pycoqc/pycoqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/qc3C/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qc3C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44688 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qc3C/qc3C.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/qorts/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qorts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14283 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qorts/qorts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/qualimap/
--rw-r--r--   0 runner    (1001) docker     (127)    29897 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qualimap/QM_BamQC.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qualimap/QM_RNASeq.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3611 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qualimap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2243 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/qualimap/qualimap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/quast/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/quast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/quast/quast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/rna_seqc/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rna_seqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13822 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rna_seqc/rna_seqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/rockhopper/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rockhopper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rockhopper/rockhopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.324896 multiqc_sgr-1.21.0/multiqc/modules/rsem/
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rsem/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7255 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rsem/rsem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.328896 multiqc_sgr-1.21.0/multiqc/modules/rseqc/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.260895 multiqc_sgr-1.21.0/multiqc/modules/rseqc/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.328896 multiqc_sgr-1.21.0/multiqc/modules/rseqc/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/assets/js/multiqc_rseqc.js
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/bam_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/gene_body_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/infer_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/inner_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/junction_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/junction_saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_duplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_gc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/rseqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/rseqc/tin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.328896 multiqc_sgr-1.21.0/multiqc/modules/salmon/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/salmon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/salmon/salmon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.328896 multiqc_sgr-1.21.0/multiqc/modules/sambamba/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sambamba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sambamba/markdup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sambamba/sambamba.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.328896 multiqc_sgr-1.21.0/multiqc/modules/samblaster/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samblaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samblaster/samblaster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/samtools/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/flagstat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/idxstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/rmdup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/samtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/samtools/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/sargasso/
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sargasso/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5877 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sargasso/sargasso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/seqera_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqera_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqera_cli/seqera_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/seqwho/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqwho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqwho/seqwho.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/seqyclean/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqyclean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/seqyclean/seqyclean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/sexdeterrmine/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sexdeterrmine/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6471 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sexdeterrmine/sexdeterrmine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/sickle/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sickle/sickle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/skewer/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/skewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/skewer/skewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/slamdunk/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/slamdunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/slamdunk/slamdunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/snippy/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snippy/snippy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.332896 multiqc_sgr-1.21.0/multiqc/modules/snpeff/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snpeff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12226 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snpeff/snpeff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/snpsplit/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snpsplit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/snpsplit/snpsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/software_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/somalier/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/somalier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26969 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/somalier/somalier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/sortmerna/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sortmerna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sortmerna/sortmerna.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/sourmash/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sourmash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sourmash/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     9812 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sourmash/gather.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/sourmash/sourmash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/spaceranger/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/spaceranger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/spaceranger/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16223 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/spaceranger/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/spaceranger/spaceranger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/stacks/stacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/star/
--rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/star/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12592 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/star/star.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/starsolo/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/starsolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/starsolo/starsolo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.336896 multiqc_sgr-1.21.0/multiqc/modules/supernova/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/supernova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/supernova/supernova.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/theta2/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/theta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/theta2/theta2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/tophat/
--rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/tophat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6122 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/tophat/tophat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/trimmomatic/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/trimmomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/trimmomatic/trimmomatic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/truvari/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/truvari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10499 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/truvari/bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/truvari/truvari.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/umitools/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/umitools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12075 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/umitools/umitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/varscan2/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/varscan2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/varscan2/varscan2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/vcftools/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/relatedness2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_by_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_by_qual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vcftools/vcftools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.340896 multiqc_sgr-1.21.0/multiqc/modules/vep/
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vep/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14834 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/vep/vep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.344896 multiqc_sgr-1.21.0/multiqc/modules/verifybamid/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/verifybamid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/verifybamid/verifybamid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.344896 multiqc_sgr-1.21.0/multiqc/modules/whatshap/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/whatshap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18781 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/whatshap/whatshap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.344896 multiqc_sgr-1.21.0/multiqc/modules/xengsort/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/xengsort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/xengsort/xengsort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.344896 multiqc_sgr-1.21.0/multiqc/modules/xenome/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/xenome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/modules/xenome/xenome.py
--rw-r--r--   0 runner    (1001) docker     (127)    54386 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/multiqc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.344896 multiqc_sgr-1.21.0/multiqc/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7609 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/bargraph.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/beeswarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/linegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.348896 multiqc_sgr-1.21.0/multiqc/plots/plotly/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/box.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    13693 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/line.py
--rw-r--r--   0 runner    (1001) docker     (127)    25647 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/plotly/violin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    16876 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/table_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/plots/violin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.348896 multiqc_sgr-1.21.0/multiqc/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.348896 multiqc_sgr-1.21.0/multiqc/templates/default/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.264895 multiqc_sgr-1.21.0/multiqc/templates/default/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.348896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   120734 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    19760 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/default_multiqc.css
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/jquery.toast.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.352896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.352896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/
--rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/MultiQC_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/MultiQC_logo_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/seqera_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/seqera_logo_mono.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.352896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/flat.js
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/multiqc.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.364896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2446 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/FileSaver.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/bootstrap.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    10286 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    86709 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery-3.1.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    44365 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery.tablesorter.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery.toast.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    97630 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jszip.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/lz-string.min.js
--rw-r--r--   0 runner    (1001) docker     (127)  8555428 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.js
--rw-r--r--   0 runner    (1001) docker     (127)  3598197 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.372896 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/bar.js
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/box.js
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/heatmap.js
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/line.js
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/scatter.js
--rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/violin.js
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plotting.js
--rw-r--r--   0 runner    (1001) docker     (127)    16233 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/tables.js
--rw-r--r--   0 runner    (1001) docker     (127)    44291 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/toolbox.js
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/content.html
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/foot.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/general_stats.html
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/includes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)    15439 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/default/toolbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.372896 multiqc_sgr-1.21.0/multiqc/templates/gathered/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/gathered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/gathered/content.html
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/gathered/nav.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.372896 multiqc_sgr-1.21.0/multiqc/templates/geo/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.268895 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.372896 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)   110058 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.376896 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1543 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/emailme.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    47162 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/flames.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     8777 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/glyphicons-halflings-white.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    13826 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/glyphicons-halflings.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    20655 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/hot.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    74176 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/mchammer.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    18387 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/microfab.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/new.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     9959 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/new2.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/progress.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     4224 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/rainbow.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)    10863 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/stars.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/geo/includes.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.376896 multiqc_sgr-1.21.0/multiqc/templates/highcharts/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.268895 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.376896 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/css/default_multiqc.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.376896 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/multiqc_mpl.js
--rw-r--r--   0 runner    (1001) docker     (127)    63654 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/multiqc_plotting.js
--rw-r--r--   0 runner    (1001) docker     (127)    14284 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/multiqc_tables.js
--rw-r--r--   0 runner    (1001) docker     (127)    43475 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/multiqc_toolbox.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.376896 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4870 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/highcharts.export-csv.js
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/highcharts.exporting.js
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/highcharts.heatmap.js
--rw-r--r--   0 runner    (1001) docker     (127)   192694 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/highcharts.js
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/assets/js/packages/highcharts.offline-exporting.js
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/includes.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.380896 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17493 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/bargraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/beeswarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    17689 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/linegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/highcharts/plots/table_object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.380896 multiqc_sgr-1.21.0/multiqc/templates/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/sections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/sections/content.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.380896 multiqc_sgr-1.21.0/multiqc/templates/simple/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/foot.html
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/includes.html
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/nav.html
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/templates/simple/toolbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.380896 multiqc_sgr-1.21.0/multiqc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18573 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/config_defaults.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    15173 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/lzstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/megaqc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/mqc_colour.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/plugin_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    22616 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    25208 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/search_patterns.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/software_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/strict_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/multiqc/utils/util_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:14:07.384896 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44731 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21886 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 08:14:07.000000 multiqc_sgr-1.21.0/multiqc_sgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 08:14:07.384896 multiqc_sgr-1.21.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-04-11 08:13:35.000000 multiqc_sgr-1.21.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.088191 multiqc_sgr-1.22.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45070 2024-03-22 05:36:04.088191 multiqc_sgr-1.22.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      695 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/adapterremoval/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/adapterremoval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16191 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/adapterremoval/adapterremoval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/afterqc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/afterqc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5639 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/afterqc/afterqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/anglerfish/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/anglerfish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/anglerfish/anglerfish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/bakta/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bakta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bakta/bakta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.972191 multiqc_sgr-1.22.post0/multiqc/modules/bamdst/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bamdst/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17969 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bamdst/bamdst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.976191 multiqc_sgr-1.22.post0/multiqc/modules/bamtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bamtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bamtools/bamtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bamtools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27525 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/base_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.976191 multiqc_sgr-1.22.post0/multiqc/modules/bbduk/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbduk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbduk/bbduk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.976191 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/bbmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/bbmap_filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_aqhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_basic_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_bhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_bqhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_covhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_idhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_ihist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_indelhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_mhist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_qahist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_qchist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_qhist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.976191 multiqc_sgr-1.22.post0/multiqc/modules/bcftools/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bcftools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bcftools/bcftools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22191 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bcftools/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bcl2fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bcl2fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23070 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bcl2fastq/bcl2fastq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bclconvert/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bclconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39918 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bclconvert/bclconvert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/biobambam2/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biobambam2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biobambam2/biobambam2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/biobloomtools/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biobloomtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biobloomtools/biobloomtools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/biscuit/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biscuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46393 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/biscuit/biscuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bismark/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bismark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22261 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bismark/bismark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bowtie1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bowtie1/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5800 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bowtie1/bowtie1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bowtie2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bowtie2/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13163 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bowtie2/bowtie2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bracken/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bracken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bracken/bracken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/busco/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/busco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/busco/busco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.980191 multiqc_sgr-1.22.post0/multiqc/modules/bustools/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bustools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11998 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/bustools/bustools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/ccs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12628 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ccs/ccs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/cellranger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21229 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14227 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cellranger/vdj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/checkqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/checkqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23236 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/checkqc/checkqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/clipandmerge/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/clipandmerge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/clipandmerge/clipandmerge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/clusterflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/clusterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14929 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/clusterflow/clusterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/conpair/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/conpair/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/conpair/conpair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/custom_content/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/custom_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28087 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/custom_content/custom_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/cutadapt/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cutadapt/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19131 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/cutadapt/cutadapt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/damageprofiler/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/damageprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/damageprofiler/damageprofiler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.984191 multiqc_sgr-1.22.post0/multiqc/modules/dedup/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dedup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dedup/dedup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.988191 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/bamPEFragmentSizeDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/bamPEFragmentSizeTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/deeptools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/estimateReadFiltering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotCorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotCoverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotEnrichment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotFingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotPCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotProfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.988191 multiqc_sgr-1.22.post0/multiqc/modules/diamond/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/diamond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/diamond/diamond.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.988191 multiqc_sgr-1.22.post0/multiqc/modules/disambiguate/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/disambiguate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/disambiguate/disambiguate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.992191 multiqc_sgr-1.22.post0/multiqc/modules/dragen/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76480 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_per_contig.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5382 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/dragen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/dragen_gc_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/fragment_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34589 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/mapping_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/overall_mean_cov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/ploidy_estimation_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/rna_quant_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/rna_transcript_cov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/sc_atac_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/sc_rna_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/time_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/trimmer_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen/vc_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.992191 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.952191 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.992191 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    23322 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/assets/js/multiqc_dragen_fastqc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/base_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/content_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4288 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/dragen_fastqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/gc_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/read_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.992191 multiqc_sgr-1.22.post0/multiqc/modules/eigenstratdatabasetools/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/eigenstratdatabasetools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3399 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/eigenstratdatabasetools/eigenstratdatabasetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.992191 multiqc_sgr-1.22.post0/multiqc/modules/fastp/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20457 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastp/fastp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fastq_screen/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       69 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastq_screen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11360 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastq_screen/fastq_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.952191 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/css/multiqc_fastqc.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/js/multiqc_fastqc.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55759 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_genome.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_txome.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_genome.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_txome.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/featureCounts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       71 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/featureCounts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5993 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/featureCounts/feature_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/fgbio/
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fgbio/ErrorRateByReadPosition.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fgbio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fgbio/fgbio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/fgbio/groupreadsbyumi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/filtlong/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/filtlong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/filtlong/filtlong.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/flash/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/flash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9463 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/flash/flash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/flexbar/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/flexbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/flexbar/flexbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.996191 multiqc_sgr-1.22.post0/multiqc/modules/freyja/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/freyja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/freyja/freyja.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/gatk/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gatk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19821 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gatk/analyze_saturation_mutagenesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gatk/base_recalibrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gatk/gatk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11045 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gatk/varianteval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/gffcompare/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gffcompare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11523 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gffcompare/gffcompare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/goleft_indexcov/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/goleft_indexcov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/goleft_indexcov/goleft_indexcov.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/gopeaks/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gopeaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/gopeaks/gopeaks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/happy/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/happy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/happy/happy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/hicexplorer/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicexplorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicexplorer/hicexplorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/hicpro/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicpro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21137 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicpro/hicpro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/hicup/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hicup/hicup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/hifiasm/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hifiasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hifiasm/hifiasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.000191 multiqc_sgr-1.22.post0/multiqc/modules/hisat2/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hisat2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hisat2/hisat2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/homer/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/homer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/homer/findpeaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/homer/homer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20246 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/homer/tagdirectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/hops/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/hops/hops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/htseq/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/htseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/htseq/htseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/humid/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/humid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/humid/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/interop/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/interop/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19184 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/interop/interop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/isoseq/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/isoseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/isoseq/isoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/ivar/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ivar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ivar/ivar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/jcvi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/jcvi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/jcvi/jcvi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.004191 multiqc_sgr-1.22.post0/multiqc/modules/jellyfish/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/jellyfish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/jellyfish/jellyfish.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/kaiju/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kaiju/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13338 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kaiju/kaiju.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/kallisto/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kallisto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kallisto/kallisto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/kat/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kat/kat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/kraken/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kraken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20481 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/kraken/kraken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/leehom/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/leehom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/leehom/leehom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/librarian/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/librarian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/librarian/librarian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/lima/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/lima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13723 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/lima/lima.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/longranger/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/longranger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18595 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/longranger/longranger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/macs2/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/macs2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/macs2/macs2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.008191 multiqc_sgr-1.22.post0/multiqc/modules/malt/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/malt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/malt/malt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/mapdamage/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mapdamage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mapdamage/mapdamage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/megahit/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/megahit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/megahit/megahit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/metaphlan/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/metaphlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/metaphlan/metaphlan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/methylqa/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/methylqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/methylqa/methylqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/minionqc/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/minionqc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/minionqc/minionqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/mirtop/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mirtop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10520 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mirtop/mirtop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/mirtrace/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mirtrace/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13804 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mirtrace/mirtrace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/mosdepth/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mosdepth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24483 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mosdepth/mosdepth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/motus/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/motus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/motus/motus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/mtnucratio/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mtnucratio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/mtnucratio/mtnucratio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.012191 multiqc_sgr-1.22.post0/multiqc/modules/multivcfanalyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/multivcfanalyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12149 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/multivcfanalyzer/multivcfanalyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/nanostat/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nanostat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13570 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nanostat/nanostat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/nextclade/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nextclade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12227 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nextclade/nextclade.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/ngsderive/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ngsderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18186 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/ngsderive/ngsderive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/nonpareil/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nonpareil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/nonpareil/nonpareil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/odgi/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/odgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14726 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/odgi/odgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/optitype/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/optitype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/optitype/optitype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/pangolin/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pangolin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pangolin/pangolin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/pbmarkdup/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pbmarkdup/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5209 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pbmarkdup/pbmarkdup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/peddy/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/peddy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13188 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/peddy/peddy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.016191 multiqc_sgr-1.22.post0/multiqc/modules/phantompeakqualtools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/phantompeakqualtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/phantompeakqualtools/phantompeakqualtools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/picard/
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/AlignmentSummaryMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/BaseDistributionByCycleMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/CrosscheckFingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/ExtractIlluminaBarcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/GcBiasMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20365 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/HsMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/IlluminaBasecallingMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/IlluminaLaneMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/InsertSizeMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/MarkDuplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/MarkIlluminaAdapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/OxoGMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityByCycleMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityScoreDistributionMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityYieldMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/RnaSeqMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/RrbsSummaryMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/TargetedPcrMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14679 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/ValidateSamFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/VariantCallingMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8817 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/WgsMetrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3212 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/picard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/picard/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/porechop/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/porechop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/porechop/porechop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/preseq/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/preseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/preseq/preseq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/prinseqplusplus/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/prinseqplusplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/prinseqplusplus/prinseqplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/profile_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/prokka/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/prokka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/prokka/prokka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/purple/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/purple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/purple/purple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/pychopper/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pychopper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pychopper/pychopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/pycoqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pycoqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/pycoqc/pycoqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/qc3C/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qc3C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44647 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qc3C/qc3C.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.024191 multiqc_sgr-1.22.post0/multiqc/modules/qorts/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qorts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qorts/qorts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.028191 multiqc_sgr-1.22.post0/multiqc/modules/qualimap/
+-rw-r--r--   0 runner    (1001) docker     (127)    29898 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qualimap/QM_BamQC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qualimap/QM_RNASeq.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3611 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qualimap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2243 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/qualimap/qualimap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.028191 multiqc_sgr-1.22.post0/multiqc/modules/quast/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/quast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14715 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/quast/quast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.028191 multiqc_sgr-1.22.post0/multiqc/modules/rna_seqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rna_seqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rna_seqc/rna_seqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.028191 multiqc_sgr-1.22.post0/multiqc/modules/rockhopper/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rockhopper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rockhopper/rockhopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.028191 multiqc_sgr-1.22.post0/multiqc/modules/rsem/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rsem/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7255 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rsem/rsem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.964191 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/assets/js/multiqc_rseqc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/bam_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/gene_body_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/infer_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/inner_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/junction_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/junction_saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_duplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_gc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/rseqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/rseqc/tin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/salmon/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/salmon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5968 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/salmon/salmon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/sambamba/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sambamba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sambamba/markdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sambamba/sambamba.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/samblaster/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samblaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samblaster/samblaster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/samtools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/flagstat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7712 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/idxstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/markdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/rmdup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/samtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/samtools/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/sargasso/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sargasso/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5877 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sargasso/sargasso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.032191 multiqc_sgr-1.22.post0/multiqc/modules/seqera_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqera_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqera_cli/seqera_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/sequali/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sequali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21080 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sequali/sequali.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/seqwho/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqwho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqwho/seqwho.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/seqyclean/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqyclean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/seqyclean/seqyclean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/sexdeterrmine/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sexdeterrmine/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6471 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sexdeterrmine/sexdeterrmine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/sickle/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sickle/sickle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/skewer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/skewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/skewer/skewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/slamdunk/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/slamdunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26181 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/slamdunk/slamdunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/snippy/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snippy/snippy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/snpeff/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snpeff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snpeff/snpeff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/snpsplit/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snpsplit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/snpsplit/snpsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/software_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.036191 multiqc_sgr-1.22.post0/multiqc/modules/somalier/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/somalier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27001 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/somalier/somalier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/sortmerna/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sortmerna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sortmerna/sortmerna.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/sourmash/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sourmash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sourmash/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sourmash/gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/sourmash/sourmash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/spaceranger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/stacks/stacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/star/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       61 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/star/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12592 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/star/star.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/supernova/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/supernova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/supernova/supernova.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/theta2/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/theta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/theta2/theta2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/tophat/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/tophat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6054 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/tophat/tophat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.040191 multiqc_sgr-1.22.post0/multiqc/modules/trimmomatic/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/trimmomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/trimmomatic/trimmomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/truvari/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/truvari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/truvari/bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/truvari/truvari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/umitools/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/umitools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/umitools/umitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/varscan2/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/varscan2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9998 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/varscan2/varscan2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/relatedness2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_by_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_by_qual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vcftools/vcftools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/vep/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vep/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14834 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/vep/vep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/verifybamid/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/verifybamid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/verifybamid/verifybamid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/whatshap/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/whatshap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18744 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/whatshap/whatshap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.044191 multiqc_sgr-1.22.post0/multiqc/modules/xengsort/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/xengsort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/xengsort/xengsort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.048191 multiqc_sgr-1.22.post0/multiqc/modules/xenome/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/xenome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/modules/xenome/xenome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54456 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/multiqc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.048191 multiqc_sgr-1.22.post0/multiqc/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/bargraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/linegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.048191 multiqc_sgr-1.22.post0/multiqc/plots/plotly/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12526 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13042 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28013 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20885 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26012 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/plotly/violin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16871 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/table_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/plots/violin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.052191 multiqc_sgr-1.22.post0/multiqc/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.052191 multiqc_sgr-1.22.post0/multiqc/templates/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.968191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.052191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   120734 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/default_multiqc.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/jquery.toast.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.056191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.056191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     7440 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/MultiQC_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/MultiQC_logo_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/seqera_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/seqera_logo_mono.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.056191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/flat.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/multiqc.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.072191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2446 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/FileSaver.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37045 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86709 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery-3.1.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44365 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery.tablesorter.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery.toast.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    97630 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jszip.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/lz-string.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)  8555428 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3598197 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.076191 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/bar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/box.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/heatmap.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/line.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/scatter.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11481 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/violin.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plotting.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/tables.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44198 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/toolbox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/foot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/general_stats.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/includes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/default/toolbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.076191 multiqc_sgr-1.22.post0/multiqc/templates/gathered/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/gathered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/gathered/content.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/gathered/nav.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.076191 multiqc_sgr-1.22.post0/multiqc/templates/geo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:03.968191 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.076191 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   110058 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.080191 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1543 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/emailme.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47162 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/flames.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8777 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/glyphicons-halflings-white.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13826 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/glyphicons-halflings.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20655 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/hot.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74176 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/mchammer.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18387 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/microfab.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/new.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9959 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/new2.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/progress.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4224 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/rainbow.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10863 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/stars.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/geo/includes.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.080191 multiqc_sgr-1.22.post0/multiqc/templates/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/sections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/sections/content.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.080191 multiqc_sgr-1.22.post0/multiqc/templates/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/foot.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/includes.html
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/nav.html
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/templates/simple/toolbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.084191 multiqc_sgr-1.22.post0/multiqc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18547 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/config_defaults.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15173 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/lzstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/megaqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19363 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/mqc_colour.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/plugin_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22574 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25353 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/search_patterns.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8193 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/software_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/strict_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9309 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/multiqc/utils/util_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 05:36:04.084191 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45070 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20680 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-22 05:36:03.000000 multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 05:36:04.088191 multiqc_sgr-1.22.post0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      143 2024-03-22 05:35:30.000000 multiqc_sgr-1.22.post0/setup.py
```

### Comparing `multiqc_sgr-1.21.0/LICENSE` & `multiqc_sgr-1.22.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/PKG-INFO` & `multiqc_sgr-1.22.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiqc_sgr
-Version: 1.21.0
+Version: 1.22.post0
 Summary: Create aggregate bioinformatics analysis reports across many samples and tools
 Author-email: Phil Ewels <phil.ewels@seqera.io>, Vlad Savelyev <vladislav.savelyev@seqera.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -621,15 +621,19 @@
         reviewing courts shall apply local law that most closely approximates
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
                              END OF TERMS AND CONDITIONS
         
-Project-URL: Repository, https://github.com/zhouyiqi91/MultiQC_SGR
+Project-URL: Homepage, https://multiqc.info
+Project-URL: Repository, https://github.com/MultiQC/MultiQC
+Project-URL: Issues, https://github.com/MultiQC/MultiQC/issues
+Project-URL: Documentation, https://multiqc.info/docs
+Project-URL: Changelog, https://github.com/MultiQC/MultiQC/blob/main/CHANGELOG.md
 Keywords: bioinformatics,biology,sequencing,NGS,next generation sequencing,quality control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -647,15 +651,14 @@
 Requires-Dist: click
 Requires-Dist: coloredlogs
 Requires-Dist: humanize
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: kaleido
 Requires-Dist: markdown
-Requires-Dist: matplotlib>=2.1.1
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: Pillow>=10
 Requires-Dist: plotly>=5.18
 Requires-Dist: pyyaml>=4
 Requires-Dist: pyaml-env
@@ -663,16 +666,16 @@
 Requires-Dist: rich-click
 Requires-Dist: spectra>=0.0.10
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 &nbsp;
-![MultiQC](docs/images/MultiQC_logo.png#gh-light-mode-only)
-![MultiQC](docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo.png#gh-light-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
 &nbsp;
 
 ### Aggregate bioinformatics results across many samples into a single report
 
 ##### Find [documentation](http://multiqc.info/docs) and [example reports](https://multiqc.info/example-reports/) at [http://multiqc.info](http://multiqc.info)
 
 [![PyPI Version](https://img.shields.io/pypi/v/multiqc)](https://pypi.python.org/pypi/multiqc/)
@@ -731,15 +734,15 @@
 ```
 
 That's it! MultiQC will scan the specified directory (`.` is the current dir)
 and produce a report detailing whatever it finds.
 
 <!-- RICH-CODEX fake_command: "multiqc ." -->
 
-![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](docs/images/screenshots/fastqc-run.svg)
+![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](https://github.com/MultiQC/MultiQC/raw/main/docs/images/screenshots/fastqc-run.svg)
 
 The report is created in `multiqc_report.html` by default. Tab-delimited data
 files are also created in `multiqc_data/`, containing extra information.
 These can be easily inspected using Excel (use `--data-format` to get `yaml`
 or `json` instead).
 
 For more detailed instructions, run `multiqc -h` or see the
```

### Comparing `multiqc_sgr-1.21.0/README.md` & `multiqc_sgr-1.22.post0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 &nbsp;
-![MultiQC](docs/images/MultiQC_logo.png#gh-light-mode-only)
-![MultiQC](docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo.png#gh-light-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
 &nbsp;
 
 ### Aggregate bioinformatics results across many samples into a single report
 
 ##### Find [documentation](http://multiqc.info/docs) and [example reports](https://multiqc.info/example-reports/) at [http://multiqc.info](http://multiqc.info)
 
 [![PyPI Version](https://img.shields.io/pypi/v/multiqc)](https://pypi.python.org/pypi/multiqc/)
@@ -63,15 +63,15 @@
 ```
 
 That's it! MultiQC will scan the specified directory (`.` is the current dir)
 and produce a report detailing whatever it finds.
 
 <!-- RICH-CODEX fake_command: "multiqc ." -->
 
-![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](docs/images/screenshots/fastqc-run.svg)
+![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](https://github.com/MultiQC/MultiQC/raw/main/docs/images/screenshots/fastqc-run.svg)
 
 The report is created in `multiqc_report.html` by default. Tab-delimited data
 files are also created in `multiqc_data/`, containing extra information.
 These can be easily inspected using Excel (use `--data-format` to get `yaml`
 or `json` instead).
 
 For more detailed instructions, run `multiqc -h` or see the
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/adapterRemoval/adapterRemoval.py` & `multiqc_sgr-1.22.post0/multiqc/modules/adapterremoval/adapterremoval.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class MultiqcModule(BaseMultiqcModule):
     def __init__(self):
         # Initialise the parent object
         super(MultiqcModule, self).__init__(
             name="Adapter Removal",
-            anchor="adapterRemoval",
+            anchor="adapterremoval",
             target="Adapter Removal",
             href="https://github.com/MikkelSchubert/adapterremoval",
             info=" rapid adapter trimming, identification, and read merging ",
             doi=["10.1186/s13104-016-1900-2", "10.1186/1756-0500-5-337"],
         )
 
         self.__read_type = None
@@ -40,15 +40,15 @@
             "collapsed": dict(),
             "collapsed_truncated": dict(),
             "discarded": dict(),
             "all": dict(),
         }
 
         parsed_data = None
-        for f in self.find_log_files("adapterRemoval", filehandles=True):
+        for f in self.find_log_files("adapterremoval", filehandles=True):
             self.s_name = f["s_name"]
             try:
                 parsed_data = self.parse_settings_file(f)
             except ModuleNoSamplesFound:
                 continue
             if parsed_data is not None:
                 self.adapter_removal_data[self.s_name] = parsed_data
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/afterqc/afterqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/afterqc/afterqc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/anglerfish/anglerfish.py` & `multiqc_sgr-1.22.post0/multiqc/modules/anglerfish/anglerfish.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ MultiQC module to parse output from Anglerfish """
 
 import json
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, beeswarm, table
+from multiqc.plots import bargraph, violin, table
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(BaseMultiqcModule):
     """
@@ -37,21 +37,21 @@
         # Stop execution of the data if no anglerfish data is found.
         if len(self.anglerfish_data) == 0:
             raise ModuleNoSamplesFound
 
         log.info(f"Found {len(self.anglerfish_data)} reports")
 
         # Write parsed report data to a file
-        ## Parse whole JSON to save all its content
+        # Parse whole JSON to save all its content
         self.write_data_file(self.anglerfish_data, "multiqc_anglerfish")
 
         # General Stats Table
         self.anglerfish_general_stats_table()
 
-        # Adds section for Sample Stats Read length table/beeswarm plot
+        # Adds section for Sample Stats Read length table/violin plot
         self.anglerfish_sample_stats()
         # Adds section for Undetermined indexes plot
         self.anglerfish_undetermined_index_chart()
 
     def parse_anglerfish_json(self, f):
         """Parse the JSON output from Anglerfish and save the summary statistics"""
         try:
@@ -104,16 +104,16 @@
             # No undetermined in file or undetermined missing info
             self.anglerfish_data[s_name]["undetermined_amount"] = -1
         self.anglerfish_data[s_name]["total_count"] = total_count
 
     # General stats table
     def anglerfish_general_stats_table(self):
         """Add Anglerfish statistics to the general statistics table"""
-        # Prepp data for general stat table
-        ## Multiple sample names per file requires dict where the first key is not file name
+        # Prep data for general stat table
+        # Multiple sample names per file requires dict where the first key is not file name
         data = {}
         for s_name in self.anglerfish_data:
             total_read = self.anglerfish_data[s_name]["total_read"]
             total_count = self.anglerfish_data[s_name]["total_count"]
             try:
                 for k in range(self.anglerfish_data[s_name]["sample_stats_amount"]):
                     key = self.anglerfish_data[s_name][f"sample_name_{k}"]
@@ -164,16 +164,16 @@
             },
         }
 
         self.general_stats_addcols(data, headers)
 
     def anglerfish_sample_stats(self):
         """Generate plot for read length from sample stats.
-        For >10 samples: generate table plot
-        for >= 10 samples: generate beeswarm plot"""
+        For < 10 samples: generate a table
+        for >= 10 samples: generate a violin plot"""
         data = {}
         total_samples = 0
         for s_name in self.anglerfish_data:
             index = self.anglerfish_data[s_name]["sample_stats_amount"]
             if index > 0:
                 total_samples += index
                 for i in range(index):
@@ -189,19 +189,19 @@
         if len(data) == 0:
             return
 
         config = {
             "id": "Sample_Stat_Read_Length",
             "title": "Anglerfish: Read Lengths Summary",
         }
-        # Plot table if less than 10 samples exist, beeswarm if more
+        # Plot table if less than 10 samples exist, a violin if more
         if total_samples < 10:
             p = table.plot(data, None, config)
         else:
-            p = beeswarm.plot(data, None, config)
+            p = violin.plot(data, None, config)
         self.add_section(
             name="Read Lengths Summary",
             anchor="anglerfish-sample-statistics",
             description="The Mean read length and the Standard Deviation for each sample.",
             plot=p,
         )
 
@@ -222,18 +222,17 @@
                 # For non existing undetermined and faulty undetermined
                 log.debug(f"Missing Undetermined Data in Anglerfish json: {s_name}")
         # Only add undetermined section if undetermined data exists
         if len(data) == 0:
             return
 
         config = {
-            "id": "Anglerfish_undetermined_index_plot",
+            "id": "anglerfish_undetermined_index_plot",
             "cpswitch": False,
             "title": "Anglerfish: Undetermined Indexes",
             "ylab": "Index Count",
-            "tt_percentages": False,
         }
         self.add_section(
             name="Undetermined Indexes",
             anchor="anglerfish-undetermined-indexes",
             plot=bargraph.plot(data, None, config),
         )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bakta/bakta.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bakta/bakta.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bamdst/bamdst.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bamdst/bamdst.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bamtools/bamtools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bamtools/bamtools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bamtools/stats.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bamtools/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ MultiQC submodule to parse output from Bamtools bam_stat.py
 http://bamtools.sourceforge.net/#bam-stat-py """
 
 import logging
 import re
 
-from multiqc.plots import beeswarm
+from multiqc.plots import violin
 from multiqc.utils import config
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 def parse_reports(self):
@@ -90,22 +90,22 @@
         self.general_stats_data[s_name].update(self.bamtools_stats_data[s_name])
 
     # Make dot plot of counts
     keys = {}
     defaults = {
         "min": 0,
         "max": 100,
-        "decimalPlaces": 2,
+        "tt_decimals": 2,
         "suffix": "%",
     }
     num_defaults = {
         "min": 0,
         "modify": lambda x: x * config.read_count_multiplier,
         "suffix": config.read_count_prefix,
-        "decimalPlaces": 2,
+        "tt_decimals": 2,
     }
 
     keys["total_reads"] = dict(num_defaults, **{"title": "Total reads", "description": "Total reads (millions)"})
     keys["mapped_reads_pct"] = dict(defaults, **{"title": "Mapped reads"})
     keys["forward_strand_pct"] = dict(defaults, **{"title": "Forward strand"})
     keys["reverse_strand_pct"] = dict(defaults, **{"title": "Reverse strand"})
     keys["failed_qc_pct"] = dict(defaults, **{"title": "Failed QC"})
@@ -116,15 +116,15 @@
     keys["bt_read_1"] = dict(num_defaults, **{"title": "Read 1", "description": "Read 1 (millions)"})
     keys["bt_read_2"] = dict(num_defaults, **{"title": "Read 2", "description": "Read 2 (millions)"})
     keys["singletons_pct"] = dict(defaults, **{"title": "Singletons"})
 
     self.add_section(
         name="Bamtools Stats",
         anchor="bamtools-stats",
-        plot=beeswarm.plot(
+        plot=violin.plot(
             self.bamtools_stats_data,
             keys,
             pconfig={
                 "id": "bamtools-stats-plot",
                 "title": "Bamtools Stats",
             },
         ),
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/base_module.py` & `multiqc_sgr-1.22.post0/multiqc/modules/base_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ MultiQC modules base class, contains helper functions """
-from typing import List, Union, Optional
+
+from typing import List, Union, Optional, Dict
 
 import fnmatch
 import io
 import itertools
 import logging
 import mimetypes
 import os
@@ -18,44 +19,46 @@
 logger = logging.getLogger(__name__)
 
 
 class ModuleNoSamplesFound(Exception):
     """Module checked all input files but couldn't find any data to use"""
 
 
-class BaseMultiqcModule(object):
+class BaseMultiqcModule:
+    # Custom options from user config that can overwrite base module values
+    mod_cust_config: Dict = {}
+
     def __init__(
         self,
         name="base",
         anchor="base",
         target=None,
         href=None,
         info=None,
         comment=None,
         extra=None,
         autoformat=True,
         autoformat_type="markdown",
-        doi=None,
+        doi: Optional[str] = None,
     ):
         # Custom options from user config that can overwrite base module values
-        mod_cust_config = getattr(self, "mod_cust_config", {})
-        self.name = mod_cust_config.get("name", name)
-        self.anchor = mod_cust_config.get("anchor", anchor)
-        target = mod_cust_config.get("target", target)
-        self.href = mod_cust_config.get("href", href)
-        self.info = mod_cust_config.get("info", info)
-        self.comment = mod_cust_config.get("comment", comment)
-        self.extra = mod_cust_config.get("extra", extra)
-        self.doi = mod_cust_config.get("doi", (doi or []))
+        self.name = self.mod_cust_config.get("name", name)
+        self.anchor = self.mod_cust_config.get("anchor", anchor)
+        target = self.mod_cust_config.get("target", target)
+        self.href = self.mod_cust_config.get("href", href)
+        self.info = self.mod_cust_config.get("info", info)
+        self.comment = self.mod_cust_config.get("comment", comment)
+        self.extra = self.mod_cust_config.get("extra", extra)
+        self.doi = self.mod_cust_config.get("doi", (doi or []))
 
         # List of software version(s) for module. Don't append directly, use add_software_version()
         self.versions = defaultdict(list)
 
         # Specific module level config to overwrite (e.g. config.bcftools, config.fastqc)
-        config.update({anchor: mod_cust_config.get("custom_config", {})})
+        config.update({anchor: self.mod_cust_config.get("custom_config", {})})
 
         # Sanitise anchor ID and check for duplicates
         self.anchor = report.save_htmlid(self.anchor)
 
         # See if we have a user comment in the config
         if self.anchor in config.section_comments:
             self.comment = config.section_comments[self.anchor]
@@ -106,23 +109,22 @@
         :param sp_key: Search pattern key specified in config
         :param filehandles: Set to true to return a file handle instead of slurped file contents
         :return: Yields a dict with filename (fn), root directory (root), cleaned sample name
                  generated from the filename (s_name) and either the file contents or file handle
                  for the current matched file (f).
                  As yield is used, the results can be iterated over without loading all files at once
         """
-
         # Pick up path filters if specified.
         # Allows modules to be called multiple times with different sets of files
-        path_filters = getattr(self, "mod_cust_config", {}).get("path_filters")
-        path_filters_exclude = getattr(self, "mod_cust_config", {}).get("path_filters_exclude")
+        path_filters: Union[str, List[str]] = self.mod_cust_config.get("path_filters", [])
+        path_filters_exclude: Union[str, List[str]] = self.mod_cust_config.get("path_filters_exclude", [])
         if isinstance(path_filters, str):
-            path_filters = [path_filters]
+            path_filters: List[str] = [path_filters]
         if isinstance(path_filters_exclude, str):
-            path_filters_exclude = [path_filters_exclude]
+            path_filters_exclude: List[str] = [path_filters_exclude]
 
         # Old, depreciated syntax support. Likely to be removed in a future version.
         if isinstance(sp_key, dict):
             report.files[self.name] = list()
             for sf in report.searchfiles:
                 if report.search_file(sp_key, {"fn": sf[0], "root": sf[1]}, module_key=None):
                     report.files[self.name].append({"fn": sf[0], "root": sf[1]})
@@ -241,17 +243,16 @@
                 nid = name.lower().strip().replace(" ", "-")
                 anchor = f"{self.anchor}-{nid}"
             else:
                 sl = len(self.sections) + 1
                 anchor = f"{self.anchor}-section-{sl}"
 
         # Append custom module anchor to the section if set
-        mod_cust_config = getattr(self, "mod_cust_config", {})
-        if "anchor" in mod_cust_config:
-            anchor = f"{mod_cust_config['anchor']}_{anchor}"
+        if "anchor" in self.mod_cust_config:
+            anchor = f"{self.mod_cust_config['anchor']}_{anchor}"
 
         # Sanitise anchor ID and check for duplicates
         anchor = report.save_htmlid(anchor)
 
         # Skip if user has a config to remove this module section
         if anchor in config.remove_sections:
             logger.debug(f"Skipping section '{anchor}' because specified in user config")
@@ -594,17 +595,16 @@
         report.software_versions[group_name][software_name] = self.versions[software_name]
 
     def write_data_file(self, data, fn, sort_cols=False, data_format=None):
         """Saves raw data to a dictionary for downstream use, then redirects
         to report.write_data_file() to create the file in the report directory"""
 
         # Append custom module anchor if set
-        mod_cust_config = getattr(self, "mod_cust_config", {})
-        if "anchor" in mod_cust_config:
-            fn = f"{fn}_{mod_cust_config['anchor']}"
+        if "anchor" in self.mod_cust_config:
+            fn = f"{fn}_{self.mod_cust_config['anchor']}"
 
         # Generate a unique filename if the file already exists (running module multiple times)
         i = 1
         base_fn = fn
         while fn in report.saved_raw_data:
             fn = f"{base_fn}_{i}"
             i += 1
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbduk/bbduk.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbduk/bbduk.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             },
         }
 
         self.general_stats_addcols(self.bbduk_data, headers)
 
     def bbduk_bargraph_plot(self):
         """
-        Beeswarm displaying all possible filtering results reported by BBDuk.
+        Violin displaying all possible filtering results reported by BBDuk.
 
         We don't display this as a barchart as the total across all categories
         of filters reported don't match exactly the total reads remaining (I
         assume there is additional default filtering carried out)
         """
         cats = [
             "Result",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/bbmap.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/bbmap.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/bbmap_filetypes.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/bbmap_filetypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,21 @@
             "Mean": ("Average GC content", {}),
             "Median": ("Median GC content", {}),
             "Mode": ("The most commonly occuring value of the GC content distribution", {}),
             "STDev": ("Standard deviation of average GC content", {}),
         },
         "cols": {"GC": float, "Count": int},
         "plot_func": plot_basic_hist,
-        "plot_params": {"xlab": "Proportion GC", "ylab": "# Reads"},
+        "plot_params": {
+            "xlab": "Proportion GC",
+            "ylab": "# Reads",
+            "xsuffix": "%",
+            "xmin": 0,
+            "xmax": 100,
+        },
     },
     "idhist": {
         "title": "Identity histogram",
         "descr": "Histogram of read count versus percent base pair identity " "of aligned reads (`idhist`).",
         "help_text": "",
         "kvrows": [
             "Mean_reads",
@@ -278,15 +284,15 @@
     },
     "lhist": {
         "title": "Read lengths",
         "descr": "Read length histogram (`lhist`).",
         "help_text": "",
         "cols": {"Length": int, "Count": int},
         "plot_func": plot_basic_hist,
-        "plot_params": {"xlab": "Read length (base pairs)", "ylab": "# Reads"},
+        "plot_params": {"xlab": "Read length (base pairs)", "xsuffix": "bp", "ylab": "# Reads"},
     },
     "mhist": {
         "title": "Match, substitution, deletion, and insertion rates",
         "descr": "Histogram of match, substitution, deleletion, " "and insertion rates by read location (`mhist`).",
         "help_text": "",
         "cols": {
             "BaseNum": int,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_aqhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_aqhist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_basic_hist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_basic_hist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_bhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_bhist.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             }
         )
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
         "xlab": "Read position",
+        "xsuffix": " bp",
         "ylab": "Percentage of G+C bases",
         "ymin": 0,
         "ymax": 100,
         "data_labels": [
             {"name": "Percentage of G+C bases"},
             {"name": "Percentage of A+T bases"},
             {"name": "Percentage of N bases"},
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_bqhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_bqhist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_covhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_covhist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_idhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_idhist.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             }
         )
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
         "xlab": "Percent identity",
+        "xsuffix": "%",
         "ylab": "Read count",
         "data_labels": [
             {"name": "Reads", "ylab": "Read count"},
             {"name": "Bases", "ylab": "Number of bases"},
         ],
     }
     plot_params.update(plot_args["plot_params"])
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_ihist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_ihist.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,14 @@
     }
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
         "xmax": xmax,
         "xlab": "Insert size (base pairs)",
+        "xsuffix": " bp",
         "ylab": "Read count",
     }
     plot_params.update(plot_args["plot_params"])
     plot = linegraph.plot(data, plot_params)
 
     return plot
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_indelhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_indelhist.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             }
         )
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
         "xlab": "Indel size",
+        "xsuffix": " bp",
         "ylab": "Insertion count",
         "data_labels": [
             {"name": "Insertions", "ylab": "Insertion count"},
             {"name": "Deletions", "ylab": "Deletion count"},
         ],
     }
     plot_params.update(plot_args["plot_params"])
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_mhist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_mhist.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             }
         )
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
         "xlab": "Location in read",
+        "xsuffix": " bp",
         "ylab": "Proportion",
         "data_labels": [
             {"name": "Read 1", "ylab": "Proportion"},
             {"name": "Read 2", "ylab": "Proportion"},
         ],
     }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_qahist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_qhist.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,36 @@
 from itertools import chain
 
 from multiqc.plots import linegraph
 
 
-def plot_qahist(samples, file_type, **plot_args):
-    """Create line graph plot of histogram data for BBMap 'qahist' output.
+def plot_qhist(samples, file_type, **plot_args):
+    """Create line graph plot of histogram data for BBMap 'qhist' output.
 
     The 'samples' parameter could be from the bbmap mod_data dictionary:
     samples = bbmap.MultiqcModule.mod_data[file_type]
     """
 
+    sumy = sum([int(samples[sample]["data"][x][0]) for sample in samples for x in samples[sample]["data"]])
+
+    cutoff = sumy * 0.999
     all_x = set()
     for item in sorted(chain(*[samples[sample]["data"].items() for sample in samples])):
-        # Skip plotting values for this x if missing columns.
-        if len(item[1]) < 6:
-            continue
         all_x.add(item[0])
+        cutoff -= item[1][0]
+        if cutoff < 0:
+            xmax = item[0]
+            break
+    else:
+        xmax = max(all_x)
 
     columns_to_plot = {
-        "Match": {
-            0: "Match",
-        },
-        "Sub": {
-            1: "Sub",
-        },
-        "Ins": {
-            2: "Ins",
-        },
-        "Del": {
-            3: "Del",
-        },
-        "TrueQuality": {
-            4: "TrueQuality",
-        },
-        "TrueQualitySub": {
-            5: "TrueQualitySub",
-        },
+        "Linear": {0: "Read1", 3: "Read2"},
+        "Logarithmic": {1: "Read1", 4: "Read2"},
+        "Measured": {2: "Read1", 5: "Read2"},
     }
 
     plot_data = []
     for column_type in columns_to_plot:
         plot_data.append(
             {
                 sample + "." + column_name: {
@@ -49,23 +40,22 @@
                 for column, column_name in columns_to_plot[column_type].items()
             }
         )
 
     plot_params = {
         "id": "bbmap-" + file_type + "_plot",
         "title": "BBTools: " + plot_args["plot_title"],
-        "xlab": "Quality score",
-        "ylab": "Match count",
+        "xmax": xmax,
+        "xlab": "Position in read",
+        "xsuffix": " bp",
+        "ylab": "Quality score",
         "data_labels": [
-            {"name": "Match", "ylab": "Match count"},
-            {"name": "Substitution", "ylab": "Substitution count"},
-            {"name": "Insertion", "ylab": "Insertion count"},
-            {"name": "Deletion", "ylab": "Deletion count"},
-            {"name": "TrueQuality", "ylab": "Count"},
-            {"name": "TrueQualitySubtitution", "ylab": "Count"},
+            {"name": "Linear", "ylab": "Quality score"},
+            {"name": "Logarithmic", "ylab": "Log score"},
+            {"name": "Measured", "ylab": "Measured quality value"},
         ],
     }
 
     plot_params.update(plot_args["plot_params"])
     plot = linegraph.plot(plot_data, plot_params)
 
     return plot
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bbmap/plot_qchist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bbmap/plot_qchist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bcftools/bcftools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bcftools/bcftools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bcftools/stats.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bcftools/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,19 +190,22 @@
                     bin_name = s[2].strip()
                     percent_sites = float(s[-1].strip())
                     self.bcftools_stats_depth_data[s_name][bin_name] = percent_sites
 
                 # Variant Qualities
                 if s[0] == "QUAL" and len(s_names) > 0:
                     s_name = s_names[int(s[1])]
-                    quality = float("0" + s[2].strip())
-                    self.bcftools_stats_vqc_snp[s_name][quality] = float(s[3].strip())
-                    self.bcftools_stats_vqc_transi[s_name][quality] = float(s[4].strip())
-                    self.bcftools_stats_vqc_transv[s_name][quality] = float(s[5].strip())
-                    self.bcftools_stats_vqc_indels[s_name][quality] = float(s[6].strip())
+                    try:
+                        quality = float(s[2].strip())
+                    except ValueError:
+                        quality = 0
+                    self.bcftools_stats_vqc_snp[s_name][quality] = int(s[3].strip())
+                    self.bcftools_stats_vqc_transi[s_name][quality] = int(s[4].strip())
+                    self.bcftools_stats_vqc_transv[s_name][quality] = int(s[5].strip())
+                    self.bcftools_stats_vqc_indels[s_name][quality] = int(s[6].strip())
 
         # Remove empty samples
         self.bcftools_stats = {k: v for k, v in self.bcftools_stats.items() if len(v) > 0}
         self.bcftools_stats_indels = {k: v for k, v in self.bcftools_stats_indels.items() if len(v) > 0}
         self.bcftools_stats_sample_variants = {
             k: v for k, v in self.bcftools_stats_sample_variants.items() if len(v) > 0
         }
@@ -272,17 +275,17 @@
         # Make histograms of variant quality
         if len(self.bcftools_stats_vqc_snp) > 0:
             pconfig = {
                 "id": "bcftools_stats_vqc",
                 "title": "Bcftools Stats: Variant Quality Count",
                 "ylab": "Count",
                 "xlab": "Quality",
-                "xDecimals": False,
                 "ymin": 0,
                 "smooth_points": 600,
+                "x_decimals": 0,
                 "data_labels": [
                     "Count SNP",
                     "Count Transitions",
                     "Count Transversions",
                     "Count Indels",
                 ],
             }
@@ -303,15 +306,15 @@
         # Make line graph of indel lengths
         if len(self.bcftools_stats_indels) > 0:
             pconfig = {
                 "id": "bcftools_stats_indel-lengths",
                 "title": "Bcftools Stats: Indel Distribution",
                 "ylab": "Count",
                 "xlab": "InDel Length (bp)",
-                "xDecimals": False,
+                "xsuffix": " bp",
                 "ymin": 0,
             }
             self.add_section(
                 name="Indel Distribution",
                 anchor="bcftools-stats_indel_plot",
                 plot=linegraph.plot(self.bcftools_stats_indels, pconfig),
             )
@@ -328,14 +331,15 @@
                 for sname in self.bcftools_stats_depth_data
             }
             pconfig = {
                 "id": "bcftools_stats_variant_depths",
                 "title": "Bcftools Stats: Variant depths",
                 "ylab": "Fraction of sites (%)",
                 "xlab": "Variant depth",
+                "ysuffix": "%",
                 "ymin": 0,
                 "ymax": 100,
                 "categories": True,
                 "tt_decimals": 1,
             }
             self.add_section(
                 name="Variant depths",
@@ -397,14 +401,15 @@
 
         # Make bargraph plot of sequencing depth stats
         if len(self.bcftools_stats_sample_depth) > 0:
             pconfig = {
                 "id": "bcftools-stats-sequencing-depth",
                 "title": "Bcftools Stats: Sequencing depth",
                 "ylab": "Sequencing depth",
+                "ysuffix": "X",
                 "cpswitch_counts_label": "Sequencing depth",
                 "cpswitch": False,
                 "data_labels": list(self.bcftools_stats_sample_depth),
             }
             self.add_section(
                 name="Sequencing depth",
                 anchor="bcftools-stats_sequencing_depth",
@@ -457,9 +462,23 @@
             "number_of_MNPs": {
                 "title": "MNP",
                 "description": "Variation multinucleotide polymorphisms",
                 "min": 0,
                 "format": "{:,.0f}",
                 "hidden": True,
             },
+            "number_of_multiallelic_sites": {
+                "title": "Multiallelic",
+                "description": "Variation sites with multiple alleles",
+                "min": 0,
+                "format": "{:,.0f}",
+                "hidden": True,
+            },
+            "number_of_multiallelic_SNP_sites": {
+                "title": "Multiallelic SNP",
+                "description": "Variation sites with multiple SNPs",
+                "min": 0,
+                "format": "{:,.0f}",
+                "hidden": True,
+            },
         }
         return stats_headers
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bcl2fastq/bcl2fastq.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bcl2fastq/bcl2fastq.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,14 @@
             plot=bargraph.plot(
                 self.get_bar_data_from_undetermined(self.bcl2fastq_bylane),
                 None,
                 {
                     "id": "bcl2fastq_undetermined",
                     "title": "bcl2fastq: Undetermined barcodes by lane",
                     "ylab": "Reads",
-                    "tt_percentages": False,
                     "use_legend": True,
                     "sort_samples": False,  # keep top barcode on top
                 },
             ),
         )
 
     def parse_file_as_json(self, f):
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bclconvert/bclconvert.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bclconvert/bclconvert.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
         # Set up and collate bclconvert run and demux files
         demuxes, qmetrics, multiple_sequencing_runs, last_run_id = self._collate_log_files()
 
         # variables to store reads for undetermined read recalculation
         self.per_lane_undetermined_reads = dict()
         self.total_reads_in_lane_per_file = dict()
+
         bclconvert_data = dict()
         for demux in demuxes.values():
             self.parse_demux_data(demux, bclconvert_data, len(demuxes))
         for qmetric in qmetrics.values():
             self.parse_qmetrics_data(bclconvert_data, qmetric)
 
         if len(demuxes) == 0:
@@ -68,36 +69,26 @@
             self._parse_top_unknown_barcodes(bclconvert_data, last_run_id)
 
         # Collect counts by lane and sample
         (
             bclconvert_by_lane,
             bclconvert_by_sample,
             counts_by_sample_by_lane,
-            source_files,
         ) = self._split_data_by_lane_and_sample(bclconvert_data)
 
         # Filter to strip out ignored sample names
         bclconvert_by_lane = self.ignore_samples(bclconvert_by_lane)
         bclconvert_by_sample = self.ignore_samples(bclconvert_by_sample)
         counts_by_sample_by_lane = self.ignore_samples(counts_by_sample_by_lane)
 
         # Return with Warning if no files are found
         if len(bclconvert_by_lane) == 0 and len(bclconvert_by_sample) == 0:
             raise ModuleNoSamplesFound
         log.info(f"{len(bclconvert_by_lane)} lanes and {len(bclconvert_by_sample)} samples found")
 
-        # Print source files
-        for s in source_files.keys():
-            self.add_data_source(
-                s_name=s,
-                source=",".join(list(set(source_files[s]))),
-                module="bclconvert",
-                section="bclconvert-bysample",
-            )
-
         # Calculate mean quality scores
         for sample_id, sample in bclconvert_by_sample.items():
             if sample["yield"] > 0:
                 sample["mean_quality"] = sample["_quality_score_sum"] / sample["yield"]
             del sample["_quality_score_sum"]
 
         for lane_id, lane in bclconvert_by_lane.items():
@@ -198,15 +189,14 @@
                 plot=bargraph.plot(
                     self.get_bar_data_from_undetermined(bclconvert_by_lane),
                     None,
                     {
                         "id": "bclconvert_undetermined",
                         "title": "bclconvert: Undetermined barcodes by lane",
                         "ylab": "Count",
-                        "tt_percentages": False,
                         "use_legend": True,
                         "tt_suffix": "reads",
                     },
                 ),
             )
 
     @staticmethod
@@ -262,24 +252,33 @@
             if element.get("Number") == "4" and element.get("IsIndexedRead") == "N":
                 return element.get("NumCycles")
 
         log.error("Could not figure out read 2 length from RunInfo.xml")
         raise ModuleNoSamplesFound
 
     def _parse_single_runinfo_file(self, runinfo_file):
-        # Get run id and cluster length from RunInfo.xml
+        """
+        Get run id and cluster length from RunInfo.xml
+        """
         try:
             root = ET.fromstring(runinfo_file["f"])
             run_id = root.find("Run").get("Id")
             read_length_r1 = root.find("./Run/Reads/Read[1]").get(
                 "NumCycles"
             )  # ET indexes first element at 1, so here we're getting the first NumCycles
         except:  # noqa: E722
             log.error(f"Could not parse RunInfo.xml to get RunID and read length in '{runinfo_file['root']}'")
             raise ModuleNoSamplesFound
+
+        self.add_data_source(
+            runinfo_file,
+            module="bclconvert",
+            section="bclconvert-runinfo-xml",
+        )
+
         if self._is_single_end_reads(root):
             cluster_length = int(read_length_r1)
         else:
             read_length_r2 = self._get_r2_length(root)
             cluster_length = int(read_length_r1) + int(read_length_r2)
         return {"run_id": run_id, "cluster_length": cluster_length}
 
@@ -364,19 +363,25 @@
                 lane = run_data.get(lane_id)
                 if lane is None:
                     lane = dict(samples={}, cluster_length=demux_file["cluster_length"], **self._reads_dictionary())
                     run_data[lane_id] = lane
                     self.per_lane_undetermined_reads[lane_id] = 0
 
                 sname = row["SampleID"]
+                self.add_data_source(
+                    demux_file,
+                    s_name=sname,
+                    module="bclconvert",
+                    section="bclconvert-runinfo-demux-csv",
+                )
                 if sname != "Undetermined":
                     # Don't include undetermined reads at all in any of the calculations...
                     if sname not in lane["samples"]:
                         lane["samples"][sname] = self._reads_dictionary()
-                        lane["samples"][sname]["filename"] = os.path.join(demux_file["root"], demux_file["fn"])
+                        lane["samples"][sname]["filename"] = filename
                         lane["samples"][sname]["samples"] = {}
 
                     sample = lane["samples"][sname]  # this sample in this lane
 
                     # total lane stats
                     lane["clusters"] += int(row["# Reads"])
                     lane["_calculated_yield"] += int(row["# Reads"]) * demux_file["cluster_length"]
@@ -428,14 +433,20 @@
             run_data = bclconvert_data[qmetrics_file["run_id"]]
             lane_id = f"L{row['Lane']}"
             if lane_id not in run_data:
                 log.warning(f"Found unrecognised lane {lane_id} in Quality Metrics file, skipping")
                 continue
             lane = run_data[lane_id]
             sample = row["SampleID"]
+            self.add_data_source(
+                qmetrics_file,
+                s_name=sample,
+                module="bclconvert",
+                section="bclconvert-runinfo-quality-metrics-csv",
+            )
             if sample != "Undetermined":  # don't include undetermined reads at all in any of the calculations...
                 if sample not in run_data[lane_id]["samples"]:
                     log.warning(f"Found unrecognised sample {sample} in Quality Metrics file, skipping")
                     continue
                 lane_sample = run_data[lane_id]["samples"][sample]  # this sample in this lane
 
                 # Parse the stats that moved to this file in v3.9.3
@@ -488,22 +499,21 @@
         except ZeroDivisionError:
             data["percent_oneMismatch"] = "NA"
         if self._get_genome_size():
             data["depth"] = float(data["basesQ30"]) / self._get_genome_size()
         else:
             data["depth"] = "NA"
 
-    def _split_data_by_lane_and_sample(self, bclconvert_data) -> Tuple[Dict, Dict, Dict, Dict]:
+    def _split_data_by_lane_and_sample(self, bclconvert_data) -> Tuple[Dict, Dict, Dict]:
         """
         Populate a collection of "stats across all lanes" and "stats across all samples"
         """
         bclconvert_by_lane = dict()
         bclconvert_by_sample = dict()
         count_by_sample_by_lane = defaultdict(lambda: defaultdict(int))  # counts only - used for a stacked bargraph
-        source_files = dict()
         for run_id, r in bclconvert_data.items():
             # set stats for each lane (across all samples) in bclconvert_bylane dictionary
             for lane_id, lane in r.items():
                 self._set_lane_percentage_stats(lane, lane["cluster_length"])
 
                 lane_key_name = self.prepend_runid(run_id, lane_id)
                 bclconvert_by_lane[lane_key_name] = {
@@ -541,22 +551,17 @@
                         pass
 
                     if not self._get_genome_size():
                         s["depth"] = "NA"
                     else:
                         s["depth"] += float(sample["basesQ30"]) / self._get_genome_size()
 
-                    if sample_id not in ["top_unknown_barcodes"]:
-                        if sample_id not in source_files:
-                            source_files[sample_id] = []
-                        source_files[sample_id].append(sample["filename"])
-
                     count_by_sample_by_lane[sample_id][lane_key_name] += sample["clusters"]
 
-        return bclconvert_by_lane, bclconvert_by_sample, count_by_sample_by_lane, source_files
+        return bclconvert_by_lane, bclconvert_by_sample, count_by_sample_by_lane
 
     def sample_stats_table(self, bclconvert_data, bclconvert_by_sample):
         sample_stats_data = dict()
         total_reads = self._total_reads_all_runs(bclconvert_data)
         depth_available = False
 
         for sample_id, sample in bclconvert_by_sample.items():
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/biobambam2/biobambam2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/biobambam2/biobambam2.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/biobloomtools/biobloomtools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/biobloomtools/biobloomtools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/biscuit/biscuit.py` & `multiqc_sgr-1.22.post0/multiqc/modules/biscuit/biscuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ MultiQC module to parse output from BISCUITqc """
 
 
 import logging
 import re
 
-from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, linegraph, beeswarm
+from multiqc.plots import bargraph, linegraph, violin
 
 # Initialize the logger
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(BaseMultiqcModule):
     """
@@ -299,18 +298,18 @@
                 pd_mapq[s_name] = dd["mapqs"]
 
         pconfig = {
             "id": "biscuit_mapq",
             "title": "BISCUIT: Distribution of Mapping Qualities",
             "ymin": 0,
             "xmin": 0,
-            "yLabelFormat": "{value}%",
             "tt_label": "<strong>Q{point.x}:</strong> {point.y:.2f}% of mapped reads",
-            "ylab": "% of Primary Mapped Reads",
-            "xlab": "Mapping Quality Score",
+            "ysuffix": "%",
+            "ylab": "% of primary mapped reads",
+            "xlab": "Mapping quality score",
         }
 
         self.add_section(
             name="Mapping Quality Distribution",
             anchor="biscuit-mapq",
             description="""
                 The percentage of the total number of mapped reads
@@ -450,31 +449,35 @@
         """
 
         pd_p = {}
         pd_r = {}
         for s_name, dd in self.mdata["align_isize"].items():
             if "no_data_available" not in dd.keys():
                 pd_p[s_name] = dd["percent"]
-                pd_r[s_name] = {ins: cnt * config.read_count_multiplier for ins, cnt in dd["readcnt"].items()}
+                pd_r[s_name] = dd["readcnt"]
 
         pconfig = {
             "id": "biscuit_isize",
             "title": "BISCUIT: Insert Size Distribution",
             "ymin": 0,
             "xmin": 0,
-            "yLabelFormat": "{value}",
             "smooth_points": 1000,  # limit number of points / smooth data
-            "tt_label": "<strong>IS{point.x}:</strong> {point.y:.2f}",
             "xlab": "Insert Size",
-            "ylab": "% of Mapped Reads",
             "data_labels": [
-                {"name": "Percent of Reads", "ylab": "% of Mapped Reads"},
                 {
-                    "name": f"{config.read_count_desc.capitalize()} of Reads",
-                    "ylab": f"{config.read_count_desc.capitalize()} of Mapped Reads",
+                    "name": "% of Mapped Reads",
+                    "ylab": "% of Mapped Reads",
+                    "ysuffix": "%",
+                    "tt_label": "<strong>IS%{x} bp:</strong> %{y:.2f}%",
+                },
+                {
+                    "name": "Mapped Reads",
+                    "ylab": "Mapped Reads",
+                    "ysuffix": "",
+                    "tt_label": "<strong>IS%{x} bp:</strong> %{y:,.0f}",
                 },
             ],
         }
 
         self.add_section(
             name="Insert Size Distribution",
             anchor="biscuit-isize",
@@ -543,31 +546,30 @@
         }
         pconfig = {
             "id": "biscuit_dup_report",
             "cpswitch": False,
             "cpswitch_c_active": False,
             "title": "BISCUIT: Percentage of Duplicate Reads",
             "data_labels": [{"name": "Overall Duplicate Rate"}, {"name": "MAPQ>=40 Duplicate Rate"}],
-            "ylab": "Duplicate Rate [%]",
+            "ylab": "Duplicate rate",
             "ymin": 0,
             "ymax": 100,
-            "yCeiling": 110,
+            "y_clipmax": 110,
             "use_legend": False,
             "tt_decimals": 1,
             "tt_suffix": "%",
-            "tt_percentages": False,
         }
 
         if len(pd1) > 0:
             self.add_section(
                 name="Duplicate Rates",
                 anchor="biscuit-dup-report",
                 description="Shows the percentage of total reads that are duplicates.",
                 helptext="""
-                    `MAPQ >= 40` shows the duplicate rate for just the reads reads
+                    `MAPQ >= 40` shows the duplicate rate for just the reads
                     with a mapping quality score of `MAPQ >= 40`.
                 """,
                 plot=bargraph.plot([pd1, pd2], [pheader, pheader], pconfig),
             )
 
     ########################################
     ####      Depths and Uniformity     ####
@@ -638,16 +640,16 @@
                 if cat in dd:
                     if dd[cat]["mu"] != -1:
                         data["mu_" + key] = dd[cat]["mu"]
                         data["cv_" + key] = dd[cat]["cv"]
             if len(data) > 0:
                 pd[s_name] = data
 
-        shared_mean = {"min": 0, "format": "{:,3f}", "minRange": 10}
-        shared_cofv = {"min": 0, "format": "{:,3f}", "minRange": 50}
+        shared_mean = {"min": 0, "format": "{:,3f}", "minrange": 10}
+        shared_cofv = {"min": 0, "format": "{:,3f}", "minrange": 50}
 
         pheader = {
             "mu_a_b": dict(
                 shared_mean, **{"title": "All Genome Mean", "description": "Mean Sequencing Depth for All Reads"}
             ),
             "mu_q_b": dict(
                 shared_mean, **{"title": "Q40 Genome Mean", "description": "Mean Sequencing Depth for Q40 Reads"}
@@ -782,15 +784,15 @@
                     "description": "Sequencing Depth CoV for Q40 CpGs in High GC-Content Regions",
                 },
             ),
         }
         pconfig = {
             "id": "biscuit_seq_depth",
             "table_title": "BISCUIT: Sequencing Depth",
-            "sortRows": False,
+            "sort_rows": False,
         }
 
         if len(pd) > 0:
             self.add_section(
                 name="Sequencing Depth Statistics",
                 anchor="biscuit-seq-depth",
                 description="""
@@ -804,15 +806,15 @@
                     * _CpGs_ - Statistics for CpGs
                     * _All_ - Statistics for any mapped bases/CpGs
                     * _Q40_ - Statistics only those bases/CpGs with mapping quality `MAPQ >= 40`
                     * _High GC_ - Bases / CpGs that overlap with the top 10% of 100bp windows for GC-content
                     * _Low GC_ - Bases / CpGs that overlap with the bottom 10% of 100bp windows for GC-content
 
                 """,
-                plot=beeswarm.plot(pd, pheader, pconfig),
+                plot=violin.plot(pd, pheader, pconfig),
             )
 
     ########################################
     #### Base Coverage and CpG Coverage ####
     ########################################
     @staticmethod
     def parse_logs_covdist_all_base(f, fn):
@@ -1102,19 +1104,20 @@
             ),
         ]
 
         pconfig = {
             "id": "biscuit_retention_cytosine",
             "title": "BISCUIT: Retention vs. Base Position in Read",
             "xlab": "Position in Read",
+            "xsuffix": "bp",
             "ylab": "CpG Retention Rate (%)",
             "ymin": 0,
             "ymax": 100,
-            "yMinRange": 0,
-            "yFloor": 0,
+            "y_minrange": 0,
+            "y_clipmin": 0,
             "tt_label": "<strong>Position {point.x}:</strong> {point.y:.2f}%",
             "data_labels": [
                 {"name": "CpG Read 1", "ylab": "CpG Retention Rate (%)"},
                 {"name": "CpG Read 2", "ylab": "CpG Retention Rate (%)"},
                 {"name": "CpH Read 1", "ylab": "CpH Retention Rate (%)"},
                 {"name": "CpH Read 2", "ylab": "CpH Retention Rate (%)"},
             ],
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bismark/bismark.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bismark/bismark.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 import logging
 import re
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, beeswarm, linegraph
+from multiqc.plots import bargraph, violin, linegraph
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 # Log parsing regexes
 regexes = {
     "alignment": {
@@ -436,25 +436,25 @@
             plot=bargraph.plot(self.bismark_data["dedup"], keys, config),
         )
 
     def bismark_methlyation_chart(self):
         """Make the methylation plot"""
 
         # Config for the plot
-        defaults = {"max": 100, "min": 0, "suffix": "%", "decimalPlaces": 1}
+        defaults = {"max": 100, "min": 0, "suffix": "%", "tt_decimals": 1}
         keys = {
             "percent_cpg_meth": dict(defaults, **{"title": "Methylated CpG"}),
             "percent_chg_meth": dict(defaults, **{"title": "Methylated CHG"}),
             "percent_chh_meth": dict(defaults, **{"title": "Methylated CHH"}),
         }
 
         self.add_section(
             name="Cytosine Methylation",
             anchor="bismark-methylation",
-            plot=beeswarm.plot(
+            plot=violin.plot(
                 self.bismark_data["methextract"],
                 keys,
                 {
                     "id": "bismark-methylation-dp",
                     "title": "Bismark: Cytosine Methylation",
                 },
             ),
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bowtie1/bowtie1.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bowtie1/bowtie1.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,14 @@
                 "modify": lambda x: x * config.read_count_multiplier,
                 "shared_key": "read_count",
             },
         }
         self.general_stats_addcols(self.bowtie_data, headers)
 
     def bowtie_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "reads_aligned": {"color": "#8bbc21", "name": "Aligned"},
             "multimapped": {"color": "#2f7ed8", "name": "Multimapped"},
             "not_aligned": {"color": "#0d233a", "name": "Not aligned"},
         }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bowtie2/bowtie2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bowtie2/bowtie2.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,14 @@
                 "suffix": "%",
                 "scale": "YlGn",
             }
         }
         self.general_stats_addcols(self.bowtie2_data, headers)
 
     def bowtie2_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         half_warning = ""
         for s_name in self.bowtie2_data:
             if (
                 "paired_aligned_mate_one_halved" in self.bowtie2_data[s_name]
                 or "paired_aligned_mate_multi_halved" in self.bowtie2_data[s_name]
                 or "paired_aligned_mate_none_halved" in self.bowtie2_data[s_name]
             ):
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bracken/bracken.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bracken/bracken.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC module to parse output from bracken """
 
 import logging
 
 from multiqc.modules.kraken import MultiqcModule as KrakenModule
 
 # Initialise the logger
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/busco/busco.py` & `multiqc_sgr-1.22.post0/multiqc/modules/busco/busco.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 parsed_data["lineage_dataset"] = str(s[0])
 
         if len(parsed_data) > 0:
             self.busco_data[f["s_name"]] = parsed_data
             self.add_data_source(f)
 
     def busco_plot(self, lin):
-        """Make the HighCharts HTML for the BUSCO plot for a particular lineage"""
+        """Make the HTML for the BUSCO plot for a particular lineage"""
 
         data = {}
         for s_name in self.busco_data:
             if self.busco_data[s_name].get("lineage_dataset") == lin:
                 data[s_name] = self.busco_data[s_name]
 
         plot_keys = ["complete_single_copy", "fragmented", "complete_duplicated", "missing"]
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/bustools/bustools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/bustools/bustools.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,14 @@
             "effectively calculate the average number of unique transcripts per cell.",
             plot=bargraph.plot(
                 mean_umis,
                 pconfig={
                     "id": "bus_umis",
                     "title": "Bustools: Mean number of UMIs per barcode per sample",
                     "cpswitch": False,
-                    "tt_percentages": False,
                     "ylab": "Mean UMIs per barcode",
                 },
             ),
         )
 
         # barplot for the percentage of reads and barcodes on the whitelist
         percentage_whitelist = {
@@ -283,14 +282,13 @@
                 percentage_whitelist,
                 pconfig={
                     "id": "bus_reads",
                     "title": "Bustools: Barcodes / reads with barcodes in the whitelist",
                     "ymax": 100,
                     "ymin": 0,
                     "cpswitch": False,
-                    "tt_percentages": False,
                     "ylab": "Percentage of barcodes / reads with barcodes in the whitelist",
                     "stacking": None,
                     "ysuffix": "%",
                 },
             ),
         )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/ccs/ccs.py` & `multiqc_sgr-1.22.post0/multiqc/modules/ccs/ccs.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/cellranger/cellranger.py` & `multiqc_sgr-1.22.post0/multiqc/modules/cellranger/cellranger.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/cellranger/count.py` & `multiqc_sgr-1.22.post0/multiqc/modules/cellranger/count.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,14 @@
                     "title": "Cell Ranger: Distribution of Antibody Counts",
                     "ylab": "% Total UMI",
                     "ymax": 100,
                     "cpswitch": False,
                     "use_legend": False,
                     "tt_decimals": 2,
                     "tt_suffix": "%",
-                    "tt_percentages": False,
                 },
                 "keys": keys,
                 "description": "Antibody Counts Distribution Plot",
                 "helptext": "Relative composition of antibody counts for features with at least 1 UMI. Box size represents fraction of total UMIs from cell barcodes that are derived from this antibody. Hover over a box to view more information on a particular antibody, including number of associated barcodes.",
             }
             plots_data["antibody_counts"] = {s_name: combined_data}
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/cellranger/utils.py` & `multiqc_sgr-1.22.post0/multiqc/modules/cellranger/utils.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/cellranger/vdj.py` & `multiqc_sgr-1.22.post0/multiqc/modules/cellranger/vdj.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/checkqc/checkqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/checkqc/checkqc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/clipandmerge/clipandmerge.py` & `multiqc_sgr-1.22.post0/multiqc/modules/clipandmerge/clipandmerge.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,14 @@
                 "scale": "Greens",
                 "format": "{:,.2f}",
             }
         }
         self.general_stats_addcols(self.clipandmerge_data, headers)
 
     def clipandmerge_alignment_plot(self):
-        """Make the HighCharts HTML to plot the duplication rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "merged_reads": {"name": "Merged Reads"},
             "usable_not_merged_forward": {"name": "Usable, not merged (forward)"},
             "usable_not_merged_reverse": {"name": "Usable, not merged (reverse)"},
             "usable_forward_no_pairing_reverse": {"name": "Usable forward-only"},
             "usable_reverse_no_pairing_forward": {"name": "Usable reverse-only"},
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/clusterflow/clusterflow.py` & `multiqc_sgr-1.22.post0/multiqc/modules/clusterflow/clusterflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     )
 
         table_config = {
             "namespace": "Cluster Flow",
             "id": "clusterflow-commands-table",
             "table_title": "Cluster Flow Commands",
             "col1_header": "Tool",
-            "sortRows": False,
+            "sort_rows": False,
             "no_violin": True,
         }
         self.add_section(
             name="Commands",
             anchor="clusterflow-commands",
             description=desc,
             plot=table.plot(tool_cmds, headers, table_config),
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/conpair/conpair.py` & `multiqc_sgr-1.22.post0/multiqc/modules/conpair/conpair.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/custom_content/custom_content.py` & `multiqc_sgr-1.22.post0/multiqc/modules/custom_content/custom_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,40 +3,41 @@
 
 import base64
 import json
 import logging
 import os
 import re
 from collections import defaultdict
+from typing import List, Dict
 
 import yaml
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, beeswarm, heatmap, linegraph, scatter, table
+from multiqc.plots import bargraph, violin, heatmap, linegraph, scatter, table
 from multiqc.utils import report
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
-def custom_module_classes():
+def custom_module_classes() -> List[BaseMultiqcModule]:
     """
     MultiQC Custom Content class. This module does a lot of different
     things depending on the input and is as flexible as possible.
 
     NB: THIS IS TOTALLY DIFFERENT TO ALL OTHER MODULES
     """
 
     # Dict to hold parsed data. Each key should contain a custom data type
     # e.g. output from a particular script. Note that this script may pick
     # up many different types of data from many different sources.
     # Second level keys should be 'config' and 'data'. Data key should then
     # contain sample names, and finally data.
-    cust_mods = defaultdict(lambda: defaultdict(lambda: dict()))
+    cust_mod_by_id: Dict[str, Dict[str, Dict]] = defaultdict(lambda: defaultdict(lambda: dict()))
 
     # Dictionary to hold search patterns - start with those defined in the config
     search_patterns = ["custom_content"]
 
     # First - find files using patterns described in the config
     config_data = getattr(config, "custom_data", {})
     mod_cust_config = {}
@@ -46,26 +47,26 @@
             log.debug(f"config.custom_data row was not a dictionary: {k}")
             continue
         c_id = f.get("id", k)
 
         # Data supplied in with config (e.g. from a multiqc_config.yaml file in working directory)
         if "data" in f:
             try:
-                cust_mods[c_id]["data"].update(f["data"])
+                cust_mod_by_id[c_id]["data"].update(f["data"])
             except ValueError:
                 # HTML plot type doesn't have a data sample-id key, so just take the whole chunk of data
-                cust_mods[c_id]["data"] = f["data"]
-            cust_mods[c_id]["config"].update({k: v for k, v in f.items() if k != "data"})
-            cust_mods[c_id]["config"]["id"] = cust_mods[c_id]["config"].get("id", c_id)
+                cust_mod_by_id[c_id]["data"] = f["data"]
+            cust_mod_by_id[c_id]["config"].update({k: v for k, v in f.items() if k != "data"})
+            cust_mod_by_id[c_id]["config"]["id"] = cust_mod_by_id[c_id]["config"].get("id", c_id)
             continue
 
         # Custom Content ID has search patterns in the config
         if c_id in report.files:
-            cust_mods[c_id]["config"] = f
-            cust_mods[c_id]["config"]["id"] = cust_mods[c_id]["config"].get("id", c_id)
+            cust_mod_by_id[c_id]["config"] = f
+            cust_mod_by_id[c_id]["config"]["id"] = cust_mod_by_id[c_id]["config"].get("id", c_id)
             search_patterns.append(c_id)
             continue
 
         # Must just be configuration for a separate custom-content class
         mod_cust_config[c_id] = f
 
     # Now go through each of the file search patterns
@@ -107,50 +108,50 @@
                     parsed_data = {
                         "id": f["s_name"],
                         "plot_type": "image",
                         "section_name": f["s_name"].replace("_", " ").replace("-", " ").replace(".", " "),
                         "data": img_html,
                     }
                     # If the search pattern 'k' has an associated custom content section config, use it
-                    parsed_data.update(cust_mods.get(k, {}).get("config", {}))
+                    parsed_data.update(cust_mod_by_id.get(k, {}).get("config", {}))
                 elif f_extension == ".html":
                     parsed_data = {"id": f["s_name"], "plot_type": "html", "data": f["f"]}
                     parsed_data.update(_find_html_file_header(f))
 
                 if parsed_data is not None:
                     if isinstance(parsed_data.get("data"), dict):
                         # Run sample-name cleaning on the data keys
                         parsed_data["data"] = {bm.clean_s_name(k, f): v for k, v in parsed_data["data"].items()}
 
                     c_id = parsed_data.get("id", k)
                     if len(parsed_data.get("data", {})) > 0:
                         if isinstance(parsed_data["data"], dict):
-                            cust_mods[c_id]["data"].update(parsed_data["data"])
+                            cust_mod_by_id[c_id]["data"].update(parsed_data["data"])
                         else:
-                            cust_mods[c_id]["data"] = parsed_data["data"]
-                        cust_mods[c_id]["config"].update({j: k for j, k in parsed_data.items() if j != "data"})
+                            cust_mod_by_id[c_id]["data"] = parsed_data["data"]
+                        cust_mod_by_id[c_id]["config"].update({j: k for j, k in parsed_data.items() if j != "data"})
                     else:
                         log.warning(f"No data found in {f['fn']}")
 
                 # txt, csv, tsv etc
                 else:
                     # Look for configuration details in the header
                     m_config = _find_file_header(f)
                     s_name = None
                     if m_config is not None:
                         c_id = m_config.get("id", k)
                         # Update the base config with anything parsed from the file
-                        b_config = cust_mods.get(c_id, {}).get("config", {})
+                        b_config = cust_mod_by_id.get(c_id, {}).get("config", {})
                         b_config.update(m_config)
                         # Now set the module config to the merged dict
                         m_config = dict(b_config)
                         s_name = m_config.get("sample_name")
                     else:
                         c_id = k
-                        m_config = cust_mods.get(c_id, {}).get("config", {})
+                        m_config = cust_mod_by_id.get(c_id, {}).get("config", {})
 
                     # Guess sample name if not given
                     if s_name is None:
                         s_name = f["s_name"]
 
                     # Guess c_id if no information known
                     if k == "custom_content":
@@ -176,46 +177,46 @@
                             log.warning(f"Not able to parse custom data in {f['fn']}")
                         else:
                             # Did we get a new section id from the file?
                             if conf.get("id") is not None:
                                 c_id = conf.get("id")
                             # heatmap - special data type
                             if isinstance(parsed_data, list):
-                                cust_mods[c_id]["data"] = parsed_data
+                                cust_mod_by_id[c_id]["data"] = parsed_data
                             elif conf.get("plot_type") == "html":
-                                cust_mods[c_id]["data"] = parsed_data
+                                cust_mod_by_id[c_id]["data"] = parsed_data
                             else:
-                                cust_mods[c_id]["data"].update(parsed_data)
-                            cust_mods[c_id]["config"].update(conf)
+                                cust_mod_by_id[c_id]["data"].update(parsed_data)
+                            cust_mod_by_id[c_id]["config"].update(conf)
                     except (IndexError, AttributeError, TypeError):
                         log.error(f"Unexpected parsing error for {f['fn']}", exc_info=True)
                         raise  # testing
             except Exception as e:
                 log.error(f"Uncaught exception raised for file '{f['fn']}'")
                 log.exception(e)
 
         # Give log message if no files found for search pattern
         if num_sp_found_files == 0 and k != "custom_content":
             log.debug(f"No samples found: custom content ({k})")
 
     # Filter to strip out ignored sample names
-    for k in cust_mods:
-        cust_mods[k]["data"] = bm.ignore_samples(cust_mods[k]["data"])
+    for k in cust_mod_by_id:
+        cust_mod_by_id[k]["data"] = bm.ignore_samples(cust_mod_by_id[k]["data"])
 
     # Remove any configs that have no data
-    remove_cids = [k for k in cust_mods if len(cust_mods[k]["data"]) == 0]
+    remove_cids = [k for k in cust_mod_by_id if len(cust_mod_by_id[k]["data"]) == 0]
     for k in remove_cids:
-        del cust_mods[k]
+        del cust_mod_by_id[k]
 
-    if len(cust_mods) == 0:
+    if len(cust_mod_by_id) == 0:
         raise ModuleNoSamplesFound
 
     # Go through each data type
     parsed_modules = dict()
-    for c_id, mod in cust_mods.items():
+    for c_id, mod in cust_mod_by_id.items():
         # General Stats
         if mod["config"].get("plot_type") == "generalstats":
             gsheaders = mod["config"].get("pconfig")
             if gsheaders is None:
                 headers = set()
                 for d in mod["data"].values():
                     headers.update(d.keys())
@@ -267,15 +268,15 @@
     sorted_modules = [parsed_mod for parsed_mod in parsed_modules.values() if parsed_mod.anchor not in mod_order]
     sorted_modules.extend(
         [parsed_mod for mod_id in mod_order for parsed_mod in parsed_modules.values() if parsed_mod.anchor == mod_id]
     )
 
     # If we only have General Stats columns then there are no module outputs
     if len(sorted_modules) == 0:
-        if mod["config"].get("plot_type") == "generalstats":
+        if len(cust_mod_by_id) == 1 and list(cust_mod_by_id.values())[0]["config"].get("plot_type") == "generalstats":
             sorted_modules = [bm]
         else:
             raise ModuleNoSamplesFound
 
     return sorted_modules
 
 
@@ -358,15 +359,15 @@
             try:
                 mod["data"] = [{k: {float(x): v[x] for x in v} for k, v in ds.items()} for ds in mod["data"]]
             except ValueError:
                 pass
 
         # Table
         if mod["config"].get("plot_type") == "table":
-            pconfig["sortRows"] = pconfig.get("sortRows", False)
+            pconfig["sort_rows"] = pconfig.get("sort_rows", pconfig.get("sortRows", False))
             headers = mod["config"].get("headers")
             plot = table.plot(mod["data"], headers, pconfig)
 
         # Bar plot
         elif mod["config"].get("plot_type") == "bargraph":
             mod["data"] = [{str(k): v for k, v in ds.items()} for ds in mod["data"]]
             plot = bargraph.plot(mod["data"], mod["config"].get("categories"), pconfig)
@@ -379,17 +380,17 @@
         elif mod["config"].get("plot_type") == "scatter":
             plot = scatter.plot(mod["data"], pconfig)
 
         # Heatmap
         elif mod["config"].get("plot_type") == "heatmap":
             plot = heatmap.plot(mod["data"], mod["config"].get("xcats"), mod["config"].get("ycats"), pconfig)
 
-        # Beeswarm plot
-        elif mod["config"].get("plot_type") == "beeswarm":
-            plot = beeswarm.plot(mod["data"], pconfig)
+        # Violin plot
+        elif mod["config"].get("plot_type") in ["violin", "beeswarm"]:
+            plot = violin.plot(mod["data"], pconfig)
 
         # Raw HTML
         elif mod["config"].get("plot_type") == "html":
             if len(mod["data"]) > 1:
                 log.warning(f"HTML plot type found with more than one dataset in {c_id}")
             content = mod["data"][0]
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/cutadapt/cutadapt.py` & `multiqc_sgr-1.22.post0/multiqc/modules/cutadapt/cutadapt.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,17 +374,17 @@
             pconfig = {
                 "id": f"cutadapt_trimmed_sequences_plot_{end}",
                 "title": "Cutadapt: Lengths of Trimmed Sequences{}".format(
                     "" if end == "default" else f" ({end}' end)"
                 ),
                 "ylab": "Counts",
                 "xlab": "Length Trimmed (bp)",
-                "xDecimals": False,
                 "ymin": 0,
                 "tt_label": "<b>{point.x} bp trimmed</b>: {point.y:.0f}",
+                "xsuffix": " bp",
                 "data_labels": [
                     {"name": "Counts", "ylab": "Count"},
                     {"name": "Obs/Exp", "ylab": "Observed / Expected"},
                 ],
             }
 
             self.add_section(
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/damageprofiler/damageprofiler.py` & `multiqc_sgr-1.22.post0/multiqc/modules/damageprofiler/damageprofiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,16 @@
 
         config = {
             "id": f"length-distribution-{orientation}",
             "title": f"DamageProfiler: Read length distribution - {orientation} ",
             "ylab": "Number of reads",
             "xlab": "Readlength (bp)",
             "xDecimals": False,
-            "tt_label": "{point.y} reads of length {point.x}",
+            "tt_label": "{point.y} reads of length {point.x} bp",
+            "ysuffix": " reads",
             "ymin": 0,
             "xmin": 0,
         }
         return linegraph.plot(data, config)
 
     # Linegraph plot for 3pGtoA
     def threeprime_plot(self):
@@ -249,15 +250,16 @@
             dict_to_add[key] = data
 
         config = {
             "id": "threeprime_misinc_plot",
             "title": "DamageProfiler: 3' G>A misincorporation plot",
             "ylab": "% G to A substituted",
             "xlab": "Nucleotide position from 3'",
-            "tt_label": "{point.y:.2f} % G>A misincorporations at nucleotide position {point.x}",
+            "tt_label": "{point.y:.2f}% G>A misincorporations at nucleotide position {point.x}",
+            "ysuffix": "%",
             "ymin": 0,
             "xmin": 1,
         }
 
         return linegraph.plot(dict_to_add, config)
 
     # Linegraph plot for 5pCtoT
@@ -275,13 +277,14 @@
             dict_to_add[key] = data
 
         config = {
             "id": "fiveprime_misinc_plot",
             "title": "DamageProfiler: 5' C>T misincorporation plot",
             "ylab": "% C to T substituted",
             "xlab": "Nucleotide position from 5'",
-            "tt_label": "{point.y:.2f} % C>T misincorporations at nucleotide position {point.x}",
+            "tt_label": "{point.y:.2f}% C>T misincorporations at nucleotide position {point.x}",
+            "ysuffix": "%",
             "ymin": 0,
             "xmin": 1,
         }
 
         return linegraph.plot(dict_to_add, config)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dedup/dedup.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dedup/dedup.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,14 @@
                 "shared_key": "read_count",
                 "min": 0,
             },
         }
         self.general_stats_addcols(self.dedup_data, headers)
 
     def dedup_alignment_plot(self):
-        """Make the HighCharts HTML to plot the duplication rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "mapped_after_dedup": {"name": "Unique Retained"},
             "not_removed": {"name": "Not Removed"},
             "reverse_removed": {"name": "Reverse Removed"},
             "forward_removed": {"name": "Forward Removed"},
             "merged_removed": {"name": "Merged Removed"},
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/bamPEFragmentSizeDistribution.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/bamPEFragmentSizeDistribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,18 @@
             # Write data to file
             self.write_data_file(self.deeptools_bamPEFragmentSizeDistribution, "deeptools_frag_size_dist")
 
             config = {
                 "id": "fragment_size_distribution_plot",
                 "title": "deeptools: Fragment Size Distribution Plot",
                 "ylab": "Occurrence",
-                "xlab": "Fragment Size (bp)",
+                "xlab": "Fragment Size",
                 "smooth_points": 50,
                 "xmax": 1000,
-                "xDecimals": False,
-                "tt_label": "<b>Fragment Size (bp) {point.x}</b>: {point.y} Occurrence",
+                "tt_label": "<b>{point.x} bp</b>: {point.y}th occurrence",
             }
 
             self.add_section(
                 name="Fragment size distribution",
                 anchor="fragment_size_distribution",
                 description="Distribution of paired-end fragment sizes",
                 plot=linegraph.plot(self.deeptools_bamPEFragmentSizeDistribution, config),
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/bamPEFragmentSizeTable.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/bamPEFragmentSizeTable.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/deeptools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/deeptools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/estimateReadFiltering.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/estimateReadFiltering.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotCorrelation.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotCorrelation.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotCoverage.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotCoverage.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotEnrichment.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotEnrichment.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotFingerprint.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotFingerprint.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotPCA.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotPCA.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/deeptools/plotProfile.py` & `multiqc_sgr-1.22.post0/multiqc/modules/deeptools/plotProfile.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/diamond/diamond.py` & `multiqc_sgr-1.22.post0/multiqc/modules/diamond/diamond.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/disambiguate/disambiguate.py` & `multiqc_sgr-1.22.post0/multiqc/modules/disambiguate/disambiguate.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_hist.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_hist.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "namespace": NAMESPACE,  # Name for grouping. Prepends desc and is in Config Columns modal
     "title": None,  # Short title, table column title
     "description": None,  # Longer description, goes in mouse hover text
     "max": None,  # Minimum value in range, for bar / colour coding
     "min": 0,  # Maximum value in range, for bar / colour coding
     "ceiling": None,  # Maximum value for automatic bar limit
     "floor": None,  # Minimum value for automatic bar limit
-    "minRange": None,  # Minimum range for automatic bar
+    "minrange": None,  # Minimum range for automatic bar
     "scale": "GnBu",  # Colour scale for colour coding. False to disable.
     "bgcols": None,  # Dict with values: background colours for categorical data.
     "colour": "15, 150, 255",  # Colour for column grouping
     "suffix": None,  # Suffix for value (eg. "%")
     "format": "{:,.2f}",  # Value format string - MultiQC default 1 decimal places
     "cond_formatting_rules": None,  # Rules for conditional formatting table cell values.
     "cond_formatting_colours": None,  # Styles for conditional formatting of table cell values
@@ -463,15 +463,15 @@
 # The TABLE_CONFIG defines common configs for all whole tables.
 TABLE_CONFIG = {
     "namespace": NAMESPACE,  # Name for grouping. Prepends desc and is in Config Columns modal
     "id": None,  # ID used for the table
     "table_title": None,  # Title of the table. Used in the column config modal
     "save_file": False,  # Whether to save the table data to a file
     "raw_data_fn": None,  # File basename to use for raw data file
-    "sortRows": True,  # Whether to sort rows alphabetically
+    "sort_rows": True,  # Whether to sort rows alphabetically
     "only_defined_headers": True,  # Only show columns that are defined in the headers config
     "col1_header": None,  # The header used for the first column with sample names.
     "no_violin": False,  # Force a table to always be plotted (beeswarm by default if many rows)
 }
 # Below are region-specific configs with higher priority.
 REGION_TABLE_CONFIG = {
     WGS: {
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/coverage_per_contig.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/coverage_per_contig.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/dragen.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/dragen.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/dragen_gc_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/dragen_gc_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/fragment_length.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/fragment_length.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/mapping_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/mapping_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/overall_mean_cov.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/overall_mean_cov.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/ploidy_estimation_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/ploidy_estimation_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/rna_quant_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/rna_quant_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/rna_transcript_cov.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/rna_transcript_cov.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/sc_atac_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/sc_atac_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/sc_rna_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/sc_rna_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/time_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/time_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/trimmer_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/trimmer_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/utils.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
     "namespace",
     "title",
     "description",
     "max",
     "min",
     "ceiling",
     "floor",
-    "minRange",
+    "minrange",
     "scale",
     "bgcols",
     "colour",
     "suffix",
     "format",
     "cond_formatting_rules",
     "cond_formatting_colours",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen/vc_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen/vc_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/assets/js/multiqc_dragen_fastqc.js` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/js/multiqc_fastqc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,10 @@
-// Javascript for the FastQC MultiQC Mod
+////////////////////////////////////////////////
+// Javascript for the FastQC MultiQC module
+////////////////////////////////////////////////
 
 ///////////////
 // Per Base Sequence Content
 ///////////////
 
 // Global vars
 fastqc_passfails = {}; // { <module>: { <section>: { <sample>: { data } } }
@@ -20,15 +22,14 @@
         var key_value = JSON.parse(elem.innerHTML);
         fastqc_seq_content[key_value[0]] = key_value[1];
     });
 }
 
 // Set up listeners etc on page load
 $(function() {
-    load_fastqc_passfails();
     load_fastqc_seq_content();
 
     // Go through each FastQC module in case there are multiple
     // #mqc-module-section-fastqc, #mqc-module-section-fastqc-1, ...
     // or #mqc-module-section-configured-anchor, #mqc-module-section-configured-anchor-1, ...
     var fastqc_modules = $(".fastqc_passfails").closest(".mqc-module-section");
     fastqc_modules.each(function() {
@@ -59,14 +60,16 @@
             orig_s_names[s_name] = s_name;
         }
     }
 
     // Function to plot heatmap
     function fastqc_seq_content_heatmap() {
         // Get sample names, rename and skip hidden samples
+        sample_names = [];
+        sample_statuses = [];
         var p_data = {};
         var hidden_samples = 0;
         $.each(fastqc_seq_content[module_key], function(s_name, data) {
             // rename sample names
             var orig_s_name = s_name;
             var t_status = fastqc_passfails[module_key]["per_base_sequence_content"][s_name];
             $.each(window.mqc_rename_f_texts, function(idx, f_text) {
@@ -405,39 +408,39 @@
     });
 
     /////////
     /// SEQ CONTENT HEATMAP LISTENERS
     /////////
 
     // Seq Content heatmap export button
-    module_element.find("#dragen_fastqc_per_base_sequence_content_export_btn").click(function(e) {
+    module_element.find("#fastqc_per_base_sequence_content_export_btn").click(function(e) {
         e.preventDefault();
-        // In case of repeated modules: #dragen_fastqc_per_base_sequence_content_plot, #dragen_fastqc_per_base_sequence_content_plot-1, ..
-        var plot_id = module_element.find(".dragen_fastqc_per_base_sequence_content_plot").attr("id");
+        // In case of repeated modules: #fastqc_per_base_sequence_content_plot, #fastqc_per_base_sequence_content_plot-1, ..
+        var plot_id = module_element.find(".fastqc_per_base_sequence_content_plot").attr("id");
         // Tick only this plot in the toolbox and slide out
         $("#mqc_export_selectplots input").prop("checked", false);
         $('#mqc_export_selectplots input[value="' + plot_id + '"]').prop("checked", true);
         mqc_toolbox_openclose("#mqc_exportplots", true);
     });
 
     // Export plot
-    module_element.find(".dragen_fastqc_per_base_sequence_content_plot").on("mqc_plotexport_image", function(e, cfg) {
+    module_element.find(".fastqc_per_base_sequence_content_plot").on("mqc_plotexport_image", function(e, cfg) {
         alert(
-            "Apologies, it's not yet possible to export the DRAGEN-FastQC per-base sequence content plot.\nPlease take a screengrab or export the JSON data.",
+            "Apologies, it's not yet possible to export the FastQC per-base sequence content plot.\nPlease take a screengrab or export the JSON data.",
         );
     });
-    module_element.find(".dragen_fastqc_per_base_sequence_content_plot").on("mqc_plotexport_data", function(e, cfg) {
+    module_element.find(".fastqc_per_base_sequence_content_plot").on("mqc_plotexport_data", function(e, cfg) {
         if (cfg["ft"] == "json") {
             json_str = JSON.stringify(fastqc_seq_content[module_key], null, 2);
             var blob = new Blob([json_str], {
                 type: "text/plain;charset=utf-8"
             });
             saveAs(blob, cfg["fname"]);
         } else {
-            alert("Apologies, the DRAGEN-FastQC per-base sequence content plot can only be exported as JSON currently.");
+            alert("Apologies, the FastQC per-base sequence content plot can only be exported as JSON currently.");
         }
     });
 
     // Seq Content heatmap mouse rollover
     module_element.find("#fastqc_seq_heatmap").mousemove(function(e) {
         // Replace the heading above the heatmap
         var pos = findPos(this);
@@ -461,15 +464,15 @@
         if (s_status == "warn") {
             s_status_class = "label-warning";
         }
         if (s_status == "fail") {
             s_status_class = "label-danger";
         }
         module_element
-            .find("#dragen_fastqc_per_base_sequence_content_plot_div .s_name")
+            .find("#fastqc_per_base_sequence_content_plot_div .s_name")
             .html(
                 '<span class="glyphicon glyphicon-info-sign"></span> ' +
                 s_name +
                 ' <span class="label s_status ' +
                 s_status_class +
                 '">' +
                 s_status +
@@ -502,15 +505,15 @@
         module_element.find("#fastqc_seq_heatmap_key_g span").text(thispoint["g"].toFixed(0) + "%");
         module_element.find("#fastqc_seq_heatmap_key_pos").text(thispoint["base"] + " bp");
     });
 
     // Remove sample name again when mouse leaves
     module_element.find("#fastqc_seq_heatmap").mouseout(function(e) {
         module_element
-            .find("#dragen_fastqc_per_base_sequence_content_plot_div .s_name")
+            .find("#fastqc_per_base_sequence_content_plot_div .s_name")
             .html('<span class="glyphicon glyphicon-info-sign"></span> Rollover for sample name');
         module_element.find("#fastqc_seq_heatmap_key_pos").text("-");
         module_element.find("#fastqc_seq_heatmap_key_t span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_c span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_a span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_g span").text("-");
     });
@@ -529,15 +532,15 @@
             plot_single_seqcontent(s_name);
         }
     });
     module_element.on("click", ".fastqc_seqcontent_single_prevnext", function(e) {
         e.preventDefault();
         // Find next / prev sample name
         var idx = sample_names.indexOf(current_single_plot);
-        if ($(this).data("action") == "next") {
+        if ($(this).data("action") === "next") {
             idx++;
         } else {
             idx--;
         }
         if (idx < 0) {
             idx = sample_names.length - 1;
         }
@@ -562,28 +565,19 @@
             base = parseFloat(base[0]);
             plot_data[0].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["t"]]);
             plot_data[1].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["c"]]);
             plot_data[2].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["a"]]);
             plot_data[3].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["g"]]);
         }
         // Update the chart
-        var hc = module_element.find("#fastqc_sequence_content_single").highcharts();
-        for (i = 0; i < plot_data.length; i++) {
-            hc.series[i].setData(plot_data[i], false);
-        }
-        hc.setTitle({
-            text: s_name
-        });
-        hc.redraw({
-            duration: 200
-        });
+        plot_single_seqcontent(s_name);
     });
     module_element.on("click", "#fastqc_sequence_content_single_back", function(e) {
         e.preventDefault();
-        module_element.find("#dragen_fastqc_per_base_sequence_content_plot_div").slideDown();
+        module_element.find("#fastqc_per_base_sequence_content_plot_div").slideDown();
         module_element.find("#fastqc_sequence_content_single_wrapper").slideUp(function() {
             $(this).remove();
         });
     });
 
     // Highlight the custom heatmap
     $(document).on("mqc_highlights mqc_hidesamples mqc_renamesamples mqc_plotresize", function(e) {
@@ -637,16 +631,16 @@
                 x: base,
                 y: data[d]["g"],
                 name: data[d]["base"]
             });
         }
 
         // Create plot div if it doesn't exist, and hide overview
-        if (module_element.find("#fastqc_sequence_content_single_wrapper").length == 0) {
-            var plot_div = module_element.find("#dragen_fastqc_per_base_sequence_content_plot_div");
+        if (module_element.find("#fastqc_sequence_content_single_wrapper").length === 0) {
+            var plot_div = module_element.find("#fastqc_per_base_sequence_content_plot_div");
             plot_div.slideUp();
             var newplot =
                 '<div id="fastqc_sequence_content_single_wrapper"> \
             <div id="fastqc_sequence_content_single_controls">\
                 <button class="btn btn-primary btn-sm" id="fastqc_sequence_content_single_back">Back to overview heatmap</button> \
                 <div class="btn-group btn-group-sm"> \
                     <button class="btn btn-default fastqc_seqcontent_single_prevnext" data-action="prev">&laquo; Prev</button> \
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/base_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/base_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,18 +73,17 @@
 
         pconfig = {
             "id": "dragen_fastqc_per_base_sequence_quality_plot",
             "title": "DRAGEN-QC: Per-Position Quality Scores",
             "ylab": "Phred Quality Score",
             "xlab": "Position (bp)",
             "ymin": 0,
-            "xDecimals": False,
             "tt_label": "<b>Base {point.x}</b>: {point.y:.2f}",
             # 'colors': self.get_status_cols('per_base_sequence_quality'),
-            "yPlotBands": [
+            "y_bands": [
                 {"from": 28, "to": 100, "color": "#c3e6c3"},
                 {"from": 20, "to": 28, "color": "#e6dcc3"},
                 {"from": 0, "to": 20, "color": "#e6c3c3"},
             ],
         }
 
         self.add_section(
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/content_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/content_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,22 +63,20 @@
             return None
 
         pconfig = {
             "id": "dragenqc_per_base_n_content_plot",
             "title": "DRAGEN-QC: Per-Position N Content",
             "ylab": "Percentage N-Count",
             "xlab": "Position in Read (bp)",
-            "yCeiling": 100,
-            "yMinRange": 5,
+            "y_clipmax": 100,
+            "y_minrange": 5,
             "ymin": 0,
             "xmin": 0,
-            "xDecimals": False,
-            # 'colors': self.get_status_cols('per_base_n_content'),
             "tt_label": "<b>Base {point.x}</b>: {point.y:.2f}%",
-            "yPlotBands": [
+            "y_bands": [
                 {"from": 20, "to": 100, "color": "#e6c3c3"},
                 {"from": 5, "to": 20, "color": "#e6dcc3"},
                 {"from": 0, "to": 5, "color": "#c3e6c3"},
             ],
         }
 
         self.add_section(
@@ -236,21 +234,20 @@
                         data[r_name][pos] = 100.0 * cumsum / total
 
         pconfig = {
             "id": "dragen_fastqc_adapter_content_plot",
             "title": "FastQC: Adapter Content",
             "ylab": "% of Sequences",
             "xlab": "Position (bp)",
-            "yCeiling": 100,
-            "yMinRange": 5,
+            "y_clipmax": 100,
+            "y_minrange": 5,
             "ymin": 0,
-            "xDecimals": False,
             "tt_label": "<b>Base {point.x}</b>: {point.y:.2f}%",
             "hide_empty": True,
-            "yPlotBands": [
+            "y_bands": [
                 {"from": 20, "to": 100, "color": "#e6c3c3"},
                 {"from": 5, "to": 20, "color": "#e6dcc3"},
                 {"from": 0, "to": 5, "color": "#c3e6c3"},
             ],
         }
 
         self.add_section(
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/dragen_fastqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/dragen_fastqc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/gc_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/gc_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/read_metrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/read_metrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/dragen_fastqc/util.py` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/util.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/eigenstratdatabasetools/eigenstratdatabasetools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/eigenstratdatabasetools/eigenstratdatabasetools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastp/fastp.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fastp/fastp.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,16 +452,16 @@
         """Make the read N content plot for Fastp"""
         data_labels, pdata = self.filter_pconfig_pdata_subplots(self.fastp_n_content_data, "Base Content Percent")
         pconfig = {
             "id": "fastp-seq-content-n-plot",
             "title": "Fastp: Read N Content",
             "xlab": "Read Position",
             "ylab": "R1 Before filtering: Base Content Percent",
-            "yCeiling": 100,
-            "yMinRange": 5,
+            "y_clipmax": 100,
+            "y_minrange": 5,
             "ymin": 0,
             "tt_label": "{point.x}: {point.y:.2f}%",
             "data_labels": data_labels,
         }
         return linegraph.plot(pdata, pconfig)
 
     def filter_pconfig_pdata_subplots(self, data, label):
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastq_screen/fastq_screen.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fastq_screen/fastq_screen.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     def fqscreen_bisulfite_plot(self):
         """Make a stacked barplot for the bisulfite data, if we have any"""
 
         pconfig = {
             "id": "fastq_screen_bisulfite_plot",
             "title": "FastQ Screen: Bisulfite Mapping Strand Orientation",
             "hide_zero_cats": False,
-            "ylab": "Percentages",
+            "ylab": "Reads",
             "data_labels": [],
         }
 
         cats = {
             "original_top_strand": {"name": "Original top strand", "color": "#80cdc1"},
             "complementary_to_original_top_strand": {
                 "name": "Complementary to original top strand",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/css/multiqc_fastqc.css` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/assets/css/multiqc_fastqc.css`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/assets/js/multiqc_fastqc.js` & `multiqc_sgr-1.22.post0/multiqc/modules/dragen_fastqc/assets/js/multiqc_dragen_fastqc.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,10 @@
-// Javascript for the FastQC MultiQC Mod
+////////////////////////////////////////////////
+// Javascript for the DRAGEN FastQC MultiQC module
+////////////////////////////////////////////////
 
 ///////////////
 // Per Base Sequence Content
 ///////////////
 
 // Global vars
 fastqc_passfails = {}; // { <module>: { <section>: { <sample>: { data } } }
@@ -20,14 +22,15 @@
         var key_value = JSON.parse(elem.innerHTML);
         fastqc_seq_content[key_value[0]] = key_value[1];
     });
 }
 
 // Set up listeners etc on page load
 $(function() {
+    load_fastqc_passfails();
     load_fastqc_seq_content();
 
     // Go through each FastQC module in case there are multiple
     // #mqc-module-section-fastqc, #mqc-module-section-fastqc-1, ...
     // or #mqc-module-section-configured-anchor, #mqc-module-section-configured-anchor-1, ...
     var fastqc_modules = $(".fastqc_passfails").closest(".mqc-module-section");
     fastqc_modules.each(function() {
@@ -58,16 +61,14 @@
             orig_s_names[s_name] = s_name;
         }
     }
 
     // Function to plot heatmap
     function fastqc_seq_content_heatmap() {
         // Get sample names, rename and skip hidden samples
-        sample_names = [];
-        sample_statuses = [];
         var p_data = {};
         var hidden_samples = 0;
         $.each(fastqc_seq_content[module_key], function(s_name, data) {
             // rename sample names
             var orig_s_name = s_name;
             var t_status = fastqc_passfails[module_key]["per_base_sequence_content"][s_name];
             $.each(window.mqc_rename_f_texts, function(idx, f_text) {
@@ -406,39 +407,39 @@
     });
 
     /////////
     /// SEQ CONTENT HEATMAP LISTENERS
     /////////
 
     // Seq Content heatmap export button
-    module_element.find("#fastqc_per_base_sequence_content_export_btn").click(function(e) {
+    module_element.find("#dragen_fastqc_per_base_sequence_content_export_btn").click(function(e) {
         e.preventDefault();
-        // In case of repeated modules: #fastqc_per_base_sequence_content_plot, #fastqc_per_base_sequence_content_plot-1, ..
-        var plot_id = module_element.find(".fastqc_per_base_sequence_content_plot").attr("id");
+        // In case of repeated modules: #dragen_fastqc_per_base_sequence_content_plot, #dragen_fastqc_per_base_sequence_content_plot-1, ..
+        var plot_id = module_element.find(".dragen_fastqc_per_base_sequence_content_plot").attr("id");
         // Tick only this plot in the toolbox and slide out
         $("#mqc_export_selectplots input").prop("checked", false);
         $('#mqc_export_selectplots input[value="' + plot_id + '"]').prop("checked", true);
         mqc_toolbox_openclose("#mqc_exportplots", true);
     });
 
     // Export plot
-    module_element.find(".fastqc_per_base_sequence_content_plot").on("mqc_plotexport_image", function(e, cfg) {
+    module_element.find(".dragen_fastqc_per_base_sequence_content_plot").on("mqc_plotexport_image", function(e, cfg) {
         alert(
-            "Apologies, it's not yet possible to export the FastQC per-base sequence content plot.\nPlease take a screengrab or export the JSON data.",
+            "Apologies, it's not yet possible to export the DRAGEN-FastQC per-base sequence content plot.\nPlease take a screengrab or export the JSON data.",
         );
     });
-    module_element.find(".fastqc_per_base_sequence_content_plot").on("mqc_plotexport_data", function(e, cfg) {
+    module_element.find(".dragen_fastqc_per_base_sequence_content_plot").on("mqc_plotexport_data", function(e, cfg) {
         if (cfg["ft"] == "json") {
             json_str = JSON.stringify(fastqc_seq_content[module_key], null, 2);
             var blob = new Blob([json_str], {
                 type: "text/plain;charset=utf-8"
             });
             saveAs(blob, cfg["fname"]);
         } else {
-            alert("Apologies, the FastQC per-base sequence content plot can only be exported as JSON currently.");
+            alert("Apologies, the DRAGEN-FastQC per-base sequence content plot can only be exported as JSON currently.");
         }
     });
 
     // Seq Content heatmap mouse rollover
     module_element.find("#fastqc_seq_heatmap").mousemove(function(e) {
         // Replace the heading above the heatmap
         var pos = findPos(this);
@@ -462,15 +463,15 @@
         if (s_status == "warn") {
             s_status_class = "label-warning";
         }
         if (s_status == "fail") {
             s_status_class = "label-danger";
         }
         module_element
-            .find("#fastqc_per_base_sequence_content_plot_div .s_name")
+            .find("#dragen_fastqc_per_base_sequence_content_plot_div .s_name")
             .html(
                 '<span class="glyphicon glyphicon-info-sign"></span> ' +
                 s_name +
                 ' <span class="label s_status ' +
                 s_status_class +
                 '">' +
                 s_status +
@@ -503,15 +504,15 @@
         module_element.find("#fastqc_seq_heatmap_key_g span").text(thispoint["g"].toFixed(0) + "%");
         module_element.find("#fastqc_seq_heatmap_key_pos").text(thispoint["base"] + " bp");
     });
 
     // Remove sample name again when mouse leaves
     module_element.find("#fastqc_seq_heatmap").mouseout(function(e) {
         module_element
-            .find("#fastqc_per_base_sequence_content_plot_div .s_name")
+            .find("#dragen_fastqc_per_base_sequence_content_plot_div .s_name")
             .html('<span class="glyphicon glyphicon-info-sign"></span> Rollover for sample name');
         module_element.find("#fastqc_seq_heatmap_key_pos").text("-");
         module_element.find("#fastqc_seq_heatmap_key_t span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_c span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_a span").text("-");
         module_element.find("#fastqc_seq_heatmap_key_g span").text("-");
     });
@@ -526,56 +527,17 @@
         var idx = Math.floor(y / s_height);
         var s_name = sample_names[idx];
         var orig_s_name = orig_s_names[sample_names[idx]];
         if (orig_s_name !== undefined) {
             plot_single_seqcontent(s_name);
         }
     });
-    module_element.on("click", ".fastqc_seqcontent_single_prevnext", function(e) {
-        e.preventDefault();
-        // Find next / prev sample name
-        var idx = sample_names.indexOf(current_single_plot);
-        if ($(this).data("action") === "next") {
-            idx++;
-        } else {
-            idx--;
-        }
-        if (idx < 0) {
-            idx = sample_names.length - 1;
-        }
-        if (idx >= sample_names.length) {
-            idx = 0;
-        }
-        var s_name = sample_names[idx];
-        var orig_s_name = orig_s_names[sample_names[idx]];
-        current_single_plot = s_name;
-        // Prep the new plot data
-        var plot_data = [
-            [],
-            [],
-            [],
-            []
-        ];
-        var bases = Object.keys(fastqc_seq_content[module_key][orig_s_name]).sort(function(a, b) {
-            return a - b;
-        });
-        for (i = 0; i < bases.length; i++) {
-            var base = fastqc_seq_content[module_key][orig_s_name][bases[i]]["base"].toString().split("-");
-            base = parseFloat(base[0]);
-            plot_data[0].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["t"]]);
-            plot_data[1].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["c"]]);
-            plot_data[2].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["a"]]);
-            plot_data[3].push([base, fastqc_seq_content[module_key][orig_s_name][bases[i]]["g"]]);
-        }
-        // Update the chart
-        plot_single_seqcontent(s_name);
-    });
     module_element.on("click", "#fastqc_sequence_content_single_back", function(e) {
         e.preventDefault();
-        module_element.find("#fastqc_per_base_sequence_content_plot_div").slideDown();
+        module_element.find("#dragen_fastqc_per_base_sequence_content_plot_div").slideDown();
         module_element.find("#fastqc_sequence_content_single_wrapper").slideUp(function() {
             $(this).remove();
         });
     });
 
     // Highlight the custom heatmap
     $(document).on("mqc_highlights mqc_hidesamples mqc_renamesamples mqc_plotresize", function(e) {
@@ -629,16 +591,16 @@
                 x: base,
                 y: data[d]["g"],
                 name: data[d]["base"]
             });
         }
 
         // Create plot div if it doesn't exist, and hide overview
-        if (module_element.find("#fastqc_sequence_content_single_wrapper").length === 0) {
-            var plot_div = module_element.find("#fastqc_per_base_sequence_content_plot_div");
+        if (module_element.find("#fastqc_sequence_content_single_wrapper").length == 0) {
+            var plot_div = module_element.find("#dragen_fastqc_per_base_sequence_content_plot_div");
             plot_div.slideUp();
             var newplot =
                 '<div id="fastqc_sequence_content_single_wrapper"> \
             <div id="fastqc_sequence_content_single_controls">\
                 <button class="btn btn-primary btn-sm" id="fastqc_sequence_content_single_back">Back to overview heatmap</button> \
                 <div class="btn-group btn-group-sm"> \
                     <button class="btn btn-default fastqc_seqcontent_single_prevnext" data-action="prev">&laquo; Prev</button> \
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,15 +617,14 @@
             "id": "fastqc_per_sequence_gc_content_plot",
             "title": "FastQC: Per Sequence GC Content",
             "xlab": "% GC",
             "ylab": "Percentage",
             "ymin": 0,
             "xmax": 100,
             "xmin": 0,
-            "yDecimals": False,
             "tt_label": "<b>{point.x}% GC</b>: {point.y}",
             "colors": self.get_status_cols("per_sequence_gc_content"),
             "data_labels": [
                 {"name": "Percentages", "ylab": "Percentage", "tt_suffix": "%"},
                 {"name": "Counts", "ylab": "Count", "tt_suffix": ""},
             ],
         }
@@ -666,24 +665,22 @@
                         pass
 
         desc = """The average GC content of reads. Normal random library typically have a
         roughly normal distribution of GC content."""
         if theoretical_gc is not None:
             # Calculate the count version of the theoretical data based on the largest data store
             max_total = max([sum(d.values()) for d in data.values()])
-            esconfig = {
+            extra_series_config = {
                 "name": "Theoretical GC Content",
-                "dashStyle": "Dash",
-                "lineWidth": 2,
-                "color": "#000000",
-                "marker": {"enabled": False},
-                "enableMouseTracking": False,
-                "showInLegend": False,
+                "dash": "dash",
+                "line": {"width": 2},
+                "color": "black",
+                "showlegend": False,
             }
-            pconfig["extra_series"] = [[dict(esconfig)], [dict(esconfig)]]
+            pconfig["extra_series"] = [[dict(extra_series_config)], [dict(extra_series_config)]]
             pconfig["extra_series"][0][0]["data"] = theoretical_gc
             pconfig["extra_series"][1][0]["data"] = [[d[0], (d[1] / 100.0) * max_total] for d in theoretical_gc]
             desc = f" **The dashed black line shows theoretical GC content:** `{theoretical_gc_name}`"
 
         self.add_section(
             name="Per Sequence GC Content",
             anchor="fastqc_per_sequence_gc_content",
@@ -727,22 +724,21 @@
             return None
 
         pconfig = {
             "id": "fastqc_per_base_n_content_plot",
             "title": "FastQC: Per Base N Content",
             "ylab": "Percentage N-Count",
             "xlab": "Position in Read (bp)",
-            "yCeiling": 100,
-            "yMinRange": 5,
+            "y_clipmax": 100,
+            "y_minrange": 5,
             "ymin": 0,
             "xmin": 0,
-            "xDecimals": False,
             "colors": self.get_status_cols("per_base_n_content"),
             "tt_label": "<b>Base {point.x}</b>: {point.y:.2f}%",
-            "yPlotBands": [
+            "y_bands": [
                 {"from": 20, "to": 100, "color": "#e6c3c3"},
                 {"from": 5, "to": 20, "color": "#e6dcc3"},
                 {"from": 0, "to": 5, "color": "#c3e6c3"},
             ],
         }
 
         self.add_section(
@@ -920,19 +916,18 @@
         }
 
         # Config for the plot
         pconfig = {
             "id": "fastqc_overrepresented_sequences_plot",
             "title": "FastQC: Overrepresented sequences sample summary",
             "ymin": 0,
-            "yCeiling": 100,
-            "yMinRange": 20,
+            "y_clipmax": 100,
+            "y_minrange": 20,
             "tt_decimals": 2,
             "tt_suffix": "%",
-            "tt_percentages": False,
             "cpswitch": False,
             "ylab": "Percentage of Total Sequences",
         }
 
         # Check if any samples have more than 1% overrepresented sequences, else don't make plot.
         if max([x["total_overrepresented"] for x in data.values()]) < 1:
             plot_html = '<div class="alert alert-info">{} samples had less than 1% of reads made up of overrepresented sequences</div>'.format(
@@ -1031,15 +1026,15 @@
                 data,
                 headers,
                 {
                     "namespace": self.name,
                     "id": "fastqc_top_overrepresented_sequences_table",
                     "table_title": "FastQC: Top overrepresented sequences",
                     "col1_header": "Overrepresented sequence",
-                    "sortRows": False,
+                    "sort_rows": False,
                 },
             ),
         )
 
     def adapter_content_plot(self):
         """Create the HTML for the FastQC adapter plot"""
 
@@ -1066,21 +1061,20 @@
         data = {k: d for k, d in data.items() if max(data[k].values()) >= 0.1}
 
         pconfig = {
             "id": "fastqc_adapter_content_plot",
             "title": "FastQC: Adapter Content",
             "ylab": "% of Sequences",
             "xlab": "Position (bp)",
-            "yCeiling": 100,
-            "yMinRange": 5,
+            "y_clipmax": 100,
+            "y_minrange": 5,
             "ymin": 0,
-            "xDecimals": False,
             "tt_label": "<b>Base {point.x}</b>: {point.y:.2f}%",
             "hide_empty": True,
-            "yPlotBands": [
+            "y_bands": [
                 {"from": 20, "to": 100, "color": "#e6c3c3"},
                 {"from": 5, "to": 20, "color": "#e6dcc3"},
                 {"from": 0, "to": 5, "color": "#c3e6c3"},
             ],
         }
 
         if len(data) > 0:
@@ -1145,15 +1139,15 @@
             "square": False,
             "colstops": [
                 [0, "#ffffff"],
                 [0.25, "#d9534f"],
                 [0.5, "#fee391"],
                 [1, "#5cb85c"],
             ],
-            "decimalPlaces": 1,
+            "tt_decimals": 1,
             "legend": False,
             "datalabels": False,
             "xcats_samples": False,
             "angled_xticks": False,
         }
 
         self.add_section(
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_genome.txt` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_genome.txt`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_txome.txt` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_hg38_txome.txt`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_genome.txt` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_genome.txt`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_txome.txt` & `multiqc_sgr-1.22.post0/multiqc/modules/fastqc/fastqc_theoretical_gc/fastqc_theoretical_gc_mm10_txome.txt`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/featureCounts/feature_counts.py` & `multiqc_sgr-1.22.post0/multiqc/modules/featureCounts/feature_counts.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fgbio/ErrorRateByReadPosition.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fgbio/ErrorRateByReadPosition.py`

 * *Files 5% similar despite different names*

```diff
@@ -99,16 +99,15 @@
 
     # Plot the data and add section
     pconfig = {
         "id": "fgbio_ErrorRateByReadPosition",
         "title": "Fgbio: Error Rate by Read Position",
         "ylab": "Error rate",
         "xlab": "Read Position",
-        "xDecimals": False,
-        "tt_label": "<b>read position {point.x}</b>: {point.y:.2f} %",
+        "tt_label": "<b>read position {point.x}</b>: {point.y:.2f}%",
         "ymax": y_max,
         "ymin": 0,
         "data_labels": [
             {"name": "Error Rate", "ylab": "Error Rate"},
             {"name": "A > C", "ylab": "A to C error rate"},
             {"name": "A > G", "ylab": "A to G error rate"},
             {"name": "A > T", "ylab": "A to T error rate"},
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fgbio/fgbio.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fgbio/fgbio.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/fgbio/groupreadsbyumi.py` & `multiqc_sgr-1.22.post0/multiqc/modules/fgbio/groupreadsbyumi.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,18 +52,24 @@
     def parse_groupreadsbyumi_plot(self):
         config = {
             "id": "fgbio-groupreadsbyumi-plot",
             "title": "fgbio: Family size count",
             "ylab": "Number of UMIs",
             "xlab": "Reads supporting UMI",
             "xmax": 15,
-            "xDecimals": False,
             "data_labels": [
-                {"name": "Counts", "ylab": "Number of UMIs"},
-                {"name": "Percentages", "ylab": "Percentage of sample"},
+                {
+                    "name": "Counts",
+                    "ylab": "Number of UMIs",
+                },
+                {
+                    "name": "Percentages",
+                    "ylab": "Percentage of sample",
+                    "ysuffix": "%",
+                },
             ],
         }
 
         self.add_section(
             name="GroupReadsByUmi statistics",
             anchor="fgbio-groupreadsbyumi",
             description="""During `GroupReadsByUmi` processing, family size count data is generated,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/filtlong/filtlong.py` & `multiqc_sgr-1.22.post0/multiqc/modules/filtlong/filtlong.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/flash/flash.py` & `multiqc_sgr-1.22.post0/multiqc/modules/flash/flash.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-
 import logging
 import re
 import traceback
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 from multiqc.plots import bargraph, linegraph
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/flexbar/flexbar.py` & `multiqc_sgr-1.22.post0/multiqc/modules/flexbar/flexbar.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,14 @@
                 s_name = f["s_name"]
                 parsed_data = dict()
 
         # Pick up any partial logs
         _save_data(parsed_data)
 
     def flexbar_barplot(self):
-        """Make the HighCharts HTML to plot the flexbar rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "remaining_reads": {"color": "#437bb1", "name": "Remaining reads"},
             "skipped_due_to_uncalled_bases": {"color": "#e63491", "name": "Skipped due to uncalled bases"},
             "short_prior_to_adapter_removal": {"color": "#b1084c", "name": "Short prior to adapter removal"},
             "finally_skipped_short_reads": {"color": "#7f0000", "name": "Finally skipped short reads"},
         }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/freyja/freyja.py` & `multiqc_sgr-1.22.post0/multiqc/modules/freyja/freyja.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC module to parse output from Freyja """
 
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 from multiqc.plots import bargraph
 from multiqc.utils import mqc_colour
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gatk/analyze_saturation_mutagenesis.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gatk/analyze_saturation_mutagenesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC submodule to parse output from GATK tool AnalyzeSaturationMutagenesis """
 
 import logging
 from collections import defaultdict
 
 from multiqc import config
 from multiqc.plots import bargraph, table
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gatk/base_recalibrator.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gatk/base_recalibrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC submodule to parse output from GATK BaseRecalibrator """
 
 import logging
 from collections import namedtuple
 from itertools import groupby
 
 from multiqc.plots import linegraph, scatter
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gatk/gatk.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gatk/gatk.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gatk/varianteval.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gatk/varianteval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC submodule to parse output from GATK varianteval """
 
 import logging
 
 from multiqc.plots import bargraph, table
 
 # Initialise the logger
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gffcompare/gffcompare.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gffcompare/gffcompare.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/goleft_indexcov/goleft_indexcov.py` & `multiqc_sgr-1.22.post0/multiqc/modules/goleft_indexcov/goleft_indexcov.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,18 +156,18 @@
 
     def bin_plot(self):
         pconfig = {
             "id": "goleft_indexcov-bin-plot",
             "title": "goleft indexcov: Problematic low and non-uniform coverage bins",
             "xlab": "Proportion of bins with depth < 0.15",
             "ylab": "Proportion of bins with depth outside of (0.85, 1.15)",
-            "yCeiling": 1.0,
-            "yFloor": 0.0,
-            "xCeiling": 1.0,
-            "xFloor": 0.0,
+            "ymax": 1.0,
+            "ymin": 0.0,
+            "x_clipmax": 1.0,
+            "x_clipmin": 0.0,
         }
         extra = ""
         if len(self.bin_plot_data_empty_samples) > 0:
             # Bootstrap alert about missing samples
             extra = f"""<div class="alert alert-warning" style="margin:2rem 0;">
                 <strong>Warning:</strong>
                 {len(self.bin_plot_data_empty_samples)} sample{'s' if len(self.bin_plot_data_empty_samples) > 1 else ''} had zero bins and could not be plotted.
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/gopeaks/gopeaks.py` & `multiqc_sgr-1.22.post0/multiqc/modules/gopeaks/gopeaks.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/happy/happy.py` & `multiqc_sgr-1.22.post0/multiqc/modules/happy/happy.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hicexplorer/hicexplorer.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hicexplorer/hicexplorer.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hicpro/hicpro.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hicpro/hicpro.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hicup/hicup.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hicup/hicup.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hifiasm/hifiasm.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hifiasm/hifiasm.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hisat2/hisat2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hisat2/hisat2.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,16 +119,14 @@
                 "suffix": "%",
                 "scale": "YlGn",
             }
         }
         self.general_stats_addcols(self.hisat2_data, headers)
 
     def hisat2_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         # Split the data into SE and PE
         sedata = {}
         pedata = {}
         for s_name, data in self.hisat2_data.items():
             if "paired_total" in data:
                 # Save half 'pairs' of mate counts
                 m_keys = ["unpaired_total", "unpaired_aligned_none", "unpaired_aligned_one", "unpaired_aligned_multi"]
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/homer/findpeaks.py` & `multiqc_sgr-1.22.post0/multiqc/modules/homer/findpeaks.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/homer/homer.py` & `multiqc_sgr-1.22.post0/multiqc/modules/homer/homer.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/homer/tagdirectory.py` & `multiqc_sgr-1.22.post0/multiqc/modules/homer/tagdirectory.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,15 @@
         """Make the petagRestrictionDistribution plot"""
 
         pconfig = {
             "id": "homer-petag-restriction-dist",
             "title": "HOMER: Restriction Distribution",
             "ylab": "Reads",
             "xlab": "Distance from cut site (bp)",
+            "tt_label": "<b>{point.x} bp</b>: {point.y} reads",
             "data_labels": [{"name": "Number of Tags"}, {"name": "Percenatge"}],
         }
         datasets = [self.tagdir_data["restriction"], self.tagdir_data["restriction_norm"]]
 
         return linegraph.plot(datasets, pconfig)
 
     def length_dist_chart(self):
@@ -404,14 +405,15 @@
 
         pconfig = {
             "id": "homer-tag-length-dist",
             "cpswitch": True,
             "title": "HOMER: Tag Length Distribution",
             "ylab": "Fraction of Tags",
             "xlab": "Tag Length (bp)",
+            "tt_label": "<b>{point.x} bp</b>: {point.y}",
         }
         return linegraph.plot(self.tagdir_data["length"], pconfig)
 
     def gc_content_plot(self):
         """Create the HTML for the Homer GC content plot"""
 
         pconfig = {
@@ -467,13 +469,12 @@
                 except ValueError:
                     pass
         pconfig = {
             "id": "homer-freq-distribution",
             "title": "HOMER: Frequency Distribution",
             "ylab": "Fraction of Reads",
             "xlab": "Log10(Distance between regions)",
-            "data_labels": ["Reads", "Percent"],
             "smooth_points": 500,
             "smooth_points_sumcounts": False,
             "yLog": True,
         }
         return linegraph.plot(pdata, pconfig)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/hops/hops.py` & `multiqc_sgr-1.22.post0/multiqc/modules/hops/hops.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             "square": False,
             "colstops": [
                 [1, "#ededed"],
                 [2, "#FFFFC5"],
                 [3, "#F2B26C"],
                 [4, "#AD2A2B"],
             ],
-            "decimalPlaces": 0,
+            "tt_decimals": 0,
             "legend": True,
             "datalabels": False,
             "xcats_samples": False,
         }
 
         extra_warning = ""
         if len(self.hops_data) > 20:
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/htseq/htseq.py` & `multiqc_sgr-1.22.post0/multiqc/modules/htseq/htseq.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/humid/clusters.py` & `multiqc_sgr-1.22.post0/multiqc/modules/humid/clusters.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/humid/counts.py` & `multiqc_sgr-1.22.post0/multiqc/modules/humid/counts.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/humid/humid.py` & `multiqc_sgr-1.22.post0/multiqc/modules/humid/humid.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/humid/neighbours.py` & `multiqc_sgr-1.22.post0/multiqc/modules/humid/neighbours.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/humid/stats.py` & `multiqc_sgr-1.22.post0/multiqc/modules/humid/stats.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/interop/interop.py` & `multiqc_sgr-1.22.post0/multiqc/modules/interop/interop.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/isoseq/isoseq.py` & `multiqc_sgr-1.22.post0/multiqc/modules/isoseq/isoseq.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/ivar/ivar.py` & `multiqc_sgr-1.22.post0/multiqc/modules/ivar/ivar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC module to parse output files from iVar """
 
 
 import logging
 import re
 
 from multiqc import config
@@ -159,15 +157,15 @@
         if len(final_ycats) == len(final_data):
             log.error(f"Number of samples and primers do not match: {len(final_ycats)} vs {len(final_data)}")
 
         if self.ivar_primers is not None:
             pconfig = {
                 "id": "ivar-primer-count-heatmap",
                 "title": "iVar: Number of primers found for each sample",
-                "decimalPlaces": 0,
+                "tt_decimals": 0,
                 "square": False,
                 "xcats_samples": False,
             }
 
             self.add_section(
                 name="iVar Primer Counts",
                 anchor="ivar-primers-heatmap",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/jcvi/jcvi.py` & `multiqc_sgr-1.22.post0/multiqc/modules/jcvi/jcvi.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,20 +295,20 @@
         return bargraph.plot(self.jcvi, keys, plot_config)
 
     def jcvi_linegraph_feature_length(self):
         plot_config = {
             "id": "jcvi_feature_length_plot",
             "title": "JCVI: Feature length repartition",
             "ylab": "# Genes",
-            "xlab": "Gene length (bp)",
-            "xDecimals": False,
+            "xlab": "Gene length",
+            "xsuffix": "bp",
             "data_labels": [
-                {"name": "Genes", "ylab": "# Genes", "xlab": "Gene length (bp)"},
-                {"name": "Exons", "ylab": "# Exons", "xlab": "Exon length (bp)"},
-                {"name": "Introns", "ylab": "# Introns", "xlab": "Intron length (bp)"},
+                {"name": "Genes", "ylab": "# Genes", "xlab": "Gene length"},
+                {"name": "Exons", "ylab": "# Exons", "xlab": "Exon length"},
+                {"name": "Introns", "ylab": "# Introns", "xlab": "Intron length"},
             ],
         }
 
         genes_plot_data = {x: self.jcvi[x]["gene_length"] for x in self.jcvi if "gene_length" in self.jcvi[x]}
         exon_plot_data = {x: self.jcvi[x]["exon_length"] for x in self.jcvi if "exon_length" in self.jcvi[x]}
         intron_plot_data = {x: self.jcvi[x]["intron_length"] for x in self.jcvi if "intron_length" in self.jcvi[x]}
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/jellyfish/jellyfish.py` & `multiqc_sgr-1.22.post0/multiqc/modules/jellyfish/jellyfish.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/kaiju/kaiju.py` & `multiqc_sgr-1.22.post0/multiqc/modules/kaiju/kaiju.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/kallisto/kallisto.py` & `multiqc_sgr-1.22.post0/multiqc/modules/kallisto/kallisto.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,14 @@
                 "modify": lambda x: x * config.read_count_multiplier,
                 "shared_key": "read_count",
             },
         }
         self.general_stats_addcols(self.kallisto_data, headers)
 
     def kallisto_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "pseudoaligned_reads": {"color": "#437bb1", "name": "Pseudoaligned"},
             "not_pseudoaligned_reads": {"color": "#b1084c", "name": "Not aligned"},
         }
 
         # Config for the plot
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/kat/kat.py` & `multiqc_sgr-1.22.post0/multiqc/modules/kat/kat.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/kraken/kraken.py` & `multiqc_sgr-1.22.post0/multiqc/modules/kraken/kraken.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/leehom/leehom.py` & `multiqc_sgr-1.22.post0/multiqc/modules/leehom/leehom.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/librarian/librarian.py` & `multiqc_sgr-1.22.post0/multiqc/modules/librarian/librarian.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             "yTitle": "Sample name",
             "min": 0,
             "max": 100,
             "square": False,
             "xcats_samples": False,
             "ycats_samples": True,
             "colstops": [[0, "#FFFFFF"], [1, "#FF0000"]],
-            "decimalPlaces": 0,
+            "tt_decimals": 0,
         }
 
         self.add_section(
             name="Library Type Prediction",
             anchor="librarian-library-type",
             description="""
                 For each projected test library, the location on the Compositions/Probability Map is determined.
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/lima/lima.py` & `multiqc_sgr-1.22.post0/multiqc/modules/lima/lima.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/longranger/longranger.py` & `multiqc_sgr-1.22.post0/multiqc/modules/longranger/longranger.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/macs2/macs2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/macs2/macs2.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/malt/malt.py` & `multiqc_sgr-1.22.post0/multiqc/modules/malt/malt.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/mapdamage/mapdamage.py` & `multiqc_sgr-1.22.post0/multiqc/modules/mapdamage/mapdamage.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/megahit/megahit.py` & `multiqc_sgr-1.22.post0/multiqc/modules/megahit/megahit.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/metaphlan/metaphlan.py` & `multiqc_sgr-1.22.post0/multiqc/modules/metaphlan/metaphlan.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/methylqa/methylqa.py` & `multiqc_sgr-1.22.post0/multiqc/modules/methylqa/methylqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,14 @@
         """Take the parsed stats from the methylQA report and add it to the
         basic stats table at the top of the report"""
 
         headers = {"coverage": {"title": "Fold Coverage", "min": 0, "suffix": "X", "scale": "YlGn"}}
         self.general_stats_addcols(self.methylqa_data, headers)
 
     def methylqa_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         if len(self.methylqa_coverage_counts) == 0:
             return '<div class="alert alert-danger">No histogram data found.</div>'
 
         pconfig = {
             "id": "methylqa_coverage",
             "title": "methylQA: CpG Coverage",
             "categories": True,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/minionqc/minionqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/minionqc/minionqc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/mirtop/mirtop.py` & `multiqc_sgr-1.22.post0/multiqc/modules/mirtop/mirtop.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/mirtrace/mirtrace.py` & `multiqc_sgr-1.22.post0/multiqc/modules/mirtrace/mirtrace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC module to parse output files from miRTrace """
 
 
 import json
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/mosdepth/mosdepth.py` & `multiqc_sgr-1.22.post0/multiqc/modules/mosdepth/mosdepth.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,17 +306,16 @@
                 xy_keys = {
                     "x": {"name": self.cfg.get("xchr") or "Chromosome X"},
                     "y": {"name": self.cfg.get("xchr") or "Chromosome Y"},
                 }
                 pconfig = {
                     "id": "mosdepth-xy-coverage-plot",
                     "title": "Mosdepth: chrXY coverage",
-                    "ylab": "Percent of X+Y coverage",
-                    "cpswitch_counts_label": "Coverage",
-                    "cpswitch_percent_label": "Percent of X+Y coverage",
+                    "ylab": "Coverage",
+                    "ysuffix": "X",
                     "cpswitch_c_active": False,
                 }
                 self.add_section(
                     name="XY coverage",
                     anchor="mosdepth-xy-coverage",
                     plot=bargraph.plot(xy_cov, xy_keys, pconfig),
                 )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/motus/motus.py` & `multiqc_sgr-1.22.post0/multiqc/modules/motus/motus.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
     def motus_filtering_bargraph_plot(self):
         """mOTUs read counts for general stats"""
         common = {
             "min": 0,
             "modify": lambda x: float(x) * config.read_count_multiplier,
             "suffix": f"{config.read_count_prefix} reads",
-            "decimalPlaces": 0,
+            "tt_decimals": 0,
             "shared_key": "read_count",
         }
         cats = {
             "Number of reads after filtering": dict(common, **{"name": "Reads after mapping"}),
             "Discarded reads": dict(common, **{"name": "Unmapped reads"}),
         }
 
@@ -185,15 +185,15 @@
 
     def motus_mapping_bargraph_plot(self):
         """mOTUs bar chart of insert types"""
         common = {
             "min": 0,
             "modify": lambda x: float(x) * config.read_count_multiplier,
             "suffix": f"{config.read_count_prefix} reads",
-            "decimalPlaces": 0,
+            "tt_decimals": 0,
             "shared_key": "read_count",
         }
         cats = {
             "Unique mappers": dict(common, **{"name": "Unique mapped inserts", "color": "#3aba5e"}),
             "Multiple mappers": dict(common, **{"name": "Multiple mapped inserts", "color": "#ebbe59"}),
             "Ignored multiple mapper without unique hit": dict(
                 common, **{"name": "Ignored multi-mapped inserts", "color": "#cf5565"}
@@ -215,15 +215,15 @@
             ),
         )
 
     def motus_motus_bargraph_plot(self):
         """mOTUs bar chart of mOTU types"""
         common = {
             "min": 0,
-            "decimalPlaces": 0,
+            "tt_decimals": 0,
         }
         cats = {
             "Number of ref-mOTUs": dict(common, **{"name": "Known mOTUs"}),
             "Number of meta-mOTUs": dict(common, **{"name": "(Unknown) Metagenome mOTUs"}),
             "Number of ext-mOTUs": dict(common, **{"name": "(Unknown) MAG mOTUs"}),
         }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/mtnucratio/mtnucratio.py` & `multiqc_sgr-1.22.post0/multiqc/modules/mtnucratio/mtnucratio.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/multivcfanalyzer/multivcfanalyzer.py` & `multiqc_sgr-1.22.post0/multiqc/modules/multivcfanalyzer/multivcfanalyzer.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/nanostat/nanostat.py` & `multiqc_sgr-1.22.post0/multiqc/modules/nanostat/nanostat.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,16 +280,14 @@
         self.add_section(
             name="Summary Statistics",
             anchor=f"nanostat_{stat_type.replace(' ', '_')}_stats",
             plot=table.plot(self.nanostat_data, headers, table_config),
         )
 
     def reads_by_quality_plot(self):
-        """Make the HighCharts HTML to plot the reads by quality"""
-
         def _get_total_reads(data_dict):
             stat_type = self._stat_types[0]
             for stat_type in self._stat_types:
                 total_key = f"Number of reads_{stat_type}"
                 if total_key in data_dict:
                     return data_dict[total_key], stat_type
             return None, None
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/nextclade/nextclade.py` & `multiqc_sgr-1.22.post0/multiqc/modules/nextclade/nextclade.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/ngsderive/ngsderive.py` & `multiqc_sgr-1.22.post0/multiqc/modules/ngsderive/ngsderive.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,15 @@
         # Config for the plot
         pconfig = {
             "id": "ngsderive_strandedness_plot",
             "title": "ngsderive: Strandedness",
             "ylab": "% Read Evidence",
             "ymin": 0,
             "ymax": 100,
-            "tt_percentages": True,
-            "ylab_format": "{value}%",
+            "ysuffix": "%",
             "cpswitch": False,
         }
 
         self.add_section(
             name="Strandedness",
             anchor="ngsderive-strandedness",
             description="""Predicted strandedness provided by ngsderive. For more information, please see
@@ -318,16 +317,22 @@
 
         # Config for the plot
         pconfig = {
             "id": "ngsderive_readlen_plot",
             "title": "ngsderive: Read Length",
             "xlab": "Read Length",
             "ylab": "% Evidence for Read Length",
+            "xsuffix": " bp",
             "data_labels": [
-                {"name": "Percentages", "ylab": "% Evidence for Read Length"},
+                {
+                    "name": "Percentages",
+                    "ylab": "% Evidence for Read Length",
+                    "ymax": 100,
+                    "y_decimals": 2,
+                },
                 {"name": "Counts", "ylab": "Number of reads"},
             ],
         }
 
         self.add_section(
             name="Read length",
             anchor="ngsderive-readlen",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/nonpareil/nonpareil.py` & `multiqc_sgr-1.22.post0/multiqc/modules/nonpareil/nonpareil.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,20 +310,18 @@
             """,
             plot=table.plot(self.data_by_sample, headers, pconfig),
         )
 
     def nonpareil_redundancy_plot(self):
         """Make the redundancy plot for nonpareil"""
 
-        esconfig = {
-            "dashStyle": "Dash",
-            "lineWidth": 2,
-            "marker": {"enabled": False},
-            "enableMouseTracking": True,
-            "showInLegend": False,
+        extra_series_config = {
+            "dash": "dash",
+            "line": {"width": 2},
+            "showlegend": False,
         }
 
         data_colors_default = mqc_colour.mqc_colour_scale().get_colours(self.plot_colours)
         data_colors = {
             s_name: data.get("nonpareil_col", data_colors_default.pop(0))
             for s_name, data in self.data_by_sample.items()
         }
@@ -342,15 +340,15 @@
                 if dataset["name"] == "Observed":
                     data_plot[idx][s_name] = data["nonpareil_observed"]
                 elif dataset["name"] == "Model" and data["nonpareil_has.model"]:
                     data_plot[idx][s_name] = data["nonpareil_model"]
                 elif dataset["name"] == "Combined":
                     data_plot[idx][s_name] = data["nonpareil_observed"]
                     if data["nonpareil_has.model"]:
-                        extra_series[idx].append(dict(esconfig))
+                        extra_series[idx].append(dict(extra_series_config))
                         extra_series[idx][-1]["name"] = s_name
                         extra_series[idx][-1]["data"] = [[x, y] for x, y in data["nonpareil_model"].items()]
                         extra_series[idx][-1]["color"] = data_colors[s_name]
 
         pconfig = {
             "id": "nonpareil-redundancy-plot",
             "colors": data_colors,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/odgi/odgi.py` & `multiqc_sgr-1.22.post0/multiqc/modules/odgi/odgi.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/optitype/optitype.py` & `multiqc_sgr-1.22.post0/multiqc/modules/optitype/optitype.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/pangolin/pangolin.py` & `multiqc_sgr-1.22.post0/multiqc/modules/pangolin/pangolin.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/pbmarkdup/pbmarkdup.py` & `multiqc_sgr-1.22.post0/multiqc/modules/pbmarkdup/pbmarkdup.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/peddy/peddy.py` & `multiqc_sgr-1.22.post0/multiqc/modules/peddy/peddy.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/phantompeakqualtools/phantompeakqualtools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/phantompeakqualtools/phantompeakqualtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC module to parse output from phantompeakqualtools """
 
 
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/AlignmentSummaryMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/AlignmentSummaryMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/BaseDistributionByCycleMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/BaseDistributionByCycleMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/CrosscheckFingerprints.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/CrosscheckFingerprints.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,45 +37,46 @@
     does pairwise comparisons between samples at the level selected by `--CROSSCHECK_BY`.
     """
 
     row_by_number = dict()
     n_found_reports = 0
 
     # Go through logs and find Metrics
+    row_number = 0
     for f in module.find_log_files("picard/crosscheckfingerprints", filehandles=True):
         # Parse an individual CrosscheckFingerprints Report
         (metrics, comments) = _take_till(f["f"], lambda line: line.startswith("#") or line == "\n")
         header = next(metrics).rstrip("\n").split("\t")
         if "LEFT_GROUP_VALUE" not in header:
             # Not a CrosscheckFingerprints Report
             continue
         # Parse out the tumor awareness option and the lod threshold setting if possible
         tumor_awareness, lod_threshold = _parse_cli(comments[1])
         reader: DictReader = DictReader(metrics, fieldnames=header, delimiter="\t")
-        lines = [
-            (i, row)
-            for i, row in enumerate(reader)
-            if not module.is_ignore_sample(row["LEFT_SAMPLE"]) and not module.is_ignore_sample(row["RIGHT_SAMPLE"])
-        ]
+        lines = []
+        for row in reader:
+            if not module.is_ignore_sample(row["LEFT_SAMPLE"]) and not module.is_ignore_sample(row["RIGHT_SAMPLE"]):
+                lines.append((row_number, row))
+            row_number += 1
         if not lines:
             continue
         n_found_reports += 1
-        for i, row in lines:
+        for row_number, row in lines:
             # Clean the sample names
             row["LEFT_SAMPLE"] = module.clean_s_name(row["LEFT_SAMPLE"], f)
             row["LEFT_GROUP_VALUE"] = module.clean_s_name(row["LEFT_GROUP_VALUE"], f)
             row["RIGHT_SAMPLE"] = module.clean_s_name(row["RIGHT_SAMPLE"], f)
             row["RIGHT_GROUP_VALUE"] = module.clean_s_name(row["RIGHT_GROUP_VALUE"], f)
 
             row["RESULT"] = row["RESULT"].capitalize().replace("_", " ")
 
             # Set the cli options of interest for this file
             row["LOD_THRESHOLD"] = lod_threshold
             row["TUMOR_AWARENESS"] = tumor_awareness
-            row_by_number[i] = row
+            row_by_number[row_number] = row
 
             try:
                 row["LOD_SCORE"] = float(row["LOD_SCORE"])
             except ValueError:
                 row["LOD_SCORE"] = None
 
             # Add BEST_MATCH and BEST_MATCH_LOD if the result is unexpected or inconclusive
@@ -90,19 +91,14 @@
 
             module.add_data_source(f, section="CrosscheckFingerprints")
 
     # Only add sections if we found data
     if n_found_reports == 0:
         return 0
 
-    # Sort the data by the left sample, then right sample
-    row_by_number = OrderedDict(
-        sorted(row_by_number.items(), key=lambda x: (x[1]["LEFT_SAMPLE"], x[1]["RIGHT_SAMPLE"]))
-    )
-
     # Superfluous function call to confirm that it is used in this module
     # Replace None with actual version if it is available
     module.add_software_version(None)
 
     # Write data to file
     module.write_data_file(row_by_number, f"{module.anchor}_crosscheckfingerprints")
 
@@ -162,15 +158,15 @@
             dict(sorted(status_by_sample.items(), key=lambda kv: _order_status(kv[1]["Crosschecks"]))),
             sample_table_headers,
             pconfig={
                 "namespace": module.name,
                 "id": f"{module.anchor}-crosscheckfingerprints-sample-table",
                 "title": f"{module.name}: Crosscheck Fingerprints: Samples",
                 "no_violin": True,
-                "sortRows": False,
+                "sort_rows": False,
             },
         ),
     )
     for h in sample_table_headers.values():
         h["hidden"] = True
     module.general_stats_addcols(
         status_by_sample,
@@ -227,15 +223,15 @@
             pconfig={
                 "namespace": module.name,
                 "id": f"{module.anchor}-crosscheckfingerprints-table",
                 "title": f"{module.name}: Crosscheck Fingerprints",
                 "save_file": True,
                 "col1_header": "ID",
                 "no_violin": True,
-                "sortRows": False,
+                "sort_rows": False,
             },
         ),
     )
 
     return n_found_reports
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/ExtractIlluminaBarcodes.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/ExtractIlluminaBarcodes.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/GcBiasMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/GcBiasMetrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,20 +115,19 @@
         pconfig = {
             "id": f"{module.anchor}_gcbias_plot",
             "title": f"{module.name}: GC Coverage Bias",
             "ylab": "Normalized Coverage",
             "xlab": "% GC",
             "xmin": 0,
             "xmax": 100,
-            "xDecimals": False,
             "ymin": 0,
-            "yCeiling": 10,
+            "y_clipmax": 10,
             "tt_label": "<b>{point.x} %GC</b>: {point.y:.2f}",
-            "yPlotLines": [
-                {"value": 1, "color": "#999999", "width": 2, "dashStyle": "LongDash"},
+            "y_lines": [
+                {"value": 1, "color": "#999999", "width": 2, "dash": "longdash"},
             ],
         }
         module.add_section(
             name="GC Coverage Bias",
             anchor=f"{module.anchor}-gcbias",
             description="This plot shows bias in coverage across regions of the genome with varying GC content."
             " A perfect library would be a flat line at <code>y = 1</code>.",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/HsMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/HsMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/IlluminaBasecallingMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/IlluminaBasecallingMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/IlluminaLaneMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/IlluminaLaneMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/InsertSizeMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/InsertSizeMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/MarkDuplicates.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/MarkDuplicates.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/MarkIlluminaAdapters.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/MarkIlluminaAdapters.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/OxoGMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/OxoGMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/QualityByCycleMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityByCycleMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/QualityScoreDistributionMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityScoreDistributionMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/QualityYieldMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/QualityYieldMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/RnaSeqMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/RnaSeqMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/RrbsSummaryMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/RrbsSummaryMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/TargetedPcrMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/TargetedPcrMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/ValidateSamFile.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/ValidateSamFile.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/VariantCallingMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/VariantCallingMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/WgsMetrics.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/WgsMetrics.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/picard.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/picard.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/picard/util.py` & `multiqc_sgr-1.22.post0/multiqc/modules/picard/util.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/porechop/porechop.py` & `multiqc_sgr-1.22.post0/multiqc/modules/porechop/porechop.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/preseq/preseq.py` & `multiqc_sgr-1.22.post0/multiqc/modules/preseq/preseq.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,21 +156,20 @@
             pconfig["xmax"] = max_x
             description += "<p>Note that the x-axis is trimmed at the point where all the datasets \
                 show 80% of their maximum y-value, to avoid ridiculous scales.</p>"
 
         # Plot perfect library as dashed line
         pconfig["extra_series"].append(
             {
-                "name": "a perfect library where each read is unique",
+                "name": "A perfect library where each read is unique",
                 "data": [[0, 0], [max_yx, max_y]],
-                "dashStyle": "Dash",
-                "lineWidth": 1,
+                "dash": "dash",
+                "line": {"width": 1},
                 "color": "#000000",
-                "marker": {"enabled": False},
-                "showInLegend": False,
+                "showlegend": False,
             }
         )
 
         self.add_section(name=name, description=description, anchor=section_id, plot=linegraph.plot(data, pconfig))
 
     def _parse_real_counts(self, sample_names):
         real_counts_file_raw = None
@@ -365,20 +364,18 @@
 
     series = []
     for si, sn in enumerate(sorted(data.keys())):
         if sn in xs_by_sample:
             x = float(xs_by_sample[sn])
             point = {
                 "color": scale.get_colour(si),
-                "showInLegend": False,
+                "showlegend": False,
                 "marker": {
-                    "enabled": True,
                     "symbol": "diamond",
-                    "lineColor": "black",
-                    "lineWidth": 1,
+                    "line": {"color": "black", "width": 1},
                 },
             }
             if sn in yx_by_sample:
                 y = float(yx_by_sample[sn])
                 point["data"] = [[x, y]]
                 point["name"] = f"{sn}: actual read count vs. deduplicated read count (externally calculated)"
                 series.append(point)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/prinseqplusplus/prinseqplusplus.py` & `multiqc_sgr-1.22.post0/multiqc/modules/prinseqplusplus/prinseqplusplus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import beeswarm
+from multiqc.plots import violin
 
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(BaseMultiqcModule):
     def __init__(self):
         # Initialise the parent object
@@ -36,15 +36,15 @@
         # Replace None with actual version if it is available
         self.add_software_version(None)
 
         # Write data to file
         self.write_data_file(self.prinseqplusplus_data, "prinseqplusplus")
 
         self.prinseqplusplus_general_stats()
-        self.prinseqplusplus_beeswarm_plot()
+        self.prinseqplusplus_violin_plot()
 
     def parse_logs(self, f):
         """Parsing Logs."""
         s_name = f["s_name"]
         if self.prinseqplusplus_data.get(s_name) is not None:
             log.warn(f"Duplicate sample name found! Overwriting: {s_name}")
 
@@ -91,16 +91,16 @@
                     "scale": "Oranges",
                     "shared_key": "read_count",
                     "modify": lambda x: x * config.read_count_multiplier,
                 }
             },
         )
 
-    def prinseqplusplus_beeswarm_plot(self):
-        """Beeswarm plot of all possible filtering results"""
+    def prinseqplusplus_violin_plot(self):
+        """Violin plot of all possible filtering results"""
         # This would be nicer as a stacked-bar plot, but as we don't have
         # the total read count it doesn't really make sense.
 
         reads = {
             "min": 0,
             "modify": lambda x: float(x) * config.read_count_multiplier,
             "suffix": config.read_count_prefix,
@@ -120,16 +120,16 @@
             "lc_dust": dict(reads, title="lc_dust"),
         }
 
         self.add_section(
             name="Filtered Reads",
             anchor="prinseqplusplus-filtered-reads",
             description="Shows the number of reads removed by the various PRINSEQ++ filter options",
-            plot=beeswarm.plot(
+            plot=violin.plot(
                 self.prinseqplusplus_data,
                 headers,
                 {
-                    "id": "prinseplusplus-filtered-reads-beeswarm",
+                    "id": "prinseplusplus-filtered-reads-violin",
                     "title": "PRINSEQ++: Filtered Reads",
                 },
             ),
         )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/profile_runtime.py` & `multiqc_sgr-1.22.post0/multiqc/modules/profile_runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-#!/usr/bin/env python
-
 """ Super Special-Case MultiQC module to produce report section on MultiQC run time """
 
-
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule
 from multiqc.plots import bargraph
 from multiqc.utils import report
 
 # Initialise the logger
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/prokka/prokka.py` & `multiqc_sgr-1.22.post0/multiqc/modules/prokka/prokka.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/purple/purple.py` & `multiqc_sgr-1.22.post0/multiqc/modules/purple/purple.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/pychopper/pychopper.py` & `multiqc_sgr-1.22.post0/multiqc/modules/pychopper/pychopper.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/pycoqc/pycoqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/pycoqc/pycoqc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qc3C/qc3C.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qc3C/qc3C.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,29 +652,28 @@
         median_lines = []
         for smpl in self.qc3c_data["bam"]:
             median_lines.append(
                 {
                     "value": self.qc3c_data["bam"][smpl]["b_obs_insert_median"],
                     "color": "#D8E2DC",
                     "width": 2,
-                    "dashStyle": "ShortDashDot",
+                    "dash": "dashdot",
                 }
             )
 
         config = {
             "id": "qc3C_bam_fragment_histogram",
             "title": "qc3C: BAM mode distribution of pair separation",
             "namespace": "qc3C",
             "cpswitch_counts_label": "Density",
             "logswitch": True,
             "logswitch_active": True,
             "logswitch_label": "Log10 [Density]",
-            "xLog": True,
-            # 'yLog': True,
-            "xPlotLines": median_lines,
+            "xlog": True,
+            "x_lines": median_lines,
             "xlab": "Log10 [Separation]",
             "ylab": "Density",
             "tt_label": "x:{point.x:.0f} bp, y:{point.y:.8f}",
         }
 
         data = {}
         for smpl in self.qc3c_data["bam"]:
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qorts/qorts.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qorts/qorts.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,14 @@
             Outliers in these plots can indicate biological variations or the presence of large mapping problems.
             They may also suggest the presence of large, highly-expressed, unannotated transcripts or genes.
             """,
             plot=bargraph.plot(self.qorts_data, cats, pconfig),
         )
 
     def qorts_splice_loci_barplot(self):
-        """Make the HighCharts HTML to plot the qorts splice loci"""
         # Specify the order of the different possible categories
         keys = [
             "SpliceLoci_Known_ManyReads",
             "SpliceLoci_Known_FewReads",
             "SpliceLoci_Known_NoReads",
             "SpliceLoci_Novel_ManyReads",
             "SpliceLoci_Novel_FewReads",
@@ -209,15 +208,14 @@
             abnormalities observed in the other plots are of sufficient severity to impact splice junction mapping and
             thus potentially compromise such analyses.
             """,
             plot=bargraph.plot(self.qorts_data, cats, pconfig),
         )
 
     def qorts_splice_events_barplot(self):
-        """Make the HighCharts HTML to plot the qorts splice events"""
         # Specify the order of the different possible categories
         keys = [
             "SpliceEvents_KnownLociWithManyReads",
             "SpliceEvents_KnownLociWithFewReads",
             "SpliceEvents_NovelLociWithManyReads",
             "SpliceEvents_NovelLociWithFewReads",
         ]
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qualimap/QM_BamQC.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qualimap/QM_BamQC.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 def report_sections(self):
     """Add results from Qualimap BamQC parsing to the report"""
     # Append to self.sections list
 
     if len(self.qualimap_bamqc_coverage_hist) > 0:
         # Chew back on histogram to prevent long flat tail
         # (find a sensible max x - lose 1% of longest tail)
-        max_x = 0
+        max_x = 20
         total_bases_by_sample = dict()
         for s_name, d in self.qualimap_bamqc_coverage_hist.items():
             total_bases_by_sample[s_name] = sum(d.values())
             cumulative = 0
             for count in sorted(d.keys(), reverse=True):
                 cumulative += d[count]
                 if cumulative / total_bases_by_sample[s_name] > 0.01:
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qualimap/QM_RNASeq.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qualimap/QM_RNASeq.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qualimap/__init__.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qualimap/__init__.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/qualimap/qualimap.py` & `multiqc_sgr-1.22.post0/multiqc/modules/qualimap/qualimap.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/quast/quast.py` & `multiqc_sgr-1.22.post0/multiqc/modules/quast/quast.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rna_seqc/rna_seqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rna_seqc/rna_seqc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ MultiQC module to parse output from RNA-SeQC """
 
 
 import logging
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, beeswarm, heatmap, linegraph
+from multiqc.plots import bargraph, violin, heatmap, linegraph
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(BaseMultiqcModule):
     def __init__(self):
@@ -319,15 +319,15 @@
                 name="Gene Body Coverage",
                 anchor="rseqc-rna_seqc_mean_coverage",
                 helptext="The metrics are calculated across the transcripts with tiered expression levels.",
                 plot=linegraph.plot(data, pconfig),
             )
 
     def bam_statplot(self):
-        pconfig = {"id": "rna_seqc_bam_stat_beeswarm", "title": "RNA-SeQC: Read metrics"}
+        pconfig = {"id": "rna_seqc_bam_stat_violin", "title": "RNA-SeQC: Read metrics"}
         columns = [
             "Total Read Number",
             "Alternative Alignments",
             "Chimeric Reads",
             "Duplicate Reads",
             "End 1 Mapped Reads",
             "End 2 Mapped Reads",
@@ -355,9 +355,9 @@
             }
 
         self.add_section(
             name="Read Counts",
             anchor="rna_seqc_bam_stat",
             description=f"Number of reads ({config.read_count_desc}) falling into different categories.",
             helptext="Note that many of these statistics are only available from RNA-SeQC v2.x",
-            plot=beeswarm.plot(self.rna_seqc_metrics, keys, pconfig),
+            plot=violin.plot(self.rna_seqc_metrics, keys, pconfig),
         )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rockhopper/rockhopper.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rockhopper/rockhopper.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rsem/rsem.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rsem/rsem.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/bam_stat.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/bam_stat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ MultiQC submodule to parse output from RSeQC bam_stat.py
 http://rseqc.sourceforge.net/#bam-stat-py """
 
 import logging
 import re
 
-from multiqc.plots import beeswarm
+from multiqc.plots import violin
 from multiqc.utils import config
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 def parse_reports(self):
@@ -100,15 +100,15 @@
     pconfig = {
         "id": "rseqc_bam_stat",
         "title": "RSeQC: Bam Stat",
     }
     defaults = {
         "min": 0,
         "shared_key": "read_count",
-        "decimalPlaces": 2,
+        "tt_decimals": 2,
         "modify": lambda x: x * config.read_count_multiplier,
         "suffix": config.read_count_prefix,
     }
     keys = dict()
     keys["total_records"] = dict(defaults, **{"title": "Total records"})
     keys["qc_failed"] = dict(defaults, **{"title": "QC failed"})
     keys["optical_pcr_duplicate"] = dict(defaults, **{"title": "Duplicates", "description": "Optical/PCR duplicate"})
@@ -133,12 +133,12 @@
             defaults, **{"title": "Different chrom", "description": "Proper-paired reads map to different chrom"}
         )
 
     self.add_section(
         name="Bam Stat",
         anchor="rseqc-bam_stat",
         description="All numbers reported in millions.",
-        plot=beeswarm.plot(self.bam_stat_data, keys, pconfig),
+        plot=violin.plot(self.bam_stat_data, keys, pconfig),
     )
 
     # Return number of samples found
     return len(self.bam_stat_data)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/gene_body_coverage.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/gene_body_coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     # Make a normalised coverage for plotting using the formula (cov - min_cov) / (max_cov - min_cov)
     for s_name in self.gene_body_cov_hist_counts:
         self.gene_body_cov_hist_percent[s_name] = dict()
         # min_cov and max_cov are required to compute the normalized coverage
         min_cov = min(self.gene_body_cov_hist_counts[s_name].values())
         max_cov = max(self.gene_body_cov_hist_counts[s_name].values())
         for k, v in self.gene_body_cov_hist_counts[s_name].items():
-            self.gene_body_cov_hist_percent[s_name][k] = (v - min_cov) / (max_cov - min_cov)
+            self.gene_body_cov_hist_percent[s_name][k] = (v - min_cov) / (max_cov - min_cov) * 100.0
 
     # Add line graph to section
     pconfig = {
         "id": "rseqc_gene_body_coverage_plot",
         "title": "RSeQC: Gene Body Coverage",
         "ylab": "Coverage",
         "xlab": "Gene Body Percentile (5' -> 3')",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/infer_experiment.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/infer_experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,15 @@
     # Config for the plot
     pconfig = {
         "id": "rseqc_infer_experiment_plot",
         "title": "RSeQC: Infer experiment",
         "ylab": "% Tags",
         "ymin": 0,
         "ymax": 100,
-        "tt_percentages": False,
-        "ylab_format": "{value}%",
+        "ysuffix": "%",
         "cpswitch": False,
     }
 
     self.add_section(
         name="Infer experiment",
         anchor="rseqc-infer_experiment",
         description='<a href="http://rseqc.sourceforge.net/#infer-experiment-py" target="_blank">Infer experiment</a>'
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/inner_distance.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/inner_distance.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/junction_annotation.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/junction_annotation.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/junction_saturation.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/junction_saturation.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,14 @@
         "ylab": "Number of Junctions",
         "ymin": 0,
         "xlab": "Percent of reads",
         "xmin": 0,
         "xmax": 100,
         "tt_label": "<strong>{point.x}% of reads</strong>: {point.y:.2f}",
         "data_labels": [{"name": "All Junctions"}, {"name": "Known Junctions"}, {"name": "Novel Junctions"}],
-        "cursor": "pointer",
-        "click_func": "single_sample_plot",
     }
     self.add_section(
         name="Junction Saturation",
         anchor="rseqc-junction_saturation",
         description="""<a href="http://rseqc.sourceforge.net/#junction-saturation-py" target="_blank">Junction Saturation</a>
             counts the number of known splicing junctions that are observed
             in each dataset. If sequencing depth is sufficient, all (annotated) splice junctions should
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_distribution.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_distribution.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_duplication.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_duplication.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/read_gc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/read_gc.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/rseqc.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/rseqc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ MultiQC module to parse output from RSeQC """
 
 import logging
-import os
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
@@ -44,19 +43,14 @@
                 "junction_annotation",
                 "junction_saturation",
                 "infer_experiment",
                 "bam_stat",
                 "tin",
             ]
 
-        # Add self.js to be included in template
-        self.js = {
-            "assets/js/multiqc_rseqc.js": os.path.join(os.path.dirname(__file__), "assets", "js", "multiqc_rseqc.js")
-        }
-
         # Call submodule functions
         for sm in rseqc_sections:
             try:
                 # Import the submodule and call parse_reports()
                 #   Function returns number of parsed logs
                 module = __import__(f"multiqc.modules.rseqc.{sm}", fromlist=[""])
                 n[sm] = getattr(module, "parse_reports")(self)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/rseqc/tin.py` & `multiqc_sgr-1.22.post0/multiqc/modules/rseqc/tin.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/salmon/salmon.py` & `multiqc_sgr-1.22.post0/multiqc/modules/salmon/salmon.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sambamba/markdup.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sambamba/markdup.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sambamba/sambamba.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sambamba/sambamba.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samblaster/samblaster.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samblaster/samblaster.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/coverage.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/coverage.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/flagstat.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/flagstat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # coding: utf-8
 """ MultiQC submodule to parse output from Samtools flagstat """
 
 import logging
 import re
 
 from multiqc import config
-from multiqc.plots import beeswarm
+from multiqc.plots import violin
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class FlagstatReportMixin:
-    def parse_samtools_flagstats(self):
+    def parse_samtools_flagstat(self):
         """Find Samtools flagstat logs and parse their data"""
 
         self.samtools_flagstat = dict()
         for f in self.find_log_files("samtools/flagstat"):
             parsed_data = parse_single_report(f["f"])
             if len(parsed_data) > 0:
                 if f["s_name"] in self.samtools_flagstat:
@@ -34,15 +34,15 @@
         # Replace None with actual version if it is available
         self.add_software_version(None)
 
         # Write parsed report data to a file (restructure first)
         self.write_data_file(self.samtools_flagstat, "multiqc_samtools_flagstat")
 
         # General Stats Table
-        flagstats_headers = {
+        flagstat_headers = {
             "flagstat_total": {
                 "title": "Reads",
                 "description": f"Total reads in the bam file ({config.read_count_desc})",
                 "shared_key": "read_count",
                 "hidden": True,
             },
             "mapped_passed": {
@@ -56,69 +56,90 @@
                 "min": 0,
                 "max": 100,
                 "suffix": "%",
                 "scale": "RdYlGn",
                 "hidden": True,
             },
         }
-        self.general_stats_addcols(self.samtools_flagstat, flagstats_headers, namespace="flagstat")
+        self.general_stats_addcols(self.samtools_flagstat, flagstat_headers, namespace="flagstat")
 
-        # Make dot plot of counts
-        keys = {}
+        # Make a violin plot
         reads = {
-            "min": 0,
-            "modify": lambda x: float(x) * config.read_count_multiplier,
-            "suffix": config.read_count_prefix,
-            "decimalPlaces": 2,
             "shared_key": "read_count",
+            "modify": None,
+            "format": None,
+            "suffix": None,
         }
-        keys["flagstat_total"] = dict(reads, title="Total Reads")
-        keys["total_passed"] = dict(reads, title="Total Passed QC")
-        keys["mapped_passed"] = dict(reads, title="Mapped")
+        keys_counts = dict()
+        keys_counts["flagstat_total"] = dict(reads, title="Total Reads")
+        keys_counts["total_passed"] = dict(reads, title="Total Passed QC")
+        keys_counts["mapped_passed"] = dict(reads, title="Mapped")
 
         if any(v.get("secondary_passed") for v in self.samtools_flagstat.values()):
-            keys["secondary_passed"] = dict(reads, title="Secondary Alignments")
+            keys_counts["secondary_passed"] = dict(reads, title="Secondary Alignments")
 
         if any(v.get("supplementary_passed") for v in self.samtools_flagstat.values()):
-            keys["supplementary_passed"] = dict(reads, title="Supplementary Alignments")
+            keys_counts["supplementary_passed"] = dict(reads, title="Supplementary Alignments")
 
-        keys["duplicates_passed"] = dict(reads, title="Duplicates")
-        keys["paired in sequencing_passed"] = dict(reads, title="Paired in Sequencing")
-        keys["properly paired_passed"] = dict(reads, title="Properly Paired")
-        keys["with itself and mate mapped_passed"] = dict(
+        keys_counts["duplicates_passed"] = dict(reads, title="Duplicates")
+        keys_counts["paired in sequencing_passed"] = dict(reads, title="Paired in Sequencing")
+        keys_counts["properly paired_passed"] = dict(reads, title="Properly Paired")
+        keys_counts["with itself and mate mapped_passed"] = dict(
             reads, title="Self and mate mapped", description="Reads with itself and mate mapped"
         )
-        keys["singletons_passed"] = dict(reads, title="Singletons")
-        keys["with mate mapped to a different chr_passed"] = dict(
+        keys_counts["singletons_passed"] = dict(reads, title="Singletons")
+        keys_counts["with mate mapped to a different chr_passed"] = dict(
             reads, title="Mate mapped to diff chr", description="Mate mapped to different chromosome"
         )
-        keys["with mate mapped to a different chr (mapQ >= 5)_passed"] = dict(
+        keys_counts["with mate mapped to a different chr (mapQ >= 5)_passed"] = dict(
             reads, title="Diff chr (mapQ >= 5)", description="Mate mapped to different chromosome (mapQ >= 5)"
         )
 
+        data_pct = dict()
+        for sample, d in self.samtools_flagstat.items():
+            data_pct[sample] = dict()
+            total = d["flagstat_total"]
+            if total > 0:
+                for metric, cnt in d.items():
+                    data_pct[sample][f"{metric}_pct"] = cnt / total * 100
+        keys_pct = {
+            f"{metric}_pct": dict(
+                title=header["title"],
+                min=0,
+                max=100,
+                suffix="%",
+                shared_key=None,
+            )
+            for metric, header in keys_counts.items()
+        }
+
         self.add_section(
             name="Flagstat",
             anchor="samtools-flagstat",
-            description="This module parses the output from <code>samtools flagstat</code>. All numbers in millions.",
-            plot=beeswarm.plot(
-                self.samtools_flagstat,
-                keys,
-                {
+            description="This module parses the output from <code>samtools flagstat</code>",
+            plot=violin.plot(
+                [self.samtools_flagstat, data_pct],
+                headers=[keys_counts, keys_pct],
+                pconfig={
                     "id": "samtools-flagstat-dp",
-                    "title": "Samtools flagstat: Read Counts",
+                    "title": "Samtools flagstat: read count",
+                    "data_labels": [
+                        {"name": "Read counts", "title": "Samtools flagstat: read count"},
+                        {"name": "Percentage of total", "title": "Samtools flagstat: percentage of total"},
+                    ],
                 },
             ),
         )
 
         # Return the number of logs that were found
         return len(self.samtools_flagstat)
 
 
-#  flagstat has one thing per line, documented here (search for flagstat):
-#  http://www.htslib.org/doc/samtools.html
+# flagstat has one thing per line, documented here (search for flagstat):
+# http://www.htslib.org/doc/samtools.html
 flagstat_regexes = {
     "total": r"(\d+) \+ (\d+) in total \(QC-passed reads \+ QC-failed reads\)",
     "secondary": r"(\d+) \+ (\d+) secondary",
     "supplementary": r"(\d+) \+ (\d+) supplementary",
     "duplicates": r"(\d+) \+ (\d+) duplicates",
     "mapped": r"(\d+) \+ (\d+) mapped \((.+):(.+)\)",
     "paired in sequencing": r"(\d+) \+ (\d+) paired in sequencing",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/idxstats.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/idxstats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC submodule to parse output from Samtools idxstats """
 
 import logging
 from collections import defaultdict
 
 from multiqc import config
 from multiqc.plots import bargraph, linegraph
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/rmdup.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/rmdup.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/samtools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/samtools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """ MultiQC module to parse output from Samtools """
 
 
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 
+from .stats import StatsReportMixin
 from .flagstat import FlagstatReportMixin
 from .idxstats import IdxstatsReportMixin
 from .rmdup import RmdupReportMixin
 from .coverage import CoverageReportMixin
-
-# Import the Samtools submodules
-from .stats import StatsReportMixin
+from .markdup import MarkdupReportMixin
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(
-    BaseMultiqcModule, StatsReportMixin, FlagstatReportMixin, IdxstatsReportMixin, RmdupReportMixin, CoverageReportMixin
+    BaseMultiqcModule,
+    StatsReportMixin,
+    FlagstatReportMixin,
+    IdxstatsReportMixin,
+    RmdupReportMixin,
+    MarkdupReportMixin,
+    CoverageReportMixin,
 ):
     """Samtools has a number of different commands and outputs.
     This MultiQC module supports some but not all. The code for
     each script is split into its own file and adds a section to
     the module output if logs are found."""
 
     def __init__(self):
@@ -42,15 +47,15 @@
         n = dict()
 
         # Call submodule functions
         n["stats"] = self.parse_samtools_stats()
         if n["stats"] > 0:
             log.info(f"Found {n['stats']} stats reports")
 
-        n["flagstat"] = self.parse_samtools_flagstats()
+        n["flagstat"] = self.parse_samtools_flagstat()
         if n["flagstat"] > 0:
             log.info(f"Found {n['flagstat']} flagstat reports")
 
         n["idxstats"] = self.parse_samtools_idxstats()
         if n["idxstats"] > 0:
             log.info(f"Found {n['idxstats']} idxstats reports")
 
@@ -58,13 +63,17 @@
         if n["rmdup"] > 0:
             log.info(f"Found {n['rmdup']} rmdup reports")
 
         n["coverage"] = self.parse_samtools_coverage()
         if n["coverage"] > 0:
             log.info(f"Found {n['coverage']} coverage reports")
 
+        n["markdup"] = self.parse_samtools_markdup()
+        if n["markdup"] > 0:
+            log.info(f"Found {n['markdup']} markdup reports")
+
         # Exit if we didn't find anything
         if sum(n.values()) == 0:
             raise ModuleNoSamplesFound
 
         # Add to the General Stats table (has to be called once per MultiQC module)
         self.general_stats_addcols(self.general_stats_data, self.general_stats_headers)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/samtools/stats.py` & `multiqc_sgr-1.22.post0/multiqc/modules/samtools/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC submodule to parse output from Samtools stats """
 
 import logging
 import re
 
 from multiqc import config
-from multiqc.plots import bargraph, beeswarm
+from multiqc.plots import bargraph, violin
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 # Regex to grab version number from samtools stats contents
 VERSION_REGEX = r"# This file was produced by samtools stats \(([\d\.]+)"
 HTSLIB_REGEX = r"\+htslib-([\d\.]+)"
@@ -144,22 +142,22 @@
 
         # Make dot plot of counts
         keys = {}
         reads = {
             "min": 0,
             "modify": lambda x: float(x) * config.read_count_multiplier,
             "suffix": config.read_count_prefix,
-            "decimalPlaces": 2,
+            "tt_decimals": 2,
             "shared_key": "read_count",
         }
         bases = {
             "min": 0,
             "modify": lambda x: float(x) * config.base_count_multiplier,
             "suffix": config.base_count_prefix,
-            "decimalPlaces": 2,
+            "tt_decimals": 2,
             "shared_key": "base_count",
         }
         keys["raw_total_sequences"] = dict(reads, **{"title": "Total sequences"})
         keys["reads_mapped_and_paired"] = dict(
             reads,
             **{"title": "Mapped &amp; paired", "description": "Paired-end technology bit set + both mates mapped"},
         )
@@ -187,15 +185,15 @@
             reads, **{"title": "Outward pairs", "description": "Outward oriented pairs"}
         )
 
         self.add_section(
             name="Alignment stats",
             anchor="samtools-stats",
             description="This module parses the output from <code>samtools stats</code>. All numbers in millions.",
-            plot=beeswarm.plot(
+            plot=violin.plot(
                 self.samtools_stats,
                 keys,
                 {
                     "id": "samtools-stats-dp",
                     "title": "Samtools stats: Alignment Stats",
                 },
             ),
@@ -243,15 +241,14 @@
             to be uniquely mapped. These reads are often filtered out in downstream analyses.
             """,
             plot=alignment_chart(bedgraph_data),
         )
 
 
 def alignment_chart(data):
-    """Make the HighCharts HTML to plot the alignment rates"""
     keys = {
         "reads_mapped_MQ1": {"color": "#437bb1", "name": "Mapped (with MQ>0)"},
         "reads_MQ0": {"color": "#FF9933", "name": "MQ0"},
         "reads_unmapped": {"color": "#b1084c", "name": "Unmapped"},
     }
 
     # Config for the plot
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sargasso/sargasso.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sargasso/sargasso.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/seqera_cli/seqera_cli.py` & `multiqc_sgr-1.22.post0/multiqc/modules/seqera_cli/seqera_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,14 @@
                 {"wallTime": {"name": "Wall time"}},
                 {
                     "id": "seqera_cli_wall_time_plot",
                     "title": "Seqera platform CLI: Wall time",
                     "ylab": "hours",
                     "tt_decimals": 1,
                     "tt_suffix": " h",
-                    "tt_percentages": False,
                     "cpswitch": False,
                     "hide_zero_cats": False,
                 },
             ),
         )
         self.add_section(
             name="CPU time",
@@ -368,15 +367,14 @@
                 {"cpuTime": {"name": "CPU time"}},
                 {
                     "id": "seqera_cli_cpu_time_plot",
                     "title": "Seqera platform CLI: CPU time",
                     "ylab": "CPU hours",
                     "tt_decimals": 1,
                     "tt_suffix": " h",
-                    "tt_percentages": False,
                     "cpswitch": False,
                     "hide_zero_cats": False,
                 },
             ),
         )
         self.add_section(
             name="Estimated cost",
@@ -386,13 +384,12 @@
                 {"cost": {"name": "Estimated cost"}},
                 {
                     "id": "seqera_cli_cost_plot",
                     "title": "Seqera platform CLI: Estimated cost",
                     "ylab": "$",
                     "tt_decimals": 1,
                     "tt_suffix": " $",
-                    "tt_percentages": False,
                     "cpswitch": False,
                     "hide_zero_cats": False,
                 },
             ),
         )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/seqwho/seqwho.py` & `multiqc_sgr-1.22.post0/multiqc/modules/seqwho/seqwho.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/seqyclean/seqyclean.py` & `multiqc_sgr-1.22.post0/multiqc/modules/seqyclean/seqyclean.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sexdeterrmine/sexdeterrmine.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sexdeterrmine/sexdeterrmine.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sickle/sickle.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sickle/sickle.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/skewer/skewer.py` & `multiqc_sgr-1.22.post0/multiqc/modules/skewer/skewer.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/slamdunk/slamdunk.py` & `multiqc_sgr-1.22.post0/multiqc/modules/slamdunk/slamdunk.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,15 +451,14 @@
             "title": "Slamdunk: Overall conversion rates in reads",
             "cpswitch": False,
             "cpswitch_c_active": False,
             "ylab": "Number of reads",
             "stacking": "normal",
             "tt_decimals": 2,
             "tt_suffix": "%",
-            "tt_percentages": False,
             "hide_zero_cats": False,
             "data_labels": [
                 "Plus Strand +",
                 "Minus Strand -",
             ],
         }
 
@@ -495,15 +494,14 @@
             "title": "Slamdunk: Overall conversion rates per UTR",
             "cpswitch": False,
             "cpswitch_c_active": False,
             "ylab": "Number of conversions",
             "stacking": "normal",
             "tt_decimals": 2,
             "tt_suffix": "%",
-            "tt_percentages": False,
             "hide_zero_cats": False,
         }
 
         self.add_section(
             name="Conversion rates per UTR",
             anchor="slamdunk_utr_rates",
             description="""This plot shows the individual conversion rates for all UTRs
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/snippy/snippy.py` & `multiqc_sgr-1.22.post0/multiqc/modules/snippy/snippy.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/snpeff/snpeff.py` & `multiqc_sgr-1.22.post0/multiqc/modules/snpeff/snpeff.py`

 * *Files 6% similar despite different names*

```diff
@@ -196,28 +196,37 @@
                             c += counts[i]
                 if len(quals) > 0:
                     self.snpeff_qualities[f["s_name"]] = quals
 
             # Everything else
             elif section in keys:
                 if keys[section] == "all" or any([k in s[0].strip() for k in keys[section]]):
+                    if len(s) < 2:
+                        continue
+                    key = s[0].strip()
+                    val = s[1].strip()
                     try:
-                        parsed_data[s[0].strip()] = float(s[1].strip())
+                        val = float(val)
                     except ValueError:
-                        parsed_data[s[0].strip()] = s[1].strip()
-                    except IndexError:
                         pass
                     else:
+                        parsed_data[key] = val
                         # Parsing the number worked - add to totals
                         try:
-                            self.snpeff_section_totals[section][s[0].strip()] += parsed_data[s[0].strip()]
+                            self.snpeff_section_totals[section][key] += val
                         except KeyError:
-                            self.snpeff_section_totals[section][s[0].strip()] = parsed_data[s[0].strip()]
+                            self.snpeff_section_totals[section][key] = val
                     if len(s) > 2 and s[2][-1:] == "%":
-                        parsed_data[f"{s[0].strip()}_percent"] = float(s[2][:-1])
+                        val = s[2].strip("%").strip()
+                        try:
+                            val = float(val)
+                        except ValueError:
+                            pass
+                        else:
+                            parsed_data[f"{key}_percent"] = val
 
         if len(parsed_data) > 0:
             if f["s_name"] in self.snpeff_data:
                 log.debug(f"Duplicate sample name found! Overwriting: {f['s_name']}")
             self.add_data_source(f)
             self.snpeff_data[f["s_name"]] = parsed_data
             self.add_software_version(version, f["s_name"])
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/snpsplit/snpsplit.py` & `multiqc_sgr-1.22.post0/multiqc/modules/snpsplit/snpsplit.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/software_versions.py` & `multiqc_sgr-1.22.post0/multiqc/modules/software_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-#!/usr/bin/env python
-
 """ Super Special-Case MultiQC module to produce report section on software versions """
 
-
 import logging
 from textwrap import dedent
 
 from multiqc.modules.base_module import BaseMultiqcModule
 from multiqc.utils import config as mqc_config
 from multiqc.utils import report as mqc_report
 from multiqc.utils import util_functions
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/somalier/somalier.py` & `multiqc_sgr-1.22.post0/multiqc/modules/somalier/somalier.py`

 * *Files 1% similar despite different names*

```diff
@@ -536,14 +536,15 @@
                 data[s_name] = {"x": d["gt_depth_mean"], "y": d["ab_std"]}
 
         if len(data) > 0:
             pconfig = {
                 "id": "somalier_het_check_plot",
                 "title": "Somalier: Sample Observed Heterozygosity",
                 "xlab": "Mean depth",
+                "xsuffix": "x",
                 "ylab": "Standard deviation of allele-balance",
             }
 
             self.add_section(
                 name="Heterozygosity",
                 description="Standard deviation of heterozygous allele balance against mean depth.",
                 helptext="A high standard deviation in allele balance suggests contamination.",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sortmerna/sortmerna.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sortmerna/sortmerna.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.write_data_file(self.sortmerna, "multiqc_sortmerna")
 
         # Superfluous function call to confirm that it is used in this module
         # Replace None with actual version if it is available
         self.add_software_version(None)
 
         # Get custom table header, default to 'rRNA'
-        tab_header = getattr(config, "sortmerna", {}).get("seqname", "% rRNA")
+        tab_header = getattr(config, "sortmerna", {}).get("seqname", "rRNA")
 
         # Add rRNA rate to the general stats table
         headers = {
             "rRNA_pct": {
                 "title": tab_header,
                 "description": "Percentage of reads matched to a SortMeRNA database",
                 "max": 100,
@@ -57,15 +57,15 @@
                 "suffix": "%",
                 "scale": "OrRd",
             }
         }
         self.general_stats_addcols(self.sortmerna, headers)
 
         # Make barplot
-        self.sortmerna_detailed_barplot()
+        self.sortmerna_detailed_rates_barplot()
 
     def parse_sortmerna(self, f):
         s_name = None
         post_results_start = False
         post_database_start = False
         db_number = 0
         err = False
@@ -125,25 +125,29 @@
             if "By database:" in line or "Coverage by database:" in line:
                 post_database_start = True
         if err:
             log.warning("Error parsing data in: " + s_name)
             self.sortmerna.pop(s_name, "None")
         s_name = None
 
-    def sortmerna_detailed_barplot(self):
-        """Make the HighCharts HTML to plot the sortmerna rates"""
-
+    def sortmerna_detailed_rates_barplot(self):
         # Specify the order of the different possible categories
         keys = {}
         metrics = set()
         for sample in self.sortmerna:
             for key in self.sortmerna[sample]:
                 if key not in ["total", "rRNA", "non_rRNA"] and "_pct" not in key:
                     metrics.add(key)
 
         for key in metrics:
             keys[key] = {"name": key.replace("_count", "")}
 
         # Config for the plot
-        pconfig = {"id": "sortmerna-detailed-plot", "title": "SortMeRNA: Hit Counts", "ylab": "Reads"}
+        pconfig = {
+            "id": "sortmerna-detailed-plot",
+            "title": "SortMeRNA: Hit Counts",
+            "ylab": "Reads",
+        }
 
-        self.add_section(plot=bargraph.plot(self.sortmerna, sorted(keys), pconfig))
+        self.add_section(
+            plot=bargraph.plot(self.sortmerna, sorted(keys), pconfig),
+        )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sourmash/compare.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sourmash/compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC module to parse similarity matrix output by sourmash compare """
 
 import logging
 import os
 import re
 
 import numpy
@@ -70,13 +68,13 @@
                     data,
                     xcats=labels,
                     ycats=labels,
                     pconfig={
                         "id": f"sourmash-compare-heatmap-{id}",
                         "title": "Sourmash: Compare",
                         "square": True,
-                        "decimalPlaces": 7,
+                        "tt_decimals": 7,
                     },
                 ),
             )
 
         return len(matrices)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sourmash/gather.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sourmash/gather.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC module to parse similarity matrix output by sourmash gather """
 
 import csv
 import logging
 
 from multiqc.plots import bargraph
 from multiqc.utils import config
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/sourmash/sourmash.py` & `multiqc_sgr-1.22.post0/multiqc/modules/sourmash/sourmash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC module to parse output from sourmash """
 
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 
 from .compare import CompareMixin
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/spaceranger/_utils.py` & `multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 def clean_title_case(col_id):
     title = col_id.title() if col_id[0:1].islower() else col_id
     for _str in ["Bc", "bc", "Umi", "Igk", "Igh", "Igl", "Vj", "q30"]:
         title = title.replace(_str, _str.upper())
     return title
 
 
-def update_dict(table, headers, rows_list, col_map, colours, prefix, int_cols=()):
+def update_data_and_headers(data, headers, new_data, new_headers, colors, prefix, int_cols=()):
     """update the data dict and headers dict
 
     :param: int_cols columns to be shown as integers in the table
     """
 
-    for col_name, col_data in rows_list:
-        if col_name in col_map:
+    for col_name, col_data in new_data:
+        if col_name in new_headers:
             # Sanitize numeric data
             is_percentage = "%" in col_data
             col_data = col_data.replace(",", "").replace("%", "")
 
             # Convert to float when possible
             if col_data == "None":
                 col_data = None
             else:
                 try:
                     col_data = float(col_data)
                 except ValueError:
                     pass
 
-            col_id = col_map[col_name]
-            table[col_id] = col_data
+            col_id = new_headers[col_name]
+            data[col_id] = col_data
             headers[col_id] = {
                 "rid": "{}_{}".format(prefix, col_id.replace(" ", "_").replace("/", "_")),
                 "title": clean_title_case(col_id),
                 "description": col_name,
                 "namespace": f"Space Ranger {prefix}",
-                "scale": colours.get(col_id, "RdYlGn" if is_percentage else "GnBu"),
+                "scale": colors.get(col_id, "RdYlGn" if is_percentage else "GnBu"),
             }
             if is_percentage:
                 headers[col_id].update(
                     {
                         "suffix": "%",
                         "max": 100,
                         "min": 0,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/spaceranger/count.py` & `multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/count.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,153 +1,149 @@
 """ MultiQC module to parse output from Space Ranger count """
 
 import json
 import logging
 import os
-from collections import OrderedDict
 
 from multiqc import config
 from multiqc.plots import linegraph, table
 
-from ._utils import set_hidden_cols, transform_data, update_dict
+from ._utils import set_hidden_cols, transform_data, update_data_and_headers
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class SpaceRangerCountMixin:
     """Space Ranger count report parser"""
 
     def parse_count_html(self):
-        self.spacerangercount_data = dict()
-        self.spacerangercount_general_data = dict()
-        self.spacerangercount_warnings = dict()
-        self.spacerangercount_plots_conf = {"saturation": dict(), "genes": dict(), "genomic_dna": dict()}
-        self.spacerangercount_plots_data = {"saturation": dict(), "genes": dict(), "genomic_dna": dict()}
-        self.count_general_data_headers = dict()
-        self.count_data_headers = OrderedDict()
-        self.count_warnings_headers = OrderedDict()
+        self.generalstats_data = dict()
+        self.summary_data = dict()
+        self.warnings_data = dict()
+        self.generalstats_headers = dict()
+        self.summary_headers = dict()
+        self.warnings_headers = dict()
+        self.plots_conf = {"saturation": dict(), "genes": dict(), "genomic_dna": dict()}
+        self.plots_data = {"saturation": dict(), "genes": dict(), "genomic_dna": dict()}
 
         for f in self.find_log_files("spaceranger/count_html", filehandles=True):
             self.parse_count_report(f)
 
-        self.spacerangercount_data = self.ignore_samples(self.spacerangercount_data)
-        self.spacerangercount_general_data = self.ignore_samples(self.spacerangercount_general_data)
-        self.spacerangercount_warnings = self.ignore_samples(self.spacerangercount_warnings)
-        for k in self.spacerangercount_plots_data.keys():
-            self.spacerangercount_plots_data[k] = self.ignore_samples(self.spacerangercount_plots_data[k])
+        self.summary_data = self.ignore_samples(self.summary_data)
+        self.generalstats_data = self.ignore_samples(self.generalstats_data)
+        self.warnings_data = self.ignore_samples(self.warnings_data)
+        for k in self.plots_data.keys():
+            self.plots_data[k] = self.ignore_samples(self.plots_data[k])
 
-        self.count_general_data_headers["reads"] = {
+        self.generalstats_headers["reads"] = {
             "rid": "count_genstats_reads",
             "title": "Reads",
             "description": f"Number of reads ({config.read_count_desc})",
             "shared_key": "read_count",
             "namespace": "Space Ranger Count",
         }
 
-        self.count_data_headers["reads"] = {
+        self.summary_headers["reads"] = {
             "rid": "count_data_reads",
             "title": "Reads",
             "description": f"Number of reads ({config.read_count_desc})",
             "shared_key": "read_count",
         }
-        self.count_data_headers = set_hidden_cols(
-            self.count_data_headers,
+        self.summary_headers = set_hidden_cols(
+            self.summary_headers,
             [
                 "Q30 bc",
                 "Q30 UMI",
                 "Q30 read",
                 "reads in spots",
                 "avg reads/spot",
                 "confident reads",
                 "confident filtered reads",
                 "genomic unis/unspliced probe",
                 "valid umi",
                 "saturation",
             ],
         )
 
-        if len(self.spacerangercount_general_data) == 0:
+        if len(self.generalstats_data) == 0:
             return 0
 
-        else:
-            self.general_stats_addcols(self.spacerangercount_general_data, self.count_general_data_headers)
+        self.general_stats_addcols(self.generalstats_data, self.generalstats_headers)
 
-            # Write parsed report data to a file
-            self.write_data_file(self.spacerangercount_data, "multiqc_spaceranger_count")
-
-            # Add sections to the report
-            if len(self.spacerangercount_warnings) > 0:
-                self.add_section(
-                    name="Count - Warnings",
-                    anchor="spaceranger-count-warnings-section",
-                    description="Warnings encountered during the analysis",
-                    plot=table.plot(
-                        self.spacerangercount_warnings,
-                        self.count_warnings_headers,
-                        {
-                            "namespace": "Space Ranger Count",
-                            "id": "spaceranger-count-warnings",
-                            "title": "Space Ranger Count: Warnings",
-                        },
-                    ),
-                )
+        # Write parsed report data to a file
+        self.write_data_file(self.summary_data, "multiqc_spaceranger_count")
 
+        # Add sections to the report
+        if len(self.warnings_data) > 0:
             self.add_section(
-                name="Count - Summary stats",
-                anchor="spaceranger-count-stats-section",
-                description="Summary QC metrics from Space Ranger count",
+                name="Count - Warnings",
+                anchor="spaceranger-count-warnings-section",
+                description="Warnings encountered during the analysis",
                 plot=table.plot(
-                    self.spacerangercount_data,
-                    self.count_data_headers,
+                    self.warnings_data,
+                    self.warnings_headers,
                     {
                         "namespace": "Space Ranger Count",
-                        "id": "spaceranger-count-stats",
-                        "title": "Space Ranger Count: Summary stats",
+                        "id": "spaceranger-count-warnings",
+                        "title": "Space Ranger Count: Warnings",
                     },
                 ),
             )
 
-            # The gDNA plots are only contained for spaceranger workflows with probesets
-            if "genomic_dna" in self.spacerangercount_plots_data:
-                self.add_section(
-                    name="Count - UMIs from Genomic DNA",
-                    anchor="spaceranger-count-bcrank-plot-section",
-                    description=self.spacerangercount_plots_conf["genomic_dna"]["description"],
-                    helptext=self.spacerangercount_plots_conf["genomic_dna"]["helptext"],
-                    plot=linegraph.plot(
-                        self.spacerangercount_plots_data["genomic_dna"],
-                        self.spacerangercount_plots_conf["genomic_dna"]["config"],
-                    ),
-                )
-
-            if "genes" in self.spacerangercount_plots_data:
-                self.add_section(
-                    name="Count - Median genes",
-                    anchor="spaceranger-count-genes-plot-section",
-                    description=self.spacerangercount_plots_conf["genes"]["description"],
-                    helptext=self.spacerangercount_plots_conf["genes"]["helptext"],
-                    plot=linegraph.plot(
-                        self.spacerangercount_plots_data["genes"], self.spacerangercount_plots_conf["genes"]["config"]
-                    ),
-                )
-
-            if "saturation" in self.spacerangercount_plots_data:
-                self.add_section(
-                    name="Count - Saturation plot",
-                    anchor="spaceranger-count-saturation-plot-section",
-                    description=self.spacerangercount_plots_conf["saturation"]["description"],
-                    helptext=self.spacerangercount_plots_conf["saturation"]["helptext"],
-                    plot=linegraph.plot(
-                        self.spacerangercount_plots_data["saturation"],
-                        self.spacerangercount_plots_conf["saturation"]["config"],
-                    ),
-                )
+        self.add_section(
+            name="Count - Summary stats",
+            anchor="spaceranger-count-stats-section",
+            description="Summary QC metrics from Space Ranger count",
+            plot=table.plot(
+                self.summary_data,
+                self.summary_headers,
+                {
+                    "namespace": "Space Ranger Count",
+                    "id": "spaceranger-count-stats",
+                    "title": "Space Ranger Count: Summary stats",
+                },
+            ),
+        )
+
+        # The gDNA plots are only contained for spaceranger workflows with probesets
+        if "genomic_dna" in self.plots_conf:
+            self.add_section(
+                name="Count - UMIs from Genomic DNA",
+                anchor="spaceranger-count-bcrank-plot-section",
+                description=self.plots_conf["genomic_dna"]["description"],
+                helptext=self.plots_conf["genomic_dna"]["helptext"],
+                plot=linegraph.plot(
+                    self.plots_data["genomic_dna"],
+                    self.plots_conf["genomic_dna"]["config"],
+                ),
+            )
+
+        if "genes" in self.plots_conf:
+            self.add_section(
+                name="Count - Median genes",
+                anchor="spaceranger-count-genes-plot-section",
+                description=self.plots_conf["genes"]["description"],
+                helptext=self.plots_conf["genes"]["helptext"],
+                plot=linegraph.plot(self.plots_data["genes"], self.plots_conf["genes"]["config"]),
+            )
+
+        if "saturation" in self.plots_conf:
+            self.add_section(
+                name="Count - Saturation plot",
+                anchor="spaceranger-count-saturation-plot-section",
+                description=self.plots_conf["saturation"]["description"],
+                helptext=self.plots_conf["saturation"]["helptext"],
+                plot=linegraph.plot(
+                    self.plots_data["saturation"],
+                    self.plots_conf["saturation"]["config"],
+                ),
+            )
 
-            return len(self.spacerangercount_general_data)
+        return len(self.generalstats_data)
 
     def parse_count_report(self, f):
         """Go through the html report of space ranger and extract the data in a dicts"""
 
         summary = None
         for line in f["f"]:
             line = line.strip()
@@ -187,29 +183,35 @@
         col_dict = {
             "Number of Spots Under Tissue": "spots under tissue",
             "Mean Reads per Spot": "avg reads/spot",
             "Fraction Reads in Spots Under Tissue": "reads in spots",
             "Number of Reads": "reads",
             "Valid Barcodes": "valid bc",
         }
-        colours = {
+        colors = {
             "spots under tissue": "RdPu",
             "avg reads/spot": "Blues",
             "reads in spots": "PiYG",
             "reads": "YlGn",
             "valid bc": "RdYlGn",
         }
         int_cols = [
             "reads",
             "spots under tissue",
             "avg reads/spot",
         ]
         data_general_stats = {}
-        update_dict(
-            data_general_stats, self.count_general_data_headers, data_rows, col_dict, colours, "Count", int_cols
+        update_data_and_headers(
+            data=data_general_stats,
+            headers=self.generalstats_headers,
+            new_data=data_rows,
+            new_headers=col_dict,
+            colors=colors,
+            prefix="Count",
+            int_cols=int_cols,
         )
 
         # Store full data from space ranger count report
         col_dict = {
             "Number of Reads": "reads",
             "Number of Spots Under Tissue": "spots under tissue",
             "Mean Reads per Spot": "avg reads/spot",
@@ -225,15 +227,15 @@
             "Q30 Bases in RNA Read": "Q30 read",
             "Reads Mapped to Probe Set": "reads mapped",
             "Reads Mapped Confidently to Probe Set": "confident reads",
             "Reads Mapped Confidently to Filtered Probe Set": "confident filtered reads",
             "Estimated UMIs from Genomic DNA": "genomic umis",
             "Estimated UMIs from Genomic DNA per Unspliced Probe": "genomic umis/unspliced probe",
         }
-        colours = {
+        colors = {
             "reads": "YlGn",
             "spots under tissue": "RdPu",
             "avg reads/spot": "Blues",
             "genes detected": "Greens",
             "median genes/spot": "Purples",
             "reads in spots": "PuBuGn",
             "valid bc": "Spectral",
@@ -248,36 +250,44 @@
             "spots under tissue",
             "avg reads/spot",
             "median genes/spot",
             "genes detected",
             "genomic umis/unspliced probe",
         ]
         data = {}
-        update_dict(data, self.count_data_headers, data_rows, col_dict, colours, "Count", int_cols)
+        update_data_and_headers(
+            data=data,
+            headers=self.summary_headers,
+            new_data=data_rows,
+            new_headers=col_dict,
+            colors=colors,
+            prefix="Count",
+            int_cols=int_cols,
+        )
 
         # Extract warnings if any
         warnings = {}
         alarms_list = summary["alarms"].get("alarms", [])
         for alarm in alarms_list:
             # "Intron mode used" alarm added in Space Ranger 7.0 lacks id
             if "id" not in alarm:
                 continue
             warnings[alarm["id"]] = "FAIL"
-            self.count_warnings_headers[alarm["id"]] = {
+            self.warnings_headers[alarm["id"]] = {
                 "title": alarm["id"].replace("_", " ").title(),
                 "description": alarm["title"],
                 "bgcols": {"FAIL": "#f7dddc"},
             }
 
         # Extract data for plots
-        plots = {}
+        plots_conf = {}
         plots_data = {}
         # `analysis_tab` may not be present in the report if there are few reads
         try:
-            plots["saturation"] = {
+            plots_conf["saturation"] = {
                 "config": {
                     "id": "mqc_spaceranger_count_saturation",
                     "title": f"Space Ranger count: {summary['analysis_tab']['seq_saturation_plot']['help']['title']}",
                     "xlab": summary["analysis_tab"]["seq_saturation_plot"]["plot"]["layout"]["xaxis"]["title"],
                     "ylab": summary["analysis_tab"]["seq_saturation_plot"]["plot"]["layout"]["yaxis"]["title"],
                     "yLog": False,
                     "xLog": False,
@@ -288,22 +298,22 @@
                 "helptext": summary["analysis_tab"]["seq_saturation_plot"]["help"]["helpText"],
             }
             plots_data["saturation"] = {
                 sample_name: transform_data(summary["analysis_tab"]["seq_saturation_plot"]["plot"]["data"][0])
             }
         except KeyError as e:
             log.debug("No saturation plot found in the spaceranger report:", e)
-            if "saturation" in plots:
-                del plots["saturation"]
+            if "saturation" in plots_conf:
+                del plots_conf["saturation"]
             if "saturation" in plots_data:
                 del plots_data["saturation"]
 
         # `analysis_tab` may not be present in the report if there are few reads
         try:
-            plots["genes"] = {
+            plots_conf["genes"] = {
                 "config": {
                     "id": "mqc_spaceranger_count_genesXspot",
                     "title": f"Space Ranger count: {summary['analysis_tab']['median_gene_plot']['help']['title']}",
                     "xlab": summary["analysis_tab"]["median_gene_plot"]["plot"]["layout"]["xaxis"]["title"],
                     "ylab": summary["analysis_tab"]["median_gene_plot"]["plot"]["layout"]["yaxis"]["title"],
                     "yLog": False,
                     "xLog": False,
@@ -312,22 +322,22 @@
                 "helptext": summary["analysis_tab"]["median_gene_plot"]["help"]["helpText"],
             }
             plots_data["genes"] = {
                 sample_name: transform_data(summary["analysis_tab"]["median_gene_plot"]["plot"]["data"][0])
             }
         except KeyError:
             log.debug("No median gene plot found in the spaceranger report")
-            if "genes" in plots:
-                del plots["genes"]
+            if "genes" in plots_conf:
+                del plots_conf["genes"]
             if "genes" in plots_data:
                 del plots_data["genes"]
 
         # The gDNA plots are only contained for spaceranger workflows with probesets
         try:
-            plots["genomic_dna"] = {
+            plots_conf["genomic_dna"] = {
                 "config": {
                     "id": "mqc_spaceranger_count_genomic_dna",
                     "title": f"Space Ranger count: {summary['analysis_tab']['gdna']['gems']['help']['title']}",
                     "xlab": summary["analysis_tab"]["gdna"]["plot"]["layout"]["xaxis"]["title"],
                     "ylab": summary["analysis_tab"]["gdna"]["plot"]["layout"]["yaxis"]["title"],
                     "yLog": False,
                     "xLog": False,
@@ -337,25 +347,25 @@
                 + "\n\nThis summary graphic in the MultiQC report only shows the estimated mean baseline level of unspliced probe counts.",
             }
             plots_data["genomic_dna"] = {
                 sample_name: transform_data(summary["analysis_tab"]["gdna"]["plot"]["data"][2])
             }
         except KeyError:
             log.debug("No genomic DNA plot found in the spaceranger report")
-            if "genomic_dna" in plots:
-                del plots["genomic_dna"]
+            if "genomic_dna" in plots_conf:
+                del plots_conf["genomic_dna"]
             if "genomic_dna" in plots_data:
                 del plots_data["genomic_dna"]
 
         if len(data) > 0:
-            if sample_name in self.spacerangercount_general_data:
+            if sample_name in self.generalstats_data:
                 log.debug(f"Duplicate sample name found in {f['fn']}! Overwriting: {sample_name}")
             self.add_data_source(f, sample_name, module="spaceranger", section="count")
-            self.spacerangercount_data[sample_name] = data
-            self.spacerangercount_general_data[sample_name] = data_general_stats
+            self.summary_data[sample_name] = data
+            self.generalstats_data[sample_name] = data_general_stats
             if len(warnings) > 0:
-                self.spacerangercount_warnings[sample_name] = warnings
-            self.spacerangercount_plots_conf = plots
+                self.warnings_data[sample_name] = warnings
+            self.plots_conf = plots_conf
             for k in plots_data.keys():
-                if k not in self.spacerangercount_plots_data.keys():
-                    self.spacerangercount_plots_data[k] = dict()
-                self.spacerangercount_plots_data[k].update(plots_data[k])
+                if k not in self.plots_data.keys():
+                    self.plots_data[k] = dict()
+                self.plots_data[k].update(plots_data[k])
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/spaceranger/spaceranger.py` & `multiqc_sgr-1.22.post0/multiqc/modules/spaceranger/spaceranger.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/stacks/stacks.py` & `multiqc_sgr-1.22.post0/multiqc/modules/stacks/stacks.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/star/star.py` & `multiqc_sgr-1.22.post0/multiqc/modules/star/star.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/supernova/supernova.py` & `multiqc_sgr-1.22.post0/multiqc/modules/supernova/supernova.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/theta2/theta2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/theta2/theta2.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/tophat/tophat.py` & `multiqc_sgr-1.22.post0/multiqc/modules/tophat/tophat.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,16 +125,14 @@
                 "modify": lambda x: x * config.read_count_multiplier,
                 "shared_key": "read_count",
             },
         }
         self.general_stats_addcols(self.tophat_data, headers)
 
     def tophat_alignment_plot(self):
-        """Make the HighCharts HTML to plot the alignment rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "aligned_not_multimapped_discordant": {"color": "#437bb1", "name": "Aligned"},
             "aligned_multimap": {"color": "#f7a35c", "name": "Multimapped"},
             "aligned_discordant": {"color": "#e63491", "name": "Discordant mappings"},
             "unaligned_total": {"color": "#7f0000", "name": "Not aligned"},
         }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/trimmomatic/trimmomatic.py` & `multiqc_sgr-1.22.post0/multiqc/modules/trimmomatic/trimmomatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,16 +113,14 @@
                         "reverse_only_surviving_pct": float(match.group(7).replace(",", ".")),
                         "dropped": float(match.group(8)),
                         "dropped_pct": float(match.group(9).replace(",", ".")),
                     }
                     s_name = None
 
     def trimmomatic_barplot(self):
-        """Make the HighCharts HTML to plot the trimmomatic rates"""
-
         # Specify the order of the different possible categories
         keys = {
             "surviving": {"color": "#437bb1", "name": "Surviving Reads"},
             "both_surviving": {"color": "#f7a35c", "name": "Both Surviving"},
             "forward_only_surviving": {"color": "#e63491", "name": "Forward Only Surviving"},
             "reverse_only_surviving": {"color": "#b1084c", "name": "Reverse Only Surviving"},
             "dropped": {"color": "#7f0000", "name": "Dropped"},
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/truvari/bench.py` & `multiqc_sgr-1.22.post0/multiqc/modules/truvari/bench.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#!/usr/bin/env python
 """ MultiQC submodule to parse output from truvari bench """
+
 import json
 import logging
 import os
 import re
 
 from multiqc.plots import bargraph, scatter
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/truvari/truvari.py` & `multiqc_sgr-1.22.post0/multiqc/modules/truvari/truvari.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-#!/usr/bin/env python
 """ MultiQC module to parse output from truvari """
+
 import logging
 
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
 
 # Import the truvari submodules
 from .bench import BenchSummary
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/umitools/umitools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/umitools/umitools.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import logging
 import re
 from typing import Dict, Optional
 
 from multiqc import config
 from multiqc.modules.base_module import BaseMultiqcModule, ModuleNoSamplesFound
-from multiqc.plots import bargraph, beeswarm
+from multiqc.plots import bargraph, violin
 
 # Initialise the logger
 log = logging.getLogger(__name__)
 
 
 class MultiqcModule(BaseMultiqcModule):
     """
@@ -211,15 +211,15 @@
         keys = {
             "read1_match": {"color": "#7fc9c7", "name": "Read1 Match"},
             "read1_mismatch": {"color": "#fd9286", "name": "Read1 Mismatch"},
             "read2_match": {"color": "#7f89c9", "name": "Read2 Match"},
             "read2_mismatch": {"color": "#fd86aa", "name": "Read2 Mismatch"},
         }
 
-        # add a section with a beeswarm plot of UMI stats to the report
+        # Add a section with a barplot plot of UMI stats to the report
         self.add_section(
             name="Extract Stats",
             anchor="umitools_extract",
             description="Read stats from `umi_tools extract`",
             plot=bargraph.plot(
                 data_by_sample,
                 keys,
@@ -269,27 +269,27 @@
                 "description": "Max number of unique UMIs per position",
                 "min": 0,
                 "format": "{:,.0f}",
                 "scale": "Oranges",
             },
         }
 
-        # add a section with a beeswarm plot of UMI stats to the report
+        # add a section with a violin plot of UMI stats to the report
         self.add_section(
             name="UMI Stats",
             anchor="umitools-umi-stats",
             description="Statistics from running `umi_tools dedup` or `umi_tools extract`",
             helptext="""
             - **Positions Dedup**: Total number of positions deduplicated
             - **Total UMIs**: Total UMIs found in sample
             - **Unique UMIs**: Unique UMIs found in sample
             - **Mean #UMI**: Mean number of unique UMIs per position
             - **Max #UMI**: Max number of unique UMIs per position
             """,
-            plot=beeswarm.plot(
+            plot=violin.plot(
                 data_by_sample,
                 headers,
                 {
                     "id": "umitools_stats_violin",
                     "table_title": "UMI-tools: UMI stats",
                 },
             ),
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/varscan2/varscan2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/varscan2/varscan2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """ MultiQC module to parse output files from VarScan2 """
 
 
 import logging
 import re
 
 from multiqc import config
@@ -197,15 +195,14 @@
                 "hidden": True,
             },
         }
 
         self.general_stats_addcols(self.varscan2_data, headers)
 
     def varscan2_counts_barplot(self):
-        """Make the HighCharts HTML to plot the reported SNPs"""
         # 146 variant positions (106 SNP, 40 indel)
         # 12 were failed by the strand-filter
         # 99 variant positions reported (99 SNP, 0 indel)
 
         # Specify the order of the different possible categories
         cats = [
             {
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vcftools/relatedness2.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vcftools/relatedness2.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                     m.data,
                     xcats=m.x_labels,
                     ycats=m.y_labels,
                     pconfig={
                         "id": f"vcftools-relatedness2-heatmap-{idx}",
                         "title": "VCFTools: Relatedness2",
                         "square": True,
-                        "decimalPlaces": 7,
+                        "tt_decimals": 7,
                     },
                 ),
             )
 
         return len(matrices)
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_by_count.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_by_count.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_by_qual.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_by_qual.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vcftools/tstv_summary.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vcftools/tstv_summary.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vcftools/vcftools.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vcftools/vcftools.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/vep/vep.py` & `multiqc_sgr-1.22.post0/multiqc/modules/vep/vep.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/verifybamid/verifybamid.py` & `multiqc_sgr-1.22.post0/multiqc/modules/verifybamid/verifybamid.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/whatshap/whatshap.py` & `multiqc_sgr-1.22.post0/multiqc/modules/whatshap/whatshap.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,14 @@
 
         configuration = {
             "id": "multiqc_whatshap_phased_bp_plot",
             "title": "WhatsHap: Phased Basepairs per Sample",
             "anchor": "multiqc_whatshap_phased_bp",
             "ylab": "Base Pairs",
             "cpswitch": False,
-            "tt_percentages": False,
         }
 
         keys = {"Phased Base Pairs": {"name": "Phased Base Pairs"}}
 
         # If the Phased Base Pairs is zero for all samples, we do not add the
         # WhatsHap section
         for sample, values in pdata.items():
```

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/xengsort/xengsort.py` & `multiqc_sgr-1.22.post0/multiqc/modules/xengsort/xengsort.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/modules/xenome/xenome.py` & `multiqc_sgr-1.22.post0/multiqc/modules/xenome/xenome.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/multiqc.py` & `multiqc_sgr-1.22.post0/multiqc/multiqc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 multiqc.multiqc
 ~~~~~~~~~~~~~~~~~~~~~
 The main function to run MultiQC. Sorry about the messy namespace.
 Primarily called by multiqc.__main__.py
 Imported by __init__.py so available as multiqc.run()
 """
+
 import base64
 import errno
 import io
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import time
 import json
 import traceback
+from importlib.metadata import EntryPoint
+from typing import Dict, Union, Callable, List
 
 import jinja2
 import requests
 import rich
 import rich_click as click
 from packaging import version
 from rich.syntax import Syntax
 
-from .modules.base_module import ModuleNoSamplesFound
+from .modules.base_module import ModuleNoSamplesFound, BaseMultiqcModule
 from .plots import table
 from .utils import config, log, megaqc, plugin_hooks, report, software_versions, strict_helpers, util_functions
 from .utils.util_functions import strtobool
 
 # Set up logging
 start_execution_time = time.time()
 logger = config.logger
@@ -496,15 +497,14 @@
         strict = True
     if strict:
         config.strict = True
         config.lint = True  # Deprecated since v1.17
         strict_helpers.run_tests()
     if development:
         config.development = True
-        config.export_plots = True
         if "png" not in config.export_plot_formats:
             config.export_plot_formats.append("png")
     if make_pdf:
         config.template = "simple"
     if no_megaqc_upload:
         config.megaqc_upload = False
     else:
@@ -737,26 +737,24 @@
     # Run the modules!
     plugin_hooks.mqc_trigger("before_modules")
     report.modules_output = list()
     sys_exit_code = 0
     total_mods_starttime = time.time()
     for mod_idx, mod_dict in enumerate(run_modules):
         mod_starttime = time.time()
-        this_module = list(mod_dict.keys())[0]
-        mod_cust_config = list(mod_dict.values())[0]
-        if mod_cust_config is None:
-            mod_cust_config = {}
+        this_module: str = list(mod_dict.keys())[0]
+        mod_cust_config: Dict = list(mod_dict.values())[0] or {}
         try:
-            mod = config.avail_modules[this_module].load()
-            mod.mod_cust_config = mod_cust_config  # feels bad doing this, but seems to work
-            output = mod()
-            if not isinstance(output, list):
-                output = [output]
-            for m in output:
-                report.modules_output.append(m)
+            entry_point: EntryPoint = config.avail_modules[this_module]
+            module_initializer: Callable[[], Union[BaseMultiqcModule, List[BaseMultiqcModule]]] = entry_point.load()
+            module_initializer.mod_cust_config = mod_cust_config
+            modules = module_initializer()
+            if not isinstance(modules, list):
+                modules = [modules]
+            report.modules_output.extend(modules)
 
             if config.make_report:
                 # Copy over css & js files if requested by the theme
                 try:
                     for to, path in report.modules_output[-1].css.items():
                         copy_to = os.path.join(tmp_dir, to)
                         os.makedirs(os.path.dirname(copy_to))
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/bargraph.py` & `multiqc_sgr-1.22.post0/multiqc/plots/bargraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,16 +174,14 @@
             plotdata.append(hc_data)
 
     if len(plotdata) == 0:
         logger.warning(f"Tried to make bar plot, but had no data: {pconfig.get('id')}")
         return '<p class="text-danger">Error - was not able to plot data.</p>'
 
     # Add colors to the categories if not set. Since the "plot_defaults" scale is
-    # identical to default scale of the Highcharts JS library, this is not strictly
-    # needed. But it future proofs when we replace Highcharts with something else.
     scale = mqc_colour.mqc_colour_scale("plot_defaults")
     for si, sd in enumerate(plotdata):
         for di, d in enumerate(sd):
             d.setdefault("color", scale.get_colour(di, lighten=1))
 
     # Make a plot - custom, interactive or flat
     mod = get_template_mod()
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/box.py` & `multiqc_sgr-1.22.post0/multiqc/plots/box.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/heatmap.py` & `multiqc_sgr-1.22.post0/multiqc/plots/heatmap.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/linegraph.py` & `multiqc_sgr-1.22.post0/multiqc/plots/linegraph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ MultiQC functions to plot a linegraph """
 
 import inspect
 import logging
 import re
-from typing import List, Dict
+from typing import List, Dict, Union, Tuple
 
 from multiqc.utils import config, mqc_colour, report
 from multiqc.plots.plotly import line
 
 logger = logging.getLogger(__name__)
 
 letters = "abcdefghijklmnopqrstuvwxyz"
@@ -20,16 +20,17 @@
 def get_template_mod():
     global _template_mod
     if not _template_mod:
         _template_mod = config.avail_templates[config.template].load()
     return _template_mod
 
 
-def plot(data, pconfig=None):
-    """Plot a line graph with X,Y data.
+def plot(data: Union[List[Dict[str, List]], Dict[str, List]], pconfig=None):
+    """
+    Plot a line graph with X,Y data.
     :param data: 2D dict, first keys as sample names, then x:y data pairs
     :param pconfig: optional dict with config key:value pairs. See CONTRIBUTING.md
     :return: HTML and JS, ready to be inserted into the page
     """
     # Don't just use {} as the default argument as it's mutable. See:
     # http://python-guide-pt-br.readthedocs.io/en/latest/writing/gotchas/
     if pconfig is None:
@@ -39,191 +40,154 @@
     if "id" in pconfig and pconfig["id"] and pconfig["id"] in config.custom_plot_config:
         for k, v in config.custom_plot_config[pconfig["id"]].items():
             pconfig[k] = v
 
     # Given one dataset - turn it into a list
     if not isinstance(data, list):
         data = [data]
+    if "data_labels" in pconfig:
+        if len(pconfig["data_labels"]) != len(data):
+            raise ValueError(
+                f"Length of data_labels does not match the number of datasets. "
+                f"Please check your module code and ensure that the data_labels "
+                f"list is the same length as the data list: {len(pconfig['data_labels'])} != {len(data)}. "
+                f"pconfig={pconfig}"
+            )
+        pconfig["data_labels"] = [dl if isinstance(dl, dict) else {"name": dl} for dl in pconfig["data_labels"]]
 
     # Validate config if linting
     if config.strict:
         # Get module name
         modname = ""
         callstack = inspect.stack()
         for n in callstack:
             if "multiqc/modules/" in n[1] and "base_module.py" not in n[1]:
                 callpath = n[1].split("multiqc/modules/", 1)[-1]
                 modname = f">{callpath}< "
                 break
         # Look for essential missing pconfig keys
         for k in ["id", "title", "ylab"]:
-            if k not in pconfig:
+            if k not in pconfig and any(k not in dl for dl in pconfig.get("data_labels", [])):
                 errmsg = f"LINT: {modname}Linegraph pconfig was missing key '{k}'"
                 logger.error(errmsg)
                 report.lint_errors.append(errmsg)
         # Check plot title format
         if not re.match(r"^[^:]*\S: \S[^:]*$", pconfig.get("title", "")):
             errmsg = "LINT: {} Linegraph title did not match format 'Module: Plot Name' (found '{}')".format(
                 modname, pconfig.get("title", "")
             )
             logger.error(errmsg)
             report.lint_errors.append(errmsg)
 
     # Smooth dataset if requested in config
     if pconfig.get("smooth_points", None) is not None:
-        for i, d in enumerate(data):
-            data[i] = smooth_line_data(d, pconfig["smooth_points"])
-
-    # Add sane plotting config defaults
-    for idx, yp in enumerate(pconfig.get("yPlotLines", [])):
-        pconfig["yPlotLines"][idx]["width"] = pconfig["yPlotLines"][idx].get("width", 2)
-
-    # Add initial axis labels if defined in `data_labels` but not main config
-    if pconfig.get("ylab") is None:
-        try:
-            pconfig["ylab"] = pconfig["data_labels"][0]["ylab"]
-        except Exception:
-            pass
-    if pconfig.get("xlab") is None:
-        try:
-            pconfig["xlab"] = pconfig["data_labels"][0]["xlab"]
-        except Exception:
-            pass
-
-    # Generate the data dict structure expected by HighCharts series
-    plotdata: List[List[Dict]] = []
-    for data_index, d in enumerate(data):
-        thisplotdata: List[Dict] = []
-
-        # Ensure any overwritten conditionals from data_labels (e.g. ymax or categories) are taken in consideration
-        dataset_config = pconfig.copy()
-        if "data_labels" in pconfig and isinstance(
-            pconfig["data_labels"][data_index], dict
-        ):  # if not a dict: only dataset name is provided
-            dataset_config.update(pconfig["data_labels"][data_index])
-
-        if "categories" in dataset_config:
-            if not isinstance(pconfig["categories"], list):
-                dataset_config["categories"] = list()
-
-            # Add any new categories
-            for s in sorted(d.keys()):
-                for k in d[s].keys():
-                    if k not in dataset_config["categories"]:
-                        dataset_config["categories"].append(k)
-
-            # Save adjusted categories per-dataset
-            del pconfig["categories"]
-            if "data_labels" not in pconfig:
-                pconfig["data_labels"] = [{}] * len(data)
-            pconfig["data_labels"] = [({"name": dl} if isinstance(dl, str) else dl) for dl in pconfig["data_labels"]]
-            pconfig["data_labels"][data_index]["categories"] = dataset_config["categories"]
+        for i, data_by_sample in enumerate(data):
+            data[i] = smooth_line_data(data_by_sample, pconfig["smooth_points"])
 
-        for s in sorted(d.keys()):
+    datasets: List[List[Dict]] = []
+    for ds_idx, data_by_sample in enumerate(data):
+        this_list_of_series: List[Dict] = []
+        for s in sorted(data_by_sample.keys()):
             # Ensure any overwritten conditionals from data_labels (e.g. ymax) are taken in consideration
-            series_config = dataset_config.copy()
-            pairs = []
+            series_config = pconfig.copy()
+            pairs: List[Tuple[Union[float, int, str], Union[float, int]]] = []
             maxval = 0
-            if "categories" in series_config:
-                # Go through categories and add either data or a blank
-                for k in series_config["categories"]:
-                    try:
-                        pairs.append(d[s][k])
-                        maxval = max(maxval, d[s][k])
-                    except KeyError:
-                        pairs.append(None)
-            else:
-                # Discard > ymax or just hide?
-                # If it never comes back into the plot, discard. If it goes above then comes back, just hide.
-                discard_ymax = None
-                discard_ymin = None
-                for k in sorted(d[s].keys()):
+            x_are_categories = pconfig.get("categories", False)
+            if "data_labels" in pconfig:
+                x_are_categories = pconfig["data_labels"][ds_idx].get("categories", x_are_categories)
+            # Discard > ymax or just hide?
+            # If it never comes back into the plot, discard. If it goes above then comes back, just hide.
+            discard_ymax = None
+            discard_ymin = None
+            xs = data_by_sample[s].keys()
+            if not x_are_categories:
+                xs = sorted(xs)
+
+            for k in xs:
+                if not x_are_categories:
                     if "xmax" in series_config and float(k) > float(series_config["xmax"]):
                         continue
                     if "xmin" in series_config and float(k) < float(series_config["xmin"]):
                         continue
-                    if d[s][k] is not None and "ymax" in series_config:
-                        if float(d[s][k]) > float(series_config["ymax"]):
-                            discard_ymax = True
-                        elif discard_ymax is True:
-                            discard_ymax = False
-                    if d[s][k] is not None and "ymin" in series_config:
-                        if float(d[s][k]) > float(series_config["ymin"]):
-                            discard_ymin = True
-                        elif discard_ymin is True:
-                            discard_ymin = False
-
-                # Build the plot data structure
-                for k in sorted(d[s].keys()):
-                    if k is not None:
-                        if "xmax" in series_config and float(k) > float(series_config["xmax"]):
-                            continue
-                        if "xmin" in series_config and float(k) < float(series_config["xmin"]):
-                            continue
-                    if d[s][k] is not None:
-                        if (
-                            "ymax" in series_config
-                            and float(d[s][k]) > float(series_config["ymax"])
-                            and discard_ymax is not False
-                        ):
-                            continue
-                        if (
-                            "ymin" in series_config
-                            and float(d[s][k]) < float(series_config["ymin"])
-                            and discard_ymin is not False
-                        ):
-                            continue
-                    pairs.append([k, d[s][k]])
-                    try:
-                        maxval = max(maxval, d[s][k])
-                    except TypeError:
-                        pass
+                if data_by_sample[s][k] is not None and "ymax" in series_config:
+                    if float(data_by_sample[s][k]) > float(series_config["ymax"]):
+                        discard_ymax = True
+                    elif discard_ymax is True:
+                        discard_ymax = False
+                if data_by_sample[s][k] is not None and "ymin" in series_config:
+                    if float(data_by_sample[s][k]) > float(series_config["ymin"]):
+                        discard_ymin = True
+                    elif discard_ymin is True:
+                        discard_ymin = False
+
+            # Build the plot data structure
+            for k in xs:
+                if not x_are_categories and k is not None:
+                    if "xmax" in series_config and float(k) > float(series_config["xmax"]):
+                        continue
+                    if "xmin" in series_config and float(k) < float(series_config["xmin"]):
+                        continue
+                if data_by_sample[s][k] is not None:
+                    if (
+                        "ymax" in series_config
+                        and float(data_by_sample[s][k]) > float(series_config["ymax"])
+                        and discard_ymax is not False
+                    ):
+                        continue
+                    if (
+                        "ymin" in series_config
+                        and float(data_by_sample[s][k]) < float(series_config["ymin"])
+                        and discard_ymin is not False
+                    ):
+                        continue
+                pairs.append((k, data_by_sample[s][k]))
+                try:
+                    maxval = max(maxval, data_by_sample[s][k])
+                except TypeError:
+                    pass
             if maxval > 0 or series_config.get("hide_empty") is not True:
                 this_series: Dict = {"name": s, "data": pairs}
                 try:
                     this_series["color"] = series_config["colors"][s]
-                except Exception:
+                except KeyError:
                     pass
-                thisplotdata.append(this_series)
-        plotdata.append(thisplotdata)
+                this_list_of_series.append(this_series)
+        datasets.append(this_list_of_series)
 
     # Add on annotation data series
     try:
         if pconfig.get("extra_series"):
             extra_series = pconfig["extra_series"]
             if isinstance(pconfig["extra_series"], dict):
                 extra_series = [[pconfig["extra_series"]]]
             elif isinstance(pconfig["extra_series"], list) and isinstance(pconfig["extra_series"][0], dict):
                 extra_series = [pconfig["extra_series"]]
             for i, es in enumerate(extra_series):
                 for s in es:
-                    plotdata[i].append(s)
+                    datasets[i].append(s)
     except Exception:
         pass
 
-    # Add colors to the categories if not set. Since the "plot_defaults" scale is
-    # identical to default scale of the Highcharts JS library, this is not strictly
-    # needed. But it future proofs when we replace Highcharts with something else.
     scale = mqc_colour.mqc_colour_scale("plot_defaults")
-    for si, sd in enumerate(plotdata):
-        for di, d in enumerate(sd):
-            d.setdefault("color", scale.get_colour(di, lighten=1))
+    for si, sd in enumerate(datasets):
+        for di, data_by_sample in enumerate(sd):
+            data_by_sample.setdefault("color", scale.get_colour(di, lighten=1))
 
     # Make a plot - template custom, or interactive or flat
     mod = get_template_mod()
     if "linegraph" in mod.__dict__ and callable(mod.linegraph):
         try:
-            return mod.linegraph(plotdata, pconfig)
+            return mod.linegraph(datasets, pconfig)
         except:  # noqa: E722
             if config.strict:
                 # Crash quickly in the strict mode. This can be helpful for interactive
                 # debugging of modules
                 raise
 
-    return line.plot(plotdata, pconfig)
+    return line.plot(datasets, pconfig)
 
 
 def smooth_line_data(data: Dict[str, Dict], numpoints: int) -> Dict[str, Dict[int, int]]:
     """
     Function to take an x-y dataset and use binning to smooth to a maximum number of datapoints.
     Each datapoint in a smoothed dataset corresponds to the first point in a bin.
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/__init__.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/bar.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,89 +40,90 @@
     )
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class BarPlot(Plot):
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        cats: List[Dict]
-        samples: List[str]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            cats: List[Dict],
-            samples: List[str],
-        ) -> "BarPlot.Dataset":
-            # Need to reverse samples as the bar plot will show them reversed
-            samples = list(reversed(samples))
-            for cat in cats:
-                # Reverse the data to match the reversed samples
-                cat["data"] = list(reversed(cat["data"]))
-                if "data_pct" in cat:
-                    cat["data_pct"] = list(reversed(cat["data_pct"]))
-
-            # Post-process categories
-            for cat in cats:
-                # Split long category names
-                if "name" not in cat:
-                    raise ValueError(f"Bar plot {dataset.plot.id}: missing 'name' key in category")
-                cat["name"] = "<br>".join(split_long_string(cat["name"]))
-
-                # Reformat color to be ready to add alpha in Plotly-JS
-                color = spectra.html(cat["color"])
-                cat["color"] = ",".join([f"{x:.2f}" for x in color.rgb])
-
-                # Check that the number of samples is the same for all categories
-                assert len(samples) == len(cat["data"])
-
-            dataset = BarPlot.Dataset(
-                **dataset.__dict__,
-                cats=cats,
-                samples=samples,
-            )
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    cats: List[Dict]
+    samples: List[str]
+
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        cats: List[Dict],
+        samples: List[str],
+    ) -> "Dataset":
+        # Need to reverse samples as the bar plot will show them reversed
+        samples = list(reversed(samples))
+        for cat in cats:
+            # Reverse the data to match the reversed samples
+            cat["data"] = list(reversed(cat["data"]))
+            if "data_pct" in cat:
+                cat["data_pct"] = list(reversed(cat["data_pct"]))
+
+        # Post-process categories
+        for cat in cats:
+            # Split long category names
+            if "name" not in cat:
+                raise ValueError(f"Bar plot {dataset.plot_id}: missing 'name' key in category")
+            cat["name"] = "<br>".join(split_long_string(cat["name"]))
+
+            # Reformat color to be ready to add alpha in Plotly-JS
+            color = spectra.html(cat["color"])
+            cat["color"] = ",".join([f"{int(x * 256)}" for x in color.rgb])
+
+            # Check that the number of samples is the same for all categories
+            assert len(samples) == len(cat["data"])
+
+        dataset = Dataset(
+            **dataset.__dict__,
+            cats=cats,
+            samples=samples,
+        )
 
-            return dataset
+        return dataset
+
+    def create_figure(
+        self,
+        layout: go.Layout,
+        is_log=False,
+        is_pct=False,
+    ) -> go.Figure:
+        """
+        Create a Plotly figure for a dataset
+        """
+        fig = go.Figure(layout=layout)
+
+        for cat in self.cats:
+            data = cat["data_pct"] if is_pct else cat["data"]
+
+            params = copy.deepcopy(self.trace_params)
+            params["marker"]["color"] = f"rgb({cat['color']})"
+            fig.add_trace(
+                go.Bar(
+                    y=self.samples,
+                    x=data,
+                    name=cat["name"],
+                    **params,
+                ),
+            )
+        return fig
 
-        def create_figure(
-            self,
-            layout: go.Layout,
-            is_log=False,
-            is_pct=False,
-        ) -> go.Figure:
-            """
-            Create a Plotly figure for a dataset
-            """
-            fig = go.Figure(layout=layout)
-
-            for cat in self.cats:
-                data = cat["data_pct"] if is_pct else cat["data"]
-
-                params = copy.deepcopy(self.trace_params)
-                params["marker"]["color"] = f"rgb({cat['color']})"
-                fig.add_trace(
-                    go.Bar(
-                        y=self.samples,
-                        x=data,
-                        name=cat["name"],
-                        **params,
-                    ),
-                )
-            return fig
 
+class BarPlot(Plot):
     def __init__(self, pconfig: Dict, cats_lists: List, samples_lists: List, max_n_samples: int):
         super().__init__(PlotType.BAR, pconfig, len(cats_lists))
         if len(cats_lists) != len(samples_lists):
             raise ValueError("Number of datasets and samples lists do not match")
 
-        self.datasets: List[BarPlot.Dataset] = [
-            BarPlot.Dataset.create(d, cats=cats, samples=samples)
+        self.datasets: List[Dataset] = [
+            Dataset.create(d, cats=cats, samples=samples)
             for d, cats, samples in zip(self.datasets, cats_lists, samples_lists)
         ]
 
         # Set the barmode
         barmode = "relative"  # stacking, but drawing negative values below zero
         if "stacking" in pconfig and (pconfig["stacking"] in ["group", None]):
             barmode = "group"  # side by side
@@ -201,29 +202,33 @@
                     for i in range(len(dataset.samples))
                 )
                 xmin_cnt = min(
                     sum(cat["data"][i] if cat["data"][i] < 0 else 0 for cat in dataset.cats)
                     for i in range(len(dataset.samples))
                 )
 
+            minallowed = 0 if xmin_cnt > 0 else xmin_cnt  # allow bar to start below zero
+            maxallowed = dataset.layout["yaxis"]["autorangeoptions"]["maxallowed"]
+            if maxallowed is None:
+                maxallowed = xmax_cnt
+
             dataset.layout.update(
                 yaxis=dict(
                     title=None,
                     hoverformat=dataset.layout["xaxis"]["hoverformat"],
                     ticksuffix=dataset.layout["xaxis"]["ticksuffix"],
-                    autorangeoptions=dataset.layout["xaxis"]["autorangeoptions"],
                 ),
                 xaxis=dict(
                     title=dict(text=dataset.layout["yaxis"]["title"]["text"]),
                     hoverformat=dataset.layout["yaxis"]["hoverformat"],
                     ticksuffix=dataset.layout["yaxis"]["ticksuffix"],
-                    autorangeoptions={
-                        "minallowed": xmin_cnt,
-                        "maxallowed": xmax_cnt,
-                    },
+                    autorangeoptions=dict(
+                        minallowed=minallowed,
+                        maxallowed=maxallowed,
+                    ),
                 ),
                 showlegend=len(dataset.cats) > 1,
             )
             dataset.trace_params.update(
                 orientation="h",
                 marker=dict(line=dict(width=0)),
                 textposition="inside",
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/box.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/box.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,80 +32,80 @@
     )
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class BoxPlot(Plot):
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        data: List[BoxT]
-        samples: List[str]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            data_by_sample: Dict[str, BoxT],
-        ) -> "BoxPlot.Dataset":
-            dataset = BoxPlot.Dataset(
-                **dataset.__dict__,
-                data=list(data_by_sample.values()),
-                samples=list(data_by_sample.keys()),
-            )
-            # Need to reverse samples as the box plot will show them reversed
-            dataset.samples = list(reversed(dataset.samples))
-            dataset.data = list(reversed(dataset.data))
-
-            dataset.trace_params.update(
-                boxpoints="outliers",
-                jitter=0.5,
-                orientation="h",
-                marker=dict(
-                    color="#4899e8",  # just use blue to indicate interactivity
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    data: List[BoxT]
+    samples: List[str]
+
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        data_by_sample: Dict[str, BoxT],
+    ) -> "Dataset":
+        dataset = Dataset(
+            **dataset.__dict__,
+            data=list(data_by_sample.values()),
+            samples=list(data_by_sample.keys()),
+        )
+        # Need to reverse samples as the box plot will show them reversed
+        dataset.samples = list(reversed(dataset.samples))
+        dataset.data = list(reversed(dataset.data))
+
+        dataset.trace_params.update(
+            boxpoints="outliers",
+            jitter=0.5,
+            orientation="h",
+            marker=dict(
+                color="#4899e8",  # just use blue to indicate interactivity
+            ),
+            # to remove the redundant sample name before "median" in the unified hover box
+            hoverinfo="x",
+        )
+        dataset.layout["yaxis"]["title"] = None
+        return dataset
+
+    def create_figure(
+        self,
+        layout: go.Layout,
+        is_log=False,
+        is_pct=False,
+    ) -> go.Figure:
+        """
+        Create a Plotly figure for a dataset
+        """
+        fig = go.Figure(layout=layout)
+
+        for sname, values in zip(self.samples, self.data):
+            params = copy.deepcopy(self.trace_params)
+            fig.add_trace(
+                go.Box(
+                    x=values,
+                    name=sname,
+                    **params,
                 ),
-                # to remove the redundant sample name before "median" in the unified hover box
-                hoverinfo="x",
             )
-            dataset.layout["yaxis"]["title"] = None
-            return dataset
+        return fig
 
-        def create_figure(
-            self,
-            layout: go.Layout,
-            is_log=False,
-            is_pct=False,
-        ) -> go.Figure:
-            """
-            Create a Plotly figure for a dataset
-            """
-            fig = go.Figure(layout=layout)
-
-            for sname, values in zip(self.samples, self.data):
-                params = copy.deepcopy(self.trace_params)
-                fig.add_trace(
-                    go.Box(
-                        x=values,
-                        name=sname,
-                        **params,
-                    ),
-                )
-            return fig
 
+class BoxPlot(Plot):
     def __init__(
         self,
         pconfig: Dict,
         list_of_data_by_sample: List[Dict[str, BoxT]],
         max_n_samples: int,
     ):
         super().__init__(PlotType.BOX, pconfig, n_datasets=len(list_of_data_by_sample))
 
-        self.datasets: List[BoxPlot.Dataset] = [
-            BoxPlot.Dataset.create(ds, data_by_sample)
-            for ds, data_by_sample in zip(self.datasets, list_of_data_by_sample)
+        self.datasets: List[Dataset] = [
+            Dataset.create(ds, data_by_sample) for ds, data_by_sample in zip(self.datasets, list_of_data_by_sample)
         ]
 
         height = determine_barplot_height(max_n_samples)
 
         self.layout.update(
             height=height,
             showlegend=False,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/heatmap.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,67 +29,68 @@
     p = HeatmapPlot(rows, pconfig, xcats, ycats)
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class HeatmapPlot(Plot):
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        rows: List[List[ElemT]]
-        xcats: List[str]
-        ycats: List[str]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            rows: Union[List[List[ElemT]], Dict[str, Dict[str, ElemT]]],
-            xcats: Optional[List[str]] = None,
-            ycats: Optional[List[str]] = None,
-        ) -> "HeatmapPlot.Dataset":
-            if isinstance(rows, dict):
-                # Convert dict to a list of lists
-                if not ycats:
-                    ycats = list(rows.keys())
-                if not xcats:
-                    xcats = []
-                    for y, value_by_x in rows.items():
-                        for x, value in value_by_x.items():
-                            if x not in xcats:
-                                xcats.append(x)
-                rows = [[rows.get(y, {}).get(x) for x in xcats] for y in ycats]
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    rows: List[List[ElemT]]
+    xcats: List[str]
+    ycats: List[str]
+
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        rows: Union[List[List[ElemT]], Dict[str, Dict[str, ElemT]]],
+        xcats: Optional[List[str]] = None,
+        ycats: Optional[List[str]] = None,
+    ) -> "Dataset":
+        if isinstance(rows, dict):
+            # Convert dict to a list of lists
+            if not ycats:
+                ycats = list(rows.keys())
+            if not xcats:
+                xcats = []
+                for y, value_by_x in rows.items():
+                    for x, value in value_by_x.items():
+                        if x not in xcats:
+                            xcats.append(x)
+            rows = [[rows.get(y, {}).get(x) for x in xcats] for y in ycats]
+
+        dataset = Dataset(
+            **dataset.__dict__,
+            rows=rows,
+            xcats=xcats,
+            ycats=ycats,
+        )
+        return dataset
 
-            dataset = HeatmapPlot.Dataset(
-                **dataset.__dict__,
-                rows=rows,
-                xcats=xcats,
-                ycats=ycats,
-            )
-            return dataset
+    def create_figure(
+        self,
+        layout: Optional[go.Layout] = None,
+        is_log=False,
+        is_pct=False,
+    ) -> go.Figure:
+        """
+        Create a Plotly figure for a dataset
+        """
+        return go.Figure(
+            data=go.Heatmap(
+                z=self.rows,
+                x=self.xcats,
+                y=self.ycats,
+                **self.trace_params,
+            ),
+            layout=layout or self.layout,
+        )
 
-        def create_figure(
-            self,
-            layout: Optional[go.Layout] = None,
-            is_log=False,
-            is_pct=False,
-        ) -> go.Figure:
-            """
-            Create a Plotly figure for a dataset
-            """
-            return go.Figure(
-                data=go.Heatmap(
-                    z=self.rows,
-                    x=self.xcats,
-                    y=self.ycats,
-                    **self.trace_params,
-                ),
-                layout=layout or self.layout,
-            )
 
+class HeatmapPlot(Plot):
     def __init__(
         self,
         rows: Union[List[List[ElemT]], Dict[str, Dict[str, ElemT]]],
         pconfig: Dict,
         xcats: Optional[List[str]],
         ycats: Optional[List[str]],
     ):
@@ -118,16 +119,16 @@
             ),
             showlegend=pconfig.get("legend", True),
         )
 
         self.square = pconfig.get("square", True)  # Keep heatmap cells square
 
         # Extend each dataset object with a list of samples
-        self.datasets: List[HeatmapPlot.Dataset] = [
-            HeatmapPlot.Dataset.create(
+        self.datasets: List[Dataset] = [
+            Dataset.create(
                 self.datasets[0],
                 rows=rows,
                 xcats=xcats,
                 ycats=ycats,
             )
         ]
 
@@ -254,15 +255,15 @@
                 [0.6, "#fee090"],
                 [0.7, "#fdae61"],
                 [0.8, "#f46d43"],
                 [0.9, "#d73027"],
                 [1, "#a50026"],
             ]
 
-        decimal_places = pconfig.get("decimalPlaces", 2)
+        decimal_places = pconfig.get("tt_decimals", 2)
 
         xlab = pconfig.get("xlab", "x")
         ylab = pconfig.get("ylab", "y")
         zlab = pconfig.get("zlab", "z")
         hovertemplate = f"{xlab}: %{{x}}<br>{ylab}: %{{y}}<br>{zlab}: %{{z}}<extra></extra>"
 
         for ds in self.datasets:
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/line.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/line.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import dataclasses
 import io
 import logging
 import os
-from typing import Dict, List, Union, Optional
+from typing import Dict, List, Union, Optional, Tuple
+
+import math
 import plotly.graph_objects as go
 
 from multiqc.plots.plotly.plot import Plot, PlotType, BaseDataset
 from multiqc.utils import util_functions, config
 from multiqc.utils.config import update_dict
 
 logger = logging.getLogger(__name__)
 
 
 # {"name": "SAMPLE1", "color": "#111111", "data": [[x, y], [x, y], ...]}
-LineT = Dict[str, Union[str, List[List[float]]]]
+LineT = Dict[str, Union[str, List[Tuple[Union[float, int, str], Union[float, int]]]]]
 
 
 def plot(lists_of_lines: List[List[LineT]], pconfig: Dict) -> str:
     """
     Build and add the plot data to the report, return an HTML wrapper.
     :param lists_of_lines: each dataset is a 2D dict, first keys as sample names, then x:y data pairs
     :param pconfig: dict with config key:value pairs. See CONTRIBUTING.md
@@ -33,178 +35,183 @@
     p = LinePlot(pconfig, lists_of_lines)
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class LinePlot(Plot):
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        lines: List[Dict]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            lines: List[Dict],
-            pconfig: Dict,
-        ) -> "LinePlot.Dataset":
-            dataset = LinePlot.Dataset(
-                **dataset.__dict__,
-                lines=lines,
-            )
-            dataset.dconfig["categories"] = dataset.dconfig.get("categories", pconfig.get("categories", []))
-            if dataset.dconfig["categories"]:
-                # Prevent JavaScript from automatically parsing categorical values as numbers
-                dataset.layout["xaxis"]["type"] = "category"
-                # check that all lines have the same number of categories
-                assert all(
-                    len(line["data"]) == len(dataset.dconfig["categories"]) for line in dataset.lines
-                ), dataset.uid
-
-            # convert HighCharts hardcoded trace parameters to Plotly
-            lines = []
-            for src_line in dataset.lines:
-                new_line = {
-                    "name": src_line["name"],
-                    "data": src_line["data"],
-                    "color": src_line.get("color"),
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    lines: List[Dict]
+
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        lines: List[Dict],
+        pconfig: Dict,
+    ) -> "Dataset":
+        dataset: Dataset = Dataset(
+            **dataset.__dict__,
+            lines=lines,
+        )
+
+        # Prevent Plotly from parsing strings as numbers
+        if pconfig.get("categories") or dataset.dconfig.get("categories"):
+            dataset.layout["xaxis"]["type"] = "category"
+
+        # convert HighCharts-style hardcoded trace parameters to Plotly style
+        lines = []
+        for src_line in dataset.lines:
+            new_line = {
+                "name": src_line["name"],
+                "data": src_line["data"],
+                "color": src_line.get("color"),
+                "showlegend": src_line.get("showlegend", src_line.get("showInLegend", True)),
+                "line": {
+                    "dash": convert_dash_style(src_line.get("dash", src_line.get("dashStyle"))),
+                    "width": src_line.get("line", {}).get("width", src_line.get("lineWidth")),
+                },
+            }
+            if "marker" in src_line:
+                new_line["mode"] = "lines+markers"
+                new_line["marker"] = {
+                    "symbol": src_line["marker"].get("symbol"),
+                    "line": {
+                        "width": src_line["marker"].get("line", {}).get("width", src_line["marker"].get("lineWidth")),
+                        "color": src_line["marker"].get("line", {}).get("color", src_line["marker"].get("lineColor")),
+                    },
                 }
-                lines.append(new_line)
-                new_line["marker"] = {}
-                if "dashStyle" in src_line:
-                    new_line["line"] = new_line.get("line", {})
-                    new_line["line"]["dash"] = convert_dash_style(src_line["dashStyle"])
-                if "lineWidth" in src_line:
-                    new_line["line"] = new_line.get("line", {})
-                    new_line["line"]["width"] = src_line["lineWidth"]
-                if "showInLegend" in src_line:
-                    new_line["showlegend"] = src_line["showInLegend"]
-                if "marker" in src_line:
-                    new_line["marker"] = new_line.get("marker", {})
-                    new_line["marker"]["line"] = new_line["marker"].get("line", {})
-                    if "lineWidth" in src_line["marker"]:
-                        new_line["marker"]["line"]["width"] = src_line["marker"]["lineWidth"]
-                    if "lineColor" in src_line["marker"]:
-                        new_line["marker"]["line"]["color"] = src_line["marker"]["lineColor"]
-                    if "symbol" in src_line["marker"]:
-                        new_line["mode"] = "lines+markers"
-                        new_line["marker"]["symbol"] = src_line["marker"]["symbol"]
-            dataset.lines = lines
-            # Update default trace parameters
+            lines.append(remove_nones_and_empty_dicts(new_line))
+
+        dataset.lines = lines
+
+        mode = pconfig.get("style", "lines")
+        if config.lineplot_style == "lines+markers":
+            mode = "lines+markers"
+
+        dataset.trace_params.update(
+            mode=mode,
+            line={"width": 2},
+        )
+        if mode == "lines+markers":
             dataset.trace_params.update(
-                mode="lines" if config.lineplot_style == "lines" else "lines+markers",
-                line={"width": 2 if config.lineplot_style == "lines" else 0.6},
-                marker={"size": 4},
+                line={"width": 0.6},
+                marker={"size": 5},
             )
-            return dataset
+        return dataset
 
-        def create_figure(
-            self,
-            layout: go.Layout,
-            is_log=False,
-            is_pct=False,
-        ) -> go.Figure:
-            """
-            Create a Plotly figure for a dataset
-            """
-            if self.plot.flat:
-                layout.height += len(self.lines) * 5  # extra space for legend
-
-            fig = go.Figure(layout=layout)
-            for line in self.lines:
-                if len(line["data"]) > 0 and isinstance(line["data"][0], list):
-                    xs = [x[0] for x in line["data"]]
-                    ys = [x[1] for x in line["data"]]
-                elif self.dconfig.get("categories"):
-                    assert len(line["data"]) == len(self.dconfig["categories"])
-                    xs = self.dconfig["categories"]
-                    ys = line["data"]
-                else:
-                    xs = [x for x in range(len(line["data"]))]
-                    ys = line["data"]
+    def create_figure(
+        self,
+        layout: go.Layout,
+        is_log=False,
+        is_pct=False,
+    ) -> go.Figure:
+        """
+        Create a Plotly figure for a dataset
+        """
+        layout.height += len(self.lines) * 5  # extra space for legend
 
-                params = dict(
-                    marker=line.get("marker", {}),
-                    line=line.get("line", {}),
-                    showlegend=line.get("showlegend", None),
-                    mode=line.get("mode", None),
-                )
-                params = update_dict(params, self.trace_params, none_only=True)
-                params["marker"]["color"] = line.get("color")
+        fig = go.Figure(layout=layout)
+        for line in self.lines:
+            xs = [x[0] for x in line["data"]]
+            ys = [x[1] for x in line["data"]]
+            params = dict(
+                marker=line.get("marker", {}),
+                line=line.get("line", {}),
+                showlegend=line.get("showlegend", None),
+                mode=line.get("mode", None),
+            )
+            params = update_dict(params, self.trace_params, none_only=True)
+            params["marker"]["color"] = line.get("color")
 
-                fig.add_trace(
-                    go.Scatter(
-                        x=xs,
-                        y=ys,
-                        name=line["name"],
-                        text=[line["name"]] * len(xs),
-                        **params,
-                    )
+            fig.add_trace(
+                go.Scatter(
+                    x=xs,
+                    y=ys,
+                    name=line["name"],
+                    text=[line["name"]] * len(xs),
+                    **params,
                 )
-            return fig
+            )
+        return fig
 
+
+class LinePlot(Plot):
     def __init__(self, pconfig: Dict, lists_of_lines: List[List[LineT]]):
         super().__init__(PlotType.LINE, pconfig, len(lists_of_lines))
 
-        self.datasets: List[LinePlot.Dataset] = [
-            LinePlot.Dataset.create(d, lines, pconfig) for d, lines in zip(self.datasets, lists_of_lines)
+        self.datasets: List[Dataset] = [
+            Dataset.create(d, lines, pconfig) for d, lines in zip(self.datasets, lists_of_lines)
         ]
 
         # Make a tooltip always show on hover over any point on plot
         self.layout.hoverdistance = -1
 
-        y_min_range = pconfig.get("yMinRange")
-        y_bands = pconfig.get("yPlotBands")
-        x_bands = pconfig.get("xPlotBands")
-        x_lines = pconfig.get("xPlotLines")
-        y_lines = pconfig.get("yPlotLines")
-        if y_min_range or y_bands or y_lines:
+        y_minrange = pconfig.get("y_minrange", pconfig.get("yMinRange"))
+        x_minrange = pconfig.get("x_minrange", pconfig.get("xMinRange"))
+        y_bands = pconfig.get("y_bands", pconfig.get("yPlotBands"))
+        x_bands = pconfig.get("x_bands", pconfig.get("xPlotBands"))
+        x_lines = pconfig.get("x_lines", pconfig.get("xPlotLines"))
+        y_lines = pconfig.get("y_lines", pconfig.get("yPlotLines"))
+        if y_minrange or y_bands or y_lines:
             # We don't want the bands to affect the calculated axis range, so we
-            # find the min and the max from data points, and manually set the range
+            # find the min and the max from data points, and manually set the range.
             for dataset in self.datasets:
-                ymin = dataset.layout["yaxis"]["autorangeoptions"]["clipmin"]
-                if ymin is None:
-                    ymin = dataset.layout["yaxis"]["autorangeoptions"]["minallowed"]
-                ymax = dataset.layout["yaxis"]["autorangeoptions"]["clipmax"]
-                if ymax is None:
-                    ymax = dataset.layout["yaxis"]["autorangeoptions"]["maxallowed"]
-                if ymin is None or ymax is None:
-                    for line in dataset.lines:
-                        if len(line["data"]) > 0 and isinstance(line["data"][0], list):
-                            ys = [x[1] for x in line["data"]]
-                        else:
-                            ys = line["data"]
-                        if ymin is None:
-                            ymin = min(ys)
-                        if ymax is None:
-                            ymax = max(ys)
-                            ymax += (ymax - ymin) * 0.05
-                dataset.layout["yaxis"]["range"] = [ymin, ymax]
+                minval = None
+                maxval = None
+                for line in dataset.lines:
+                    ys = [x[1] for x in line["data"]]
+                    if len(ys) > 0:
+                        minval = min(ys) if minval is None else min(minval, min(ys))
+                        maxval = max(ys) if maxval is None else max(maxval, max(ys))
+                if maxval is not None and minval is not None:
+                    maxval += (maxval - minval) * 0.05
+                if minval is None:
+                    minval = dataset.layout["yaxis"]["autorangeoptions"]["minallowed"]
+                if maxval is None:
+                    maxval = dataset.layout["yaxis"]["autorangeoptions"]["maxallowed"]
+                clipmin = dataset.layout["yaxis"]["autorangeoptions"]["clipmin"]
+                clipmax = dataset.layout["yaxis"]["autorangeoptions"]["clipmax"]
+                if clipmin is not None and minval is not None and clipmin > minval:
+                    minval = clipmin
+                if clipmax is not None and maxval is not None and clipmax < maxval:
+                    maxval = clipmax
+                if y_minrange is not None and maxval is not None and minval is not None:
+                    maxval = max(maxval, minval + y_minrange)
+                if self.layout.yaxis.type == "log":
+                    minval = math.log10(minval) if minval is not None and minval > 0 else None
+                    maxval = math.log10(maxval) if maxval is not None and maxval > 0 else None
+                dataset.layout["yaxis"]["range"] = [minval, maxval]
 
-        if x_bands or x_lines:
+        if not pconfig.get("categories", False) and x_minrange or x_bands or x_lines:
             # same as above but for x-axis
             for dataset in self.datasets:
-                xmin = dataset.layout["xaxis"]["autorangeoptions"]["clipmin"]
-                if xmin is None:
-                    xmin = dataset.layout["xaxis"]["autorangeoptions"]["minallowed"]
-                xmax = dataset.layout["xaxis"]["autorangeoptions"]["clipmax"]
-                if xmax is None:
-                    xmax = dataset.layout["xaxis"]["autorangeoptions"]["maxallowed"]
-                if xmin is None or xmax is None:
-                    for line in dataset.lines:
-                        if len(line["data"]) > 0 and isinstance(line["data"][0], list):
-                            xs = [x[0] for x in line["data"]]
-                        else:
-                            xs = [x for x in range(len(line["data"]))]
-                        if xmin is None:
-                            xmin = min(xs)
-                        if xmax is None:
-                            xmax = max(xs)
-                dataset.layout["xaxis"]["range"] = [xmin, xmax]
+                minval = None
+                maxval = None
+                for line in dataset.lines:
+                    xs = [x[0] for x in line["data"]]
+                    if len(xs) > 0:
+                        minval = min(xs) if minval is None else min(minval, min(xs))
+                        maxval = max(xs) if maxval is None else max(maxval, max(xs))
+                if minval is None:
+                    minval = dataset.layout["xaxis"]["autorangeoptions"]["minallowed"]
+                if maxval is None:
+                    maxval = dataset.layout["xaxis"]["autorangeoptions"]["maxallowed"]
+                clipmin = dataset.layout["xaxis"]["autorangeoptions"]["clipmin"]
+                clipmax = dataset.layout["xaxis"]["autorangeoptions"]["clipmax"]
+                if clipmin is not None and minval is not None and clipmin > minval:
+                    minval = clipmin
+                if clipmax is not None and maxval is not None and clipmax < maxval:
+                    maxval = clipmax
+                if x_minrange is not None and maxval is not None and minval is not None:
+                    maxval = max(maxval, minval + x_minrange)
+                if self.layout.xaxis.type == "log":
+                    minval = math.log10(minval) if minval is not None and minval > 0 else None
+                    maxval = math.log10(maxval) if maxval is not None and maxval > 0 else None
+                dataset.layout["xaxis"]["range"] = [minval, maxval]
 
         self.layout.shapes = (
             [
                 dict(
                     type="rect",
                     y0=band["from"],
                     y1=band["to"],
@@ -241,16 +248,16 @@
                     xref="paper",
                     yref="y",
                     x0=0,
                     y0=line["value"],
                     x1=1,
                     y1=line["value"],
                     line={
-                        "width": line["width"],
-                        "dash": convert_dash_style(line.get("dashStyle")),
+                        "width": line.get("width", 2),
+                        "dash": convert_dash_style(line.get("dash", line.get("dashStyle"))),
                         "color": line["color"],
                     },
                 )
                 for line in (y_lines or [])
             ]
             + [
                 dict(
@@ -258,16 +265,16 @@
                     yref="paper",
                     xref="x",
                     x0=line["value"],
                     y0=0,
                     x1=line["value"],
                     y1=1,
                     line={
-                        "width": line["width"],
-                        "dash": convert_dash_style(line.get("dashStyle")),
+                        "width": line.get("width", 2),
+                        "dash": convert_dash_style(line.get("dash", line.get("dashStyle"))),
                         "color": line["color"],
                     },
                 )
                 for line in (x_lines or [])
             ]
         )
 
@@ -320,20 +327,32 @@
                 f.write(fout.encode("utf-8", "ignore").decode("utf-8"))
         else:
             util_functions.write_data_file(y_by_x_by_sample, dataset.uid)
 
 
 def convert_dash_style(dash_style: str) -> str:
     """Convert dash style from Highcharts to Plotly"""
-    return {
+    mapping = {
         "Solid": "solid",
         "ShortDash": "dash",
         "ShortDot": "dot",
         "ShortDashDot": "dashdot",
         "ShortDashDotDot": "dashdot",
         "Dot": "dot",
         "Dash": "dash",
         "DashDot": "dashdot",
         "LongDash": "longdash",
         "LongDashDot": "longdashdot",
         "LongDashDotDot": "longdashdot",
-    }.get(dash_style, "solid")
+    }
+    if dash_style in mapping.values():  # Plotly style?
+        return dash_style
+    elif dash_style in mapping.keys():  # Highcharts style?
+        return mapping[dash_style]
+    return "solid"
+
+
+def remove_nones_and_empty_dicts(d: Dict) -> Dict:
+    """Remove None and empty dicts from a dict recursively."""
+    if not isinstance(d, Dict):
+        return d
+    return {k: remove_nones_and_empty_dicts(v) for k, v in d.items() if v is not None and v != {}}
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/plot.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,26 +34,24 @@
 
 @dataclasses.dataclass
 class BaseDataset(ABC):
     """
     Structured version of dataset config dictionary
     """
 
-    plot: "Plot"
+    plot_id: str
     label: str
     uid: str
     dconfig: Dict  # user dataset-specific configuration
     layout: Dict  # update when a datasets toggle is clicked, or percentage switch is unselected
     trace_params: Dict
     pct_range: Dict
 
     def dump_for_javascript(self) -> Dict:
-        d = {k: v for k, v in self.__dict__.items()}
-        del d["plot"]
-        return d
+        return {k: v for k, v in self.__dict__.items()}
 
     def create_figure(self, layout: go.Layout, is_log=False, is_pct=False):
         """
         To be overridden by specific plots: create a Plotly figure for a dataset, update layout if needed.
         """
         raise NotImplementedError
 
@@ -93,15 +91,15 @@
         self.add_pct_tab = pconfig.get("cpswitch", True) is not False and plot_type == PlotType.BAR
         self.l_active = self.add_log_tab and pconfig.get("logswitch_active") is True
         self.p_active = self.add_pct_tab and pconfig.get("cpswitch_c_active", True) is not True
 
         # Per-dataset configurations
         self.datasets: List[BaseDataset] = [
             BaseDataset(
-                self,
+                plot_id=self.id,
                 label=str(i + 1),
                 uid=self.id,
                 dconfig=dict(),
                 layout=dict(),
                 trace_params=dict(),
                 pct_range=dict(  # range for the percentage view for each axis
                     xaxis=dict(min=0, max=100),
@@ -180,20 +178,20 @@
         # Layout update for the counts/percentage switch
         self.pct_axis_update = dict(
             ticksuffix="%",
             hoverformat=".1f",
         )
 
         self._axis_controlled_by_switches = self.axis_controlled_by_switches()
-        if self.pconfig.get("xLog"):
-            self.layout.xaxis.type = "log"
+        if self.pconfig.get("xlog", self.pconfig.get("xLog")):
+            self._set_axis_log_scale(self.layout.xaxis)
             if "xaxis" in self._axis_controlled_by_switches:
                 self._axis_controlled_by_switches.remove("xaxis")
-        if self.pconfig.get("yLog"):
-            self.layout.yaxis.type = "log"
+        if self.pconfig.get("ylog", self.pconfig.get("yLog")):
+            self._set_axis_log_scale(self.layout.yaxis)
             if "yaxis" in self._axis_controlled_by_switches:
                 self._axis_controlled_by_switches.remove("yaxis")
         if self.add_log_tab and self.l_active:
             for axis in self._axis_controlled_by_switches:
                 self.layout[axis].type = "log"
 
         dconfigs: List[Union[str, Dict[str, str]]] = pconfig.get("data_labels", [])
@@ -213,14 +211,24 @@
             if "ylab" not in dconfig and "ylab" not in self.pconfig:
                 dconfig["ylab"] = dconfig.get("name", dconfig.get("label"))
 
             dataset.layout, dataset.trace_params = _dataset_layout(pconfig, dconfig, self.tt_label())
             dataset.dconfig = dconfig
 
     @staticmethod
+    def _set_axis_log_scale(axis):
+        axis.type = "log"
+        minval = axis.autorangeoptions["minallowed"]
+        maxval = axis.autorangeoptions["maxallowed"]
+        minval = math.log10(minval) if minval is not None and minval > 0 else None
+        maxval = math.log10(maxval) if maxval is not None and maxval > 0 else None
+        axis.autorangeoptions["minallowed"] = minval
+        axis.autorangeoptions["maxallowed"] = maxval
+
+    @staticmethod
     def axis_controlled_by_switches() -> List[str]:
         """
         Return a list of axis names that are controlled by the log10 scale and percentage
         switch buttons, e.g. ["yaxis"]
         """
         return []
 
@@ -244,14 +252,16 @@
             if len(self.datasets) > 1:  # for flat plots, each dataset will have its own unique ID
                 ds.uid = report.save_htmlid(f"{self.id}_{ds.label}", skiplint=True)
 
         if self.flat:
             html = self.flat_plot()
         else:
             html = self.interactive_plot(report)
+            if config.export_plots:
+                self.flat_plot()
         return html
 
     def interactive_plot(self, report) -> str:
         html = '<div class="mqc_hcplot_plotgroup">'
 
         html += self.__control_panel()
 
@@ -275,15 +285,15 @@
 
     def flat_plot(self) -> str:
         html = "".join(
             [
                 '<p class="text-info">',
                 "<small>" '<span class="glyphicon glyphicon-picture" aria-hidden="true"></span> ',
                 "Flat image plot. Toolbox functions such as highlighting / hiding samples will not work ",
-                '(see the <a href="http://multiqc.info/docs/#flat--interactive-plots" target="_blank">docs</a>).',
+                '(see the <a href="https://multiqc.info/docs/development/plots/#interactive--flat-image-plots" target="_blank">docs</a>).',
                 "</small>",
                 "</p>",
             ]
         )
         html += f'<div class="mqc_mplplot_plotgroup" id="plotgroup-{self.id}" data-pid={self.id}>'
 
         if not config.simple_output:
@@ -552,39 +562,75 @@
     Given plot config and dataset config, set layout and trace params.
     """
     pconfig = pconfig.copy()
     pconfig.update(dconfig)
 
     # Format on-hover tooltips
     ysuffix = pconfig.get("ysuffix", pconfig.get("tt_suffix"))
-    ylabformat = pconfig.get("ylab_format", pconfig.get("yLabFormat"))
-    if ylabformat and "%" in ylabformat:
-        ysuffix = "%"
-
     xsuffix = pconfig.get("xsuffix")
+
+    # Options deprecated in 1.21
+    ylabformat = pconfig.get("ylab_format", pconfig.get("yLabFormat"))
+    if ysuffix is None and ylabformat:
+        if "}" in ylabformat:
+            ysuffix = ylabformat.split("}")[1]
     xlabformat = pconfig.get("xlab_format", pconfig.get("xLabFormat"))
-    if xlabformat and "%" in xlabformat:
-        xsuffix = "%"
+    if xsuffix is None and xlabformat:
+        if "}" in xlabformat:
+            xsuffix = xlabformat.split("}")[1]
+
+    # Set or remove space in known suffixes
+    KNOWN_SUFFIXES = ["%", "x", "X", "k", "M", " bp", " kbp", " Mbp"]
+    for suf in KNOWN_SUFFIXES:
+        if ysuffix is not None and ysuffix == suf.strip():
+            ysuffix = suf
+        if xsuffix is not None and xsuffix == suf.strip():
+            xsuffix = suf
+
+    # Set % suffix from ylab if it's in form like "% reads"
+    ylab = pconfig.get("ylab")
+    xlab = pconfig.get("xlab")
+    if ysuffix is None and ylab:
+        if "%" in ylab or "percentage" in ylab.lower():
+            ysuffix = "%"
+        for suf in KNOWN_SUFFIXES:
+            if ylab.endswith(f" ({suf.strip()})"):
+                ysuffix = suf
+    if xsuffix is None and xlab:
+        if "%" in xlab or "percentage" in xlab.lower():
+            xsuffix = "%"
+        for suf in KNOWN_SUFFIXES:
+            if xlab.endswith(f" ({suf.strip()})"):
+                xsuffix = suf
 
     if "tt_label" in pconfig:
-        # clean label, add missing <br> into the beginning, and populate tt_suffix if missing
+        # Clean the hover tooltip label, add missing <br> into the beginning, populate suffixes if missing
         tt_label = pconfig["tt_label"]
         tt_label = _clean_config_tt_label(tt_label)
 
-        # if "%" character is inside the Y label, add suffix to the Y ticks as well
-        parts = tt_label.split("%{")
-        for part in parts:
-            if ysuffix is None and part.startswith("y") and "}" in part:
-                ysuffix = part.split("}")[1].replace("</b>", "").replace(":", "").rstrip()
-                if "," in ysuffix:
-                    ysuffix = ysuffix.split(",")[0]
-            elif xsuffix is None and part.startswith("x") and "}" in part:
-                xsuffix = part.split("}")[1].replace("</b>", "").replace(":", "").rstrip()
-                if "," in xsuffix:
-                    xsuffix = xsuffix.split(",")[0]
+        if ysuffix is None or xsuffix is None:
+            # if "%" or other suffix is in the hover label, parse that suffix to add it to the ticks
+            parts = tt_label.split("%{")
+            for part in parts:
+                if ysuffix is None and part.startswith("y") and "}" in part:
+                    info = part.split("}")[1].replace("</b>", "")
+                    info = info.split(":")[0].split(",")[0].strip().split(" ")[0]
+                    if info:
+                        for suf in KNOWN_SUFFIXES:
+                            if info == suf.strip():
+                                ysuffix = suf
+                                break
+                elif xsuffix is None and part.startswith("x") and "}" in part:
+                    info = part.split("}")[1].replace("</b>", "")
+                    info = info.split(":")[0].split(",")[0].strip().split(" ")[0]
+                    if info:
+                        for suf in KNOWN_SUFFIXES:
+                            if info == suf.strip():
+                                xsuffix = suf
+                                break
 
         # As the suffix will be added automatically for the simple format ({y}), remove it from the label
         if ysuffix is not None and "{y}" + ysuffix in tt_label:
             tt_label = tt_label.replace("{y}" + ysuffix, "{y}")
         if xsuffix is not None and "{x}" + xsuffix in tt_label:
             tt_label = tt_label.replace("{x}" + xsuffix, "{x}")
 
@@ -596,39 +642,42 @@
 
     if tt_label:
         hovertemplate = "<b>%{text}</b>" + tt_label + "<extra></extra>"
     else:
         hovertemplate = None
 
     # `hoverformat` describes how plain "{y}" or "{x}" are formatted in `hovertemplate`
-    tt_decimals = pconfig.get("tt_decimals", pconfig.get("decimalPlaces"))
-    y_hoverformat = f",.{tt_decimals}f" if tt_decimals is not None else None
+    y_decimals = pconfig.get("tt_decimals", pconfig.get("y_decimals", pconfig.get("decimalPlaces")))
+    y_hoverformat = f",.{y_decimals}f" if y_decimals is not None else None
+
+    x_decimals = pconfig.get("x_decimals")
+    x_hoverformat = f",.{x_decimals}f" if x_decimals is not None else None
 
     layout = dict(
         title=dict(text=pconfig.get("title")),
         xaxis=dict(
-            hoverformat=None,
+            hoverformat=x_hoverformat,
             ticksuffix=xsuffix or "",
             title=dict(text=pconfig.get("xlab")),
             rangemode="tozero" if pconfig.get("xmin") == 0 else "normal",
             autorangeoptions=dict(
-                clipmin=pconfig.get("xFloor"),
-                clipmax=pconfig.get("xCeiling"),
+                clipmin=pconfig.get("x_clipmin", pconfig.get("xFloor")),
+                clipmax=pconfig.get("x_clipmax", pconfig.get("xCeiling")),
                 minallowed=pconfig.get("xmin"),
                 maxallowed=pconfig.get("xmax"),
             ),
         ),
         yaxis=dict(
             hoverformat=y_hoverformat,
             ticksuffix=ysuffix or "",
             title=dict(text=pconfig.get("ylab")),
             rangemode="tozero" if pconfig.get("ymin") == 0 == 0 else "normal",
             autorangeoptions=dict(
-                clipmin=pconfig.get("yFloor"),
-                clipmax=pconfig.get("yCeiling"),
+                clipmin=pconfig.get("y_clipmin", pconfig.get("yFloor")),
+                clipmax=pconfig.get("y_clipmax", pconfig.get("yCeiling")),
                 minallowed=pconfig.get("ymin"),
                 maxallowed=pconfig.get("ymax"),
             ),
         ),
     )
 
     trace_params = {}
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/scatter.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/scatter.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,165 +27,161 @@
     p = ScatterPlot(pconfig, points_lists)
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class ScatterPlot(Plot):
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        points: List[PointT]
-        categories: List[str]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            points: List[Dict],
-            pconfig: Dict,
-        ) -> "ScatterPlot.Dataset":
-            dataset = ScatterPlot.Dataset(
-                **dataset.__dict__,
-                points=points,
-                categories=pconfig.get("categories", []),
-            )
-
-            dataset.trace_params.update(
-                textfont=dict(size=8),
-                marker=dict(
-                    size=10,
-                    line=dict(width=1),
-                    opacity=1,
-                    color="rgba(124, 181, 236, .5)",
-                ),
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    points: List[PointT]
+
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        points: List[Dict],
+        pconfig: Dict,
+    ) -> "Dataset":
+        dataset = Dataset(
+            **dataset.__dict__,
+            points=points,
+        )
+
+        dataset.trace_params.update(
+            textfont=dict(size=8),
+            marker=dict(
+                size=10,
+                line=dict(width=1),
+                opacity=1,
+                color="rgba(124, 181, 236, .5)",
+            ),
+        )
+
+        # if categories is provided, set them as x-axis ticks
+        categories = pconfig.get("categories")
+        if categories:
+            dataset.layout["xaxis"]["tickmode"] = "array"
+            dataset.layout["xaxis"]["tickvals"] = list(range(len(categories)))
+            dataset.layout["xaxis"]["ticktext"] = categories
+
+        return dataset
+
+    def create_figure(
+        self,
+        layout: Optional[go.Layout] = None,
+        is_log=False,
+        is_pct=False,
+    ) -> go.Figure:
+        """
+        Create a Plotly figure for a dataset
+        """
+        fig = go.Figure(layout=layout)
+
+        MAX_ANNOTATIONS = 10  # Maximum number of dots to be annotated directly on the plot
+        n_annotated = len([el for el in self.points if "annotation" in el])
+        if n_annotated < MAX_ANNOTATIONS:
+            # Finding and marking outliers to only label them
+            # 1. Calculate Z-scores
+            points = [(i, x) for i, x in enumerate(self.points) if x.get("annotate", True) is not False]
+            x_values = np.array([x["x"] for (i, x) in points])
+            y_values = np.array([x["y"] for (i, x) in points])
+            x_std = np.std(x_values)
+            y_std = np.std(y_values)
+            if x_std == 0 and y_std == 0:
+                logger.warning(f"Scatter plot {self.plot_id}: all {len(points)} points have the same coordinates")
+                if len(points) == 1:  # Only single point - annotate it!
+                    for i, point in points:
+                        point["annotation"] = point["name"]
+            else:
+                x_z_scores = np.abs((x_values - np.mean(x_values)) / x_std) if x_std else np.zeros_like(x_values)
+                y_z_scores = np.abs((y_values - np.mean(y_values)) / y_std) if y_std else np.zeros_like(y_values)
+                # 2. Find a reasonable threshold so there are not too many outliers
+                threshold = 1.0
+                while threshold <= 6.0:
+                    n_outliers = np.count_nonzero((x_z_scores > threshold) | (y_z_scores > threshold))
+                    logger.debug(f"Scatter plot outlier threshold: {threshold:.2f}, outliers: {n_outliers}")
+                    if n_annotated + n_outliers <= MAX_ANNOTATIONS:
+                        break
+                    # If there are too many outliers, we increase the threshold until we have less than 10
+                    threshold += 0.2
+                # 3. Annotate outliers that pass the threshold
+                for (i, point), x_z_score, y_z_score in zip(points, x_z_scores, y_z_scores):
+                    # Check if point is an outlier or if total points are less than 10
+                    if x_z_score > threshold or y_z_score > threshold:
+                        point["annotation"] = point["name"]
+            n_annotated = len([point for point in self.points if "annotation" in point])
+
+        # If there are few unique colors, we can additionally put a unique list into a legend
+        # (even though some color might belong to many distinct names - we will just crop the list)
+        names_by_legend_key = defaultdict(set)
+        for el in self.points:
+            legend_key = (el.get("color"), el.get("marker_size"), el.get("marker_line_width"), el.get("group"))
+            names_by_legend_key[legend_key].add(el["name"])
+        layout.showlegend = True
+
+        in_legend = set()
+        for element in self.points:
+            x = element["x"]
+            name = element["name"]
+            group = element.get("group")
+            color = element.get("color")
+            annotation = element.get("annotation")
+
+            show_in_legend = False
+            if layout.showlegend and not element.get("hide_in_legend"):
+                key = (color, element.get("marker_size"), element.get("marker_line_width"), group)
+                if key not in in_legend:
+                    in_legend.add(key)
+                    names = sorted(names_by_legend_key.get(key))
+                    label = ", ".join(names)
+                    if group:
+                        label = f"{group}: {label}"
+                    MAX_WIDTH = 60
+                    if len(label) > MAX_WIDTH:  # Crop long labels
+                        label = label[:MAX_WIDTH] + "..."
+                    show_in_legend = True
+                    name = label
+
+            params = copy.deepcopy(self.trace_params)
+            marker = params.pop("marker")
+            if color:
+                marker["color"] = color
+            if "marker_line_width" in element:
+                marker["line"]["width"] = element["marker_line_width"]
+            if "marker_size" in element:
+                marker["size"] = element["marker_size"]
+            if "opacity" in element:
+                marker["opacity"] = element["opacity"]
+
+            if annotation:
+                params["mode"] = "markers+text"
+            if n_annotated > 0:  # Reduce opacity of the borders that clutter the annotations:
+                marker["line"]["color"] = "rgba(0, 0, 0, .2)"
+
+            fig.add_trace(
+                go.Scatter(
+                    x=[x],
+                    y=[element["y"]],
+                    name=name,
+                    text=[annotation or name],
+                    showlegend=show_in_legend,
+                    marker=marker,
+                    **params,
+                )
             )
-            return dataset
+        fig.layout.height += len(in_legend) * 5  # extra space for legend
+        return fig
 
-        def create_figure(
-            self,
-            layout: Optional[go.Layout] = None,
-            is_log=False,
-            is_pct=False,
-        ) -> go.Figure:
-            """
-            Create a Plotly figure for a dataset
-            """
-            fig = go.Figure(layout=layout)
-
-            MAX_ANNOTATIONS = 10  # Maximum number of dots to be annotated directly on the plot
-            n_annotated = len([el for el in self.points if "annotation" in el])
-            if n_annotated < MAX_ANNOTATIONS:
-                # Finding and marking outliers to only label them
-                # 1. Calculate Z-scores
-                points = [(i, x) for i, x in enumerate(self.points) if x.get("annotate", True) is not False]
-                x_values = np.array([x["x"] for (i, x) in points])
-                y_values = np.array([x["y"] for (i, x) in points])
-                x_std = np.std(x_values)
-                y_std = np.std(y_values)
-                if x_std == 0 and y_std == 0:
-                    logger.warning(f"Scatter plot {self.plot.id}: all {len(points)} points have the same coordinates")
-                    if len(points) == 1:  # Only single point - annotate it!
-                        for i, point in points:
-                            point["annotation"] = point["name"]
-                else:
-                    x_z_scores = np.abs((x_values - np.mean(x_values)) / x_std) if x_std else np.zeros_like(x_values)
-                    y_z_scores = np.abs((y_values - np.mean(y_values)) / y_std) if y_std else np.zeros_like(y_values)
-                    # 2. Find a reasonable threshold so there are not too many outliers
-                    threshold = 1.0
-                    while threshold <= 6.0:
-                        n_outliers = np.count_nonzero((x_z_scores > threshold) | (y_z_scores > threshold))
-                        logger.debug(f"Scatter plot outlier threshold: {threshold:.2f}, outliers: {n_outliers}")
-                        if n_annotated + n_outliers <= MAX_ANNOTATIONS:
-                            break
-                        # If there are too many outliers, we increase the threshold until we have less than 10
-                        threshold += 0.2
-                    # 3. Annotate outliers that pass the threshold
-                    for (i, point), x_z_score, y_z_score in zip(points, x_z_scores, y_z_scores):
-                        # Check if point is an outlier or if total points are less than 10
-                        if x_z_score > threshold or y_z_score > threshold:
-                            point["annotation"] = point["name"]
-                n_annotated = len([point for point in self.points if "annotation" in point])
-
-            # If there are few unique colors, we can additionally put a unique list into a legend
-            # (even though some color might belong to many distinct names - we will just crop the list)
-            names_by_legend_key = defaultdict(set)
-            for el in self.points:
-                legend_key = (el.get("color"), el.get("marker_size"), el.get("marker_line_width"), el.get("group"))
-                names_by_legend_key[legend_key].add(el["name"])
-            layout.showlegend = True
-
-            in_legend = set()
-            for element in self.points:
-                x = element["x"]
-                if self.categories:
-                    if isinstance(x, float):
-                        x = int(round(x))
-                    if isinstance(x, int) and (0 <= x < len(self.categories)):
-                        x = self.categories[x]
-                    else:
-                        logger.error(
-                            f"Scatter plot {self.plot.id}: x={x} must be an index in the list of categories: {self.categories}"
-                        )
-                        continue
-
-                name = element["name"]
-                group = element.get("group")
-                color = element.get("color")
-                annotation = element.get("annotation")
-
-                show_in_legend = False
-                if layout.showlegend and not element.get("hide_in_legend"):
-                    key = (color, element.get("marker_size"), element.get("marker_line_width"), group)
-                    if key not in in_legend:
-                        in_legend.add(key)
-                        names = sorted(names_by_legend_key.get(key))
-                        label = ", ".join(names)
-                        if group:
-                            label = f"{group}: {label}"
-                        MAX_WIDTH = 60
-                        if len(label) > MAX_WIDTH:  # Crop long labels
-                            label = label[:MAX_WIDTH] + "..."
-                        show_in_legend = True
-                        name = label
-
-                params = copy.deepcopy(self.trace_params)
-                marker = params.pop("marker")
-                if color:
-                    marker["color"] = color
-                if "marker_line_width" in element:
-                    marker["line"]["width"] = element["marker_line_width"]
-                if "marker_size" in element:
-                    marker["size"] = element["marker_size"]
-                if "opacity" in element:
-                    marker["opacity"] = element["opacity"]
-
-                if annotation:
-                    params["mode"] = "markers+text"
-                if n_annotated > 0:  # Reduce opacity of the borders that clutter the annotations:
-                    marker["line"]["color"] = "rgba(0, 0, 0, .2)"
-
-                fig.add_trace(
-                    go.Scatter(
-                        x=[x],
-                        y=[element["y"]],
-                        name=name,
-                        text=[annotation or name],
-                        showlegend=show_in_legend,
-                        marker=marker,
-                        **params,
-                    )
-                )
-            fig.layout.height += len(in_legend) * 5  # extra space for legend
-            return fig
 
+class ScatterPlot(Plot):
     def __init__(self, pconfig: Dict, points_lists: List[List[PointT]]):
         super().__init__(PlotType.SCATTER, pconfig, len(points_lists))
 
-        self.datasets: List[ScatterPlot.Dataset] = [
-            ScatterPlot.Dataset.create(d, points, pconfig) for d, points in zip(self.datasets, points_lists)
+        self.datasets: List[Dataset] = [
+            Dataset.create(d, points, pconfig) for d, points in zip(self.datasets, points_lists)
         ]
 
         # Make a tooltip always show on hover over nearest point on plot
         self.layout.hoverdistance = -1
 
     def tt_label(self) -> Optional[str]:
         """Default tooltip label"""
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/table.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 from collections import defaultdict
-from typing import Tuple, Optional
+from typing import Tuple, Optional, List
 
 from multiqc.plots.table_object import DataTable
 from multiqc.utils import config, mqc_colour, util_functions, report
 
 logger = logging.getLogger(__name__)
 
 
-def plot(dt: DataTable) -> str:
+def plot(dt: List[DataTable]) -> str:
     from multiqc.plots.plotly import violin
 
     return violin.plot(dt, show_table_by_default=True)
 
 
 def make_table(dt: DataTable, violin_id: Optional[str] = None) -> Tuple[str, str]:
     """
-    Build the HTML needed for a MultiQC table.
+    Build HTML for a MultiQC table, and HTML for the modal for configuring the table.
     :param dt: MultiQC datatable object
     :param violin_id: optional, will add a button to switch to a violin plot with this ID
     """
 
     t_headers = dict()
     t_modal_headers = dict()
     t_rows = dict()
@@ -355,15 +355,15 @@
     # Build the header row
     col1_header = dt.pconfig.get("col1_header", "Sample Name")
     html += f"<thead><tr><th class=\"rowheader\">{col1_header}</th>{''.join(t_headers.values())}</tr></thead>"
 
     # Build the table body
     html += "<tbody>"
     t_row_keys = t_rows.keys()
-    if dt.pconfig.get("sortRows") is not False:
+    if dt.pconfig.get("sort_rows", dt.pconfig.get("sortRows")) is not False:
         t_row_keys = sorted(t_row_keys)
     for s_name in t_row_keys:
         # Hide the row if all cells are empty or hidden
         row_hidden = ' style="display:none"' if all(t_rows_empty[s_name].values()) else ""
         html += f"<tr{row_hidden}>"
         # Sample name row header
         html += f'<th class="rowheader" data-original-sn="{s_name}">{s_name}</th>'
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/plotly/violin.py` & `multiqc_sgr-1.22.post0/multiqc/plots/plotly/violin.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,315 +11,318 @@
 from multiqc.plots.table_object import DataTable
 from multiqc.plots.plotly.plot import Plot, PlotType, BaseDataset
 from multiqc.plots.plotly.table import make_table
 
 logger = logging.getLogger(__name__)
 
 
-def plot(dt: DataTable, show_table_by_default=False) -> str:
+def plot(dts: List[DataTable], show_table_by_default=False) -> str:
     """
     Build and add the plot data to the report, return an HTML wrapper.
     """
-    p = ViolinPlot.from_dt(dt, show_table_by_default)
+    p = ViolinPlot.from_dt(dts, show_table_by_default)
 
     from multiqc.utils import report
 
     return p.add_to_report(report)
 
 
-class ViolinPlot(Plot):
-    VIOLIN_HEIGHT = 70  # single violin height
-    EXTRA_HEIGHT = 63  # extra space for the title and footer
+@dataclasses.dataclass
+class Dataset(BaseDataset):
+    metrics: List[str]
+    header_by_metric: Dict[str, Dict[str, Any]]
+    violin_values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]]
+    scatter_values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]]
+    all_samples: List[str]  # unique list of all samples in this dataset
+    scatter_trace_params: Dict[str, Any]
 
-    @dataclasses.dataclass
-    class Dataset(BaseDataset):
-        metrics: List[str]
-        header_by_metric: Dict[str, Dict[str, Any]]
-        violin_values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]]
-        scatter_values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]]
-        all_samples: List[str]  # unique list of all samples in this dataset
-        scatter_trace_params: Dict[str, Any]
-
-        @staticmethod
-        def create(
-            dataset: BaseDataset,
-            values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]],
-            header_by_metric: Dict[str, Dict[str, Any]],
-        ) -> "ViolinPlot.Dataset":
-            ds = ViolinPlot.Dataset(
-                **dataset.__dict__,
-                metrics=[],
-                header_by_metric=header_by_metric,
-                violin_values_by_sample_by_metric=dict(),
-                scatter_values_by_sample_by_metric=dict(),
-                all_samples=[],
-                scatter_trace_params=dict(),
-            )
+    @staticmethod
+    def create(
+        dataset: BaseDataset,
+        values_by_sample_by_metric: Dict[str, Dict[str, Union[List[int], List[float], List[str]]]],
+        header_by_metric: Dict[str, Dict[str, Any]],
+    ) -> "Dataset":
+        ds = Dataset(
+            **dataset.__dict__,
+            metrics=[],
+            header_by_metric=header_by_metric,
+            violin_values_by_sample_by_metric=dict(),
+            scatter_values_by_sample_by_metric=dict(),
+            all_samples=[],
+            scatter_trace_params=dict(),
+        )
 
-            all_samples = set()
-            for metric, header in header_by_metric.items():
-                # Add Plotly-specific parameters to the header
-                xaxis = {"ticksuffix": header.get("suffix")}
-                header["xaxis"] = xaxis
-                header["show_points"] = True
-                header["show_only_outliers"] = False
-
-                # Take non-empty values for the violin
-                value_by_sample = values_by_sample_by_metric[metric]
-                value_by_sample = {s: v for s, v in value_by_sample.items() if v is not None and str(v).strip() != ""}
-
-                # Parse values to numbers if possible
-                for s, v in value_by_sample.items():
-                    if isinstance(v, str):
+        all_samples = set()
+        for metric, header in header_by_metric.items():
+            # Add Plotly-specific parameters to the header
+            xaxis = {"ticksuffix": header.get("suffix")}
+            header["xaxis"] = xaxis
+            header["show_points"] = True
+            header["show_only_outliers"] = False
+
+            # Take non-empty values for the violin
+            value_by_sample = values_by_sample_by_metric[metric]
+            value_by_sample = {s: v for s, v in value_by_sample.items() if v is not None and str(v).strip() != ""}
+
+            # Parse values to numbers if possible
+            for s, v in value_by_sample.items():
+                if isinstance(v, str):
+                    try:
+                        value_by_sample[s] = int(v)
+                    except ValueError:
                         try:
-                            value_by_sample[s] = int(v)
+                            value_by_sample[s] = float(v)
                         except ValueError:
-                            try:
-                                value_by_sample[s] = float(v)
-                            except ValueError:
-                                pass
-                    if "modify" in header and callable(header["modify"]):
-                        # noinspection PyBroadException
-                        try:
-                            value_by_sample[s] = header["modify"](v)
-                        except Exception:  # User-provided modify function can raise any exception
                             pass
+                if "modify" in header and callable(header["modify"]):
+                    # noinspection PyBroadException
+                    try:
+                        value_by_sample[s] = header["modify"](v)
+                    except Exception:  # User-provided modify function can raise any exception
+                        pass
+
+            if not value_by_sample:
+                logger.debug(f"No non-empty values found for metric: {header['title']}")
+                if "modify" in header and callable(header["modify"]):
+                    del header["modify"]  # To keep the data JSON-serializable
+                continue
 
+            values_are_numeric = all(isinstance(v, (int, float)) for v in value_by_sample.values())
+            values_are_integer = all(isinstance(v, int) for v in value_by_sample.values())
+            if values_are_numeric:
+                # Remove NaN and Inf values
+                value_by_sample = {s: v for s, v in value_by_sample.items() if np.isfinite(v)}
                 if not value_by_sample:
-                    logger.debug(f"No non-empty values found for metric: {header['title']}")
+                    logger.warning(f"All values are NaN or Inf for metric: {header['title']}")
+                    if "modify" in header and callable(header["modify"]):
+                        del header["modify"]  # To keep the data JSON-serializable
                     continue
 
-                values_are_numeric = all(isinstance(v, (int, float)) for v in value_by_sample.values())
-                values_are_integer = all(isinstance(v, int) for v in value_by_sample.values())
-                if values_are_numeric:
-                    # Remove NaN and Inf values
-                    value_by_sample = {s: v for s, v in value_by_sample.items() if np.isfinite(v)}
-                    if not value_by_sample:
-                        logger.warning(f"All values are NaN or Inf for metric: {header['title']}")
-                        continue
-
-                header["show_points"] = len(value_by_sample) <= config.violin_min_threshold_no_points
-                header["show_only_outliers"] = len(value_by_sample) > config.violin_min_threshold_outliers
-
-                if values_are_numeric:
-                    # Calculate range
-                    xmin = header.get("dmin")
-                    xmax = header.get("dmax")
-                    tickvals = None
-                    if xmin == xmax == 0:  # Plotly will modify the 0:0 range to -1:1, and we want to keep it 0-centered
-                        xmax = 1
-                        tickvals = [0]
-                    xaxis["tickvals"] = tickvals
-                    if xmin is not None and xmax is not None:
-                        if header["show_points"]:
-                            # add extra padding to avoid clipping the points at range limits
-                            xmin -= (xmax - xmin) * 0.005
-                            xmax += (xmax - xmin) * 0.005
-                        xaxis["range"] = [xmin, xmax]
+            header["show_points"] = len(value_by_sample) <= config.violin_min_threshold_no_points
+            header["show_only_outliers"] = len(value_by_sample) > config.violin_min_threshold_outliers
 
-                if not header["show_points"]:  # Do not add any interactive points
+            if values_are_numeric:
+                # Calculate range
+                xmin = header.get("dmin")
+                xmax = header.get("dmax")
+                tickvals = None
+                if xmin == xmax == 0:  # Plotly will modify the 0:0 range to -1:1, and we want to keep it 0-centered
+                    xmax = 1
+                    tickvals = [0]
+                xaxis["tickvals"] = tickvals
+                if xmin is not None and xmax is not None:
+                    if header["show_points"]:
+                        # add extra padding to avoid clipping the points at range limits
+                        xmin -= (xmax - xmin) * 0.005
+                        xmax += (xmax - xmin) * 0.005
+                    xaxis["range"] = [xmin, xmax]
+
+            if not header["show_points"]:  # Do not add any interactive points
+                scatter_values_by_sample = {}
+            elif not header["show_only_outliers"]:
+                scatter_values_by_sample = {}  # will use the violin values
+            else:
+                if not values_are_numeric:
+                    logger.debug(
+                        f"Violin for '{header['title']}': sample number is {len(value_by_sample)} > {header['show_only_outliers']}. "
+                        f"As values are not numeric, will not add any interactive points."
+                    )
                     scatter_values_by_sample = {}
-                elif not header["show_only_outliers"]:
-                    scatter_values_by_sample = {}  # will use the violin values
                 else:
-                    if not values_are_numeric:
-                        logger.debug(
-                            f"Violin for '{header['title']}': sample number is {len(value_by_sample)} > {header['show_only_outliers']}. "
-                            f"As values are not numeric, will not add any interactive points."
-                        )
-                        scatter_values_by_sample = {}
-                    else:
-                        logger.debug(
-                            f"Violin for '{header['title']}': sample number is {len(value_by_sample)} > {header['show_only_outliers']}. "
-                            f"Will add interactive points only for the outlier values."
-                        )
-                        samples = list(value_by_sample.keys())
-                        values = list(value_by_sample.values())
-                        outlier_statuses = find_outliers(
-                            values,
-                            minval=header.get("dmin"),
-                            maxval=header.get("dmax"),
-                            metric=header["title"],
-                        )
-                        logger.debug(
-                            f"Violin for '{header['title']}': found {np.count_nonzero(outlier_statuses)} outliers"
-                        )
-                        scatter_values_by_sample = {
-                            samples[idx]: values[idx] for idx in range(len(samples)) if outlier_statuses[idx]
-                        }
-
-                ds.scatter_values_by_sample_by_metric[metric] = scatter_values_by_sample
-
-                # Now sort and downsample values to keep max 2000 points for each metric
-                violin_values_by_sample = value_by_sample
-                max_violin_points = config.violin_downsample_after
-                if max_violin_points is not None and len(violin_values_by_sample) > max_violin_points:
                     logger.debug(
-                        f"Violin for '{header['title']}': sample number is {len(violin_values_by_sample)}. "
-                        f"Will downsample to max {max_violin_points} points."
+                        f"Violin for '{header['title']}': sample number is {len(value_by_sample)} > {header['show_only_outliers']}. "
+                        f"Will add interactive points only for the outlier values."
                     )
-                    samples = list(violin_values_by_sample.keys())
-                    values = list(violin_values_by_sample.values())
-                    indices = np.argsort(values)
-                    indices = indices[:: int(math.ceil(len(indices) / max_violin_points))]
-                    violin_values_by_sample = {samples[idx]: values[idx] for idx in indices}
-
-                ds.violin_values_by_sample_by_metric[metric] = violin_values_by_sample
-
-                # Clean up the header
-                if values_are_numeric and not values_are_integer and "tt_decimals" in header:
-                    header["hoverformat"] = f".{header['tt_decimals']}f"
-                    del header["tt_decimals"]
-                if "modify" in header and callable(header["modify"]):
-                    del header["modify"]  # To keep the data JSON-serializable
+                    samples = list(value_by_sample.keys())
+                    values = list(value_by_sample.values())
+                    outlier_statuses = find_outliers(
+                        values,
+                        minval=header.get("dmin"),
+                        maxval=header.get("dmax"),
+                        metric=header["title"],
+                    )
+                    logger.debug(f"Violin for '{header['title']}': found {np.count_nonzero(outlier_statuses)} outliers")
+                    scatter_values_by_sample = {
+                        samples[idx]: values[idx] for idx in range(len(samples)) if outlier_statuses[idx]
+                    }
 
-                all_samples.update(set(list(scatter_values_by_sample.keys())))
-                all_samples.update(set(list(violin_values_by_sample.keys())))
-                ds.metrics.append(metric)
-
-            ds.all_samples = sorted(all_samples)
-
-            ds.trace_params.update(
-                orientation="h",
-                box={"visible": True},
-                meanline={"visible": True},
-                fillcolor="grey",
-                line={"width": 2, "color": "grey"},
-                opacity=0.5,
-                points=False,  # Don't show points, we'll add them manually
-                # The hover information is useful, but the formatting is ugly and not
-                # configurable as far as I can see. Also, it's not possible to disable it,
-                # so setting it to "points" as we don't show points, so it's effectively
-                # disabling it.
-                hoveron="points",
-            )
+            ds.scatter_values_by_sample_by_metric[metric] = scatter_values_by_sample
+
+            # Now sort and downsample values to keep max 2000 points for each metric
+            violin_values_by_sample = value_by_sample
+            max_violin_points = config.violin_downsample_after
+            if max_violin_points is not None and len(violin_values_by_sample) > max_violin_points:
+                logger.debug(
+                    f"Violin for '{header['title']}': sample number is {len(violin_values_by_sample)}. "
+                    f"Will downsample to max {max_violin_points} points."
+                )
+                samples = list(violin_values_by_sample.keys())
+                values = list(violin_values_by_sample.values())
+                indices = np.argsort(values)
+                indices = indices[:: int(math.ceil(len(indices) / max_violin_points))]
+                violin_values_by_sample = {samples[idx]: values[idx] for idx in indices}
+
+            ds.violin_values_by_sample_by_metric[metric] = violin_values_by_sample
+
+            # Clean up the header
+            if values_are_numeric and not values_are_integer and "tt_decimals" in header:
+                header["hoverformat"] = f".{header['tt_decimals']}f"
+                del header["tt_decimals"]
+            if "modify" in header and callable(header["modify"]):
+                del header["modify"]  # To keep the data JSON-serializable
+
+            all_samples.update(set(list(scatter_values_by_sample.keys())))
+            all_samples.update(set(list(violin_values_by_sample.keys())))
+            ds.metrics.append(metric)
+
+        ds.all_samples = sorted(all_samples)
+
+        ds.trace_params.update(
+            orientation="h",
+            box={"visible": True},
+            meanline={"visible": True},
+            fillcolor="#b5b5b5",
+            line={"width": 2, "color": "#b5b5b5"},
+            opacity=0.5,
+            points=False,  # Don't show points, we'll add them manually
+            # The hover information is useful, but the formatting is ugly and not
+            # configurable as far as I can see. Also, it's not possible to disable it,
+            # so setting it to "points" as we don't show points, so it's effectively
+            # disabling it.
+            hoveron="points",
+        )
+
+        # If all violins are grey, make the dots blue to make it more clear that it's interactive
+        # if some violins are color-coded, make the dots black to make them less distracting
+        marker_color = "black" if any(h.get("color") for h in ds.header_by_metric.values()) else "#0b79e6"
+        ds.scatter_trace_params = {
+            "mode": "markers",
+            "marker": {
+                "size": 4,
+                "color": marker_color,
+            },
+            "showlegend": False,
+            "hovertemplate": ds.trace_params["hovertemplate"],
+            "hoverlabel": {"bgcolor": "white"},
+        }
+        return ds
 
-            # If all violins are grey, make the dots blue to make it more clear that it's interactive
-            # if some violins are color-coded, make the dots black to make them less distracting
-            marker_color = "black" if any(h.get("color") for h in ds.header_by_metric.values()) else "#0b79e6"
-            ds.scatter_trace_params = {
-                "mode": "markers",
-                "marker": {
-                    "size": 4,
-                    "color": marker_color,
-                },
-                "showlegend": False,
-                "hovertemplate": ds.trace_params["hovertemplate"],
-                "hoverlabel": {"bgcolor": "white"},
+    def create_figure(
+        self,
+        layout: go.Layout,
+        is_log=False,
+        is_pct=False,
+        add_scatter=True,
+    ):
+        """
+        Create a Plotly figure for a dataset
+        """
+        metrics = [m for m in self.metrics if not self.header_by_metric[m].get("hidden", False)]
+
+        layout = copy.deepcopy(layout)
+        layout.grid.rows = len(metrics)
+        layout.grid.subplots = [[(f"x{i + 1}y{i + 1}" if i > 0 else "xy")] for i in range(len(metrics))]
+        layout.height = ViolinPlot.VIOLIN_HEIGHT * len(metrics) + ViolinPlot.EXTRA_HEIGHT
+
+        for metric_idx, metric in enumerate(metrics):
+            header = self.header_by_metric[metric]
+
+            layout[f"xaxis{metric_idx + 1}"] = {
+                "automargin": layout["xaxis"]["automargin"],
+                "color": layout["xaxis"]["color"],
+                "gridcolor": layout["xaxis"]["gridcolor"],
+                "zerolinecolor": layout["xaxis"]["zerolinecolor"],
+                "hoverformat": layout["xaxis"]["hoverformat"],
+                "tickfont": copy.deepcopy(layout["xaxis"]["tickfont"]),
+            }
+            layout[f"xaxis{metric_idx + 1}"].update(header.get("xaxis", {}))
+            layout[f"yaxis{metric_idx + 1}"] = {
+                "automargin": layout["yaxis"]["automargin"],
+                "color": layout["yaxis"]["color"],
+                "gridcolor": layout["yaxis"]["gridcolor"],
+                "zerolinecolor": layout["yaxis"]["zerolinecolor"],
+                "hoverformat": layout["yaxis"]["hoverformat"],
+                "tickfont": copy.deepcopy(layout["yaxis"]["tickfont"]),
             }
-            return ds
 
-        def create_figure(
-            self,
-            layout: go.Layout,
-            is_log=False,
-            is_pct=False,
-            add_scatter=True,
-        ):
-            """
-            Create a Plotly figure for a dataset
-            """
-            metrics = [m for m in self.metrics if not self.header_by_metric[m].get("hidden", False)]
-
-            layout = copy.deepcopy(layout)
-            layout.grid.rows = len(metrics)
-            layout.grid.subplots = [[(f"x{i + 1}y{i + 1}" if i > 0 else "xy")] for i in range(len(metrics))]
-            layout.height = ViolinPlot.VIOLIN_HEIGHT * len(metrics) + ViolinPlot.EXTRA_HEIGHT
-
-            for metric_idx, metric in enumerate(metrics):
-                header = self.header_by_metric[metric]
-
-                layout[f"xaxis{metric_idx + 1}"] = {
-                    "automargin": layout["xaxis"]["automargin"],
-                    "color": layout["xaxis"]["color"],
-                    "gridcolor": layout["xaxis"]["gridcolor"],
-                    "zerolinecolor": layout["xaxis"]["zerolinecolor"],
-                    "hoverformat": layout["xaxis"]["hoverformat"],
-                    "tickfont": copy.deepcopy(layout["xaxis"]["tickfont"]),
-                }
-                layout[f"xaxis{metric_idx + 1}"].update(header.get("xaxis", {}))
-                layout[f"yaxis{metric_idx + 1}"] = {
-                    "automargin": layout["yaxis"]["automargin"],
-                    "color": layout["yaxis"]["color"],
-                    "gridcolor": layout["yaxis"]["gridcolor"],
-                    "zerolinecolor": layout["yaxis"]["zerolinecolor"],
-                    "hoverformat": layout["yaxis"]["hoverformat"],
-                    "tickfont": copy.deepcopy(layout["yaxis"]["tickfont"]),
+            padding = "  "  # otherwise the labels will stick too close to the axis
+            title = header["title"] + padding
+            if header.get("namespace"):
+                title = f"{header['namespace']}{padding}<br>" + title
+            layout[f"yaxis{metric_idx + 1}"].update(
+                {
+                    "tickmode": "array",
+                    "tickvals": [metric_idx],
+                    "ticktext": [title],
                 }
+            )
 
-                padding = "  "  # otherwise the labels will stick too close to the axis
-                title = header["title"] + padding
-                if header.get("namespace"):
-                    title = f"{header['namespace']}{padding}<br>" + title
-                layout[f"yaxis{metric_idx + 1}"].update(
-                    {
-                        "tickmode": "array",
-                        "tickvals": [metric_idx],
-                        "ticktext": [title],
-                    }
-                )
+            if "hoverformat" in header:
+                layout[f"xaxis{metric_idx + 1}"]["hoverformat"] = header["hoverformat"]
+
+            if header.get("color"):
+                layout[f"yaxis{metric_idx + 1}"]["tickfont"] = {
+                    "color": f"rgb({header['color']})",
+                }
 
-                if "hoverformat" in header:
-                    layout[f"xaxis{metric_idx + 1}"]["hoverformat"] = header["hoverformat"]
+        layout["xaxis"] = layout["xaxis1"]
+        layout["yaxis"] = layout["yaxis1"]
 
-                if header.get("color"):
-                    layout[f"yaxis{metric_idx + 1}"]["tickfont"] = {
-                        "color": f"rgb({header['color']})",
-                    }
+        fig = go.Figure(layout=layout)
 
-            layout["xaxis"] = layout["xaxis1"]
-            layout["yaxis"] = layout["yaxis1"]
+        violin_values_by_sample_by_metric = self.violin_values_by_sample_by_metric
 
-            fig = go.Figure(layout=layout)
+        for metric_idx, metric in enumerate(metrics):
+            header = self.header_by_metric[metric]
+            params = copy.deepcopy(self.trace_params)
+            color = header.get("color")
+            if color:
+                params["fillcolor"] = f"rgb({color})"
+                params["line"]["color"] = f"rgb({color})"
+
+            violin_values_by_sample = violin_values_by_sample_by_metric[metric]
+            axis_key = "" if metric_idx == 0 else str(metric_idx + 1)
+            fig.add_trace(
+                go.Violin(
+                    x=list(violin_values_by_sample.values()),
+                    name=metric_idx,
+                    text=list(violin_values_by_sample.keys()),
+                    xaxis=f"x{axis_key}",
+                    yaxis=f"y{axis_key}",
+                    **params,
+                ),
+            )
 
-            violin_values_by_sample_by_metric = self.violin_values_by_sample_by_metric
+            if add_scatter and header["show_points"]:
+                if header["show_only_outliers"]:
+                    scatter_values_by_sample = self.scatter_values_by_sample_by_metric[metric]
+                else:
+                    scatter_values_by_sample = violin_values_by_sample
+                scatter_params = copy.deepcopy(self.scatter_trace_params)
+                for sample, value in scatter_values_by_sample.items():
+                    # add vertical jitter (not working in python version currently)
+                    y = float(metric_idx)
+                    # y += random.uniform(-0.2, 0.2)
+                    # y += random.random() * 0.3 - 0.3 / 2
+                    fig.add_trace(
+                        go.Scatter(
+                            x=[value],
+                            y=[y],
+                            text=[sample],
+                            xaxis=f"x{axis_key}",
+                            yaxis=f"y{axis_key}",
+                            **scatter_params,
+                        ),
+                    )
+        return fig
 
-            for metric_idx, metric in enumerate(metrics):
-                header = self.header_by_metric[metric]
-                params = copy.deepcopy(self.trace_params)
-                color = header.get("color")
-                if color:
-                    params["fillcolor"] = f"rgb({color})"
-                    params["line"]["color"] = f"rgb({color})"
-
-                violin_values_by_sample = violin_values_by_sample_by_metric[metric]
-                axis_key = "" if metric_idx == 0 else str(metric_idx + 1)
-                fig.add_trace(
-                    go.Violin(
-                        x=list(violin_values_by_sample.values()),
-                        name=metric_idx,
-                        text=list(violin_values_by_sample.keys()),
-                        xaxis=f"x{axis_key}",
-                        yaxis=f"y{axis_key}",
-                        **params,
-                    ),
-                )
 
-                if add_scatter and header["show_points"]:
-                    if header["show_only_outliers"]:
-                        scatter_values_by_sample = self.scatter_values_by_sample_by_metric[metric]
-                    else:
-                        scatter_values_by_sample = violin_values_by_sample
-                    scatter_params = copy.deepcopy(self.scatter_trace_params)
-                    for sample, value in scatter_values_by_sample.items():
-                        # add vertical jitter (not working in python version currently)
-                        y = float(metric_idx)
-                        # y += random.uniform(-0.2, 0.2)
-                        # y += random.random() * 0.3 - 0.3 / 2
-                        fig.add_trace(
-                            go.Scatter(
-                                x=[value],
-                                y=[y],
-                                text=[sample],
-                                xaxis=f"x{axis_key}",
-                                yaxis=f"y{axis_key}",
-                                **scatter_params,
-                            ),
-                        )
-            return fig
+class ViolinPlot(Plot):
+    VIOLIN_HEIGHT = 70  # single violin height
+    EXTRA_HEIGHT = 63  # extra space for the title and footer
 
     def __init__(
         self,
         list_of_values_by_sample_by_metric: List[Dict[str, Dict[str, Union[List[int], List[float], List[str]]]]],
         list_of_header_by_metric: List[Dict[str, Dict]],
         pconfig: Dict,
         dt: Optional[DataTable] = None,
@@ -338,16 +341,16 @@
         self.dt = dt
         self.no_violin = pconfig.get("no_violin", pconfig.get("no_beeswarm", False))
         self.show_table = dt is not None
         self.show_table_by_default = show_table_by_default or self.no_violin
         if dt:  # to make it different from the violin id
             dt.id = "table-" + dt.id
 
-        self.datasets: List[ViolinPlot.Dataset] = [
-            ViolinPlot.Dataset.create(ds, values_by_sample_by_metric, headers_by_metric)
+        self.datasets: List[Dataset] = [
+            Dataset.create(ds, values_by_sample_by_metric, headers_by_metric)
             for ds, values_by_sample_by_metric, headers_by_metric in zip(
                 self.datasets,
                 list_of_values_by_sample_by_metric,
                 list_of_header_by_metric,
             )
         ]
 
@@ -389,52 +392,56 @@
             if self.show_table_by_default:
                 logger.debug(
                     f"Table '{self.id}': sample number {self.n_samples} > {config.max_table_rows}, "
                     "Will render only a violin plot instead of the table"
                 )
 
     @staticmethod
-    def from_dt(dt: DataTable, show_table_by_default=False) -> "ViolinPlot":
-        values_by_sample_by_metric = dict()
-        header_by_metric = dict()
-
-        for idx, k, header in dt.get_headers_in_order():
-            rid = header["rid"]
-            header_by_metric[rid] = {
-                "namespace": header["namespace"],
-                "title": header["title"],
-                "description": header["description"],
-                "dmax": header.get("dmax"),
-                "dmin": header.get("dmin"),
-                "suffix": header.get("suffix", ""),
-                "color": header.get("colour", header.get("color")),
-                "hidden": header.get("hidden"),
-                "modify": header.get("modify"),
-                "tt_decimals": header.get("decimalPlaces", 2),
-            }
-            values_by_sample_by_metric[rid] = dict()
-            for s_name, val_by_metric in dt.data[idx].items():
-                if k in val_by_metric:
-                    values_by_sample_by_metric[rid][s_name] = val_by_metric[k]
-
-        # If all colors are the same, remove them
-        if len(set([v["color"] for v in header_by_metric.values()])) == 1:
-            for v in header_by_metric.values():
-                v.pop("color", None)
-
-        # If all namespaces are the same as well, remove them too (usually they follow the colors pattern)
-        if len(set([v["namespace"] for v in header_by_metric.values()])) == 1:
-            for v in header_by_metric.values():
-                v.pop("namespace", None)
+    def from_dt(dts: List[DataTable], show_table_by_default=False) -> "ViolinPlot":
+        list_values_by_sample_by_metric = []
+        list_header_by_metric = []
+
+        for dt in dts:
+            list_values_by_sample_by_metric.append(dict())
+            list_header_by_metric.append(dict())
+
+            for idx, k, header in dt.get_headers_in_order():
+                rid = header["rid"]
+                list_header_by_metric[-1][rid] = {
+                    "namespace": header["namespace"],
+                    "title": header["title"],
+                    "description": header["description"],
+                    "dmax": header.get("dmax"),
+                    "dmin": header.get("dmin"),
+                    "suffix": header.get("suffix", ""),
+                    "color": header.get("colour", header.get("color")),
+                    "hidden": header.get("hidden"),
+                    "modify": header.get("modify"),
+                    "tt_decimals": header.get("tt_decimals", header.get("decimalPlaces", 2)),
+                }
+                list_values_by_sample_by_metric[-1][rid] = dict()
+                for s_name, val_by_metric in dt.data[idx].items():
+                    if k in val_by_metric:
+                        list_values_by_sample_by_metric[-1][rid][s_name] = val_by_metric[k]
+
+            # If all colors are the same, remove them
+            if len(set([v["color"] for v in list_header_by_metric[-1].values()])) == 1:
+                for v in list_header_by_metric[-1].values():
+                    v.pop("color", None)
+
+            # If all namespaces are the same as well, remove them too (usually they follow the colors pattern)
+            if len(set([v["namespace"] for v in list_header_by_metric[-1].values()])) == 1:
+                for v in list_header_by_metric[-1].values():
+                    v.pop("namespace", None)
 
         return ViolinPlot(
-            [values_by_sample_by_metric],
-            [header_by_metric],
-            pconfig=dt.pconfig,
-            dt=dt,
+            list_values_by_sample_by_metric,
+            list_header_by_metric,
+            pconfig=dts[0].pconfig,
+            dt=dts[0],
             show_table_by_default=show_table_by_default,
         )
 
     @staticmethod
     def tt_label() -> str:
         return ": %{x}"
 
@@ -442,26 +449,24 @@
         warning = ""
         if self.show_table_by_default and not self.show_table:
             warning = (
                 f'<p class="text-muted" id="table-violin-info-{self.id}">'
                 + '<span class="glyphicon glyphicon-exclamation-sign" '
                 + 'title="An interactive table is not available because of the large number of samples. '
                 + "A violin plot is generated instead, showing density of values for each metric, as "
-                + "well as hoverable points for outlier samples in each metric. "
-                + 'See http://multiqc.info/docs/#tables--beeswarm-plots"'
+                + 'well as hoverable points for outlier samples in each metric."'
                 + f' data-toggle="tooltip"></span> Showing {self.n_samples} samples.</p>'
             )
         elif not self.show_table:
             warning = (
                 f'<p class="text-muted" id="table-violin-info-{self.id}">'
                 + '<span class="glyphicon glyphicon-exclamation-sign" '
                 + 'title="An interactive table is not available because of the large number of samples. '
                 + "The violin plot displays hoverable points only for outlier samples in each metric, "
-                + "and the hiding/highlighting functionality through the toolbox only works for outliers "
-                + 'See http://multiqc.info/docs/#tables--beeswarm-plots"'
+                + 'and the hiding/highlighting functionality through the toolbox only works for outliers"'
                 + f' data-toggle="tooltip"></span> Showing {self.n_samples} samples.</p>'
             )
 
         if not self.show_table:
             # Show violin alone.
             # Note that "no_violin" will be ignored here as we need to render _something_. The only case it can
             # happen if violin.plot() is called directly, and "no_violin" is passed, which doesn't make sense.
@@ -496,15 +501,15 @@
             }
         )
         return d
 
     def buttons(self) -> []:
         """Add a control panel to the plot"""
         buttons = []
-        if not self.flat and any(len(ds.metrics) > 1 for ds in self.datasets) and self.dt.id is not None:
+        if not self.flat and any(len(ds.metrics) > 1 for ds in self.datasets) and self.dt is not None:
             buttons.append(
                 self._btn(
                     cls="mqc_table_configModal_btn",
                     label="<span class='glyphicon glyphicon-th'></span> Configure columns",
                     data_attrs={"toggle": "modal", "target": f"#{self.dt.id}_configModal"},
                 )
             )
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/scatter.py` & `multiqc_sgr-1.22.post0/multiqc/plots/scatter.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         for point, v in config.custom_plot_config[pconfig["id"]].items():
             pconfig[point] = v
 
     # Given one dataset - turn it into a list
     if not isinstance(data, list):
         data = [data]
 
-    # Generate the data dict structure expected by HighCharts series
     plotdata = list()
     for data_index, ds in enumerate(data):
         d = list()
         for s_name in ds:
             # Ensure any overwriting conditionals from data_labels (e.g. ymax) are taken in consideration
             series_config = pconfig.copy()
             if "data_labels" in pconfig and isinstance(
@@ -76,16 +75,14 @@
                             point[k] = v[s_name]
                         else:
                             point[k] = v
                 d.append(point)
         plotdata.append(d)
 
     if pconfig.get("square"):
-        # Making sure HighCharts doesn't get creative in adding different paddings
-        pconfig["endOnTick"] = False
         if "ymax" not in pconfig and "xmax" not in pconfig:
             # Find the max value
             max_val = 0
             for d in plotdata:
                 for s in d:
                     max_val = max(max_val, s["x"], s["y"])
             max_val = 1.02 * max_val  # add 2% padding
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/table.py` & `multiqc_sgr-1.22.post0/multiqc/plots/table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,49 @@
-""" MultiQC functions to plot a table """
-
 import logging
+from typing import List, Dict, Union, Optional
 
 from multiqc.plots import table_object
 from multiqc.utils import config
 from multiqc.plots.plotly import table
 
 logger = logging.getLogger(__name__)
 
-letters = "abcdefghijklmnopqrstuvwxyz"
-
 # Load the template so that we can access its configuration
 # Do this lazily to mitigate import-spaghetti when running unit tests
 _template_mod = None
 
 
 def get_template_mod():
     global _template_mod
     if not _template_mod:
         _template_mod = config.avail_templates[config.template].load()
     return _template_mod
 
 
-def plot(data, headers=None, pconfig=None):
+def plot(data: Union[List[Dict], Dict], headers: Optional[Union[List[Dict], Dict]] = None, pconfig=None):
     """Return HTML for a MultiQC table.
     :param data: 2D dict, first keys as sample names, then x:y data pairs
     :param headers: list of optional dicts with column config in key:value pairs.
+    :param pconfig: plot config dict
     :return: HTML ready to be inserted into the page
     """
     # Make a datatable object
     dt = table_object.DataTable(data, headers, pconfig)
 
-    # Collect unique sample names
-    s_names = set()
-    for d in dt.data:
-        for s_name in d.keys():
-            s_names.add(s_name)
-
     mod = get_template_mod()
     if "table" in mod.__dict__ and callable(mod.table):
+        # Collect unique sample names
+        s_names = set()
+        for d in dt.data:
+            for s_name in d.keys():
+                s_names.add(s_name)
+
         # noinspection PyBroadException
         try:
             return mod.table(dt, s_names, pconfig)
         except:  # noqa: E722
             if config.strict:
                 # Crash quickly in the strict mode. This can be helpful for interactive
                 # debugging of modules
                 raise
 
-    return table.plot(dt)
+    return table.plot([dt])
```

### Comparing `multiqc_sgr-1.21.0/multiqc/plots/table_object.py` & `multiqc_sgr-1.22.post0/multiqc/plots/table_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 
 from multiqc.utils import config, report
 
 logger = logging.getLogger(__name__)
 
 
 class DataTable:
-    """Data table class. Prepares and holds data and configuration
-    for either a table or a beeswarm plot."""
+    """
+    Data table class. Prepares and holds data and configuration
+    for either a table or a violin plot.
+    """
 
     def __init__(
         self,
-        data: Union[List, Dict],
+        data: Union[List[Dict], Dict],
         headers: Optional[Union[List, Dict]] = None,
         pconfig: Optional[Dict] = None,
     ):
         """Prepare data for use in a table or plot"""
         self.headers_in_order = defaultdict(list)
         self.data: Dict = {}
         self.headers: Optional[List] = None
@@ -50,16 +52,16 @@
                 report.lint_errors.append(errmsg)
             self.id = report.save_htmlid(f"table-{''.join(random.sample(string.ascii_lowercase, 4))}")
 
         self._build(data, headers, pconfig)
 
     def _build(
         self,
-        data: List,
-        headers: List,
+        data: List[Dict],
+        headers: List[Dict],
         pconfig: Dict,
     ):
         # Allow user to overwrite any given config for this plot
         if self.id in config.custom_plot_config:
             for k, v in config.custom_plot_config[self.id].items():
                 pconfig[k] = v
 
@@ -79,30 +81,30 @@
         for idx, d in enumerate(data):
             # Get the header keys
             try:
                 keys = headers[idx].keys()
                 assert len(keys) > 0
             except (IndexError, AttributeError, AssertionError):
                 pconfig["only_defined_headers"] = False
+                keys = list()
 
             # Add header keys from the data
             if pconfig.get("only_defined_headers", True) is False:
                 # Get the keys from the data
                 keys = list()
                 for samp in d.values():
                     for k in samp.keys():
                         if k not in keys:
                             keys.append(k)
 
                 # If we don't have a headers dict for this data set yet, create one
                 try:
                     headers[idx]
                 except IndexError:
-                    headers.append(list)
-                    headers[idx] = dict()
+                    headers.append(dict())
                 else:
                     # Convert the existing headers into a dict (e.g. if parsed from a config)
                     od_tuples = [(key, headers[idx][key]) for key in headers[idx].keys()]
                     headers[idx] = dict(od_tuples)
 
                 # Create empty header configs for each new data key
                 for k in keys:
@@ -151,40 +153,39 @@
                         multiplier = config.long_read_count_multiplier
                         shared_key_suffix = config.long_read_count_prefix
                     elif shared_key == "base_count" and config.base_count_prefix:
                         multiplier = config.base_count_multiplier
                         shared_key_suffix = config.base_count_prefix
                     else:
                         multiplier = 1
-                    if headers[idx][k].get("modify") is None:
+                    if "modify" not in headers[idx][k]:
                         headers[idx][k]["modify"] = lambda x: x * multiplier
-                    if headers[idx][k].get("min") is None:
+                    if "min" not in headers[idx][k] is None:
                         headers[idx][k]["min"] = 0
-                    if headers[idx][k].get("format") is None:
+                    if "format" not in headers[idx][k] is None:
                         if multiplier == 1:
                             headers[idx][k]["format"] = "{:,d}"
-                suffix = headers[idx][k].get("suffix")
-                if suffix is None and shared_key_suffix is not None:
-                    suffix = " " + shared_key_suffix
-                if suffix is not None:
-                    headers[idx][k]["suffix"] = suffix
+                if "suffix" not in headers[idx][k] and shared_key_suffix is not None:
+                    headers[idx][k]["suffix"] = " " + shared_key_suffix
 
                 # Use defaults / data keys if headers not given
                 headers[idx][k]["namespace"] = headers[idx][k].get("namespace", pconfig.get("namespace", ""))
                 headers[idx][k]["title"] = headers[idx][k].get("title", k)
                 headers[idx][k]["description"] = headers[idx][k].get("description", headers[idx][k]["title"])
                 headers[idx][k]["scale"] = headers[idx][k].get("scale", pconfig.get("scale", "GnBu"))
                 headers[idx][k]["format"] = headers[idx][k].get("format", pconfig.get("format", "{:,.1f}"))
                 headers[idx][k]["colour"] = headers[idx][k].get("colour", pconfig.get("colour", None))
                 headers[idx][k]["hidden"] = headers[idx][k].get("hidden", pconfig.get("hidden", None))
                 headers[idx][k]["max"] = headers[idx][k].get("max", pconfig.get("max", None))
                 headers[idx][k]["min"] = headers[idx][k].get("min", pconfig.get("min", None))
                 headers[idx][k]["ceiling"] = headers[idx][k].get("ceiling", pconfig.get("ceiling", None))
                 headers[idx][k]["floor"] = headers[idx][k].get("floor", pconfig.get("floor", None))
-                headers[idx][k]["minRange"] = headers[idx][k].get("minRange", pconfig.get("minRange", None))
+                headers[idx][k]["minrange"] = headers[idx][k].get(
+                    "minrange", pconfig.get("minrange", headers[idx][k].get("minRange", pconfig.get("minRange", None)))
+                )
                 headers[idx][k]["shared_key"] = headers[idx][k].get("shared_key", pconfig.get("shared_key", None))
                 headers[idx][k]["modify"] = headers[idx][k].get("modify", pconfig.get("modify", None))
                 headers[idx][k]["placement"] = float(headers[idx][k].get("placement", 1000))
 
                 if headers[idx][k]["colour"] is None:
                     cidx = idx
                     while cidx >= len(SECTION_COLORS):
@@ -279,23 +280,23 @@
                                     headers[idx][k]["dmax"] = max(headers[idx][k]["dmax"], val)
                                 if setdmin:
                                     headers[idx][k]["dmin"] = min(headers[idx][k]["dmin"], val)
                         except (ValueError, TypeError):
                             val = samp[k]  # couldn't convert to float - keep as a string
                         except KeyError:
                             pass  # missing data - skip
-                    # Limit auto-generated scales with floor, ceiling and minRange.
+                    # Limit auto-generated scales with floor, ceiling and minrange.
                     if headers[idx][k]["ceiling"] is not None and headers[idx][k]["max"] is None:
                         headers[idx][k]["dmax"] = min(headers[idx][k]["dmax"], float(headers[idx][k]["ceiling"]))
                     if headers[idx][k]["floor"] is not None and headers[idx][k]["min"] is None:
                         headers[idx][k]["dmin"] = max(headers[idx][k]["dmin"], float(headers[idx][k]["floor"]))
-                    if headers[idx][k]["minRange"] is not None:
+                    if headers[idx][k]["minrange"] is not None:
                         drange = headers[idx][k]["dmax"] - headers[idx][k]["dmin"]
-                        if drange < float(headers[idx][k]["minRange"]):
-                            headers[idx][k]["dmax"] = headers[idx][k]["dmin"] + float(headers[idx][k]["minRange"])
+                        if drange < float(headers[idx][k]["minrange"]):
+                            headers[idx][k]["dmax"] = headers[idx][k]["dmin"] + float(headers[idx][k]["minrange"])
 
         # Collect settings for shared keys
         shared_keys = defaultdict(lambda: dict())
         for idx, hs in enumerate(headers):
             for k in hs.keys():
                 sk = headers[idx][k]["shared_key"]
                 if sk is not None:
@@ -316,15 +317,15 @@
                 if sk is not None:
                     headers[idx][k]["dmax"] = shared_keys[sk]["dmax"]
                     headers[idx][k]["dmin"] = shared_keys[sk]["dmin"]
 
                 self.headers_in_order[headers[idx][k]["placement"]].append((idx, k))
 
         # Skip any data that is not used in the table
-        # Would be ignored for making the table anyway, but can affect whether a beeswarm plot is used
+        # Would be ignored for making the table anyway, but can affect whether a violin plot is used
         for idx, d in enumerate(data):
             for s_name in list(d.keys()):
                 if not any(h in data[idx][s_name].keys() for h in headers[idx]):
                     del data[idx][s_name]
 
         # Assign to class
         self.data = data
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/__init__.py` & `multiqc_sgr-1.22.post0/multiqc/templates/default/__init__.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/bootstrap.min.css` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/default_multiqc.css` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/default_multiqc.css`

 * *Files 1% similar despite different names*

```diff
@@ -877,26 +877,26 @@
 }
 .mqc_table .val {
   display: block;
   padding: 5px;
   left: 0;
 }
 
-/* Flat MatPlotLib plots */
+/* Flat plots */
 .mqc_mplplot {
   border: 1px solid #dedede;
   margin-top: 0;
   width: 100%;
 }
 .mqc_mplplot img {
   max-width: 100%;
   height: auto;
 }
 
-/* Draggable height bar for HighCharts Plots */
+/* Draggable height bar interactive plots */
 .hc-plot {
   height: 500px;
   width: 100%;
 }
 .hc-plot.not_rendered {
   background-color: #ededed;
   text-align: center;
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/css/jquery.toast.css` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/css/jquery.toast.css`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.eot` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.svg` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.ttf` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff2` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/MultiQC_logo.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/MultiQC_logo.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/MultiQC_logo_dark.svg` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/MultiQC_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-16x16.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-32x32.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/favicon-96x96.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/seqera_logo.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/seqera_logo.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/img/seqera_logo_mono.png` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/img/seqera_logo_mono.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/flat.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/flat.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/multiqc.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/multiqc.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/FileSaver.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/bootstrap.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery-3.1.1.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery-ui.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery.tablesorter.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jquery.toast.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jquery.toast.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/jszip.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/jszip.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/lz-string.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/lz-string.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.min.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/packages/plotly-2.27.0.min.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/bar.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/bar.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
         this.filteredSettings = samplesSettings.filter((s) => !s.hidden);
         samples = this.filteredSettings.map((s) => s.name);
 
         cats = cats.map((cat) => {
             let data = this.pActive ? cat["data_pct"] : cat.data;
             return {
                 data: data.filter((_, si) => !samplesSettings[si].hidden),
-                color: cat.color,
+                color: cat.color, // formatted as "r,g,b", to be wrapped with "rgb()" or "rgba()"
                 name: cat.name,
             };
         });
 
         return [cats, samples];
     }
 
@@ -78,15 +78,15 @@
                 });
             } else {
                 // "group"
                 // Plotly adds giant gaps between bars in the group mode when adding each sample as a
                 // separate trace. Sacrificing dimming the de-highlighted bars to get rid of this gap.
                 let params = JSON.parse(JSON.stringify(traceParams)); // deep copy
                 samples = this.filteredSettings.map((s) => s.name);
-                params.marker.color = "rgba(" + cat.color + ")";
+                params.marker.color = "rgb(" + cat.color + ")";
 
                 return {
                     type: "bar",
                     x: cat.data,
                     y: samples,
                     name: cat.name,
                     meta: cat.name,
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/box.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/box.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/heatmap.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/heatmap.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/line.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/line.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -29,45 +29,32 @@
         if (lines.length === 0 || samples.length === 0) return [];
 
         // Reorder points so highlighted points are on top
         let highlighted = lines.filter((p) => p.highlight);
         let nonHighlighted = lines.filter((p) => !p.highlight);
         lines = nonHighlighted.concat(highlighted);
 
-        let categories = dataset["dconfig"]["categories"] ?? [];
         return lines.map((line) => {
-            let x, y;
-            if (line.data.length > 0 && Array.isArray(line.data[0])) {
-                x = line.data.map((x) => x[0]);
-                y = line.data.map((x) => x[1]);
-            } else if (categories.length > 0) {
-                x = categories;
-                y = line.data;
-            } else {
-                x = [...Array(line.data.length).keys()];
-                y = line.data;
-            }
-
             let params = {
                 marker: line["marker"] ?? {},
                 line: line["line"] ?? {},
                 showlegend: line["showlegend"] ?? null,
                 mode: line["mode"] ?? null,
             };
             updateObject(params, dataset["trace_params"], true);
 
             if (highlighted.length > 0) params.marker.color = line.highlight ?? "#cccccc";
             else params.marker.color = line.color;
 
             return {
                 type: "scatter",
-                x: x,
-                y: y,
+                x: line.data.map((x) => x[0]),
+                y: line.data.map((x) => x[1]),
                 name: line.name,
-                text: x.map(() => line.name),
+                text: line.data.map(() => line.name),
                 ...params,
             };
         });
     }
 
     exportData(format) {
         let dataset = this.datasets[this.activeDatasetIdx];
@@ -75,19 +62,15 @@
         let [_, lines] = this.prepData();
 
         // check if all lines have the same x values
         let sharedX = true;
         let x = null;
         lines.forEach((line) => {
             let thisX;
-            if (line.data.length > 0 && Array.isArray(line.data[0])) {
-                thisX = line.data.map((x) => x[0]);
-            } else {
-                thisX = dataset["dconfig"]["categories"];
-            }
+            thisX = line.data.map((x) => x[0]);
             if (x === null) {
                 x = thisX;
             } else if (x.length !== thisX.length) {
                 sharedX = false;
             } else if (x.some((v, i) => v !== thisX[i])) {
                 sharedX = false;
             }
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/scatter.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/scatter.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -15,20 +15,14 @@
 
         points = points.map((point, idx) => {
             point.name = sampleSettings[idx].name ?? point.name;
             point.highlight = sampleSettings[idx].highlight;
             if (!sampleSettings[idx].hidden) return point;
         });
 
-        points = points.map((point) => {
-            if (dataset.categories && Number.isInteger(point.x) && point.x < dataset.categories.length)
-                point.x = dataset.categories[point.x];
-            return point;
-        });
-
         return [samples, points];
     }
 
     buildTraces() {
         let dataset = this.datasets[this.activeDatasetIdx];
 
         let [samples, points] = this.prepData();
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plots/violin.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plots/violin.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/plotting.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/plotting.js`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/tables.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/tables.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -50,25 +50,34 @@
             e.preventDefault();
             let tableId = $(this).data("table-id");
             let violinId = $(this).data("violin-id");
             $("#mqc_violintable_wrapper_" + tableId).show();
             $("#mqc_violintable_wrapper_" + violinId).hide();
         });
 
-        // Copy table contents to clipboard
-        let clipboard = new Clipboard(".mqc_table_copy_btn");
-        clipboard.on("success", function(e) {
-            e.clearSelection();
-        });
         $(".mqc_table_copy_btn").click(function() {
             let btn = $(this);
-            btn.addClass("active").html('<span class="glyphicon glyphicon-copy"></span> Copied!');
-            setTimeout(function() {
-                btn.removeClass("active").html('<span class="glyphicon glyphicon-copy"></span> Copy table');
-            }, 2000);
+            let table = $(btn.data("clipboard-target"))[0];
+
+            const range = document.createRange();
+            range.selectNode(table);
+            window.getSelection().removeAllRanges();
+            window.getSelection().addRange(range);
+
+            try {
+                document.execCommand("copy");
+                window.getSelection().removeAllRanges();
+
+                btn.addClass("active").html('<span class="glyphicon glyphicon-copy"></span> Copied!');
+                setTimeout(() => {
+                    btn.removeClass("active").html('<span class="glyphicon glyphicon-copy"></span> Copied!');
+                }, 2000);
+            } catch (err) {
+                console.error("Failed to copy table: ", err);
+            }
         });
 
         // Make table headers fixed when table body scrolls (use CSS transforms)
         // http://stackoverflow.com/a/25902860/713980
         $(".mqc-table-responsive").scroll(function() {
             $(this)
                 .find("thead")
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/assets/js/toolbox.js` & `multiqc_sgr-1.22.post0/multiqc/templates/default/assets/js/toolbox.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -455,17 +455,15 @@
                             if (checked_plots.length <= zip_threshold) {
                                 // Not many plots to export, just trigger a download for each
                                 saveAs(blob, fname);
                             } else {
                                 // Lots of plots - add to a zip file for download
                                 zip.file(fname, blob);
                             }
-                        }
-                        // Normal plot - use HighCharts plugin to get the data from the plot
-                        else if (format === "tsv" || format === "csv") {
+                        } else if (format === "tsv" || format === "csv") {
                             let plot = mqc_plots[target];
                             if (plot !== undefined) {
                                 let text = plot.exportData(format);
                                 const blob = new Blob([text], {
                                     type: "text/plain;charset=utf-8"
                                 });
                                 if (checked_plots.length <= zip_threshold) {
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/base.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/base.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/content.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/content.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/foot.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/foot.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/footer.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/footer.html`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     <strong>
         <a href="http://multiqc.info" target="_blank">MultiQC v{{ config.version }}</a>
     </strong>
     - Written by <a href="http://phil.ewels.co.uk" target="_blank">Phil Ewels</a>,
     available on <a href="https://github.com/MultiQC/MultiQC" target="_blank">GitHub</a>.
 </p>
 <p>
-    This report uses <a href="http://www.highcharts.com/" target="_blank">HighCharts</a>,
+    This report uses <a href="https://www.plotly.com/" target="_blank">Plotly</a>,
     <a href="https://jquery.com/" target="_blank">jQuery</a>,
     <a href="https://jqueryui.com/" target="_blank">jQuery UI</a>,
     <a href="http://getbootstrap.com/" target="_blank">Bootstrap</a>,
     <a href="https://github.com/eligrey/FileSaver.js" target="_blank">FileSaver.js</a> and
     <a href="https://clipboardjs.com/" target="_blank">clipboard.js</a>.
 </p>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {# ####################### footer.html ########################## Content for
 the report footer. #}
 _[_d_a_t_a_:_i_m_a_g_e_/_p_n_g_;_b_a_s_e_6_4_,_{_{_ _i_n_c_l_u_d_e___f_i_l_e_(_'_a_s_s_e_t_s_/_i_m_g_/_s_e_q_e_r_a___l_o_g_o_._p_n_g_'_,_ _b_6_4_=_T_r_u_e_)
 _}_}_]_MM_uu_ll_tt_ii_QQ_CC_ _vv_{{_{{_ _cc_oo_nn_ff_ii_gg_.._vv_ee_rr_ss_ii_oo_nn_ _}}_}} - Written by _P_h_i_l_ _E_w_e_l_s, available on _G_i_t_H_u_b.
-This report uses _H_i_g_h_C_h_a_r_t_s, _j_Q_u_e_r_y, _j_Q_u_e_r_y_ _U_I, _B_o_o_t_s_t_r_a_p, _F_i_l_e_S_a_v_e_r_._j_s and
+This report uses _P_l_o_t_l_y, _j_Q_u_e_r_y, _j_Q_u_e_r_y_ _U_I, _B_o_o_t_s_t_r_a_p, _F_i_l_e_S_a_v_e_r_._j_s and
 _c_l_i_p_b_o_a_r_d_._j_s.
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/general_stats.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/general_stats.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/head.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/head.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/header.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/header.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/includes.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/includes.html`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 {%- endfor %}{% endif %}{% endfor %}
 
 <!-- Include javascript files -->
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery-3.1.1.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery-ui.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/bootstrap.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery.tablesorter.min.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/clipboard.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/FileSaver.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/lz-string.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery.toast.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jszip.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/plotly-2.27.0.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/multiqc.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/flat.js') }}</script>
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/nav.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/nav.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/default/toolbox.html` & `multiqc_sgr-1.22.post0/multiqc/templates/default/toolbox.html`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         <button id="mqc_cols_apply" class="btn btn-xs btn-default pull-right" disabled>Apply</button>
         Highlight Samples
       </h4>
       {% if report.num_mpl_plots > 0 %}
       <p>
         <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
         This report has flat image plots that won't be highlighted.<br/>
-        See the <a href="http://multiqc.info/docs/#flat--interactive-plots" target="_blank">documentation</a>
+        See the <a href="https://multiqc.info/docs/development/plots/#interactive--flat-image-plots" target="_blank">documentation</a>
         for help.
       </p>
       {% endif %}
       <form class="form-inline" id="mqc_color_form">
         <input id="mqc_colour_filter" type="text" placeholder="Custom Pattern" class="form-control input-sm">
         <input id="mqc_colour_filter_color" type="color" value="#e41a1c" class="form-control input-sm">
         <button type="submit" id="mqc_colour_filter_update" class="btn btn-default btn-sm">+</button>
@@ -62,15 +62,15 @@
         <button id="mqc_rename_apply" class="btn btn-xs btn-default pull-right" disabled>Apply</button>
         Rename Samples
       </h4>
       {% if report.num_mpl_plots > 0 %}
       <p>
         <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
         This report has flat image plots that won't be renamed.<br/>
-        See the <a href="http://multiqc.info/docs/#flat--interactive-plots" target="_blank">documentation</a>
+        See the <a href="https://multiqc.info/docs/development/plots/#interactive--flat-image-plots" target="_blank">documentation</a>
         for help.
       </p>
       {% endif %}
       <form class="form-inline" id="mqc_renamesamples_form">
         <input id="mqc_renamesamples_from" type="text" placeholder="From" class="form-control input-sm">
         <input id="mqc_renamesamples_to" type="text" placeholder="To" class="form-control input-sm">
         <button type="submit" id="mqc_renamesamples_filter_update" class="btn btn-default btn-sm">+</button>
@@ -98,15 +98,15 @@
         <button id="mqc_hide_apply" class="btn btn-xs btn-default pull-right" disabled>Apply</button>
         Show / Hide Samples
       </h4>
       {% if report.num_mpl_plots > 0 %}
       <p>
         <span class="glyphicon glyphicon-warning-sign" aria-hidden="true"></span>
         This report has flat image plots that won't be hidden.<br/>
-        See the <a href="http://multiqc.info/docs/#flat--interactive-plots" target="_blank">documentation</a>
+        See the <a href="https://multiqc.info/docs/development/plots/#interactive--flat-image-plots" target="_blank">documentation</a>
         for help.
       </p>
       {% endif %}
       <form id="mqc_hidesamples_form">
         <div class="radio input-sm">
           <label><input type="radio" name="mqc_hidesamples_showhide" class="mqc_hidesamples_showhide" value="hide" checked> Hide matching samples</label>
         </div>
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/gathered/content.html` & `multiqc_sgr-1.22.post0/multiqc/templates/gathered/content.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/gathered/nav.html` & `multiqc_sgr-1.22.post0/multiqc/templates/gathered/nav.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/css/bootstrap.min.css` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/emailme.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/emailme.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/flames.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/flames.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/glyphicons-halflings-white.png` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/glyphicons-halflings.png` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/hot.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/hot.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/mchammer.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/mchammer.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/microfab.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/microfab.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/new.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/new.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/new2.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/new2.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/progress.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/progress.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/rainbow.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/rainbow.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/geo/assets/img/stars.gif` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/assets/img/stars.gif`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/highcharts/includes.html` & `multiqc_sgr-1.22.post0/multiqc/templates/geo/includes.html`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,19 @@
   src:url(data:font/eot;base64,{{ include_file('assets/fonts/glyphicons-halflings-regular.eot', b64=True) }}) format('embedded-opentype'),
       url(data:x-font-woff/woff2;base64,{{ include_file('assets/fonts/glyphicons-halflings-regular.woff2', b64=True) }}) format('woff2'),
       url(data:x-font-woff/woff;base64,{{ include_file('assets/fonts/glyphicons-halflings-regular.woff', b64=True) }}) format('woff'),
       url(data:font/ttf;base64,{{ include_file('assets/fonts/glyphicons-halflings-regular.ttf', b64=True) }}) format('truetype'),
       url(data:image/svg;base64,{{ include_file('assets/fonts/glyphicons-halflings-regular.svg', b64=True) }}) format('svg');
 }
 </style>
-<style>{{ include_file('assets/css/bootstrap.min.css') }}</style>
-<style>{{ include_file('assets/css/default_multiqc.css') }}</style>
-<style>{{ include_file('assets/css/jquery.toast.css') }}</style>
+<style type="text/css">
+    {{ include_file('assets/css/bootstrap.min.css') }}
+    {{ include_file('assets/css/default_multiqc.css') }}
+    {{ include_file('assets/css/jquery.toast.css') }}
+</style>
 {% for css_href in config.custom_css_files %}
 <style type="text/css">{{ include_file(css_href, None) }}</style>
 {% endfor %}
 {% set included_css = [] %}
 {%- for m in report.modules_output %}{% if m.css and m.css|length > 0 -%}{% for css_href in m.css.values() %}
 {% if css_href not in included_css -%}
 {{ '' if included_css.append( css_href ) }}
@@ -41,31 +43,31 @@
 {% endif %}
 {%- endfor %}{% endif %}{% endfor %}
 
 <!-- Include javascript files -->
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery-3.1.1.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery-ui.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/bootstrap.min.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/highcharts.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/highcharts.heatmap.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/highcharts.exporting.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/highcharts.offline-exporting.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/highcharts.export-csv.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery.tablesorter.min.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/packages/clipboard.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/FileSaver.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/lz-string.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jquery.toast.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/jszip.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/packages/plotly-2.27.0.min.js') }}</script>
 <script type="text/javascript">{{ include_file('assets/js/multiqc.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/multiqc_tables.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/multiqc_plotting.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/multiqc_mpl.js') }}</script>
-<script type="text/javascript">{{ include_file('assets/js/multiqc_toolbox.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/flat.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plotting.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/tables.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/toolbox.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/bar.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/box.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/line.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/scatter.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/heatmap.js') }}</script>
+<script type="text/javascript">{{ include_file('assets/js/plots/violin.js') }}</script>
 {% set included_js = [] %}
 {%- for m in report.modules_output %}{% if m.js and m.js|length > 0 -%}{% for js_href in m.js.values() %}
 {% if js_href not in included_js -%}
 {{ '' if included_js.append( js_href ) }}
 <script type="text/javascript">{{ include_file( js_href, None ) }}</script>
 {% endif %}
 {%- endfor %}{% endif %}{% endfor %}
```

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/sections/__init__.py` & `multiqc_sgr-1.22.post0/multiqc/templates/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/sections/content.html` & `multiqc_sgr-1.22.post0/multiqc/templates/sections/content.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/simple/header.html` & `multiqc_sgr-1.22.post0/multiqc/templates/simple/header.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/templates/simple/includes.html` & `multiqc_sgr-1.22.post0/multiqc/templates/simple/includes.html`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/config.py` & `multiqc_sgr-1.22.post0/multiqc/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-#!/usr/bin/env python
-
 """ MultiQC config module. Holds a single copy of
 config variables to be used across all other modules """
+
 from pathlib import Path
 from typing import List, Dict, Optional, Union
 
 import inspect
 
 # Default logger will be replaced by caller
 import logging
@@ -20,15 +19,15 @@
 
 import multiqc
 from multiqc.utils.util_functions import strtobool
 
 logger = logging.getLogger("multiqc")
 
 # Get the MultiQC version
-version = importlib_metadata.version("multiqc_sgr")
+version = importlib_metadata.version("multiqc")
 short_version = version
 git_hash = None
 git_hash_short = None
 script_path = str(Path(__file__).parent)  # dynamically used by util_functions.multiqc_dump_json()
 git_root = None
 try:
     git_root = subprocess.check_output(
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/config_defaults.yaml` & `multiqc_sgr-1.22.post0/multiqc/utils/config_defaults.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -468,15 +468,15 @@
   - freyja
   # Pre-alignment QC
   - humid
   - kat
   - leehom
   - librarian
   - nonpareil
-  - adapterRemoval
+  - adapterremoval
   - bbduk
   - clipandmerge
   - cutadapt
   - flexbar
   - sourmash
   - kaiju
   - bracken
@@ -488,14 +488,15 @@
   - skewer
   - sortmerna
   - biobloomtools
   - fastq_screen
   - afterqc
   - fastp
   - fastqc
+  - sequali
   - filtlong
   - prinseqplusplus
   - pychopper
   - porechop
   - pycoqc
   - minionqc
   - anglerfish
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/log.py` & `multiqc_sgr-1.22.post0/multiqc/utils/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-#!/usr/bin/env python
-
 """
-Code to initilise the MultiQC logging
+Code to initialise the MultiQC logging
 """
 
 import logging
 import os
 import shutil
 import sys
 import tempfile
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/lzstring.py` & `multiqc_sgr-1.22.post0/multiqc/utils/lzstring.py`

 * *Files identical despite different names*

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/megaqc.py` & `multiqc_sgr-1.22.post0/multiqc/utils/megaqc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-#!/usr/bin/env python
-
 """ MultiQC code to export data to MegaQC / flat JSON files """
 
-
 import gzip
 import io
 import json
 
 import requests
 
 from . import config
-from .util_functions import MQCJSONEncoder
+from .util_functions import dump_json
 
 log = config.logger
 
 
 def multiqc_api_post(exported_data):
     headers = {"Content-Type": "application/json", "content-encoding": "gzip"}
     if config.megaqc_access_token is not None:
         headers["access_token"] = config.megaqc_access_token
-    post_data = json.dumps({"data": exported_data}, cls=MQCJSONEncoder, ensure_ascii=False, indent=2)
+    post_data = dump_json({"data": exported_data}, ensure_ascii=False, indent=2)
     post_data = post_data.encode("utf-8", "ignore")
 
     # Gzip the JSON for massively decreased filesize
     sio_obj = io.BytesIO()
     gzfh = gzip.GzipFile(fileobj=sio_obj, mode="w")
     gzfh.write(post_data)
     gzfh.close()
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/mqc_colour.py` & `multiqc_sgr-1.22.post0/multiqc/utils/mqc_colour.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-#!/usr/bin/env python
 """
 Helper functions to manipulate colours and colour scales
 """
+
 import hashlib
 
 # Default logger will be replaced by caller
 import logging
 import re
 
 import numpy as np
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/plugin_hooks.py` & `multiqc_sgr-1.22.post0/multiqc/utils/plugin_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC plugin hooks. Enables MultiQC plugins
 to run their own custom subroutines at predefined
 trigger points during MultiQC execution. """
 
 from importlib_metadata import entry_points
 
 # Load the hooks
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/report.py` & `multiqc_sgr-1.22.post0/multiqc/utils/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC report module. Holds the output from each
 module. Is available to subsequent modules. Contains
 helper functions to generate markup for report. """
 
 
 import fnmatch
 import inspect
@@ -108,15 +106,14 @@
     multiqc_installation_dir_files = [
         "LICENSE",
         "CHANGELOG.md",
         "Dockerfile",
         "MANIFEST.in",
         ".gitmodules",
         "README.md",
-        "CSP.txt",
         "setup.py",
         ".gitignore",
     ]
 
     filenames = [f.name for f in path.iterdir() if f.is_file()]
 
     if len(filenames) > 0 and all([fn in filenames for fn in multiqc_installation_dir_files]):
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/search_patterns.yaml` & `multiqc_sgr-1.22.post0/multiqc/utils/search_patterns.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MultiQC search patterns.
 # Default configurations for how modules can find their log files.
 # Loaded by the config module so that these patterns can be overwritten in user config files.
 
-adapterRemoval:
+adapterremoval:
   fn: "*.settings"
   contents: "AdapterRemoval"
   num_lines: 1
 afterqc:
   fn: "*.json"
   contents: "allow_mismatch_in_poly"
   num_lines: 10000
@@ -595,14 +595,18 @@
   fn: "*.sex_check.csv"
 peddy/background_pca:
   fn: "*.background_pca.json"
 seqera_cli/run_dump:
   fn: "runs_*.tar.gz"
 seqera_cli/json:
   fn: "workflow.json"
+sequali:
+  fn: "*.json"
+  contents: '"sequali_version"'
+  num_lines: 10
 somalier/somalier-ancestry:
   fn: "*.somalier-ancestry.tsv"
 somalier/samples:
   fn: "*.samples.tsv"
   contents: "#family_id"
   num_lines: 5
 somalier/pairs:
@@ -789,14 +793,20 @@
 samtools/idxstats:
   fn: "*idxstat*"
 samtools/rmdup:
   contents: "[bam_rmdup"
 samtools/coverage:
   contents: "#rname	startpos	endpos	numreads	covbases	coverage	meandepth	meanbaseq	meanmapq"
   num_lines: 10
+samtools/markdup_txt:
+  contents: "COMMAND: samtools markdup"
+  num_lines: 2
+samtools/markdup_json:
+  contents: '"COMMAND": "samtools markdup'
+  num_lines: 10
 sargasso:
   fn: "overall_filtering_summary.txt"
 seqwho:
   contents: '  "Per Base Seq": ['
   num_lines: 10
 seqyclean:
   fn: "*_SummaryStatistics.tsv"
@@ -930,11 +940,7 @@
   num_lines: 1
 xenome:
   contents: "B	G	H	M	count	percent	class"
   num_lines: 2
 xengsort:
   contents: "# Xengsort classify"
   num_lines: 2
-starsolo/summary:
-  fn: "*Summary.csv"
-  contents: "GeneFull_Ex50pAS"
-  num_lines: 50
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/software_versions.py` & `multiqc_sgr-1.22.post0/multiqc/utils/software_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-#!/usr/bin/env python
-
 """ Utility functions to handle software version reporting """
 
-
 import logging
 import os
 from collections import defaultdict
 from typing import List, Dict
 
 import packaging.version
 import yaml
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/strict_helpers.py` & `multiqc_sgr-1.22.post0/multiqc/utils/strict_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-
 """ MultiQC lint helpers. Simple additional tests to run when
 --strict is specified (outside scope of normal functions) """
 
 
 import glob
 import os
```

### Comparing `multiqc_sgr-1.21.0/multiqc/utils/util_functions.py` & `multiqc_sgr-1.22.post0/multiqc/utils/util_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-#!/usr/bin/env python
-
 """ MultiQC Utility functions, used in a variety of places. """
 
-
 import io
 import json
 import logging
+import math
 import os
 import shutil
 import sys
 import time
 import datetime
 from typing import Dict, List, Union
 
@@ -64,25 +62,14 @@
     if config.data_dir is None:
         return
 
     # Get data format from config
     if data_format is None:
         data_format = config.data_format
 
-    # JSON encoder class to handle lambda functions
-    class MQCJSONEncoder(json.JSONEncoder):
-        def default(self, obj):
-            if callable(obj):
-                # noinspection PyBroadException
-                try:
-                    return obj(1)
-                except Exception:
-                    return None
-            return json.JSONEncoder.default(self, obj)
-
     body = None
     # Some metrics can't be coerced to tab-separated output, test and handle exceptions
     if data_format in ["tsv", "csv"]:
         sep = "\t" if data_format == "tsv" else ","
         # Attempt to reshape data to tsv
         # noinspection PyBroadException
         try:
@@ -129,15 +116,15 @@
             log.debug(f"{fn} could not be saved as tsv/csv, falling back to YAML. {e}")
 
     # Add relevant file extension to filename, save file.
     fn = f"{fn}.{config.data_format_extensions[data_format]}"
     fpath = os.path.join(config.data_dir, fn)
     with io.open(fpath, "w", encoding="utf-8") as f:
         if data_format == "json":
-            jsonstr = json.dumps(data, indent=4, cls=MQCJSONEncoder, ensure_ascii=False)
+            jsonstr = dump_json(data, indent=4, ensure_ascii=False)
             print(jsonstr.encode("utf-8", "ignore").decode("utf-8"), file=f)
         elif data_format == "yaml":
             yaml.dump(data, f, default_flow_style=False)
         elif body:
             # Default - tab separated output
             print(body.encode("utf-8", "ignore").decode("utf-8"), file=f)
     log.debug(f"Wrote data file {fn}")
@@ -192,23 +179,36 @@
         date_range_start = special_date - datetime.timedelta(days=days_before)
         date_range_end = special_date + datetime.timedelta(days=days_after)
         if date_range_start <= today <= date_range_end:
             return emoji
     return "mag"
 
 
-# Custom encoder to handle lambda functions
-class MQCJSONEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if callable(obj):
-            try:
-                return obj(1)
-            except Exception:
-                return None
-        return json.JSONEncoder.default(self, obj)
+def dump_json(data, **kwargs):
+    """
+    Recursively replace non-JSON-conforming NaNs and lambdas with None.
+    Note that a custom JSONEncoder would have worked for lambdas, but not for NaNs: https://stackoverflow.com/a/28640141
+    """
+
+    # Recursively replace NaNs with None
+    def replace_nan(obj):
+        if isinstance(obj, dict):
+            return {k: replace_nan(v) for k, v in obj.items()}
+        elif isinstance(obj, list):
+            return [replace_nan(v) for v in obj]
+        elif isinstance(obj, set):
+            return {replace_nan(v) for v in obj}
+        elif callable(obj):
+            return None
+        elif isinstance(obj, float) and math.isnan(obj):
+            return None
+        else:
+            return obj
+
+    return json.dumps(replace_nan(data), **kwargs)
 
 
 def multiqc_dump_json(report):
     """
     Export the parsed data in memory to a JSON file.
     Used for MegaQC and other data export.
     WARNING: May be depreciated and removed in future versions.
@@ -243,15 +243,15 @@
             try:
                 d = None
                 if s == "config":
                     d = {f"{s}_{k}": getattr(config, k)}
                 elif s == "report":
                     d = {f"{s}_{k}": getattr(report, k)}
                 if d:
-                    json.dumps(d, cls=MQCJSONEncoder, ensure_ascii=False)  # Test that exporting to JSON works
+                    dump_json(d, ensure_ascii=False)  # Test that exporting to JSON works
                     exported_data.update(d)
             except (TypeError, KeyError, AttributeError) as e:
                 log.warning(f"Couldn't export data key '{s}.{k}': {e}")
         # Get the absolute paths of analysis directories
         exported_data["config_analysis_dir_abs"] = list()
         for d in exported_data.get("config_analysis_dir", []):
             try:
```

### Comparing `multiqc_sgr-1.21.0/multiqc_sgr.egg-info/PKG-INFO` & `multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiqc_sgr
-Version: 1.21.0
+Version: 1.22.post0
 Summary: Create aggregate bioinformatics analysis reports across many samples and tools
 Author-email: Phil Ewels <phil.ewels@seqera.io>, Vlad Savelyev <vladislav.savelyev@seqera.io>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -621,15 +621,19 @@
         reviewing courts shall apply local law that most closely approximates
         an absolute waiver of all civil liability in connection with the
         Program, unless a warranty or assumption of liability accompanies a
         copy of the Program in return for a fee.
         
                              END OF TERMS AND CONDITIONS
         
-Project-URL: Repository, https://github.com/zhouyiqi91/MultiQC_SGR
+Project-URL: Homepage, https://multiqc.info
+Project-URL: Repository, https://github.com/MultiQC/MultiQC
+Project-URL: Issues, https://github.com/MultiQC/MultiQC/issues
+Project-URL: Documentation, https://multiqc.info/docs
+Project-URL: Changelog, https://github.com/MultiQC/MultiQC/blob/main/CHANGELOG.md
 Keywords: bioinformatics,biology,sequencing,NGS,next generation sequencing,quality control
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
@@ -647,15 +651,14 @@
 Requires-Dist: click
 Requires-Dist: coloredlogs
 Requires-Dist: humanize
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: kaleido
 Requires-Dist: markdown
-Requires-Dist: matplotlib>=2.1.1
 Requires-Dist: numpy
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: Pillow>=10
 Requires-Dist: plotly>=5.18
 Requires-Dist: pyyaml>=4
 Requires-Dist: pyaml-env
@@ -663,16 +666,16 @@
 Requires-Dist: rich-click
 Requires-Dist: spectra>=0.0.10
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 
 &nbsp;
-![MultiQC](docs/images/MultiQC_logo.png#gh-light-mode-only)
-![MultiQC](docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo.png#gh-light-mode-only)
+![MultiQC](https://github.com/MultiQC/MultiQC/raw/main/docs/images/MultiQC_logo_darkbg.png#gh-dark-mode-only)
 &nbsp;
 
 ### Aggregate bioinformatics results across many samples into a single report
 
 ##### Find [documentation](http://multiqc.info/docs) and [example reports](https://multiqc.info/example-reports/) at [http://multiqc.info](http://multiqc.info)
 
 [![PyPI Version](https://img.shields.io/pypi/v/multiqc)](https://pypi.python.org/pypi/multiqc/)
@@ -731,15 +734,15 @@
 ```
 
 That's it! MultiQC will scan the specified directory (`.` is the current dir)
 and produce a report detailing whatever it finds.
 
 <!-- RICH-CODEX fake_command: "multiqc ." -->
 
-![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](docs/images/screenshots/fastqc-run.svg)
+![`cd test_data/data/modules/fastqc/v0.10.1 && multiqc .`](https://github.com/MultiQC/MultiQC/raw/main/docs/images/screenshots/fastqc-run.svg)
 
 The report is created in `multiqc_report.html` by default. Tab-delimited data
 files are also created in `multiqc_data/`, containing extra information.
 These can be easily inspected using Excel (use `--data-format` to get `yaml`
 or `json` instead).
 
 For more detailed instructions, run `multiqc -h` or see the
```

### Comparing `multiqc_sgr-1.21.0/multiqc_sgr.egg-info/SOURCES.txt` & `multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 multiqc/__init__.py
 multiqc/__main__.py
 multiqc/multiqc.py
 multiqc/modules/__init__.py
 multiqc/modules/base_module.py
 multiqc/modules/profile_runtime.py
 multiqc/modules/software_versions.py
-multiqc/modules/adapterRemoval/__init__.py
-multiqc/modules/adapterRemoval/adapterRemoval.py
+multiqc/modules/adapterremoval/__init__.py
+multiqc/modules/adapterremoval/adapterremoval.py
 multiqc/modules/afterqc/__init__.py
 multiqc/modules/afterqc/afterqc.py
 multiqc/modules/anglerfish/__init__.py
 multiqc/modules/anglerfish/anglerfish.py
 multiqc/modules/bakta/__init__.py
 multiqc/modules/bakta/bakta.py
 multiqc/modules/bamdst/__init__.py
@@ -340,21 +340,24 @@
 multiqc/modules/sambamba/sambamba.py
 multiqc/modules/samblaster/__init__.py
 multiqc/modules/samblaster/samblaster.py
 multiqc/modules/samtools/__init__.py
 multiqc/modules/samtools/coverage.py
 multiqc/modules/samtools/flagstat.py
 multiqc/modules/samtools/idxstats.py
+multiqc/modules/samtools/markdup.py
 multiqc/modules/samtools/rmdup.py
 multiqc/modules/samtools/samtools.py
 multiqc/modules/samtools/stats.py
 multiqc/modules/sargasso/__init__.py
 multiqc/modules/sargasso/sargasso.py
 multiqc/modules/seqera_cli/__init__.py
 multiqc/modules/seqera_cli/seqera_cli.py
+multiqc/modules/sequali/__init__.py
+multiqc/modules/sequali/sequali.py
 multiqc/modules/seqwho/__init__.py
 multiqc/modules/seqwho/seqwho.py
 multiqc/modules/seqyclean/__init__.py
 multiqc/modules/seqyclean/seqyclean.py
 multiqc/modules/sexdeterrmine/__init__.py
 multiqc/modules/sexdeterrmine/sexdeterrmine.py
 multiqc/modules/sickle/__init__.py
@@ -381,16 +384,14 @@
 multiqc/modules/spaceranger/_utils.py
 multiqc/modules/spaceranger/count.py
 multiqc/modules/spaceranger/spaceranger.py
 multiqc/modules/stacks/__init__.py
 multiqc/modules/stacks/stacks.py
 multiqc/modules/star/__init__.py
 multiqc/modules/star/star.py
-multiqc/modules/starsolo/__init__.py
-multiqc/modules/starsolo/starsolo.py
 multiqc/modules/supernova/__init__.py
 multiqc/modules/supernova/supernova.py
 multiqc/modules/theta2/__init__.py
 multiqc/modules/theta2/theta2.py
 multiqc/modules/tophat/__init__.py
 multiqc/modules/tophat/tophat.py
 multiqc/modules/trimmomatic/__init__.py
@@ -416,15 +417,14 @@
 multiqc/modules/whatshap/whatshap.py
 multiqc/modules/xengsort/__init__.py
 multiqc/modules/xengsort/xengsort.py
 multiqc/modules/xenome/__init__.py
 multiqc/modules/xenome/xenome.py
 multiqc/plots/__init__.py
 multiqc/plots/bargraph.py
-multiqc/plots/beeswarm.py
 multiqc/plots/box.py
 multiqc/plots/heatmap.py
 multiqc/plots/linegraph.py
 multiqc/plots/scatter.py
 multiqc/plots/table.py
 multiqc/plots/table_object.py
 multiqc/plots/violin.py
@@ -467,15 +467,14 @@
 multiqc/templates/default/assets/js/flat.js
 multiqc/templates/default/assets/js/multiqc.js
 multiqc/templates/default/assets/js/plotting.js
 multiqc/templates/default/assets/js/tables.js
 multiqc/templates/default/assets/js/toolbox.js
 multiqc/templates/default/assets/js/packages/FileSaver.min.js
 multiqc/templates/default/assets/js/packages/bootstrap.min.js
-multiqc/templates/default/assets/js/packages/clipboard.min.js
 multiqc/templates/default/assets/js/packages/jquery-3.1.1.min.js
 multiqc/templates/default/assets/js/packages/jquery-ui.min.js
 multiqc/templates/default/assets/js/packages/jquery.tablesorter.min.js
 multiqc/templates/default/assets/js/packages/jquery.toast.min.js
 multiqc/templates/default/assets/js/packages/jszip.min.js
 multiqc/templates/default/assets/js/packages/lz-string.min.js
 multiqc/templates/default/assets/js/packages/plotly-2.27.0.js
@@ -500,35 +499,14 @@
 multiqc/templates/geo/assets/img/mchammer.gif
 multiqc/templates/geo/assets/img/microfab.gif
 multiqc/templates/geo/assets/img/new.gif
 multiqc/templates/geo/assets/img/new2.gif
 multiqc/templates/geo/assets/img/progress.gif
 multiqc/templates/geo/assets/img/rainbow.gif
 multiqc/templates/geo/assets/img/stars.gif
-multiqc/templates/highcharts/__init__.py
-multiqc/templates/highcharts/includes.html
-multiqc/templates/highcharts/assets/css/default_multiqc.css
-multiqc/templates/highcharts/assets/js/multiqc_mpl.js
-multiqc/templates/highcharts/assets/js/multiqc_plotting.js
-multiqc/templates/highcharts/assets/js/multiqc_tables.js
-multiqc/templates/highcharts/assets/js/multiqc_toolbox.js
-multiqc/templates/highcharts/assets/js/packages/highcharts.export-csv.js
-multiqc/templates/highcharts/assets/js/packages/highcharts.exporting.js
-multiqc/templates/highcharts/assets/js/packages/highcharts.heatmap.js
-multiqc/templates/highcharts/assets/js/packages/highcharts.js
-multiqc/templates/highcharts/assets/js/packages/highcharts.offline-exporting.js
-multiqc/templates/highcharts/plots/__init__.py
-multiqc/templates/highcharts/plots/bargraph.py
-multiqc/templates/highcharts/plots/beeswarm.py
-multiqc/templates/highcharts/plots/boxplot.py
-multiqc/templates/highcharts/plots/heatmap.py
-multiqc/templates/highcharts/plots/linegraph.py
-multiqc/templates/highcharts/plots/scatter.py
-multiqc/templates/highcharts/plots/table.py
-multiqc/templates/highcharts/plots/table_object.py
 multiqc/templates/sections/__init__.py
 multiqc/templates/sections/content.html
 multiqc/templates/simple/__init__.py
 multiqc/templates/simple/foot.html
 multiqc/templates/simple/header.html
 multiqc/templates/simple/includes.html
 multiqc/templates/simple/nav.html
```

### Comparing `multiqc_sgr-1.21.0/multiqc_sgr.egg-info/entry_points.txt` & `multiqc_sgr-1.22.post0/multiqc_sgr.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [console_scripts]
 multiqc = multiqc.__main__:run_multiqc
 
 [multiqc.modules.v1]
-adapterRemoval = multiqc.modules.adapterRemoval:MultiqcModule
+adapterremoval = multiqc.modules.adapterremoval:MultiqcModule
 afterqc = multiqc.modules.afterqc:MultiqcModule
 anglerfish = multiqc.modules.anglerfish:MultiqcModule
 bakta = multiqc.modules.bakta:MultiqcModule
 bamdst = multiqc.modules.bamdst:MultiqcModule
 bamtools = multiqc.modules.bamtools:MultiqcModule
 bbduk = multiqc.modules.bbduk:MultiqcModule
 bbmap = multiqc.modules.bbmap:MultiqcModule
@@ -115,14 +115,15 @@
 rseqc = multiqc.modules.rseqc:MultiqcModule
 salmon = multiqc.modules.salmon:MultiqcModule
 sambamba = multiqc.modules.sambamba:MultiqcModule
 samblaster = multiqc.modules.samblaster:MultiqcModule
 samtools = multiqc.modules.samtools:MultiqcModule
 sargasso = multiqc.modules.sargasso:MultiqcModule
 seqera_cli = multiqc.modules.seqera_cli:MultiqcModule
+sequali = multiqc.modules.sequali:MultiqcModule
 seqwho = multiqc.modules.seqwho:MultiqcModule
 seqyclean = multiqc.modules.seqyclean:MultiqcModule
 sexdeterrmine = multiqc.modules.sexdeterrmine:MultiqcModule
 sickle = multiqc.modules.sickle:MultiqcModule
 skewer = multiqc.modules.skewer:MultiqcModule
 slamdunk = multiqc.modules.slamdunk:MultiqcModule
 snippy = multiqc.modules.snippy:MultiqcModule
@@ -130,15 +131,14 @@
 snpsplit = multiqc.modules.snpsplit:MultiqcModule
 somalier = multiqc.modules.somalier:MultiqcModule
 sortmerna = multiqc.modules.sortmerna:MultiqcModule
 sourmash = multiqc.modules.sourmash:MultiqcModule
 spaceranger = multiqc.modules.spaceranger:MultiqcModule
 stacks = multiqc.modules.stacks:MultiqcModule
 star = multiqc.modules.star:MultiqcModule
-starsolo = multiqc.modules.starsolo:MultiqcModule
 supernova = multiqc.modules.supernova:MultiqcModule
 theta2 = multiqc.modules.theta2:MultiqcModule
 tophat = multiqc.modules.tophat:MultiqcModule
 trimmomatic = multiqc.modules.trimmomatic:MultiqcModule
 truvari = multiqc.modules.truvari:MultiqcModule
 umitools = multiqc.modules.umitools:MultiqcModule
 varscan2 = multiqc.modules.varscan2:MultiqcModule
@@ -149,10 +149,9 @@
 xengsort = multiqc.modules.xengsort:MultiqcModule
 xenome = multiqc.modules.xenome:MultiqcModule
 
 [multiqc.templates.v1]
 default = multiqc.templates.default
 gathered = multiqc.templates.gathered
 geo = multiqc.templates.geo
-highcharts = multiqc.templates.highcharts
 sections = multiqc.templates.sections
 simple = multiqc.templates.simple
```

### Comparing `multiqc_sgr-1.21.0/pyproject.toml` & `multiqc_sgr-1.22.post0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiqc_sgr"
-version = "1.21.0"
+version = "1.22.post0"
 dependencies = [
     "click",
     "coloredlogs",
     "humanize",
     "importlib-metadata",
     "jinja2>=3.0.0",
     "kaleido",  # for flat plot export
     "markdown",
-    "matplotlib>=2.1.1",
     "numpy",
     "packaging",
     "requests",
     "Pillow>=10",  # to add a logo into flat plots
     "plotly>=5.18",
     "pyyaml>=4",
     "pyaml-env",
@@ -54,21 +53,25 @@
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "ruff",
 ]
 
 [project.urls]
-Repository = "https://github.com/zhouyiqi91/MultiQC_SGR"
+Homepage = "https://multiqc.info"
+Repository = "https://github.com/MultiQC/MultiQC"
+Issues = "https://github.com/MultiQC/MultiQC/issues"
+Documentation = "https://multiqc.info/docs"
+Changelog = "https://github.com/MultiQC/MultiQC/blob/main/CHANGELOG.md"
 
 [project.entry-points.console_scripts]
 multiqc = "multiqc.__main__:run_multiqc"
 
 [project.entry-points."multiqc.modules.v1"]
-adapterRemoval = "multiqc.modules.adapterRemoval:MultiqcModule"
+adapterremoval = "multiqc.modules.adapterremoval:MultiqcModule"
 afterqc = "multiqc.modules.afterqc:MultiqcModule"
 anglerfish = "multiqc.modules.anglerfish:MultiqcModule"
 bakta = "multiqc.modules.bakta:MultiqcModule"
 bamdst = "multiqc.modules.bamdst:MultiqcModule"
 bamtools = "multiqc.modules.bamtools:MultiqcModule"
 bbduk = "multiqc.modules.bbduk:MultiqcModule"
 bbmap = "multiqc.modules.bbmap:MultiqcModule"
@@ -172,14 +175,15 @@
 qualimap = "multiqc.modules.qualimap:MultiqcModule"
 quast = "multiqc.modules.quast:MultiqcModule"
 rna_seqc = "multiqc.modules.rna_seqc:MultiqcModule"
 rockhopper = "multiqc.modules.rockhopper:MultiqcModule"
 rsem = "multiqc.modules.rsem:MultiqcModule"
 rseqc = "multiqc.modules.rseqc:MultiqcModule"
 seqera_cli = "multiqc.modules.seqera_cli:MultiqcModule"
+sequali = "multiqc.modules.sequali:MultiqcModule"
 salmon = "multiqc.modules.salmon:MultiqcModule"
 sambamba = "multiqc.modules.sambamba:MultiqcModule"
 samblaster = "multiqc.modules.samblaster:MultiqcModule"
 samtools = "multiqc.modules.samtools:MultiqcModule"
 sargasso = "multiqc.modules.sargasso:MultiqcModule"
 seqyclean = "multiqc.modules.seqyclean:MultiqcModule"
 seqwho = "multiqc.modules.seqwho:MultiqcModule"
@@ -205,22 +209,20 @@
 varscan2 = "multiqc.modules.varscan2:MultiqcModule"
 vcftools = "multiqc.modules.vcftools:MultiqcModule"
 vep = "multiqc.modules.vep:MultiqcModule"
 verifybamid = "multiqc.modules.verifybamid:MultiqcModule"
 whatshap = "multiqc.modules.whatshap:MultiqcModule"
 xenome = "multiqc.modules.xenome:MultiqcModule"
 xengsort = "multiqc.modules.xengsort:MultiqcModule"
-starsolo = "multiqc.modules.starsolo:MultiqcModule"
 
 [project.entry-points."multiqc.templates.v1"]
 default = "multiqc.templates.default"
 sections = "multiqc.templates.sections"
 simple = "multiqc.templates.simple"
 gathered = "multiqc.templates.gathered"
-highcharts = "multiqc.templates.highcharts"
 geo = "multiqc.templates.geo"
 
 ### See https://multiqc.info/docs/#multiqc-plugins for documentation
 #[project.entry-points."multiqc.cli_options.v1"]
 #my-new-option = "myplugin.cli:new_option"
 #
 #[project.entry-points."multiqc.hooks.v1"]
```

