# Comparing `tmp/pami-2024.4.11.1.tar.gz` & `tmp/pami-2024.4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2024.4.11.1.tar", last modified: Thu Apr 11 09:56:19 2024, max compression
+gzip compressed data, was "pami-2024.4.9.1.tar", last modified: Tue Apr  9 02:13:28 2024, max compression
```

## Comparing `pami-2024.4.11.1.tar` & `pami-2024.4.9.1.tar`

### file list

```diff
@@ -1,506 +1,505 @@
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.699152 pami-2024.4.11.1/
--rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.4.11.1/LICENSE
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.214649 pami-2024.4.11.1/PAMI/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.215464 pami-2024.4.11.1/PAMI/AssociationRules/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.221488 pami-2024.4.11.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    14314 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14661 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14622 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20378 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6594 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.222323 pami-2024.4.11.1/PAMI/correlatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.227201 pami-2024.4.11.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27142 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    29081 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.227867 pami-2024.4.11.1/PAMI/coveragePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.231244 pami-2024.4.11.1/PAMI/coveragePattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    15616 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18923 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.242899 pami-2024.4.11.1/PAMI/extras/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.251992 pami-2024.4.11.1/PAMI/extras/DF2DB/
--rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/DenseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/SparseFormatDF.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.253850 pami-2024.4.11.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/calculateMISValues/usingSD.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7350 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/convertMultiTSIntoFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.263729 pami-2024.4.11.1/PAMI/extras/dbStats/
--rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/FuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/dbStats/SequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/dbStats/UtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/dbStats/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.266927 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.270317 pami-2024.4.11.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5157 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.275978 pami-2024.4.11.1/PAMI/extras/graph/
--rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/DF2Fig.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/DF2Tex.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.276741 pami-2024.4.11.1/PAMI/extras/image2Database/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.277774 pami-2024.4.11.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.279442 pami-2024.4.11.1/PAMI/extras/messaging/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/messaging/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/messaging/discord.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/messaging/gmail.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.283465 pami-2024.4.11.1/PAMI/extras/neighbours/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4789 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4415 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4310 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5013 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5183 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/plotPointOnMap_dump.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.285619 pami-2024.4.11.1/PAMI/extras/sampleDatasets/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/sampleDatasets/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4024 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.292102 pami-2024.4.11.1/PAMI/extras/stats/
--rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/stats/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/stats/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/stats/graphDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/stats/sequentialDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/stats/temporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/stats/utilityDatabase.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.318043 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/
--rw-r--r--   0 vanithak   (502) staff       (20)     8471 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5543 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
--rw-r--r--   0 vanithak   (502) staff       (20)     3240 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2322 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.325511 pami-2024.4.11.1/PAMI/extras/visualize/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/extras/visualize/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/extras/visualize/graphs.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.326767 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.333280 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    15253 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24431 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.334629 pami-2024.4.11.1/PAMI/frequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.345396 pami-2024.4.11.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    17024 2024-04-11 09:55:12.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15219 2024-04-11 09:55:12.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/AprioriOLD.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14362 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14885 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15362 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7867 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.352510 pami-2024.4.11.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    22294 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.365993 pami-2024.4.11.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15188 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16228 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14636 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16604 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16419 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21681 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 vanithak   (502) staff       (20)    15055 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.369495 pami-2024.4.11.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    27531 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.375122 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    16543 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 vanithak   (502) staff       (20)    14856 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19036 2024-04-11 09:55:12.000000 pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.379724 pami-2024.4.11.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    16687 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.380399 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.383810 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    32988 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6645 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.384657 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.389050 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25855 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32901 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6428 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.390035 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.394995 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29496 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32795 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6724 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.395810 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.399555 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33628 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    39030 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.400667 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.404335 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25016 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6463 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.405598 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.410061 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29275 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32773 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6678 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.410884 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.413815 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23633 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6782 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.415979 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.420600 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23719 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22366 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6689 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.422694 pami-2024.4.11.1/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6690 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.424726 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.428554 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    23257 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.430130 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.433276 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    41228 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.434164 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.436490 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    46718 2024-04-11 09:55:13.000000 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.437332 pami-2024.4.11.1/PAMI/highUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.444735 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    37128 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    30770 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    32709 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20285 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.447938 pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18207 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.452975 pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 vanithak   (502) staff       (20)    32873 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    35784 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.454815 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.460693 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35564 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)    40140 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.463511 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)    40254 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.464399 pami-2024.4.11.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.468886 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    36343 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25563 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24596 2024-04-10 08:52:08.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.469679 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.474280 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    25470 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23153 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.475440 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.480831 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28279 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    22083 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.481603 pami-2024.4.11.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.498870 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    26417 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26878 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20736 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.502679 pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24133 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.507006 pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    29141 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.511800 pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    30910 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.515637 pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20928 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.520203 pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 vanithak   (502) staff       (20)    28158 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5556 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.521584 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.524904 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27514 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6640 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.526362 pami-2024.4.11.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.539050 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    17905 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6545 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.543594 pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)    24312 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.549551 pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.556776 pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.559684 pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.561320 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.566831 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.572676 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.575690 pami-2024.4.11.1/PAMI/recurringPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.580107 pami-2024.4.11.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.580966 pami-2024.4.11.1/PAMI/relativeFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.584010 pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.584952 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.587580 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.588603 pami-2024.4.11.1/PAMI/sequence/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequence/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.589202 pami-2024.4.11.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.595335 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/SPAM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.598860 pami-2024.4.11.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.599301 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.605926 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    19114 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26504 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    21391 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.611865 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.612890 pami-2024.4.11.1/PAMI/subgraphMining/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.623859 pami-2024.4.11.1/PAMI/subgraphMining/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/dfsCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/gspan.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/basic/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.637946 pami-2024.4.11.1/PAMI/subgraphMining/topK/
--rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/DFSCode.py
--rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/DFSThread.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/edge.py
--rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/extendedEdge.py
--rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/frequentSubgraph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/graph.py
--rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
--rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/tkg.py
--rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/subgraphMining/topK/vertex.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.642344 pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)    17358 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.643468 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.662929 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    28610 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 vanithak   (502) staff       (20)    26391 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19572 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19454 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 vanithak   (502) staff       (20)    27790 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 vanithak   (502) staff       (20)    25664 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    19522 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.664289 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.668174 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30868 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.669118 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.673631 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    33395 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)    33912 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.674600 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.679158 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30821 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.679887 pami-2024.4.11.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.682727 pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    27246 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.683480 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.685964 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    30320 2024-04-09 02:02:26.000000 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.686816 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.689551 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 vanithak   (502) staff       (20)    31958 2024-03-29 21:11:29.000000 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 vanithak   (502) staff       (20)    68883 2024-04-11 09:56:19.698136 pami-2024.4.11.1/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    67413 2024-04-11 09:55:12.000000 pami-2024.4.11.1/README.md
-drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-11 09:56:19.694463 pami-2024.4.11.1/pami.egg-info/
--rw-r--r--   0 vanithak   (502) staff       (20)    68883 2024-04-11 09:56:18.000000 pami-2024.4.11.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 vanithak   (502) staff       (20)    18099 2024-04-11 09:56:19.000000 pami-2024.4.11.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-04-11 09:56:18.000000 pami-2024.4.11.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 vanithak   (502) staff       (20)      248 2024-04-11 09:56:18.000000 pami-2024.4.11.1/pami.egg-info/requires.txt
--rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-04-11 09:56:18.000000 pami-2024.4.11.1/pami.egg-info/top_level.txt
--rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-04-11 09:56:19.699291 pami-2024.4.11.1/setup.cfg
--rw-r--r--   0 vanithak   (502) staff       (20)     1518 2024-04-11 09:56:12.000000 pami-2024.4.11.1/setup.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.602975 pami-2024.4.9.1/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35149 2024-03-12 04:33:29.000000 pami-2024.4.9.1/LICENSE
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.793712 pami-2024.4.9.1/PAMI/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.795296 pami-2024.4.9.1/PAMI/AssociationRules/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.809616 pami-2024.4.9.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14314 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14661 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14622 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20378 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6594 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      139 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.811156 pami-2024.4.9.1/PAMI/correlatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.817103 pami-2024.4.9.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27142 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    29081 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6208 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.818346 pami-2024.4.9.1/PAMI/coveragePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.826282 pami-2024.4.9.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15616 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18923 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7155 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.838845 pami-2024.4.9.1/PAMI/extras/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.853335 pami-2024.4.9.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 vanithak   (502) staff       (20)     4360 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4287 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    10331 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/DenseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5413 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/SparseFormatDF.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3103 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6948 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11940 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5336 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.858573 pami-2024.4.9.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6468 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6499 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingSD.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6964 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/convertMultiTSIntoFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.876165 pami-2024.4.9.1/PAMI/extras/dbStats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    14951 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/FuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    13796 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16034 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/dbStats/SequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16883 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12839 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15120 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    11953 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12679 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/dbStats/UtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/dbStats/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.880811 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5238 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8594 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8792 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8313 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.889684 pami-2024.4.9.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5685 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     9558 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5971 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5156 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.901708 pami-2024.4.9.1/PAMI/extras/graph/
+-rw-r--r--   0 vanithak   (502) staff       (20)     3223 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/DF2Fig.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3577 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/DF2Tex.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2750 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3599 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4465 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/visualizeFuzzyPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4240 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.904228 pami-2024.4.9.1/PAMI/extras/image2Database/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.906815 pami-2024.4.9.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6488 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.911056 pami-2024.4.9.1/PAMI/extras/messaging/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/messaging/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      533 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/messaging/discord.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1575 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/messaging/gmail.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.917378 pami-2024.4.9.1/PAMI/extras/neighbours/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4789 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4415 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4310 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5011 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5182 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/plotPointOnMap_dump.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.922472 pami-2024.4.9.1/PAMI/extras/sampleDatasets/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/sampleDatasets/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4023 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.932869 pami-2024.4.9.1/PAMI/extras/stats/
+-rw-r--r--   0 vanithak   (502) staff       (20)    12724 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/stats/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4144 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/stats/graphDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15998 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/sequentialDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16926 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/temporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    12692 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/stats/utilityDatabase.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.964837 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/
+-rw-r--r--   0 vanithak   (502) staff       (20)     8471 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5543 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2325 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2254 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2539 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1880 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1843 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2117 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2066 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2262 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/fuzzyDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1121 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1111 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1625 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1610 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3613 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3603 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/georeferencedTemporalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/georeferencedTransactionalDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4324 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3283 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4842 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     3238 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2321 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.969666 pami-2024.4.9.1/PAMI/extras/visualize/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/extras/visualize/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1897 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/extras/visualize/graphs.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.971091 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.976128 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15253 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24431 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6856 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.977409 pami-2024.4.9.1/PAMI/frequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.988154 pami-2024.4.9.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    15220 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14362 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14885 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15362 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22703 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7867 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:27.991640 pami-2024.4.9.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    22294 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6580 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.052468 pami-2024.4.9.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5980 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15188 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16228 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14636 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16604 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16419 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21681 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    15055 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.056713 pami-2024.4.9.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27531 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6561 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.064878 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5573 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    16543 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    14856 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19026 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.073549 pami-2024.4.9.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    16687 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4575 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.075074 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.080427 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    32988 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6645 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.085119 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.092414 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25855 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32901 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6428 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.094061 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.101426 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29496 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32795 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6724 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.103125 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.110674 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    33628 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    39030 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.114640 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.121669 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25016 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6463 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.122749 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.128995 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29275 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32773 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6678 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.130182 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.138617 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23633 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6782 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.139762 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.145864 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23719 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22366 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6689 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.148990 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6690 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.150420 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.155070 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    23257 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6178 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.156998 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.160629 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    41228 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6179 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.162526 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.169244 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    46718 2024-04-09 02:02:27.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6307 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.170240 pami-2024.4.9.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.178668 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    37128 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    30770 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    32709 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20285 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.185414 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5166 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18207 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.191526 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 vanithak   (502) staff       (20)    32873 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    35784 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5193 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.194856 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6716 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.201955 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35564 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    40140 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5934 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.205999 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)    40254 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6618 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.207268 pami-2024.4.9.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.214488 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    34480 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23965 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22949 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     8385 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.217320 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.222491 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    25470 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23153 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5921 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.224344 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.234442 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28279 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    22083 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5398 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.235758 pami-2024.4.9.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.251077 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    26417 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4329 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26878 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20736 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5520 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.257160 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24133 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5605 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.274878 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29141 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4278 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.286087 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5765 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    30910 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.293743 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6441 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20928 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.303465 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28158 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5556 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.309577 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.319198 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27514 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6640 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.320539 pami-2024.4.9.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.340954 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17905 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28583 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26383 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18106 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    36300 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      726 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6545 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26643 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.347343 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)    24312 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6539 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.356329 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6568 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    23867 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    18982 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.363446 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31832 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7869 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.373650 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     5219 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26749 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.376040 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.383726 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 vanithak   (502) staff       (20)    19951 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6862 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.387608 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4589 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    17514 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.389862 pami-2024.4.9.1/PAMI/recurringPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.394287 pami-2024.4.9.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    29135 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6637 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.396535 pami-2024.4.9.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.403016 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30349 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4261 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.404650 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.407969 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    35406 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6052 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.410534 pami-2024.4.9.1/PAMI/sequence/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.411261 pami-2024.4.9.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.421832 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    42265 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19986 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPAM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6569 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    24786 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.426003 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6285 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.427496 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.436338 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    19114 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26504 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    21391 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7271 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.440665 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27859 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7173 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.441985 pami-2024.4.9.1/PAMI/subgraphMining/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.456287 pami-2024.4.9.1/PAMI/subgraphMining/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1241 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2396 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/dfsCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2616 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      670 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4943 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    28244 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/gspan.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1748 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      826 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/basic/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.478210 pami-2024.4.9.1/PAMI/subgraphMining/topK/
+-rw-r--r--   0 vanithak   (502) staff       (20)     1949 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSCode.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      593 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSThread.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1316 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      772 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/edge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     2613 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/extendedEdge.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      674 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/frequentSubgraph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4295 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/graph.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     1486 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    20979 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/tkg.py
+-rw-r--r--   0 vanithak   (502) staff       (20)      818 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/subgraphMining/topK/vertex.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.482255 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)    17358 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6756 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.483938 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.506622 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    28610 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    26391 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19572 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19454 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    27790 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    25664 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    19522 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4945 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.508127 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.520288 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30868 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4986 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.524799 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)      727 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.537346 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    33395 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    33912 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6536 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.538277 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.546173 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30821 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6603 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.549586 pami-2024.4.9.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.558446 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    27246 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     6659 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.563418 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.574205 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    30320 2024-04-09 02:02:26.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     7495 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.575583 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.579690 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 vanithak   (502) staff       (20)    31958 2024-03-29 21:11:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 vanithak   (502) staff       (20)        0 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 vanithak   (502) staff       (20)     4771 2024-03-12 04:33:29.000000 pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 vanithak   (502) staff       (20)    67204 2024-04-09 02:13:28.599349 pami-2024.4.9.1/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    65760 2024-03-29 21:11:29.000000 pami-2024.4.9.1/README.md
+drwxr-xr-x   0 vanithak   (502) staff       (20)        0 2024-04-09 02:13:28.589956 pami-2024.4.9.1/pami.egg-info/
+-rw-r--r--   0 vanithak   (502) staff       (20)    67204 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 vanithak   (502) staff       (20)    18058 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        1 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)      237 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/requires.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)        5 2024-04-09 02:13:27.000000 pami-2024.4.9.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 vanithak   (502) staff       (20)       38 2024-04-09 02:13:28.603191 pami-2024.4.9.1/setup.cfg
+-rw-r--r--   0 vanithak   (502) staff       (20)     1494 2024-04-09 02:13:23.000000 pami-2024.4.9.1/setup.py
```

### Comparing `pami-2024.4.11.1/LICENSE` & `pami-2024.4.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2024.4.9.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/correlatedPattern/__init__.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/coveragePattern/basic/CMine.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/coveragePattern/basic/CPPG.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/coveragePattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/DenseFormatDF.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/DenseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/SparseFormatDF.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/SparseFormatDF.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2024.4.9.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2024.4.9.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/convertMultiTSIntoFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/convertMultiTSIntoFuzzy.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,19 @@
 #
 #     from PAMI.extras.syntheticDataGenerator import convertMultiTSIntoFuzzy as fuz
 #
 #     obj = fuz.convertMultiTSIntoFuzzy(iFile, FuzFile)
 #
 #     obj.save()
 #
-#     obj.mine()
+#     obj.startMine()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -52,15 +49,16 @@
 
                 from PAMI.extras.syntheticDataGenerator import convertMultiTSIntoFuzzy as fuz
 
                 obj = fuz.convertMultiTSIntoFuzzy(iFile, FuzFile)
 
                 obj.save()
 
-                obj.mine()
+                obj.startMine()
+
 
     """
 
 
     def __init__(self, iFile: str,  FuzFile: str) -> None:
         #super().__init__(iFile, nFile, FuzFile, minSup, maxPer, sep)
         self._iFile = iFile
@@ -165,32 +163,22 @@
                     s = s +  item + '.' + self._LabelKeyOne[k]  + '\t'
                     ss = ss + str(round(self.list[k], 2))+ '\t'
             s2 = s1 + ':' + s + ':' + ss
             # print(s2)
             # break
             writer.write("%s\n" %s2)
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
+
     def startMine(self) -> None:
-        """
-        Frequent pattern mining process will start from here
+        """ Frequent pattern mining process will start from here
         """
         
         self._creatingItemSets()
         self._fuzzyMembershipFunc()
         self._finalPatterns = {}
-
-    def mine(self) -> None:
-        """
-        Frequent pattern mining process will start from here
-        """
-
-        self._creatingItemSets()
-        self._fuzzyMembershipFunc()
-        self._finalPatterns = {}
         
 if __name__ == "__main__":
     convertMultipleTSIntoFuzzy(sys.argv[1], sys.argv[2])
```

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/FuzzyDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/FuzzyDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/MultipleTimeSeriesFuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/SequentialDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/SequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/TemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UncertainTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/dbStats/UtilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/dbStats/UtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2024.4.9.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2024.4.9.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 #
 #     obj = fuz.generateLatexGraphFile(idf)
 #
 #     obj.save()
 #
 
 
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/DF2Fig.py` & `pami-2024.4.9.1/PAMI/extras/graph/DF2Fig.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/DF2Tex.py` & `pami-2024.4.9.1/PAMI/extras/graph/DF2Tex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2024.4.9.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/visualizeFuzzyPatterns.py` & `pami-2024.4.9.1/PAMI/extras/graph/visualizeFuzzyPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2024.4.9.1/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2024.4.9.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/messaging/discord.py` & `pami-2024.4.9.1/PAMI/extras/messaging/discord.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/messaging/gmail.py` & `pami-2024.4.9.1/PAMI/extras/messaging/gmail.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighborsUsingEuclideanDistanceforPointInfo.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2024.4.9.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/plotPointOnMap.py` & `pami-2024.4.9.1/PAMI/extras/plotPointOnMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #     from PAMI.extras.syntheticDataGenerator import plotPointOnMap as plt
 #
 #     obj = plt.plotPointOnMap(" ", 10, "\t")
 #
 #     obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.11.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2024.4.9.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 #
 #     from PAMI.extras.syntheticDataGenerator import plotPointOnMap_dump as plt
 #
 #     obj = plt.plotPointOnMap_dump(" ", 10, "\t")
 #
 #     obj.save()
 #
-
-
-
-
+#
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.11.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2024.4.9.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #   from PAMI.extras.syntheticDataGenerator import scatterPlotSpatialPoints as plt
 #
 #   obj = plt.scatterPlotSpatialPoints(iFile, "\t")
 #
 #   obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -50,14 +47,15 @@
 
                 from PAMI.extras.syntheticDataGenerator import scatterPlotSpatialPoints as plt
 
                 obj = plt.scatterPlotSpatialPoints(iFile, "\t" )
 
                 obj.save(oFile)
 
+
     """
 
     def __init__(self, iFile: str, sep: str = '\t') ->None:
 
         self._iFile = iFile
         self._sep = sep
```

### Comparing `pami-2024.4.11.1/PAMI/extras/stats/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/stats/graphDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/graphDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/stats/sequentialDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/sequentialDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/stats/temporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/temporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/stats/utilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/stats/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/TransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUncertainTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/generateUtilityTransactional.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/syntheticUtilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/temporalDatabaseGen.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py` & `pami-2024.4.9.1/PAMI/extras/syntheticDataGenerator/utilityDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/extras/topKPatterns.py` & `pami-2024.4.9.1/PAMI/extras/topKPatterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 #     from PAMI.extras.syntheticDataGenerator import topKPatterns as tK
 #
 #     obj = tK.topKPatterns(" ", 10, "\t")
 #
 #     obj.save()
 #
 
-
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.11.1/PAMI/extras/uncertaindb_convert.py` & `pami-2024.4.9.1/PAMI/extras/uncertaindb_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,16 @@
 #
 #     obj = un.predictedClass2Transaction(predicted_classes, 0.8)
 #
 #     obj.save()
 #
 
 
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
```

### Comparing `pami-2024.4.11.1/PAMI/extras/visualize/graphs.py` & `pami-2024.4.9.1/PAMI/extras/visualize/graphs.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
-#
+# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
+
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------
+# ---------------------------------------------------------
 #
-#             import PAMI.frequentPattern.basic.Apriori as alg
+#             import PAMI.frequentPattern.basic.ECLATDiffset as alg
 #
-#             obj = alg.Apriori(iFile, minSup)
+#             obj = alg.ECLATDiffset(iFile, minSup)
 #
 #             obj.mine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.save(oFile)
+#             obj.savePatterns(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -30,14 +30,15 @@
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
 
 
+
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -47,91 +48,89 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+
+# from abstract import *
+
 from PAMI.frequentPattern.basic import abstract as _ab
-from typing import List, Dict, Tuple, Set, Union, Any, Generator
 from deprecated import deprecated
-import numpy as np
 
-class Apriori(_ab._frequentPatterns):
-    """
-    :Description: Apriori is one of the fundamental algorithm to discover frequent patterns in a transactional database. This program employs apriori property (or downward closure property) to  reduce the search space effectively. This algorithm employs breadth-first search technique to find the complete set of frequent patterns in a transactional database.
 
-    :Reference:  Agrawal, R., Imieli ́nski, T., Swami, A.: Mining association rules between sets of items in large databases.
-            In: SIGMOD. pp. 207–216 (1993), https://doi.org/10.1145/170035.170072
+class ECLATDiffset(_ab._frequentPatterns):
+    """
+    :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
 
+    :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
+            August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
+            
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count. Otherwise, it will be treated as float.
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-
+    
     :Attributes:
-
+    
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
 
         finalPatterns : dict
           Storing the complete set of patterns in a dictionary variable
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
-
+        
         Database : list
           To store the transactions of a database in list
-
-
-
+          
+        
     **Methods to execute code on terminal**
-    ----------------------------------------------------
+    ------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 Apriori.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 Apriori.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
 
     .. note:: minSup will be considered in percentage of database transactions
 
-
+    
     **Importing this algorithm into a python program**
-    -----------------------------------------------------
-
+    ---------------------------------------------------------
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.Apriori as alg
+            import PAMI.frequentPattern.basic.ECLATDiffset as alg
 
-            obj = alg.Apriori(iFile, minSup)
+            obj = alg.ECLATDiffset(iFile, minSup)
 
             obj.mine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
             Df = obj.getPatternInDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
@@ -141,360 +140,283 @@
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
 
     **Credits:**
-    -------------
+    -------------------
 
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+               The complete program was written by Kundai under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _minSup = float()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
+    _diffSets = {}
+    _trans_set = set()
 
