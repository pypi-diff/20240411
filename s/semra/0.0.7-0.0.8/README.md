# Comparing `tmp/semra-0.0.7.tar.gz` & `tmp/semra-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "semra-0.0.8.tar", last modified: Thu Apr 11 14:45:18 2024, max compression
```

## Comparing `semra-0.0.7.tar` & `semra-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,120 @@
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 semra-0.0.7/tox.ini
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 semra-0.0.7/.github/workflows/tests.yml
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 semra-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 semra-0.0.7/.idea/semra.iml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 semra-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0   419828 2020-02-02 00:00:00.000000 semra-0.0.7/docs/img/logo.png
--rw-r--r--   0        0        0    10076 2020-02-02 00:00:00.000000 semra-0.0.7/notebooks/Inference Example.ipynb
--rw-r--r--   0        0        0    72962 2020-02-02 00:00:00.000000 semra-0.0.7/notebooks/umls-inference-analysis.ipynb
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 semra-0.0.7/scripts/cancer_cell_reproduction.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 semra-0.0.7/scripts/gilda_reprocess.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/__about__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/__init__.py
--rw-r--r--   0        0        0    20900 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/api.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/client.py
--rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/database.py
--rw-r--r--   0        0        0     5211 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/gilda_utils.py
--rw-r--r--   0        0        0    23833 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/io.py
--rw-r--r--   0        0        0    14105 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/pipeline.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/rules.py
--rw-r--r--   0        0        0     9203 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/struct.py
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/wsgi.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/__init__.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/biopragmatics.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/chembl.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/clo.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/famplex.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/gilda.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/intact.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/ncit.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/sources/pubchem.py
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/templates/base.html
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/templates/concept.html
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/templates/home.html
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/templates/mapping.html
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 semra-0.0.7/src/semra/templates/mapping_set.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semra-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 semra-0.0.7/tests/test_api.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 semra-0.0.7/tests/test_pipeline.py
--rw-r--r--   0        0        0    16420 2020-02-02 00:00:00.000000 semra-0.0.7/.gitignore
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 semra-0.0.7/README.md
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 semra-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 semra-0.0.7/PKG-INFO
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.737529 semra-0.0.8/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2024-03-19 12:30:21.000000 semra-0.0.8/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      430 2024-03-21 09:11:47.000000 semra-0.0.8/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-11 14:45:18.737444 semra-0.0.8/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6983 2024-03-19 12:30:21.000000 semra-0.0.8/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.710554 semra-0.0.8/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.713943 semra-0.0.8/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.724916 semra-0.0.8/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.assemble_evidences.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.assert_projection.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.count_source_target.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.deduplicate_evidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_many_to_many.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      127 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_minimum_confidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.filter_self_matches.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.flip.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.from_digraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       79 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_many_to_many.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 16:59:05.000000 semra-0.0.8/docs/source/api/semra.api.get_priority_reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_test_evidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.get_test_reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_chains.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_dbxref_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      139 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_mutual_dbxref_mutations.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.infer_reversible.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_object_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       91 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      115 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.keep_subject_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.print_source_target_counts.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.prioritize.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.project.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       88 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.project_dict.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.str_source_target_counts.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.summarize_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.tabulate_index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.to_digraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-04-08 07:29:19.000000 semra-0.0.8/docs/source/api/semra.api.to_multidigraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.unindex.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.api.validate_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Configuration.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      391 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Input.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      409 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.Mutation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      129 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.get_mappings_from_config.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      105 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.get_raw_mappings.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       78 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.pipeline.process.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      898 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.Mapping.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      624 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.MappingSet.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      894 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.ReasonedEvidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      736 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.SimpleEvidence.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       67 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.line.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       85 2024-03-19 13:29:23.000000 semra-0.0.8/docs/source/api/semra.struct.triple_key.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      206 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7337 2024-04-11 14:45:18.000000 semra-0.0.8/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      295 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      498 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)   419828 2024-03-19 12:30:21.000000 semra-0.0.8/docs/source/logo.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)      150 2024-03-20 14:12:09.000000 semra-0.0.8/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      386 2024-03-19 12:31:11.000000 semra-0.0.8/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2750 2024-04-11 14:45:18.737923 semra-0.0.8/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.710778 semra-0.0.8/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.728981 semra-0.0.8/src/semra/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      792 2024-03-19 17:14:37.000000 semra-0.0.8/src/semra/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      322 2024-03-19 12:30:21.000000 semra-0.0.8/src/semra/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    49080 2024-04-10 11:07:02.000000 semra-0.0.8/src/semra/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      854 2024-03-19 12:30:21.000000 semra-0.0.8/src/semra/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    14620 2024-04-09 15:51:10.000000 semra-0.0.8/src/semra/client.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4832 2024-03-20 13:27:01.000000 semra-0.0.8/src/semra/database.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5340 2024-03-20 13:58:32.000000 semra-0.0.8/src/semra/gilda_utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    30750 2024-04-11 14:38:39.000000 semra-0.0.8/src/semra/io.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.731830 semra-0.0.8/src/semra/landscape/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       26 2024-04-10 09:49:05.000000 semra-0.0.8/src/semra/landscape/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      720 2024-04-11 12:30:31.000000 semra-0.0.8/src/semra/landscape/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2395 2024-04-10 09:49:05.000000 semra-0.0.8/src/semra/landscape/anatomy.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4441 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/cells.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2218 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/complexes.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3277 2024-04-10 11:11:49.000000 semra-0.0.8/src/semra/landscape/diseases.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2651 2024-04-10 22:44:43.000000 semra-0.0.8/src/semra/landscape/genes.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    26871 2024-04-10 12:51:01.000000 semra-0.0.8/src/semra/landscape/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    16944 2024-04-09 15:51:11.000000 semra-0.0.8/src/semra/pipeline.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        0 2024-03-20 12:33:07.000000 semra-0.0.8/src/semra/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1968 2024-03-26 15:25:38.000000 semra-0.0.8/src/semra/rules.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.734430 semra-0.0.8/src/semra/sources/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2904 2024-04-03 14:15:40.000000 semra-0.0.8/src/semra/sources/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3104 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/biopragmatics.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2342 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/chembl.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6892 2024-03-28 13:16:11.000000 semra-0.0.8/src/semra/sources/clo.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1523 2024-04-03 14:15:40.000000 semra-0.0.8/src/semra/sources/famplex.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1938 2024-04-03 14:25:30.000000 semra-0.0.8/src/semra/sources/gilda.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1773 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/intact.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4162 2024-03-20 13:52:23.000000 semra-0.0.8/src/semra/sources/ncit.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1410 2024-04-02 14:00:35.000000 semra-0.0.8/src/semra/sources/omim.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1946 2024-03-19 12:23:21.000000 semra-0.0.8/src/semra/sources/pubchem.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1741 2024-04-04 08:38:28.000000 semra-0.0.8/src/semra/sources/wikidata.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11079 2024-03-20 14:11:18.000000 semra-0.0.8/src/semra/struct.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.735494 semra-0.0.8/src/semra/templates/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1471 2024-01-30 20:05:30.000000 semra-0.0.8/src/semra/templates/base.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4204 2024-03-26 15:11:46.000000 semra-0.0.8/src/semra/templates/concept.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4662 2024-04-08 21:10:21.000000 semra-0.0.8/src/semra/templates/home.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2037 2024-03-26 15:35:48.000000 semra-0.0.8/src/semra/templates/mapping.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)      993 2024-03-26 16:16:16.000000 semra-0.0.8/src/semra/templates/mapping_set.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)      799 2024-04-08 21:07:18.000000 semra-0.0.8/src/semra/templates/utils.html
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1027 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra/version.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7486 2024-04-09 15:51:10.000000 semra-0.0.8/src/semra/wsgi.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.736748 semra-0.0.8/src/semra.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9392 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3742 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       41 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-19 13:13:03.000000 semra-0.0.8/src/semra.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      277 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        6 2024-04-11 14:45:18.000000 semra-0.0.8/src/semra.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-11 14:45:18.736477 semra-0.0.8/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       23 2024-03-20 13:36:03.000000 semra-0.0.8/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    18468 2024-04-10 09:49:23.000000 semra-0.0.8/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      696 2024-03-20 14:28:21.000000 semra-0.0.8/tests/test_io.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2886 2024-03-20 13:54:27.000000 semra-0.0.8/tests/test_pipeline.py
```

### Comparing `semra-0.0.7/docs/img/logo.png` & `semra-0.0.8/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/scripts/cancer_cell_reproduction.py` & `semra-0.0.8/src/semra/landscape/cells.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-"""
-Reproduce the scenario from the Biomappings paper on cancer cell lines
+"""A configuration for assembling mappings for cell and cell line terms.
+
+This configuration can be used to reproduce the results from the Biomappings paper
+by doing the following:
 
 1. Load positive mappings
    - PyOBO: EFO, DepMap, CCLE
    - Custom: Cellosaurus
    - Biomappings
 2. Upgrade mappings from dbxrefs to skos:exactMatch
 3. Use transitive closure to infer new mappings
@@ -16,92 +18,94 @@
 import click
 import pystow
 
 from semra.api import project, str_source_target_counts
 from semra.io import write_sssom
 from semra.pipeline import Configuration, Input, Mutation, get_mappings_from_config
 
-MODULE = pystow.module("semra", "case-studies", "cancer-cell-lines")
-PRIORITY_SSSOM_PATH = MODULE.join(name="priority.sssom.tsv")
+__all__ = [
+    "MODULE",
+    "CONFIGURATION",
+]
 
