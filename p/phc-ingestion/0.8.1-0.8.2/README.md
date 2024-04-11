# Comparing `tmp/phc-ingestion-0.8.1.tar.gz` & `tmp/phc-ingestion-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.8.1.tar", last modified: Tue Apr  9 10:46:09 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.2.tar", last modified: Thu Apr 11 21:19:02 2024, max compression
```

## Comparing `phc-ingestion-0.8.1.tar` & `phc-ingestion-0.8.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0       16 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      507 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      770 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0    12312 2024-04-09 10:45:46.802468 phc-ingestion-0.8.1/ingestion/caris/util/ihc.py
--rw-r--r--   0        0        0      555 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4706 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/json.py
--rw-r--r--   0        0        0     9497 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     2051 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/specimen_details.py
--rw-r--r--   0        0        0     4363 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0     1027 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tmb.py
--rw-r--r--   0        0        0     1595 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3298 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5451 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0       68 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-09 10:45:46.806468 phc-ingestion-0.8.1/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1010 2024-04-09 10:45:46.810468 phc-ingestion-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4441 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      770 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9536 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4599 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0      372 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tests.py
+-rw-r--r--   0        0        0     1027 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3440 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5451 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0       68 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1010 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.2/PKG-INFO
```

### Comparing `phc-ingestion-0.8.1/ingestion/caris/process.py` & `phc-ingestion-0.8.2/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.2/ingestion/caris/util/cnv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from logging import Logger
+
 from ingestion.shared_util.gene_to_coords import gene_to_coords
+from ingestion.caris.util.tests import safely_extract_tests_from_json_data
 
 
 def extract_cnv(prefix, data, log: Logger):
     # Get all CNV calls into a csv
     caris_lo_keywords = {"intermediate": "gain", "amplified": "amplification", "deleted": "loss"}
-    tests = []
-    for test in data["tests"]:
+    extracted_tests = safely_extract_tests_from_json_data(data)
+    copy_number_variant_tests = []
+    for test in extracted_tests:
         # We don't want to bring in "not detected" or wild type results
         test_name = test["testName"]
         if ("CNA" in test_name or "CND" in test_name) and "testResults" in test.keys():
             test = test["testResults"]
             if isinstance(test, dict):
                 test = [test]
             for cna in test:
@@ -22,15 +25,15 @@
                         "indeterminate",
                         "wild type",
                     ]:
                         status = results["result"].lower()
                         if status in caris_lo_keywords.keys():
                             # We only accept 2 of their results and they have to match our PHC keywords to be searchable
                             results["result"] = caris_lo_keywords[status]
-                            tests.append(results)
+                            copy_number_variant_tests.append(results)
                     elif (
                         "Exome CNA Panel - Additional Genes" in test_name
                         and "result" in results.keys()
                         and "copyNumber" in results.keys()
                     ):
                         status = results["result"].lower()
 
@@ -44,25 +47,25 @@
                             elif copy_number >= 6:
                                 cn_status = "amplification"
                             elif copy_number < 1.3:
                                 cn_status = "loss"
                             else:
                                 continue
                             results["result"] = cn_status
-                            tests.append(results)
+                            copy_number_variant_tests.append(results)
 
-    if not tests:
+    if not copy_number_variant_tests:
         return None
 
     # Save our results
     with open(f"{prefix}.copynumber.csv", "w") as f:
         f.write(
             "sample_id,gene,copy_number,status,attributes,chromosome,start_position,end_position,interpretation\n"
         )
-        for alt in tests:
+        for alt in copy_number_variant_tests:
             if "genomicCoordinates" in alt.keys():
                 chrom = alt["genomicCoordinates"].split(":")[1]
                 coords = alt["genomicCoordinates"].split(":")[2].split("-")
             else:
                 chrom, coords = gene_to_coords("GRCh37", alt["gene"])
 
             # Get pathogenic result