-    def _creatingItemSets(self) -> None:
+    def _creatingItemSets(self):
         """
         Storing the complete transactions of the database/input file in a database variable
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                temp = self._iFile['Transactions'].tolist()
-
-            for k in temp:
-                self._Database.append(set(k))
+                self._Database = self._iFile['Transactions'].tolist()
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(set(temp))
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(set(temp))
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _convert(self, value: Union[int, float, str]) -> Union[int, float]:
+    def _convert(self, value):
         """
         To convert the user specified minSup value
-
         :param value: user specified minSup value
-
-        :type value: int or float or str
-
         :return: converted type
-
-        :rtype: int or float
-
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
+    def _getUniqueItemList(self):
+
+        # tidSets will store all the initial tids
+        tidSets = {}
+        # uniqueItem will store all frequent 1 items
+        uniqueItem = []
+        for line in self._Database:
+                transNum = 0
+                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
+                for transaction in self._Database:
+                    transNum += 1
+                    self._trans_set.add(transNum)
+                    for item in transaction:
+                        if item in tidSets:
+                            tidSets[item].add(transNum)
+                        else:
+                            tidSets[item] = {transNum}
+        for key, value in tidSets.items():
+            supp = len(value)
+            if supp >= self._minSup:
+                self._diffSets[key] = [supp, self._trans_set.difference(value)]
+                uniqueItem.append(key)
+        # for x, y in self._diffSets.items():
+        #     print(x, y)
+        uniqueItem.sort()
+        # print()
+        return uniqueItem
+
+    def _runDeclat(self, candidateList):
+        """
+        It will generate the combinations of frequent items
+        :param candidateList :it represents the items with their respective transaction identifiers
+        :type candidateList: list
+        :return: returning transaction dictionary
+        :rtype: dict
+        """
+
+        newList = []
+        for i in range(0, len(candidateList)):
+            item1 = candidateList[i]
+            iList = item1.split()
+            for j in range(i + 1, len(candidateList)):
+                item2 = candidateList[j]
+                jList = item2.split()
+                if iList[:-1] == jList[:-1]:
+                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
+                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
+                    if unionSup >= self._minSup:
+                        newKey = item1 + "\t" + jList[-1]
+                        self._diffSets[newKey] = [unionSup, unionDiffSet]
+                        newList.append(newKey)
+                    else: 
+                        break
+
+        if len(newList) > 0:
+            self._runDeclat(newList)
 
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self) -> None:
+    def startMine(self):
         """
         Frequent pattern mining process will start from here
         """
-        self._Database = []
+
         self._startTime = _ab._time.time()
+        self._Database = []
+        self._finalPatterns = {}
+        self._diffSets = {}
+        self._trans_set = set()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        itemsList = sorted(list(set.union(*self._Database)))  # because Database is list
-        items = [{i} for i in itemsList]
-        itemsCount = len(items)
+        #print(len(self._Database))
         self._minSup = self._convert(self._minSup)
-        self._finalPatterns = {}
-        for i in range(1, itemsCount):
-            frequentSet = self._candidateToFrequent(items)
-            for x, y in frequentSet.items():
-                sample = str()
-                for k in x:
-                    sample = sample + k + "\t"
-                self._finalPatterns[sample] = y
-            items = self._frequentToCandidate(frequentSet, i + 1)
-            if len(items) == 0:
-                break  # finish apriori
+        uniqueItemList = []
+        uniqueItemList = self._getUniqueItemList()
+        self._runDeclat(uniqueItemList)
+        self._finalPatterns = self._diffSets
+        #print(len(self._finalPatterns), len(uniqueItemList))
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using Apriori algorithm ")
+        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
-    def bitPacker(self, data, maxIndex):
-        packed_bits = 0
-        for i in data:
-            packed_bits |= 1 << (maxIndex - i)
-
-        return packed_bits
-
-    # # @profile
-    # def mineLowMemory(self) -> None:
-    #     """
-    #     Frequent pattern mining process will start from here
-    #     # Bitset implementation
-    #     """
-    #     self._startTime = _ab._time.time()
-
-    #     self._Database = []
-
-    #     self._creatingItemSets()
-
-    #     self._minSup = self._convert(self._minSup)
-
-    #     items = {}
-    #     index = 0
-    #     for line in self._Database:
-    #         for item in line:
-    #             if tuple([item]) in items:
-    #                 items[tuple([item])].append(index)
-    #             else:
-    #                 items[tuple([item])] = [index]
-    #         index += 1
-
-    #     # sort by length in descending order
-    #     items = dict(sorted(items.items(), key=lambda x: len(x[1]), reverse=True))
-    #     cands = []
-    #     for key in items:
-    #         if len(items[key]) >= self._minSup:
-    #             self._finalPatterns[key] = len(items[key])
-    #             cands.append(key)
-    #             items[key] = self.bitPacker(items[key], index)
-    #         else:
-    #             break
-
-    #     while cands:
-    #         newCands = []
-    #         for i in range(len(cands)):
-    #             for j in range(i + 1, len(cands)):
-    #                 if cands[i][:-1] == cands[j][:-1]:
-    #                     newCand = tuple(cands[i] + tuple([cands[j][-1]]))
-    #                     intersection = items[tuple([newCand[0]])]
-    #                     for k in range(1, len(newCand)):
-    #                         intersection &= items[tuple([newCand[k]])]
-    #                     count = int.bit_count(intersection)
-    #                     if count >= self._minSup:
-    #                         # items[newCand] = intersection
-    #                         newCands.append(newCand)
-    #                         self._finalPatterns[newCand] = count
-    #                 else:
-    #                     break
-            
-    #         cands = newCands
-
-    #     self._endTime = _ab._time.time()
-    #     process = _ab._psutil.Process(_ab._os.getpid())
-    #     self._memoryUSS = float()
-    #     self._memoryRSS = float()
-    #     self._memoryUSS = process.memory_full_info().uss
-    #     self._memoryRSS = process.memory_info().rss
-    #     print("Frequent patterns were generated successfully using Apriori algorithm ")
-
-    def mine(self) -> None:
+    def mine(self):
         """
         Frequent pattern mining process will start from here
         """
-        self._Database = []
-        self._startTime = _ab._time.time()
 
+        self._startTime = _ab._time.time()
+        self._Database = []
+        self._finalPatterns = {}
+        self._diffSets = {}
+        self._trans_set = set()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-
+        #print(len(self._Database))
         self._minSup = self._convert(self._minSup)
-
-        items = {}
-        index = 0
-        for line in self._Database:
-            for item in line:
-                if tuple([item]) in items:
-                    items[tuple([item])].append(index)
-                else:
-                    items[tuple([item])] = [index]
-            index += 1
-
-        # sort by length in descending order
-        items = dict(sorted(items.items(), key=lambda x: len(x[1]), reverse=True))
-
-        cands = []
-        fileData = {}
-        for key in items:
-            if len(items[key]) >= self._minSup:
-                cands.append(key)
-                self._finalPatterns["\t".join(key)] = len(items[key])
-                fileData[key] = set(items[key])
-            else:
-                break
-
-
-        while cands:
-            newKeys = []
-            for i in range(len(cands)):
-                for j in range(i+1, len(cands)):
-                    if cands[i][:-1] == cands[j][:-1]:
-                        newCand = cands[i] + tuple([cands[j][-1]])
-                        intersection = fileData[tuple([newCand[0]])]
-                        for k in range(1, len(newCand)):
-                            intersection = intersection.intersection(fileData[tuple([newCand[k]])])
-                        if len(intersection) >= self._minSup:
-                            newKeys.append(newCand)
-                            newCand = "\t".join(newCand)
-                            self._finalPatterns[newCand] = len(intersection)
-            del cands
-            cands = newKeys
-            del newKeys
-            
-        process = _ab._psutil.Process(_ab._os.getpid())
+        uniqueItemList = []
+        uniqueItemList = self._getUniqueItemList()
+        self._runDeclat(uniqueItemList)
+        self._finalPatterns = self._diffSets
+        #print(len(self._finalPatterns), len(uniqueItemList))
         self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using Apriori algorithm ")
+        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
-    def getMemoryUSS(self) -> float:
+    def getMemoryUSS(self):
         """
-
         Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
-
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self) -> float:
+    def getMemoryRSS(self):
         """
-
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
-
         """
 
         return self._memoryRSS
 
-    def getRuntime(self) -> float:
+    def getRuntime(self):
         """
-
         Calculating the total amount of runtime taken by the mining process
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
-
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _ab._pd.DataFrame:
+    def getPatternsAsDataFrame(self):
         """
-
         Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
-
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
+            data.append([a.replace('\t', ' '), b[0]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
-    def save(self, outFile) -> None:
+    def save(self, outFile):
         """
-
         Complete set of frequent patterns will be loaded in to an output file
-
         :param outFile: name of the output file
-
         :type outFile: csvfile
-
-        :return: None
-
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y[0])
+            writer.write("%s \n" % patternsAndSupport)
 
-    def getPatterns(self) -> Dict[str, int]:
+    def getPatterns(self):
         """
-
         Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
-
         :rtype: dict
-
         """
         return self._finalPatterns
 
-    def printResults(self) -> None:
+    def printResults(self):
         """
-        This function is used to print the result
+        This function is used to print the results
         """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = Apriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = Apriori(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ap._sys.argv[2])
+        _ap.save(_ab._sys.argv[2])
+        print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
```

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/AprioriOLD.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,7 +443,8 @@
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ap._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
```

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2024.4.9.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ECLATDiffest uses diffset to extract the frequent patterns in a transactional database.
-
+# Top - K is and algorithm to discover top frequent patterns in a transactional database.
+#
 # **Importing this algorithm into a python program**
 # ---------------------------------------------------------
 #
-#             import PAMI.frequentPattern.basic.ECLATDiffset as alg
+#             import PAMI.frequentPattern.topK.FAE as alg
 #
-#             obj = alg.ECLATDiffset(iFile, minSup)
+#             obj = alg.FAE(iFile, K)
 #
 #             obj.mine()
 #
-#             frequentPatterns = obj.getPatterns()
+#             topKFrequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(frequentPatterns))
+#             print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 #
-#             obj.savePatterns(oFile)
+#             obj.save(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
@@ -30,15 +30,14 @@
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
 
 
-
 __copyright__ = """
 Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -48,136 +47,142 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-
-# from abstract import *
-
-from PAMI.frequentPattern.basic import abstract as _ab
+from PAMI.frequentPattern.topk import abstract as _ab
 from deprecated import deprecated
 
 
-class ECLATDiffset(_ab._frequentPatterns):
+class FAE(_ab._frequentPatterns):
     """
-    :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
+    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
+
+
+    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
+                  https://ieeexplore.ieee.org/document/4370261
 
-    :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
-            August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
-            
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent pattern's
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param  k: int :
+                    User specified count of top frequent patterns
+    :param minimum: int :
+                    Minimum number of frequent patterns to consider in analysis
+
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-    
+
+
+
     :Attributes:
-    
+
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
 
         finalPatterns : dict
           Storing the complete set of patterns in a dictionary variable
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
-        
-        Database : list
-          To store the transactions of a database in list
-          
-        
+
+        finalPatterns : dict
+            it represents to store the patterns
+
+
     **Methods to execute code on terminal**
-    ------------------------------------------
+    -------------------------------------------
 
     .. code-block:: console
 
       Format:
 
-      (.venv) $ python3 ECLATDiffset.py <inputFile> <outputFile> <minSup>
+      (.venv) $ python3 FAE.py <inputFile> <outputFile> <K>
 
       Example Usage:
 
-      (.venv) $ python3 ECLATDiffset.py sampleDB.txt patterns.txt 10.0
+      (.venv) $ python3 FAE.py sampleDB.txt patterns.txt 10
+
+    .. note:: k will be considered as count of top frequent patterns to consider in analysis
+
 
-    .. note:: minSup will be considered in percentage of database transactions
 
-    
     **Importing this algorithm into a python program**
     ---------------------------------------------------------
     .. code-block:: python
 
-            import PAMI.frequentPattern.basic.ECLATDiffset as alg
-
-            obj = alg.ECLATDiffset(iFile, minSup)
+        import PAMI.frequentPattern.topK.FAE as alg
 
-            obj.mine()
+        obj = alg.FAE(iFile, K)
 
-            frequentPatterns = obj.getPatterns()
+        obj.mine()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+        topKFrequentPatterns = obj.getPatterns()
 
-            obj.savePatterns(oFile)
+        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 
-            Df = obj.getPatternInDataFrame()
+        obj.save(oFile)
 
-            memUSS = obj.getMemoryUSS()
+        Df = obj.getPatternInDataFrame()
 
-            print("Total Memory in USS:", memUSS)
+        memUSS = obj.getMemoryUSS()
 
-            memRSS = obj.getMemoryRSS()
+        print("Total Memory in USS:", memUSS)
 
-            print("Total Memory in RSS", memRSS)
+        memRSS = obj.getMemoryRSS()
 
-            run = obj.getRuntime()
+        print("Total Memory in RSS", memRSS)
 
-            print("Total ExecutionTime in seconds:", run)
+        run = obj.getRuntime()
 
+        print("Total ExecutionTime in seconds:", run)
 
-    **Credits:**
-    -------------------
-
-               The complete program was written by Kundai under the supervision of Professor Rage Uday Kiran.
+    Credits:
+    --------
+        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
-    _minSup = float()
     _startTime = float()
     _endTime = float()
+    _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _diffSets = {}
-    _trans_set = set()
+    _tidList = {}
+    _minimum = int()
 
     def _creatingItemSets(self):
         """
-        Storing the complete transactions of the database/input file in a database variable
+            Storing the complete transactions of the database/input file in a database variable
+
         """
+
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
@@ -191,232 +196,293 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
+    def _frequentOneItem(self):
+        """
+        Generating one frequent patterns
+        """
+        candidate = {}
+        self._tidList = {}
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                if j not in candidate:
+                    candidate[j] = 1
+                    self._tidList[j] = [i]
+                else:
+                    candidate[j] += 1
+                    self._tidList[j].append(i)
+        self._finalPatterns = {}
+        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+        for i in plist:
+            if len(self._finalPatterns) >= self._k:
+                break
+            else:
+                self._finalPatterns[i] = candidate[i]
+        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        plist = list(self._finalPatterns.keys())
+        return plist
+
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
+
+            :param prefix: the prefix of a pattern
+            :type prefix: list
+            :param suffix: the suffix of a patterns
+            :type suffix: list
+            :param tidSetI: the timestamp of a patterns
+            :type tidSetI: list
+        """
+
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = len(tidSetI)
+        sample = str()
+        for i in prefix:
+            sample = sample + i + "\t"
+        if len(self._finalPatterns) < self._k:
+            if val > self._minimum:
+                self._finalPatterns[sample] = val
+                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                self._minimum = min([i for i in self._finalPatterns.values()])
+        else:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
+                if val > y:
+                    del self._finalPatterns[x]
+                    self._finalPatterns[sample] = val
+                    self._finalPatterns = {k: v for k, v in
+                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
+                                                     reverse=True)}
+                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    return
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+            :param prefix:  main equivalence prefix
+            :type prefix: periodic-frequent item or pattern
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
+            :type itemSets: list
+            :param tidSets: timestamps of the items in the argument itemSets
+            :type tidSets: list
+
+
+                    """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = list(set(tidSetI).intersection(tidSetJ))
+                if len(y) >= self._minimum:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
+
     def _convert(self, value):
         """
-        To convert the user specified minSup value
+        to convert the type of user specified minSup value
         :param value: user specified minSup value
+        :type value: int or float or str
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self._Database) * value)
+                value = ((len(self._Database)) * value)
             else:
                 value = int(value)
         return value
 
-    def _getUniqueItemList(self):
-
-        # tidSets will store all the initial tids
-        tidSets = {}
-        # uniqueItem will store all frequent 1 items
-        uniqueItem = []
-        for line in self._Database:
-                transNum = 0
-                # Database = [set([i.rstrip() for i in transaction.split('\t')]) for transaction in f]
-                for transaction in self._Database:
-                    transNum += 1
-                    self._trans_set.add(transNum)
-                    for item in transaction:
-                        if item in tidSets:
-                            tidSets[item].add(transNum)
-                        else:
-                            tidSets[item] = {transNum}
-        for key, value in tidSets.items():
-            supp = len(value)
-            if supp >= self._minSup:
-                self._diffSets[key] = [supp, self._trans_set.difference(value)]
-                uniqueItem.append(key)
-        # for x, y in self._diffSets.items():
-        #     print(x, y)
-        uniqueItem.sort()
-        # print()
-        return uniqueItem
-
-    def _runDeclat(self, candidateList):
-        """
-        It will generate the combinations of frequent items
-        :param candidateList :it represents the items with their respective transaction identifiers
-        :type candidateList: list
-        :return: returning transaction dictionary
-        :rtype: dict
-        """
-
-        newList = []
-        for i in range(0, len(candidateList)):
-            item1 = candidateList[i]
-            iList = item1.split()
-            for j in range(i + 1, len(candidateList)):
-                item2 = candidateList[j]
-                jList = item2.split()
-                if iList[:-1] == jList[:-1]:
-                    unionDiffSet = self._diffSets[item2][1].difference(self._diffSets[item1][1])
-                    unionSup = self._diffSets[item1][0] - len(unionDiffSet)
-                    if unionSup >= self._minSup:
-                        newKey = item1 + "\t" + jList[-1]
-                        self._diffSets[newKey] = [unionSup, unionDiffSet]
-                        newList.append(newKey)
-                    else: 
-                        break
-
-        if len(newList) > 0:
-            self._runDeclat(newList)
-
     @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self):
         """
-        Frequent pattern mining process will start from here
+            Main function of the program
         """
-
         self._startTime = _ab._time.time()
-        self._Database = []
-        self._finalPatterns = {}
-        self._diffSets = {}
-        self._trans_set = set()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._k is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        #print(len(self._Database))
-        self._minSup = self._convert(self._minSup)
-        uniqueItemList = []
-        uniqueItemList = self._getUniqueItemList()
-        self._runDeclat(uniqueItemList)
-        self._finalPatterns = self._diffSets
-        #print(len(self._finalPatterns), len(uniqueItemList))
+        self._k = self._convert(self._k)
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i + 1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                if len(y1) >= self._minimum:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
     def mine(self):
         """
-        Frequent pattern mining process will start from here
+            Main function of the program
         """
-
         self._startTime = _ab._time.time()
-        self._Database = []
-        self._finalPatterns = {}
-        self._diffSets = {}
-        self._trans_set = set()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._k is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        #print(len(self._Database))
-        self._minSup = self._convert(self._minSup)
-        uniqueItemList = []
-        uniqueItemList = self._getUniqueItemList()
-        self._runDeclat(uniqueItemList)
-        self._finalPatterns = self._diffSets
-        #print(len(self._finalPatterns), len(uniqueItemList))
+        self._k = self._convert(self._k)
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i + 1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                if len(y1) >= self._minimum:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Frequent patterns were generated successfully using ECLAT Diffset algorithm")
 
     def getMemoryUSS(self):
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """
         Calculating the total amount of runtime taken by the mining process
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
         Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b[0]])
+            data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
         """
         Complete set of frequent patterns will be loaded in to an output file
+
         :param outFile: name of the output file
-        :type outFile: csvfile
+
+        :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y[0])
+            patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
+    def printTOPK(self):
         """
         This function is used to print the results
         """
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Top K Frequent  Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = ECLATDiffset(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _ap.mine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print(_ap.getPatternsAsDataFrame())
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
+
```

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2024.4.9.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2024.4.9.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
         self._startTime = _ab._time.time()
 
         conf = _SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
         sc = _SparkContext(conf=conf)
 
         rdd = sc.textFile(self._iFile, self._numPartitions)\
-            .map(lambda x: x.rstrip().split(self._sep))\
+            .map(lambda x: x.rstrip().split('\t'))\
             .persist()
 
         self._lno = rdd.count()
         self._minSup = self._convert(self._minSup)
 
         freqItems = rdd.flatMap(lambda trans: [(item, 1) for item in trans])\
             .reduceByKey(add)\
@@ -311,15 +311,15 @@
 
         self._startTime = _ab._time.time()
 
         conf = _SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
         sc = _SparkContext(conf=conf)
 
         rdd = sc.textFile(self._iFile, self._numPartitions)\
-            .map(lambda x: x.rstrip().split(self._sep))\
+            .map(lambda x: x.rstrip().split('\t'))\
             .persist()
 
         self._lno = rdd.count()
         self._minSup = self._convert(self._minSup)
 
         freqItems = rdd.flatMap(lambda trans: [(item, 1) for item in trans])\
             .reduceByKey(add)\
```

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# Top - K is and algorithm to discover top frequent patterns in a transactional database.
-#
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# --------------------------------------------------------
 #
-#             import PAMI.frequentPattern.topK.FAE as alg
+
+#             import PAMI.periodicFrequentPattern.kPFPMiner as alg
 #
-#             obj = alg.FAE(iFile, K)
+#             obj = alg.kPFPMiner(iFile, k)
 #
-#             obj.mine()
+#             obj.startMine()
 #
-#             topKFrequentPatterns = obj.getPatterns()
+#             periodicFrequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+#             print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -28,150 +27,171 @@
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
 
-
-
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
+
 """
 
-from PAMI.frequentPattern.topk import abstract as _ab
+from PAMI.periodicFrequentPattern.basic import abstract as _ab
+import pandas as pd
 from deprecated import deprecated
 
+from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
 
-class FAE(_ab._frequentPatterns):
-    """
-    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
 
+class kPFPMiner(_ab._periodicFrequentPatterns):
+    """
+    :Description:   Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
 
-    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
-                  https://ieeexplore.ieee.org/document/4370261
+    :Reference:   Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
+                  Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
+                 BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of periodic frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  k: int :
-                    User specified count of top frequent patterns
-    :param minimum: int :
-                    Minimum number of frequent patterns to consider in analysis
+                   Name of the output file to store complete set of periodic frequent pattern's
 
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
-
-
     :Attributes:
 
-        startTime : float
-          To record the start time of the mining process
-
-        endTime : float
-          To record the completion time of the mining process
-
-        finalPatterns : dict
-          Storing the complete set of patterns in a dictionary variable
-
+        iFile : str
+            Input file name or path of the input file
+        k: int
+            User specified counte of top-k periodic frequent patterns
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
+        oFile : str
+            Name of the output file or the path of the output file
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        finalPatterns: dict
+            Storing the complete set of patterns in a dictionary variable
         memoryUSS : float
-          To store the total amount of USS memory consumed by the program
-
+            To store the total amount of USS memory consumed by the program
         memoryRSS : float
-          To store the total amount of RSS memory consumed by the program
-
-        finalPatterns : dict
-            it represents to store the patterns
+            To store the total amount of RSS memory consumed by the program
 
+    :Methods:
 
