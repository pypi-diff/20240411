# Comparing `tmp/flams-1.1.3.tar.gz` & `tmp/flams-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flams-1.1.3.tar", last modified: Tue Nov 28 17:57:02 2023, max compression
+gzip compressed data, was "flams-1.1.4.tar", last modified: Thu Apr 11 11:59:32 2024, max compression
```

## Comparing `flams-1.1.3.tar` & `flams-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:57:02.327974 flams-1.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-11-28 17:56:48.000000 flams-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20776 2023-11-28 17:57:02.327974 flams-1.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    20104 2023-11-28 17:56:48.000000 flams-1.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-11-28 17:56:48.000000 flams-1.1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-11-28 17:56:48.000000 flams-1.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-28 17:57:02.327974 flams-1.1.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:57:02.323974 flams-1.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:57:02.327974 flams-1.1.3/src/flams/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:57:02.327974 flams-1.1.3/src/flams/databases/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/databases/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2874 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/databases/cplmv4.py
--rw-rw-rw-   0 root         (0) root         (0)     5695 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/databases/dbptm.py
--rw-rw-rw-   0 root         (0) root         (0)    23906 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/databases/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8289 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/display.py
--rw-rw-rw-   0 root         (0) root         (0)     5019 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/flams.py
--rw-rw-rw-   0 root         (0) root         (0)    30708 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/input.py
--rw-rw-rw-   0 root         (0) root         (0)    13730 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/run_blast.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-11-28 17:56:48.000000 flams-1.1.3/src/flams/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-28 17:57:02.327974 flams-1.1.3/src/flams.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20776 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      216 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-11-28 17:57:02.000000 flams-1.1.3/src/flams.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:59:32.475398 flams-1.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2024-04-11 11:59:20.000000 flams-1.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    21942 2024-04-11 11:59:32.475398 flams-1.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    21270 2024-04-11 11:59:20.000000 flams-1.1.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      456 2024-04-11 11:59:20.000000 flams-1.1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      656 2024-04-11 11:59:20.000000 flams-1.1.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 11:59:32.475398 flams-1.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:59:32.471398 flams-1.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:59:32.471398 flams-1.1.4/src/flams/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:59:21.000000 flams-1.1.4/src/flams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:59:32.475398 flams-1.1.4/src/flams/databases/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 11:59:21.000000 flams-1.1.4/src/flams/databases/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2874 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/databases/cplmv4.py
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/databases/dbptm.py
+-rw-rw-rw-   0 root         (0) root         (0)    24304 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/databases/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8289 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/display.py
+-rw-rw-rw-   0 root         (0) root         (0)     5019 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/flams.py
+-rw-rw-rw-   0 root         (0) root         (0)    30812 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/input.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/run_blast.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-04-11 11:59:20.000000 flams-1.1.4/src/flams/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 11:59:32.475398 flams-1.1.4/src/flams.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    21942 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      216 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-11 11:59:32.000000 flams-1.1.4/src/flams.egg-info/top_level.txt
```

### Comparing `flams-1.1.3/LICENSE` & `flams-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/PKG-INFO` & `flams-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flams
-Version: 1.1.3
+Version: 1.1.4
 Summary: Find Lysine Acylations & other Modification Sites
 Project-URL: repository, https://github.com/hannelorelongin/FLAMS
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: appdirs==1.4.4
 Requires-Dist: biopython==1.81
@@ -98,29 +98,29 @@
 
 Optional arguments:
 * `errorRange` is an number of positions before and after `position` to also search for modifications. [default: 0]
 * `outputFilePath` is the path to where the result will be saved (in a .tsv file format). [default: out.tsv] If FLAMS is run with --batch, the specified -o/--output is used as preposition, followed by '\_$UniProtID\_$position.tsv'. [default: '']
 * `dataDir` is the path to the directory where intermediate files (the UniProt sequence files) are stored. [default: $PWD/data]
 * `threadsBLAST` is a BLAST parameter, allows you to speed up the search by multithreading. [default: 1]
 * `evalueBLAST` is a BLAST parameter, allows you to filter out low quality BLAST hits. [default: 0.01]