```

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.2/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.2/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/ihc.py` & `phc-ingestion-0.8.2/ingestion/caris/util/ihc.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.2/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/json.py` & `phc-ingestion-0.8.2/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/metadata.py` & `phc-ingestion-0.8.2/ingestion/caris/util/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from logging import Logger
 
 from ingestion.caris.util.hla import extract_hla_result_from_test_result
 from ingestion.caris.util.ihc import get_ihc_results
 from ingestion.caris.util.specimen_details import extract_and_parse_specimen_details
+from ingestion.caris.util.tests import safely_extract_tests_from_json_data
 from ingestion.caris.util.tmb import parse_tumor_mutation_burden
 
 MSI_MAPPINGS = {
     "low": "low",
     "stable": "stable",
     "high": "high",
     "indeterminate": "indeterminate",
@@ -148,20 +149,18 @@
     # Ensure no null entries
     metadata["patientInfo"] = {k: v for k, v in patientInfo.items() if v}
     metadata.update({"name": "Caris", "reference": "GRCh37"})
     metadata["hlaResults"] = []
 
     # Now find the test information
 
-    tests = data["tests"]
+    tests = safely_extract_tests_from_json_data(data)
 
     # if not sufficient quantity we won't have test results
     if test_details["reportType"] != "QNS":
-        if isinstance(tests, dict):
-            tests = [tests]
         for test in tests:
             if not is_valid_test_entry(test):
                 continue
             # Sometimes, if there is only a single test result,
             # Caris will set it as a dict instead of a list
             test_results = (
                 [test["testResults"]]
```

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/specimen_details.py` & `phc-ingestion-0.8.2/ingestion/caris/util/specimen_details.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.2/ingestion/caris/util/structural.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pandas as pd
 from logging import Logger
 
+from ingestion.caris.util.tests import safely_extract_tests_from_json_data
 from ingestion.caris.util.interpretation import calculate_interpretation
 from ingestion.caris.util.detect_genome_ref import detect_caris_gr
 
 
 def extract_structural(prefix, data, log: Logger):
     log.info("Extracting fusion variants from json")
-    tests = []
-    for test in data["tests"]:
+    extracted_tests = safely_extract_tests_from_json_data(data)
+    structural_variant_tests = []
+    for test in extracted_tests:
         if (
             test["platformTechnology"] in ["Transcriptome", "Hybrid Transcriptome"]
             and "testResults" in test.keys()
         ):
             for test_result in test["testResults"]:
                 this_result = test_result["translocation"]
 
@@ -28,19 +30,19 @@
                 #     - Pathogenic Fusion
                 if this_result["result_group"].lower() not in [
                     "normal",
                     "no result",
                     "indeterminate",
                     "wild type",
                 ]:
-                    tests.append(this_result)
-    if not tests:
+                    structural_variant_tests.append(this_result)
+    if not structural_variant_tests:
         return None
 
-    df = pd.DataFrame(tests)
+    df = pd.DataFrame(structural_variant_tests)
 
     def split_coords(x):
         return x.strip(":+").replace("+/", "").strip(":-").replace("-/", "")
 
     df["genomicBreakpoint"] = df["genomicBreakpoint"].apply(split_coords)
 
     df[["chromosome1", "start_position1", "chromosome2", "start_position2"]] = df[
@@ -100,14 +102,14 @@
             "in_frame",
             "attributes",
         ]
     ]
 
     df_out.to_csv(f"{prefix}.structural.csv", na_rep="N/A", index=False)
 
-    genome_reference = detect_caris_gr(tests, "structural", log)
+    genome_reference = detect_caris_gr(structural_variant_tests, "structural", log)
     return {
         "fileName": f".lifeomic/caris/{prefix}/{prefix}.structural.csv",
         "sequenceType": "somatic",
         "type": "structuralVariant",
         "reference": genome_reference,
     }
```

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/tmb.py` & `phc-ingestion-0.8.2/ingestion/caris/util/tmb.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.2/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.2/ingestion/caris/util/vcf.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import subprocess
 import sys
 import zipfile
 
 from logging import Logger
 
+from ingestion.caris.util.tests import safely_extract_tests_from_json_data
 from ingestion.vcf_standardization.standardize import standardize_vcf
 
 
 # This is done in next step, we are just adding to yaml
 def extract_sv(prefix, include_somatic: bool, include_germline: bool):
     vcfs = []
 
@@ -41,15 +42,17 @@
 
     return vcfs
 
 
 def get_vendsig_dict(json_data, log: Logger):
     # Return a dicitionary of {'chr:star_pos:ref:alt' : 'vendsig'}
     vendsig_dict = {"vendor": "caris"}
-    for test in json_data["tests"]:
+    extracted_tests = safely_extract_tests_from_json_data(json_data)
+
+    for test in extracted_tests:
         results = [
             result
             for result in test.get("testResults", {})
             if isinstance(result, dict) and "genomicAlteration" in result.keys()
         ]
         for result in results:
             if "alterationDetails" in result["genomicAlteration"].keys():
```

### Comparing `phc-ingestion-0.8.1/ingestion/foundation/process.py` & `phc-ingestion-0.8.2/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.2/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.2/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.2/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.2/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/generic/process.py` & `phc-ingestion-0.8.2/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/generic/utils.py` & `phc-ingestion-0.8.2/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/process.py` & `phc-ingestion-0.8.2/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.2/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.2/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.2/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.2/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.8.2/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.2/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.2/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.2/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.2/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.2/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.2/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.1/pyproject.toml` & `phc-ingestion-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.8.1"
+version = "0.8.2"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