-    **Methods to execute code on terminal**
-    -------------------------------------------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        savePatterns(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingItemSets()
+            Scans the dataset or dataframes and stores in list format
+        frequentOneItem()
+            Generates one frequent patterns
+        eclatGeneration(candidateList)
+            It will generate the combinations of frequent items
+        generateFrequentPatterns(tidList)
+            It will generate the combinations of frequent items from a list of items
 
+    **Executing the code on terminal:**
+    ------------------------------------------
     .. code-block:: console
 
-      Format:
 
-      (.venv) $ python3 FAE.py <inputFile> <outputFile> <K>
+       Format:
 
-      Example Usage:
 
-      (.venv) $ python3 FAE.py sampleDB.txt patterns.txt 10
+       (.venv) $ python3 kPFPMiner.py <inputFile> <outputFile> <k>
 
-    .. note:: k will be considered as count of top frequent patterns to consider in analysis
+       Examples :
 
+       (.venv) $  python3 kPFPMiner.py sampleDB.txt patterns.txt 10
 
 
-    **Importing this algorithm into a python program**
-    ---------------------------------------------------------
+    **Sample run of the importing code:
+    --------------------------------------
     .. code-block:: python
 
-        import PAMI.frequentPattern.topK.FAE as alg
+            import PAMI.periodicFrequentPattern.kPFPMiner as alg
 
-        obj = alg.FAE(iFile, K)
+            obj = alg.kPFPMiner(iFile, k)
 
-        obj.mine()
+            obj.startMine()
 
-        topKFrequentPatterns = obj.getPatterns()
+            periodicFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
-        obj.save(oFile)
+            obj.save(oFile)
 
-        Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-        memUSS = obj.getMemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
-        print("Total Memory in USS:", memUSS)
+            print("Total Memory in USS:", memUSS)
 
-        memRSS = obj.getMemoryRSS()
+            memRSS = obj.getMemoryRSS()
 
-        print("Total Memory in RSS", memRSS)
+            print("Total Memory in RSS", memRSS)
 
-        run = obj.getRuntime()
+            run = obj.getRuntime()
 
-        print("Total ExecutionTime in seconds:", run)
+            print("Total ExecutionTime in seconds:", run)
 
-    Credits:
-    --------
-        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    **Credits:**
+    --------------
+            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _startTime = float()
     _endTime = float()
     _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _tidList = {}
-    _minimum = int()
+    lno = int()
+    _maximum = int()
 
     def _creatingItemSets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
-
+        Storing the complete transactions of the database/input file in a database variable
         """
 
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
@@ -195,88 +215,109 @@
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
+                    
+    def getPer_Sup(self, tids):
+        tids.sort()
+        cur=0
+        per=list()
+        sup=0
+        #print(tids)
+        for i in range(len(tids)-1):
+            j = i + 1
+            #if tids[j] - cur <= periodicity:
+                #return [0,0]
+            per.append(tids[j] - cur)
+            cur = tids[j]
+        per.append(self.lno - cur)
+        return max(per)
 
     def _frequentOneItem(self):
         """
         Generating one frequent patterns
         """
-        candidate = {}
+        self._mapSupport = {}
         self._tidList = {}
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                if j not in candidate:
-                    candidate[j] = 1
-                    self._tidList[j] = [i]
+        n = 0
+        for line in self._Database:
+            self.lno += 1
+            n = int(line[0])
+            for i in range(1, len(line)):
+                si = line[i]
+                if self._mapSupport.get(si) is None:
+                    self._mapSupport[si] = [1, abs(0 - n), n]
+                    self._tidList[si] = [n]
                 else:
-                    candidate[j] += 1
-                    self._tidList[j].append(i)
-        self._finalPatterns = {}
-        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+                    self._mapSupport[si][0] += 1
+                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
+                    self._mapSupport[si][2] = n
+                    self._tidList[si].append(n)
+        for x, y in self._mapSupport.items():
+            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
+        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in plist:
             if len(self._finalPatterns) >= self._k:
                 break
             else:
-                self._finalPatterns[i] = candidate[i]
-        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+                self._finalPatterns[i] = self._mapSupport[i][1]
+        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
         plist = list(self._finalPatterns.keys())
         return plist
 
+
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
 
-            :param prefix: the prefix of a pattern
-            :type prefix: list
-            :param suffix: the suffix of a patterns
-            :type suffix: list
-            :param tidSetI: the timestamp of a patterns
-            :type tidSetI: list
+        :param prefix: the prefix of a pattern
+        :type prefix: list
+        :param suffix: the suffix of a patterns
+        :type suffix: list
+        :param tidSetI: the timestamp of a patterns
+        :type tidSetI: list
         """
 
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = len(tidSetI)
+        val = self.getPer_Sup(tidSetI)
         sample = str()
         for i in prefix:
-            sample = sample + i + "\t"
+            sample = sample + i + " "
         if len(self._finalPatterns) < self._k:
-            if val > self._minimum:
+            if val < self._maximum:
                 self._finalPatterns[sample] = val
                 self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._minimum = min([i for i in self._finalPatterns.values()])
+                self._maximum = max([i for i in self._finalPatterns.values()])
         else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
-                if val > y:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
+                if val < y:
                     del self._finalPatterns[x]
                     self._finalPatterns[sample] = val
                     self._finalPatterns = {k: v for k, v in
                                               sorted(self._finalPatterns.items(), key=lambda item: item[1],
                                                      reverse=True)}
-                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    self._maximum = max([i for i in self._finalPatterns.values()])
                     return
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
-            :param prefix:  main equivalence prefix
-            :type prefix: periodic-frequent item or pattern
-            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
-                            and frequent with their timestamps
-            :type itemSets: list
-            :param tidSets: timestamps of the items in the argument itemSets
-            :type tidSets: list
+        :param prefix:  main equivalence prefix
+        :type prefix: periodic-frequent item or pattern
+        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
+        :type itemSets: list
+        :param tidSets: timestamps of the items in the argument itemSets
+        :type tidSets: list
 
-
-                    """
+        """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
         for i in range(len(itemSets)):
             itemI = itemSets[i]
@@ -286,78 +327,44 @@
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
                 y = list(set(tidSetI).intersection(tidSetJ))
-                if len(y) >= self._minimum:
+                if self.getPer_Sup(y) <= self._maximum:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
             self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
+
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = ((len(self._Database)) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self):
         """
-            Main function of the program
-        """
-        self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
-        self._creatingItemSets()
-        self._k = self._convert(self._k)
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i + 1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                if len(y1) >= self._minimum:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
-        self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        Main function of the program
 
-    def mine(self):
-        """
-            Main function of the program
         """
         self._startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         if self._k is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
@@ -369,120 +376,109 @@
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i + 1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
                 y1 = list(set(tidSetI).intersection(tidSetJ))
-                if len(y1) >= self._minimum:
+                if self.getPer_Sup(y1) <= self._maximum:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
+        print("kPFPMiner has successfully generated top-k frequent patterns")
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
-        """
-        Storing final frequent patterns in a dataframe
+        """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            data.append([a, b])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
         return dataFrame
 
     def save(self, outFile):
-        """
-        Complete set of frequent patterns will be loaded in to an output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
+            patternsAndSupport = x + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
-        """
-        Function to send the set of frequent patterns after completion of the mining process
+        """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
-
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printTOPK(self):
-        """
-        This function is used to print the results
-        """
-        print("Top K Frequent  Patterns:", len(self.getPatterns()))
+    def printResults(self):
+        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        _ap.mine()
-        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
+        _Patterns = _ap.getPatterns()
+        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2024.4.11.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/F3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyPartialPeriodicPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2024.4.9.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,45 @@
 # lengths where a pattern is continuously periodic, while the minDur (minimal duration) measure ensures that those
 # time-intervals have a minimum duration.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#             from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
 #
-#             obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
+#
+#     print(f'Total execution time in seconds: {runtime})
 #
-#             print(f'Total execution time in seconds: {runtime})
 #
-
-
-
 
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -58,15 +56,14 @@
 
 """
 
 
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
-from deprecated import deprecated
 
 class Node:
     """
     A class used to represent the node of localPeriodicPatternTree
 
     :Attributes:
 
@@ -93,22 +90,16 @@
         self.child = []
         self.nodeLink = None
         self.tidList = set()
 
     def getChild(self, item: int) -> 'Node':
         """
         This function is used to get child node from the parent node
-
-        :param item: item of the parent node
-
-        :type item: int
-
+        :param item:
         :return: if node have node of item, then return it. if node don't have return []
-
-        :rtype: Node
         """
         for child in self.child:
             if child.item == item:
                 return child
         return []
 
 
@@ -146,15 +137,14 @@
         """
         add transaction into tree
 
         :param transaction: it represents the one transaction in database
         :type transaction: list
         :param tid: represents the timestamp of transaction
         :type tid: list or int
-        :return: None
         """
         current = self.root
         for item in transaction:
             child = current.getChild(item)
             if not child:
                 newNode = Node()
                 newNode.item = item
@@ -170,30 +160,28 @@
         """
         fix node link
 
         :param item: it represents item name of newNode
         :type item: string
         :param newNode: it represents node which is added
         :type newNode: Node
-        :return: None
         """
         if item in self.nodeLinks:
             lastNode = self.nodeLinks[item]
             lastNode.nodeLink = newNode
         self.nodeLinks[item] = newNode
         if item not in self.firstNodeLink:
             self.firstNodeLink[item] = newNode
 
     def deleteNode(self, item: int) -> None:
         """
         delete the node from tree
 
         :param item: it represents the item name of node
         :type item: str
-        :return: None
         """
         deleteNode = self.firstNodeLink[item]
         parentNode = deleteNode.parent
         parentNode.child.remove(deleteNode)
         parentNode.child += deleteNode.child
         parentNode.tidList |= deleteNode.tidList
         for child in deleteNode.child:
@@ -211,15 +199,14 @@
         """
         create prefix tree by path
 
         :param path: it represents path to root from prefix node
         :type path: list
         :param tidList: it represents tid of each item
         :type tidList: list
-        :return: None
         """
         currentNode = self.root
         for item in path:
             child = currentNode.getChild(item)
             if not child:
                 newNode = Node()
                 newNode.item = item
@@ -244,17 +231,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -308,15 +295,15 @@
                 Create LPPTree of local periodic item from input data.
             patternGrowth(tree, prefix, prefixPFList)
                 Execute pattern growth algorithm. It is important function in this program.
             calculatePTL(tsList)
                 Calculate PTL from input tsList as integer list.
             calculatePTLbit(tsList)
                 Calculate PTL from input tsList as bit vector.
-            mine()
+            startMine()
                 Mining process will start from here.
             getMemoryUSS()
                 Total amount of USS memory consumed by the mining process will be retrieved from this function.
             getMemoryRSS()
                 Total amount of RSS memory consumed by the mining process will be retrieved from this function.
             getRuntime()
                 Total amount of runtime taken by the mining process will be retrieved from this function.
@@ -324,38 +311,31 @@
                 return local periodic patterns and its PTL
             save(oFile)
                 Complete set of local periodic patterns will be loaded in to an output file.
             getPatternsAsDataFrame()
                 Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    ---------------------------------------
-
-    .. code-block:: console
-
-      Format:
+    -------------------------------------
+            Format:
+                    >>> python3 LPPMGrowth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
 
-      (.venv) $ python3 LPPMGrowth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
-
-      Example Usage:
-
-      (.venv) $ python3 LPPMGrowth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+            Examples:
+                    >>> python3 LPPMGrowth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
 
     **Sample run of importing the code:**
     ----------------------------------------
     .. code-block:: python
 
             from PAMI.localPeriodicPattern.basic import LPPGrowth as alg
 
             obj = alg.LPPGrowth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -601,15 +581,14 @@
 
         :param tree: The root node of prefix tree.
         :type tree: Node or Tree
         :param prefix: Prefix item list.
         :type prefix: list
         :param prefixPFList: tsList of prefix patterns.
         :type prefixPFList: dict or list
-        :return: None
         """
         items = list(prefixPFList)
         if not prefix:
             items = reversed(items)
         for item in items:
             prefixCopy = prefix.copy()
             prefixCopy.append(item)
@@ -658,15 +637,14 @@
     def __calculatePTL(self, tsList: List[int]) -> set:
         """
         Calculate PTL from input tsList as integer list
 
         :param tsList: It is tsList which store time stamp as integer.
         :type tsList: list
         :return: PTL
-        :rtype: set
         """
         start = -1
         PTL = set()
         tsList = sorted(tsList)
         tsPre = tsList[0]
         soPer = ' '
         for ts in tsList[1:]:
@@ -692,15 +670,14 @@
     def __calculatePTLbit(self, tsList: List[int]) -> set:
         """
         Calculate PTL from input tsList as bit vector.
 
         :param tsList: It is tsList which store time stamp as bit vector.
         :type tsList: list
         :return: PTL
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -739,31 +716,28 @@
         return PTL
 
     def __convert(self, value: Any) -> float:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
         Mining process start from here.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self._localPeriodicPatterns__finalPatterns = {}
         self.__creatingItemSets()
@@ -777,68 +751,43 @@
         self._localPeriodicPatterns__endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
-        """
-        Mining process start from here.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self.__createTSList()
-        self.__generateLPP()
-        self.__createLPPTree()
-        self.__patternGrowth(self.__root, [], self.__items)
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
-
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
     def getPatternsAsDataFrame(self) -> '_ab._pd.DataFrame':
-        """
-        Storing final local periodic patterns in a dataframe
+        """Storing final local periodic patterns in a dataframe
 
         :return: returning local periodic patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
@@ -852,31 +801,29 @@
 
     def save(self, outFile: str) -> None:
         """
         Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -893,15 +840,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,46 +5,43 @@
 # time-intervals have a minimum duration.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
 #
-#             obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
 #
-#             print(f'Total execution time in seconds: {runtime})
-#
-
-
+#     print(f'Total execution time in seconds: {runtime})
 
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -57,16 +54,14 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
 import pandas as pd
-from deprecated import deprecated
-
 
 class LPPMBreadth(_ab._localPeriodicPatterns):
 
     """
     :Description:
 
         Local Periodic Patterns, which are patterns (sets of events) that have a periodic behavior in some non predefined
@@ -77,17 +72,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -128,15 +123,15 @@
             Create the tsList as bit vector from input data.
         generateLPP()
             Generate 1 length local periodic pattens by tsList and execute depth first search.
         calculatePTL(tsList)
             Calculate PTL from input tsList as bit vector
         LPPMBreathSearch(extensionOfP)
             Mining local periodic patterns using breadth first search.
-        mine()
+        startMine()
             Mining process will start from here.
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function.
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function.
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function.
@@ -144,37 +139,29 @@
             return local periodic patterns and its PTL
         save(oFile)
             Complete set of local periodic patterns will be loaded in to an output file.
         getPatternsAsDataFrame()
             Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    --------------------------------------
-
-    .. code-block:: console
-
-      Format:
-
-      (.venv) $ python3 LPPBreadth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
-
-      Example Usage:
-
-      (.venv) $ python3 LPPMBreadth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+    ------------------------------------
+            Format:
+                >>> python3 LPPBreadth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
+            Examples:
+                >>> python3 LPPMBreadth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
     **Sample run of importing the code:**
     -------------------------------------
     .. code-block:: python
     
             from PAMI.localPeriodicPattern.basic import LPPMBreadth as alg
 
             obj = alg.LPPMBreadth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -358,15 +345,14 @@
     def __calculatePTL(self, tsList: int) -> Set[Tuple[int, int]]:
         """
         calculate PTL from tsList as bit vector.
 
         :param tsList: it is one item's tsList which is used bit vector.
         :type tsList: int
         :return: it is PTL of input item.
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -451,31 +437,28 @@
         return w1map
 
     def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: int or float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
     def startMine(self) -> None:
         """
         Mining process start from here.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self.__creatingItemSets()
         self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
@@ -487,66 +470,43 @@
         self._localPeriodicPatterns__endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
-        """
-        Mining process start from here.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__createTSList()
-        self.__generateLPP()
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
-
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
     def getPatternsAsDataFrame(self) -> pd.DataFrame:
-        """
-        Storing final local periodic patterns in a dataframe
+        """Storing final local periodic patterns in a dataframe
 
         :return: returning local periodic patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
@@ -555,36 +515,33 @@
             for i in a:
                 pat = pat + i + ' '
             data.append([pat, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'PTL'])
         return dataFrame
 
     def save(self, outFile: str) -> None:
-        """
-        Complete set of local periodic patterns will be loaded in to an output file
+        """Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict[Union[Tuple[str, ...], str], Set[Tuple[int, int]]]:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -601,15 +558,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPMBreadth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPMBreadth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,46 +4,42 @@
 # lengths where a pattern is continuously periodic, while the minDur (minimal duration) measure ensures that those
 # time-intervals have a minimum duration.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
+#     from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
 #
-#             obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
+#     obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
 #
-#             obj.mine()
+#     obj.startMine()
 #
-#             localPeriodicPatterns = obj.getPatterns()
+#     localPeriodicPatterns = obj.getPatterns()
 #
-#             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
+#     print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 #
-#             obj.save(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print(f'Total memory in USS: {memUSS}')
+#     print(f'Total memory in USS: {memUSS}')
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print(f'Total memory in RSS: {memRSS}')
+#     print(f'Total memory in RSS: {memRSS}')
 #
-#             runtime = obj.getRuntime()
+#     runtime = obj.getRuntime()
 #
-#             print(f'Total execution time in seconds: {runtime})
-#
-
-
-
+#     print(f'Total execution time in seconds: {runtime})
 
 __copyright__ = """
-Copyright (C)  2021 Rage Uday Kiran
+ Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
@@ -56,16 +52,14 @@
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 from PAMI.localPeriodicPattern.basic import abstract as _ab
 from typing import List, Dict, Tuple, Set, Union, Any, Generator
 import pandas as pd
-from deprecated import deprecated
-
 
 class LPPMDepth(_ab._localPeriodicPatterns):
 
     """
     :Description:
 
         Local Periodic Patterns, which are patterns (sets of events) that have a periodic behavior in some non predefined
@@ -76,17 +70,17 @@
 
     :Reference:
 
         Fournier-Viger, P., Yang, P., Kiran, R. U., Ventura, S., Luna, J. M.. (2020). Mining Local Periodic Patterns in
         a Discrete Sequence. Information Sciences, Elsevier, to appear. [ppt] DOI: 10.1016/j.ins.2020.09.044
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of local periodic pattern's
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
-                   Name of the output file to store complete set of local periodic patterns
+                   Name of the output file to store complete set of frequent patterns
     :param  minDur: str:
                    Minimal duration in seconds between consecutive periods of time-intervals where a pattern is continuously periodic.
     :param  maxPer: float:
                    Controls the maximum number of transactions in which any two items within a pattern can reappear.
     :param  maxSoPer: float:
                    Controls the maximum number of time periods between consecutive periods of time-intervals where a pattern is continuously periodic.
 
@@ -142,38 +136,32 @@
             return local periodic patterns and its PTL
         save(oFile)
             Complete set of local periodic patterns will be loaded in to an output file.
         getPatternsAsDataFrame()
             Complete set of local periodic patterns will be loaded in to a dataframe.
 
     **Executing the code on terminal:**
-    --------------------------------------
-
-    .. code-block:: console
-
-      Format:
-
-      (.venv) $ python3 LPPMDepth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur>
+    -------------------------------------
+            Format:
 
-      Example Usage:
+                >>> python3 LPPMDepth.py <inputFile> <outputFile> <maxPer> <minSoPer> <minDur> <sep>
+            Examples:
 
-      (.venv) $ python3 LPPMDepth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
-
-    .. note: minDur will be considered as time interval between two consecutive periods
+                >>> python3 LPPMDepth.py sampleDB.txt patterns.txt 0.3 0.4 0.5
 
 
     **Sample run of importing the code:**
     ----------------------------------------
     .. code-block:: python
 
             from PAMI.localPeriodicPattern.basic import LPPMDepth as alg
 
             obj = alg.LPPMDepth(iFile, maxPer, maxSoPer, minDur)
 
-            obj.mine()
+            obj.startMine()
 
             localPeriodicPatterns = obj.getPatterns()
 
             print(f'Total number of local periodic patterns: {len(localPeriodicPatterns)}')
 
             obj.save(oFile)
 
@@ -341,20 +329,19 @@
                 self._localPeriodicPatterns__finalPatterns[item] = PTL[item]
         I = sorted(list(I))
         # I = set(I)
         self.__LPPMDepthSearch(I)
 
     def __calculatePTL(self, tsList: int) -> Set[Tuple[int, int]]:
         """
-        calculate PTL from tsList as bit vector.
+         calculate PTL from tsList as bit vector.
 
         :param tsList: it is one item's tsList which is used bit vector.
         :type tsList: int
         :return: it is PTL of input item.
-        :rtype: set
         """
         tsList = list(bin(tsList))
         tsList = tsList[2:]
         start = -1
         currentTs = 1
         PTL = set()
         tsPre = ' '
@@ -394,15 +381,14 @@
 
     def __LPPMDepthSearch(self, extensionsOfP: List[Union[Tuple[str, ...], str]]) -> None:
         """
         Mining n-length local periodic pattens from n-1-length patterns by depth first search.
 
         :param extensionsOfP: it is n-1 length patterns list.
         :type extensionsOfP: list
-        :return: None
         """
         for x in range(len(extensionsOfP)-1):
             extensionsOfPx = set()
             for y in range(x+1,len(extensionsOfP)):
                 tspxy = self.__tsList[extensionsOfP[x]] & self.__tsList[extensionsOfP[y]]
                 PTL = self.__calculatePTL(tspxy)
                 if len(PTL) > 0:
@@ -422,51 +408,30 @@
                 self.__LPPMDepthSearch(list(extensionsOfPx))
 
     def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
-        :type value: int or float or str
         :return: converted type
-        :rtype: int or float
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
                 value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    @deprecated("It is recommended to use 'mine()' instead of 'startMine()' for mining process. Starting from January 2025, 'startMine()' will be completely terminated.")
-    def startMine(self) -> None:
-        """
-        Mining process start from here. This function calls createTSlist and generateLPP.
-        """
-        self._localPeriodicPatterns__startTime = _ab._time.time()
-        self._localPeriodicPatterns__finalPatterns = {}
-        self.__creatingItemSets()
-        self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
-        self._localPeriodicPatterns__maxSoPer = self.__convert(self._localPeriodicPatterns__maxSoPer)
-        self._localPeriodicPatterns__minDur = self.__convert(self._localPeriodicPatterns__minDur)
-        self.__createTSlist()
-        self.__generateLPP()
-        self._localPeriodicPatterns__endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._localPeriodicPatterns__memoryRSS = float()
-        self._localPeriodicPatterns__memoryUSS = float()
-        self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
-        self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
-    def mine(self) -> None:
+    def startMine(self) -> None:
         """
         Mining process start from here. This function calls createTSlist and generateLPP.
         """
         self._localPeriodicPatterns__startTime = _ab._time.time()
         self._localPeriodicPatterns__finalPatterns = {}
         self.__creatingItemSets()
         self._localPeriodicPatterns__maxPer = self.__convert(self._localPeriodicPatterns__maxPer)
@@ -478,36 +443,33 @@
         process = _ab._psutil.Process(_ab._os.getpid())
         self._localPeriodicPatterns__memoryRSS = float()
         self._localPeriodicPatterns__memoryUSS = float()
         self._localPeriodicPatterns__memoryUSS = process.memory_full_info().uss
         self._localPeriodicPatterns__memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryUSS
 
     def getMemoryRSS(self) -> float:
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__memoryRSS
 
     def getRuntime(self) -> float:
-        """
-        Calculating the total amount of runtime taken by the mining process
+        """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._localPeriodicPatterns__endTime - self._localPeriodicPatterns__startTime
 
@@ -531,31 +493,29 @@
 
     def save(self, outFile: str) -> None:
         """
         Complete set of local periodic patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
-        :return: None
         """
         self._localPeriodicPatterns__oFile = outFile
         writer = open(self._localPeriodicPatterns__oFile, 'w+')
         for x, y in self._localPeriodicPatterns__finalPatterns.items():
             pat = str()
             for i in x:
                 pat = pat + i + '\t'
             pat = pat + ":"
             for i in y:
                 pat = pat + str(i) + '\t'
             patternsAndPTL = pat.strip()
             writer.write("%s \n" % patternsAndPTL)
 
     def getPatterns(self) -> Dict[Union[Tuple[str, ...], str], Set[Tuple[int, int]]]:
-        """
-        Function to send the set of local periodic patterns after completion of the mining process
+        """ Function to send the set of local periodic patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._localPeriodicPatterns__finalPatterns
 
     def printResults(self) -> None:
@@ -572,15 +532,14 @@
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
             _ap = LPPMDepth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = LPPMDepth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        _ap.mine()
         print("Total number of Local Periodic Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.11.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/__init__.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/pyspark/parallel3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2024.4.9.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/basic/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2024.4.9.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+# Stable periodic pattern mining aims to discover all interesting patterns in a temporal database using three constraints minimum support,
+# maximum period and maximum liability, that have support no less than the user-specified minimum support  constraint and liability no
+# greater than maximum liability.
+#
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-
-#             import PAMI.periodicFrequentPattern.kPFPMiner as alg
 #
-#             obj = alg.kPFPMiner(iFile, k)
+#             from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
+#
+#             obj = alg.SPPEclat("../basic/sampleTDB.txt", 5, 3, 3)
 #
 #             obj.startMine()
 #
-#             periodicFrequentPatterns = obj.getPatterns()
+#             Patterns = obj.getPatterns()
 #
-#             print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#             print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
 #
-#             obj.save(oFile)
+#             obj.save("patterns")
 #
-#             Df = obj.getPatternInDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
@@ -45,164 +49,205 @@
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
-
-from PAMI.periodicFrequentPattern.basic import abstract as _ab
 import pandas as pd
 from deprecated import deprecated
 
-from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
+from PAMI.stablePeriodicFrequentPattern.basic import abstract as _ab
 
-
-class kPFPMiner(_ab._periodicFrequentPatterns):
+class SPPEclat(_ab._stablePeriodicFrequentPatterns):
     """
-    :Description:   Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
+    :Description:   Stable periodic pattern mining aims to dicover all interesting patterns in a temporal database using three contraints minimum support,
+                    maximum period and maximum lability, that have support no less than the user-specified minimum support  constraint and lability no
+                    greater than maximum lability.
 
-    :Reference:   Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
-                  Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
-                 BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
+    :Reference:   Fournier-Viger, P., Yang, P., Lin, J. C.-W., Kiran, U. (2019). Discovering Stable Periodic-Frequent Patterns in Transactional Data. Proc.
+                  32nd Intern. Conf. on Industrial, Engineering and Other Applications of Applied Intelligent Systems (IEA AIE 2019), Springer LNAI, pp. 230-244
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of periodic frequent pattern's
+                   Name of the Input file to mine complete set of stable periodic Frequent Pattern.
     :param  oFile: str :
-                   Name of the output file to store complete set of periodic frequent pattern's
-
+                   Name of the output file to store complete set of stable periodic Frequent Pattern.
+    :param  minSup: float or int or str :
+                    The user can specify minSup either in count or proportion of database size.
+                    If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+                    Otherwise, it will be treated as float.
+                    Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+    :param  itemSup: int or float :
+                    Frequency of an item
+    :param maxLa: float :
+                  minimum loss of a pattern
     :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+                 This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+
 
     :Attributes:
 
-        iFile : str
-            Input file name or path of the input file
-        k: int
-            User specified counte of top-k periodic frequent patterns
+        iFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup : int or float or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        maxPer : int or float or str
+            The user can specify maxPer either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        maxLa : int or float or str
+            The user can specify maxLa either in count or proportion of database size.
+            If the program detects the data type of maxLa is integer, then it treats maxLa is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxLa=10 will be treated as integer, while maxLa=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
-        oFile : str
-            Name of the output file or the path of the output file
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
-        finalPatterns: dict
-            Storing the complete set of patterns in a dictionary variable
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            it represents the total no of transactions
+        tree : class
+            it represents the Tree class
+        itemSetCount : int
+            it represents the total no of patterns
+        finalPatterns : dict
+            it represents to store the patterns
+        tidList : dict
+            stores the timestamps of an item
 
     :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        savePatterns(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
+        save(oFile)
+            Complete set of periodic-frequent patterns will be loaded in to an output file
         getPatternsAsDataFrame()
-            Complete set of frequent patterns will be loaded in to a dataframe
+            Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets()
-            Scans the dataset or dataframes and stores in list format
-        frequentOneItem()
-            Generates one frequent patterns
-        eclatGeneration(candidateList)
-            It will generate the combinations of frequent items
-        generateFrequentPatterns(tidList)
-            It will generate the combinations of frequent items from a list of items
+            Scan the database and store the items with their timestamps which are periodic frequent
+        calculateLa()
+            Calculates the support and period for a list of timestamps.
+        Generation()
+            Used to implement prefix class equivalence method to generate the periodic patterns recursively
+
 
-    **Executing the code on terminal:**
-    ------------------------------------------
+
+    **Methods to execute code on terminal**
+    -----------------------------------------
     .. code-block:: console
 
 
        Format:
 
+       (.venv) $ python3 basic.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
 
-       (.venv) $ python3 kPFPMiner.py <inputFile> <outputFile> <k>
+       Example usage:
 
-       Examples :
+       (.venv) $ python3 basic.py sampleDB.txt patterns.txt 10.0 4.0 2.0
 
-       (.venv) $  python3 kPFPMiner.py sampleDB.txt patterns.txt 10
 
+               .. note:: constraints will be considered in percentage of database transactions
 
-    **Sample run of the importing code:
-    --------------------------------------
-    .. code-block:: python
+    **Importing this algorithm into a python program**
+    ---------------------------------------------------
+    ... code-block:: python
 
-            import PAMI.periodicFrequentPattern.kPFPMiner as alg
+                    from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
 
-            obj = alg.kPFPMiner(iFile, k)
+                    obj = alg.PFPECLAT("../basic/sampleTDB.txt", 5, 3, 3)
 
-            obj.startMine()
+                    obj.startMine()
 
-            periodicFrequentPatterns = obj.getPatterns()
+                    Patterns = obj.getPatterns()
 
-            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+                    print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
 
-            obj.save(oFile)
+                    obj.save("patterns")
 
-            Df = obj.getPatternInDataFrame()
+                    Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+                    memUSS = obj.getMemoryUSS()
 
-            print("Total Memory in USS:", memUSS)
+                    print("Total Memory in USS:", memUSS)
 
-            memRSS = obj.getMemoryRSS()
+                    memRSS = obj.getMemoryRSS()
 
-            print("Total Memory in RSS", memRSS)
+                    print("Total Memory in RSS", memRSS)
 
-            run = obj.getRuntime()
+                    run = obj.getRuntime()
 
-            print("Total ExecutionTime in seconds:", run)
+                    print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
     --------------
-            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
-
-    """
+             The complete program was written by  P.Likhitha under the supervision of Professor Rage Uday Kiran.
 
-    _startTime = float()
-    _endTime = float()
-    _k = int()
-    _finalPatterns = {}
+       """
     _iFile = " "
     _oFile = " "
+    _minSup = str()
+    _maxPer = str()
+    _maxLa = float()
     _sep = " "
+    _SPPList = {}
+    _itemList = []
+    _last = int()
+    _finalPatterns = {}
+    _tsList = {}
+    _startTime = float()
+    _endTime = float()
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _tidList = {}
-    lno = int()
-    _maximum = int()
 
-    def _creatingItemSets(self):
+    def __init__(self, inputFile, minSup, maxPer, maxLa, sep='\t'):
+        self._iFile = inputFile
+        self._minSup = minSup
+        self._maxPer = maxPer
+        self._maxLa = maxLa
+        self._sep = sep
+
+    def _creatingItemsets(self):
         """
         Storing the complete transactions of the database/input file in a database variable
         """
-
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-
-            # print(self.Database)
+            if 'Patterns' in i:
+                self._Database = self._iFile['Patterns'].tolist()
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
@@ -215,132 +260,14 @@
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
-                    
-    def getPer_Sup(self, tids):
-        tids.sort()
-        cur=0
-        per=list()
-        sup=0
-        #print(tids)
-        for i in range(len(tids)-1):
-            j = i + 1
-            #if tids[j] - cur <= periodicity:
-                #return [0,0]
-            per.append(tids[j] - cur)
-            cur = tids[j]
-        per.append(self.lno - cur)
-        return max(per)
-
-    def _frequentOneItem(self):
-        """
-        Generating one frequent patterns
-        """
-        self._mapSupport = {}
-        self._tidList = {}
-        n = 0
-        for line in self._Database:
-            self.lno += 1
-            n = int(line[0])
-            for i in range(1, len(line)):
-                si = line[i]
-                if self._mapSupport.get(si) is None:
-                    self._mapSupport[si] = [1, abs(0 - n), n]
-                    self._tidList[si] = [n]
-                else:
-                    self._mapSupport[si][0] += 1
-                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
-                    self._mapSupport[si][2] = n
-                    self._tidList[si].append(n)
-        for x, y in self._mapSupport.items():
-            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
-        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        for i in plist:
-            if len(self._finalPatterns) >= self._k:
-                break
-            else:
-                self._finalPatterns[i] = self._mapSupport[i][1]
-        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        plist = list(self._finalPatterns.keys())
-        return plist
-
-
-    def _save(self, prefix, suffix, tidSetI):
-        """Saves the patterns that satisfy the periodic frequent property.
-
-        :param prefix: the prefix of a pattern
-        :type prefix: list
-        :param suffix: the suffix of a patterns
-        :type suffix: list
-        :param tidSetI: the timestamp of a patterns
-        :type tidSetI: list
-        """
-
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = self.getPer_Sup(tidSetI)
-        sample = str()
-        for i in prefix:
-            sample = sample + i + " "
-        if len(self._finalPatterns) < self._k:
-            if val < self._maximum:
-                self._finalPatterns[sample] = val
-                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._maximum = max([i for i in self._finalPatterns.values()])
-        else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
-                if val < y:
-                    del self._finalPatterns[x]
-                    self._finalPatterns[sample] = val
-                    self._finalPatterns = {k: v for k, v in
-                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
-                                                     reverse=True)}
-                    self._maximum = max([i for i in self._finalPatterns.values()])
-                    return
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
-        :param prefix:  main equivalence prefix
-        :type prefix: periodic-frequent item or pattern
-        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
-        :type itemSets: list
-        :param tidSets: timestamps of the items in the argument itemSets
-        :type tidSets: list
-
-        """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y) <= self._maximum:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
 
         :param value: user specified minSup value
         :return: converted type
@@ -348,137 +275,206 @@
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = ((len(self._Database)) * value)
+                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
+    def _createSPPList(self):
+        """
+        to convert the single length stable periodic patterns
+        """
+        tidLast = {}
+        la = {}
+        self._SPPList = {}
+        self._tsList = {}
+        for transaction in self._Database:
+            ts = int(transaction[0])
+            for item in transaction[1:]:
+                if item not in self._SPPList:
+                    la[item] = max(0, ts - self._maxPer)
+                    self._SPPList[item] = [1, la[item]]
+                    self._tsList[item] = [ts]
+                else:
+                    s = self._SPPList[item][0] + 1
+                    la[item] = max(0, la[item] + ts - tidLast.get(item) - self._maxPer)
+                    self._SPPList[item] = [s, max(la[item], self._SPPList[item][1])]
+                    self._tsList[item].append(ts)
+                tidLast[item] = ts
+            self._last = ts
+        for item in self._SPPList:
+            la[item] = max(0, la[item] + self._last - tidLast[item] - self._maxPer)
+            self._SPPList[item][1] = max(la[item], self._SPPList[item][1])
+        self._SPPList = {k: v for k, v in self._SPPList.items() if v[0] >= self._minSup and v[1] <= self._maxLa}
+        self._SPPList = {k: v for k, v in sorted(self._SPPList.items(), key=lambda x: x[1][0], reverse=True)}
+        self._Generation(list(self._SPPList), set())
+
+    def _Generation(self, GPPFList, CP):
+        """
+        To generate the patterns using depth-first search
+        """
+        for i in range(len(GPPFList)):
+            item = GPPFList[i]
+            CP1 = CP | {item}
+            if CP != set():
+                self._tsList['\t'.join(CP1)] = list(set(self._tsList['\t'.join(CP)]) & set(self._tsList[item]))
+            la = self._calculateLa(self._tsList['\t'.join(CP1)])
+            support = len(self._tsList['\t'.join(CP1)])
+            if la <= self._maxLa and len(self._tsList['\t'.join(CP1)]) >= self._minSup:
+                #CP = CP1
+                self._finalPatterns['\t'.join(CP1)] = [support, la]
+                if i+1 < len(GPPFList):
+                    self._Generation(GPPFList[i+1:], CP1)
+
+    def _calculateLa(self, tsList):
+        """
+        To calculate the liability of a patterns based on its timestamps
+        """
+        previous = 0
+        la = 0
+        tsList = sorted(tsList)
+        laList = []
+        for ts in tsList:
+            la = max(0, la + ts - previous - self._maxPer)
+            laList.append(la)
+            previous = ts
+            
+        la = max(0, la + self._last - previous - self._maxPer)
+        laList.append(la)
+        maxla = max(laList)
+        return maxla
+
+    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
     def startMine(self):
         """
-        Main function of the program
+        Method to start the mining of patterns
+        """
+        self._startTime = _ab._time.time()
+        self._creatingItemsets()
+        self._minSup = self._convert(self._minSup)
+        self._maxPer = self._convert(self._maxPer)
+        self._maxLa = self._convert(self._maxLa)
+        self._finalPatterns = {}
+        #print(self._minSup, self._maxPer, self._maxLa)
+        self._createSPPList()
+        self._endTime = _ab._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
+        print("Stable Periodic Frequent patterns were generated successfully using basic algorithm ")
 
+    def Mine(self):
+        """
+        Method to start the mining of patterns
         """
         self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
-        self._creatingItemSets()
-        self._k = self._convert(self._k)
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i + 1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y1) <= self._maximum:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-        print("kPFPMiner has successfully generated top-k frequent patterns")
+        self._creatingItemsets()
+        self._minSup = self._convert(self._minSup)
+        self._maxPer = self._convert(self._maxPer)
+        self._maxLa = self._convert(self._maxLa)
+        self._finalPatterns = {}
+        #print(self._minSup, self._maxPer, self._maxLa)
+        self._createSPPList()
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
+        print("Stable Periodic Frequent patterns were generated successfully using basic algorithm ")
 
-    def getMemoryUSS(self):
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-        :return: returning USS memory consumed by the mining process
+    def getRuntime(self):
+        """
+        Calculating the total amount of runtime taken by the mining process
+
+        :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
+        return self._endTime - self._startTime
 
-        return self._memoryUSS
+    def getPatterns(self):
+        """
+        Function to return the set of stable periodic-frequent patterns after completion of the mining process
 
-    def getMemoryRSS(self):
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        :return: returning stable periodic-frequent patterns
+        :rtype: dict
+        """
+        return self._finalPatterns
 
-        :return: returning RSS memory consumed by the mining process
+    def getMemoryUSS(self):
+        """
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryRSS
-
-    def getRuntime(self):
-        """Calculating the total amount of runtime taken by the mining process
+        return self._memoryUSS
 
-        :return: returning total amount of runtime taken by the mining process
-        :rtype: float
+    def save(self, outFile):
         """
+        Complete set of periodic-frequent patterns will be loaded in to an output file
 
-        return self._endTime - self._startTime
+        :param outFile: name of the output file
+        :type outFile: csv file
+        """
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            s1 = x.strip() + ":" + str(y[0]) + ":" + str(y[1])
+            writer.write("%s \n" % s1)
 
     def getPatternsAsDataFrame(self):
-        """Storing final frequent patterns in a dataframe
+        """
+        Storing final periodic-frequent patterns in a dataframe
 
-        :return: returning frequent patterns in a dataframe
+        :return: returning periodic-frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
+            data.append([a.replace('\t', ' '), b[0], b[1]])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
         return dataFrame
 
-    def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
-
-        :param outFile: name of the output file
-
-        :type outFile: file
+    def getMemoryRSS(self):
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
-        for x, y in self._finalPatterns.items():
-            patternsAndSupport = x + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
-
-    def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
-
-        :return: returning frequent patterns
-        :rtype: dict
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        :return: returning RSS memory consumed by the mining process
+        :rtype: float
         """
-        return self._finalPatterns
+
+        return self._memoryRSS
 
     def printResults(self):
-        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
+        """
+        This function is used to print the results
+        """
+        print("Total number of Stable Periodic  Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = SPPEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+        if len(_ab._sys.argv) == 6:
+            _ap = SPPEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
-        _Patterns = _ap.getPatterns()
-        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
+        print("Total number of Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
```

### Comparing `pami-2024.4.11.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2024.4.9.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/SPAM.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/SPAM.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2024.4.9.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,95 @@
-# Stable periodic pattern mining aims to discover all interesting patterns in a temporal database using three constraints minimum support,
-# maximum period and maximum liability, that have support no less than the user-specified minimum support  constraint and liability no
-# greater than maximum liability.
+# UVEclat is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
+#     from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
 #
-#             obj = alg.SPPEclat("../basic/sampleTDB.txt", 5, 3, 3)
+#     obj = alg.UVEclat(iFile, minSup)
 #
-#             obj.startMine()
+#     obj.startMine()
 #
-#             Patterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#             print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.save("patterns")
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
-#             print("Total Memory in USS:", memUSS)
+#     print("Total Memory in USS:", memUSS)
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print("Total Memory in RSS", memRSS)
+#     print("Total Memory in RSS", memRSS)
 #
-#             run = obj.getRuntime()
+#     run = obj.getRuntime()
 #
-#             print("Total ExecutionTime in seconds:", run)
+#     print("Total ExecutionTime in seconds:", run)
 #
 
-
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
-
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
-
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
-
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
-
 """
-import pandas as pd
-from deprecated import deprecated
 
-from PAMI.stablePeriodicFrequentPattern.basic import abstract as _ab
+import operator as _operator
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
 
-class SPPEclat(_ab._stablePeriodicFrequentPatterns):
-    """
-    :Description:   Stable periodic pattern mining aims to dicover all interesting patterns in a temporal database using three contraints minimum support,
-                    maximum period and maximum lability, that have support no less than the user-specified minimum support  constraint and lability no
-                    greater than maximum lability.
-
-    :Reference:   Fournier-Viger, P., Yang, P., Lin, J. C.-W., Kiran, U. (2019). Discovering Stable Periodic-Frequent Patterns in Transactional Data. Proc.
-                  32nd Intern. Conf. on Industrial, Engineering and Other Applications of Applied Intelligent Systems (IEA AIE 2019), Springer LNAI, pp. 230-244
-
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of stable periodic Frequent Pattern.
-    :param  oFile: str :
-                   Name of the output file to store complete set of stable periodic Frequent Pattern.
-    :param  minSup: float or int or str :
-                    The user can specify minSup either in count or proportion of database size.
-                    If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-                    Otherwise, it will be treated as float.
-                    Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-    :param  itemSup: int or float :
-                    Frequency of an item
-    :param maxLa: float :
-                  minimum loss of a pattern
-    :param  sep: str :
-                 This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+
+_minSup = float()
+_finalPatterns = {}
 
 
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
     :Attributes:
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
+
 
+class UVEclat(_ab._frequentPatterns):
+    """
+    :Description: It is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
+    :Reference:
+    Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
+    SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
+    https://doi.org/10.1145/1982185.1982399
+    :Attributes:
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
-        minSup : int or float or str
+        minSup : float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        maxPer : int or float or str
-            The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        maxLa : int or float or str
-            The user can specify maxLa either in count or proportion of database size.
-            If the program detects the data type of maxLa is integer, then it treats maxLa is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxLa=10 will be treated as integer, while maxLa=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
@@ -117,363 +98,411 @@
         endTime:float
             To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
         tree : class
-            it represents the Tree class
+            To represents the Tree class
         itemSetCount : int
-            it represents the total no of patterns
+            To represents the total no of patterns
         finalPatterns : dict
-            it represents to store the patterns
-        tidList : dict
-            stores the timestamps of an item
-
+            To store the complete patterns
     :Methods:
-
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to an output file
-        getPatternsAsDataFrame()
-            Complete set of periodic-frequent patterns will be loaded in to a dataframe
+        storePatternsInFile(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsInDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent
-        calculateLa()
-            Calculates the support and period for a list of timestamps.
-        Generation()
-            Used to implement prefix class equivalence method to generate the periodic patterns recursively
-
-
-
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
     **Methods to execute code on terminal**
-    -----------------------------------------
-    .. code-block:: console
-
-
-       Format:
-
-       (.venv) $ python3 basic.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
-
-       Example usage:
-
-       (.venv) $ python3 basic.py sampleDB.txt patterns.txt 10.0 4.0 2.0
-
-
-               .. note:: constraints will be considered in percentage of database transactions
-
+    ------------------------------------------
+            Format:
+                      >>> python3 uveclat.py <inputFile> <outputFile> <minSup>
+            Example:
+                      >>>  python3 uveclat.py sampleTDB.txt patterns.txt 3
+                      .. note:: minSup  will be considered in support count or frequency
     **Importing this algorithm into a python program**
     ---------------------------------------------------
-    ... code-block:: python
-
-                    from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
-
-                    obj = alg.PFPECLAT("../basic/sampleTDB.txt", 5, 3, 3)
-
-                    obj.startMine()
-
-                    Patterns = obj.getPatterns()
-
-                    print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
-
-                    obj.save("patterns")
-
-                    Df = obj.getPatternsAsDataFrame()
-
-                    memUSS = obj.getMemoryUSS()
-
-                    print("Total Memory in USS:", memUSS)
-
-                    memRSS = obj.getMemoryRSS()
-
-                    print("Total Memory in RSS", memRSS)
-
-                    run = obj.getRuntime()
-
-                    print("Total ExecutionTime in seconds:", run)
-
+    .. code-block:: python
+            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+            obj = alg.UVEclat(iFile, minSup)
+            obj.startMine()
+            frequentPatterns = obj.getPatterns()
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
+            obj.save(oFile)
+            Df = obj.getPatternsAsDataFrame()
+            memUSS = obj.getmemoryUSS()
+            print("Total Memory in USS:", memUSS)
+            memRSS = obj.getMemoryRSS()
+            print("Total Memory in RSS", memRSS)
+            run = obj.getRuntime()
+            print("Total ExecutionTime in seconds:", run)
     **Credits:**
-    --------------
-             The complete program was written by  P.Likhitha under the supervision of Professor Rage Uday Kiran.
-
-       """
+    ---------------
+         The complete program was written by   P.Likhitha    under the supervision of Professor Rage Uday Kiran.
+    """
+    _startTime = float()
+    _endTime = float()
+    _minSup = str()
+    _finalPatterns = {}
     _iFile = " "
     _oFile = " "
-    _minSup = str()
-    _maxPer = str()
-    _maxLa = float()
     _sep = " "
-    _SPPList = {}
-    _itemList = []
-    _last = int()
-    _finalPatterns = {}
-    _tsList = {}
-    _startTime = float()
-    _endTime = float()
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
+    _tidList = {}
+    _rank = {}
 
-    def __init__(self, inputFile, minSup, maxPer, maxLa, sep='\t'):
-        self._iFile = inputFile
-        self._minSup = minSup
-        self._maxPer = maxPer
-        self._maxLa = maxLa
-        self._sep = sep
-
-    def _creatingItemsets(self):
+    def _creatingItemSets(self):
         """
-        Storing the complete transactions of the database/input file in a database variable
+        Scans the dataset
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-            if 'Patterns' in i:
-                self._Database = self._iFile['Patterns'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
 
-    def _convert(self, value):
+    def _frequentOneItem(self):
         """
-        to convert the type of user specified minSup value
+        takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
+        """
+
+        mapSupport = {}
+        k = 0
+        for i in self._Database:
+            k += 1
+            for j in i:
+                if j.item not in mapSupport:
+                    mapSupport[str(j.item)] = j.probability
+                    self._tidList[str(j.item)] = {k: j.probability}
+                else:
+                    mapSupport[str(j.item)] += j.probability
+                    self._tidList[str(j.item)].update({k: j.probability})
+        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
+        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
+        return list(plist.keys())
+
+    @staticmethod
+    def _check(i, x):
+        """
+        To check the presence of item or pattern in transaction
+        :param x: it represents the pattern
+        :type x : list
+        :param i : represents the uncertain self.Database
+        :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
+    @staticmethod
+    def _convert(value):
+        """
+        To convert the type of user specified minSup value
         :param value: user specified minSup value
-        :return: converted type
+        :return: converted type minSup value
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self._Database) * value)
+            value = float(value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _createSPPList(self):
+    def _removeFalsePositives(self):
         """
-        to convert the single length stable periodic patterns
+        To remove the false positive patterns generated in frequent patterns
+        :return: patterns with accurate probability
         """
-        tidLast = {}
-        la = {}
-        self._SPPList = {}
-        self._tsList = {}
-        for transaction in self._Database:
-            ts = int(transaction[0])
-            for item in transaction[1:]:
-                if item not in self._SPPList:
-                    la[item] = max(0, ts - self._maxPer)
-                    self._SPPList[item] = [1, la[item]]
-                    self._tsList[item] = [ts]
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
                 else:
-                    s = self._SPPList[item][0] + 1
-                    la[item] = max(0, la[item] + ts - tidLast.get(item) - self._maxPer)
-                    self._SPPList[item] = [s, max(la[item], self._SPPList[item][1])]
-                    self._tsList[item].append(ts)
-                tidLast[item] = ts
-            self._last = ts
-        for item in self._SPPList:
-            la[item] = max(0, la[item] + self._last - tidLast[item] - self._maxPer)
-            self._SPPList[item][1] = max(la[item], self._SPPList[item][1])
-        self._SPPList = {k: v for k, v in self._SPPList.items() if v[0] >= self._minSup and v[1] <= self._maxLa}
-        self._SPPList = {k: v for k, v in sorted(self._SPPList.items(), key=lambda x: x[1][0], reverse=True)}
-        self._Generation(list(self._SPPList), set())
-
-    def _Generation(self, GPPFList, CP):
-        """
-        To generate the patterns using depth-first search
-        """
-        for i in range(len(GPPFList)):
-            item = GPPFList[i]
-            CP1 = CP | {item}
-            if CP != set():
-                self._tsList['\t'.join(CP1)] = list(set(self._tsList['\t'.join(CP)]) & set(self._tsList[item]))
-            la = self._calculateLa(self._tsList['\t'.join(CP1)])
-            support = len(self._tsList['\t'.join(CP1)])
-            if la <= self._maxLa and len(self._tsList['\t'.join(CP1)]) >= self._minSup:
-                #CP = CP1
-                self._finalPatterns['\t'.join(CP1)] = [support, la]
-                if i+1 < len(GPPFList):
-                    self._Generation(GPPFList[i+1:], CP1)
-
-    def _calculateLa(self, tsList):
-        """
-        To calculate the liability of a patterns based on its timestamps
-        """
-        previous = 0
-        la = 0
-        tsList = sorted(tsList)
-        laList = []
-        for ts in tsList:
-            la = max(0, la + ts - previous - self._maxPer)
-            laList.append(la)
-            previous = ts
-            
-        la = max(0, la + self._last - previous - self._maxPer)
-        laList.append(la)
-        maxla = max(laList)
-        return maxla
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            if y >= self._minSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
+
+    @staticmethod
+    def _Intersection(tidSetx, tidSetY):
+        """
+        This function is used to find the intersection
+        :param tidSetx: the timestamp of a patterns
+        :type tidSetx: dict
+        :param tidSetY: the timestamp of a patterns
+        :type tidSetY: dict
+        """
+        tids = []
+        support = []
+        tidDict = {}
+        for x, y in tidSetx.items():
+            for x1, y1 in tidSetY.items():
+                if x == x1:
+                    tids.append(x)
+                    support.append(y * y1)
+                    tidDict.update({x: y * y1})
+        return tidDict
+
+    def _calculateExpSup(self, tidList):
+        """
+        This function is used to calculate support of tidList
+        :param tidList: timestamp of a list.
+        :type tidList: List
+        """
+        return sum(tidList.values())
+
+    def _save(self, prefix, suffix, tidSetI):
+        """
+        Saves the patterns that satisfy the periodic frequent property.
+        :param prefix: the prefix of a pattern
+        :type prefix: list
+        :param suffix: the suffix of a patterns
+        :type suffix: list
+        :param tidSetI: the timestamp of a patterns
+        :type tidSetI: dict
+        """
+
+        global _finalPatterns
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = self._calculateExpSup(tidSetI)
+        _finalPatterns[tuple(prefix)] = val
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """
+        Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+        :param prefix:  main equivalence prefix
+        :type prefix: periodic-frequent item or pattern
+        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
+        :type itemSets: list
+        :param tidSets: timestamps of the items in the argument itemSets
+        :type tidSets: list
+        """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y) >= self._minSup:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
-    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
     def startMine(self):
         """
-        Method to start the mining of patterns
+        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
         """
+        global _minSup
         self._startTime = _ab._time.time()
-        self._creatingItemsets()
+        self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
-        self._maxPer = self._convert(self._maxPer)
-        self._maxLa = self._convert(self._maxLa)
-        self._finalPatterns = {}
-        #print(self._minSup, self._maxPer, self._maxLa)
-        self._createSPPList()
+        _minSup = self._minSup
+        plist = self._frequentOneItem()
+        for i in range(len(plist)):
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
+            for j in range(i+1, len(plist)):
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y1) >= self._minSup:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+            self._save(None, itemSetX, tidSetI)
+        self._removeFalsePositives()
+        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
         self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
-        print("Stable Periodic Frequent patterns were generated successfully using basic algorithm ")
-
-    def Mine(self):
-        """
-        Method to start the mining of patterns
-        """
-        self._startTime = _ab._time.time()
-        self._creatingItemsets()
-        self._minSup = self._convert(self._minSup)
-        self._maxPer = self._convert(self._maxPer)
-        self._maxLa = self._convert(self._maxLa)
-        self._finalPatterns = {}
-        #print(self._minSup, self._maxPer, self._maxLa)
-        self._createSPPList()
-        self._endTime = _ab._time.time()
-        self._memoryUSS = float()
         self._memoryRSS = float()
-        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Stable Periodic Frequent patterns were generated successfully using basic algorithm ")
-
-
-    def getRuntime(self):
-        """
-        Calculating the total amount of runtime taken by the mining process
-
-        :return: returning total amount of runtime taken by the mining process
-        :rtype: float
-        """
-        return self._endTime - self._startTime
-
-    def getPatterns(self):
-        """
-        Function to return the set of stable periodic-frequent patterns after completion of the mining process
-
-        :return: returning stable periodic-frequent patterns
-        :rtype: dict
-        """
-        return self._finalPatterns
 
     def getMemoryUSS(self):
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def save(self, outFile):
+    def getMemoryRSS(self):
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        :return: returning RSS memory consumed by the mining process
+        :rtype: float
         """
-        Complete set of periodic-frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
-        :type outFile: csv file
-        """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
-        for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y[0]) + ":" + str(y[1])
-            writer.write("%s \n" % s1)
+        return self._memoryRSS
 
-    def getPatternsAsDataFrame(self):
+    def getRuntime(self):
+        """Calculating the total amount of runtime taken by the mining process
+        :return: returning total amount of runtime taken by the mining process
+        :rtype: float
         """
-        Storing final periodic-frequent patterns in a dataframe
 
-        :return: returning periodic-frequent patterns in a dataframe
+        return self._endTime - self._startTime
+
+    def getPatternsAsDataFrame(self):
+        """Storing final frequent patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b[0], b[1]])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
-        return dataFrame
-
-    def getMemoryRSS(self):
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
-        :return: returning RSS memory consumed by the mining process
-        :rtype: float
+            data.append([a.replace('\t', ' '), b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        return dataframe
+
+    def save(self, oFile):
+        """Complete set of frequent patterns will be loaded in to an output file
+        :param oFile: name of the output file
+        :type oFile: csv file
         """
+        self.oFile = oFile
+        writer = open(self.oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            s1 = x.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
-        return self._memoryRSS
+    def getPatterns(self):
+        """ Function to send the set of frequent patterns after completion of the mining process
+        :return: returning frequent patterns
+        :rtype: dict
+        """
+        return self._finalPatterns
 
     def printResults(self):
         """
         This function is used to print the results
         """
-        print("Total number of Stable Periodic  Patterns:", len(self.getPatterns()))
+        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
-        if len(_ab._sys.argv) == 7:
-            _ap = SPPEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
-        if len(_ab._sys.argv) == 6:
-            _ap = SPPEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         print("Total number of Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2024.4.9.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/abstract.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/dfsCode.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/dfsCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/edge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/extendedEdge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/frequentSubgraph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/graph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/gspan.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/gspan.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/basic/vertex.py` & `pami-2024.4.9.1/PAMI/subgraphMining/basic/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/DFSCode.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSCode.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/DFSThread.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/DFSThread.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/abstract.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/edge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/edge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/extendedEdge.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/extendedEdge.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/frequentSubgraph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/frequentSubgraph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/graph.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/graph.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/sparseTriangularMatrix.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/tkg.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/tkg.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/subgraphMining/topK/vertex.py` & `pami-2024.4.9.1/PAMI/subgraphMining/topK/vertex.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,509 +1,723 @@
-# UVEclat is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
+# WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
+# It stores the database in compressed fp-tree decreasing the memory usage and extracts the
+# patterns from tree.It employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
-# --------------------------------------------------------
+# ----------------------------------------------------------
 #
 #
-#     from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+#             from PAMI.weightFrequentPattern.basic import basic as alg
 #
-#     obj = alg.UVEclat(iFile, minSup)
+#             obj = alg.basic(iFile, wFile, minSup, minWeight)
 #
-#     obj.startMine()
+#             obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#             frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#             print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#             obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternsAsDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#             memUSS = obj.getMemoryUSS()
 #
-#     print("Total Memory in USS:", memUSS)
+#             print("Total Memory in USS:", memUSS)
 #
-#     memRSS = obj.getMemoryRSS()
+#             memRSS = obj.getMemoryRSS()
 #
-#     print("Total Memory in RSS", memRSS)
+#             print("Total Memory in RSS", memRSS)
 #
-#     run = obj.getRuntime()
+#             run = obj.getRuntime()
 #
-#     print("Total ExecutionTime in seconds:", run)
+#             print("Total ExecutionTime in seconds:", run)
 #
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
+
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
+
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
+
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
+
 """
 
-import operator as _operator
-from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+from PAMI.weightedFrequentPattern.basic import abstract as _fp
+from typing import List, Dict, Tuple, Set, Union, Any, Generator
+import pandas as pd
+from deprecated import deprecated
 
 
-_minSup = float()
-_finalPatterns = {}
+_minSup = str()
+_minWeight = int()
+_miniWeight = int()
+_maxWeight = int()
+_weights = {}
+_fp._sys.setrecursionlimit(20000)
 
 
-class _Item:
+class _Node:
     """
-    A class used to represent the item with probability in transaction of dataset
+    A class used to represent the node of frequentPatternTree
+
     :Attributes:
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
+
+        itemId: int
+            storing item of a node
+        counter: int
+            To maintain the support of node
+        parent: node
+            To maintain the parent of node
+        children: list
+            To maintain the children of node
+
+    :Methods:
+
+        addChild(node)
+            Updates the nodes children list and parent for the given node
     """
 
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
+    def __init__(self, item: str, children: list) -> None:
+        self.itemId = item
+        self.counter = 1
+        self.parent = None
+        self.children = children
+
+    def addChild(self, node: '_Node') -> None:
+        """
+        Retrieving the child from the tree
 
+        :param node: Children node
+        :type node: Node
+        :return: Updates the children nodes and parent nodes
+        """
+        self.children[node.itemId] = node
+        node.parent = self
 
-class UVEclat(_ab._frequentPatterns):
+
+class _Tree:
     """
-    :Description: It is one of the fundamental algorithm to discover frequent patterns in an uncertain transactional database using PUF-Tree.
-    :Reference:
-    Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
-    SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
-    https://doi.org/10.1145/1982185.1982399
+    A class used to represent the frequentPatternGrowth tree structure
+
     :Attributes:
+
+        root : Node
+            The first node of the tree set to Null.
+        summaries : dictionary
+            Stores the nodes itemId which shares same itemId
+        info : dictionary
+            frequency of items in the transactions
+
+    :Methods:
+
+        addTransaction(transaction, freq)
+            adding items of  transactions into the tree as nodes and freq is the count of nodes
+        getFinalConditionalPatterns(node)
+            getting the conditional patterns from fp-tree for a node
+        getConditionalPatterns(patterns, frequencies)
+            sort the patterns by removing the items with lower minSup
+        generatePatterns(prefix)
+            generating the patterns from fp-tree
+    """
+
+    def __init__(self) -> None:
+        self.root = _Node(None, {})
+        self.summaries = {}
+        self.info = {}
+
+    def addTransaction(self, transaction: List[str], count: int) -> None:
+        """
+        Adding transaction into tree
+
+        :param transaction: it represents the one transaction in database
+        :type transaction: list
+        :param count: frequency of item
+        :type count: int
+        :return: None
+        """
+        # This method takes transaction as input and returns the tree
+        currentNode = self.root
+        for i in range(len(transaction)):
+            if transaction[i] not in currentNode.children:
+                newNode = _Node(transaction[i], {})
+                newNode.freq = count
+                currentNode.addChild(newNode)
+                if transaction[i] in self.summaries:
+                    self.summaries[transaction[i]].append(newNode)
+                else:
+                    self.summaries[transaction[i]] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i]]
+                currentNode.freq += count
+
+    def getFinalConditionalPatterns(self, alpha: str) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+        """
+        Generates the conditional patterns for a node
+
+        :param alpha: node to generate conditional patterns
+        :return: returns conditional patterns, frequency of each item in conditional patterns
+        """
+        finalPatterns = []
+        finalFreq = []
+        for i in self.summaries[alpha]:
+            set1 = i.freq
+            set2 = []
+            while i.parent.itemId is not None:
+                set2.append(i.parent.itemId)
+                i = i.parent
+            if len(set2) > 0:
+                set2.reverse()
+                finalPatterns.append(set2)
+                finalFreq.append(set1)
+        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
+        return finalPatterns, finalFreq, info
+
+    @staticmethod
+    def getConditionalTransactions(ConditionalPatterns: List[List[str]], conditionalFreq: List[int]) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+        """
+        To calculate the frequency of items in conditional patterns and sorting the patterns
+
+        :param ConditionalPatterns: paths of a node
+        :param conditionalFreq: frequency of each item in the path
+        :return: conditional patterns and frequency of each item in transactions
+        """
+        global _minSup, _miniWeight
+        pat = []
+        freq = []
+        data1 = {}
+        for i in range(len(ConditionalPatterns)):
+            for j in ConditionalPatterns[i]:
+                if j in data1:
+                    data1[j] += conditionalFreq[i]
+                else:
+                    data1[j] = conditionalFreq[i]
+        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+        count = 0
+        for p in ConditionalPatterns:
+            p1 = [v for v in p if v in up_dict]
+            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+            if len(trans) > 0:
+                pat.append(trans)
+                freq.append(conditionalFreq[count])
+            count += 1
+        return pat, freq, up_dict
+
+    def generatePatterns(self, prefix: List[str]) -> Generator[Tuple[List[str], int], None, None]:
+        """
+        To generate the frequent patterns
+
+        :param prefix: an empty list
+        :return: Frequent patterns that are extracted from fp-tree
+        """
+        global _miniWeight, _maxWeight, _minWeight, _minSup
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+            pattern = prefix[:]
+            pattern.append(i)
+            yield pattern, self.info[i]
+            patterns, freq, info = self.getFinalConditionalPatterns(i)
+            conditionalTree = _Tree()
+            conditionalTree.info = info.copy()
+            for pat in range(len(patterns)):
+                conditionalTree.addTransaction(patterns[pat], freq[pat])
+            if len(patterns) > 0:
+                for q in conditionalTree.generatePatterns(pattern):
+                    yield q
+
+
+class WFIM(_fp._weightedFrequentPatterns):
+    """
+    :Description:
+       * WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
+       * It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+
+    :Reference :
+           U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
+           in Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
+           https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of weighted Frequent Patterns.
+    :param  oFile: str :
+                   Name of the output file to store complete set of weighted Frequent Patterns.
+    :param  minSup: str or int or float:
+                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+
+
+    :Attributes :
+
         iFile : file
-            Name of the Input file or path of the input file
-        oFile : file
-            Name of the output file or path of the output file
-        minSup : float or int or str
+            Input file name or path of the input file
+        minSup: float or int or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        minWeight: float or int or str
+            The user can specify minWeight either in count or proportion of database size.
+            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
+        oFile : file
+            Name of the output file or the path of the output file
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            To represent the total no of transaction
+            it represents the total no of transactions
         tree : class
-            To represents the Tree class
-        itemSetCount : int
-            To represents the total no of patterns
+            it represents the Tree class
         finalPatterns : dict
-            To store the complete patterns
-    :Methods:
+            it represents to store the patterns
+
+    :Methods :
+
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        storePatternsInFile(oFile)
+        save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
-        getPatternsInDataFrame()
+        getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
+        creatingItemSets()
+            Scans the dataset or dataframes and stores in list format
         frequentOneItem()
-            Extracts the one-length frequent patterns from database
+            Extracts the one-frequent patterns from transactions
+
     **Methods to execute code on terminal**
-    ------------------------------------------
-            Format:
-                      >>> python3 uveclat.py <inputFile> <outputFile> <minSup>
-            Example:
-                      >>>  python3 uveclat.py sampleTDB.txt patterns.txt 3
-                      .. note:: minSup  will be considered in support count or frequency
+    -------------------------------------------
+    .. code-block:: console
+
+
+       Format:
+
+       (.venv) $ python3 basic.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
+
+       Example Usage:
+
+       (.venv) $ python3 basic.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
+
+
+               .. note:: minSup and maxPer will be considered in support count or frequency
+
+
     **Importing this algorithm into a python program**
-    ---------------------------------------------------
+    -----------------------------------------------------
     .. code-block:: python
-            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
-            obj = alg.UVEclat(iFile, minSup)
+
+            from PAMI.weightFrequentPattern.basic import basic as alg
+
+            obj = alg.basic(iFile, wFile, minSup, minWeight)
+
             obj.startMine()
+
             frequentPatterns = obj.getPatterns()
+
             print("Total number of Frequent Patterns:", len(frequentPatterns))
-            obj.save(oFile)
+
+            obj.savePatterns(oFile)
+
             Df = obj.getPatternsAsDataFrame()
+
             memUSS = obj.getmemoryUSS()
+
             print("Total Memory in USS:", memUSS)
+
             memRSS = obj.getMemoryRSS()
+
             print("Total Memory in RSS", memRSS)
+
             run = obj.getRuntime()
+
             print("Total ExecutionTime in seconds:", run)
+
     **Credits:**
-    ---------------
-         The complete program was written by   P.Likhitha    under the supervision of Professor Rage Uday Kiran.
-    """
-    _startTime = float()
-    _endTime = float()
+    ----------------------
+             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+
+        """
+
+    __startTime = float()
+    __endTime = float()
     _minSup = str()
-    _finalPatterns = {}
+    __finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _Database = []
-    _tidList = {}
-    _rank = {}
-
-    def _creatingItemSets(self):
-        """
-        Scans the dataset
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __mapSupport = {}
+    __lno = 0
+    __tree = _Tree()
+    __rank = {}
+    __rankDup = {}
+
+    def __init__(self, iFile: str, wFile: str, minSup: str, minWeight: int, sep: str='\t') -> None:
+        super().__init__(iFile, wFile, minSup, minWeight, sep)
+
+    def __creatingItemSets(self) -> None:
+        """
+        Storing the complete transactions of the database/input file in a database variable
+        :return: None
+        """
+        self.__Database = []
+        if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
+                self.__Database = self._iFile['Transactions'].tolist()
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
+            if _fp._validators.url(self._iFile):
+                data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    tr = []
-                    for i in temp:
-                        i1 = i.index('(')
-                        i2 = i.index(')')
-                        item = i[0:i1]
-                        probability = float(i[i1 + 1:i2])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(temp)
+                    self.__Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            tr = []
-                            for i in temp:
-                                i1 = i.index('(')
-                                i2 = i.index(')')
-                                item = i[0:i1]
-                                probability = float(i[i1 + 1:i2])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
+                            # print(len(temp))
+                            self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
+    def _scanningWeights(self) -> None:
         """
-        takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
+        Storing the weights of the variables in input file in a weights variable
+        :return: None
         """
+        global _weights
+        _weights = {}
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            items, weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                items = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for i in range(len(weights)):
+                _weights[items[i]] = weights[i]
 
-        mapSupport = {}
-        k = 0
-        for i in self._Database:
-            k += 1
-            for j in i:
-                if j.item not in mapSupport:
-                    mapSupport[str(j.item)] = j.probability
-                    self._tidList[str(j.item)] = {k: j.probability}
-                else:
-                    mapSupport[str(j.item)] += j.probability
-                    self._tidList[str(j.item)].update({k: j.probability})
-        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
-        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
-        return list(plist.keys())
+            # print(self.Database)
+        if isinstance(self._wFile, str):
+            if _fp._validators.url(self._wFile):
+                data = _fp._urlopen(self._wFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    _weights[temp[0]] = temp[1]
+            else:
+                try:
+                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            s = int(float(temp[1]))
+                            _weights[temp[0]] = s
+                except IOError:
+                    print("File Not Found")
+                    quit()
 
-    @staticmethod
-    def _check(i, x):
+    def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
         """
-        To check the presence of item or pattern in transaction
-        :param x: it represents the pattern
-        :type x : list
-        :param i : represents the uncertain self.Database
-        :type i : list
-        """
-
-        # This method taken a transaction as input and returns the tree
-        for m in x:
-            k = 0
-            for n in i:
-                if m == n.item:
-                    k += 1
-            if k == 0:
-                return 0
-        return 1
+        To convert the type of user specified minSup value.
 
-    @staticmethod
-    def _convert(value):
-        """
-        To convert the type of user specified minSup value
         :param value: user specified minSup value
-        :return: converted type minSup value
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = float(value)
+            value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
+                value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _removeFalsePositives(self):
+    def __frequentOneItem(self) -> List[str]:
         """
-        To remove the false positive patterns generated in frequent patterns
-        :return: patterns with accurate probability
+        Generating One frequent items sets
+        :return: list
         """
-        global _finalPatterns
-        periods = {}
-        for i in self._Database:
-            for x, y in _finalPatterns.items():
-                if len(x) == 1:
-                    periods[x] = y
+        global _maxWeight
+        self.__mapSupport = {}
+        for tr in self.__Database:
+            for i in range(0, len(tr)):
+                if tr[i] not in self.__mapSupport:
+                    self.__mapSupport[tr[i]] = 1
                 else:
-                    s = 1
-                    check = self._check(i, x)
-                    if check == 1:
-                        for j in i:
-                            if j.item in x:
-                                s *= j.probability
-                        if x in periods:
-                            periods[x] += s
-                        else:
-                            periods[x] = s
-        for x, y in periods.items():
-            if y >= self._minSup:
-                sample = str()
-                for i in x:
-                    sample = sample + i + "\t"
-                self._finalPatterns[sample] = y
+                    self.__mapSupport[tr[i]] += 1
+        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
+        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        return genList
+
+    def __updateTransactions(self, itemSet: List[str]) -> List[List[int]]:
+        """
+        Updates the items in transactions with rank of items according to their support
+        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
+                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+
+        :param itemSet: list of one-frequent items
+        :return: list
+        """
+        list1 = []
+        for tr in self.__Database:
+            list2 = []
+            for i in range(len(tr)):
+                if tr[i] in itemSet:
+                    list2.append(self.__rank[tr[i]])
+            if len(list2) >= 1:
+                list2.sort()
+                list1.append(list2)
+        return list1
 
     @staticmethod
-    def _Intersection(tidSetx, tidSetY):
+    def __buildTree(transactions: List[List[int]], info: Dict[int, int]) -> '_Tree':
         """
-        This function is used to find the intersection
-        :param tidSetx: the timestamp of a patterns
-        :type tidSetx: dict
-        :param tidSetY: the timestamp of a patterns
-        :type tidSetY: dict
-        """
-        tids = []
-        support = []
-        tidDict = {}
-        for x, y in tidSetx.items():
-            for x1, y1 in tidSetY.items():
-                if x == x1:
-                    tids.append(x)
-                    support.append(y * y1)
-                    tidDict.update({x: y * y1})
-        return tidDict
-
-    def _calculateExpSup(self, tidList):
-        """
-        This function is used to calculate support of tidList
-        :param tidList: timestamp of a list.
-        :type tidList: List
-        """
-        return sum(tidList.values())
-
-    def _save(self, prefix, suffix, tidSetI):
-        """
-        Saves the patterns that satisfy the periodic frequent property.
-        :param prefix: the prefix of a pattern
-        :type prefix: list
-        :param suffix: the suffix of a patterns
-        :type suffix: list
-        :param tidSetI: the timestamp of a patterns
-        :type tidSetI: dict
-        """
-
-        global _finalPatterns
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = self._calculateExpSup(tidSetI)
-        _finalPatterns[tuple(prefix)] = val
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """
-        Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-        :param prefix:  main equivalence prefix
-        :type prefix: periodic-frequent item or pattern
-        :param itemSets: patterns which are items combined with prefix and satisfying the periodicity and frequent with their timestamps
-        :type itemSets: list
-        :param tidSets: timestamps of the items in the argument itemSets
-        :type tidSets: list
-        """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y) >= self._minSup:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
-
-    def startMine(self):
-        """
-        Main method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns
-        """
-        global _minSup
-        self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
+        Builds the tree with updated transactions
+
+        :param transactions: updated transactions
+        :param info: support details of each item in transactions.
+        :return: Transactions compressed in fp-tree
+        """
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(transactions)):
+            rootNode.addTransaction(transactions[i], 1)
+        return rootNode
+
+    def __savePeriodic(self, itemSet: List[int]) -> str:
+        """
+        The duplication items and their ranks
+
+        :param itemSet: frequent itemSet that generated
+        :return: patterns with original item names.
+        """
+        temp = str()
+        for i in itemSet:
+            temp = temp + self.__rankDup[i] + "\t"
+        return temp
+
+    @deprecated("It is recommended to use mine() instead of startMine() for mining process")
+    def startMine(self) -> None:
+        """
+        main program to start the operation
+        :return: None
+        """
+        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
+        self.__startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self.__creatingItemSets()
+        self._scanningWeights()
+        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
+        _maxWeight = max([s for s in _weights.values()])
+        _miniWeight = min([s for s in _weights.values()])
+        self._minSup = self.__convert(self._minSup)
+        _minSup = self._minSup
+        itemSet = self.__frequentOneItem()
+        updatedTransactions = self.__updateTransactions(itemSet)
+        for x, y in self.__rank.items():
+            self.__rankDup[y] = x
+        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
+        __Tree = self.__buildTree(updatedTransactions, info)
+        patterns = __Tree.generatePatterns([])
+        self.__finalPatterns = {}
+        for k in patterns:
+            s = self.__savePeriodic(k[0])
+            self.__finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent patterns were generated successfully using basic algorithm")
+        self.__endTime = _fp._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
+
+    def Mine(self) -> None:
+        """
+        main program to start the operation
+        :return: None
+        """
+        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
+        self.__startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self.__creatingItemSets()
+        self._scanningWeights()
+        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
+        _maxWeight = max([s for s in _weights.values()])
+        _miniWeight = min([s for s in _weights.values()])
+        self._minSup = self.__convert(self._minSup)
         _minSup = self._minSup
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i+1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y1) >= self._minSup:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-            self._save(None, itemSetX, tidSetI)
-        self._removeFalsePositives()
-        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
-        self._memoryUSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        itemSet = self.__frequentOneItem()
+        updatedTransactions = self.__updateTransactions(itemSet)
+        for x, y in self.__rank.items():
+            self.__rankDup[y] = x
+        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
+        __Tree = self.__buildTree(updatedTransactions, info)
+        patterns = __Tree.generatePatterns([])
+        self.__finalPatterns = {}
+        for k in patterns:
+            s = self.__savePeriodic(k[0])
+            self.__finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent patterns were generated successfully using basic algorithm")
+        self.__endTime = _fp._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
+
+
+    def getMemoryUSS(self) -> float:
+        """
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-    def getMemoryUSS(self):
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryUSS
+        return self.__memoryUSS
+
+    def getMemoryRSS(self) -> float:
+        """
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function.
 
-    def getMemoryRSS(self):
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.__memoryRSS
+
+    def getRuntime(self) -> float:
+        """
+        Calculating the total amount of runtime taken by the mining process.
 
-    def getRuntime(self):
-        """Calculating the total amount of runtime taken by the mining process
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self._endTime - self._startTime
+        return self.__endTime - self.__startTime
+
+    def getPatternsAsDataFrame(self) -> pd.DataFrame:
+        """
+        Storing final frequent patterns in a dataframe.
 
-    def getPatternsAsDataFrame(self):
-        """Storing final frequent patterns in a dataframe
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
+        for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def save(self, oFile):
-        """Complete set of frequent patterns will be loaded in to an output file
-        :param oFile: name of the output file
-        :type oFile: csv file
-        """
-        self.oFile = oFile
-        writer = open(self.oFile, 'w+')
-        for x, y in self._finalPatterns.items():
+    def save(self, outFile: str) -> None:
+        """
+        Complete set of frequent patterns will be loaded in to an output file.
+
+        :param outFile: name of the output file
+        :type outFile: csv file
+        :return: None
+        """
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        for x, y in self.__finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
+    def getPatterns(self) -> Dict[str, int]:
+        """
+        Function to send the set of frequent patterns after completion of the mining process.
+
         :return: returning frequent patterns
         :rtype: dict
         """
-        return self._finalPatterns
+        return self.__finalPatterns
 
-    def printResults(self):
+    def printResults(self) -> None:
         """
         This function is used to print the results
+        :return: None
         """
-        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
+        
+
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
+        if len(_fp._sys.argv) == 7:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 6:
+            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        print("Total number of Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_fp._sys.argv[2])
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.11.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
-# It stores the database in compressed fp-tree decreasing the memory usage and extracts the
-# patterns from tree.It employs downward closure property to  reduce the search space effectively.
+# WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
+# It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------------
+# --------------------------------------------------------
 #
 #
-#             from PAMI.weightFrequentPattern.basic import basic as alg
+#             from PAMI.weightedFrequentRegularPattern.basic import WFRIMiner as alg
 #
-#             obj = alg.basic(iFile, wFile, minSup, minWeight)
+#             obj = alg.WFRIMiner(iFile, WS, regularity)
 #
 #             obj.startMine()
 #
-#             frequentPatterns = obj.getPatterns()
+#             weightedFrequentRegularPatterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(frequentPatterns))
+#             print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 #
-#             obj.savePatterns(oFile)
+#             obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#             Df = obj.getPatternInDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
 #             print("Total Memory in RSS", memRSS)
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -48,82 +48,89 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.weightedFrequentPattern.basic import abstract as _fp
-from typing import List, Dict, Tuple, Set, Union, Any, Generator
+from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
 import pandas as pd
 from deprecated import deprecated
+from typing import List, Dict
 
 
-_minSup = str()
-_minWeight = int()
-_miniWeight = int()
-_maxWeight = int()
+_WS = str()
+_regularity = str()
+_lno = int()
 _weights = {}
+_wf = {}
 _fp._sys.setrecursionlimit(20000)
 
 
 class _Node:
     """
     A class used to represent the node of frequentPatternTree
 
     :Attributes:
-
         itemId: int
             storing item of a node
         counter: int
             To maintain the support of node
         parent: node
             To maintain the parent of node
         children: list
             To maintain the children of node
 
     :Methods:
-
         addChild(node)
             Updates the nodes children list and parent for the given node
+
     """
 
-    def __init__(self, item: str, children: list) -> None:
-        self.itemId = item
-        self.counter = 1
-        self.parent = None
+    def __init__(self, item: int, children: dict) -> None:
+        """
+        Initializing the Node class
+
+        :param item: Storing the item of a node
+        :type item: int or None
+        :param children: To maintain the children of a node
+        :type children: dict
+        :return: None
+        """
+
+        self.item = item
         self.children = children
+        self.parent = None
+        self.timeStamps = []
 
-    def addChild(self, node: '_Node') -> None:
+    def addChild(self, node) -> None:
         """
-        Retrieving the child from the tree
+        To add the children to a node
 
-        :param node: Children node
-        :type node: Node
-        :return: Updates the children nodes and parent nodes
+        :param node: parent node in the tree
+        :return: None
         """
-        self.children[node.itemId] = node
+
+        self.children[node.item] = node
         node.parent = self
 
 
 class _Tree:
     """
     A class used to represent the frequentPatternGrowth tree structure
 
     :Attributes:
-
         root : Node
             The first node of the tree set to Null.
         summaries : dictionary
             Stores the nodes itemId which shares same itemId
         info : dictionary
             frequency of items in the transactions
 
     :Methods:
-
         addTransaction(transaction, freq)
             adding items of  transactions into the tree as nodes and freq is the count of nodes
         getFinalConditionalPatterns(node)
             getting the conditional patterns from fp-tree for a node
         getConditionalPatterns(patterns, frequencies)
             sort the patterns by removing the items with lower minSup
         generatePatterns(prefix)
@@ -131,149 +138,223 @@
     """
 
     def __init__(self) -> None:
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction: List[str], count: int) -> None:
+    def addTransaction(self, transaction: list, tid: list) -> None:
         """
-        Adding transaction into tree
+        Adding a transaction into tree
 
-        :param transaction: it represents the one transaction in database
+        :param transaction: To represent the complete database
         :type transaction: list
-        :param count: frequency of item
-        :type count: int
-        :return: None
+        :param tid: To represent the timestamp of a database
+        :type tid: list
+        :return: pfp-growth tree
         """
-        # This method takes transaction as input and returns the tree
         currentNode = self.root
         for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
-                newNode.freq = count
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-                currentNode.freq += count
+        currentNode.timeStamps = currentNode.timeStamps + tid
 
-    def getFinalConditionalPatterns(self, alpha: str) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+    def getConditionalPatterns(self, alpha, pattern) -> tuple:
         """
-        Generates the conditional patterns for a node
+        Generates all the conditional patterns of a respective node
 
-        :param alpha: node to generate conditional patterns
-        :return: returns conditional patterns, frequency of each item in conditional patterns
+        :param alpha: To represent a Node in the tree
+        :type alpha: Node
+        :param pattern: prefix of the pattern
+        :type alpha: list
+        :return: A tuple consisting of finalPatterns, conditional pattern base and information
         """
         finalPatterns = []
-        finalFreq = []
+        finalSets = []
         for i in self.summaries[alpha]:
-            set1 = i.freq
+            set1 = i.timeStamps
             set2 = []
-            while i.parent.itemId is not None:
-                set2.append(i.parent.itemId)
+            while i.parent.item is not None:
+                set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalFreq.append(set1)
-        finalPatterns, finalFreq, info = self.getConditionalTransactions(finalPatterns, finalFreq)
-        return finalPatterns, finalFreq, info
+                finalSets.append(set1)
+        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
+        return finalPatterns, finalSets, info
 
     @staticmethod
-    def getConditionalTransactions(ConditionalPatterns: List[List[str]], conditionalFreq: List[int]) -> Tuple[List[List[str]], List[int], Dict[str, int]]:
+    def generateTimeStamps(node) -> list:
+        """
+        To get the timestamps of a node
+
+        :param node: A node in the tree
+        :return: Timestamps of a node
+        """
+
+        finalTimeStamps = node.timeStamps
+        return finalTimeStamps
+
+    def removeNode(self, nodeValue) -> None:
+        """
+        Removing the node from tree
+
+        :param nodeValue: To represent a node in the tree
+        :type nodeValue: node
+        :return: Tree with their nodes updated with timestamps
         """
-        To calculate the frequency of items in conditional patterns and sorting the patterns
 
-        :param ConditionalPatterns: paths of a node
-        :param conditionalFreq: frequency of each item in the path
-        :return: conditional patterns and frequency of each item in transactions
+        for i in self.summaries[nodeValue]:
+            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
+            del i.parent.children[nodeValue]
+
+    def getTimeStamps(self, alpha) -> list:
+        """
+        To get all the timestamps of the nodes which share same item name
+
+        :param alpha: Node in a tree
+        :return: Timestamps of a  node
+        """
+        temporary = []
+        for i in self.summaries[alpha]:
+            temporary += i.timeStamps
+        return temporary
+
+    @staticmethod
+    def getSupportAndPeriod(timeStamps: list, pattern: list) -> list:
         """
-        global _minSup, _miniWeight
+        To calculate the periodicity and support
+
+        :param timeStamps: Timestamps of an item set
+        :type timeStamps: list
+        :param pattern: pattern to evaluate the weighted frequent regular or not
+        :type pattern: list
+        :return: support, periodicity
+        """
+        global _WS, _regularity, _lno, _weights
+        timeStamps.sort()
+        cur = 0
+        per = list()
+        sup = 0
+        for j in range(len(timeStamps)):
+            per.append(timeStamps[j] - cur)
+            cur = timeStamps[j]
+            sup += 1
+        per.append(_lno - cur)
+        l = int()
+        for i in pattern:
+            l = l + _weights[i]
+        wf = (l / (len(pattern))) * sup
+        if len(per) == 0:
+            return [0, 0]
+        return [sup, max(per), wf]
+
+    def conditionalDatabases(self, conditionalPatterns: list, conditionalTimeStamps: list, pattern: list) -> tuple:
+        """
+        It generates the conditional patterns with periodic-frequent items
+
+        :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
+        :type conditionalPatterns: list
+        :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
+        :type conditionalTimeStamps: list
+        :param pattern: prefix of the pattern
+        :type pattern: list
+        :returns: Returns conditional transactions by removing non-periodic and non-frequent items
+        """
+        global _WS, _regularity
         pat = []
-        freq = []
+        timeStamps = []
         data1 = {}
-        for i in range(len(ConditionalPatterns)):
-            for j in ConditionalPatterns[i]:
+        for i in range(len(conditionalPatterns)):
+            for j in conditionalPatterns[i]:
                 if j in data1:
-                    data1[j] += conditionalFreq[i]
+                    data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
-                    data1[j] = conditionalFreq[i]
-        up_dict = {k: v for k, v in data1.items() if v >= _minSup and v * _miniWeight > _minSup}
+                    data1[j] = conditionalTimeStamps[i]
+        updatedDictionary = {}
+        for m in data1:
+            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
         count = 0
-        for p in ConditionalPatterns:
-            p1 = [v for v in p if v in up_dict]
-            trans = sorted(p1, key=lambda x: (up_dict.get(x), -x), reverse=True)
+        for p in conditionalPatterns:
+            p1 = [v for v in p if v in updatedDictionary]
+            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                freq.append(conditionalFreq[count])
+                timeStamps.append(conditionalTimeStamps[count])
             count += 1
-        return pat, freq, up_dict
+        return pat, timeStamps, updatedDictionary
 
-    def generatePatterns(self, prefix: List[str]) -> Generator[Tuple[List[str], int], None, None]:
+    def generatePatterns(self, prefix: list) -> None:
         """
-        To generate the frequent patterns
+        Generates the patterns
 
-        :param prefix: an empty list
-        :return: Frequent patterns that are extracted from fp-tree
+        :param prefix: Forms the combination of items
+        :type prefix: list
+        :returns: yields patterns with their support and periodicity
         """
-        global _miniWeight, _maxWeight, _minWeight, _minSup
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
+        global _WS
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
             pattern = prefix[:]
             pattern.append(i)
-            yield pattern, self.info[i]
-            patterns, freq, info = self.getFinalConditionalPatterns(i)
-            conditionalTree = _Tree()
-            conditionalTree.info = info.copy()
-            for pat in range(len(patterns)):
-                conditionalTree.addTransaction(patterns[pat], freq[pat])
-            if len(patterns) > 0:
-                for q in conditionalTree.generatePatterns(pattern):
-                    yield q
+            if self.info[i][2] >= _WS:
+                yield pattern, self.info[i]
+                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+                conditionalTree = _Tree()
+                conditionalTree.info = info.copy()
+                for pat in range(len(patterns)):
+                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                if len(patterns) > 0:
+                    for q in conditionalTree.generatePatterns(pattern):
+                        yield q
+            self.removeNode(i)
 
 
-class WFIM(_fp._weightedFrequentPatterns):
+class WFRIMiner(_fp._weightedFrequentRegularPatterns):
     """
-    :Description:
-       * WFMiner is one of the fundamental algorithm to discover weighted frequent patterns in a transactional database.
-       * It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
-
-    :Reference :
-           U. Yun and J. J. Leggett, “Wfim: weighted frequent itemset mining with a weight range and a minimum weight,”
-           in Proceedings of the 2005 SIAM International Conference on Data Mining. SIAM, 2005, pp. 636–640.
-           https://epubs.siam.org/doi/pdf/10.1137/1.9781611972757.76
+    :Description: WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
+       * It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+
+    :Reference:
+           K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
+           2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
+           doi: 10.1109/KST.2017.7886090.
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of weighted Frequent Patterns.
+                   Name of the Input file to mine complete set of Weighted Frequent Regular Patterns.
     :param  oFile: str :
-                   Name of the output file to store complete set of weighted Frequent Patterns.
-    :param  minSup: str or int or float:
-                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
+                   Name of the output file to store complete set of Weighted Frequent Regular Patterns.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+    :param  wFile: str :
+                This is a weighted file.
 
-
-    :Attributes :
+    :Attributes:
 
         iFile : file
             Input file name or path of the input file
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        WS: float or int or str
+            The user can specify WS either in count or proportion of database size.
+            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        minWeight: float or int or str
-            The user can specify minWeight either in count or proportion of database size.
-            If the program detects the data type of minWeight is integer, then it treats minWeight is expressed in count.
+            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
+        regularity: float or int or str
+            The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minWeight=10 will be treated as integer, while minWeight=10.0 will be treated as float
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
         oFile : file
             Name of the output file or the path of the output file
         startTime:float
             To record the start time of the mining process
@@ -290,22 +371,22 @@
         lno : int
             it represents the total no of transactions
         tree : class
             it represents the Tree class
         finalPatterns : dict
             it represents to store the patterns
 
-    :Methods :
+    :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
+            Complete set of frequent patterns will be loaded in to an output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
@@ -316,408 +397,423 @@
             Extracts the one-frequent patterns from transactions
 
     **Methods to execute code on terminal**
     -------------------------------------------
     .. code-block:: console
 
 
-       Format:
+      Format:
 
-       (.venv) $ python3 basic.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
+      (.venv) $ python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
 
-       Example Usage:
+      Example Usage:
 
-       (.venv) $ python3 basic.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
+      (.venv) $ python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
 
 
-               .. note:: minSup and maxPer will be considered in support count or frequency
+              .. note:: WS & regularity will be considered in support count or frequency
 
 
     **Importing this algorithm into a python program**
-    -----------------------------------------------------
+    ----------------------------------------------------
     .. code-block:: python
 
-            from PAMI.weightFrequentPattern.basic import basic as alg
+            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 
-            obj = alg.basic(iFile, wFile, minSup, minWeight)
+            obj = alg.WFRIMiner(iFile, WS, regularity)
 
             obj.startMine()
 
-            frequentPatterns = obj.getPatterns()
+            weightedFrequentRegularPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 
-            obj.savePatterns(oFile)
+            obj.save(oFile)
 
-            Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getmemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    ----------------------
+    ----------------
              The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
         """
 
-    __startTime = float()
-    __endTime = float()
-    _minSup = str()
-    __finalPatterns = {}
+    _startTime = float()
+    _endTime = float()
+    _WS = str()
+    _regularity = str()
+    _weight = {}
+    _finalPatterns = {}
+    _wFile = " "
     _iFile = " "
     _oFile = " "
     _sep = " "
-    __memoryUSS = float()
-    __memoryRSS = float()
-    __Database = []
-    __mapSupport = {}
-    __lno = 0
-    __tree = _Tree()
-    __rank = {}
-    __rankDup = {}
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _mapSupport = {}
+    _lno = 0
+    _tree = _Tree()
+    _rank = {}
+    _rankDup = {}
 
-    def __init__(self, iFile: str, wFile: str, minSup: str, minWeight: int, sep: str='\t') -> None:
-        super().__init__(iFile, wFile, minSup, minWeight, sep)
+    def __init__(self, iFile, _wFile, WS, regularity, sep='\t') -> None:
+        super().__init__(iFile, _wFile, WS, regularity, sep)
 
-    def __creatingItemSets(self) -> None:
+    def _creatingItemSets(self) -> None:
         """
         Storing the complete transactions of the database/input file in a database variable
         :return: None
         """
-        self.__Database = []
+        self._Database = []
+        self._weight = {}
         if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self.__Database = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
+
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            _items, _weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                _items = self._wFile['items'].tolist()
+            if 'weight' in i:
+                _weights = self._wFile['weight'].tolist()
+            for i in range(len(_items)):
+                self._weight[_items[i]] = _weights[i]
 
             # print(self.Database)
         if isinstance(self._iFile, str):
             if _fp._validators.url(self._iFile):
                 data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self.__Database.append(temp)
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            # print(len(temp))
-                            self.__Database.append(temp)
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _scanningWeights(self) -> None:
-        """
-        Storing the weights of the variables in input file in a weights variable
-        :return: None
-        """
-        global _weights
-        _weights = {}
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            items, weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                items = self._wFile['items'].tolist()
-            if 'weights' in i:
-                weights = self._wFile['weights'].tolist()
-            for i in range(len(weights)):
-                _weights[items[i]] = weights[i]
-
-            # print(self.Database)
         if isinstance(self._wFile, str):
             if _fp._validators.url(self._wFile):
                 data = _fp._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    _weights[temp[0]] = temp[1]
+                    self._weight[temp[0]] = float(temp[1])
             else:
                 try:
                     with open(self._wFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            s = int(float(temp[1]))
-                            _weights[temp[0]] = s
+                            self._weight[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def __convert(self, value: Union[int, float, str]) -> Union[int, float]:
+    def _convert(self, value) -> float:
         """
-        To convert the type of user specified minSup value.
+        To convert the type of user specified minSup value
 
         :param value: user specified minSup value
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self.__Database) * value)
+            value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self.__Database) * value)
+                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def __frequentOneItem(self) -> List[str]:
+    def _frequentOneItem(self) -> List[str]:
         """
         Generating One frequent items sets
         :return: list
         """
