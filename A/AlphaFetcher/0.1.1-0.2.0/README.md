# Comparing `tmp/AlphaFetcher-0.1.1.tar.gz` & `tmp/AlphaFetcher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlphaFetcher-0.1.1.tar", last modified: Mon Oct  2 11:10:28 2023, max compression
+gzip compressed data, was "AlphaFetcher-0.2.0.tar", last modified: Thu Apr 11 15:09:40 2024, max compression
```

## Comparing `AlphaFetcher-0.1.1.tar` & `AlphaFetcher-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-10-02 11:10:28.563860 AlphaFetcher-0.1.1/
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-10-02 11:10:28.560818 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4828 2023-10-02 11:10:28.000000 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/PKG-INFO
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      301 2023-10-02 11:10:28.000000 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/SOURCES.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2023-10-02 11:10:28.000000 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/dependency_links.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       14 2023-10-02 11:10:28.000000 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/requires.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       13 2023-10-02 11:10:28.000000 AlphaFetcher-0.1.1/AlphaFetcher.egg-info/top_level.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      736 2023-08-31 16:05:49.000000 AlphaFetcher-0.1.1/LICENSE
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4828 2023-10-02 11:10:28.563501 AlphaFetcher-0.1.1/PKG-INFO
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     3531 2023-10-02 11:08:02.000000 AlphaFetcher-0.1.1/README.md
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-10-02 11:10:28.561362 AlphaFetcher-0.1.1/alphafetcher/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       47 2023-08-31 16:05:49.000000 AlphaFetcher-0.1.1/alphafetcher/__init__.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-10-02 11:10:28.562566 AlphaFetcher-0.1.1/alphafetcher/wrapper/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-31 16:05:49.000000 AlphaFetcher-0.1.1/alphafetcher/wrapper/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9303 2023-10-02 11:08:02.000000 AlphaFetcher-0.1.1/alphafetcher/wrapper/wrapper_utils.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-10-02 11:10:28.563971 AlphaFetcher-0.1.1/setup.cfg
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1638 2023-10-02 11:09:17.000000 AlphaFetcher-0.1.1/setup.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2024-04-11 15:09:40.079313 AlphaFetcher-0.2.0/
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2024-04-11 15:09:40.077388 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4949 2024-04-11 15:09:40.000000 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/PKG-INFO
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      301 2024-04-11 15:09:40.000000 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/SOURCES.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2024-04-11 15:09:40.000000 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/dependency_links.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       14 2024-04-11 15:09:40.000000 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/requires.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       13 2024-04-11 15:09:40.000000 AlphaFetcher-0.2.0/AlphaFetcher.egg-info/top_level.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      736 2023-08-31 16:05:49.000000 AlphaFetcher-0.2.0/LICENSE
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4949 2024-04-11 15:09:40.078526 AlphaFetcher-0.2.0/PKG-INFO
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     3577 2024-04-11 15:07:40.000000 AlphaFetcher-0.2.0/README.md
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2024-04-11 15:09:40.075315 AlphaFetcher-0.2.0/alphafetcher/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       47 2023-08-31 16:05:49.000000 AlphaFetcher-0.2.0/alphafetcher/__init__.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2024-04-11 15:09:40.076341 AlphaFetcher-0.2.0/alphafetcher/wrapper/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-31 16:05:49.000000 AlphaFetcher-0.2.0/alphafetcher/wrapper/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9303 2023-10-02 11:08:02.000000 AlphaFetcher-0.2.0/alphafetcher/wrapper/wrapper_utils.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2024-04-11 15:09:40.079493 AlphaFetcher-0.2.0/setup.cfg
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1688 2024-04-11 15:09:25.000000 AlphaFetcher-0.2.0/setup.py
```

### Comparing `AlphaFetcher-0.1.1/AlphaFetcher.egg-info/PKG-INFO` & `AlphaFetcher-0.2.0/AlphaFetcher.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: AlphaFetcher
-Version: 0.1.1
+Version: 0.2.0
 Summary: This package allows interface with the AlphaFold Protein Structure Database. This package allows the download of entries' metadata an AlphaFold files (e.g. mmCIF, PAE, PDB...)
 Home-page: https://bitbucket.org/bio2byte/alphafetcher/
 Author: Jose Gavalda-Garcia
 Author-email: jose.gavalda.garcia@vub.be
 Maintainer: Jose Gavalda-Garcia
 Maintainer-email: jose.gavalda.garcia@vub.be
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.6, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
 
 # AlphaFetcher
 
 `AlphaFetcher` facilitates fetching and downloading protein metadata and related files from the 
 [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/) 
 using Uniprot access codes.
 
