# Comparing `tmp/hiscanner-0.1a0.tar.gz` & `tmp/hiscanner-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiscanner-0.1a0.tar", max compression
+gzip compressed data, was "hiscanner-0.2a0.tar", max compression
```

## Comparing `hiscanner-0.1a0.tar` & `hiscanner-0.2a0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2024-02-20 18:56:31.532381 hiscanner-0.1a0/LICENSE
--rw-r--r--   0        0        0     2751 2024-02-20 18:59:21.971952 hiscanner-0.1a0/README.md
--rw-r--r--   0        0        0      584 2024-02-20 18:56:31.936093 hiscanner-0.1a0/hiscanner/__init__.py
--rw-r--r--   0        0        0      902 2024-02-20 18:56:31.944335 hiscanner-0.1a0/hiscanner/cli.py
--rwxr-xr-x   0        0        0    78024 2024-02-20 18:56:31.947735 hiscanner-0.1a0/hiscanner/cli_tools/linux/mbicseq
--rwxr-xr-x   0        0        0    68976 2024-02-20 18:56:31.946173 hiscanner-0.1a0/hiscanner/cli_tools/osx/mbicseq
--rw-r--r--   0        0        0   109724 2024-02-20 18:56:31.946931 hiscanner-0.1a0/hiscanner/cli_tools/win/mbicseq.exe
--rw-r--r--   0        0        0     3291 2024-02-20 18:56:31.948256 hiscanner-0.1a0/hiscanner/create_config.py
--rw-r--r--   0        0        0     2377 2024-02-20 18:56:31.935400 hiscanner-0.1a0/hiscanner/pl.py
--rw-r--r--   0        0        0     8120 2024-02-20 18:56:31.934805 hiscanner-0.1a0/hiscanner/pp.py
--rw-r--r--   0        0        0    12787 2024-02-20 18:56:31.949619 hiscanner-0.1a0/hiscanner/src/bin.c
--rw-r--r--   0        0        0     2546 2024-02-20 18:56:31.951669 hiscanner-0.1a0/hiscanner/src/bin.h
--rw-r--r--   0        0        0     5641 2024-02-20 18:56:31.950840 hiscanner-0.1a0/hiscanner/src/mbic-seq.c
--rw-r--r--   0        0        0    12271 2024-02-20 18:56:31.949125 hiscanner-0.1a0/hiscanner/src/rbtree.c
--rw-r--r--   0        0        0     1997 2024-02-20 18:56:31.950454 hiscanner-0.1a0/hiscanner/src/rbtree.h
--rw-r--r--   0        0        0     4435 2024-02-20 18:56:31.950103 hiscanner-0.1a0/hiscanner/src/read.c
--rw-r--r--   0        0        0      947 2024-02-20 18:56:31.951132 hiscanner-0.1a0/hiscanner/src/read.h
--rw-r--r--   0        0        0     2868 2024-02-20 18:56:31.936931 hiscanner-0.1a0/hiscanner/tl.py
--rw-r--r--   0        0        0    15918 2024-02-20 18:56:31.944922 hiscanner-0.1a0/hiscanner/utils.py
--rw-r--r--   0        0        0       23 2024-02-20 18:56:31.934058 hiscanner-0.1a0/hiscanner/version.py
--rw-r--r--   0        0        0     1058 2024-02-20 19:00:27.148440 hiscanner-0.1a0/pyproject.toml
--rwxr-xr-x   0        0        0    22192 2024-02-20 18:56:31.771959 hiscanner-0.1a0/scripts/mbicseq-norm/BICseq2-norm.pl
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 hiscanner-0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-20 18:56:31.532381 hiscanner-0.2a0/LICENSE
+-rw-r--r--   0        0        0     3603 2024-02-22 16:14:58.965768 hiscanner-0.2a0/README.md
+-rw-r--r--   0        0        0      584 2024-02-20 18:56:31.936093 hiscanner-0.2a0/hiscanner/__init__.py
+-rw-r--r--   0        0        0      902 2024-02-20 18:56:31.944335 hiscanner-0.2a0/hiscanner/cli.py
+-rwxr-xr-x   0        0        0    78024 2024-02-20 18:56:31.947735 hiscanner-0.2a0/hiscanner/cli_tools/linux/mbicseq
+-rwxr-xr-x   0        0        0    68976 2024-02-20 18:56:31.946173 hiscanner-0.2a0/hiscanner/cli_tools/osx/mbicseq
+-rw-r--r--   0        0        0   109724 2024-02-20 18:56:31.946931 hiscanner-0.2a0/hiscanner/cli_tools/win/mbicseq.exe
+-rw-r--r--   0        0        0     3291 2024-02-20 18:56:31.948256 hiscanner-0.2a0/hiscanner/create_config.py
+-rw-r--r--   0        0        0     2377 2024-02-20 18:56:31.935400 hiscanner-0.2a0/hiscanner/pl.py
+-rw-r--r--   0        0        0     8120 2024-02-20 18:56:31.934805 hiscanner-0.2a0/hiscanner/pp.py
+-rw-r--r--   0        0        0    12787 2024-02-20 18:56:31.949619 hiscanner-0.2a0/hiscanner/src/bin.c
+-rw-r--r--   0        0        0     2546 2024-02-20 18:56:31.951669 hiscanner-0.2a0/hiscanner/src/bin.h
+-rw-r--r--   0        0        0     5641 2024-02-20 18:56:31.950840 hiscanner-0.2a0/hiscanner/src/mbic-seq.c
+-rw-r--r--   0        0        0    12271 2024-02-20 18:56:31.949125 hiscanner-0.2a0/hiscanner/src/rbtree.c
+-rw-r--r--   0        0        0     1997 2024-02-20 18:56:31.950454 hiscanner-0.2a0/hiscanner/src/rbtree.h
+-rw-r--r--   0        0        0     4435 2024-02-20 18:56:31.950103 hiscanner-0.2a0/hiscanner/src/read.c
+-rw-r--r--   0        0        0      947 2024-02-20 18:56:31.951132 hiscanner-0.2a0/hiscanner/src/read.h
+-rw-r--r--   0        0        0     2870 2024-02-22 16:10:31.835844 hiscanner-0.2a0/hiscanner/tl.py
+-rw-r--r--   0        0        0    15918 2024-02-20 18:56:31.944922 hiscanner-0.2a0/hiscanner/utils.py
+-rw-r--r--   0        0        0       20 2024-02-22 15:54:55.636170 hiscanner-0.2a0/hiscanner/version.py
+-rw-r--r--   0        0        0     1058 2024-04-11 15:34:02.327000 hiscanner-0.2a0/pyproject.toml
+-rwxr-xr-x   0        0        0    22192 2024-02-20 18:56:31.771959 hiscanner-0.2a0/scripts/mbicseq-norm/BICseq2-norm.pl
+-rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 hiscanner-0.2a0/PKG-INFO
```

### Comparing `hiscanner-0.1a0/LICENSE` & `hiscanner-0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/README.md` & `hiscanner-0.2a0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <img src="image.png" alt="Logo generated by DALLE-3" width="80" height="90" style="float: right;"/>
 
