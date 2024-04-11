# Comparing `tmp/rocco-0.9.4.tar.gz` & `tmp/rocco-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocco-0.9.4.tar", last modified: Fri Jan 26 22:01:20 2024, max compression
+gzip compressed data, was "rocco-0.9.5.tar", last modified: Mon Jan 29 20:28:31 2024, max compression
```

## Comparing `rocco-0.9.4.tar` & `rocco-0.9.5.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-26 22:01:20.256579 rocco-0.9.4/
--rw-r--r--   0 nhh        (501) staff       (20)     1071 2024-01-25 20:23:36.000000 rocco-0.9.4/LICENSE
--rw-r--r--   0 nhh        (501) staff       (20)       55 2024-01-25 20:23:36.000000 rocco-0.9.4/MANIFEST.in
--rw-r--r--   0 nhh        (501) staff       (20)     3729 2024-01-26 22:01:20.256358 rocco-0.9.4/PKG-INFO
--rw-r--r--   0 nhh        (501) staff       (20)     2514 2024-01-25 20:23:36.000000 rocco-0.9.4/README.md
-drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-26 22:01:20.254470 rocco-0.9.4/docs/
--rw-r--r--   0 nhh        (501) staff       (20)    89265 2024-01-25 20:23:36.000000 rocco-0.9.4/docs/logo.png
-drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-26 22:01:20.254800 rocco-0.9.4/rocco/
--rw-r--r--   0 nhh        (501) staff       (20)       50 2024-01-25 20:23:36.000000 rocco-0.9.4/rocco/__init__.py
--rw-r--r--   0 nhh        (501) staff       (20)    47308 2024-01-26 21:28:55.000000 rocco-0.9.4/rocco/rocco.py
-drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-26 22:01:20.255565 rocco-0.9.4/rocco.egg-info/
--rw-r--r--   0 nhh        (501) staff       (20)     3729 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/PKG-INFO
--rw-r--r--   0 nhh        (501) staff       (20)      302 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/SOURCES.txt
--rw-r--r--   0 nhh        (501) staff       (20)        1 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/dependency_links.txt
--rw-r--r--   0 nhh        (501) staff       (20)       43 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/entry_points.txt
--rw-r--r--   0 nhh        (501) staff       (20)      117 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/requires.txt
--rw-r--r--   0 nhh        (501) staff       (20)        6 2024-01-26 22:01:20.000000 rocco-0.9.4/rocco.egg-info/top_level.txt
--rw-r--r--   0 nhh        (501) staff       (20)       38 2024-01-26 22:01:20.256616 rocco-0.9.4/setup.cfg
--rw-r--r--   0 nhh        (501) staff       (20)     1708 2024-01-26 22:00:13.000000 rocco-0.9.4/setup.py
-drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-26 22:01:20.255795 rocco-0.9.4/tests/
--rw-r--r--   0 nhh        (501) staff       (20)     1729 2024-01-25 20:23:36.000000 rocco-0.9.4/tests/test_rocco.py
--rw-r--r--   0 nhh        (501) staff       (20)      655 2024-01-26 21:58:02.000000 rocco-0.9.4/tests/test_sample.py
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.814421 rocco-0.9.5/
+-rw-r--r--   0 nhh        (501) staff       (20)     1071 2024-01-29 14:52:32.000000 rocco-0.9.5/LICENSE
+-rw-r--r--   0 nhh        (501) staff       (20)       55 2024-01-29 14:52:32.000000 rocco-0.9.5/MANIFEST.in
+-rw-r--r--   0 nhh        (501) staff       (20)     3729 2024-01-29 20:28:31.814199 rocco-0.9.5/PKG-INFO
+-rw-r--r--   0 nhh        (501) staff       (20)     2514 2024-01-29 14:52:32.000000 rocco-0.9.5/README.md
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.811701 rocco-0.9.5/docs/
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.810895 rocco-0.9.5/docs/build_/
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.811895 rocco-0.9.5/docs/build_/_images/
+-rw-r--r--   0 nhh        (501) staff       (20)    89265 2024-01-29 14:52:32.000000 rocco-0.9.5/docs/build_/_images/logo.png
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.812320 rocco-0.9.5/docs/build_/_static/
+-rw-r--r--   0 nhh        (501) staff       (20)      286 2023-09-13 23:25:39.000000 rocco-0.9.5/docs/build_/_static/file.png
+-rw-r--r--   0 nhh        (501) staff       (20)       90 2023-09-13 23:25:39.000000 rocco-0.9.5/docs/build_/_static/minus.png
+-rw-r--r--   0 nhh        (501) staff       (20)       90 2023-09-13 23:25:39.000000 rocco-0.9.5/docs/build_/_static/plus.png
+-rw-r--r--   0 nhh        (501) staff       (20)    89265 2024-01-29 14:52:32.000000 rocco-0.9.5/docs/logo.png
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.812527 rocco-0.9.5/rocco/
+-rw-r--r--   0 nhh        (501) staff       (20)       50 2024-01-29 14:52:32.000000 rocco-0.9.5/rocco/__init__.py
+-rw-r--r--   0 nhh        (501) staff       (20)    48495 2024-01-29 20:24:15.000000 rocco-0.9.5/rocco/rocco.py
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.813437 rocco-0.9.5/rocco.egg-info/
+-rw-r--r--   0 nhh        (501) staff       (20)     3729 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/PKG-INFO
+-rw-r--r--   0 nhh        (501) staff       (20)      419 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/SOURCES.txt
+-rw-r--r--   0 nhh        (501) staff       (20)        1 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/dependency_links.txt
+-rw-r--r--   0 nhh        (501) staff       (20)       43 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/entry_points.txt
+-rw-r--r--   0 nhh        (501) staff       (20)      117 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/requires.txt
+-rw-r--r--   0 nhh        (501) staff       (20)        6 2024-01-29 20:28:31.000000 rocco-0.9.5/rocco.egg-info/top_level.txt
+-rw-r--r--   0 nhh        (501) staff       (20)       38 2024-01-29 20:28:31.814466 rocco-0.9.5/setup.cfg
+-rw-r--r--   0 nhh        (501) staff       (20)     1708 2024-01-29 20:25:06.000000 rocco-0.9.5/setup.py
+drwxr-xr-x   0 nhh        (501) staff       (20)        0 2024-01-29 20:28:31.813679 rocco-0.9.5/tests/
+-rw-r--r--   0 nhh        (501) staff       (20)     1729 2024-01-29 14:52:32.000000 rocco-0.9.5/tests/test_rocco.py
+-rw-r--r--   0 nhh        (501) staff       (20)      655 2024-01-29 14:52:32.000000 rocco-0.9.5/tests/test_sample.py
```

### Comparing `rocco-0.9.4/LICENSE` & `rocco-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rocco-0.9.4/PKG-INFO` & `rocco-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocco
-Version: 0.9.4
+Version: 0.9.5
 Summary: Robust ATAC-seq Peak Calling for Many Samples via Convex Optimization
 Home-page: https://github.com/nolan-h-hamilton/rocco
 Author: Nolan Holt Hamilton
 Author-email: nolan.hamilton@unc.edu
 Keywords: peak-caller,atac-seq,consensus-peaks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rocco-0.9.4/README.md` & `rocco-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `rocco-0.9.4/docs/logo.png` & `rocco-0.9.5/docs/build_/_images/logo.png`

 * *Files identical despite different names*