@@ -67,14 +69,15 @@
 fetcher = AlphaFetcher(base_savedir="my_savedir")
 
 # Add desired Uniprot access codes
 fetcher.add_proteins(["A1KXE4", "H0YL14", "B2RXH2", "A8MVW5"])
 
 # Retrieve metadata
 fetcher.fetch_metadata(multithread=True, workers=4)
+# Metadata available at fetcher.metadata_dict
 
 # Commence download of specified files
 fetcher.download_all_files(pdb=True, cif=True, multithread=True, workers=4)
 ```
 
 ---
 
@@ -130,9 +133,7 @@
 - **Wim Vranken** - *Supervisor* - [wim.vranken@vub.be](mailto:wim.vranken@vub.be)
 
 ---
 
 ## 📄 License
 
 This project is licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-
```

### Comparing `AlphaFetcher-0.1.1/LICENSE` & `AlphaFetcher-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AlphaFetcher-0.1.1/PKG-INFO` & `AlphaFetcher-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: AlphaFetcher
-Version: 0.1.1
+Version: 0.2.0
 Summary: This package allows interface with the AlphaFold Protein Structure Database. This package allows the download of entries' metadata an AlphaFold files (e.g. mmCIF, PAE, PDB...)
 Home-page: https://bitbucket.org/bio2byte/alphafetcher/
 Author: Jose Gavalda-Garcia
 Author-email: jose.gavalda.garcia@vub.be
 Maintainer: Jose Gavalda-Garcia
 Maintainer-email: jose.gavalda.garcia@vub.be
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
-Platform: UNKNOWN
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.12
+Requires-Python: >=3.6, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: tqdm
 
 # AlphaFetcher
 
 `AlphaFetcher` facilitates fetching and downloading protein metadata and related files from the 
 [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/) 
 using Uniprot access codes.
 
@@ -67,14 +69,15 @@
 fetcher = AlphaFetcher(base_savedir="my_savedir")
 
 # Add desired Uniprot access codes
 fetcher.add_proteins(["A1KXE4", "H0YL14", "B2RXH2", "A8MVW5"])
 
 # Retrieve metadata
 fetcher.fetch_metadata(multithread=True, workers=4)
+# Metadata available at fetcher.metadata_dict
 
 # Commence download of specified files
 fetcher.download_all_files(pdb=True, cif=True, multithread=True, workers=4)
 ```
 
 ---
 
@@ -130,9 +133,7 @@
 - **Wim Vranken** - *Supervisor* - [wim.vranken@vub.be](mailto:wim.vranken@vub.be)
 
 ---
 
 ## 📄 License
 
 This project is licensed under the [GNU General Public License v3 (GPLv3)](https://www.gnu.org/licenses/gpl-3.0.en.html).
-
-
```

### Comparing `AlphaFetcher-0.1.1/README.md` & `AlphaFetcher-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 fetcher = AlphaFetcher(base_savedir="my_savedir")
 
 # Add desired Uniprot access codes
 fetcher.add_proteins(["A1KXE4", "H0YL14", "B2RXH2", "A8MVW5"])
 
 # Retrieve metadata
 fetcher.fetch_metadata(multithread=True, workers=4)
+# Metadata available at fetcher.metadata_dict
 
 # Commence download of specified files
 fetcher.download_all_files(pdb=True, cif=True, multithread=True, workers=4)
 ```
 
 ---
```

### Comparing `AlphaFetcher-0.1.1/alphafetcher/wrapper/wrapper_utils.py` & `AlphaFetcher-0.2.0/alphafetcher/wrapper/wrapper_utils.py`

 * *Files identical despite different names*

### Comparing `AlphaFetcher-0.1.1/setup.py` & `AlphaFetcher-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="AlphaFetcher",
-    version="0.1.1",
+    version="0.2.0",
     author="Jose Gavalda-Garcia",
     author_email="jose.gavalda.garcia@vub.be",
     description="This package allows interface with the AlphaFold Protein Structure Database. "
                 "This package allows the download of entries' metadata an AlphaFold files (e.g. mmCIF, PAE, PDB...)",
     license="OSI Approved :: GNU General Public License v3 (GPLv3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -22,20 +22,21 @@
         "Natural Language :: English",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "Development Status :: 5 - Production/Stable"
     ],
-    python_requires=">=3.6, <3.12",
+    python_requires=">=3.6, <3.13",
     install_requires=[
         "requests",
         "tqdm",
     ],
 )
```