-* `modification` is a space-seperated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
+* `modification` is a space-separated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
 
 ### Example use case
 
 We provide two example use cases for FLAMS:
 
 With the following command, you search whether the TatA (UniProt ID: A0A916NWA0) acetylation on K66 in *Dehalococcoide mccartyi* strain CBDB1, as described by [Greiner-Haas (2021)](https://doi.org/10.3390/microorganisms9020365), had been previously detected.
 
 `FLAMS --in A0A916NWA0.fa -p 66 -m acetylation -o tatA.tsv`
 
 With the following command, you search whether the *Mycobabcterium smegmatis*' FadD2 (UniProt ID: A0QQ22) K537 is known to carry any modifications of the 'acylations' category, similar to what was reported by [Xu (2020)](https://doi.org/10.1128/mSystems.00424-19).
 
 `FLAMS --id A0QQ22 -p 537 -m CPLM-Acylations -o FadD2.tsv`
 
-You can find the example input and output data in the folder `test_data`.
+You can find the example input and output data in the folder `test_data`. The output data is organized in folders reflecting the FLAMS version used to generate it, as the output can vary depending on the exact FLAMS version (due to FLAMS database updates).
 
 For more example use cases, see the Supplementary information of the paper.
 
 ## Output
 
 The output file is a .tsv containing one row per modification that matched the query, i.e., a modification aligning (within the user-specified range) to the query position, in a protein similar to the query protein. In case of batch jobs (ran with --batch), one output file per query (= a single line in the batch job file) will be generated.
 
@@ -145,20 +145,21 @@
 
 ## Supported PTMs
 
 ### Supported PTM databases
 
 FLAMS updates its search databases regularly. To get an overview of the supported databases, see the table below.
 
-|FLAMS version|CPLM version|dbPTM version|database available for download|
-|:----|:----|:----|:----|
-|v1.1|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|
-|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|
+|FLAMS version|CPLM version|dbPTM version|database available for download|UniProt release|
+|:----|:----|:----|:----|:----|
+|v1.1.4|v4|2024_April|[yes](https://doi.org/10.5281/zenodo.10958721)|2024_02|
+|v1.1.0-3|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|2023_05|
+|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|NA|
 
-Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). Moreover, proteins that carry a UniProt ID that was obsolete or missing at the time of database creation are also not included in the database.
+Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). As dbPTM does not store complete protein sequences, these are fetched during database creation based on UniProt identifiers reported in dbPTM and the UniProt release available at the time of database creation. As a consequence, FLAMS database updates can change the content of the PTM databases, beyond the simple addition of new dbPTM and/or CPLM entries, reflecting changes in UniProt. The most common UniProt changes affecting FLAMS databases are removed UniProt entries (leading to the removal of PTM entries on the affected protein in our database) and sequence updates. We are aware of this issue, impacting the completeness and interpretation of FLAMS' results, and will consider solutions in future FLAMS releases.
 
 Instructions on how to download the CPLM and dbPTM database yourself are in [section 'Local CPLM and dbPTM install'](#local-cplm-and-dbptm-install). This is not recommended, as it takes multiple hours to generate some databases.
 
 ### Supported PTM types
 
 FLAMS allows searches for all PTM types included in CPLM, and for those with experimental evidence in dbPTM. An overview of the PTM types, how to call them in FLAMS, how they are called in CPLM and/or dbPTM, and on which amino acid they can be found is given in the table below. This table can also be found as a tab seperated file named FLAMS_supported_ptms_v11.txt .
 
@@ -181,15 +182,17 @@
 |citrullination| |Citrullination| | | | | | | |  | | | | | | |X| | | | | | | | | |
 |crotonylation|Crotonylation|Crotonylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
 |c-linked_glycosylation| |C-linked Glycosylation| | | | | | | | | | | | | | | | | | |X| | | | | |
 |deamidation| |Deamidation| | | | | | | | | | | |X| |X| | | | | | | | | | |
 |deamination| |Deamination| | | | | | | | |X| | | | | | | | | | | | | | | |
 |decanoylation| |Decanoylation| | | | | | | | | | | | | | | |X|X| | | | | | | |
 |decarboxylation| |Decarboxylation| | |X| | | | | | | | | | | | | |X| | | | | | | |
+|dephosphorylation| |Dephosphorylation| | | | | | | | | | | | | | | |X|X| | |X| | | | |
 |dietylphosphorylation|Dietylphosphorylation| | | | | | | | | |X| | | | | | | | | | | | | |X|X|
+|disulfide_bond| |Disulfide bond| |X| | | | | | | | | | | | | | | | | | | | | | |
 |d-glucuronylation| |D-glucuronoylation| | | | | |X| | | | | | | | | | | | | | | | | | |
 |farnesylation| |Farnesylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |formation_of_an_isopeptide_bond| |Formation of an isopeptide bond| | | |X| | | | | | | | | |X| | | | | | | | | | |
 |formylation|Formylation|Formylation| | | | | |X| | |X| |X| | | | | | | | | |X| | |X|
 |gamma-carboxyglutamic_acid| |Gamma-carboxyglutamic acid| | | |X| | | | | | | | | | | | | | | | | | | | |
 |geranylgeranylation| |Geranylgeranylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |glutarylation|Glutarylation|Glutarylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
@@ -283,23 +286,25 @@
       ),`
 
     - comment out lines 503-508 (function `_generate_blastdb_if_not_up_to_date` - the try/except _get_fasta_from_zenodo)
     - uncomment line 512 (function `_generate_blastdb_if_not_up_to_date` - the _get_fasta_for_blast)
 
 3. Install your adapted FLAMS version locally:
 
-  `python -m pip install ./PathToLocalFLAMS`
+    `python -m pip install ./PathToLocalFLAMS`
 
 ## Contact
 
 Laboratory of Computational Systems Biology, KU Leuven.
 
 ## References
 
-If you use FLAMS in your work, please cite us.
+If you use FLAMS in your work, please cite:
+
+Longin, H. *et al* (2024) "FLAMS: Find Lysine Acylations and other Modification Sites." Bioinformatics. 40(1):btae005.
 
 In addition, FLAMS relies on third-party software & databases:
 
 Altschul, S.F. *et al* (1990) "Basic local alignment search tool." J. Mol. Biol. 215:403-410.
 
 Li, Z. *et al* (2022) "dbPTM in 2022: an updated database for exploring regulatory networks and functional associations of protein post-translational modifications." Nucleic Acids Research. 50:D471–D479.
```