### Comparing `rocco-0.9.4/rocco/rocco.py` & `rocco-0.9.5/rocco/rocco.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 If using ROCCO in your research, please cite the `original paper <https://doi.org/10.1093/bioinformatics/btad725>`_ in *Bioinformatics*
 
 .. code-block:: text
 
     Nolan H Hamilton, Terrence S Furey, ROCCO: a robust method for detection of open chromatin via convex optimization,
     Bioinformatics, Volume 39, Issue 12, December 2023
 
-**DOI**: ``10.1093/bioinformatics/btad725``
+**DOI**: `10.1093/bioinformatics/btad725 <https://doi.org/10.1093/bioinformatics/btad725>`_
 
 
 Installation
 ===============
 
 ``pip install rocco``
 
@@ -203,15 +203,15 @@
 
 * Default parameters (constant or chromosome-specific) generally provide strong results, but users may consider tweaking the default parameters or filtering peaks by score with the `--peak_score_filter` argument.
 
 * Peak scores are computed as the average number of reads over the given peak region (w.r.t samples), divided by the length of the region, and then scaled to units of kilobases. A suitable peak score cutoff will depend on several experimental factors and may be evaluated by viewing the output histogram of peak scores.
 
 * If you encounter issues during the coverage track parsing/generation step, consider altering your pipeline to supply BedGraph input and verify constant bin sizes. Alternatively, you can use the API and manually supply a coverage matrix to execute ROCCO.
 
