# Comparing `tmp/ligo-1.0.2.tar.gz` & `tmp/ligo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-1.0.2.tar", last modified: Fri Nov  3 09:30:16 2023, max compression
+gzip compressed data, was "ligo-1.0.3.tar", last modified: Thu Apr 11 17:34:35 2024, max compression
```

## Comparing `ligo-1.0.2.tar` & `ligo-1.0.3.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.775344 ligo-1.0.2/
--rw-r--r--   0 milenpa    (502) staff       (20)    34523 2023-06-21 13:16:03.000000 ligo-1.0.2/LICENSE.md
--rw-r--r--   0 milenpa    (502) staff       (20)     3849 2023-11-03 09:30:16.775118 ligo-1.0.2/PKG-INFO
--rw-r--r--   0 milenpa    (502) staff       (20)     3086 2023-10-11 12:49:47.000000 ligo-1.0.2/README.md
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.746048 ligo-1.0.2/ligo/
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.747112 ligo-1.0.2/ligo/IO/
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.748035 ligo-1.0.2/ligo/IO/dataset_export/
--rw-r--r--   0 milenpa    (502) staff       (20)    11333 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/IO/dataset_export/AIRRExporter.py
--rw-r--r--   0 milenpa    (502) staff       (20)      310 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/IO/dataset_export/DataExporter.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5648 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_export/ImmuneMLExporter.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_export/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.750616 ligo-1.0.2/ligo/IO/dataset_import/
--rw-r--r--   0 milenpa    (502) staff       (20)    12239 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/AIRRImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)      243 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/DataImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1680 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/DatasetImportParams.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10228 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/GenericImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10316 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/IGoRImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    20507 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/IReceptorImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)     6592 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/ImmuneMLImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10193 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/ImmunoSEQRearrangementImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10091 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/ImmunoSEQSampleImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10549 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/MiXCRImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)     6411 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/OLGAImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    11299 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/SingleLineReceptorImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10455 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/TenxGenomicsImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)    12139 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/VDJdbImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.750731 ligo-1.0.2/ligo/IO/dataset_import/conversion/
--rw-r--r--   0 milenpa    (502) staff       (20)    14265 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
--rw-r--r--   0 milenpa    (502) staff       (20)       82 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.751029 ligo-1.0.2/ligo/app/
--rw-r--r--   0 milenpa    (502) staff       (20)     2704 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/app/LigoApp.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/app/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.742902 ligo-1.0.2/ligo/config/
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.743067 ligo-1.0.2/ligo/config/default_params/
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.753147 ligo-1.0.2/ligo/config/default_params/datasets/
--rw-r--r--   0 milenpa    (502) staff       (20)      634 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/airr_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      424 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/generic_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      637 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/i_receptor_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      587 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/igor_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)     1109 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)     1145 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/immuno_seq_sample_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      746 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/mixcr_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      608 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/olga_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      170 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/random_receptor_dataset_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      723 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/random_repertoire_dataset_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)       93 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/random_sequence_dataset_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      803 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/tenx_genomics_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      619 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/datasets/vdjdb_params.yaml
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.753449 ligo-1.0.2/ligo/config/default_params/instructions/
--rw-r--r--   0 milenpa    (502) staff       (20)       44 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/config/default_params/instructions/feasibility_summary_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)       69 2023-10-11 12:34:16.000000 ligo-1.0.2/ligo/config/default_params/instructions/ligo_sim_params.yaml
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.753730 ligo-1.0.2/ligo/config/default_params/simulation/
--rw-r--r--   0 milenpa    (502) staff       (20)      248 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/config/default_params/simulation/ligo_sim_config_item_params.yaml
--rw-r--r--   0 milenpa    (502) staff       (20)      200 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/config/default_params/simulation/ligo_sim_config_params.yaml
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.754035 ligo-1.0.2/ligo/data_model/
--rw-r--r--   0 milenpa    (502) staff       (20)      133 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/DatasetItem.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.754465 ligo-1.0.2/ligo/data_model/cell/
--rw-r--r--   0 milenpa    (502) staff       (20)      396 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/cell/Cell.py
--rw-r--r--   0 milenpa    (502) staff       (20)      703 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/cell/CellList.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/cell/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.755472 ligo-1.0.2/ligo/data_model/dataset/
--rw-r--r--   0 milenpa    (502) staff       (20)     1304 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/dataset/Dataset.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4456 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/data_model/dataset/ElementDataset.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2841 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/dataset/ReceptorDataset.py
--rw-r--r--   0 milenpa    (502) staff       (20)    10381 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/data_model/dataset/RepertoireDataset.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2931 2023-08-24 09:43:03.000000 ligo-1.0.2/ligo/data_model/dataset/SequenceDataset.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/dataset/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.755742 ligo-1.0.2/ligo/data_model/encoded_data/
--rw-r--r--   0 milenpa    (502) staff       (20)     2372 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/encoded_data/EncodedData.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/encoded_data/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.757521 ligo-1.0.2/ligo/data_model/receptor/
--rw-r--r--   0 milenpa    (502) staff       (20)     1958 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/BCKReceptor.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1968 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/BCReceptor.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1245 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/ChainPair.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5897 2023-09-14 15:39:47.000000 ligo-1.0.2/ligo/data_model/receptor/ElementGenerator.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1454 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/Receptor.py
--rw-r--r--   0 milenpa    (502) staff       (20)     3154 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/ReceptorBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)      309 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/RegionType.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1981 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/TCABReceptor.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1992 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/TCGDReceptor.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.758449 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/
--rw-r--r--   0 milenpa    (502) staff       (20)      957 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/Chain.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5456 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/ReceptorSequence.py
--rw-r--r--   0 milenpa    (502) staff       (20)      636 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/SequenceAnnotation.py
--rw-r--r--   0 milenpa    (502) staff       (20)      153 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/SequenceFrameType.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1821 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/SequenceMetadata.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.758737 ligo-1.0.2/ligo/data_model/repertoire/
--rw-r--r--   0 milenpa    (502) staff       (20)    18070 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/repertoire/Repertoire.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/data_model/repertoire/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.759718 ligo-1.0.2/ligo/dsl/
--rw-r--r--   0 milenpa    (502) staff       (20)     1902 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/DefaultParamsLoader.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5631 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/InstructionParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)     7909 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/dsl/LigoParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)     3871 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/ObjectParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1073 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/OutputParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)      139 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/Parser.py
--rw-r--r--   0 milenpa    (502) staff       (20)      835 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/Util.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.760936 ligo-1.0.2/ligo/dsl/definition_parsers/
--rw-r--r--   0 milenpa    (502) staff       (20)     3563 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/definition_parsers/DefinitionParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)      515 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/definition_parsers/DefinitionParserOutput.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2721 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/definition_parsers/MotifParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)     3918 2023-08-27 15:14:03.000000 ligo-1.0.2/ligo/dsl/definition_parsers/SignalParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)    14057 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/dsl/definition_parsers/SimulationParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/definition_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.761201 ligo-1.0.2/ligo/dsl/import_parsers/
--rw-r--r--   0 milenpa    (502) staff       (20)     4281 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/import_parsers/ImportParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/import_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.761698 ligo-1.0.2/ligo/dsl/instruction_parsers/
--rw-r--r--   0 milenpa    (502) staff       (20)     1417 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/instruction_parsers/FeasibilitySummaryParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1853 2023-10-11 12:44:39.000000 ligo-1.0.2/ligo/dsl/instruction_parsers/LigoSimParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/instruction_parsers/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.762072 ligo-1.0.2/ligo/dsl/semantic_model/
--rw-r--r--   0 milenpa    (502) staff       (20)       72 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/semantic_model/MLResult.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1870 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/semantic_model/SemanticModel.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/semantic_model/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.762595 ligo-1.0.2/ligo/dsl/symbol_table/
--rw-r--r--   0 milenpa    (502) staff       (20)     2505 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/symbol_table/SymbolTable.py
--rw-r--r--   0 milenpa    (502) staff       (20)      294 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/symbol_table/SymbolTableEntry.py
--rw-r--r--   0 milenpa    (502) staff       (20)      220 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/symbol_table/SymbolType.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/dsl/symbol_table/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.763118 ligo-1.0.2/ligo/environment/
--rw-r--r--   0 milenpa    (502) staff       (20)      413 2023-11-03 09:29:02.000000 ligo-1.0.2/ligo/environment/Constants.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2510 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/environment/EnvironmentSettings.py
--rw-r--r--   0 milenpa    (502) staff       (20)      109 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/environment/SequenceType.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/environment/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.763747 ligo-1.0.2/ligo/presentation/
--rw-r--r--   0 milenpa    (502) staff       (20)      170 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/InstructionPresentation.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1048 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/PresentationFactory.py
--rw-r--r--   0 milenpa    (502) staff       (20)       74 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/PresentationFormat.py
--rw-r--r--   0 milenpa    (502) staff       (20)      456 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/TemplateParser.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.764749 ligo-1.0.2/ligo/presentation/html/
--rw-r--r--   0 milenpa    (502) staff       (20)     3115 2023-08-24 11:36:23.000000 ligo-1.0.2/ligo/presentation/html/FeasibilitySummaryHTMLBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)     3348 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/html/HTMLBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2918 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/presentation/html/LIgOSimulationHTMLBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4745 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/presentation/html/Util.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/html/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.765291 ligo-1.0.2/ligo/presentation/html/templates/
--rw-r--r--   0 milenpa    (502) staff       (20)     2940 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/html/templates/DatasetExport.html
--rw-r--r--   0 milenpa    (502) staff       (20)    10629 2023-08-24 11:36:23.000000 ligo-1.0.2/ligo/presentation/html/templates/FeasibilitySummary.html
--rw-r--r--   0 milenpa    (502) staff       (20)     3539 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/presentation/html/templates/Simulation.html
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.765443 ligo-1.0.2/ligo/presentation/html/templates/css/
--rw-r--r--   0 milenpa    (502) staff       (20)     2562 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/html/templates/css/custom.css
--rw-r--r--   0 milenpa    (502) staff       (20)      705 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/presentation/html/templates/index.html
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.766424 ligo-1.0.2/ligo/simulation/
--rw-r--r--   0 milenpa    (502) staff       (20)      590 2023-10-11 12:34:16.000000 ligo-1.0.2/ligo/simulation/LigoSimState.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4583 2023-10-12 11:29:25.000000 ligo-1.0.2/ligo/simulation/SimConfig.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4998 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/SimConfigItem.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.766641 ligo-1.0.2/ligo/simulation/dataset_generation/
--rw-r--r--   0 milenpa    (502) staff       (20)    14380 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/dataset_generation/RandomDatasetGenerator.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/dataset_generation/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.767532 ligo-1.0.2/ligo/simulation/generative_models/
--rw-r--r--   0 milenpa    (502) staff       (20)     1767 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/generative_models/BackgroundSequences.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4713 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/generative_models/ExperimentalImport.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1231 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/generative_models/GenerativeModel.py
--rw-r--r--   0 milenpa    (502) staff       (20)      510 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/generative_models/InternalOlgaModel.py
--rw-r--r--   0 milenpa    (502) staff       (20)    11754 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/generative_models/OLGA.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/generative_models/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.768501 ligo-1.0.2/ligo/simulation/implants/
--rw-r--r--   0 milenpa    (502) staff       (20)      274 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/implants/ImplantAnnotation.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2589 2023-08-23 13:10:09.000000 ligo-1.0.2/ligo/simulation/implants/LigoPWM.py
--rw-r--r--   0 milenpa    (502) staff       (20)      642 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/implants/Motif.py
--rw-r--r--   0 milenpa    (502) staff       (20)      734 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/implants/MotifInstance.py
--rw-r--r--   0 milenpa    (502) staff       (20)     9917 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/implants/SeedMotif.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5918 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/implants/Signal.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/implants/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.769255 ligo-1.0.2/ligo/simulation/simulation_strategy/
--rw-r--r--   0 milenpa    (502) staff       (20)    11537 2023-10-11 12:58:39.000000 ligo-1.0.2/ligo/simulation/simulation_strategy/ImplantingStrategy.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1449 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/simulation_strategy/RejectionSamplingStrategy.py
--rw-r--r--   0 milenpa    (502) staff       (20)      606 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/simulation_strategy/SimulationStrategy.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/simulation_strategy/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.769814 ligo-1.0.2/ligo/simulation/util/
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/util/__init__.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4089 2023-08-22 22:11:56.000000 ligo-1.0.2/ligo/simulation/util/bnp_util.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5363 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/simulation/util/igor_helper.py
--rw-r--r--   0 milenpa    (502) staff       (20)    26794 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/simulation/util/util.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.772143 ligo-1.0.2/ligo/util/
--rw-r--r--   0 milenpa    (502) staff       (20)     3767 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/AdaptiveImportHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)      448 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/DistanceMetrics.py
--rw-r--r--   0 milenpa    (502) staff       (20)      405 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/DocEnumHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)      761 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/util/ExporterHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1157 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/FilenameHandler.py
--rw-r--r--   0 milenpa    (502) staff       (20)    26271 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/ImportHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1199 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/Logger.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1043 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/NameBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1602 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/NumpyHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)     5877 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/util/ParameterValidator.py
--rw-r--r--   0 milenpa    (502) staff       (20)      776 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/PathBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)     6510 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/util/PositionHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)       85 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/ReadsType.py
--rw-r--r--   0 milenpa    (502) staff       (20)     4112 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/ReflectionHandler.py
--rw-r--r--   0 milenpa    (502) staff       (20)     2676 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/RepertoireBuilder.py
--rw-r--r--   0 milenpa    (502) staff       (20)      593 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/Reports.py
--rw-r--r--   0 milenpa    (502) staff       (20)      401 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/StringHelper.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/util/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.772236 ligo-1.0.2/ligo/workflows/
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/workflows/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.772507 ligo-1.0.2/ligo/workflows/instructions/
--rw-r--r--   0 milenpa    (502) staff       (20)      156 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/workflows/instructions/Instruction.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/workflows/instructions/__init__.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.773254 ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/
--rw-r--r--   0 milenpa    (502) staff       (20)    12647 2023-10-12 11:20:23.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/__init__.py
--rw-r--r--   0 milenpa    (502) staff       (20)     7417 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.773991 ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/
--rw-r--r--   0 milenpa    (502) staff       (20)    23974 2023-10-12 11:37:01.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/LigoSimInstruction.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/__init__.py
--rw-r--r--   0 milenpa    (502) staff       (20)      794 2023-10-02 11:57:55.000000 ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/runtime_reports.py
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.746975 ligo-1.0.2/ligo.egg-info/
--rw-r--r--   0 milenpa    (502) staff       (20)     3849 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/PKG-INFO
--rw-r--r--   0 milenpa    (502) staff       (20)     7529 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/SOURCES.txt
--rw-r--r--   0 milenpa    (502) staff       (20)        1 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/dependency_links.txt
--rw-r--r--   0 milenpa    (502) staff       (20)       47 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/entry_points.txt
--rw-r--r--   0 milenpa    (502) staff       (20)      110 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/requires.txt
--rw-r--r--   0 milenpa    (502) staff       (20)       13 2023-11-03 09:30:16.000000 ligo-1.0.2/ligo.egg-info/top_level.txt
-drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2023-11-03 09:30:16.774784 ligo-1.0.2/scripts/
--rw-r--r--   0 milenpa    (502) staff       (20)      326 2023-06-21 13:16:03.000000 ligo-1.0.2/scripts/DocumentatonFormat.py
--rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.2/scripts/__init__.py
--rw-r--r--   0 milenpa    (502) staff       (20)     1303 2023-06-21 13:16:03.000000 ligo-1.0.2/scripts/specification_util.py
--rw-r--r--   0 milenpa    (502) staff       (20)      702 2023-06-21 13:16:03.000000 ligo-1.0.2/scripts/specs_docs_generation.py
--rw-r--r--   0 milenpa    (502) staff       (20)       38 2023-11-03 09:30:16.775385 ligo-1.0.2/setup.cfg
--rw-r--r--   0 milenpa    (502) staff       (20)     1391 2023-11-03 09:22:59.000000 ligo-1.0.2/setup.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.484327 ligo-1.0.3/
+-rw-r--r--   0 milenpa    (502) staff       (20)    34523 2023-06-21 13:16:03.000000 ligo-1.0.3/LICENSE.md
+-rw-r--r--   0 milenpa    (502) staff       (20)     4429 2024-04-11 17:34:35.484109 ligo-1.0.3/PKG-INFO
+-rw-r--r--   0 milenpa    (502) staff       (20)     3666 2024-04-11 17:24:57.000000 ligo-1.0.3/README.md
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.456894 ligo-1.0.3/ligo/
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.457975 ligo-1.0.3/ligo/IO/
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.458907 ligo-1.0.3/ligo/IO/dataset_export/
+-rw-r--r--   0 milenpa    (502) staff       (20)    11333 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/IO/dataset_export/AIRRExporter.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      310 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/IO/dataset_export/DataExporter.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5648 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_export/ImmuneMLExporter.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_export/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.461699 ligo-1.0.3/ligo/IO/dataset_import/
+-rw-r--r--   0 milenpa    (502) staff       (20)    12239 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/AIRRImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      243 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/DataImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1680 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/DatasetImportParams.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10228 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/GenericImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10316 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/IGoRImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    20507 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/IReceptorImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     6592 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/ImmuneMLImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10193 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/ImmunoSEQRearrangementImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10091 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/ImmunoSEQSampleImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10549 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/MiXCRImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     6411 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/OLGAImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    11299 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/SingleLineReceptorImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10455 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/TenxGenomicsImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    12139 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/VDJdbImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.461830 ligo-1.0.3/ligo/IO/dataset_import/conversion/
+-rw-r--r--   0 milenpa    (502) staff       (20)    14265 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
+-rw-r--r--   0 milenpa    (502) staff       (20)       82 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.462171 ligo-1.0.3/ligo/app/
+-rw-r--r--   0 milenpa    (502) staff       (20)     2704 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/app/LigoApp.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/app/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.453519 ligo-1.0.3/ligo/config/
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.453678 ligo-1.0.3/ligo/config/default_params/
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.464193 ligo-1.0.3/ligo/config/default_params/datasets/
+-rw-r--r--   0 milenpa    (502) staff       (20)      634 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/airr_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      424 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/generic_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      637 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/i_receptor_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      587 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/igor_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)     1109 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)     1145 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/immuno_seq_sample_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      746 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/mixcr_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      608 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/olga_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      170 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/random_receptor_dataset_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      723 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/random_repertoire_dataset_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)       93 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/random_sequence_dataset_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      803 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/tenx_genomics_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      619 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/datasets/vdjdb_params.yaml
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.464462 ligo-1.0.3/ligo/config/default_params/instructions/
+-rw-r--r--   0 milenpa    (502) staff       (20)       44 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/config/default_params/instructions/feasibility_summary_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)       69 2023-10-11 12:34:16.000000 ligo-1.0.3/ligo/config/default_params/instructions/ligo_sim_params.yaml
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.464833 ligo-1.0.3/ligo/config/default_params/simulation/
+-rw-r--r--   0 milenpa    (502) staff       (20)      248 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/config/default_params/simulation/ligo_sim_config_item_params.yaml
+-rw-r--r--   0 milenpa    (502) staff       (20)      200 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/config/default_params/simulation/ligo_sim_config_params.yaml
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.465080 ligo-1.0.3/ligo/data_model/
+-rw-r--r--   0 milenpa    (502) staff       (20)      133 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/DatasetItem.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.465470 ligo-1.0.3/ligo/data_model/cell/
+-rw-r--r--   0 milenpa    (502) staff       (20)      396 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/cell/Cell.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      703 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/cell/CellList.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/cell/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.466417 ligo-1.0.3/ligo/data_model/dataset/
+-rw-r--r--   0 milenpa    (502) staff       (20)     1304 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/dataset/Dataset.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4456 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/data_model/dataset/ElementDataset.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2841 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/dataset/ReceptorDataset.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    10381 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/data_model/dataset/RepertoireDataset.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2931 2023-08-24 09:43:03.000000 ligo-1.0.3/ligo/data_model/dataset/SequenceDataset.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/dataset/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.466652 ligo-1.0.3/ligo/data_model/encoded_data/
+-rw-r--r--   0 milenpa    (502) staff       (20)     2372 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/encoded_data/EncodedData.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/encoded_data/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.468051 ligo-1.0.3/ligo/data_model/receptor/
+-rw-r--r--   0 milenpa    (502) staff       (20)     1958 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/BCKReceptor.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1968 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/BCReceptor.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1245 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/ChainPair.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5897 2023-09-14 15:39:47.000000 ligo-1.0.3/ligo/data_model/receptor/ElementGenerator.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1454 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/Receptor.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     3154 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/ReceptorBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      309 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/RegionType.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1981 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/TCABReceptor.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1992 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/TCGDReceptor.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.468864 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/
+-rw-r--r--   0 milenpa    (502) staff       (20)      957 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/Chain.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5456 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/ReceptorSequence.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      636 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/SequenceAnnotation.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      153 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/SequenceFrameType.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1821 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/SequenceMetadata.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.469131 ligo-1.0.3/ligo/data_model/repertoire/
+-rw-r--r--   0 milenpa    (502) staff       (20)    18070 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/repertoire/Repertoire.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/data_model/repertoire/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.470257 ligo-1.0.3/ligo/dsl/
+-rw-r--r--   0 milenpa    (502) staff       (20)     1902 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/DefaultParamsLoader.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5631 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/InstructionParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     7909 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/dsl/LigoParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     3871 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/ObjectParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1073 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/OutputParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      139 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/Parser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      835 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/Util.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.471222 ligo-1.0.3/ligo/dsl/definition_parsers/
+-rw-r--r--   0 milenpa    (502) staff       (20)     3563 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/definition_parsers/DefinitionParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      515 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/definition_parsers/DefinitionParserOutput.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2721 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/definition_parsers/MotifParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     3918 2023-08-27 15:14:03.000000 ligo-1.0.3/ligo/dsl/definition_parsers/SignalParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    14057 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/dsl/definition_parsers/SimulationParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/definition_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.471453 ligo-1.0.3/ligo/dsl/import_parsers/
+-rw-r--r--   0 milenpa    (502) staff       (20)     4281 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/import_parsers/ImportParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/import_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.471871 ligo-1.0.3/ligo/dsl/instruction_parsers/
+-rw-r--r--   0 milenpa    (502) staff       (20)     1417 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/instruction_parsers/FeasibilitySummaryParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1853 2023-10-11 12:44:39.000000 ligo-1.0.3/ligo/dsl/instruction_parsers/LigoSimParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/instruction_parsers/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.472186 ligo-1.0.3/ligo/dsl/semantic_model/
+-rw-r--r--   0 milenpa    (502) staff       (20)       72 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/semantic_model/MLResult.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1870 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/semantic_model/SemanticModel.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/semantic_model/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.472665 ligo-1.0.3/ligo/dsl/symbol_table/
+-rw-r--r--   0 milenpa    (502) staff       (20)     2505 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/symbol_table/SymbolTable.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      294 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/symbol_table/SymbolTableEntry.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      220 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/symbol_table/SymbolType.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/dsl/symbol_table/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.473174 ligo-1.0.3/ligo/environment/
+-rw-r--r--   0 milenpa    (502) staff       (20)      413 2024-04-11 17:24:43.000000 ligo-1.0.3/ligo/environment/Constants.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2510 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/environment/EnvironmentSettings.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      109 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/environment/SequenceType.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/environment/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.473918 ligo-1.0.3/ligo/presentation/
+-rw-r--r--   0 milenpa    (502) staff       (20)      170 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/InstructionPresentation.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1048 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/PresentationFactory.py
+-rw-r--r--   0 milenpa    (502) staff       (20)       74 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/PresentationFormat.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      456 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/TemplateParser.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.474736 ligo-1.0.3/ligo/presentation/html/
+-rw-r--r--   0 milenpa    (502) staff       (20)     3115 2023-08-24 11:36:23.000000 ligo-1.0.3/ligo/presentation/html/FeasibilitySummaryHTMLBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     3348 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/html/HTMLBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2918 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/presentation/html/LIgOSimulationHTMLBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4745 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/presentation/html/Util.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/html/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.475515 ligo-1.0.3/ligo/presentation/html/templates/
+-rw-r--r--   0 milenpa    (502) staff       (20)     2940 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/html/templates/DatasetExport.html
+-rw-r--r--   0 milenpa    (502) staff       (20)    10629 2023-08-24 11:36:23.000000 ligo-1.0.3/ligo/presentation/html/templates/FeasibilitySummary.html
+-rw-r--r--   0 milenpa    (502) staff       (20)     3539 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/presentation/html/templates/Simulation.html
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.475682 ligo-1.0.3/ligo/presentation/html/templates/css/
+-rw-r--r--   0 milenpa    (502) staff       (20)     2562 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/html/templates/css/custom.css
+-rw-r--r--   0 milenpa    (502) staff       (20)      705 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/presentation/html/templates/index.html
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.476495 ligo-1.0.3/ligo/simulation/
+-rw-r--r--   0 milenpa    (502) staff       (20)      590 2023-10-11 12:34:16.000000 ligo-1.0.3/ligo/simulation/LigoSimState.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4583 2023-10-12 11:29:25.000000 ligo-1.0.3/ligo/simulation/SimConfig.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4998 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/SimConfigItem.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.476745 ligo-1.0.3/ligo/simulation/dataset_generation/
+-rw-r--r--   0 milenpa    (502) staff       (20)    14380 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/dataset_generation/RandomDatasetGenerator.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/dataset_generation/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.477460 ligo-1.0.3/ligo/simulation/generative_models/
+-rw-r--r--   0 milenpa    (502) staff       (20)     1767 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/generative_models/BackgroundSequences.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4713 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/generative_models/ExperimentalImport.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1231 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/generative_models/GenerativeModel.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      510 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/generative_models/InternalOlgaModel.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    11754 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/generative_models/OLGA.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/generative_models/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.478351 ligo-1.0.3/ligo/simulation/implants/
+-rw-r--r--   0 milenpa    (502) staff       (20)      274 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/implants/ImplantAnnotation.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2589 2023-08-23 13:10:09.000000 ligo-1.0.3/ligo/simulation/implants/LigoPWM.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      642 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/implants/Motif.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      734 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/implants/MotifInstance.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     9917 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/implants/SeedMotif.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5918 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/implants/Signal.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/implants/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.478841 ligo-1.0.3/ligo/simulation/simulation_strategy/
+-rw-r--r--   0 milenpa    (502) staff       (20)    11379 2024-04-11 14:44:18.000000 ligo-1.0.3/ligo/simulation/simulation_strategy/ImplantingStrategy.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1449 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/simulation_strategy/RejectionSamplingStrategy.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      606 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/simulation/simulation_strategy/SimulationStrategy.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/simulation_strategy/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.479348 ligo-1.0.3/ligo/simulation/util/
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/util/__init__.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4089 2023-08-22 22:11:56.000000 ligo-1.0.3/ligo/simulation/util/bnp_util.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5363 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/simulation/util/igor_helper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    26794 2024-04-11 17:13:44.000000 ligo-1.0.3/ligo/simulation/util/util.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.481613 ligo-1.0.3/ligo/util/
+-rw-r--r--   0 milenpa    (502) staff       (20)     3767 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/AdaptiveImportHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      448 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/DistanceMetrics.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      405 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/DocEnumHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      761 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/util/ExporterHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1157 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/FilenameHandler.py
+-rw-r--r--   0 milenpa    (502) staff       (20)    26271 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/ImportHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1199 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/Logger.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1043 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/NameBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1602 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/NumpyHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     5877 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/util/ParameterValidator.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      776 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/PathBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     6510 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/util/PositionHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)       85 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/ReadsType.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     4112 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/ReflectionHandler.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     2676 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/RepertoireBuilder.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      593 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/Reports.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      401 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/StringHelper.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/util/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.481696 ligo-1.0.3/ligo/workflows/
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/workflows/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.481909 ligo-1.0.3/ligo/workflows/instructions/
+-rw-r--r--   0 milenpa    (502) staff       (20)      156 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/workflows/instructions/Instruction.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/workflows/instructions/__init__.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.482371 ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/
+-rw-r--r--   0 milenpa    (502) staff       (20)    12647 2023-10-12 11:20:23.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/__init__.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     7417 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.482955 ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/
+-rw-r--r--   0 milenpa    (502) staff       (20)    23974 2023-10-12 11:37:01.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/LigoSimInstruction.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/__init__.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      794 2023-10-02 11:57:55.000000 ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/runtime_reports.py
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.483808 ligo-1.0.3/ligo.egg-info/
+-rw-r--r--   0 milenpa    (502) staff       (20)     4429 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/PKG-INFO
+-rw-r--r--   0 milenpa    (502) staff       (20)     7529 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/SOURCES.txt
+-rw-r--r--   0 milenpa    (502) staff       (20)        1 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/dependency_links.txt
+-rw-r--r--   0 milenpa    (502) staff       (20)       47 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/entry_points.txt
+-rw-r--r--   0 milenpa    (502) staff       (20)      110 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/requires.txt
+-rw-r--r--   0 milenpa    (502) staff       (20)       13 2024-04-11 17:34:35.000000 ligo-1.0.3/ligo.egg-info/top_level.txt
+drwxr-xr-x   0 milenpa    (502) staff       (20)        0 2024-04-11 17:34:35.483600 ligo-1.0.3/scripts/
+-rw-r--r--   0 milenpa    (502) staff       (20)      326 2023-06-21 13:16:03.000000 ligo-1.0.3/scripts/DocumentatonFormat.py
+-rw-r--r--   0 milenpa    (502) staff       (20)        0 2023-06-21 13:16:03.000000 ligo-1.0.3/scripts/__init__.py
+-rw-r--r--   0 milenpa    (502) staff       (20)     1303 2023-06-21 13:16:03.000000 ligo-1.0.3/scripts/specification_util.py
+-rw-r--r--   0 milenpa    (502) staff       (20)      702 2023-06-21 13:16:03.000000 ligo-1.0.3/scripts/specs_docs_generation.py
+-rw-r--r--   0 milenpa    (502) staff       (20)       38 2024-04-11 17:34:35.484374 ligo-1.0.3/setup.cfg
+-rw-r--r--   0 milenpa    (502) staff       (20)     1391 2023-11-03 09:22:59.000000 ligo-1.0.3/setup.py
```

### Comparing `ligo-1.0.2/LICENSE.md` & `ligo-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/PKG-INFO` & `ligo-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo
-Version: 1.0.2
+Version: 1.0.3
 Summary: LIgO is a tool for simulation of adaptive immune receptors and repertoires.
 Home-page: https://github.com/uio-bmi/ligo
 Author: Milena Pavlovic
 Author-email: milenpa@student.matnat.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.11