### Comparing `flams-1.1.3/README.md` & `flams-1.1.4/src/flams.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: flams
+Version: 1.1.4
+Summary: Find Lysine Acylations & other Modification Sites
+Project-URL: repository, https://github.com/hannelorelongin/FLAMS
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: appdirs==1.4.4
+Requires-Dist: biopython==1.81
+Requires-Dist: certifi==2023.5.7
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: idna==3.4
+Requires-Dist: numpy==1.24.3
+Requires-Dist: pandas==2.1.2
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: pytz==2023.3.post1
+Requires-Dist: requests==2.29.0
+Requires-Dist: six==1.16.0
+Requires-Dist: tzdata==2023.3
+Requires-Dist: urllib3==1.26.18
+
 # FLAMS: Find Lysine Acylations & other Modification Sites
 
 A bioinformatics tool to analyze the conservation of post-translational modifications (PTMs), by means of a position-based search against the Compendium of Protein Lysine Modifications (CPLM database) v.4 and the experimental PTM sites in dbPTM. FLAMS is available as command-line tool and as a [web service](https://www.biw.kuleuven.be/m2s/cmpg/research/CSB/tools/flams/).
 
 # Table of contents
 
 1.  [Introduction](#introduction)
@@ -76,29 +98,29 @@
 
 Optional arguments:
 * `errorRange` is an number of positions before and after `position` to also search for modifications. [default: 0]
 * `outputFilePath` is the path to where the result will be saved (in a .tsv file format). [default: out.tsv] If FLAMS is run with --batch, the specified -o/--output is used as preposition, followed by '\_$UniProtID\_$position.tsv'. [default: '']
 * `dataDir` is the path to the directory where intermediate files (the UniProt sequence files) are stored. [default: $PWD/data]
 * `threadsBLAST` is a BLAST parameter, allows you to speed up the search by multithreading. [default: 1]
 * `evalueBLAST` is a BLAST parameter, allows you to filter out low quality BLAST hits. [default: 0.01]
-* `modification` is a space-seperated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
+* `modification` is a space-separated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
 
 ### Example use case
 
 We provide two example use cases for FLAMS:
 
 With the following command, you search whether the TatA (UniProt ID: A0A916NWA0) acetylation on K66 in *Dehalococcoide mccartyi* strain CBDB1, as described by [Greiner-Haas (2021)](https://doi.org/10.3390/microorganisms9020365), had been previously detected.
 
 `FLAMS --in A0A916NWA0.fa -p 66 -m acetylation -o tatA.tsv`
 
 With the following command, you search whether the *Mycobabcterium smegmatis*' FadD2 (UniProt ID: A0QQ22) K537 is known to carry any modifications of the 'acylations' category, similar to what was reported by [Xu (2020)](https://doi.org/10.1128/mSystems.00424-19).
 
 `FLAMS --id A0QQ22 -p 537 -m CPLM-Acylations -o FadD2.tsv`
 
-You can find the example input and output data in the folder `test_data`.
+You can find the example input and output data in the folder `test_data`. The output data is organized in folders reflecting the FLAMS version used to generate it, as the output can vary depending on the exact FLAMS version (due to FLAMS database updates).
 
 For more example use cases, see the Supplementary information of the paper.
 
 ## Output
 
 The output file is a .tsv containing one row per modification that matched the query, i.e., a modification aligning (within the user-specified range) to the query position, in a protein similar to the query protein. In case of batch jobs (ran with --batch), one output file per query (= a single line in the batch job file) will be generated.
 
@@ -123,20 +145,21 @@
 
 ## Supported PTMs
 
 ### Supported PTM databases
 
 FLAMS updates its search databases regularly. To get an overview of the supported databases, see the table below.
 
-|FLAMS version|CPLM version|dbPTM version|database available for download|
-|:----|:----|:----|:----|
-|v1.1|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|
-|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|
+|FLAMS version|CPLM version|dbPTM version|database available for download|UniProt release|
+|:----|:----|:----|:----|:----|
+|v1.1.4|v4|2024_April|[yes](https://doi.org/10.5281/zenodo.10958721)|2024_02|
+|v1.1.0-3|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|2023_05|
+|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|NA|
 
-Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). Moreover, proteins that carry a UniProt ID that was obsolete or missing at the time of database creation are also not included in the database.
+Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). As dbPTM does not store complete protein sequences, these are fetched during database creation based on UniProt identifiers reported in dbPTM and the UniProt release available at the time of database creation. As a consequence, FLAMS database updates can change the content of the PTM databases, beyond the simple addition of new dbPTM and/or CPLM entries, reflecting changes in UniProt. The most common UniProt changes affecting FLAMS databases are removed UniProt entries (leading to the removal of PTM entries on the affected protein in our database) and sequence updates. We are aware of this issue, impacting the completeness and interpretation of FLAMS' results, and will consider solutions in future FLAMS releases.
 
 Instructions on how to download the CPLM and dbPTM database yourself are in [section 'Local CPLM and dbPTM install'](#local-cplm-and-dbptm-install). This is not recommended, as it takes multiple hours to generate some databases.
 
 ### Supported PTM types
 
 FLAMS allows searches for all PTM types included in CPLM, and for those with experimental evidence in dbPTM. An overview of the PTM types, how to call them in FLAMS, how they are called in CPLM and/or dbPTM, and on which amino acid they can be found is given in the table below. This table can also be found as a tab seperated file named FLAMS_supported_ptms_v11.txt .
 
@@ -159,15 +182,17 @@
 |citrullination| |Citrullination| | | | | | | |  | | | | | | |X| | | | | | | | | |
 |crotonylation|Crotonylation|Crotonylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
 |c-linked_glycosylation| |C-linked Glycosylation| | | | | | | | | | | | | | | | | | |X| | | | | |
 |deamidation| |Deamidation| | | | | | | | | | | |X| |X| | | | | | | | | | |
 |deamination| |Deamination| | | | | | | | |X| | | | | | | | | | | | | | | |
 |decanoylation| |Decanoylation| | | | | | | | | | | | | | | |X|X| | | | | | | |
 |decarboxylation| |Decarboxylation| | |X| | | | | | | | | | | | | |X| | | | | | | |
+|dephosphorylation| |Dephosphorylation| | | | | | | | | | | | | | | |X|X| | |X| | | | |
 |dietylphosphorylation|Dietylphosphorylation| | | | | | | | | |X| | | | | | | | | | | | | |X|X|
+|disulfide_bond| |Disulfide bond| |X| | | | | | | | | | | | | | | | | | | | | | |
 |d-glucuronylation| |D-glucuronoylation| | | | | |X| | | | | | | | | | | | | | | | | | |
 |farnesylation| |Farnesylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |formation_of_an_isopeptide_bond| |Formation of an isopeptide bond| | | |X| | | | | | | | | |X| | | | | | | | | | |
 |formylation|Formylation|Formylation| | | | | |X| | |X| |X| | | | | | | | | |X| | |X|
 |gamma-carboxyglutamic_acid| |Gamma-carboxyglutamic acid| | | |X| | | | | | | | | | | | | | | | | | | | |
 |geranylgeranylation| |Geranylgeranylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |glutarylation|Glutarylation|Glutarylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
@@ -261,23 +286,25 @@
       ),`
 
     - comment out lines 503-508 (function `_generate_blastdb_if_not_up_to_date` - the try/except _get_fasta_from_zenodo)
     - uncomment line 512 (function `_generate_blastdb_if_not_up_to_date` - the _get_fasta_for_blast)
 
 3. Install your adapted FLAMS version locally:
 
-  `python -m pip install ./PathToLocalFLAMS`
+    `python -m pip install ./PathToLocalFLAMS`
 
 ## Contact
 
 Laboratory of Computational Systems Biology, KU Leuven.
 
 ## References
 
-If you use FLAMS in your work, please cite us.
+If you use FLAMS in your work, please cite:
+
+Longin, H. *et al* (2024) "FLAMS: Find Lysine Acylations and other Modification Sites." Bioinformatics. 40(1):btae005.
 
 In addition, FLAMS relies on third-party software & databases:
 
 Altschul, S.F. *et al* (1990) "Basic local alignment search tool." J. Mol. Biol. 215:403-410.
 
 Li, Z. *et al* (2022) "dbPTM in 2022: an updated database for exploring regulatory networks and functional associations of protein post-translational modifications." Nucleic Acids Research. 50:D471–D479.
```

### Comparing `flams-1.1.3/requirements.txt` & `flams-1.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/databases/cplmv4.py` & `flams-1.1.4/src/flams/databases/cplmv4.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/databases/dbptm.py` & `flams-1.1.4/src/flams/databases/dbptm.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/databases/setup.py` & `flams-1.1.4/src/flams/databases/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,403 +62,414 @@
     dbs: List[ModificationDatabase]
     aas: List[str]
 
 
 # Here we store a dict of Zenodo URLs that can be queried for.
 version_urls = {
     1.0: "https://zenodo.org/records/10143464/files/{0}-{1}.zip?download=1",
-    1.1: "https://zenodo.org/records/10171879/files/{0}-{1}.zip?download=1"
+    1.1: "https://zenodo.org/records/10171879/files/{0}-{1}.zip?download=1",
+    1.2: "https://zenodo.org/records/10958721/files/{0}-{1}.fasta.zip?download=1"
     }
 
 # Here we store a dict of modifications that can be queried for.
     # sorted alphabetically
 MODIFICATIONS = {
     "acetylation": ModificationType(
-        "acetylation", 1.1,
+        "acetylation", 1.2,
         [ModificationDatabase(cplmv4, "Acetylation"), ModificationDatabase(dbptm,"Acetylation")],
         ["A","C","D","E","G","K","M","P","R","S","T","V","Y"]
     ),
     "adp-ribosylation": ModificationType(
-        "adp-ribosylation", 1.1,
+        "adp-ribosylation", 1.2,
         [ModificationDatabase(dbptm, "ADP-ribosylation")],
         ["C","D","E","G","H","K","N","R","S","Y"]
     ),
     "amidation": ModificationType(
-        "amidation", 1.1,
+        "amidation", 1.2,
         [ModificationDatabase(dbptm, "Amidation")],
         ["A","C","D","E","F","G","H","I","K","L","M","N","P","Q","R","S","T","V","W","Y"]
     ),
     "ampylation" : ModificationType(
-        "ampylation", 1.1,
+        "ampylation", 1.2,
         [ModificationDatabase(dbptm, "AMPylation")],
         ["S","T","Y"]
     ),
     "benzoylation": ModificationType(
-        "benzoylation", 1.1, [ModificationDatabase(cplmv4, "Benzoylation")],
+        "benzoylation", 1.2, [ModificationDatabase(cplmv4, "Benzoylation")],
         ["K"]
     ),
     "beta-hydroxybutyrylation": ModificationType(
-        "beta-hydroxybutyrylation", 1.1, [ModificationDatabase(cplmv4, "β-Hydroxybutyrylation")],
+        "beta-hydroxybutyrylation", 1.2, [ModificationDatabase(cplmv4, "β-Hydroxybutyrylation")],
         ["K"]
     ),
     "biotinylation": ModificationType(
-        "biotinylation", 1.1,
+        "biotinylation", 1.2,
         [ModificationDatabase(cplmv4, "Biotinylation"), ModificationDatabase(dbptm, "Biotinylation")],
         ["K"]
     ),
     "blocked_amino_end": ModificationType(
-        "blocked_amino_end", 1.1,
+        "blocked_amino_end", 1.2,
         [ModificationDatabase(dbptm, "Blocked amino end")],
         ["A","C","D","E","G","H","I","L","M","N","P","Q","R","S","T","V"]
     ),
     "butyrylation": ModificationType(
-        "butyrylation", 1.1,
+        "butyrylation", 1.2,
         [ModificationDatabase(cplmv4, "Butyrylation"), ModificationDatabase(dbptm, "Butyrylation")],
         ["K"]
     ),
     "carbamidation": ModificationType(
-        "carbamidation", 1.1,
+        "carbamidation", 1.2,
         [ModificationDatabase(dbptm, "Carbamidation")],
         ["C"]
     ),
     "carboxyethylation": ModificationType(
-        "carboxyethylation", 1.1,
+        "carboxyethylation", 1.2,
         [ModificationDatabase(cplmv4, "Carboxyethylation"), ModificationDatabase(dbptm, "Carboxyethylation")],
         ["K"]
     ),
     "carboxylation": ModificationType(
-        "carboxylation", 1.1,
+        "carboxylation", 1.2,
         [ModificationDatabase(cplmv4, "Carboxylation"), ModificationDatabase(dbptm, "Carboxylation")],
         ["K"]
     ),
     "carboxymethylation": ModificationType(
-        "carboxymethylation", 1.1, [ModificationDatabase(cplmv4, "Carboxymethylation")],
+        "carboxymethylation", 1.2, [ModificationDatabase(cplmv4, "Carboxymethylation")],
         ["K"]
     ),
     "cholesterol_ester": ModificationType(
-        "cholesterol_ester", 1.1,
+        "cholesterol_ester", 1.2,
         [ModificationDatabase(dbptm, "Cholesterol ester")],
         ["G"]
     ),
     "citrullination": ModificationType(
-        "citrullination", 1.1,
+        "citrullination", 1.2,
         [ModificationDatabase(dbptm, "Citrullination")],
         ["R"]
     ),
     "crotonylation": ModificationType(
-        "crotonylation", 1.1,
+        "crotonylation", 1.2,
         [ModificationDatabase(cplmv4, "Crotonylation"), ModificationDatabase(dbptm, "Crotonylation")],
         ["K"]
     ),
     "c-linked_glycosylation": ModificationType(
-        "c-linked_glycosylation", 1.1,
+        "c-linked_glycosylation", 1.2,
         [ModificationDatabase(dbptm, "C-linked Glycosylation")],
         ["W"]
     ),
     "deamidation": ModificationType(
-        "deamidation", 1.1,
+        "deamidation", 1.2,
         [ModificationDatabase(dbptm, "Deamidation")],
         ["N","Q"]
     ),
     "deamination": ModificationType(
-        "deamination", 1.1,
+        "deamination", 1.2,
         [ModificationDatabase(dbptm, "Deamination")],
         ["K"]
     ),
     "decanoylation": ModificationType(
-        "decanoylation", 1.1,
+        "decanoylation", 1.2,
         [ModificationDatabase(dbptm, "Decanoylation")],
         ["S","T"]
     ),
     "decarboxylation": ModificationType(
-        "decarboxylation", 1.1,
+        "decarboxylation", 1.2,
         [ModificationDatabase(dbptm, "Decarboxylation")],
         ["D","T"]
     ),
+    "dephosphorylation": ModificationType(
+        "dephosphorylation", 1.2,
+        [ModificationDatabase(dbptm, "Dephosphorylation")],
+        ["S","T","Y"]
+    ),
     "dietylphosphorylation": ModificationType(
-        "dietylphosphorylation", 1.1, [ModificationDatabase(cplmv4, "Dietylphosphorylation")],
+        "dietylphosphorylation", 1.2, [ModificationDatabase(cplmv4, "Dietylphosphorylation")],
         ["K"] #OK
     ),
+    "disulfide_bond": ModificationType(
+        "disulfide_bond", 1.2,
+        [ModificationDatabase(dbptm, "Disulfide bond")],
+        ["C"]
+    ),
     "d-glucuronoylation": ModificationType(
-        "d-glucuronoylation", 1.1,
+        "d-glucuronoylation", 1.2,
         [ModificationDatabase(dbptm, "D-glucuronoylation")],
         ["G"]
     ),
     "farnesylation": ModificationType(
-        "farnesylation", 1.1,
+        "farnesylation", 1.2,
         [ModificationDatabase(dbptm, "Farnesylation")],
         ["C"]
     ),
     "formation_of_an_isopeptide_bond": ModificationType(
-        "formation_of_an_isopeptide_bond", 1.1,
+        "formation_of_an_isopeptide_bond", 1.2,
         [ModificationDatabase(dbptm, "Formation of an isopeptide bond")],
         ["E","Q"]
     ),
     "formylation": ModificationType(
-        "formylation", 1.1,
+        "formylation", 1.2,
         [ModificationDatabase(cplmv4, "Formylation"), ModificationDatabase(dbptm, "Formylation")],
         ["G","K","M"]
     ),
     "gamma-carboxyglutamic_acid": ModificationType(
-        "gamma-carboxyglutamic_acid", 1.1,
+        "gamma-carboxyglutamic_acid", 1.2,
         [ModificationDatabase(dbptm, "Gamma-carboxyglutamic acid")],
         ["E"]
     ),
     "geranylgeranylation": ModificationType(
-        "geranylgeranylation", 1.1,
+        "geranylgeranylation", 1.2,
         [ModificationDatabase(dbptm, "Geranylgeranylation")],
         ["C"]
     ),
     "glutarylation": ModificationType(
-        "glutarylation", 1.1,
+        "glutarylation", 1.2,
         [ModificationDatabase(cplmv4, "Glutarylation"), ModificationDatabase(dbptm, "Glutarylation")],
         ["K"]
     ),
     "glutathionylation": ModificationType(
-        "glutathionylation", 1.1,
+        "glutathionylation", 1.2,
         [ModificationDatabase(dbptm, "Glutathionylation")],
         ["C"]
     ),
     "glycation": ModificationType(
-        "glycation", 1.1, [ModificationDatabase(cplmv4, "Glycation")],
+        "glycation", 1.2, [ModificationDatabase(cplmv4, "Glycation")],
         ["K"]
     ),
     "gpi-anchor": ModificationType(
-        "gpi-anchor", 1.1, [ModificationDatabase(dbptm, "GPI-anchor")],
+        "gpi-anchor", 1.2, [ModificationDatabase(dbptm, "GPI-anchor")],
         ["A","C","D","G","N","S","T"]
     ),
     "hmgylation": ModificationType(
-        "hmgylation", 1.1, [ModificationDatabase(cplmv4, "HMGylation")],
+        "hmgylation", 1.2, [ModificationDatabase(cplmv4, "HMGylation")],
         ["K"] #OK
     ),
     "hydroxyceramide_ester": ModificationType(
-        "hydroxyceramide_ester", 1.1, [ModificationDatabase(dbptm, "Hydroxyceramide ester")],
+        "hydroxyceramide_ester", 1.2, [ModificationDatabase(dbptm, "Hydroxyceramide ester")],
         ["Q"]
     ),
     "hydroxylation": ModificationType(
-        "hydroxylation", 1.1,
+        "hydroxylation", 1.2,
         [ModificationDatabase(cplmv4, "Hydroxylation"), ModificationDatabase(dbptm, "Hydroxylation")],
         ["C","D","E","F","H","I","K","L","N","P","R","S","T","V","W","Y"]
     ),
     "iodination": ModificationType(
-        "iodination", 1.1,
+        "iodination", 1.2,
         [ModificationDatabase(dbptm, "Iodination")],
         ["Y"]
     ),
     "lactoylation": ModificationType(
-        "lactoylation", 1.1,
+        "lactoylation", 1.2,
         [ModificationDatabase(dbptm, "Lactoylation")],
         ["K"]
     ),
     "lactylation": ModificationType(
-        "lactylation", 1.1,
+        "lactylation", 1.2,
         [ModificationDatabase(cplmv4, "Lactylation"), ModificationDatabase(dbptm, "Lactylation")],
         ["K"]
     ),
     "lipoylation": ModificationType(
-        "lipoylation", 1.1,
+        "lipoylation", 1.2,
         [ModificationDatabase(cplmv4, "Lipoylation"), ModificationDatabase(dbptm, "Lipoylation")],
         ["K"]
     ),
     "malonylation": ModificationType(
-        "malonylation", 1.1,
+        "malonylation", 1.2,
         [ModificationDatabase(cplmv4, "Malonylation"), ModificationDatabase(dbptm, "Malonylation")],
         ["K"]
     ),
     "methylation": ModificationType(
-        "methylation", 1.1,
+        "methylation", 1.2,
         [ModificationDatabase(cplmv4, "Methylation"), ModificationDatabase(dbptm, "Methylation")],
         ["A","C","D","E","F","G","H","I","K","L","M","N","P","Q","R","S","T","V","Y"]
     ),
     "mgcylation": ModificationType(
-        "mgcylation", 1.1, [ModificationDatabase(cplmv4, "MGcylation")],
+        "mgcylation", 1.2, [ModificationDatabase(cplmv4, "MGcylation")],
         ["K"]
     ),
     "mgylation": ModificationType(
-        "mgylation", 1.1, [ModificationDatabase(cplmv4, "MGylation")],
+        "mgylation", 1.2, [ModificationDatabase(cplmv4, "MGylation")],
         ["K"]
     ),
     "myristoylation": ModificationType(
-        "myristoylation", 1.1, [ModificationDatabase(dbptm, "Myristoylation")],
+        "myristoylation", 1.2, [ModificationDatabase(dbptm, "Myristoylation")],
         ["C","G","K"]
     ),
     "neddylation": ModificationType(
-        "neddylation", 1.1,
+        "neddylation", 1.2,
         [ModificationDatabase(cplmv4, "Neddylation"), ModificationDatabase(dbptm, "Neddylation")],
         ["K"]
     ),
     "nitration": ModificationType(
-        "nitration", 1.1, [ModificationDatabase(dbptm, "Nitration")],
+        "nitration", 1.2, [ModificationDatabase(dbptm, "Nitration")],
         ["Y"]
     ),
     "n-carbamoylation": ModificationType(
-        "n-carbamoylation", 1.1, [ModificationDatabase(dbptm, "N-carbamoylation")],
+        "n-carbamoylation", 1.2, [ModificationDatabase(dbptm, "N-carbamoylation")],
         ["A"]
     ),
     "n-linked_glycosylation": ModificationType(
-        "n-linked_glycosylation", 1.1,
+        "n-linked_glycosylation", 1.2,
         [ModificationDatabase(dbptm, "N-linked Glycosylation")],
         ["D","I","K","N","R","S","T","V","W"]
     ),
     "n-palmitoylation": ModificationType(
-        "n-palmitoylation", 1.1, [ModificationDatabase(dbptm, "N-palmitoylation")],
+        "n-palmitoylation", 1.2, [ModificationDatabase(dbptm, "N-palmitoylation")],
         ["C","G","K"]
     ),
     "octanoylation": ModificationType(
-        "octanoylation", 1.1,
+        "octanoylation", 1.2,
         [ModificationDatabase(dbptm, "Octanoylation")],
         ["S","T"]
     ),
     "oxidation": ModificationType(
-        "oxidation", 1.1,
+        "oxidation", 1.2,
         [ModificationDatabase(dbptm, "Oxidation")],
         ["C","L","M","S","W"]
     ),
     "o-linked_glycosylation": ModificationType(
-        "o-linked_glycosylation", 1.1,
+        "o-linked_glycosylation", 1.2,
         [ModificationDatabase(dbptm, "O-linked Glycosylation")],
         ["K","P","S","T","Y"]
     ),
     "o-palmitoleoylation": ModificationType(
-        "o-palmitoleoylation", 1.1,
+        "o-palmitoleoylation", 1.2,
         [ModificationDatabase(dbptm, "O-palmitoleoylation")],
         ["S"]
     ),
     "o-palmitoylation": ModificationType(
-        "o-palmitoylation", 1.1,
+        "o-palmitoylation", 1.2,
         [ModificationDatabase(dbptm, "O-palmitoylation")],
         ["S","T"]
     ),
     "phosphatidylethanolamine_amidation": ModificationType(
-        "phosphatidylethanolamine_amidation", 1.1, [ModificationDatabase(dbptm, "Phosphatidylethanolamine amidation")],
+        "phosphatidylethanolamine_amidation", 1.2, [ModificationDatabase(dbptm, "Phosphatidylethanolamine amidation")],
         ["G"]
     ),
     "phosphoglycerylation": ModificationType(
-        "phosphoglycerylation", 1.1,
+        "phosphoglycerylation", 1.2,
         [ModificationDatabase(cplmv4, "Phosphoglycerylation")],
         ["K"]
     ),
     "phosphorylation": ModificationType(
-        "phosphorylation", 1.1,
+        "phosphorylation", 1.2,
         [ModificationDatabase(dbptm, "Phosphorylation")],
         ["A","C","D","E","F","G","H","I","K","L","N","P","Q","R","S","T","V","W","Y"]
     ),
     "propionylation": ModificationType(
-        "propionylation", 1.1,
+        "propionylation", 1.2,
         [ModificationDatabase(cplmv4, "Propionylation"), ModificationDatabase(dbptm, "Propionylation")],
         ["K"]
     ),
     "pupylation": ModificationType(
-        "pupylation", 1.1, [ModificationDatabase(cplmv4, "Pupylation")],
+        "pupylation", 1.2, [ModificationDatabase(cplmv4, "Pupylation")],
         ["K"]
     ),
     "pyrrolidone_carboxylic_acid": ModificationType(
-        "pyrrolidone_carboxylic_acid", 1.1, [ModificationDatabase(dbptm, "Pyrrolidone carboxylic acid")],
+        "pyrrolidone_carboxylic_acid", 1.2, [ModificationDatabase(dbptm, "Pyrrolidone carboxylic acid")],
         ["E","Q"]
     ),
     "pyrrolylation": ModificationType(
-        "pyrrolylation", 1.1, [ModificationDatabase(dbptm, "Pyrrolylation")],
+        "pyrrolylation", 1.2, [ModificationDatabase(dbptm, "Pyrrolylation")],
         ["C"]
     ),
     "pyruvate": ModificationType(
-        "pyruvate", 1.1, [ModificationDatabase(dbptm, "Pyruvate")],
+        "pyruvate", 1.2, [ModificationDatabase(dbptm, "Pyruvate")],
         ["C","S"]
     ),
     "serotonylation" : ModificationType(
-        "serotonylation", 1.1,
+        "serotonylation", 1.2,
         [ModificationDatabase(dbptm, "Serotonylation")],
         ["Q"]
     ),
     "stearoylation" : ModificationType(
-        "stearoylation", 1.1,
+        "stearoylation", 1.2,
         [ModificationDatabase(dbptm, "Stearoylation")],
         ["C"]
     ),
     "succinylation": ModificationType(
-        "succinylation", 1.1,
+        "succinylation", 1.2,
         [ModificationDatabase(cplmv4, "Succinylation"), ModificationDatabase(dbptm, "Succinylation")],
         ["C","K","W"]
     ),
     "sulfation" : ModificationType(
-        "sulfation", 1.1,
+        "sulfation", 1.2,
         [ModificationDatabase(dbptm, "Sulfation")],
         ["C","S","T","Y"]
     ),
     "sulfhydration" : ModificationType(
-        "sulfhydration", 1.1,
+        "sulfhydration", 1.2,
         [ModificationDatabase(dbptm, "Sulfhydration")],
         ["C"]
     ),
     "sulfoxidation" : ModificationType(
-        "sulfoxidation", 1.1,
+        "sulfoxidation", 1.2,
         [ModificationDatabase(dbptm, "Sulfoxidation")],
         ["M"]
     ),
     "sumoylation": ModificationType(
-        "sumoylation", 1.1,
+        "sumoylation", 1.2,
         [ModificationDatabase(cplmv4, "Sumoylation"), ModificationDatabase(dbptm, "Sumoylation")],
         ["K"]
     ),
     "s-archaeol" : ModificationType(
-        "s-archaeol", 1.1,
+        "s-archaeol", 1.2,
         [ModificationDatabase(dbptm, "S-archaeol")],
         ["C"]
     ),
     "s-carbamoylation" : ModificationType(
-        "s-carbamoylation", 1.1,
+        "s-carbamoylation", 1.2,
         [ModificationDatabase(dbptm, "S-carbamoylation")],
         ["C"]
     ),
     "s-cyanation" : ModificationType(
-        "s-cyanation", 1.1,
+        "s-cyanation", 1.2,
         [ModificationDatabase(dbptm, "S-Cyanation")],
         ["C"]
     ),
     "s-cysteinylation" : ModificationType(
-        "s-cysteinylation", 1.1,
+        "s-cysteinylation", 1.2,
         [ModificationDatabase(dbptm, "S-cysteinylation")],
         ["C"]
     ),
     "s-diacylglycerol" : ModificationType(
-        "s-diacylglycerol", 1.1,
+        "s-diacylglycerol", 1.2,
         [ModificationDatabase(dbptm, "S-diacylglycerol")],
         ["C"]
     ),
     "s-linked_glycosylation": ModificationType(
-        "s-linked_glycosylation", 1.1,
+        "s-linked_glycosylation", 1.2,
         [ModificationDatabase(dbptm, "S-linked Glycosylation")],
         ["C"]
     ),
     "s-nitrosylation" : ModificationType(
-        "s-nitrosylation", 1.1,
+        "s-nitrosylation", 1.2,
         [ModificationDatabase(dbptm, "S-nitrosylation")],
         ["C"]
     ),
     "s-palmitoylation" : ModificationType(
-        "s-palmitoylation", 1.1,
+        "s-palmitoylation", 1.2,
         [ModificationDatabase(dbptm, "S-palmitoylation")],
         ["C"]
     ),
     "thiocarboxylation" : ModificationType(
-        "thiocarboxylation", 1.1,
+        "thiocarboxylation", 1.2,
         [ModificationDatabase(dbptm, "Thiocarboxylation")],
         ["G"]
     ),
     "ubiquitination": ModificationType(
-        "ubiquitination", 1.1,
+        "ubiquitination", 1.2,
         [ModificationDatabase(cplmv4, "Ubiquitination"), ModificationDatabase(dbptm, "Ubiquitination")],
         ["C","K","R","S"]
     ),
     "umpylation" : ModificationType(
-        "umpylation", 1.1,
+        "umpylation", 1.2,
         [ModificationDatabase(dbptm, "UMPylation")],
         ["S","T","Y"]
     ),
     "2-hydroxyisobutyrylation": ModificationType(
-        "2-hydroxyisobutyrylation", 1.1, [ModificationDatabase(cplmv4, "2-Hydroxyisobutyrylation")],
+        "2-hydroxyisobutyrylation", 1.2, [ModificationDatabase(cplmv4, "2-Hydroxyisobutyrylation")],
         ["K"]
     ),
     }
 
 
 def update_db_for_modifications(list_of_mods_to_check: List[str]):
     """
```

### Comparing `flams-1.1.3/src/flams/display.py` & `flams-1.1.4/src/flams/display.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/flams.py` & `flams-1.1.4/src/flams/flams.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/input.py` & `flams-1.1.4/src/flams/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,15 +694,15 @@
             modifications.extend(['phosphorylation','acetylation','pyruvate','gpi-anchor',
             'adp-ribosylation','amidation','hydroxylation','blocked_amino_end',
             'oxidation','methylation','sulfation','ubiquitination','carbamidation',
             'farnesylation','geranylgeranylation','glutathionylation','myristoylation',
             'n-palmitoylation','pyrrolylation','s-archaeol','s-carbamoylation',
             's-cyanation','s-cysteinylation','s-diacylglycerol','s-linked_glycosylation',
             's-nitrosylation','s-palmitoylation','stearoylation',
-            'succinylation','sulfhydration'])
+            'succinylation','sulfhydration','disulfide_bond'])
         if 'D-All' in modifications:
             modifications.remove('D-All')
             modifications.extend(['phosphorylation','acetylation','gpi-anchor',
             'adp-ribosylation','amidation','hydroxylation','blocked_amino_end',
             'methylation','n-linked_glycosylation','decarboxylation'])
         if 'E-All' in modifications:
             modifications.remove('E-All')
@@ -770,28 +770,30 @@
             'n-linked_glycosylation','acetylation','ubiquitination'])
         if 'S-All' in modifications:
             modifications.remove('S-All')
             modifications.extend(['phosphorylation','decanoylation','octanoylation',
             'o-palmitoylation','umpylation','ampylation','blocked_amino_end',
             'o-palmitoleoylation','adp-ribosylation','gpi-anchor','sulfation',
             'oxidation','pyruvate','amidation','hydroxylation','o-linked_glycosylation',
-            'methylation','n-linked_glycosylation','acetylation','ubiquitination'])
+            'methylation','n-linked_glycosylation','acetylation','ubiquitination',
+            'dephosphorylation'])
         if 'T-All' in modifications:
             modifications.remove('T-All')
             modifications.extend(['phosphorylation','decarboxylation','decanoylation',
             'octanoylation','o-palmitoylation','umpylation','ampylation',
             'blocked_amino_end','gpi-anchor','sulfation',
             'amidation','hydroxylation','o-linked_glycosylation',
-            'methylation','n-linked_glycosylation','acetylation'])
+            'methylation','n-linked_glycosylation','acetylation', 'dephosphorylation'])
         if 'V-All' in modifications:
             modifications.remove('V-All')
             modifications.extend(['phosphorylation','blocked_amino_end','amidation',
             'hydroxylation','methylation','n-linked_glycosylation','acetylation'])
         if 'W-All' in modifications:
             modifications.remove('W-All')
             modifications.extend(['phosphorylation','c-linked_glycosylation','oxidation',
             'amidation','hydroxylation','succinylation','n-linked_glycosylation'])
         if 'Y-All' in modifications:
             modifications.remove('Y-All')
             modifications.extend(['phosphorylation','umpylation','iodination',
             'ampylation','adp-ribosylation','sulfation','nitration','amidation',
-            'hydroxylation','o-linked_glycosylation','methylation','acetylation'])
+            'hydroxylation','o-linked_glycosylation','methylation','acetylation',
+            'dephosphorylation'])
```

### Comparing `flams-1.1.3/src/flams/run_blast.py` & `flams-1.1.4/src/flams/run_blast.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams/utils.py` & `flams-1.1.4/src/flams/utils.py`

 * *Files identical despite different names*

### Comparing `flams-1.1.3/src/flams.egg-info/PKG-INFO` & `flams-1.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: flams
-Version: 1.1.3
-Summary: Find Lysine Acylations & other Modification Sites
-Project-URL: repository, https://github.com/hannelorelongin/FLAMS
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: appdirs==1.4.4
-Requires-Dist: biopython==1.81
-Requires-Dist: certifi==2023.5.7
-Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: idna==3.4
-Requires-Dist: numpy==1.24.3
-Requires-Dist: pandas==2.1.2
-Requires-Dist: python-dateutil==2.8.2
-Requires-Dist: pytz==2023.3.post1
-Requires-Dist: requests==2.29.0
-Requires-Dist: six==1.16.0
-Requires-Dist: tzdata==2023.3
-Requires-Dist: urllib3==1.26.18
-
 # FLAMS: Find Lysine Acylations & other Modification Sites
 
 A bioinformatics tool to analyze the conservation of post-translational modifications (PTMs), by means of a position-based search against the Compendium of Protein Lysine Modifications (CPLM database) v.4 and the experimental PTM sites in dbPTM. FLAMS is available as command-line tool and as a [web service](https://www.biw.kuleuven.be/m2s/cmpg/research/CSB/tools/flams/).
 
 # Table of contents
 
 1.  [Introduction](#introduction)
@@ -98,29 +76,29 @@
 
 Optional arguments:
 * `errorRange` is an number of positions before and after `position` to also search for modifications. [default: 0]
 * `outputFilePath` is the path to where the result will be saved (in a .tsv file format). [default: out.tsv] If FLAMS is run with --batch, the specified -o/--output is used as preposition, followed by '\_$UniProtID\_$position.tsv'. [default: '']
 * `dataDir` is the path to the directory where intermediate files (the UniProt sequence files) are stored. [default: $PWD/data]
 * `threadsBLAST` is a BLAST parameter, allows you to speed up the search by multithreading. [default: 1]
 * `evalueBLAST` is a BLAST parameter, allows you to filter out low quality BLAST hits. [default: 0.01]
-* `modification` is a space-seperated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
+* `modification` is a space-separated list of modifications (all lower case) to search for at the given position. Possible values are any (combinations) of the CPLM and dbPTM modifications. We also provide aggregated combinations for each amino acid ($AA-All), and the CPLM combinations. For a full list of all supported PTMs, and how they are named, see the [Supported PTM types](#supported-ptm-types) section of the README. In general, PTMs are written all lowercase, and spaces within a PTM name are replaced by underscores. [default: K-All]
 
 ### Example use case
 
 We provide two example use cases for FLAMS:
 
 With the following command, you search whether the TatA (UniProt ID: A0A916NWA0) acetylation on K66 in *Dehalococcoide mccartyi* strain CBDB1, as described by [Greiner-Haas (2021)](https://doi.org/10.3390/microorganisms9020365), had been previously detected.
 
 `FLAMS --in A0A916NWA0.fa -p 66 -m acetylation -o tatA.tsv`
 
 With the following command, you search whether the *Mycobabcterium smegmatis*' FadD2 (UniProt ID: A0QQ22) K537 is known to carry any modifications of the 'acylations' category, similar to what was reported by [Xu (2020)](https://doi.org/10.1128/mSystems.00424-19).
 
 `FLAMS --id A0QQ22 -p 537 -m CPLM-Acylations -o FadD2.tsv`
 
-You can find the example input and output data in the folder `test_data`.
+You can find the example input and output data in the folder `test_data`. The output data is organized in folders reflecting the FLAMS version used to generate it, as the output can vary depending on the exact FLAMS version (due to FLAMS database updates).
 
 For more example use cases, see the Supplementary information of the paper.
 
 ## Output
 
 The output file is a .tsv containing one row per modification that matched the query, i.e., a modification aligning (within the user-specified range) to the query position, in a protein similar to the query protein. In case of batch jobs (ran with --batch), one output file per query (= a single line in the batch job file) will be generated.
 
@@ -145,20 +123,21 @@
 
 ## Supported PTMs
 
 ### Supported PTM databases
 
 FLAMS updates its search databases regularly. To get an overview of the supported databases, see the table below.
 
-|FLAMS version|CPLM version|dbPTM version|database available for download|
-|:----|:----|:----|:----|
-|v1.1|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|
-|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|
+|FLAMS version|CPLM version|dbPTM version|database available for download|UniProt release|
+|:----|:----|:----|:----|:----|
+|v1.1.4|v4|2024_April|[yes](https://doi.org/10.5281/zenodo.10958721)|2024_02|
+|v1.1.0-3|v4|2023_November|[yes](https://doi.org/10.5281/zenodo.10171879)|2023_05|
+|v1.0|v4| |[yes](https://cplm.biocuckoo.cn/Download.php)|NA|
 
-Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). Moreover, proteins that carry a UniProt ID that was obsolete or missing at the time of database creation are also not included in the database.
+Please note that only part of dbPTM is integrated into FLAMS, namely the PTM sites with experimental evidence, as found [here](https://awi.cuhk.edu.cn/dbPTM/download.php). As dbPTM does not store complete protein sequences, these are fetched during database creation based on UniProt identifiers reported in dbPTM and the UniProt release available at the time of database creation. As a consequence, FLAMS database updates can change the content of the PTM databases, beyond the simple addition of new dbPTM and/or CPLM entries, reflecting changes in UniProt. The most common UniProt changes affecting FLAMS databases are removed UniProt entries (leading to the removal of PTM entries on the affected protein in our database) and sequence updates. We are aware of this issue, impacting the completeness and interpretation of FLAMS' results, and will consider solutions in future FLAMS releases.
 
 Instructions on how to download the CPLM and dbPTM database yourself are in [section 'Local CPLM and dbPTM install'](#local-cplm-and-dbptm-install). This is not recommended, as it takes multiple hours to generate some databases.
 
 ### Supported PTM types
 
 FLAMS allows searches for all PTM types included in CPLM, and for those with experimental evidence in dbPTM. An overview of the PTM types, how to call them in FLAMS, how they are called in CPLM and/or dbPTM, and on which amino acid they can be found is given in the table below. This table can also be found as a tab seperated file named FLAMS_supported_ptms_v11.txt .
 
@@ -181,15 +160,17 @@
 |citrullination| |Citrullination| | | | | | | |  | | | | | | |X| | | | | | | | | |
 |crotonylation|Crotonylation|Crotonylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
 |c-linked_glycosylation| |C-linked Glycosylation| | | | | | | | | | | | | | | | | | |X| | | | | |
 |deamidation| |Deamidation| | | | | | | | | | | |X| |X| | | | | | | | | | |
 |deamination| |Deamination| | | | | | | | |X| | | | | | | | | | | | | | | |
 |decanoylation| |Decanoylation| | | | | | | | | | | | | | | |X|X| | | | | | | |
 |decarboxylation| |Decarboxylation| | |X| | | | | | | | | | | | | |X| | | | | | | |
+|dephosphorylation| |Dephosphorylation| | | | | | | | | | | | | | | |X|X| | |X| | | | |
 |dietylphosphorylation|Dietylphosphorylation| | | | | | | | | |X| | | | | | | | | | | | | |X|X|
+|disulfide_bond| |Disulfide bond| |X| | | | | | | | | | | | | | | | | | | | | | |
 |d-glucuronylation| |D-glucuronoylation| | | | | |X| | | | | | | | | | | | | | | | | | |
 |farnesylation| |Farnesylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |formation_of_an_isopeptide_bond| |Formation of an isopeptide bond| | | |X| | | | | | | | | |X| | | | | | | | | | |
 |formylation|Formylation|Formylation| | | | | |X| | |X| |X| | | | | | | | | |X| | |X|
 |gamma-carboxyglutamic_acid| |Gamma-carboxyglutamic acid| | | |X| | | | | | | | | | | | | | | | | | | | |
 |geranylgeranylation| |Geranylgeranylation| |X| | | | | | | | | | | | | | | | | | | | | | |
 |glutarylation|Glutarylation|Glutarylation| | | | | | | | |X| | | | | | | | | | | |X| | |X|
@@ -283,23 +264,25 @@
       ),`
 
     - comment out lines 503-508 (function `_generate_blastdb_if_not_up_to_date` - the try/except _get_fasta_from_zenodo)
     - uncomment line 512 (function `_generate_blastdb_if_not_up_to_date` - the _get_fasta_for_blast)
 
 3. Install your adapted FLAMS version locally:
 
-  `python -m pip install ./PathToLocalFLAMS`
+    `python -m pip install ./PathToLocalFLAMS`
 
 ## Contact
 
 Laboratory of Computational Systems Biology, KU Leuven.
 
 ## References
 
-If you use FLAMS in your work, please cite us.
+If you use FLAMS in your work, please cite:
+
+Longin, H. *et al* (2024) "FLAMS: Find Lysine Acylations and other Modification Sites." Bioinformatics. 40(1):btae005.
 
 In addition, FLAMS relies on third-party software & databases:
 
 Altschul, S.F. *et al* (1990) "Basic local alignment search tool." J. Mol. Biol. 215:403-410.
 
 Li, Z. *et al* (2022) "dbPTM in 2022: an updated database for exploring regulatory networks and functional associations of protein post-translational modifications." Nucleic Acids Research. 50:D471–D479.
```