-* If RAM is a special consideration, you can try increasing `--step` or using a lightweight solver for the optimization, e.g., `pip` install `ortools` and run ROCCO with `--solver PDLP`
+* If RAM is a special consideration, you can try increasing `--step` from its default of `50` to, e.g., `100` and/or using a lightweight solver for the optimization, e.g., `pip` install `ortools` and run ROCCO with `--solver PDLP`
 
 
 To-Do Items
 ======================
 
 .. todolist::
 
@@ -225,14 +225,15 @@
 import multiprocessing
 import os
 from datetime import datetime
 from io import StringIO
 from pprint import pformat
 import random
 import subprocess
+import sys
 import types
 
 import cvxpy as cp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pysam
@@ -374,25 +375,28 @@
 
         return file_type
 
 
     def bam_to_coverage_dict(self, bamcov_cmd=None, additional_args=None):
         r"""
         Wraps deeptools' bamCoverage to generate a dictionary of chromosome-specific coverage tracks
-
         """
+        
         if bamcov_cmd is None:
             bamcov_cmd = ['bamCoverage', '--bam', self.input_file,
                     '--binSize', str(self.step),
                     '-o', f"{self.input_file + '.bw'}",
                     '-p', str(self.proc_num), '--samFlagInclude', '64']
             if additional_args:
                 bamcov_cmd.extend(additional_args)