@@ -58,73 +58,83 @@
 somewhere in the receptor sequence), the next 100 receptors will contain signal2 (sequences will contain `G/G`
 with the gap denoted by '\' sign and the gap size between 1 and 2 inclusive), and the final 100 receptors
 will not contain any of these signals.
 
 ```yaml
 
   definitions:
-  motifs:
-    motif1:
-      seed: AS
-    motif2:
-      seed: G/G
-      max_gap: 2
-      min_gap: 1
-  signals:
-    signal1:
-      v_call: TRBV7
-      motifs:
-        - motif1
-    signal2:
-      motifs:
-        - motif2
-  simulations:
-    sim1:
-      is_repertoire: false
-      paired: false
-      sequence_type: amino_acid
-      simulation_strategy: RejectionSampling
-      remove_seqs_with_signals: true 
-      sim_items:
-        sim_item1: # group of AIRs with the same parameters
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal1: 1
-        sim_item2:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal2: 1
-        sim_item3:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals: {} # no signal
+    motifs:
+      motif1:
+        seed: AS
+      motif2:
+        seed: G/G
+        max_gap: 2
+        min_gap: 1
+    signals:
+      signal1:
+        v_call: TRBV7
+        motifs:
+          - motif1
+      signal2:
+        motifs:
+          - motif2
+    simulations:
+      sim1:
+        is_repertoire: false
+        paired: false
+        sequence_type: amino_acid
+        simulation_strategy: RejectionSampling
+        remove_seqs_with_signals: true 
+        sim_items:
+          sim_item1: # group of AIRs with the same parameters
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal1: 1
+          sim_item2:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal2: 1
+          sim_item3:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals: {} # no signal
   instructions:
     my_sim_inst:
       export_p_gens: false
       max_iterations: 100
       number_of_processes: 4
       sequence_batch_size: 1000
       simulation: sim1
       type: LigoSim
 ```
 
-To run this simulations, save the YAML file above as specs.yaml and run the following:
+To run this simulation, save the YAML file above as specs.yaml and run the following:
 
 ```commandline
 ligo specs.yaml output_folder
 ```
 
 Note that `output_folder` (user-defined name) should not exist before the run.
+
+
+## Citing LIgO
+
+If you are using LIgO in any published work, please cite:
+
+Chernigovskaya, M.; Pavlović, M.; Kanduri, C.; Gielis, S.; Robert, P. A.; Scheffer, L.; Slabodkin, A.; Haff, I. H.; Meysman, P.; Yaari, G.; Sandve, G. K.; Greiff, V
+“Simulation of Adaptive Immune Receptors and Repertoires with Complex Immune Information to Guide the Development and Benchmarking of AIRR Machine Learning” 
+bioRxiv, 2023, 2023.10.20.562936. https://doi.org/10.1101/2023.10.20.562936.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ligo-1.0.2/README.md` & `ligo-1.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -32,73 +32,83 @@
 somewhere in the receptor sequence), the next 100 receptors will contain signal2 (sequences will contain `G/G`
 with the gap denoted by '\' sign and the gap size between 1 and 2 inclusive), and the final 100 receptors
 will not contain any of these signals.
 
 ```yaml
 
   definitions:
-  motifs:
-    motif1:
-      seed: AS
-    motif2:
-      seed: G/G
-      max_gap: 2
-      min_gap: 1
-  signals:
-    signal1:
-      v_call: TRBV7
-      motifs:
-        - motif1
-    signal2:
-      motifs:
-        - motif2
-  simulations:
-    sim1:
-      is_repertoire: false
-      paired: false
-      sequence_type: amino_acid
-      simulation_strategy: RejectionSampling
-      remove_seqs_with_signals: true 
-      sim_items:
-        sim_item1: # group of AIRs with the same parameters
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal1: 1
-        sim_item2:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal2: 1
-        sim_item3:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals: {} # no signal
+    motifs:
+      motif1:
+        seed: AS
+      motif2:
+        seed: G/G
+        max_gap: 2
+        min_gap: 1
+    signals:
+      signal1:
+        v_call: TRBV7
+        motifs:
+          - motif1
+      signal2:
+        motifs:
+          - motif2
+    simulations:
+      sim1:
+        is_repertoire: false
+        paired: false
+        sequence_type: amino_acid
+        simulation_strategy: RejectionSampling
+        remove_seqs_with_signals: true 
+        sim_items:
+          sim_item1: # group of AIRs with the same parameters
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal1: 1
+          sim_item2:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal2: 1
+          sim_item3:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals: {} # no signal
   instructions:
     my_sim_inst:
       export_p_gens: false
       max_iterations: 100
       number_of_processes: 4
       sequence_batch_size: 1000
       simulation: sim1
       type: LigoSim
 ```
 
-To run this simulations, save the YAML file above as specs.yaml and run the following:
+To run this simulation, save the YAML file above as specs.yaml and run the following:
 
 ```commandline
 ligo specs.yaml output_folder
 ```
 
 Note that `output_folder` (user-defined name) should not exist before the run.
+
+
+## Citing LIgO
+
+If you are using LIgO in any published work, please cite:
+
+Chernigovskaya, M.; Pavlović, M.; Kanduri, C.; Gielis, S.; Robert, P. A.; Scheffer, L.; Slabodkin, A.; Haff, I. H.; Meysman, P.; Yaari, G.; Sandve, G. K.; Greiff, V
+“Simulation of Adaptive Immune Receptors and Repertoires with Complex Immune Information to Guide the Development and Benchmarking of AIRR Machine Learning” 
+bioRxiv, 2023, 2023.10.20.562936. https://doi.org/10.1101/2023.10.20.562936.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ligo-1.0.2/ligo/IO/dataset_export/AIRRExporter.py` & `ligo-1.0.3/ligo/IO/dataset_export/AIRRExporter.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_export/ImmuneMLExporter.py` & `ligo-1.0.3/ligo/IO/dataset_export/ImmuneMLExporter.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/AIRRImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/AIRRImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/DatasetImportParams.py` & `ligo-1.0.3/ligo/IO/dataset_import/DatasetImportParams.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/GenericImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/GenericImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/IGoRImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/IGoRImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/IReceptorImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/IReceptorImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/ImmuneMLImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/ImmuneMLImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/ImmunoSEQRearrangementImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/ImmunoSEQRearrangementImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/ImmunoSEQSampleImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/ImmunoSEQSampleImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/MiXCRImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/MiXCRImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/OLGAImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/OLGAImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/SingleLineReceptorImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/SingleLineReceptorImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/TenxGenomicsImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/TenxGenomicsImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/VDJdbImport.py` & `ligo-1.0.3/ligo/IO/dataset_import/VDJdbImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/IO/dataset_import/conversion/imgt_adaptive_conversion.csv` & `ligo-1.0.3/ligo/IO/dataset_import/conversion/imgt_adaptive_conversion.csv`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/app/LigoApp.py` & `ligo-1.0.3/ligo/app/LigoApp.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/airr_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/airr_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/i_receptor_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/i_receptor_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/igor_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/igor_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/immuno_seq_rearrangement_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/immuno_seq_rearrangement_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/immuno_seq_sample_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/immuno_seq_sample_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/mixcr_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/mixcr_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/olga_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/olga_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/random_repertoire_dataset_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/random_repertoire_dataset_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/tenx_genomics_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/tenx_genomics_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/config/default_params/datasets/vdjdb_params.yaml` & `ligo-1.0.3/ligo/config/default_params/datasets/vdjdb_params.yaml`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/cell/CellList.py` & `ligo-1.0.3/ligo/data_model/cell/CellList.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/dataset/Dataset.py` & `ligo-1.0.3/ligo/data_model/dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/dataset/ElementDataset.py` & `ligo-1.0.3/ligo/data_model/dataset/ElementDataset.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/dataset/ReceptorDataset.py` & `ligo-1.0.3/ligo/data_model/dataset/ReceptorDataset.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/dataset/RepertoireDataset.py` & `ligo-1.0.3/ligo/data_model/dataset/RepertoireDataset.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/dataset/SequenceDataset.py` & `ligo-1.0.3/ligo/data_model/dataset/SequenceDataset.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/encoded_data/EncodedData.py` & `ligo-1.0.3/ligo/data_model/encoded_data/EncodedData.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/BCKReceptor.py` & `ligo-1.0.3/ligo/data_model/receptor/BCKReceptor.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/BCReceptor.py` & `ligo-1.0.3/ligo/data_model/receptor/BCReceptor.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/ChainPair.py` & `ligo-1.0.3/ligo/data_model/receptor/ChainPair.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/ElementGenerator.py` & `ligo-1.0.3/ligo/data_model/receptor/ElementGenerator.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/Receptor.py` & `ligo-1.0.3/ligo/data_model/receptor/Receptor.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/ReceptorBuilder.py` & `ligo-1.0.3/ligo/data_model/receptor/ReceptorBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/TCABReceptor.py` & `ligo-1.0.3/ligo/data_model/receptor/TCABReceptor.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/TCGDReceptor.py` & `ligo-1.0.3/ligo/data_model/receptor/TCGDReceptor.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/Chain.py` & `ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/Chain.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/ReceptorSequence.py` & `ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/ReceptorSequence.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/SequenceAnnotation.py` & `ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/SequenceAnnotation.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/receptor/receptor_sequence/SequenceMetadata.py` & `ligo-1.0.3/ligo/data_model/receptor/receptor_sequence/SequenceMetadata.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/data_model/repertoire/Repertoire.py` & `ligo-1.0.3/ligo/data_model/repertoire/Repertoire.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/DefaultParamsLoader.py` & `ligo-1.0.3/ligo/dsl/DefaultParamsLoader.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/InstructionParser.py` & `ligo-1.0.3/ligo/dsl/InstructionParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/LigoParser.py` & `ligo-1.0.3/ligo/dsl/LigoParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/ObjectParser.py` & `ligo-1.0.3/ligo/dsl/ObjectParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/OutputParser.py` & `ligo-1.0.3/ligo/dsl/OutputParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/Util.py` & `ligo-1.0.3/ligo/dsl/Util.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/definition_parsers/DefinitionParser.py` & `ligo-1.0.3/ligo/dsl/definition_parsers/DefinitionParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/definition_parsers/DefinitionParserOutput.py` & `ligo-1.0.3/ligo/dsl/definition_parsers/DefinitionParserOutput.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/definition_parsers/MotifParser.py` & `ligo-1.0.3/ligo/dsl/definition_parsers/MotifParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/definition_parsers/SignalParser.py` & `ligo-1.0.3/ligo/dsl/definition_parsers/SignalParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/definition_parsers/SimulationParser.py` & `ligo-1.0.3/ligo/dsl/definition_parsers/SimulationParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/import_parsers/ImportParser.py` & `ligo-1.0.3/ligo/dsl/import_parsers/ImportParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/instruction_parsers/FeasibilitySummaryParser.py` & `ligo-1.0.3/ligo/dsl/instruction_parsers/FeasibilitySummaryParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/instruction_parsers/LigoSimParser.py` & `ligo-1.0.3/ligo/dsl/instruction_parsers/LigoSimParser.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/semantic_model/SemanticModel.py` & `ligo-1.0.3/ligo/dsl/semantic_model/SemanticModel.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/dsl/symbol_table/SymbolTable.py` & `ligo-1.0.3/ligo/dsl/symbol_table/SymbolTable.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/environment/EnvironmentSettings.py` & `ligo-1.0.3/ligo/environment/EnvironmentSettings.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/PresentationFactory.py` & `ligo-1.0.3/ligo/presentation/PresentationFactory.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/FeasibilitySummaryHTMLBuilder.py` & `ligo-1.0.3/ligo/presentation/html/FeasibilitySummaryHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/HTMLBuilder.py` & `ligo-1.0.3/ligo/presentation/html/HTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/LIgOSimulationHTMLBuilder.py` & `ligo-1.0.3/ligo/presentation/html/LIgOSimulationHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/Util.py` & `ligo-1.0.3/ligo/presentation/html/Util.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/templates/DatasetExport.html` & `ligo-1.0.3/ligo/presentation/html/templates/DatasetExport.html`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/templates/FeasibilitySummary.html` & `ligo-1.0.3/ligo/presentation/html/templates/FeasibilitySummary.html`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/templates/Simulation.html` & `ligo-1.0.3/ligo/presentation/html/templates/Simulation.html`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/templates/css/custom.css` & `ligo-1.0.3/ligo/presentation/html/templates/css/custom.css`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/presentation/html/templates/index.html` & `ligo-1.0.3/ligo/presentation/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/LigoSimState.py` & `ligo-1.0.3/ligo/simulation/LigoSimState.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/SimConfig.py` & `ligo-1.0.3/ligo/simulation/SimConfig.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/SimConfigItem.py` & `ligo-1.0.3/ligo/simulation/SimConfigItem.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/dataset_generation/RandomDatasetGenerator.py` & `ligo-1.0.3/ligo/simulation/dataset_generation/RandomDatasetGenerator.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/generative_models/BackgroundSequences.py` & `ligo-1.0.3/ligo/simulation/generative_models/BackgroundSequences.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/generative_models/ExperimentalImport.py` & `ligo-1.0.3/ligo/simulation/generative_models/ExperimentalImport.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/generative_models/GenerativeModel.py` & `ligo-1.0.3/ligo/simulation/generative_models/GenerativeModel.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/generative_models/OLGA.py` & `ligo-1.0.3/ligo/simulation/generative_models/OLGA.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/implants/LigoPWM.py` & `ligo-1.0.3/ligo/simulation/implants/LigoPWM.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/implants/Motif.py` & `ligo-1.0.3/ligo/simulation/implants/Motif.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/implants/MotifInstance.py` & `ligo-1.0.3/ligo/simulation/implants/MotifInstance.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/implants/SeedMotif.py` & `ligo-1.0.3/ligo/simulation/implants/SeedMotif.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/implants/Signal.py` & `ligo-1.0.3/ligo/simulation/implants/Signal.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/simulation_strategy/ImplantingStrategy.py` & `ligo-1.0.3/ligo/simulation/simulation_strategy/ImplantingStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,18 +137,16 @@
             new_sequence['p_gen'] = sim_item.generative_model.compute_p_gen(
                 {key: val.to_string() if hasattr(val, "to_string") else val for key, val in new_sequence.items()},
                 sequence_type)
         else:
             new_sequence['p_gen'] = -1.
 
         new_sequence[signal.id] = 1
-        new_sequence[f'{signal.id}_positions'] = "m" + "".join("0" for _ in range(implant_position)) + "1" + \
-                                                 "".join("0" for _ in
-                                                         range(len(getattr(sequence_row,
-                                                                           sequence_type.value)) - implant_position))
+        new_sequence[f'{signal.id}_positions'] = ["m"] + ["0" if ind != implant_position else "1" for ind in range(sequence_length)]
+        new_sequence[f'{signal.id}_positions'] = "".join(new_sequence[f'{signal.id}_positions'])
 
         zero_mask = "m" + "".join(["0" for _ in range(len(new_sequence[sequence_type.value]))])
         new_sequence = {**{f"{s.id}_positions": zero_mask for s in all_signals},
                         **{s.id: 0 for s in all_signals if s.id != signal.id},
                         **new_sequence,
                         f'observed_{signal.id}': int(random.uniform(0, 1) > sim_item.false_negative_prob_in_receptors),
                         f'from_default_model': 0, 'duplicate_count': -1, 'signals_aggregated': signal.id,
```

### Comparing `ligo-1.0.2/ligo/simulation/simulation_strategy/RejectionSamplingStrategy.py` & `ligo-1.0.3/ligo/simulation/simulation_strategy/RejectionSamplingStrategy.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/simulation_strategy/SimulationStrategy.py` & `ligo-1.0.3/ligo/simulation/simulation_strategy/SimulationStrategy.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/util/bnp_util.py` & `ligo-1.0.3/ligo/simulation/util/bnp_util.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/util/igor_helper.py` & `ligo-1.0.3/ligo/simulation/util/igor_helper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/simulation/util/util.py` & `ligo-1.0.3/ligo/simulation/util/util.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/AdaptiveImportHelper.py` & `ligo-1.0.3/ligo/util/AdaptiveImportHelper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/ExporterHelper.py` & `ligo-1.0.3/ligo/util/ExporterHelper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/FilenameHandler.py` & `ligo-1.0.3/ligo/util/FilenameHandler.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/ImportHelper.py` & `ligo-1.0.3/ligo/util/ImportHelper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/Logger.py` & `ligo-1.0.3/ligo/util/Logger.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/NameBuilder.py` & `ligo-1.0.3/ligo/util/NameBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/NumpyHelper.py` & `ligo-1.0.3/ligo/util/NumpyHelper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/ParameterValidator.py` & `ligo-1.0.3/ligo/util/ParameterValidator.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/PathBuilder.py` & `ligo-1.0.3/ligo/util/PathBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/PositionHelper.py` & `ligo-1.0.3/ligo/util/PositionHelper.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/ReflectionHandler.py` & `ligo-1.0.3/ligo/util/ReflectionHandler.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/RepertoireBuilder.py` & `ligo-1.0.3/ligo/util/RepertoireBuilder.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/util/Reports.py` & `ligo-1.0.3/ligo/util/Reports.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py` & `ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py` & `ligo-1.0.3/ligo/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/LigoSimInstruction.py` & `ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/LigoSimInstruction.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo/workflows/instructions/ligo_simulation/runtime_reports.py` & `ligo-1.0.3/ligo/workflows/instructions/ligo_simulation/runtime_reports.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/ligo.egg-info/PKG-INFO` & `ligo-1.0.3/ligo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo
-Version: 1.0.2
+Version: 1.0.3
 Summary: LIgO is a tool for simulation of adaptive immune receptors and repertoires.
 Home-page: https://github.com/uio-bmi/ligo
 Author: Milena Pavlovic
 Author-email: milenpa@student.matnat.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.11
@@ -58,73 +58,83 @@
 somewhere in the receptor sequence), the next 100 receptors will contain signal2 (sequences will contain `G/G`
 with the gap denoted by '\' sign and the gap size between 1 and 2 inclusive), and the final 100 receptors
 will not contain any of these signals.
 
 ```yaml
 
   definitions:
-  motifs:
-    motif1:
-      seed: AS
-    motif2:
-      seed: G/G
-      max_gap: 2
-      min_gap: 1
-  signals:
-    signal1:
-      v_call: TRBV7
-      motifs:
-        - motif1
-    signal2:
-      motifs:
-        - motif2
-  simulations:
-    sim1:
-      is_repertoire: false
-      paired: false
-      sequence_type: amino_acid
-      simulation_strategy: RejectionSampling
-      remove_seqs_with_signals: true 
-      sim_items:
-        sim_item1: # group of AIRs with the same parameters
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal1: 1
-        sim_item2:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals:
-            signal2: 1
-        sim_item3:
-          generative_model:
-            chain: beta
-            default_model_name: humanTRB
-            model_path: null
-            type: OLGA
-          number_of_examples: 100
-          signals: {} # no signal
+    motifs:
+      motif1:
+        seed: AS
+      motif2:
+        seed: G/G
+        max_gap: 2
+        min_gap: 1
+    signals:
+      signal1:
+        v_call: TRBV7
+        motifs:
+          - motif1
+      signal2:
+        motifs:
+          - motif2
+    simulations:
+      sim1:
+        is_repertoire: false
+        paired: false
+        sequence_type: amino_acid
+        simulation_strategy: RejectionSampling
+        remove_seqs_with_signals: true 
+        sim_items:
+          sim_item1: # group of AIRs with the same parameters
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal1: 1
+          sim_item2:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals:
+              signal2: 1
+          sim_item3:
+            generative_model:
+              chain: beta
+              default_model_name: humanTRB
+              model_path: null
+              type: OLGA
+            number_of_examples: 100
+            signals: {} # no signal
   instructions:
     my_sim_inst:
       export_p_gens: false
       max_iterations: 100
       number_of_processes: 4
       sequence_batch_size: 1000
       simulation: sim1
       type: LigoSim
 ```
 
-To run this simulations, save the YAML file above as specs.yaml and run the following:
+To run this simulation, save the YAML file above as specs.yaml and run the following:
 
 ```commandline
 ligo specs.yaml output_folder
 ```
 
 Note that `output_folder` (user-defined name) should not exist before the run.
+
+
+## Citing LIgO
+
+If you are using LIgO in any published work, please cite:
+
+Chernigovskaya, M.; Pavlović, M.; Kanduri, C.; Gielis, S.; Robert, P. A.; Scheffer, L.; Slabodkin, A.; Haff, I. H.; Meysman, P.; Yaari, G.; Sandve, G. K.; Greiff, V
+“Simulation of Adaptive Immune Receptors and Repertoires with Complex Immune Information to Guide the Development and Benchmarking of AIRR Machine Learning” 
+bioRxiv, 2023, 2023.10.20.562936. https://doi.org/10.1101/2023.10.20.562936.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ligo-1.0.2/ligo.egg-info/SOURCES.txt` & `ligo-1.0.3/ligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/scripts/specification_util.py` & `ligo-1.0.3/scripts/specification_util.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/scripts/specs_docs_generation.py` & `ligo-1.0.3/scripts/specs_docs_generation.py`

 * *Files identical despite different names*

### Comparing `ligo-1.0.2/setup.py` & `ligo-1.0.3/setup.py`

 * *Files identical despite different names*