-        global _maxWeight
-        self.__mapSupport = {}
-        for tr in self.__Database:
-            for i in range(0, len(tr)):
-                if tr[i] not in self.__mapSupport:
-                    self.__mapSupport[tr[i]] = 1
+        global _lno, _wf, _weights
+        self._mapSupport = {}
+        _owf = {}
+        for tr in self._Database:
+            for i in range(1, len(tr)):
+                if tr[i] not in self._mapSupport:
+                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
                 else:
-                    self.__mapSupport[tr[i]] += 1
-        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup and v * _maxWeight > self._minSup}
-        genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
+                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
+                    self._mapSupport[tr[i]][1] = int(tr[0])
+                    self._mapSupport[tr[i]][2] += 1
+        for key in self._mapSupport:
+            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
+        _lno = len(self._Database)
+        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
+        for x, y in self._mapSupport.items():
+            if self._weight.get(x) is None:
+                self._weight[x] = 0
+        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
+        for x, y in self._mapSupport.items():
+            _owf[x] = y[0] * gmax
+        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
+        for x, y in self._mapSupport.items():
+            temp = self._weight[x] * y[0]
+            _wf[x] = temp
+            self._mapSupport[x].append(temp)
+        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
+        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        for x, y in self._rank.items():
+            _weights[y] = self._weight[x]
         return genList
 