-
-        subprocess.run(bamcov_cmd, check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        try:
+            subprocess.run(bamcov_cmd, check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        except:
+            logging.info(f"{bamcov_cmd} failed. Ensure input is a sorted/indexed BAM file and that deepTools is installed.")
+            raise
         self.bigwig_to_coverage_dict(input_=f"{self.input_file + '.bw'}")
         os.remove(f"{self.input_file + '.bw'}")
 
 
     def bedgraph_to_coverage_dict(self):
         r"""
         Parse a bedgraph file and store chromosome-specific coverage data in self.coverage_dict
@@ -530,14 +534,15 @@
         """
         vals = []
         try:
             vals = np.array([float(x) for x in self.coverage_dict[chromosome][1]])
         except KeyError:
             logging.info('coverage_dict has not been generated yet')
         return vals
+       
 
 
 class Rocco:
 
     r"""
     :param input_files: a list of samples' BAM files, or a list of samples' BigWig, or a list of samples' BedGraph files
     :type input_files: list
@@ -967,14 +972,16 @@
                 \begin{aligned}
                 & \underset{\boldsymbol{\ell}}{\text{ Minimize:}}
                 & & f_{\mathsf{IP}}(\boldsymbol{\ell}) = \sum_{i=1}^{n}-\left(\mathcal{S}(i)\cdot\ell_i\right) + \gamma\sum_{i=1}^{n-1} |\ell_i - \ell_{i+1}| \\
                 & \text{Subject To:} & &  \text{(i)}~~\sum_{i=1}^{n}\ell_i \leq \lfloor nb\rfloor \\
                 & & &  \text{(ii)}~~\ell_i \in \{0,1\}, ~\forall i=1 \ldots n.
                 \end{aligned}
 
+            where :math:`\ell_i` denotes the binary decision variable for the :math:`i` -th locus, :math:`\mathcal{S}(i)` denotes the 'score' for the :math:`i` -th locus, etc.
+            See paper for more details.
         """
         if Smat_chr or common_loci is None:
             common_loci, Smat_chr = self.get_Smat(chromosome)
         if scores is None:
             scores = self.get_scores(chromosome, Smat_chr)
         if budget is None:
             budget = self.param_df.loc[self.param_df['chrom'] == chromosome, 'budget'].values[0]
@@ -1096,19 +1103,19 @@
             plt.savefig(f"peak_score_hist_{self.curr_time}.pdf")
             plt.close()
 
         if not self.keep_chrom_bedfiles:
             self.delete_tempfiles()
 
 def main():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(description="ROCCO: [R]obust [O]pen [C]hromatin Detection via [C]onvex [O]ptimization", add_help=True)
     parser.add_argument('--input_files', '-i', nargs='+', type=str, help="Samples' corresponding BAM, bigwig, or bedgraph files. Accepts wildcard values, e.g., '*.bam', '*.bw'")
-    parser.add_argument('--chrom_param_file', type=str, default=None, help="Path to CSV param_file OR `hg38`/`mm10` for human/mouse default parameters")
+    parser.add_argument('--chrom_param_file', type=str, default=None, help="(Optional) Path to CSV param_file OR use `hg38`/`mm10` for human/mouse default parameters. If left unspecified, the 'constant_' parameters are used for all chromosomes.")
     parser.add_argument('--skip_chroms', nargs='+', type=str, default=[], help="Skip these chromosomes")
-    parser.add_argument('--genome_file', type=str, help="Genome sizes file")
+    parser.add_argument('--genome_file', type=str, help="Genome sizes file. A tab-separated file of the genome's chromosomes and their respective sizes measured in base pairs, e.g., `https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes`")
     parser.add_argument('--sample_weights', nargs='+', type=float, default=None)
     parser.add_argument('--pr_bed', type=str, help="BED file of blacklisted/problematic regions to exclude from peak annotation", default=None)
     parser.add_argument('--proc_num', '-p', default=max(multiprocessing.cpu_count()-1,1), type=int,
                         help='Number of processes to run simultaneously when generating coverage signals from BAM files')
     parser.add_argument('--constant_budget', default=0.035, type=float, help="'constant' parameters are used to fill in missing or NaN entries in the chromosome-specific parameter files/tables")
     parser.add_argument('--constant_gamma', default=1.0, type=float, help="'constant' parameters are used to fill in missing or NaN entries in the chromosome-specific parameter files/tables")
     parser.add_argument('--constant_tau', default=0.0, type=float, help="'constant' parameters are used to fill in missing or NaN entries in the chromosome-specific parameter files/tables")
@@ -1125,15 +1132,23 @@
     parser.add_argument('--peak_score_filter', default = 0.0, type=float, help='Only include peaks in the final annotation with peak scores above `--peak_score_filter`')
     parser.add_argument('--plot_hist', action='store_true', help="If `True` save a plotted histogram of peak scores")
     parser.add_argument('--outfile', '-o',
                         default=f"rocco_peaks_{datetime.now().strftime('%m%d%Y_%H%M%S')}.bed",
                         help='Name of output peak/BED file')
     parser.add_argument('--verbose_solving', action='store_true', default=False)
     args = vars(parser.parse_args())
-
+    
+    if args['input_files'] is None:
+        print('No input files `--input_files` were supplied. See `rocco --help`')
+        sys.exit(1)
+    
+    if args['genome_file'] is None:
+        print('No genome sizes file `--genome_file` was supplied. See `rocco --help`')
+        sys.exit(1)
+        
     filler_params = {'budget':args['constant_budget'],
                      'gamma':args['constant_gamma'],
                      'tau':args['constant_tau'],
                      'c_1':args['constant_c_1'],
                      'c_2':args['constant_c_2'],
                      'c_3':args['constant_c_3']}
```

### Comparing `rocco-0.9.4/rocco.egg-info/PKG-INFO` & `rocco-0.9.5/rocco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocco
-Version: 0.9.4
+Version: 0.9.5
 Summary: Robust ATAC-seq Peak Calling for Many Samples via Convex Optimization
 Home-page: https://github.com/nolan-h-hamilton/rocco
 Author: Nolan Holt Hamilton
 Author-email: nolan.hamilton@unc.edu
 Keywords: peak-caller,atac-seq,consensus-peaks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rocco-0.9.4/setup.py` & `rocco-0.9.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "- 'pytest': allows local execution of the Tests workflow.\n"
 )
 
 long_description += "\n\n" + optional_dependencies_message
 
 setup(
     name='rocco',
-    version='0.9.4',
+    version='0.9.5',
     author='Nolan Holt Hamilton',
     author_email='nolan.hamilton@unc.edu',
     description='Robust ATAC-seq Peak Calling for Many Samples via Convex Optimization',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/nolan-h-hamilton/rocco',
     packages=find_packages(),
```

### Comparing `rocco-0.9.4/tests/test_rocco.py` & `rocco-0.9.5/tests/test_rocco.py`

 * *Files identical despite different names*

### Comparing `rocco-0.9.4/tests/test_sample.py` & `rocco-0.9.5/tests/test_sample.py`

 * *Files identical despite different names*

