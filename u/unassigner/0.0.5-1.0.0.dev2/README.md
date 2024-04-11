# Comparing `tmp/unassigner-0.0.5.tar.gz` & `tmp/unassigner-1.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unassigner-0.0.5.tar", last modified: Tue May 23 19:19:24 2023, max compression
+gzip compressed data, was "unassigner-1.0.0.dev2.tar", last modified: Thu Apr 11 13:20:07 2024, max compression
```

## Comparing `unassigner-0.0.5.tar` & `unassigner-1.0.0.dev2.tar`

### file list

```diff
@@ -1,36 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 19:19:24.073719 unassigner-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-23 19:19:13.000000 unassigner-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:19:24.073719 unassigner-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 19:19:13.000000 unassigner-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_aligned.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_ani.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_mismatch_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_trim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/unassigner/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/ani.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/mismatch_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2856 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/prepare_strain_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/unassignment_probability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/unassigner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:07.953408 unassigner-1.0.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-11 13:20:07.953408 unassigner-1.0.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:20:07.953408 unassigner-1.0.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:07.953408 unassigner-1.0.0.dev2/unassigner/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8430 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/align.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17321 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/ani.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/mismatch_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2856 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/prepare_strain_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14782 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/trim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 13:20:03.000000 unassigner-1.0.0.dev2/unassigner/unassignment_probability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:20:07.953408 unassigner-1.0.0.dev2/unassigner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 13:20:07.000000 unassigner-1.0.0.dev2/unassigner.egg-info/top_level.txt
```

### Comparing `unassigner-0.0.5/PKG-INFO` & `unassigner-1.0.0.dev2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: unassigner
-Version: 0.0.5
+Version: 1.0.0.dev2
 Summary: Bacterial species unassigner
 Home-page: https://github.com/kylebittinger/unassigner
 Author: Kyle Bittinger
 Author-email: kylebittinger@gmail.com
 License: GPLv2+
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+Requires-Dist: biopython
+Requires-Dist: scipy
 
 # Unassigner
 