-    def __updateTransactions(self, itemSet: List[str]) -> List[List[int]]:
+    def _updateTransactions(self, itemSet) -> List[List[int]]:
         """
         Updates the items in transactions with rank of items according to their support
-        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
-                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+
+        :Example:
+        oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
+        rank = {'a':0, 'b':1, 'c':2, 'd':3}
 
         :param itemSet: list of one-frequent items
-        :return: list
+        :return: None
         """
         list1 = []
-        for tr in self.__Database:
-            list2 = []
-            for i in range(len(tr)):
+        for tr in self._Database:
+            list2 = [int(tr[0])]
+            for i in range(1, len(tr)):
                 if tr[i] in itemSet:
-                    list2.append(self.__rank[tr[i]])
-            if len(list2) >= 1:
-                list2.sort()
+                    list2.append(self._rank[tr[i]])
+            if len(list2) >= 2:
+                basket = list2[1:]
+                basket.sort()
+                list2[1:] = basket[0:]
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def __buildTree(transactions: List[List[int]], info: Dict[int, int]) -> '_Tree':
+    def _buildTree(transactions, info) -> _Tree:
         """
         Builds the tree with updated transactions
 
         :param transactions: updated transactions
-        :param info: support details of each item in transactions.
-        :return: Transactions compressed in fp-tree
+        :param info: support details of each item in transactions
+        :return: transactions compressed in fp-tree
+
         """
         rootNode = _Tree()
         rootNode.info = info.copy()
         for i in range(len(transactions)):