-# HiScanner (High-resolutionSingle cell Allelic copy Number callER)
+# HiScanner (HIgh-resolution Single-Cell Allelic copy Number callER)
 [![PyPI version](https://badge.fury.io/py/hiscanner.svg)](https://badge.fury.io/py/hiscanner)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 HiScanner is a lightweight python package for high-resolution single-cell copy number analysis.
 
 ## Content
 - [Installation](#installation)
@@ -17,14 +17,15 @@
 - [LICENSE](#license)
 
 ## Installation
 
 It is recommended to install HiScanner in a virtual environment. Here's how to create one using conda:
 ```bash
 conda create -n hiscanner_env python=3.8
+conda activate hiscanner_env
 ```
 To install HiScanner, simply use pip:
 ```bash
 pip install hiscanner
 ```
 ## Requirements
 HiScanner requires [`bcftools`](https://samtools.github.io/bcftools/bcftools.html), which must be included in `PATH`. All other dependencies should be installed automatically with pip.
@@ -49,14 +50,43 @@
 ## Command line interface
 For advanced users interested in multi-sample segmentation (e.g., repurposing for bulk samples), HiScanner provides a command line interface. In bash, simply run:
 ```bash
 hiscanner-segment -i {input_file} -l {LAMBDA} -o {output_file}
 ```
 For more details, please refer to our [documentation](https://github.com/parklab/hiscanner/tree/main/docs).
 
+## Required input
+### 1) JSON 
+HiScanner requires a json file as input. Here's an example:
+```
+{
+    "bin_path": "/Users/yifan/dev/scanner_tutorial/tests/data/bins",
+    "phase_file": "/Users/yifan/dev/scanner_tutorial/tests/data/hsnps/samplename_phased_hsnps.vcf",
+    "germline": "bulkname",
+    "gatk_vcf": "/Users/yifan/dev/scanner_tutorial/tests/data/hsnps/samplename_gatk.vcf",
+    "stem": "/Users/yifan/dev/scanner_tutorial/tests/data/output/",
+    "j": 20,
+    "singlecell":"cellA,cellB",
+    "MAX_WGD": 1,
+    "LAMBDA":200
+}
+
+```
+### 2) BAM
+The BAM file should be indexed and sorted.
+### 3) Unphased VCF 
+output from GATK  or SCAN-SNV;
+The VCF file should be indexed and sorted.
+### 4) Phased VCF 
+output from Eagle or other phasing tools;
+### 5) Bins
+The bins file should be a bed file (output from BIC-seq2)
+
+
+
 ## Operating System
 HiScanner was tested in the following operating systems:
 - macOS Ventura 13.5.2
 - CentOS Linux 7.9
 - Windows 11
 
 ## Documentation
```

### Comparing `hiscanner-0.1a0/hiscanner/__init__.py` & `hiscanner-0.2a0/hiscanner/__init__.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/cli.py` & `hiscanner-0.2a0/hiscanner/cli.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/cli_tools/linux/mbicseq` & `hiscanner-0.2a0/hiscanner/cli_tools/linux/mbicseq`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/cli_tools/osx/mbicseq` & `hiscanner-0.2a0/hiscanner/cli_tools/osx/mbicseq`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/cli_tools/win/mbicseq.exe` & `hiscanner-0.2a0/hiscanner/cli_tools/win/mbicseq.exe`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/create_config.py` & `hiscanner-0.2a0/hiscanner/create_config.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/pl.py` & `hiscanner-0.2a0/hiscanner/pl.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/pp.py` & `hiscanner-0.2a0/hiscanner/pp.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/bin.c` & `hiscanner-0.2a0/hiscanner/src/bin.c`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/bin.h` & `hiscanner-0.2a0/hiscanner/src/bin.h`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/mbic-seq.c` & `hiscanner-0.2a0/hiscanner/src/mbic-seq.c`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/rbtree.c` & `hiscanner-0.2a0/hiscanner/src/rbtree.c`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/rbtree.h` & `hiscanner-0.2a0/hiscanner/src/rbtree.h`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/read.c` & `hiscanner-0.2a0/hiscanner/src/read.c`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/src/read.h` & `hiscanner-0.2a0/hiscanner/src/read.h`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/hiscanner/tl.py` & `hiscanner-0.2a0/hiscanner/tl.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(json_file_path, 'r') as file:
         args = json.load(file)
     # check if bicseq is in the path
     bicseq = args.get('bicseq_path')
     singlecell = args.get('singlecell').split(',')
     stem = args.get('stem')
     RDR_LAMBDA = args.get('LAMBDA')
-    assert os.system('scanner-segment -h > /dev/null 2>&1') == 0
+    assert os.system('hiscanner-segment -h > /dev/null 2>&1') == 0
 
     print('Reshaping data for bicseq segmentation')
     # reshape the data for bicseq segmentation
     for c in singlecell:
         cell_df = pd.read_csv(f'{stem}/{c}.data.txt',sep='\t')
         cell_df = cell_df[['CHROM','START','END','OBS','EXP']]
         cell_df.columns = ['CHROM','START','END',f'A_{c}',f'B_{c}']
```

### Comparing `hiscanner-0.1a0/hiscanner/utils.py` & `hiscanner-0.2a0/hiscanner/utils.py`

 * *Files identical despite different names*

### Comparing `hiscanner-0.1a0/pyproject.toml` & `hiscanner-0.2a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hiscanner"
-version = "0.1a"
+version = "0.2a"
 description = "High-resolution copy number variant calling in single-cell whole-genome sequencing."
 authors = ["Yifan Zhao"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["genomics", "CNV", "CNA", "single cell"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `hiscanner-0.1a0/scripts/mbicseq-norm/BICseq2-norm.pl` & `hiscanner-0.2a0/scripts/mbicseq-norm/BICseq2-norm.pl`

 * *Files identical despite different names*