-[![Tests](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml)
-[![Super-Linter](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml)
-[![codecov](https://codecov.io/gh/Ulthran/unassigner/branch/master/graph/badge.svg?token=76YWJFWGON)](https://codecov.io/gh/Ulthran/unassigner)
-[![PyPi](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml)
+<!-- Begin badges -->
+[![Tests](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml/badge.svg)](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml)
+[![codecov](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner/graph/badge.svg?token=LAFU84K088)](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner)
+[![PyPI](https://badge.fury.io/py/unassigner.svg)](https://pypi.org/project/unassigner/)
+[![Bioconda](https://anaconda.org/bioconda/unassigner/badges/downloads.svg)](https://anaconda.org/bioconda/unassigner/)
+[![DockerHub](https://img.shields.io/docker/pulls/ctbushman/unassigner)](https://hub.docker.com/repository/docker/ctbushman/unassigner/)
+<!-- End badges -->
 
 Evaluate consistency with named bacterial species for short 16S rRNA
 marker gene sequences.
 
 ## Summary
 
 The [16S rRNA gene](https://en.wikipedia.org/wiki/16S_ribosomal_RNA)
@@ -57,53 +62,40 @@
 The unassigner library provides a command-line program, `unassign`,
 that takes a FASTA file of DNA sequences in a 16S gene region, and
 gives the probability that the sequence is inconsistent with nearby
 bacterial species.
 
 ## Installation
 
-The Python library and command-line program can be installed using
-[pip](https://pypi.org/project/pip/).
+Install with conda using:
 
 ```bash
-pip install unassigner
+conda create --name unassigner -c conda-forge -c bioconda unassigner
 ```
 
-Besides the python libraries listed in the setup file, this program
-requires `vsearch` to be installed.  This program is used to search
-for the closest matching bacterial species and return pairwise
-sequence alignments.  It's available through
-[conda](https://anaconda.org/bioconda/vsearch), and this is our
-recommended method for installation.
+Or run with Docker using:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-pip install unassigner
+docker run --rm -it ctbushman/unassigner:latest unassign --help
 ```
 
 ### Alternative Installation
 
-If `pip install unassigner` isn't working or if you want to use a development 
-version, you can also install via git.
+Unassigner can be installed using pip:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-git clone https://github.com/kylebittinger/unassigner.git
-cd unassigner
-pip install -r requirements.txt
-pip install .
+pip install unassigner
 ```
 
-If you don't want to use conda, see the 
-[vsearch repo](https://github.com/torognes/vsearch) for alternative install 
-methods.
+But will require ``vsearch`` to be installed separately. It can also be installed from GitHub:
+
+```bash
+git clone https://github.com/PennChopMicrobiomeProgram/unassigner.git
+pip install unassigner/
+```
 
 ## Usage
 
 The `unassign` program requires one argument, a FASTA-formatted file
 of short 16S sequences:
 
 ```bash
```

### Comparing `unassigner-0.0.5/README.md` & `unassigner-1.0.0.dev2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Unassigner
 
-[![Tests](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml)
-[![Super-Linter](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml)
-[![codecov](https://codecov.io/gh/Ulthran/unassigner/branch/master/graph/badge.svg?token=76YWJFWGON)](https://codecov.io/gh/Ulthran/unassigner)
-[![PyPi](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml)
+<!-- Begin badges -->
+[![Tests](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml/badge.svg)](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml)
+[![codecov](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner/graph/badge.svg?token=LAFU84K088)](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner)
+[![PyPI](https://badge.fury.io/py/unassigner.svg)](https://pypi.org/project/unassigner/)
+[![Bioconda](https://anaconda.org/bioconda/unassigner/badges/downloads.svg)](https://anaconda.org/bioconda/unassigner/)
+[![DockerHub](https://img.shields.io/docker/pulls/ctbushman/unassigner)](https://hub.docker.com/repository/docker/ctbushman/unassigner/)
+<!-- End badges -->
 
 Evaluate consistency with named bacterial species for short 16S rRNA
 marker gene sequences.
 
 ## Summary
 
 The [16S rRNA gene](https://en.wikipedia.org/wiki/16S_ribosomal_RNA)
@@ -41,53 +44,40 @@
 The unassigner library provides a command-line program, `unassign`,
 that takes a FASTA file of DNA sequences in a 16S gene region, and
 gives the probability that the sequence is inconsistent with nearby
 bacterial species.
 
 ## Installation
 
-The Python library and command-line program can be installed using
-[pip](https://pypi.org/project/pip/).
+Install with conda using:
 
 ```bash
-pip install unassigner
+conda create --name unassigner -c conda-forge -c bioconda unassigner
 ```
 
-Besides the python libraries listed in the setup file, this program
-requires `vsearch` to be installed.  This program is used to search
-for the closest matching bacterial species and return pairwise
-sequence alignments.  It's available through
-[conda](https://anaconda.org/bioconda/vsearch), and this is our
-recommended method for installation.
+Or run with Docker using:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-pip install unassigner
+docker run --rm -it ctbushman/unassigner:latest unassign --help
 ```
 
 ### Alternative Installation
 
-If `pip install unassigner` isn't working or if you want to use a development 
-version, you can also install via git.
+Unassigner can be installed using pip:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-git clone https://github.com/kylebittinger/unassigner.git
-cd unassigner
-pip install -r requirements.txt
-pip install .
+pip install unassigner
 ```
 
-If you don't want to use conda, see the 
-[vsearch repo](https://github.com/torognes/vsearch) for alternative install 
-methods.
+But will require ``vsearch`` to be installed separately. It can also be installed from GitHub:
+
+```bash
+git clone https://github.com/PennChopMicrobiomeProgram/unassigner.git
+pip install unassigner/
+```
 
 ## Usage
 
 The `unassign` program requires one argument, a FASTA-formatted file
 of short 16S sequences:
 
 ```bash
```

### Comparing `unassigner-0.0.5/setup.py` & `unassigner-1.0.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 PACKAGE_DIR = os.path.abspath(os.path.dirname(__file__))
 README_FP = os.path.join(PACKAGE_DIR, "README.md")
 with open(README_FP, encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="unassigner",
-    version="0.0.5",
+    version="1.0.0.dev2",
     description="Bacterial species unassigner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Kyle Bittinger",
     author_email="kylebittinger@gmail.com",
     url="https://github.com/kylebittinger/unassigner",
     packages=["unassigner"],
```

### Comparing `unassigner-0.0.5/unassigner/algorithm.py` & `unassigner-1.0.0.dev2/unassigner/algorithm.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/align.py` & `unassigner-1.0.0.dev2/unassigner/align.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/alignment.py` & `unassigner-1.0.0.dev2/unassigner/alignment.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/ani.py` & `unassigner-1.0.0.dev2/unassigner/ani.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/command.py` & `unassigner-1.0.0.dev2/unassigner/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import argparse
 import datetime
 import gzip
 import logging
 import os
+import pkg_resources
 
 from unassigner.algorithm import (
     UnassignAligner,
     FileAligner,
     UnassignerApp,
     VariableMismatchRate,
 )
 from unassigner.parse import parse_fasta, parse_species_names
 from unassigner.prepare_strain_data import download_type_strain_data
 
 
+__version__ = pkg_resources.get_distribution("unassigner").version
+
+
 def main(argv=None):
     p = argparse.ArgumentParser()
     p.add_argument(
         "query_fasta", type=argparse.FileType("r"), help="Query sequences FASTA file"
     )
     p.add_argument(
         "--output_dir",
@@ -59,14 +63,15 @@
             "use all the CPUs)"
         ),
     )
     p.add_argument(
         "--soft_threshold", action="store_true", help="Use soft threshold algorithm."
     )
     p.add_argument("--verbose", action="store_true", help="Activate verbose mode.")
+    p.add_argument("--version", action="version", version=f"{__version__}")
     args = p.parse_args(argv)
 
     if args.threshold is None:
         if args.soft_threshold:
             min_id = 0.991
         else:
             min_id = 0.975
```

### Comparing `unassigner-0.0.5/unassigner/download.py` & `unassigner-1.0.0.dev2/unassigner/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,19 @@
     "hi_tax_ltp",
     "riskgroup_ltp",
     "url_lpsn_ltp",
     "tax_ltp",
     "rel_ltp",
     "NJ_support_pk4_ltp",
 ]
+LTP_VERSION = "08_2023"
 LTP_METADATA_URL = (
-    "https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_06_2022.csv"
+    f"https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_{LTP_VERSION}.csv"
 )
-LTP_SEQS_URL = "https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_06_2022_blastdb.fasta"
+LTP_SEQS_URL = f"https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_{LTP_VERSION}_blastdb.fasta"
 GG_SEQS_URL = "ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_5.fasta.gz"
 GG_ACCESSIONS_URL = (
     "ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_5_accessions.txt.gz"
 )
 SPECIES_FASTA_FP = "unassigner_species.fasta"
 REFSEQS_FASTA_FP = "refseqs.fasta"
 GG_DUPLICATE_FP = "gg_duplicate_ids.txt"
```

### Comparing `unassigner-0.0.5/unassigner/find.py` & `unassigner-1.0.0.dev2/unassigner/find.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/mismatch_db.py` & `unassigner-1.0.0.dev2/unassigner/mismatch_db.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/parse.py` & `unassigner-1.0.0.dev2/unassigner/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,20 @@
         else:
             seq.write(line.replace(" ", "").replace("U", "T"))
     yield desc, seq.getvalue()
 
 
 def parse_desc(desc):
     try:
-        accession = re.findall(r"\[accession=(.*?)\]", desc)[0]
-        species_name = re.findall(r"\[organism=(.*?)\]", desc)[0]
+        arr = desc.split("|")
+        accession = arr[2]
+        species_name = arr[3]
+        # This is the old way of parsing the description, 01_2022
+        # accession = re.findall(r"\[accession=(.*?)\]", desc)[0]
+        # species_name = re.findall(r"\[organism=(.*?)\]", desc)[0]
     except IndexError as e:
         logging.error(f"Couldn't find accession and/or organism identifier in {desc}")
         logging.error(f"Skipping this sequence...")
         return None, None
     return accession, species_name
```

### Comparing `unassigner-0.0.5/unassigner/prepare_strain_data.py` & `unassigner-1.0.0.dev2/unassigner/prepare_strain_data.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner/trim.py` & `unassigner-1.0.0.dev2/unassigner/trim.py`

 * *Files identical despite different names*

### Comparing `unassigner-0.0.5/unassigner.egg-info/PKG-INFO` & `unassigner-1.0.0.dev2/unassigner.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 Metadata-Version: 2.1
 Name: unassigner
-Version: 0.0.5
+Version: 1.0.0.dev2
 Summary: Bacterial species unassigner
 Home-page: https://github.com/kylebittinger/unassigner
 Author: Kyle Bittinger
 Author-email: kylebittinger@gmail.com
 License: GPLv2+
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
+Requires-Dist: biopython
+Requires-Dist: scipy
 
 # Unassigner
 
-[![Tests](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/tests.yml)
-[![Super-Linter](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/linter.yml)
-[![codecov](https://codecov.io/gh/Ulthran/unassigner/branch/master/graph/badge.svg?token=76YWJFWGON)](https://codecov.io/gh/Ulthran/unassigner)
-[![PyPi](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Ulthran/unassigner/actions/workflows/python-publish.yml)
+<!-- Begin badges -->
+[![Tests](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml/badge.svg)](https://github.com/PennChopMicrobiomeProgram/unassigner/actions/workflows/pr.yml)
+[![codecov](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner/graph/badge.svg?token=LAFU84K088)](https://codecov.io/gh/PennChopMicrobiomeProgram/unassigner)
+[![PyPI](https://badge.fury.io/py/unassigner.svg)](https://pypi.org/project/unassigner/)
+[![Bioconda](https://anaconda.org/bioconda/unassigner/badges/downloads.svg)](https://anaconda.org/bioconda/unassigner/)
+[![DockerHub](https://img.shields.io/docker/pulls/ctbushman/unassigner)](https://hub.docker.com/repository/docker/ctbushman/unassigner/)
+<!-- End badges -->
 
 Evaluate consistency with named bacterial species for short 16S rRNA
 marker gene sequences.
 
 ## Summary
 
 The [16S rRNA gene](https://en.wikipedia.org/wiki/16S_ribosomal_RNA)
@@ -57,53 +62,40 @@
 The unassigner library provides a command-line program, `unassign`,
 that takes a FASTA file of DNA sequences in a 16S gene region, and
 gives the probability that the sequence is inconsistent with nearby
 bacterial species.
 
 ## Installation
 
-The Python library and command-line program can be installed using
-[pip](https://pypi.org/project/pip/).
+Install with conda using:
 
 ```bash
-pip install unassigner
+conda create --name unassigner -c conda-forge -c bioconda unassigner
 ```
 
-Besides the python libraries listed in the setup file, this program
-requires `vsearch` to be installed.  This program is used to search
-for the closest matching bacterial species and return pairwise
-sequence alignments.  It's available through
-[conda](https://anaconda.org/bioconda/vsearch), and this is our
-recommended method for installation.
+Or run with Docker using:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-pip install unassigner
+docker run --rm -it ctbushman/unassigner:latest unassign --help
 ```
 
 ### Alternative Installation
 
-If `pip install unassigner` isn't working or if you want to use a development 
-version, you can also install via git.
+Unassigner can be installed using pip:
 
 ```bash
-conda create --name unassigner
-conda activate unassigner
-conda install -c bioconda vsearch
-git clone https://github.com/kylebittinger/unassigner.git
-cd unassigner
-pip install -r requirements.txt
-pip install .
+pip install unassigner
 ```
 
-If you don't want to use conda, see the 
-[vsearch repo](https://github.com/torognes/vsearch) for alternative install 
-methods.
+But will require ``vsearch`` to be installed separately. It can also be installed from GitHub:
+
+```bash
+git clone https://github.com/PennChopMicrobiomeProgram/unassigner.git
+pip install unassigner/
+```
 
 ## Usage
 
 The `unassign` program requires one argument, a FASTA-formatted file
 of short 16S sequences:
 
 ```bash
```