-            rootNode.addTransaction(transactions[i], 1)
+            set1 = [transactions[i][0]]
+            rootNode.addTransaction(transactions[i][1:], set1)
         return rootNode
 
-    def __savePeriodic(self, itemSet: List[int]) -> str:
+    def _savePeriodic(self, itemSet) -> str:
         """
         The duplication items and their ranks
 
         :param itemSet: frequent itemSet that generated
         :return: patterns with original item names.
+
         """
         temp = str()
         for i in itemSet:
-            temp = temp + self.__rankDup[i] + "\t"
+            temp = temp + self._rankDup[i] + "\t"
         return temp
 
     @deprecated("It is recommended to use mine() instead of startMine() for mining process")
     def startMine(self) -> None:
         """
         main program to start the operation
         :return: None
         """
-        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
-        self.__startTime = _fp._time.time()
+        global _WS, _regularity, _weights
+        self._startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._WS is None:
             raise Exception("Please enter the Minimum Support")
-        self.__creatingItemSets()
-        self._scanningWeights()
-        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
-        _maxWeight = max([s for s in _weights.values()])
-        _miniWeight = min([s for s in _weights.values()])
-        self._minSup = self.__convert(self._minSup)
-        _minSup = self._minSup
-        itemSet = self.__frequentOneItem()
-        updatedTransactions = self.__updateTransactions(itemSet)
-        for x, y in self.__rank.items():
-            self.__rankDup[y] = x
-        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
-        __Tree = self.__buildTree(updatedTransactions, info)
-        patterns = __Tree.generatePatterns([])
-        self.__finalPatterns = {}
+        self._creatingItemSets()
+        self._WS = self._convert(self._WS)
+        self._regularity = self._convert(self._regularity)
+        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
+        itemSet = self._frequentOneItem()
+        updatedTransactions = self._updateTransactions(itemSet)
+        for x, y in self._rank.items():
+            self._rankDup[y] = x
+        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
+        _Tree = self._buildTree(updatedTransactions, info)
+        patterns = _Tree.generatePatterns([])
+        self._finalPatterns = {}
         for k in patterns:
-            s = self.__savePeriodic(k[0])
-            self.__finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent patterns were generated successfully using basic algorithm")
-        self.__endTime = _fp._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
+            s = self._savePeriodic(k[0])
+            self._finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
+        self._endTime = _fp._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
 
     def Mine(self) -> None:
         """
         main program to start the operation
         :return: None
         """
-        global _minSup, _minWeight, _miniWeight, _maxWeight, _weights
-        self.__startTime = _fp._time.time()
+        global _WS, _regularity, _weights
+        self._startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
+        if self._WS is None:
             raise Exception("Please enter the Minimum Support")
-        self.__creatingItemSets()
-        self._scanningWeights()
-        _weights = {k: v for k, v in _weights.items() if v >= _minWeight}
-        _maxWeight = max([s for s in _weights.values()])
-        _miniWeight = min([s for s in _weights.values()])
-        self._minSup = self.__convert(self._minSup)
-        _minSup = self._minSup
-        itemSet = self.__frequentOneItem()
-        updatedTransactions = self.__updateTransactions(itemSet)
-        for x, y in self.__rank.items():
-            self.__rankDup[y] = x
-        info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
-        __Tree = self.__buildTree(updatedTransactions, info)
-        patterns = __Tree.generatePatterns([])
-        self.__finalPatterns = {}
+        self._creatingItemSets()
+        self._WS = self._convert(self._WS)
+        self._regularity = self._convert(self._regularity)
+        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
+        itemSet = self._frequentOneItem()
+        updatedTransactions = self._updateTransactions(itemSet)
+        for x, y in self._rank.items():
+            self._rankDup[y] = x
+        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
+        _Tree = self._buildTree(updatedTransactions, info)
+        patterns = _Tree.generatePatterns([])
+        self._finalPatterns = {}
         for k in patterns:
-            s = self.__savePeriodic(k[0])
-            self.__finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent patterns were generated successfully using basic algorithm")
-        self.__endTime = _fp._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
+            s = self._savePeriodic(k[0])
+            self._finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
+        self._endTime = _fp._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
-
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryUSS
+        return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
         """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function.
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryRSS
+        return self._memoryRSS
 
     def getRuntime(self) -> float:
         """
-        Calculating the total amount of runtime taken by the mining process.
+        Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self.__endTime - self.__startTime
+        return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> pd.DataFrame:
+    def getPatternsAsDataFrame(self) -> _fp._pd.DataFrame:
         """
-        Storing final frequent patterns in a dataframe.
+        Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self.__finalPatterns.items():
+        for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
-        Complete set of frequent patterns will be loaded in to an output file.
+        Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: csv file
         :return: None
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
-        for x, y in self.__finalPatterns.items():
+        for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, int]:
+    def getPatterns(self) -> Dict[str, float]:
         """
-        Function to send the set of frequent patterns after completion of the mining process.
+        Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
-        return self.__finalPatterns
+        return self._finalPatterns
 
     def printResults(self) -> None:
         """
         This function is used to print the results
         :return: None
         """