-PREFIXES = {
+MODULE = pystow.module("semra", "case-studies", "cells")
+PREFIXES = PRIORITY = [
+    "mesh",
     "efo",
     "cellosaurus",
-    "depmap",
     "ccle",
-    "clo",
-    "cl",
+    "depmap",
     "bto",
-    "mesh",
+    "cl",
+    "clo",
+    "ncit",
+    "umls",
+]
+
+# some resources are generic, so we want to cut to a relevant subset
+SUBSETS = {
+    "mesh": ["mesh:D002477"],
+    "efo": ["efo:0000324"],
+    "ncit": ["ncit:C12508"],
+    "umls": ["sty:T025"],  # see https://uts.nlm.nih.gov/uts/umls/semantic-network/root
 }
-PRIORITY = ["mesh", "efo", "cellosaurus", "ccle", "depmap", "bto", "cl", "clo"]
-for prefix in PREFIXES:
-    if prefix not in PRIORITY:
-        raise ValueError(f"Missing prioirty order for {prefix}")
 
 CONFIGURATION = Configuration(
     name="Cell and Cell Line Mappings",
     description="Originally a reproduction of the EFO/Cellosaurus/DepMap/CCLE scenario posed in the Biomappings paper, "
     "this configuration imports several different cell and cell line resources and identifies mappings between them.",
     inputs=[
         Input(source="biomappings"),
         Input(source="gilda"),
-        # Cellosaurus removed its xrefs to depmap after v43
-        # FIXME need to upgrade these mappings to SSSOM and trash this old source file
-        # Input(
-        #     source="custom",
-        #     extras={
-        #         "path": "/Users/cthoyt/dev/biomappings/notebooks/cellosaurus_43_xrefs.tsv",
-        #         "source_prefix": "cellosaurus",
-        #         "prefixes": PREFIXES,
-        #         "version": "43",
-        #         "license": "CC-BY-4.0",
-        #     },
-        # ),
         Input(prefix="cellosaurus", source="pyobo", confidence=0.99),
         Input(prefix="bto", source="bioontologies", confidence=0.99),
         Input(prefix="cl", source="bioontologies", confidence=0.99),
-        Input(prefix="clo", source="custom", confidence=0.99),
+        Input(prefix="clo", source="custom", confidence=0.65),
         Input(prefix="efo", source="pyobo", confidence=0.99),
         Input(
             prefix="depmap",
             source="pyobo",
             confidence=0.99,
             extras={"version": "22Q4", "standardize": True, "license": "CC-BY-4.0"},
         ),
         Input(prefix="ccle", source="pyobo", confidence=0.99, extras={"version": "2019"}),
+        Input(prefix="ncit", source="pyobo", confidence=0.99),
+        Input(prefix="umls", source="pyobo", confidence=0.99),
     ],
-    add_labels=False,
+    subsets=SUBSETS,
     priority=PRIORITY,
     keep_prefixes=PREFIXES,
     remove_imprecise=False,
     mutations=[
         Mutation(source="efo", confidence=0.7),
         Mutation(source="bto", confidence=0.7),
         Mutation(source="cl", confidence=0.7),
         Mutation(source="clo", confidence=0.7),
         Mutation(source="depmap", confidence=0.7),
         Mutation(source="ccle", confidence=0.7),
         Mutation(source="cellosaurus", confidence=0.7),
+        Mutation(source="ncit", confidence=0.7),
+        Mutation(source="umls", confidence=0.7),
     ],
     raw_pickle_path=MODULE.join(name="raw.pkl"),
     raw_sssom_path=MODULE.join(name="raw.sssom.tsv"),
-    raw_neo4j_path=MODULE.join("neo4j_raw"),
+    # raw_neo4j_path=MODULE.join("neo4j_raw"),
+    add_labels=True,
     processed_pickle_path=MODULE.join(name="processed.pkl"),
     processed_sssom_path=MODULE.join(name="processed.sssom.tsv"),
     processed_neo4j_path=MODULE.join("neo4j"),
     processed_neo4j_name="semra-cell",
     priority_pickle_path=MODULE.join(name="priority.pkl"),
-    priority_sssom_path=PRIORITY_SSSOM_PATH,
+    priority_sssom_path=MODULE.join(name="priority.sssom.tsv"),
 )
 
 
 @click.command()
 def main():
-    # 1. load mappings
+    """Build the mapping database for cell and cell line terms."""
     mappings = get_mappings_from_config(CONFIGURATION, refresh_raw=True, refresh_processed=True)
 
     click.echo(f"Processing returned {len(mappings):,} mappings")
     click.echo(str_source_target_counts(mappings))
 
     # Produce consolidation mappings
     for s_prefix, t_prefix in [
```

### Comparing `semra-0.0.7/src/semra/__init__.py` & `semra-0.0.8/src/semra/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,35 @@
+"""Semantic Mapping Reasoner and Assembler."""
+
 from semra.pipeline import Configuration, Input, Mutation
-from semra.rules import DB_XREF, EXACT_MATCH, LEXICAL_MAPPING, MANUAL_MAPPING, REPLACED_BY, UNSPECIFIED_MAPPING
+from semra.rules import (
+    BROAD_MATCH,
+    DB_XREF,
+    EXACT_MATCH,
+    LEXICAL_MAPPING,
+    MANUAL_MAPPING,
+    NARROW_MATCH,
+    REPLACED_BY,
+    UNSPECIFIED_MAPPING,
+)
 from semra.struct import Evidence, Mapping, MappingSet, ReasonedEvidence, Reference, SimpleEvidence
 
 __all__ = [
     "Mapping",
     "Evidence",
     "SimpleEvidence",
     "ReasonedEvidence",
     "Reference",
     "MappingSet",
     # Mapping predicates
     "EXACT_MATCH",
     "DB_XREF",
     "REPLACED_BY",
+    "NARROW_MATCH",
+    "BROAD_MATCH",
     # Mapping justifications
     "LEXICAL_MAPPING",
     "MANUAL_MAPPING",
     "UNSPECIFIED_MAPPING",
     # Pipeline
     "Configuration",
     "Input",
```

### Comparing `semra-0.0.7/src/semra/client.py` & `semra-0.0.8/src/semra/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,92 +14,93 @@
 import pydantic
 from neo4j import unit_of_work
 from typing_extensions import TypeAlias
 
 import semra
 from semra import Evidence, MappingSet, Reference
 from semra.io import _get_name_by_curie
+from semra.rules import RELATIONS
 
 __all__ = [
     "Node",
     "Neo4jClient",
 ]
 
 Node: TypeAlias = t.Mapping[str, Any]
 
 TxResult: TypeAlias = t.Optional[t.List[t.List[Any]]]
 
 ReferenceHint: TypeAlias = t.Union[str, Reference]
 
+DEFAULT_MAX_LENGTH = 3
+
+
+def _safe_curie(curie_or_luid: ReferenceHint, prefix: str) -> str:
+    if isinstance(curie_or_luid, Reference):
+        return curie_or_luid.curie
+    if curie_or_luid.startswith(prefix):
+        return curie_or_luid
+    return f"{prefix}:{curie_or_luid}"
+
 
 class Neo4jClient:
     """A client to Neo4j."""
 
     _session: neo4j.Session | None = None
 
     def __init__(
         self,
         uri: str | None = None,
         user: str | None = None,
         password: str | None = None,
     ):
         """Initialize the client.
 
-        Parameters
-        ----------
-        uri :
-            The URI of the Neo4j database.
-        user :
-            The username for the Neo4j database.
-        password :
-            The password for the Neo4j database.
+        :param uri: The URI of the Neo4j database.
+        :param user: The username for the Neo4j database.
+        :param password: The password for the Neo4j database.
         """
         uri = uri or os.environ.get("NEO4J_URL") or "bolt://0.0.0.0:7687"
         user = user or os.environ.get("NEO4J_USER")
         password = password or os.environ.get("NEO4J_PASSWORD")
 
         self.driver = neo4j.GraphDatabase.driver(uri=uri, auth=(user, password), max_connection_lifetime=180)
 
+        query = "CALL db.relationshipTypes() YIELD relationshipType RETURN relationshipType"
+        self._all_relations = {curie for curie, in self.read_query(query)}
+        self._rel_q = "|".join(
+            f"`{reference.curie}`" for reference in RELATIONS if reference.curie in self._all_relations
+        )
+
     def __del__(self):
-        # Ensure driver is shut down when client is destroyed
+        """Ensure driver is shut down when client is destroyed."""
         if self.driver is not None:
             self.driver.close()
 
     def read_query(self, query: str, **query_params) -> list[list]:
-        """Run a read-only query
+        """Run a read-only query.
 
-        Parameters
-        ----------
-        query :
-            The cypher query to run
-        query_params :
-            The parameters to pass to the query
-
-        Returns
-        -------
-        :
-            The result of the query
+        :param query: The cypher query to run
+        :param query_params: The parameters to pass to the query
+        :return: The result of the query
         """
         with self.driver.session() as session:
-            values = session.execute_read(do_cypher_tx, query, **query_params)
+            values = session.execute_read(_do_cypher_tx, query, **query_params)
 
         return values
 
     def write_query(self, query: str, **query_params):
         """Run a write query.
 
-        Parameters
-        ----------
-        query :
-            The cypher query to run
-        query_params :
-            The parameters to pass to the query
+        :param query: The cypher query to run
+        :param query_params: The parameters to pass to the query
+        :return: The result of the write query
         """
         with self.driver.session() as session:
-            return session.write_transaction(do_cypher_tx, query, **query_params)
+            return session.write_transaction(_do_cypher_tx, query, **query_params)
 
     def create_single_property_node_index(
         self, index_name: str, label: str, property_name: str, *, exist_ok: bool = False
     ) -> None:
         """Create a single-property node index.
 
         :param index_name: The name of the index to create.
@@ -120,29 +121,34 @@
         if isinstance(curie, Reference):
             curie = curie.curie
         query = "MATCH (n {curie: $curie}) RETURN n"
         res = self.read_query(query, curie=curie)
         return res[0][0]
 
     def get_mapping(self, curie: ReferenceHint) -> semra.Mapping:
-        """Get a mapping."""
-        if isinstance(curie, Reference):
-            curie = curie.curie
-        if not curie.startswith("semra.mapping:"):
-            curie = f"semra.mapping:{curie}"
+        """Get a mapping.
+
+        :param curie: Either a Reference object, a string representing
+            a curie with ``semra.mapping`` as the prefix, or a local
+            unique identifier representing a SeMRA mapping.
+        :return: A semantic mapping object
+        """
+        curie = _safe_curie(curie, "semra.mapping")
         query = """\
         MATCH
-            (mapping {curie: $curie})-[:`owl:annotatedSource`]->(source) ,
-            (mapping {curie: $curie})-[:`owl:annotatedTarget`]->(target) ,
-            (mapping {curie: $curie})-[:hasEvidence]->(evidence)
+            (mapping {curie: $curie}) ,
+            (mapping)-[:`owl:annotatedSource`]->(source) ,
+            (mapping)-[:`owl:annotatedTarget`]->(target) ,
+            (mapping)-[:hasEvidence]->(evidence)
         OPTIONAL MATCH
             (evidence)-[:fromSet]->(mset)
         OPTIONAL MATCH
             (evidence)-[:hasAuthor]->(author)
         RETURN mapping, source.curie, target.curie, collect([evidence, mset, author.curie])
+        LIMIT 1
         """
         mapping, source_curie, target_curie, evidence_pairs = self.read_query(query, curie=curie)[0]
         evidence: list[Evidence] = []
         for evidence_node, mapping_set_node, author_curie in evidence_pairs:
             evidence_dict = dict(evidence_node)
             if mapping_set_node:
                 evidence_dict["mapping_set"] = MappingSet.parse_obj(mapping_set_node)
@@ -171,24 +177,27 @@
         return [MappingSet.parse_obj(record) for record, in records]
 
     def get_mapping_set(self, curie: ReferenceHint) -> MappingSet:
         """Get a mappings set.
 
         :param curie: The CURIE for a mapping set, using ``semra.mappingset`` as a prefix.
             For example, use ``semra.mappingset:7831d5bc95698099fb6471667e5282cd`` for biomappings
-        :return: A mapping set
+        :return: A mapping set object
         """
-        if isinstance(curie, Reference):
-            curie = curie.curie
-        if not curie.startswith("semra.mappingset:"):
-            curie = f"semra.mappingset:{curie}"
+        curie = _safe_curie(curie, "semra.mappingset")
         node = self._get_node_by_curie(curie)
         return MappingSet.parse_obj(node)
 
-    def get_evidence(self, curie: str) -> Evidence:
+    def get_evidence(self, curie: ReferenceHint) -> Evidence:
+        """Get an evidence.
+
+        :param curie: The CURIE for a mapping set, using ``semra.evidence`` as a prefix.
+        :return: An evidence object
+        """
+        curie = _safe_curie(curie, "semra.evidence")
         query = "MATCH (n {curie: $curie}) RETURN n"
         res = self.read_query(query, curie=curie)
         return res[0][0]
 
     def summarize_predicates(self) -> t.Counter[str]:
         """Get a counter of predicates."""
         query = "MATCH (m:mapping) RETURN m.predicate, count(m.predicate)"
@@ -196,89 +205,148 @@
 
     def summarize_justifications(self) -> t.Counter[str]:
         """Get a counter of mapping justifications."""
         query = "MATCH (e:evidence) RETURN e.mapping_justification, count(e.mapping_justification)"
         return Counter({k.removeprefix("semapv:"): v for k, v in self.read_query(query)})
 
     def summarize_evidence_types(self) -> t.Counter[str]:
+        """Get a counter of evidence types."""
         query = "MATCH (e:evidence) RETURN e.type, count(e.type)"
         return Counter(dict(self.read_query(query)))
 
     def summarize_mapping_sets(self) -> t.Counter[str]:
         """Get the number of evidences in each mapping set."""
         query = "MATCH (e:evidence)-[:fromSet]->(s:mappingset) RETURN s.curie, count(e)"
         return Counter(dict(self.read_query(query)))
 
     def summarize_nodes(self) -> t.Counter[str]:
+        """Get a counter of node types (concepts, evidences, mappings, mapping sets)."""
         query = """\
         MATCH (n:evidence)   WITH count(n) as count RETURN 'Evidences'    as label, count UNION ALL
         MATCH (n:concept)    WITH count(n) as count RETURN 'Concepts'     as label, count UNION ALL
         MATCH (n:concept)    WHERE n.priority WITH count(n) as count RETURN 'Equivalence Classes' \
 as label, count UNION ALL
         MATCH (n:mapping)    WITH count(n) as count RETURN 'Mappings'     as label, count UNION ALL
         MATCH (n:mappingset) WITH count(n) as count RETURN 'Mapping Sets' as label, count
         """
         return Counter(dict(self.read_query(query)))
 
     def summarize_concepts(self) -> t.Counter[tuple[str, str]]:
+        """Get a counter of prefixes in concept nodes."""
         query = "MATCH (e:concept) WHERE e.prefix <> 'orcid' RETURN e.prefix, count(e.prefix)"
         return Counter(
             {(prefix, t.cast(str, bioregistry.get_name(prefix))): count for prefix, count in self.read_query(query)}
         )
 
     def summarize_authors(self) -> t.Counter[tuple[str, str]]:
+        """Get a counter of the number of evidences each author has contributed to."""
         query = "MATCH (e:evidence)-[:hasAuthor]->(a:concept) RETURN a.curie, a.name, count(e)"
         return self._count_with_name(query)
 
     def get_highest_exact_matches(self, limit: int = 10) -> t.Counter[tuple[str, str]]:
+        """Get a counter of concepts with the highest exact matches.
+
+        :param limit: The number of top concepts to return
+        :return: A counter with keys that are CURIE/name pairs
+        """
         query = """\
-            MATCH (a)-[:`skos:exactMatch`]-(b)
+            MATCH (a:concept)-[:`skos:exactMatch`]-(b:concept)
             WHERE a.priority
             RETURN a.curie, a.name, count(distinct b) as c
             ORDER BY c DESCENDING
             LIMIT $limit
         """
         return self._count_with_name(query, limit=limit)
 
     def _count_with_name(self, query: str, **kwargs: Any) -> t.Counter[tuple[str, str]]:
         return Counter({(curie, name): count for curie, name, count in self.read_query(query, **kwargs)})
 
-    def get_exact_matches(self, curie: str) -> dict[Reference, str]:
-        query = "MATCH (a {curie: $curie})-[:`skos:exactMatch`]-(b) RETURN a.curie, a.name"
+    def get_exact_matches(self, curie: ReferenceHint, *, max_distance: t.Optional[int] = None) -> dict[Reference, str]:
+        """Get a mapping of references->name for all concepts equivalent to the given concept."""
+        if isinstance(curie, Reference):
+            curie = curie.curie
+        if max_distance is None:
+            max_distance = DEFAULT_MAX_LENGTH
+        query = f"""\
+            MATCH (a:concept {{curie: $curie}})-[:`skos:exactMatch`*1..{max_distance}]-(b:concept)
+            WHERE a.curie <> b.curie
+            RETURN b.curie, b.name
+        """
         return {Reference.from_curie(n_curie): name for n_curie, name in self.read_query(query, curie=curie)}
 
-    def get_connected_component(self, curie: str) -> tuple[list[neo4j.graph.Node], list[neo4j.graph.Relationship]]:
-        query = """\
-        MATCH (:concept {curie: $curie})-[r *..3 {hasPrimary: true}]-(n:concept)
-        RETURN collect(DISTINCT n) AS nodes, collect(DISTINCT r) AS relations
+    def get_connected_component(
+        self, curie: ReferenceHint, max_distance: t.Optional[int] = None
+    ) -> tuple[list[neo4j.graph.Node], list[neo4j.graph.Relationship]]:
+        """Get the nodes and relations in the connected component of mappings around the given CURIE.
+
+        :param curie: A CURIE string or reference
+        :param max_distance: The maximum number of hops to consider
+        :return: A pair of:
+
+            1. The nodes in the connected component, as Neo4j node objects
+            2. The relationships in the connected component, as Neo4j relationship objects
+        """
+        if isinstance(curie, Reference):
+            curie = curie.curie
+        if max_distance is None:
+            max_distance = DEFAULT_MAX_LENGTH
+        query = f"""\
+            MATCH (:concept {{curie: $curie}})-[r:{self._rel_q} *..{max_distance}]-(n:concept)
+            WHERE ALL(p IN r WHERE p.primary or p.secondary)
+            RETURN collect(DISTINCT n) AS nodes, collect(DISTINCT r) AS relations
         """
         res = self.read_query(query, curie=curie)
         nodes = res[0][0]
-        relations = list({r for relations in res[0][1] for r in relations})
+        relations = sorted({r for relations in res[0][1] for r in relations}, key=lambda r: r.type)
         return nodes, relations
 
-    def get_connected_component_graph(self, curie: str) -> nx.MultiDiGraph:
+    def get_connected_component_graph(self, curie: ReferenceHint) -> nx.MultiDiGraph:
+        """Get a networkx MultiDiGraph representing the connected component of mappings around the given CURIE.
+
+        :param curie: A CURIE string or reference
+        :returns: A networkx MultiDiGraph where mappings subject CURIE strings are th
+        """
         nodes, relations = self.get_connected_component(curie)
         g = nx.MultiDiGraph()
         for node in nodes:
             g.add_node(node["curie"], **node)
         for relation in relations:
             g.add_edge(
                 relation.nodes[0]["curie"],  # type: ignore
                 relation.nodes[1]["curie"],  # type: ignore
                 key=relation.element_id,
                 type=relation.type,
                 **relation,
             )
         return g
 
-    def get_concept_name(self, curie: str) -> str | None:
+    def get_concept_name(self, curie: ReferenceHint) -> str | None:
+        """Get the name for a CURIE or reference."""
+        if isinstance(curie, Reference):
+            curie = curie.curie
         return _get_name_by_curie(curie)
 
+    def sample_mappings_from_set(self, curie: ReferenceHint, n: int = 10) -> t.List:
+        """Get n mappings from a given set (by CURIE)."""
+        if isinstance(curie, Reference):
+            curie = curie.curie
+        query = f"""\
+        MATCH
+            (:mappingset {{curie: $curie}})<-[:fromSet]-()<-[:hasEvidence]-(n:mapping)
+        MATCH
+            (n)-[:`owl:annotatedSource`]->(s:concept)
+        MATCH
+            (n)-[:`owl:annotatedTarget`]->(t:concept)
+        WHERE s.name IS NOT NULL and t.name IS NOT NULL and s.curie < t.curie
+        RETURN n.curie, n.predicate, s.curie, s.name, t.curie, t.name
+        LIMIT {n}
+        """
+        return list(self.read_query(query, curie=curie))
+
 
 # Follows example here:
 # https://neo4j.com/docs/python-manual/current/session-api/#python-driver-simple-transaction-fn
 # and from the docstring of neo4j.Session.read_transaction
 @unit_of_work()
-def do_cypher_tx(tx, query, **query_params) -> list[list]:
+def _do_cypher_tx(tx, query, **query_params) -> list[list]:
     result = tx.run(query, parameters=query_params)
     return [record.values() for record in result]
```

### Comparing `semra-0.0.7/src/semra/database.py` & `semra-0.0.8/src/semra/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 EMPTY = []
 
 summaries = []
 
 
 @click.command()
 def main():
+    """Construct the full SeMRA database."""
     skip = {
         "ado",  # trash
         "epio",  # trash
         "chebi",  # too big
         "pr",  # too big
         "ncbitaxon",  # too big
         "ncit",  # too big
```

### Comparing `semra-0.0.7/src/semra/gilda_utils.py` & `semra-0.0.8/src/semra/gilda_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Utilities for working with Gilda."""
+
 from __future__ import annotations
 
 import itertools as itt
 import logging
 import typing as t
 from collections import defaultdict
 
@@ -133,14 +135,15 @@
 
 def make_new_term(
     term: Term,
     target_db: str,
     target_id: str,
     target_name: str | None = None,
 ) -> Term:
+    """Make a new gilda term object by replacing the database, identifier, and name."""
     if target_name is None:
         from indra.ontology.bio import bio_ontology
 
         target_name = bio_ontology.get_name(target_db, target_id)
     return Term(
         norm_text=term.norm_text,
         text=term.text,
```

### Comparing `semra-0.0.7/src/semra/pipeline.py` & `semra-0.0.8/src/semra/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 import logging
 import time
 import typing as t
 from pathlib import Path
 from typing import Any, Literal, Optional
 
 from pydantic import BaseModel, Field, root_validator
-from tqdm.autonotebook import tqdm
+from tqdm.auto import tqdm
 
 from semra.api import (
     assemble_evidences,
     filter_mappings,
     filter_prefixes,
     filter_self_matches,
+    filter_subsets,
+    hydrate_subsets,
     infer_chains,
     infer_mutual_dbxref_mutations,
     infer_reversible,
     keep_prefixes,
     prioritize,
     validate_mappings,
 )
@@ -37,69 +39,86 @@
 from semra.sources import SOURCE_RESOLVER
 from semra.sources.biopragmatics import (
     from_biomappings_negative,
     from_biomappings_predicted,
     get_biomappings_positive_mappings,
 )
 from semra.sources.gilda import get_gilda_mappings
+from semra.sources.wikidata import get_wikidata_mappings_by_prefix
 from semra.struct import Mapping, Reference
 
 __all__ = [
     # Configuration model
     "Configuration",
+    "SubsetConfiguration",
     "Input",
     "Mutation",
     # Functions
     "get_mappings_from_config",
     "get_raw_mappings",
     "process",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 class Input(BaseModel):
     """Represents the input to a mapping assembly."""
 
-    source: Literal["pyobo", "bioontologies", "biomappings", "custom", "sssom", "gilda"]
+    source: Literal["pyobo", "bioontologies", "biomappings", "custom", "sssom", "gilda", "wikidata"]
     prefix: Optional[str] = None
     confidence: float = 1.0
     extras: t.Dict[str, Any] = Field(default_factory=dict)
 
 
 class Mutation(BaseModel):
     """Represents a mutation operation on a mapping set."""
 
     source: str = Field(..., description="The source type")
     confidence: float = 1.0
     old: Reference = Field(default=DB_XREF)
     new: Reference = Field(default=EXACT_MATCH)
 
 
+SubsetConfiguration = t.Mapping[str, t.Collection[str]]
+
+
 class Configuration(BaseModel):
     """Represents the steps taken during mapping assembly."""
 
     name: str = Field(description="The name of the mapping set configuration")
     description: Optional[str] = Field(
         None, description="An explanation of the purpose of the mapping set configuration"
     )
     inputs: t.List[Input] = Field(..., description="A list of sources of mappings")
     negative_inputs: t.List[Input] = Field(default=[Input(source="biomappings", prefix="negative")])
     priority: t.List[str] = Field(
         default_factory=list, description="If no priority is given, is inferred from the order of inputs"
     )
     mutations: t.List[Mutation] = Field(default_factory=list)
+    subsets: t.Optional[t.Mapping[str, t.List[str]]] = Field(
+        None,
+        description="A field to put restrictions on the subhierarchies from each resource. For example, if "
+        "you want to assemble cell mappings from MeSH, you don't need all possible mesh mappings, but only "
+        "ones that have to do with terms in the cell hierchy under the mesh:D002477 term. Therefore, this "
+        "dictionary allows for specifying such restrictions",
+        examples=[
+            {"mesh": ["mesh:D002477"]},
+        ],
+    )
 
     exclude_pairs: t.List[t.Tuple[str, str]] = Field(
         default_factory=list,
         description="A list of pairs of prefixes. Remove all mappings whose source "
         "prefix is the first in a pair and target prefix is second in a pair. Order matters.",
     )
-    remove_prefixes: Optional[t.List[str]] = None
-    keep_prefixes: Optional[t.List[str]] = None
+    remove_prefixes: Optional[t.List[str]] = Field(None, description="Prefixes to remove before processing")
+    keep_prefixes: Optional[t.List[str]] = Field(None, description="Prefixes to keep before processing")
+    post_remove_prefixes: Optional[t.List[str]] = Field(None, description="Prefixes to remove after processing")
+    post_keep_prefixes: Optional[t.List[str]] = Field(None, description="Prefixes to keep after processing")
     remove_imprecise: bool = True
     validate_raw: bool = Field(
         default=False,
         description="Should the raw mappings be validated against Bioregistry "
         "prefixes and local unique identifier regular expressions (when available)?",
     )
 
@@ -144,14 +163,36 @@
         *,
         refresh_raw: bool = False,
         refresh_processed: bool = False,
     ) -> t.List[Mapping]:
         """Run assembly based on this configuration."""
         return get_mappings_from_config(self, refresh_raw=refresh_raw, refresh_processed=refresh_processed)
 
+    def read_raw_mappings(self) -> t.List[Mapping]:
+        """Read raw mappings from pickle, if already cached."""
+        if self.raw_pickle_path is None:
+            raise ValueError
+        if not self.raw_pickle_path.is_file():
+            raise FileNotFoundError
+        return from_pickle(self.raw_pickle_path)
+
+    def read_processed_mappings(self) -> t.List[Mapping]:
+        """Read processed mappings from pickle, if already cached."""
+        if self.processed_pickle_path is None:
+            raise ValueError
+        if not self.processed_pickle_path.is_file():
+            raise FileNotFoundError
+        return from_pickle(self.processed_pickle_path)
+
+    def get_hydrated_subsets(self) -> t.Mapping[str, t.Collection[str]]:
+        """Get the full subset filter lists based on the parent configuration."""
+        if not self.subsets:
+            return {}
+        return hydrate_subsets(self.subsets)
+
 
 def get_mappings_from_config(
     configuration: Configuration,
     *,
     refresh_raw: bool = False,
     refresh_processed: bool = False,
 ) -> t.List[Mapping]:
@@ -175,32 +216,35 @@
     else:
         raw_mappings = get_raw_mappings(configuration)
         if configuration.validate_raw:
             validate_mappings(raw_mappings)
         if configuration.raw_pickle_path:
             write_pickle(raw_mappings, configuration.raw_pickle_path)
         if configuration.raw_sssom_path:
-            write_sssom(raw_mappings, configuration.raw_sssom_path, add_labels=configuration.add_labels)
+            write_sssom(raw_mappings, configuration.raw_sssom_path)  # , add_labels=configuration.add_labels)
         if configuration.raw_neo4j_path:
             write_neo4j(
                 raw_mappings,
                 configuration.raw_neo4j_path,
                 docker_name=configuration.raw_neo4j_name,
-                add_labels=configuration.add_labels,
+                add_labels=False,  # configuration.add_labels,
             )
 
     # click.echo(semra.api.str_source_target_counts(mappings, minimum=20))
     processed_mappings = process(
         raw_mappings,
         upgrade_prefixes=[  # TODO more carefully compile a set of mutations together for applying
             m.source for m in configuration.mutations
         ],
         remove_prefix_set=configuration.remove_prefixes,
         keep_prefix_set=configuration.keep_prefixes,
+        post_remove_prefixes=configuration.post_remove_prefixes,
+        post_keep_prefixes=configuration.post_keep_prefixes,
         remove_imprecise=configuration.remove_imprecise,
+        subsets=configuration.get_hydrated_subsets(),
     )
     prioritized_mappings = prioritize(processed_mappings, configuration.priority)
 
     if configuration.processed_pickle_path:
         write_pickle(processed_mappings, configuration.processed_pickle_path)
     if configuration.processed_sssom_path:
         write_sssom(processed_mappings, configuration.processed_sssom_path, add_labels=configuration.add_labels)
@@ -256,40 +300,48 @@
             else:
                 raise ValueError
         elif inp.source == "gilda":
             mappings.extend(get_gilda_mappings(confidence=inp.confidence))
         elif inp.source == "custom":
             func = SOURCE_RESOLVER.make(inp.prefix, inp.extras)
             mappings.extend(func())
+        elif inp.source == "wikidata":
+            mappings.extend(get_wikidata_mappings_by_prefix(inp.prefix, **inp.extras))
         elif inp.source == "sssom":
             mappings.extend(from_sssom(inp.prefix, **inp.extras))
         elif inp.source == "cache":
             mappings.extend(from_cache_df(**inp.extras))
         else:
             raise ValueError
     return mappings
 
 
 def process(
     mappings: t.List[Mapping],
     upgrade_prefixes=None,
-    remove_prefix_set=None,
-    keep_prefix_set=None,
+    remove_prefix_set: t.Optional[t.Collection[str]] = None,
+    keep_prefix_set: t.Optional[t.Collection[str]] = None,
+    post_remove_prefixes: t.Optional[t.Collection[str]] = None,
+    post_keep_prefixes: t.Optional[t.Collection[str]] = None,
+    subsets: t.Optional[t.Mapping[str, t.Collection[str]]] = None,
     *,
     remove_imprecise: bool = True,
 ) -> t.List[Mapping]:
     """Run a full deduplication, reasoning, and inference pipeline over a set of mappings."""
     from semra.sources.biopragmatics import from_biomappings_negative
 
     if keep_prefix_set:
         mappings = keep_prefixes(mappings, keep_prefix_set)
 
     if remove_prefix_set:
         mappings = filter_prefixes(mappings, remove_prefix_set)
 
+    if subsets:
+        mappings = list(filter_subsets(mappings, subsets))
+
     start = time.time()
     negatives = from_biomappings_negative()
     logger.info(f"Loaded {len(negatives):,} negative mappings in %.2f seconds", time.time() - start)
 
     before = len(mappings)
     start = time.time()
     mappings = filter_mappings(mappings, negatives)
@@ -349,14 +401,20 @@
     start = time.time()
     mappings = filter_mappings(mappings, negatives)
     _log_diff(before, mappings, verb="Filtered negative mappings", elapsed=time.time() - start)
 
     # filter out self mappings again, just in case
     mappings = filter_self_matches(mappings)
 
+    if post_keep_prefixes:
+        mappings = keep_prefixes(mappings, post_keep_prefixes)
+
+    if post_remove_prefixes:
+        mappings = filter_prefixes(mappings, post_remove_prefixes)
+
     return mappings
 
 
 def _log_diff(before: int, mappings: t.List[Mapping], *, verb: str, elapsed) -> None:
     logger.info(
         f"{verb} from {before:,} to {len(mappings):,} mappings (Δ={len(mappings) - before:,}) in %.2f seconds.",
         elapsed,
```

### Comparing `semra-0.0.7/src/semra/rules.py` & `semra-0.0.8/src/semra/rules.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 BROAD_MATCH = Reference(prefix="skos", identifier="broadMatch")
 NARROW_MATCH = Reference(prefix="skos", identifier="narrowMatch")
 CLOSE_MATCH = Reference(prefix="skos", identifier="closeMatch")
 DB_XREF = Reference(prefix="oboinowl", identifier="hasDbXref")
 EQUIVALENT_TO = Reference(prefix="owl", identifier="equivalentTo")
 REPLACED_BY = Reference(prefix="iao", identifier="0100001")
 
+RELATIONS = [EXACT_MATCH, DB_XREF, BROAD_MATCH, NARROW_MATCH, CLOSE_MATCH, EQUIVALENT_TO, REPLACED_BY]
+
 IMPRECISE = {DB_XREF, CLOSE_MATCH}
 FLIP = {
     BROAD_MATCH: NARROW_MATCH,
     NARROW_MATCH: BROAD_MATCH,
     EXACT_MATCH: EXACT_MATCH,
     CLOSE_MATCH: CLOSE_MATCH,
     DB_XREF: DB_XREF,
```

### Comparing `semra-0.0.7/src/semra/struct.py` & `semra-0.0.8/src/semra/struct.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,21 +35,16 @@
 
 
 def triple_key(triple: Triple) -> t.Tuple[str, str, str]:
     """Get a sortable key for a triple."""
     return triple[0].curie, triple[2].curie, triple[1].curie
 
 
-EPSILON = 1e-6
-EvidenceType = Literal["simple", "mutated", "reasoned"]
-JUSTIFICATION_FIELD = Field(description="A SSSOM-compliant justification")
-
-
 def _md5_hexdigest(picklable) -> str:
-    hasher = md5()  # noqa:S324
+    hasher = md5()  # noqa:S324,S303
     hasher.update(pickle.dumps(picklable))
     return hasher.hexdigest()
 
 
 class KeyedMixin:
     """A mixin for a class that can be hashed and CURIE-encoded."""
 
@@ -75,23 +70,43 @@
     @property
     def curie(self) -> str:
         """Get a string representing the CURIE."""
         return self.get_reference().curie
 
 
 class ConfidenceMixin:
+    """A mixin for classes that have confidence information."""
+
     def get_confidence(self) -> float:
+        """Get the confidence.
+
+        :return:
+            The confidence, which can either be a direct annotation
+            or computed based on other related objects. For example,
+            a :class:`MappingSet` has an explicitly annotated confidence,
+            whereas a :class:`ReasonedEvidence` calculates its confidence
+            based on all of its prior probability *and* the confidences
+            of the mappings on which it depends.
+        """  # noqa:DAR401,DAR202
         raise NotImplementedError
 
 
 class EvidenceMixin:
+    """A mixin for evidence classes."""
+
     @property
     def explanation(self) -> str:
+        """Get a textual explanation for this evidence."""
         return ""
 
+    @property
+    def mapping_set_names(self) -> t.Set[str]:
+        """Get set of mapping set names that contribute to this evidence."""
+        raise NotImplementedError
+
 
 class MappingSet(pydantic.BaseModel, ConfidenceMixin, KeyedMixin, prefix="semra.mappingset"):
     """Represents a set of semantic mappings.
 
     For example, this might correspond to:
 
     1. All the mappings extracted from an ontology
@@ -105,15 +120,15 @@
     confidence: float = Field(..., description="Mapping set level confidence")
 
     def key(self):
         """Get a picklable key representing the mapping set."""
         return self.name, self.version or "", self.license or "", self.confidence
 
     def get_confidence(self) -> float:
-        """Get the confidence for the mapping set."""
+        """Get the explicit confidence for the mapping set."""
         return self.confidence
 
 
 class SimpleEvidence(pydantic.BaseModel, KeyedMixin, EvidenceMixin, ConfidenceMixin, prefix="semra.evidence"):
     """Evidence for a mapping.
 
     Ideally, this matches the SSSOM data model.
@@ -147,17 +162,19 @@
 
         Note: this should be extended to include basically _all_ fields
         """
         return self.evidence_type, self.justification, self.author, self.mapping_set.key(), self.uuid
 
     @property
     def mapping_set_names(self) -> t.Set[str]:
+        """Get a set containing 1 element - this evidence's mapping set's name."""
         return {self.mapping_set.name}
 
     def get_confidence(self) -> float:
+        """Get the confidence from the mapping set."""
         return self.confidence if self.confidence is not None else self.mapping_set.confidence
 
 
 class ReasonedEvidence(pydantic.BaseModel, KeyedMixin, EvidenceMixin, ConfidenceMixin, prefix="semra.evidence"):
     """A complex evidence based on multiple mappings."""
 
     class Config:
@@ -170,39 +187,57 @@
     mappings: t.List[Mapping] = Field(
         ..., description="A list of mappings and their evidences consumed to create this evidence"
     )
     author: Optional[Reference] = None
     confidence_factor: float = Field(1.0, description="The probability that the reasoning method is correct")
 
     def key(self):
+        """Get a key for reasoned evidence."""
         return (
             self.evidence_type,
             self.justification,
             *((*m.triple, *(e.key() for e in m.evidence)) for m in self.mappings),
         )
 
     def get_confidence(self) -> float:
+        r"""Calculate confidence for the reasoned evidence.
+
+        :returns:
+            The joint binomial probability that all reasoned evidences
+            are correct. This is calculated with the following:
+
+            $\alpha \times (1 - \sum_{e \in E} 1 - \text{confidence}_e)$
+
+            where $E$ is the set of all evidences in this object and
+            $\alpha$ is the confidence factor for the reasoning approach.
+        """
         confidences = [mapping.get_confidence() for mapping in self.mappings]
         return _joint_probability([self.confidence_factor, *confidences])
 
     @property
     def mapping_set(self) -> None:
+        """Return an empty mapping set, since this is a reasoned evidence."""
         return None
 
     @property
     def mapping_set_names(self) -> t.Set[str]:
+        """Get a set containing the union of all the mappings' evidences' mapping set names."""
         return {
-            name
-            for mapping in self.mappings
-            for evidence in mapping.evidence
-            for name in evidence.mapping_set_names  # type:ignore
+            name for mapping in self.mappings for evidence in mapping.evidence for name in evidence.mapping_set_names
         }
 
     @property
     def explanation(self) -> str:
+        """Get a textual explanation for this reasoned evidence.
+
+        :returns:
+            Assuming this reasoned evidence represents a pathway where each mapping
+            in the chain's subject shares the object from the previous mapping, returns
+            a space-delmited list of the CURIEs for these entities.
+        """
         return " ".join(mapping.s.curie for mapping in self.mappings) + " " + self.mappings[-1].o.curie
 
 
 Evidence = Annotated[
     Union[ReasonedEvidence, SimpleEvidence],
     Field(discriminator="evidence_type"),
 ]
@@ -223,14 +258,15 @@
 
     @property
     def triple(self) -> Triple:
         """Get the mapping's core triple as a tuple."""
         return self.s, self.p, self.o
 
     def key(self):
+        """Get a hashable key for the mapping, based on the subject, predicate, and object."""
         return self.triple
 
     @classmethod
     def from_triple(cls, triple: Triple, evidence: Optional[t.List[Evidence]] = None) -> Mapping:
         """Instantiate a mapping from a triple."""
         s, p, o = triple
         return cls(s=s, p=p, o=o, evidence=evidence or [])
```

### Comparing `semra-0.0.7/src/semra/wsgi.py` & `semra-0.0.8/src/semra/wsgi.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import typing as t
 
 import fastapi
 import flask
 import networkx as nx
 from curies import Reference
-from fastapi import Path
+from fastapi import Path, Query
 from fastapi.responses import JSONResponse
 from flask import Flask, render_template
 from flask_bootstrap import Bootstrap5
 from starlette.middleware.wsgi import WSGIMiddleware
 
 from semra import Evidence, Mapping, MappingSet
 from semra.client import Neo4jClient
@@ -29,17 +29,26 @@
 
 api_router = fastapi.APIRouter(prefix="/api")
 
 flask_app = Flask(__name__)
 flask_app.secret_key = os.urandom(8)
 Bootstrap5(flask_app)
 
-
 EXAMPLE_CONCEPTS = ["efo:0002142"]
-EXAMPLE_MAPPINGS = ["25b67912bc720127a43a06ce4688b672", "5a56bf7ac409d8de84c3382a99e17715"]
+EXAMPLE_MAPPINGS = list(
+    client.read_query(
+        """\
+    MATCH
+        (t:concept)<-[`owl:annotatedTarget`]-(n:mapping)-[`owl:annotatedSource`]->(s:concept)
+    WHERE n.predicate = 'skos:exactMatch'
+    RETURN n.curie, n.predicate, s.curie, s.name, t.curie, t.name
+    LIMIT 5
+    """
+    )
+)
 
 
 PREDICATE_COUNTER = client.summarize_predicates()
 MAPPING_SET_COUNTER = client.summarize_mapping_sets()
 NODE_COUNTER = client.summarize_nodes()
 JUSTIFICATION_COUNTER = client.summarize_justifications()
 EVIDENCE_TYPE_COUNTER = client.summarize_evidence_types()
@@ -66,14 +75,15 @@
             return round(lead), "K"
     else:
         return n, ""
 
 
 @flask_app.get("/")
 def home():
+    """View the homepage, with a dashboard for several statistics over the database."""
     # TODO
     #  1. Mapping with most evidences
     #  7. Nodes with equivalent entity sharing its prefix
     return render_template(
         "home.html",
         example_mappings=EXAMPLE_MAPPINGS,
         predicate_counter=PREDICATE_COUNTER,
@@ -111,17 +121,15 @@
         exact_matches=exact_matches,
         has_biomappings=BIOMAPPINGS_GIT_HASH is not None,
     )
 
 
 @flask_app.get("/concept/<source>/invalidate/<target>")
 def mark_exact_incorrect(source: str, target: str):
-    """
-    Add a negative relationship to biomappings.
-    """
+    """Add a negative relationship to biomappings."""
     if not BIOMAPPINGS_GIT_HASH:
         flask.flash("Can't interact with biomappings", category="error")
         return flask.redirect(flask.url_for(view_concept.__name__, curie=source))
 
     import biomappings.resources
 
     source_reference = Reference.from_curie(source)
@@ -143,57 +151,73 @@
     }
     biomappings.resources.append_false_mappings([mapping])
 
     flask.flash("Appended negative mapping")
     return flask.redirect(flask.url_for(view_concept.__name__, curie=source))
 
 
-@flask_app.get("/mapping_set/<curie>")
-def view_mapping_set(curie: str):
-    """View a mapping."""
-    m = client.get_mapping_set(curie)
-    # TODO sample 10 mappings
-    return render_template("mapping_set.html", mapping_set=m)
+@flask_app.get("/mapping_set/{mapping_set_id}")
+def view_mapping_set(mapping_set_id: str):
+    """View a mapping set by its ID."""
+    mapping_set = client.get_mapping_set(mapping_set_id)
+    examples = client.sample_mappings_from_set(mapping_set_id, n=10)
+    return render_template("mapping_set.html", mapping_set=mapping_set, mapping_examples=examples)
 
 
-@api_router.get("/evidence/{curie}", response_model=Evidence)
-def get_evidence(curie: str = Path(description="An evidence's MD5 hex digest.")):
-    return client.get_evidence(curie)
+@api_router.get("/evidence/{evidence_id}", response_model=Evidence)
+def get_evidence(evidence_id: str = Path(description="An evidence's MD5 hex digest.")):
+    """Get an evidence by its MD5 hex digest."""
+    return client.get_evidence(evidence_id)
 
 
 @api_router.get("/cytoscape/{curie}")
 def get_concept_cytoscape(
     curie: str = Path(description="the compact URI (CURIE) for a concept", examples=EXAMPLE_CONCEPTS)
 ):
     """Get the mapping graph surrounding the concept as a Cytoscape.js JSON object."""
     graph = client.get_connected_component_graph(curie)
     cytoscape_json = nx.cytoscape_data(graph)["elements"]
     return JSONResponse(cytoscape_json)
 
 
-@api_router.get("/mapping/{mapping}", response_model=Mapping)
-def get_mapping(mapping: str = Path(description="A mapping's MD5 hex digest.", examples=EXAMPLE_MAPPINGS)):
-    return client.get_mapping(mapping)
+@api_router.get("/exact/{curie}", response_model=t.List[Reference])
+def get_exact_matches(
+    curie: str = Path(description="the compact URI (CURIE) for a concept", examples=EXAMPLE_CONCEPTS),
+    max_distance: int = Query(None, description="the distance in the mapping graph to traverse. Defaults to 7"),
+):
+    """Get the exact matches to the concept."""
+    return list(client.get_exact_matches(curie, max_distance=max_distance))
+
+
+@api_router.get("/mapping/{mapping_id}", response_model=Mapping)
+def get_mapping(
+    mapping_id: str = Path(description="A mapping's MD5 hex digest.", examples=[t[0] for t in EXAMPLE_MAPPINGS])
+):
+    """Get the mapping by its MD5 hex digest."""
+    return client.get_mapping(mapping_id)
 
 
-@api_router.get("/mapping_set/{mapping_set}", response_model=MappingSet)
+@api_router.get("/mapping_set/{mapping_set_id}", response_model=MappingSet)
 def get_mapping_set(
-    mapping_set: str = Path(
+    mapping_set_id: str = Path(
         description="A mapping set's MD5 hex digest.", examples=["7831d5bc95698099fb6471667e5282cd"]
     )
 ):
-    return client.get_mapping_set(mapping_set)
+    """Get a mapping set by its MD5 hex digest."""
+    return client.get_mapping_set(mapping_set_id)
 
 
 @api_router.get("/mapping_set/", response_model=t.List[MappingSet])
 def get_mapping_sets():
+    """Get all mapping sets."""
     return client.get_mapping_sets()
 
 
 def get_app():
+    """Get the SeMRA FastAPI app."""
     app = fastapi.FastAPI(
         title="Semantic Reasoning Assembler",
         description="A web app to access a SeMRA Neo4j database",
     )
     app.include_router(api_router)
     app.mount("/", WSGIMiddleware(flask_app))
     return app
```

### Comparing `semra-0.0.7/src/semra/sources/__init__.py` & `semra-0.0.8/src/semra/sources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,62 +8,69 @@
 from semra.sources.biopragmatics import (
     from_biomappings_negative,
     from_biomappings_predicted,
     get_biomappings_positive_mappings,
 )
 from semra.sources.chembl import get_chembl_compound_mappings, get_chembl_protein_mappings
 from semra.sources.clo import get_clo_mappings
-from semra.sources.famplex import get_famplex_mappings
+from semra.sources.famplex import get_fplx_mappings
 from semra.sources.gilda import get_gilda_mappings
 from semra.sources.intact import get_intact_complexportal_mappings, get_intact_reactome_mappings
 from semra.sources.ncit import (
     get_ncit_chebi_mappings,
     get_ncit_go_mappings,
     get_ncit_hgnc_mappings,
     get_ncit_uniprot_mappings,
 )
+from semra.sources.omim import get_omim_gene_mappings
 from semra.sources.pubchem import get_pubchem_mesh_mappings
+from semra.sources.wikidata import get_wikidata_mappings
 from semra.struct import Mapping
 
 __all__ = [
+    "SOURCE_RESOLVER",
     "get_chembl_compound_mappings",
     "get_ncit_chebi_mappings",
     "get_ncit_uniprot_mappings",
     "get_ncit_go_mappings",
     "get_ncit_hgnc_mappings",
     "get_pubchem_mesh_mappings",
     "get_chembl_protein_mappings",
-    "get_famplex_mappings",
+    "get_fplx_mappings",
     "get_intact_complexportal_mappings",
     "get_intact_reactome_mappings",
     "get_custom",
     "get_biomappings_positive_mappings",
     "from_biomappings_predicted",
     "from_biomappings_negative",
     "get_gilda_mappings",
     "get_clo_mappings",
+    "get_wikidata_mappings",
+    "get_omim_gene_mappings",
 ]
 
 SOURCE_RESOLVER: FunctionResolver[t.Callable[[], t.List[Mapping]]] = FunctionResolver(
     [
         get_chembl_compound_mappings,
         get_chembl_protein_mappings,
         get_intact_reactome_mappings,
         get_intact_complexportal_mappings,
-        get_famplex_mappings,
+        get_fplx_mappings,
         get_pubchem_mesh_mappings,
         get_ncit_chebi_mappings,
         get_ncit_hgnc_mappings,
         get_ncit_go_mappings,
         get_ncit_uniprot_mappings,
         # from_biomappings_negative,
         # from_biomappings_predicted,
         get_biomappings_positive_mappings,
         get_gilda_mappings,
         get_clo_mappings,
+        get_wikidata_mappings,
+        get_omim_gene_mappings,
     ]
 )
 
 # Add synonyms for short name
 for func in SOURCE_RESOLVER:
     if not func.__name__.startswith("get_"):
         raise NameError(f"Custom source function name does not start with `_get`: {func.__name__}")
```

### Comparing `semra-0.0.7/src/semra/sources/biopragmatics.py` & `semra-0.0.8/src/semra/sources/biopragmatics.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/sources/chembl.py` & `semra-0.0.8/src/semra/sources/chembl.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/sources/clo.py` & `semra-0.0.8/src/semra/sources/clo.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,27 @@
 
 def _removeprefix(s: str, prefix: str) -> str:
     if s.startswith(prefix):
         return s[len(prefix) :]
     return s
 
 
-def get_clo_mappings(confidence: float = 0.8) -> list[Mapping]:
+def get_clo_mappings(confidence: float = 0.8) -> list[Mapping]:  # noqa:C901
+    """Get Cell Line Ontology mappings.
+
+    :param confidence: How confidence are you in the quality of these mappings being exact? By default, is 0.8.
+    :return: Semantic mappings extracted from the CLO
+    :raises ValueError:
+        if a prefix is encountered that doesn't have a regular expression defined in the
+        Bioregistry. If you get this error, please report it on the Bioregistry's issue
+        tracker https://github.com/biopragmatics/bioregistry/issues/new?&labels=Update&template=update-misc.yml
+
+    Note that this function exists because CLO doesn't use standard curation for xrefs
+    and instead uses a combination of messy references inside rdfs:seeAlso annotations
+    """
     graph = bioontologies.get_obograph_by_prefix("clo", check=False).guess("clo")
     mapping_set = MappingSet(
         name="clo",
         version=graph.version,
         license=bioregistry.get_license("clo"),
         confidence=confidence,
     )
@@ -43,15 +55,15 @@
         if not node.id.startswith(CLO_URI_PREFIX):
             continue
         clo_id = node.id[len(CLO_URI_PREFIX) :]
         for p in node.properties or []:
             if p.predicate_raw != "http://www.w3.org/2000/01/rdf-schema#seeAlso":
                 continue
             for raw_curie in _split(p.value_raw):
-                curie = _removeprefix(_removeprefix(raw_curie, "rrid:"), "RRID")
+                curie = _removeprefix(_removeprefix(raw_curie, "rrid:"), "RRID:")
                 prefix: Optional[str]
                 identifier: Optional[str]
                 if curie.startswith("Sanger:COSMICID:"):
                     prefix, identifier = "cosmic.cell", _removeprefix(curie, "Sanger:COSMICID:")
                 elif curie.startswith("RRID:CVCL_"):
                     prefix, identifier = "cellosaurus", _removeprefix(curie, "RRID:CVCL_")
                 elif curie.startswith("RRID: CVCL_"):
```

### Comparing `semra-0.0.7/src/semra/sources/famplex.py` & `semra-0.0.8/src/semra/sources/famplex.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from curies import Reference
 
 from semra.api import validate_mappings
 from semra.rules import BEN_ORCID, EXACT_MATCH, MANUAL_MAPPING
 from semra.struct import Mapping, MappingSet, SimpleEvidence
 
 __all__ = [
-    "get_famplex_mappings",
+    "get_fplx_mappings",
 ]
 
 logger = logging.getLogger(__name__)
 
 URL = "https://github.com/sorgerlab/famplex/raw/master/equivalences.csv"
-MAPPING_SET = MappingSet(name="famplex", confidence=0.99, license="CC0")
+MAPPING_SET = MappingSet(name="fplx", confidence=0.99, license="CC0")
 
 
-def get_famplex_mappings() -> list[Mapping]:
+def get_fplx_mappings() -> list[Mapping]:
     """Get xrefs from FamPlex."""
     df = pd.read_csv(URL, header=None, names=["target_prefix", "target_id", "source_id"], sep=",")
     df = df[df["target_prefix"] != "MEDSCAN"]
     rv = [
         Mapping(
             s=Reference(prefix="fplx", identifier=source_id),
             p=EXACT_MATCH,
@@ -43,8 +43,8 @@
         )
     ]
     validate_mappings(rv)
     return rv
 
 
 if __name__ == "__main__":
-    get_famplex_mappings()
+    get_fplx_mappings()
```

### Comparing `semra-0.0.7/src/semra/sources/gilda.py` & `semra-0.0.8/src/semra/sources/gilda.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     for k in ("source_prefix", "target_prefix"):
         df[k] = df[k].map(bioregistry.normalize_prefix)  # type:ignore
     rv = []
     for sp, si, tp, ti in tqdm(df.values, desc="Loading Gilda", unit="mapping", unit_scale=True):
         if not sp or not tp:
             continue
         m = Mapping(
-            s=Reference(prefix=sp, identifier=bioregistry.standardize_identifier(sp, si)),
+            s=Reference(prefix=bioregistry.normalize_prefix(sp), identifier=bioregistry.standardize_identifier(sp, si)),
             p=EXACT_MATCH,
-            o=Reference(prefix=tp, identifier=bioregistry.standardize_identifier(tp, ti)),
+            o=Reference(prefix=bioregistry.normalize_prefix(tp), identifier=bioregistry.standardize_identifier(tp, ti)),
             evidence=[
                 SimpleEvidence(
                     justification=LEXICAL_MAPPING,
                     mapping_set=MappingSet(name="gilda_mesh", confidence=confidence, license="CC0"),
                     author=BEN_ORCID,
                 )
             ],
```

### Comparing `semra-0.0.7/src/semra/sources/intact.py` & `semra-0.0.8/src/semra/sources/intact.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/sources/ncit.py` & `semra-0.0.8/src/semra/sources/ncit.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,47 +49,51 @@
     return SimpleEvidence(
         justification=UNSPECIFIED_MAPPING,
         mapping_set=MappingSet(name="ncit", version=version, license=license, confidence=CONFIDENCE),
     )
 
 
 def get_ncit_hgnc_mappings() -> list[Mapping]:
+    """Get NCIT to HGNC semantic mappings."""
     df = pd.read_csv(HGNC_MAPPINGS_URL, sep="\t", header=None, names=["ncit", "hgnc"])
     df["hgnc"] = df["hgnc"].map(lambda s: s.removeprefix("HGNC:"))  # type:ignore
     return _df_to_mappings(
         df,
         source_prefix="ncit",
         target_prefix="hgnc",
         evidence=_get_evidence,
     )
 
 
 def get_ncit_go_mappings() -> list[Mapping]:
+    """Get NCIT to Gene Ontology (GO) semantic mappings."""
     df = pd.read_csv(HGNC_MAPPINGS_URL, sep="\t", header=None, names=["go", "ncit"])
     df["go"] = df["go"].map(lambda s: s.removeprefix("GO:"))  # type:ignore
     return _df_to_mappings(
         df,
         source_prefix="ncit",
         target_prefix="go",
         evidence=_get_evidence,
     )
 
 
 def get_ncit_chebi_mappings() -> list[Mapping]:
+    """Get NCIT to ChEBI semantic mappings."""
     df = pd.read_csv(HGNC_MAPPINGS_URL, sep="\t", header=None, names=["ncit", "chebi"])
     df["chebi"] = df["chebi"].map(lambda s: s.removeprefix("CHEBI:"))  # type:ignore
     return _df_to_mappings(
         df,
         source_prefix="ncit",
         target_prefix="chebi",
         evidence=_get_evidence,
     )
 
 
 def get_ncit_uniprot_mappings() -> list[Mapping]:
+    """Get NCIT to UniProt semantic mappings."""
     df = pd.read_csv(SWISSPROT_MAPPINGS_URL, sep="\t", header=None, names=["ncit", "uniprot"])
     return _df_to_mappings(
         df,
         source_prefix="ncit",
         target_prefix="uniprot",
         evidence=_get_evidence,
     )
```

### Comparing `semra-0.0.7/src/semra/sources/pubchem.py` & `semra-0.0.8/src/semra/sources/pubchem.py`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/templates/base.html` & `semra-0.0.8/src/semra/templates/base.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/templates/concept.html` & `semra-0.0.8/src/semra/templates/concept.html`

 * *Files identical despite different names*

### Comparing `semra-0.0.7/src/semra/templates/home.html` & `semra-0.0.8/src/semra/templates/home.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% extends "base.html" %}
 
-{% import "bootstrap5/utils.html" as util %}
+{% import "bootstrap5/utils.html" as bs_util %}
+{% import "utils.html" as util %}
 
 {% block title %}SeMRA{% endblock %}
 
 
 {% macro count_column(counter, key, icon) -%}
 <div class="col">
     {% set count, suffix = format_number(counter[key]) %}
@@ -18,58 +19,63 @@
 <div class="card-body">
     <h6>{{ label }} Summary</h6>
 </div>
 <table class="table">
     <thead>
     <tr>
         <th>{{ label }}</th>
-        {% if has_names %}<th>Name</th>{% endif %}
+        {% if has_names %}
+        <th>Name</th>
+        {% endif %}
         <th>Count</th>
     </tr>
     </thead>
     <tbody>
     {% for key, count in counter.most_common() %}
     <tr>
         <td><code>
-        {%- if is_concept -%}
+            {%- if is_concept -%}
             {% if has_names %}
             <a href="{{ url_for('view_concept', curie=key[0]) }}">{{ key[0] }}</a>
             {% else %}
             FAILURE!
             <a href="{{ url_for('view_concept', curie=key) }}">{{ key }}</a>
             {% endif %}
             {%- else -%}
             {% if has_names %}{{ key[0] }}{% else %}{{ key }}{% endif %}
             {%- endif -%}
         </code></td>
-        {% if has_names %}<td>{{ key[1] }}</td>{% endif %}
+        {% if has_names %}
+        <td>{{ key[1] }}</td>
+        {% endif %}
         <td align="right">{{ "{:,}".format(count) }}</td>
     </tr>
     {% endfor %}
     </tbody>
 </table>
 {% endmacro %}
 
 {% block content %}
 <div class="container" style="margin-top: 50px; margin-bottom: 50px">
-    {{ util.render_messages(dismissible=True, container=False) }}
+    {{ bs_util.render_messages(dismissible=True, container=False) }}
     <div class="row justify-content-md-center">
         <div class="col-8">
             <div class="card">
                 <div class="card-body">
                     <h5 class="card-title">
                         Semantic Reasoning Assembler
                     </h5>
                     <div class="row text-center stats" style="padding-top: 1em; padding-bottom: 1em;">
                         {{ count_column(node_counter, "Concepts", "dna") }}
                         {{ count_column(node_counter, "Equivalence Classes", "dna") }}
                         {{ count_column(node_counter, "Mappings", "arrows-alt") }}
                         {{ count_column(node_counter, "Evidences", "book") }}
                         {{ count_column(node_counter, "Mapping Sets", "puzzle-piece") }}
                     </div>
+                    <p>See the <a href="/docs">API Documentation</a>.</p>
                     <h6>Mapping Sets</h6>
                 </div>
                 <table class="table">
                     <thead>
                     <tr>
                         <th>Name</th>
                         <th>Version</th>
@@ -104,22 +110,13 @@
                 {{ do_table(prefix_counter, "Prefix", has_names=True) }}
                 {{ do_table(author_counter, "Author", has_names=True) }}
                 {{ do_table(high_matches_counter, "Potential Data Issues", is_concept=True, has_names=True) }}
 
                 <div class="card-body">
                     <h6>Example Mappings</h6>
                 </div>
-                <ul class="list-group list-group-flush">
-                    {%- for example_mapping in example_mappings -%}
-                    <li class="list-group-item">
-                        <a href="{{ url_for('view_mapping', curie=example_mapping) }}">
-                            <code>{{ example_mapping[:8]}}</code>
-                        </a>
-                    </li>
-                    {%- endfor -%}
-                </ul>
+                {{ util.mapping_table(example_mappings) }}
             </div>
         </div>
     </div>
 </div>
-</div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-{% extends "base.html" %} {% import "bootstrap5/utils.html" as util %} {% block
-title %}SeMRA{% endblock %} {% macro count_column(counter, key, icon) -%}
+{% extends "base.html" %} {% import "bootstrap5/utils.html" as bs_util %} {%
+import "utils.html" as util %} {% block title %}SeMRA{% endblock %} {% macro
+count_column(counter, key, icon) -%}
 {% set count, suffix = format_number(counter[key]) %}
 ********** {{{{ ccoouunntt }}}}{{{{ ssuuffffiixx }}}} **********
 {{ key }}
 {% endmacro %} {% macro do_table(counter, label, is_concept=False,
 has_names=False) %}
 ** {{{{ llaabbeell }}}} SSuummmmaarryy **
 {{{{ llaabbeell }}}}                             NNaammee         CCoouunntt
 {%- if is_concept -%} {% if has_names
 %} _{_{_ _k_e_y_[_0_]_ _}_} {% else %} FAILURE! _{
 _{_ _k_e_y_ _}_} {% endif %} {%- else -%} {% if {{ key[1] }} {{ "{:,}".format(count) }}
 has_names %}{{ key[0] }}{% else %}{
 { key }}{% endif %} {%- endif -%}
 {% endmacro %} {% block content %}
-{{ util.render_messages(dismissible=True, container=False) }}
+{{ bs_util.render_messages(dismissible=True, container=False) }}
 **** SSeemmaannttiicc RReeaassoonniinngg AAsssseemmbblleerr ****
 {{ count_column(node_counter, "Concepts", "dna") }} {{ count_column
 (node_counter, "Equivalence Classes", "dna") }} {{ count_column(node_counter,
 "Mappings", "arrows-alt") }} {{ count_column(node_counter, "Evidences", "book")
 }} {{ count_column(node_counter, "Mapping Sets", "puzzle-piece") }}
+See the _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n.
 ** MMaappppiinngg SSeettss **
 NNaammee             VVeerrssiioonn             LLiicceennssee             CCoonnffiiddeennccee             EEvviiddeenncceess
                                                                                       {{ "{:,}".format
 Inferred         -                   -                   -                      (evidence_type_counter
                                                                                       ["reasoned"]) }}
                                      {% if
 _{                {                   mapping_set.license {                            {{ "{:,}".format
@@ -33,11 +35,9 @@
 {{ do_table(evidence_type_counter, "Evidence Type") }} {{ do_table
 (predicate_counter, "Predicate") }} {{ do_table(justification_counter, "Mapping
 Justification") }} {{ do_table(prefix_counter, "Prefix", has_names=True) }} {
 { do_table(author_counter, "Author", has_names=True) }} {{ do_table
 (high_matches_counter, "Potential Data Issues", is_concept=True,
 has_names=True) }}
 ** EExxaammppllee MMaappppiinnggss **
-    * {%- for example_mapping in example_mappings -%}
-    * _{_{_ _e_x_a_m_p_l_e___m_a_p_p_i_n_g_[_:_8_]_}_}
-    * {%- endfor -%}
+{{ util.mapping_table(example_mappings) }}
 {% endblock %}
```

### Comparing `semra-0.0.7/src/semra/templates/mapping.html` & `semra-0.0.8/src/semra/templates/mapping.html`

 * *Files 14% similar despite different names*

```diff
@@ -12,19 +12,19 @@
         <div class="card">
             <div class="card-body">
                 <h5 class="card-title">
                     Mapping <code>{{ mapping.curie["semra.mapping:" | length:][:8] }}</code>
                 </h5>
                 <dl>
                     <dt>Subject</dt>
-                    <dd><a href="https://bioregistry.io/{{ mapping.s.curie }}"><code>{{ mapping.s.curie }}</code></a></dd>
+                    <dd><a href="{{ url_for('view_concept', curie=mapping.s.curie) }}"><code>{{ mapping.s.curie }}</code></a></dd>
                     <dt>Predicate</dt>
-                    <dd><a href="https://bioregistry.io/{{ mapping.p.curie }}"><code>{{ mapping.p.curie }}</code></a></dd>
+                    <dd><code>{{ mapping.p.curie }}</code></dd>
                     <dt>Object</dt>
-                    <dd><a href="https://bioregistry.io/{{ mapping.o.curie }}"><code>{{ mapping.o.curie }}</code></a></dd>
+                    <dd><a href="{{ url_for('view_concept', curie=mapping.o.curie) }}"><code>{{ mapping.o.curie }}</code></a></dd>
                     <dt>Evidence</dt>
                     {%- for evidence in mapping.evidence -%}
                     <dd>
                         <code>{{ evidence.curie["semra.evidence:" | length:][:8] }}</code><br>
                         Confidence: {{ evidence.confidence}}<br>
                         Type: {{ evidence.evidence_type }}<br>
                         {% if evidence.author %}
```

### Comparing `semra-0.0.7/tests/test_api.py` & `semra-0.0.8/tests/test_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,71 @@
+"""Tests for the core SeMRA API."""
+
 from __future__ import annotations
 
 import typing as t
 import unittest
 
 from semra import api
 from semra.api import (
     BROAD_MATCH,
     DB_XREF,
     EXACT_MATCH,
     NARROW_MATCH,
     Index,
+    count_component_sizes,
+    count_coverage_sizes,
     filter_mappings,
     filter_self_matches,
     flip,
+    from_digraph,
     get_index,
     get_many_to_many,
     infer_chains,
     infer_mutations,
     infer_reversible,
     keep_prefixes,
     project,
+    to_digraph,
 )
 from semra.rules import KNOWLEDGE_MAPPING, MANUAL_MAPPING
-from semra.struct import Mapping, MappingSet, ReasonedEvidence, Reference, SimpleEvidence, line, triple_key
+from semra.struct import (
+    Mapping,
+    MappingSet,
+    ReasonedEvidence,
+    Reference,
+    SimpleEvidence,
+    line,
+    triple_key,
+)
 
 
-def _get_references(n: int, prefix: str = "test") -> t.List[Reference]:
-    return [Reference(prefix=prefix, identifier=str(i)) for i in range(1, n + 1)]
+def _get_references(n: int, *, prefix: str = "test", different_prefixes: bool = False) -> t.List[Reference]:
+    if different_prefixes:
+        prefixes = [f"{prefix}{i + 1}" for i in range(n)]
+    else:
+        prefixes = [prefix for _ in range(n)]
+    identifiers = [str(i + 1) for i in range(n)]
+    return [Reference(prefix=prefix, identifier=identifier) for prefix, identifier in zip(prefixes, identifiers)]
 
 
 def _exact(s, o, evidence: t.Optional[t.List[SimpleEvidence]] = None) -> Mapping:
     return Mapping(s=s, p=EXACT_MATCH, o=o, evidence=evidence or [])
 
 
 EV = SimpleEvidence(
     justification=MANUAL_MAPPING,
     mapping_set=MappingSet(name="test_mapping_set", confidence=0.95),
 )
 MS = MappingSet(name="test", confidence=0.95)
 
 
 class TestOperations(unittest.TestCase):
+    """Test mapping operations."""
+
     def test_path(self):
         """Test quickly creating mapping lists."""
         r1, r2, r3 = _get_references(3)
         m1 = Mapping(s=r1, p=EXACT_MATCH, o=r2)
         m2 = Mapping(s=r2, p=BROAD_MATCH, o=r3)
         self.assertEqual([m1], line(r1, EXACT_MATCH, r2))
         self.assertEqual([m1, m2], line(r1, EXACT_MATCH, r2, BROAD_MATCH, r3))
@@ -80,14 +101,15 @@
         actual = flip(broad_mapping)
         self.assertIsNotNone(actual)
         self.assertEqual(docetaxel_mesh, actual.s)
         self.assertEqual(NARROW_MATCH, actual.p)
         self.assertEqual(docetaxel_anhydrous_chebi, actual.o)
 
     def test_index(self):
+        """Test indexing semantic mappings."""
         r1, r2 = _get_references(2)
         e1 = SimpleEvidence(justification=Reference(prefix="semapv", identifier="LexicalMatching"), mapping_set=MS)
         e2 = SimpleEvidence(
             justification=Reference(prefix="semapv", identifier="ManualMappingCuration"), mapping_set=MS
         )
         m1 = Mapping(s=r1, p=EXACT_MATCH, o=r2, evidence=[e1])
         m2 = Mapping(s=r1, p=EXACT_MATCH, o=r2, evidence=[e2])
@@ -121,15 +143,15 @@
     @staticmethod
     def _clean_index(index: Index) -> t.List[str]:
         triples = sorted(set(index), key=triple_key)
         return ["<" + ", ".join(element.curie for element in triple) + ">" for triple in triples]
 
     def test_infer_exact_match(self):
         """Test inference through the transitivity of SKOS exact matches."""
-        r1, r2, r3, r4 = _get_references(4)
+        r1, r2, r3, r4 = _get_references(4, different_prefixes=True)
         m1, m2, m3 = line(r1, EXACT_MATCH, r2, EXACT_MATCH, r3, EXACT_MATCH, r4)
         m4 = _exact(r1, r3)
         m5 = _exact(r1, r4)
         m6 = _exact(r2, r4)
         m4_inv, m5_inv, m6_inv = (flip(m) for m in (m4, m5, m6))
 
         backwards_msg = "backwards inference is not supposed to be done here"
@@ -162,15 +184,16 @@
         # ------ Same but in reverse ---------
         m1, m2 = line(r1, BROAD_MATCH, r2, NARROW_MATCH, r3)
         self.assert_same_triples(
             [m1, m2], infer_chains([m1, m2], progress=False), msg="No inference between broad and narrow"
         )
 
     def test_infer_broad_match_1(self):
-        r1, r2, r3, r4 = _get_references(4)
+        """Test inferring broad matches."""
+        r1, r2, r3, r4 = _get_references(4, different_prefixes=True)
         m1, m2, m3 = line(r1, EXACT_MATCH, r2, BROAD_MATCH, r3, EXACT_MATCH, r4)
         m4 = Mapping(s=r1, p=BROAD_MATCH, o=r3, evidence=[EV])
         m5 = Mapping(s=r1, p=BROAD_MATCH, o=r4, evidence=[EV])
         m6 = Mapping(s=r2, p=BROAD_MATCH, o=r4, evidence=[EV])
         m4_i = Mapping(o=r1, p=NARROW_MATCH, s=r3, evidence=[EV])
         m5_i = Mapping(o=r1, p=NARROW_MATCH, s=r4, evidence=[EV])
         m6_i = Mapping(o=r2, p=NARROW_MATCH, s=r4, evidence=[EV])
@@ -195,15 +218,16 @@
         self.assert_same_triples(
             [m1, m2, m3, m4, m5, m6, m4_i, m5_i, m6_i],
             infer_chains([m1, m2, m3], backwards=True, progress=False),
             msg="inference over multiple steps is broken",
         )
 
     def test_infer_broad_match_2(self):
-        r1, r2, r3, r4 = _get_references(4)
+        """Test inferring broad matches."""
+        r1, r2, r3, r4 = _get_references(4, different_prefixes=True)
         m1, m2, m3 = line(r1, BROAD_MATCH, r2, EXACT_MATCH, r3, BROAD_MATCH, r4)
         m4 = Mapping(s=r1, p=BROAD_MATCH, o=r3)
         m5 = Mapping(s=r1, p=BROAD_MATCH, o=r4)
         m6 = Mapping(s=r2, p=BROAD_MATCH, o=r4)
         m4_i = Mapping(o=r1, p=NARROW_MATCH, s=r3)
         m5_i = Mapping(o=r1, p=NARROW_MATCH, s=r4)
         m6_i = Mapping(o=r2, p=NARROW_MATCH, s=r4)
@@ -215,23 +239,25 @@
         # Check inference over multiple steps
         self.assert_same_triples([m1, m2, m3, m4, m5, m6], infer_chains([m1, m2, m3], backwards=False, progress=False))
         self.assert_same_triples(
             [m1, m2, m3, m4, m5, m6, m4_i, m5_i, m6_i], infer_chains([m1, m2, m3], backwards=True, progress=False)
         )
 
     def test_infer_narrow_match(self):
-        r1, r2, r3 = _get_references(3)
+        """Test inferring narrow matches."""
+        r1, r2, r3 = _get_references(3, different_prefixes=True)
         m1, m2 = line(r1, EXACT_MATCH, r2, NARROW_MATCH, r3)
         m3 = Mapping(s=r1, p=NARROW_MATCH, o=r3)
         m3_i = Mapping(o=r1, p=BROAD_MATCH, s=r3)
         self.assert_same_triples([m1, m2, m3], infer_chains([m1, m2], backwards=False, progress=False))
         self.assert_same_triples([m1, m2, m3, m3_i], infer_chains([m1, m2], backwards=True, progress=False))
 
     def test_mixed_inference_1(self):
-        r1, r2, r3 = _get_references(3)
+        """Test inferring over a mix of narrow, broad, and exact matches."""
+        r1, r2, r3 = _get_references(3, different_prefixes=True)
         m1 = Mapping(s=r1, p=EXACT_MATCH, o=r2)
         m2 = Mapping(s=r2, p=NARROW_MATCH, o=r3)
         m3 = Mapping(s=r1, p=NARROW_MATCH, o=r3)
 
         m4 = Mapping(s=r2, p=EXACT_MATCH, o=r1)
         m5 = Mapping(s=r3, p=BROAD_MATCH, o=r2)
         m6 = Mapping(s=r3, p=BROAD_MATCH, o=r1)
@@ -305,27 +331,81 @@
         (a1, a2) = _get_references(2, prefix="a")
         (b1, b2) = _get_references(2, prefix="b")
         m1 = Mapping(s=a1, p=DB_XREF, o=b1, evidence=[SimpleEvidence(confidence=0.95, mapping_set=MS)])
         m2 = Mapping(s=a1, p=DB_XREF, o=b1, evidence=[SimpleEvidence(confidence=0.65, mapping_set=MS)])
         mmm = list(api.filter_minimum_confidence([m1, m2], cutoff=0.7))
         self.assertEqual([m1], mmm)
 
+    def test_filter_subsets(self):
+        """Test filtering by subsets."""
+        a1, a2 = _get_references(2, prefix="a")
+        b1, b2 = _get_references(2, prefix="b")
+        c1, c2 = _get_references(2, prefix="c")
+        ev = SimpleEvidence(confidence=0.95, mapping_set=MS)
+        m1 = Mapping(s=a1, p=EXACT_MATCH, o=b1, evidence=[ev])
+        m2 = Mapping(s=b1, p=EXACT_MATCH, o=a1, evidence=[ev])
+        m3 = Mapping(s=a2, p=EXACT_MATCH, o=b2, evidence=[ev])
+        m4 = Mapping(s=b2, p=EXACT_MATCH, o=a2, evidence=[ev])
+        m5 = Mapping(s=b1, p=EXACT_MATCH, o=c1, evidence=[ev])
+        m6 = Mapping(s=c1, p=EXACT_MATCH, o=b1, evidence=[ev])
+
+        terms = {"a": ["1", "2"], "b": ["1"]}
+        mmm = list(api.filter_subsets([m1, m2, m3, m4, m5, m6], terms))
+        self.assertEqual(
+            [m1, m2, m5, m6], mmm, msg="Mappings 3 and 4 should not pass since b2 is not in the term filter"
+        )
+
+        terms = {"a": ["1", "2"], "b": ["1"], "c": []}
+        # the fact that c has an empty dictionary will get ignored
+        mmm = list(api.filter_subsets([m1, m2, m3, m4, m5, m6], terms))
+        self.assertEqual(
+            [m1, m2, m5, m6], mmm, msg="Mappings 3 and 4 should not pass since b2 is not in the term filter"
+        )
+
+    def test_count_component_sizes(self):
+        """Test counting component sizes."""
+        priority = "abc"
+        a1, a2 = _get_references(2, prefix="a")
+        b1, b2 = _get_references(2, prefix="b")
+        c1, _ = _get_references(2, prefix="c")
+        ev = SimpleEvidence(confidence=0.95, mapping_set=MS)
+        m1 = Mapping(s=a1, p=EXACT_MATCH, o=b1, evidence=[ev])
+        m2 = Mapping(s=b1, p=EXACT_MATCH, o=c1, evidence=[ev])
+        m3 = Mapping(s=a2, p=EXACT_MATCH, o=b2, evidence=[ev])
+        m4 = Mapping(s=a2, p=DB_XREF, o=b2, evidence=[ev])  # this shouldn't hae an effect
+        mappings = [m1, m2, m3, m4]
+        self.assertEqual({frozenset("ab"): 1, frozenset("abc"): 1}, dict(count_component_sizes(mappings, priority)))
+        self.assertEqual({1: 0, 2: 1, 3: 1}, dict(count_coverage_sizes(mappings, priority)))
+
+    def test_digraph_roundtrip(self):
+        """Test I/O roundtrip through a directed graph."""
+        a1, a2 = _get_references(2, prefix="a")
+        b1, b2 = _get_references(2, prefix="b")
+        c1, _ = _get_references(2, prefix="c")
+        ev = SimpleEvidence(confidence=0.95, mapping_set=MS)
+        m1 = Mapping(s=a1, p=EXACT_MATCH, o=b1, evidence=[ev])
+        m2 = Mapping(s=b1, p=EXACT_MATCH, o=c1, evidence=[ev])
+        m3 = Mapping(s=a2, p=EXACT_MATCH, o=b2, evidence=[ev])
+        m4 = Mapping(s=a2, p=DB_XREF, o=b2, evidence=[ev])  # this shouldn't hae an effect
+        mappings = [m1, m2, m3, m4]
+        self.assertEqual(mappings, from_digraph(to_digraph(mappings)))
+
 
 class TestUpgrades(unittest.TestCase):
     """Test inferring mutations."""
 
     def test_infer_mutations(self):
         """Test inferring mutations."""
         (a1,) = _get_references(1, prefix="a")
         (b1,) = _get_references(1, prefix="b")
         original_confidence = 0.95
         mutation_confidence = 0.80
         m1 = Mapping(s=a1, p=DB_XREF, o=b1, evidence=[SimpleEvidence(confidence=original_confidence, mapping_set=MS)])
         new_mappings = infer_mutations(
-            [m1], {("a", "b"): mutation_confidence}, old=DB_XREF, new=EXACT_MATCH, progress=False
+            [m1], {("a", "b"): mutation_confidence}, old_predicate=DB_XREF, new_predicate=EXACT_MATCH, progress=False
         )
         self.assertEqual(2, len(new_mappings))
         new_m1, new_m2 = new_mappings
         self.assertEqual(m1, new_m1)
         self.assertEqual(a1, new_m2.s)
         self.assertEqual(EXACT_MATCH, new_m2.p)
         self.assertEqual(b1, new_m2.o)
```

### Comparing `semra-0.0.7/tests/test_pipeline.py` & `semra-0.0.8/tests/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,19 @@
             )
         ],
     )
 ]
 
 
 def get_test_mappings() -> t.List[Mapping]:
-    """A test function to get mappings."""
+    """Get test mappings."""
     return TEST_MAPPINGS
 
 
+# Register a function for getting test mappings in order to test the way Inputs are handled
 SOURCE_RESOLVER.register(get_test_mappings)
 
 
 class TestPipeline(unittest.TestCase):
     """Test case for the automated assembly pipeline."""
 
     def assert_test_mappings(self, mappings):
```