-        print("Total number of  Weighted Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
-        
-
 
 if __name__ == "__main__":
     _ap = str()
     if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
         if len(_fp._sys.argv) == 7:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 6:
-            _ap = WFIM(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 5:
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        print("Total number of Weighted Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
         _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
-# It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+# WUFIM is one of the algorithm to discover weighted frequent patterns in an uncertain transactional database using PUF-Tree.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.weightedFrequentRegularPattern.basic import WFRIMiner as alg
+#             from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 #
-#             obj = alg.WFRIMiner(iFile, WS, regularity)
+#             obj = alg.basic(iFile, wFile, minSup, sep)
 #
 #             obj.startMine()
 #
-#             weightedFrequentRegularPatterns = obj.getPatterns()
+#             Patterns = obj.getPatterns()
 #
-#             print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+#             print("Total number of  Patterns:", len(Patterns))
 #
 #             obj.save(oFile)
 #
-#             Df = obj.getPatternInDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
 #             print("Total Memory in USS:", memUSS)
 #
 #             memRSS = obj.getMemoryRSS()
 #
@@ -29,791 +28,825 @@
 #
 #             run = obj.getRuntime()
 #
 #             print("Total ExecutionTime in seconds:", run)
 #
 
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
 
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
-     along with this program.  If not, see <https://www.gnu.org/licenses/>.
-     Copyright (C)  2021 Rage Uday Kiran
-
+     along with this program.  If not, see `<https://www.gnu.org/licenses/>`_.
+     
 """
 
-from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
+from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
 import pandas as pd
 from deprecated import deprecated
-from typing import List, Dict
-
 
-_WS = str()
-_regularity = str()
-_lno = int()
+_expSup = str()
+_expWSup = str()
 _weights = {}
-_wf = {}
-_fp._sys.setrecursionlimit(20000)
+_finalPatterns = {}
+_ab._sys.setrecursionlimit(20000)
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+
+    :Attributes:
+
+        item : int or word
+            Represents the name of the item
+
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item: int, probability: float) -> None:
+        self.item = item
+        self.probability = probability
 
 
-class _Node:
+class _Node(object):
     """
     A class used to represent the node of frequentPatternTree
 
     :Attributes:
-        itemId: int
+
+        item : int
             storing item of a node
-        counter: int
-            To maintain the support of node
-        parent: node
-            To maintain the parent of node
-        children: list
+        probability : int
+            To maintain the expected support of node
+        parent : node
+            To maintain the parent of every node
+        children : list
             To maintain the children of node
 
     :Methods:
-        addChild(node)
-            Updates the nodes children list and parent for the given node
 
+        addChild(itemName)
+            storing the children to their respective parent nodes
     """
 
-    def __init__(self, item: int, children: dict) -> None:
-        """
-        Initializing the Node class
-
-        :param item: Storing the item of a node
-        :type item: int or None
-        :param children: To maintain the children of a node
-        :type children: dict
-        :return: None
-        """
-
+    def __init__(self, item, children: list) -> None:
         self.item = item
+        self.probability = 1
         self.children = children
         self.parent = None
-        self.timeStamps = []
 
     def addChild(self, node) -> None:
-        """
-        To add the children to a node
-
-        :param node: parent node in the tree
-        :return: None
-        """
-
         self.children[node.item] = node
         node.parent = self
 
 
-class _Tree:
+class _Tree(object):
     """
     A class used to represent the frequentPatternGrowth tree structure
 
     :Attributes:
+
         root : Node
-            The first node of the tree set to Null.
+            Represents the root node of the tree
         summaries : dictionary
-            Stores the nodes itemId which shares same itemId
+            storing the nodes with same item name
         info : dictionary
-            frequency of items in the transactions
+            stores the support of items
 
     :Methods:
-        addTransaction(transaction, freq)
-            adding items of  transactions into the tree as nodes and freq is the count of nodes
-        getFinalConditionalPatterns(node)
-            getting the conditional patterns from fp-tree for a node
-        getConditionalPatterns(patterns, frequencies)
-            sort the patterns by removing the items with lower minSup
-        generatePatterns(prefix)
-            generating the patterns from fp-tree
+
+        addTransaction(transaction)
+            creating transaction as a branch in frequentPatternTree
+        addConditionalPattern(prefixPaths, supportOfItems)
+            construct the conditional tree for prefix paths
+        conditionalPatterns(Node)
+            generates the conditional patterns from tree for specific node
+        conditionalTransactions(prefixPaths,Support)
+            takes the prefixPath of a node and support at child of the path and extract the frequent items from prefixPaths and generates prefixPaths with items which are frequent
+        remove(Node)
+            removes the node from tree once after generating all the patterns respective to the node
+        generatePatterns(Node)
+            starts from the root node of the tree and mines the frequent patterns
+
     """
 
     def __init__(self) -> None:
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
-    def addTransaction(self, transaction: list, tid: list) -> None:
+    def addTransaction(self, transaction) -> None:
         """
-        Adding a transaction into tree
+        Adding transaction into tree
 
-        :param transaction: To represent the complete database
-        :type transaction: list
-        :param tid: To represent the timestamp of a database
-        :type tid: list
-        :return: pfp-growth tree
+        :param transaction : it represents the one self.Database in database
+        :type transaction : list
+        :return: None
         """
         currentNode = self.root
         for i in range(len(transaction)):
+            if transaction[i].item not in currentNode.children:
+                newNode = _Node(transaction[i].item, {})
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    newNode.probability = transaction[i].probability
+                else:
+                    newNode.probability = max(lp) * transaction[i].probability
+                currentNode.addChild(newNode)
+                if transaction[i].item in self.summaries:
+                    self.summaries[transaction[i].item].append(newNode)
+                else:
+                    self.summaries[transaction[i].item] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i].item]
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    currentNode.probability += transaction[i].probability
+                else:
+                    currentNode.probability += max(lp) * transaction[i].probability
+
+    def addConditionalPattern(self, transaction, sup) -> None:
+        """
+        constructing conditional tree from prefixPaths
+
+        :param transaction : it represents the one self.Database in database
+        :type transaction : list
+        :param sup : support of prefixPath taken at last child of the path
+        :type sup : int
+        :return: None
+
+        """
+        # This method takes transaction, support and constructs the conditional tree
+        currentNode = self.root
+        for i in range(len(transaction)):
             if transaction[i] not in currentNode.children:
                 newNode = _Node(transaction[i], {})
+                newNode.probability = sup
                 currentNode.addChild(newNode)
                 if transaction[i] in self.summaries:
                     self.summaries[transaction[i]].append(newNode)
                 else:
                     self.summaries[transaction[i]] = [newNode]
                 currentNode = newNode
             else:
                 currentNode = currentNode.children[transaction[i]]
-        currentNode.timeStamps = currentNode.timeStamps + tid
+                currentNode.probability += sup
 
-    def getConditionalPatterns(self, alpha, pattern) -> tuple:
+    def conditionalPatterns(self, alpha) -> tuple:
         """
-        Generates all the conditional patterns of a respective node
+        generates all the conditional patterns of respective node
+
+        :param alpha : it represents the Node in tree
+        :type alpha : _Node
 
-        :param alpha: To represent a Node in the tree
-        :type alpha: Node
-        :param pattern: prefix of the pattern
-        :type alpha: list
-        :return: A tuple consisting of finalPatterns, conditional pattern base and information
         """
+        # This method generates conditional patterns of node by traversing the tree
         finalPatterns = []
-        finalSets = []
+        sup = []
         for i in self.summaries[alpha]:
-            set1 = i.timeStamps
+            s = i.probability
             set2 = []
             while i.parent.item is not None:
                 set2.append(i.parent.item)
                 i = i.parent
             if len(set2) > 0:
                 set2.reverse()
                 finalPatterns.append(set2)
-                finalSets.append(set1)
-        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
-        return finalPatterns, finalSets, info
-
-    @staticmethod
-    def generateTimeStamps(node) -> list:
-        """
-        To get the timestamps of a node
-
-        :param node: A node in the tree
-        :return: Timestamps of a node
-        """
-
-        finalTimeStamps = node.timeStamps
-        return finalTimeStamps
+                sup.append(s)
+        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
+        return finalPatterns, support, info
 
     def removeNode(self, nodeValue) -> None:
+
         """
         Removing the node from tree
 
-        :param nodeValue: To represent a node in the tree
-        :type nodeValue: node
-        :return: Tree with their nodes updated with timestamps
+        :param nodeValue : it represents the node in tree
+        :type nodeValue : node
+        :return: None
         """
 
         for i in self.summaries[nodeValue]:
-            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
             del i.parent.children[nodeValue]
 
-    def getTimeStamps(self, alpha) -> list:
+    def conditionalTransactions(self, condPatterns, support) -> tuple:
         """
-        To get all the timestamps of the nodes which share same item name
+        It generates the conditional patterns with frequent items
 
-        :param alpha: Node in a tree
-        :return: Timestamps of a  node
+        :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
+        :type condPatterns : list
+        :support : the support of conditional pattern in tree
+        :support : int
+        :return: tuple
         """
-        temporary = []
-        for i in self.summaries[alpha]:
-            temporary += i.timeStamps
-        return temporary
-
-    @staticmethod
-    def getSupportAndPeriod(timeStamps: list, pattern: list) -> list:
-        """
-        To calculate the periodicity and support
-
-        :param timeStamps: Timestamps of an item set
-        :type timeStamps: list
-        :param pattern: pattern to evaluate the weighted frequent regular or not
-        :type pattern: list
-        :return: support, periodicity
-        """
-        global _WS, _regularity, _lno, _weights
-        timeStamps.sort()
-        cur = 0
-        per = list()
-        sup = 0
-        for j in range(len(timeStamps)):
-            per.append(timeStamps[j] - cur)
-            cur = timeStamps[j]
-            sup += 1
-        per.append(_lno - cur)
-        l = int()
-        for i in pattern:
-            l = l + _weights[i]
-        wf = (l / (len(pattern))) * sup
-        if len(per) == 0:
-            return [0, 0]
-        return [sup, max(per), wf]
-
-    def conditionalDatabases(self, conditionalPatterns: list, conditionalTimeStamps: list, pattern: list) -> tuple:
-        """
-        It generates the conditional patterns with periodic-frequent items
-
-        :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
-        :type conditionalPatterns: list
-        :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
-        :type conditionalTimeStamps: list
-        :param pattern: prefix of the pattern
-        :type pattern: list
-        :returns: Returns conditional transactions by removing non-periodic and non-frequent items
-        """
-        global _WS, _regularity
+        global _expSup, _expWSup
         pat = []
-        timeStamps = []
-        data1 = {}
-        for i in range(len(conditionalPatterns)):
-            for j in conditionalPatterns[i]:
-                if j in data1:
-                    data1[j] = data1[j] + conditionalTimeStamps[i]
+        sup = []
+        count = {}
+        for i in range(len(condPatterns)):
+            for j in condPatterns[i]:
+                if j in count:
+                    count[j] += support[i]
                 else:
-                    data1[j] = conditionalTimeStamps[i]
-        updatedDictionary = {}
-        for m in data1:
-            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
-        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
+                    count[j] = support[i]
+        updatedDict = {}
+        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
         count = 0
-        for p in conditionalPatterns:
-            p1 = [v for v in p if v in updatedDictionary]
-            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
+        for p in condPatterns:
+            p1 = [v for v in p if v in updatedDict]
+            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
             if len(trans) > 0:
                 pat.append(trans)
-                timeStamps.append(conditionalTimeStamps[count])
-            count += 1
-        return pat, timeStamps, updatedDictionary
+                sup.append(support[count])
+                count += 1
+        return pat, sup, updatedDict
 
-    def generatePatterns(self, prefix: list) -> None:
+    def generatePatterns(self, prefix) -> None:
         """
         Generates the patterns
 
-        :param prefix: Forms the combination of items
-        :type prefix: list
-        :returns: yields patterns with their support and periodicity
+        :param prefix : forms the combination of items
+        :type prefix : list
+        :return: None
         """
-        global _WS
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
+
+        global _finalPatterns, _expSup, _expWSup, _weights
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
             pattern = prefix[:]
             pattern.append(i)
-            if self.info[i][2] >= _WS:
-                yield pattern, self.info[i]
-                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+            weight = 0
+            for k in pattern:
+                weight = weight + _weights[k]
+            weight = weight/len(pattern)
+            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
+                _finalPatterns[tuple(pattern)] = self.info.get(i)
+                patterns, support, info = self.conditionalPatterns(i)
                 conditionalTree = _Tree()
                 conditionalTree.info = info.copy()
                 for pat in range(len(patterns)):
-                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
                 if len(patterns) > 0:
-                    for q in conditionalTree.generatePatterns(pattern):
-                        yield q
+                    conditionalTree.generatePatterns(pattern)
             self.removeNode(i)
 
-
-class WFRIMiner(_fp._weightedFrequentRegularPatterns):
+class WUFIM(_ab._weightedFrequentPatterns):
     """
-    :Description: WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
-       * It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
+    :Description: It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database using PUF-Tree.
 
-    :Reference:
-           K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
-           2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
-           doi: 10.1109/KST.2017.7886090.
+    :Reference: Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases, In book: Machine Learning and Data Mining in Pattern Recognition Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of Weighted Frequent Regular Patterns.
+                   Name of the Input file to mine complete set of Weighted Uncertain Periodic Frequent Patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of Weighted Frequent Regular Patterns.
+                   Name of the output file to store complete set of Weighted  Uncertain Periodic Frequent Patterns
+    :param  minSup: str:
+                   minimum support thresholds were tuned to find the appropriate ranges in the limited memory
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
     :param  wFile: str :
-                This is a weighted file.
+                    This is a weighted file.
+
 
     :Attributes:
 
         iFile : file
-            Input file name or path of the input file
-        WS: float or int or str
-            The user can specify WS either in count or proportion of database size.
-            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
-        regularity: float or int or str
-            The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+            Name of the Input file or path of the input file
+        wFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup : float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
-        oFile : file
-            Name of the output file or the path of the output file
-        startTime:float
-            To record the start time of the mining process
-        endTime:float
-            To record the completion time of the mining process
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
         tree : class
-            it represents the Tree class
+            To represents the Tree class
+        itemSetCount : int
+            To represents the total no of patterns
         finalPatterns : dict
-            it represents to store the patterns
+            To store the complete patterns
 
     :Methods:
 
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to an output file
+            Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets()
-            Scans the dataset or dataframes and stores in list format
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
         frequentOneItem()
-            Extracts the one-frequent patterns from transactions
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
     **Methods to execute code on terminal**
-    -------------------------------------------
+    --------------------------------------------
     .. code-block:: console
 
 
       Format:
 
-      (.venv) $ python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
+      (.venv) $ python3 basic.py <inputFile> <outputFile> <minSup>
 
       Example Usage:
 
-      (.venv) $ python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
+      (.venv) $ python3 basic.py sampleTDB.txt patterns.txt 3
 
 
-              .. note:: WS & regularity will be considered in support count or frequency
+              .. note:: minSup  will be considered in support count or frequency
 
 
     **Importing this algorithm into a python program**
-    ----------------------------------------------------
+    -----------------------------------------------------
     .. code-block:: python
 
-            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
+            from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 
-            obj = alg.WFRIMiner(iFile, WS, regularity)
+            obj = alg.basic(iFile, wFile, expSup, expWSup)
 
             obj.startMine()
 
-            weightedFrequentRegularPatterns = obj.getPatterns()
+            Patterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
+            print("Total number of  Patterns:", len(Patterns))
 
             obj.save(oFile)
 
-            Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
             memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
-
-    **Credits:**
-    ----------------
-             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
-
-        """
-
+   """
     _startTime = float()
     _endTime = float()
-    _WS = str()
-    _regularity = str()
-    _weight = {}
+    _minSup = str()
     _finalPatterns = {}
-    _wFile = " "
     _iFile = " "
+    _wFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
-    _lno = 0
-    _tree = _Tree()
     _rank = {}
-    _rankDup = {}
+    _expSup = float()
+    _expWSup = float()
 
-    def __init__(self, iFile, _wFile, WS, regularity, sep='\t') -> None:
-        super().__init__(iFile, _wFile, WS, regularity, sep)
+    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t') -> None:
+        super().__init__(iFile, wFile, expSup, expWSup, sep)
 
     def _creatingItemSets(self) -> None:
         """
-        Storing the complete transactions of the database/input file in a database variable
+        Scans the uncertain transactional dataset
         :return: None
         """
         self._Database = []
-        self._weight = {}
-        if isinstance(self._iFile, _fp._pd.DataFrame):
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-
-        if isinstance(self._wFile, _fp._pd.DataFrame):
-            _items, _weights = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                _items = self._wFile['items'].tolist()
-            if 'weight' in i:
-                _weights = self._wFile['weight'].tolist()
-            for i in range(len(_items)):
-                self._weight[_items[i]] = _weights[i]
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _fp._validators.url(self._iFile):
-                data = _fp._urlopen(self._iFile)
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line.strip()
                     line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    line = line.strip()
+                    line = [i for i in line.split(':')]
+                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                    temp1 = [x for x in temp1 if x]
+                    temp2 = [x for x in temp2 if x]
+                    tr = []
+                    for i in range(len(temp1)):
+                        item = temp1[i]
+                        probability = float(temp2[i])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(tr)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            line = line.strip()
+                            line = [i for i in line.split(':')]
+                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                            temp1 = [x for x in temp1 if x]
+                            temp2 = [x for x in temp2 if x]
+                            tr = []
+                            for i in range(len(temp1)):
+                                item = temp1[i]
+                                probability = float(temp2[i])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
 
+    def _scanningWeights(self) -> None:
+        """
+        Scans the uncertain transactional dataset
+        :return: None
+        """
+        self._weights = {}
+        if isinstance(self._wFile, _ab._pd.DataFrame):
+            weights, data = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                data = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for k in range(len(data)):
+                self._weights[data[k]] = int(float(weights[k]))
+
+            # print(self.Database)
         if isinstance(self._wFile, str):
-            if _fp._validators.url(self._wFile):
-                data = _fp._urlopen(self._wFile)
+            if _ab._validators.url(self._wFile):
+                data = _ab._urlopen(self._wFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._weight[temp[0]] = float(temp[1])
+                    self._weights[temp[0]] = int(float(temp[1]))
             else:
                 try:
-                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                    with open(self._wFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._weight[temp[0]] = float(temp[1])
+                            self._weights[temp[0]] = float(temp[1])
                 except IOError:
                     print("File Not Found")
-                    quit()
 
-    def _convert(self, value) -> float:
+    def _frequentOneItem(self) -> tuple:
         """
-        To convert the type of user specified minSup value
+        Takes the self.Database and calculates the support of each item in the dataset and assign the ranks to the items by decreasing support and returns the frequent items list
 
-        :param value: user specified minSup value
-        :return: converted type
+        :param self.Database : it represents the one self.Database in database
+        :type self.Database : list
+        :return: tuple
         """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
 
-    def _frequentOneItem(self) -> List[str]:
+        mapSupport = {}
+        for i in self._Database:
+            for j in i:
+                if j.item not in mapSupport:
+                    if self._weights.get(j.item) is not None:
+                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
+                else:
+                    mapSupport[j.item][0] += j.probability
+        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
+        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
+        return mapSupport, plist
+
+    @staticmethod
+    def _buildTree(data, info) -> _Tree:
         """
-        Generating One frequent items sets
-        :return: list
+        It takes the self.Database and support of each item and construct the main tree with setting root node as null
+        :param data : it represents the one self.Database in database
+        :type data : list
+        :param info : it represents the support of each item
+        :type info : dictionary
+        :return: tree
         """
-        global _lno, _wf, _weights
-        self._mapSupport = {}
-        _owf = {}
-        for tr in self._Database:
-            for i in range(1, len(tr)):
-                if tr[i] not in self._mapSupport:
-                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
-                else:
-                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
-                    self._mapSupport[tr[i]][1] = int(tr[0])
-                    self._mapSupport[tr[i]][2] += 1
-        for key in self._mapSupport:
-            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
-        _lno = len(self._Database)
-        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
-        for x, y in self._mapSupport.items():
-            if self._weight.get(x) is None:
-                self._weight[x] = 0
-        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
-        for x, y in self._mapSupport.items():
-            _owf[x] = y[0] * gmax
-        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
-        for x, y in self._mapSupport.items():
-            temp = self._weight[x] * y[0]
-            _wf[x] = temp
-            self._mapSupport[x].append(temp)
-        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
-        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
-        for x, y in self._rank.items():
-            _weights[y] = self._weight[x]
-        return genList
-
-    def _updateTransactions(self, itemSet) -> List[List[int]]:
-        """
-        Updates the items in transactions with rank of items according to their support
-
-        :Example:
-        oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
-        rank = {'a':0, 'b':1, 'c':2, 'd':3}
 
-        :param itemSet: list of one-frequent items
-        :return: None
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(data)):
+            rootNode.addTransaction(data[i])
+        return rootNode
+
+    def _updateTransactions(self, dict1) -> list:
+        """
+        Remove the items which are not frequent from self.Database and updates the self.Database with rank of items
+
+        :param dict1 : frequent items with support
+        :type dict1 : dictionary
+        :return: list
         """
         list1 = []
         for tr in self._Database:
-            list2 = [int(tr[0])]
-            for i in range(1, len(tr)):
-                if tr[i] in itemSet:
-                    list2.append(self._rank[tr[i]])
+            list2 = []
+            for i in range(0, len(tr)):
+                if tr[i].item in dict1:
+                    list2.append(tr[i])
             if len(list2) >= 2:
-                basket = list2[1:]
-                basket.sort()
-                list2[1:] = basket[0:]
+                basket = list2
+                basket.sort(key=lambda val: self.rank[val.item])
+                list2 = basket
                 list1.append(list2)
         return list1
 
     @staticmethod
-    def _buildTree(transactions, info) -> _Tree:
+    def _check(i, x) -> int:
         """
-        Builds the tree with updated transactions
+        To check the presence of item or pattern in transaction
 
-        :param transactions: updated transactions
-        :param info: support details of each item in transactions
-        :return: transactions compressed in fp-tree
+        :param x: it represents the pattern
+        :type x : list
+        :param i : represents the uncertain self.Database
+        :type i : list
+        :return: integer number
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
+    def _convert(self, value) -> float:
         """
-        rootNode = _Tree()
-        rootNode.info = info.copy()
-        for i in range(len(transactions)):
-            set1 = [transactions[i][0]]
-            rootNode.addTransaction(transactions[i][1:], set1)
-        return rootNode
+        To convert the type of user specified minSup value
 
-    def _savePeriodic(self, itemSet) -> str:
+        :param value: user specified minSup value
+        :return: converted type minSup value
         """
-        The duplication items and their ranks
-
-        :param itemSet: frequent itemSet that generated
-        :return: patterns with original item names.
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
+    def _removeFalsePositives(self) -> None:
+        """
+        To remove the false positive patterns generated in frequent patterns.
+        :return: patterns with accurate probability
         """
-        temp = str()
-        for i in itemSet:
-            temp = temp + self._rankDup[i] + "\t"
-        return temp
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            weight = 0
+            for i in x:
+                weight += self._weights[i]
+            weight = weight / len(x)
+            if weight * y >= self._expWSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
 
     @deprecated("It is recommended to use mine() instead of startMine() for mining process")
     def startMine(self) -> None:
         """
-        main program to start the operation
-        :return: None
+        startMine() method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patterns.
         """
-        global _WS, _regularity, _weights
-        self._startTime = _fp._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._WS is None:
-            raise Exception("Please enter the Minimum Support")
+        global _expSup, _expWSup, _weights, _finalPatterns
+        self._startTime = _ab._time.time()
+        self._Database, self._weights = [], {}
         self._creatingItemSets()
-        self._WS = self._convert(self._WS)
-        self._regularity = self._convert(self._regularity)
-        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
-        itemSet = self._frequentOneItem()
-        updatedTransactions = self._updateTransactions(itemSet)
-        for x, y in self._rank.items():
-            self._rankDup[y] = x
-        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
-        _Tree = self._buildTree(updatedTransactions, info)
-        patterns = _Tree.generatePatterns([])
+        self._scanningWeights()
+        _weights = self._weights
+        self._expSup = float(self._expSup)
+        self._expWSup = float(self._expWSup)
+        _expSup = self._expSup
+        _expWSup = self._expWSup
         self._finalPatterns = {}
-        for k in patterns:
-            s = self._savePeriodic(k[0])
-            self._finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
-        self._endTime = _fp._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        process = _fp._psutil.Process(_fp._os.getpid())
-        self._memoryRSS = float()
+        mapSupport, plist = self._frequentOneItem()
+        self.Database1 = self._updateTransactions(mapSupport)
+        info = {k: v for k, v in mapSupport.items()}
+        Tree1 = self._buildTree(self.Database1, info)
+        Tree1.generatePatterns([])
+        self._removeFalsePositives()
+        print("Weighted Frequent patterns were generated  successfully using basic algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
+        self.memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.memoryRSS = process.memory_info().rss
 
-    def Mine(self) -> None:
+    def mine(self) -> None:
         """
-        main program to start the operation
-        :return: None
+        mine() method where the patterns are mined by constructing tree and remove the false patterns by counting the original support of a patternS
         """
-        global _WS, _regularity, _weights
-        self._startTime = _fp._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._WS is None:
-            raise Exception("Please enter the Minimum Support")
+        global _expSup, _expWSup, _weights, _finalPatterns
+        self._startTime = _ab._time.time()
+        self._Database, self._weights = [], {}
         self._creatingItemSets()
-        self._WS = self._convert(self._WS)
-        self._regularity = self._convert(self._regularity)
-        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
-        itemSet = self._frequentOneItem()
-        updatedTransactions = self._updateTransactions(itemSet)
-        for x, y in self._rank.items():
-            self._rankDup[y] = x
-        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
-        _Tree = self._buildTree(updatedTransactions, info)
-        patterns = _Tree.generatePatterns([])
+        self._scanningWeights()
+        _weights = self._weights
+        self._expSup = float(self._expSup)
+        self._expWSup = float(self._expWSup)
+        _expSup = self._expSup
+        _expWSup = self._expWSup
         self._finalPatterns = {}
-        for k in patterns:
-            s = self._savePeriodic(k[0])
-            self._finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
-        self._endTime = _fp._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
-        process = _fp._psutil.Process(_fp._os.getpid())
-        self._memoryRSS = float()
+        mapSupport, plist = self._frequentOneItem()
+        self.Database1 = self._updateTransactions(mapSupport)
+        info = {k: v for k, v in mapSupport.items()}
+        Tree1 = self._buildTree(self.Database1, info)
+        Tree1.generatePatterns([])
+        self._removeFalsePositives()
+        print("Weighted Frequent patterns were generated  successfully using basic algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
+        self.memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self) -> float:
         """
         Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self) -> float:
         """
         Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
-
-        return self._memoryRSS
+        return self.memoryRSS
 
     def getRuntime(self) -> float:
         """
         Calculating the total amount of runtime taken by the mining process
-
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
-    def getPatternsAsDataFrame(self) -> _fp._pd.DataFrame:
+    def getPatternsAsDataFrame(self) -> pd.DataFrame:
         """
         Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
-
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            s = str()
+            for i in a:
+                s = s + i + " "
+            data.append([s, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile: str) -> None:
         """
         Complete set of frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
+        :param outFile: Specify name of the output file
         :type outFile: csv file
         :return: None
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x.strip() + ":" + str(y)
+            s = str()
+            for i in x:
+                s = s + i + "\t"
+            s1 = s.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
-    def getPatterns(self) -> Dict[str, float]:
+    def getPatterns(self) -> dict:
         """
         Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self) -> None:
         """
         This function is used to print the results
         :return: None
         """
-        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
-        if len(_fp._sys.argv) == 7:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 5:
-            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+        if len(_ab._sys.argv) == 6:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
-        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
-        _ap.save(_fp._sys.argv[2])
-        print("Total Memory in USS:",  _ap.getMemoryUSS())
+        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
+        print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        for k in [120, 140, 160, 180, 200]:
+            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
+                        k, 500, '\t')
+            _ap.startMine()
+            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
+            print("Total Memory in USS:", _ap.getMemoryUSS())
+            print("Total Memory in RSS", _ap.getMemoryRSS())
+            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2024.4.11.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2024.4.9.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2024.4.11.1/PKG-INFO` & `pami-2024.4.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.4.11.1
+Version: 2024.4.9.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,14 @@
 Requires-Dist: urllib3
 Requires-Dist: Pillow
 Requires-Dist: numpy
 Requires-Dist: sphinx-rtd-theme
 Requires-Dist: validators
 Requires-Dist: discord.py
 Requires-Dist: networkx
-Requires-Dist: deprecated
 Provides-Extra: gpu
 Requires-Dist: cupy; extra == "gpu"
 Requires-Dist: pycuda; extra == "gpu"
 Provides-Extra: spark
 Requires-Dist: pyspark; extra == "spark"
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
@@ -57,20 +56,15 @@
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
-
-
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -82,64 +76,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
-- [Evaluation](#evaluation)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -181,19 +161,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -214,95 +191,21 @@
 Frequent patterns were generated successfully using frequentPatternGrowth algorithm
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
-# Evaluation:
-
-***
-
-1. we compared three different Python libraries such as PAMI, mlxtend and efficient-apriori for Apriori.
-2. (Transactional_T10I4D100K.csv)is a transactional database downloaded from PAMI and
-used as a input file for all libraries.
-3. Minimum support values and seperator are also same.
-
-* The performance of the **Apriori algorithm** is shown in the graphical results below:
-1. Comparing the **Patterns Generated** by different Python libraries for the Apriori algorithm:
-
-   <img width="573" alt="Screenshot 2024-04-11 at 13 31 31" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/fd7974bc-ffe2-44dd-82e3-a5306a8a23bd">
-   
-2. Evaluating the **Runtime** of the Apriori algorithm across different Python libraries:
-
-   <img width="567" alt="Screenshot 2024-04-11 at 13 31 20" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d615ae3-dc0d-49ba-a880-4890bb1f11c5">
-
-3. Comparing the **Memory Consumption** of the Apriori algorithm across different Python libraries:
-
-   <img width="570" alt="Screenshot 2024-04-11 at 13 31 08" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d5991ca-51ae-442d-9b5e-2d21bbebfedd">
-
-For more information, we have uploaded the evaluation file in two formats:
-- One **ipynb** file format, please check it here. [Evaluation File ipynb](https://github.com/UdayLab/PAMI/blob/main/notebooks/Evaluation-neverDelete.ipynb) 
-- Two **pdf** file format, check here. [Evaluation File Pdf](https://github.com/UdayLab/PAMI/blob/main/notebooks/evaluation.pdf)
-
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
+ 
 ***
 
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
-***
-
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -491,14 +394,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -596,8 +501,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.11.1/README.md` & `pami-2024.4.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,15 @@
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
-
-
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -36,64 +31,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
-- [Evaluation](#evaluation)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -135,19 +116,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -168,95 +146,21 @@
 Frequent patterns were generated successfully using frequentPatternGrowth algorithm
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
-# Evaluation:
-
-***
-
-1. we compared three different Python libraries such as PAMI, mlxtend and efficient-apriori for Apriori.
-2. (Transactional_T10I4D100K.csv)is a transactional database downloaded from PAMI and
-used as a input file for all libraries.
-3. Minimum support values and seperator are also same.
-
-* The performance of the **Apriori algorithm** is shown in the graphical results below:
-1. Comparing the **Patterns Generated** by different Python libraries for the Apriori algorithm:
-
-   <img width="573" alt="Screenshot 2024-04-11 at 13 31 31" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/fd7974bc-ffe2-44dd-82e3-a5306a8a23bd">
-   
-2. Evaluating the **Runtime** of the Apriori algorithm across different Python libraries:
-
-   <img width="567" alt="Screenshot 2024-04-11 at 13 31 20" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d615ae3-dc0d-49ba-a880-4890bb1f11c5">
-
-3. Comparing the **Memory Consumption** of the Apriori algorithm across different Python libraries:
-
-   <img width="570" alt="Screenshot 2024-04-11 at 13 31 08" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d5991ca-51ae-442d-9b5e-2d21bbebfedd">
-
-For more information, we have uploaded the evaluation file in two formats:
-- One **ipynb** file format, please check it here. [Evaluation File ipynb](https://github.com/UdayLab/PAMI/blob/main/notebooks/Evaluation-neverDelete.ipynb) 
-- Two **pdf** file format, check here. [Evaluation File Pdf](https://github.com/UdayLab/PAMI/blob/main/notebooks/evaluation.pdf)
-
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
+ 
 ***
 
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
-***
-
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -445,14 +349,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -550,8 +456,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.11.1/pami.egg-info/PKG-INFO` & `pami-2024.4.9.1/pami.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2024.4.11.1
+Version: 2024.4.9.1
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,14 @@
 Requires-Dist: urllib3
 Requires-Dist: Pillow
 Requires-Dist: numpy
 Requires-Dist: sphinx-rtd-theme
 Requires-Dist: validators
 Requires-Dist: discord.py
 Requires-Dist: networkx
-Requires-Dist: deprecated
 Provides-Extra: gpu
 Requires-Dist: cupy; extra == "gpu"
 Requires-Dist: pycuda; extra == "gpu"
 Provides-Extra: spark
 Requires-Dist: pyspark; extra == "spark"
 Provides-Extra: dev
 Requires-Dist: twine; extra == "dev"
@@ -57,20 +56,15 @@
 [![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
 [![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
 
 [Click here for more information](https://pepy.tech/project/pami)
 
 
-
-
 # Introduction
-
-***
-
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in a wide-spectrum of datasets across multiple computing platforms. Useful links to utilize the services of this library were provided below:
 
 
 1. Youtube tutorial https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ
 
 2. Tutorials (Notebooks) https://github.com/UdayLab/PAMI/tree/main/notebooks
    
@@ -82,64 +76,50 @@
 
 6. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
 7. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
 8. Report issues https://github.com/UdayLab/PAMI/issues
 
-
 # Recent Updates  
 
-***
-
 - Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
-
 # Features
 
-***
-
 - ✅ Well-tested and production-ready
 - 🔋 Highly optimized to our best effort, light-weight, and energy-efficient
 - 👀 Proper code documentation
 - 🍼 Ample examples of using various algorithms at [./notebooks](https://github.com/UdayLab/PAMI/tree/main/notebooks) folder
 - 🤖 Works with AI libraries such as TensorFlow, PyTorch, and sklearn. 
 - ⚡️ Supports Cuda and PySpark 
 - 🖥️ Operating System Independence
 - 🔬 Knowledge discovery in static data and streams
 - 🐎 Snappy
 - 🐻 Ease of use
 
-
-
 # Table of Content
 
-***
-
 - [Maintenance](#Maintenance)
 - [Try your first PAMI program](#try-your-first-PAMI-program)
-- [Evaluation](#evaluation)
 - [Reading Material](#Reading-Material)
+- [Tutorials](#Tutorials)
 - [License](#License)
 - [Documentation](#Documentation)
 - [Background](#Background)
 - [Getting Help](#Getting-Help)
 - [Discussion and Development](#Discussion-and-Development)
 - [Contribution to PAMI](#Contribution-to-PAMI)
-- [Tutorials](#Tutorials)
-
 
 # Maintenance
 
-***
-
   __Installation__
   
   1. Installing basic pami package (recommended)
 
 
          pip install pami
 
@@ -181,19 +161,16 @@
        
 
   __Information__ 
 
 
         pip show pami
 
-
 # *Try your first PAMI program*
 
-***
-
 ```shell
 $ python
 ```
 
 ```python
 # first import pami 
 from PAMI.frequentPattern.basic import FPGrowth as alg
@@ -214,95 +191,21 @@
 Frequent patterns were generated successfully using frequentPatternGrowth algorithm
 Total No of patterns: 4540
 Runtime: 8.749667644500732
 Memory (RSS): 522911744
 Memory (USS): 475353088
 ```
 
-# Evaluation:
-
-***
-
-1. we compared three different Python libraries such as PAMI, mlxtend and efficient-apriori for Apriori.
-2. (Transactional_T10I4D100K.csv)is a transactional database downloaded from PAMI and
-used as a input file for all libraries.
-3. Minimum support values and seperator are also same.
-
-* The performance of the **Apriori algorithm** is shown in the graphical results below:
-1. Comparing the **Patterns Generated** by different Python libraries for the Apriori algorithm:
-
-   <img width="573" alt="Screenshot 2024-04-11 at 13 31 31" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/fd7974bc-ffe2-44dd-82e3-a5306a8a23bd">
-   
-2. Evaluating the **Runtime** of the Apriori algorithm across different Python libraries:
-
-   <img width="567" alt="Screenshot 2024-04-11 at 13 31 20" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d615ae3-dc0d-49ba-a880-4890bb1f11c5">
-
-3. Comparing the **Memory Consumption** of the Apriori algorithm across different Python libraries:
-
-   <img width="570" alt="Screenshot 2024-04-11 at 13 31 08" src="https://github.com/vanithakattumuri/PAMI/assets/134862983/5d5991ca-51ae-442d-9b5e-2d21bbebfedd">
-
-For more information, we have uploaded the evaluation file in two formats:
-- One **ipynb** file format, please check it here. [Evaluation File ipynb](https://github.com/UdayLab/PAMI/blob/main/notebooks/Evaluation-neverDelete.ipynb) 
-- Two **pdf** file format, check here. [Evaluation File Pdf](https://github.com/UdayLab/PAMI/blob/main/notebooks/evaluation.pdf)
-
 # Reading Material
-
-***
-
 For more examples, refer this YouTube link [YouTube](https://www.youtube.com/playlist?list=PLKP768gjVJmDer6MajaLbwtfC9ULVuaCZ)
-
-
-# License
-
+ 
 ***
 
-[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
-
-
-# Documentation
-
-***
-
-The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
-
-
-
-# Background
-
-***
-
-The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
-has been under active development since then.
-
-
-# Getting Help
-
-***
-
-For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
-
-
-# Discussion and Development
-
-***
-
-In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
-
-
-# Contribution to PAMI
-
-***
-
-We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
-
-
 # Tutorials 
 
-***
-
 ### 1. Pattern mining in binary transactional databases
 
 #### 1.1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
@@ -491,14 +394,16 @@
 #### 5.1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                   |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FFI-Miner <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyFrequentPattern/basic/FFIMiner.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
+
+
 #### 5.2. Fuzzy correlated pattern mining: [Sample](https://udaylab.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                       |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | FCP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/fuzzyCorrelatedPattern/basic/FCPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
 
@@ -596,8 +501,28 @@
 ## 11. Mining patterns from Graphs
 
 #### 11.1. Frequent sub-graph mining
 | Basic                                                                                                                                                                                                                                      | topk                                                                                                                                                                                                                                  |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
  | Gspan <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/basic/gspan.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | TKG <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/subgraphMining/topk/tkg.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 
-[Go to Top](#table-of-content)
+# License
+
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
+
+# Documentation
+The official documentation is hosted on [PAMI](https://pami-1.readthedocs.io).
+
+# Background
+The idea and motivation to develop PAMI was from [Kitsuregawa Lab](https://www.tkl.iis.u-tokyo.ac.jp/new/resources?lang=en) at the University of Tokyo. Work on ``PAMI`` started at [University of Aizu](https://u-aizu.ac.jp/en/) in 2020 and
+has been under active development since then.
+
+# Getting Help
+For any queries, the best place to go to is github Issues [GithubIssues](https://github.com/orgs/UdayLab/discussions/categories/q-a).
+
+# Discussion and Development
+In our GitHub repository, the primary platform for discussing development-related matters is the university lab. We encourage our team members and contributors to utilize this platform for a wide range of discussions, including bug reports, feature requests, design decisions, and implementation details.
+
+# Contribution to PAMI
+We invite and encourage all community members to contribute, report bugs, fix bugs, enhance documentation, propose improvements, and share their creative ideas.
+
+[Go to Top](#table-of-contents)
```

### Comparing `pami-2024.4.11.1/pami.egg-info/SOURCES.txt` & `pami-2024.4.9.1/pami.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 PAMI/faultTolerantFrequentPattern/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
 PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
 PAMI/faultTolerantFrequentPattern/basic/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/abstract.py
 PAMI/frequentPattern/__init__.py
 PAMI/frequentPattern/basic/Apriori.py
-PAMI/frequentPattern/basic/AprioriOLD.py
 PAMI/frequentPattern/basic/ECLAT.py
 PAMI/frequentPattern/basic/ECLATDiffset.py
 PAMI/frequentPattern/basic/ECLATbitset.py
 PAMI/frequentPattern/basic/FPGrowth.py
 PAMI/frequentPattern/basic/__init__.py
 PAMI/frequentPattern/basic/abstract.py
 PAMI/frequentPattern/closed/CHARM.py
```

### Comparing `pami-2024.4.11.1/setup.py` & `pami-2024.4.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2024.4.11.1',
+    version='2024.4.9.1',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
@@ -24,15 +24,14 @@
         'urllib3',
         'Pillow',
         'numpy',
         'sphinx-rtd-theme',
         'validators',
         'discord.py',
         'networkx',
-        'deprecated',
     ],
     extras_require={
         'gpu':  ['cupy', 'pycuda'],
         'spark': ['pyspark'],
         'dev': ['twine', 'setuptools', 'build'],
         'all': ['cupy', 'pycuda', 'pyspark', 'twine', 'setuptools', 'build']
     },
@@ -40,8 +39,7 @@
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.5',
 )
-
```

