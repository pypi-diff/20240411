# Comparing `tmp/fine-2.3.5.tar.gz` & `tmp/fine-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fine-2.3.5.tar", last modified: Mon Mar 11 12:14:56 2024, max compression
+gzip compressed data, was "fine-2.3.6.tar", last modified: Thu Apr 11 08:36:59 2024, max compression
```

## Comparing `fine-2.3.5.tar` & `fine-2.3.6.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.447958 fine-2.3.5/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1655 2024-02-23 13:39:25.000000 fine-2.3.5/LICENSE.txt
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)       48 2024-02-23 13:39:25.000000 fine-2.3.5/MANIFEST.in
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12631 2024-03-11 12:14:56.447958 fine-2.3.5/PKG-INFO
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    11555 2024-02-23 13:39:25.000000 fine-2.3.5/README.md
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.427958 fine-2.3.5/fine/
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.427958 fine-2.3.5/fine/IOManagement/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      233 2024-02-23 13:39:25.000000 fine-2.3.5/fine/IOManagement/__init__.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4618 2024-02-23 13:39:25.000000 fine-2.3.5/fine/IOManagement/dictIO.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2088 2024-02-23 13:39:25.000000 fine-2.3.5/fine/IOManagement/exploitOutput.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    44389 2024-03-07 16:30:37.000000 fine-2.3.5/fine/IOManagement/standardIO.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    27777 2024-03-07 16:30:37.000000 fine-2.3.5/fine/IOManagement/utilsIO.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    49003 2024-03-07 16:30:37.000000 fine-2.3.5/fine/IOManagement/xarrayIO.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      453 2024-03-07 16:30:37.000000 fine-2.3.5/fine/__init__.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.427958 fine-2.3.5/fine/aggregations/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      157 2024-02-23 13:39:25.000000 fine-2.3.5/fine/aggregations/__init__.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.437958 fine-2.3.5/fine/aggregations/spatialAggregation/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      218 2024-02-23 13:39:25.000000 fine-2.3.5/fine/aggregations/spatialAggregation/__init__.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    20824 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/spatialAggregation/aggregation.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12152 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/spatialAggregation/grouping.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    19659 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/spatialAggregation/groupingUtils.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15231 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/spatialAggregation/manager.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4709 2024-02-23 13:39:25.000000 fine-2.3.5/fine/aggregations/spatialAggregation/managerUtils.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.437958 fine-2.3.5/fine/aggregations/technologyAggregation/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      154 2024-02-23 13:39:25.000000 fine-2.3.5/fine/aggregations/technologyAggregation/__init__.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    16319 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/technologyAggregation/techAggregation.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5245 2024-03-07 16:30:37.000000 fine-2.3.5/fine/aggregations/technologyAggregation/techAggregationUtils.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)   191078 2024-03-07 16:30:37.000000 fine-2.3.5/fine/component.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    60527 2024-03-07 16:30:37.000000 fine-2.3.5/fine/conversion.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)   110346 2024-03-07 16:30:37.000000 fine-2.3.5/fine/energySystemModel.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.437958 fine-2.3.5/fine/expansionModules/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      156 2024-02-23 13:39:25.000000 fine-2.3.5/fine/expansionModules/__init__.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     7984 2024-02-23 13:39:25.000000 fine-2.3.5/fine/expansionModules/optimizeTSAmultiStage.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    10444 2024-02-23 13:39:25.000000 fine-2.3.5/fine/expansionModules/transformationPath.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    62159 2024-03-07 13:57:16.000000 fine-2.3.5/fine/sourceSink.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    98402 2024-03-07 16:30:37.000000 fine-2.3.5/fine/storage.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.437958 fine-2.3.5/fine/subclasses/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      237 2024-03-07 16:30:37.000000 fine-2.3.5/fine/subclasses/__init__.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    22246 2024-03-07 16:30:37.000000 fine-2.3.5/fine/subclasses/conversionDynamic.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    44560 2024-03-07 16:30:37.000000 fine-2.3.5/fine/subclasses/conversionPartLoad.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    16614 2024-03-07 16:30:37.000000 fine-2.3.5/fine/subclasses/lopf.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    50553 2024-03-07 16:30:37.000000 fine-2.3.5/fine/transmission.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)   109028 2024-03-07 16:30:37.000000 fine-2.3.5/fine/utils.py
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.447958 fine-2.3.5/fine.egg-info/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12631 2024-03-11 12:14:56.000000 fine-2.3.5/fine.egg-info/PKG-INFO
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2204 2024-03-11 12:14:56.000000 fine-2.3.5/fine.egg-info/SOURCES.txt
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)        1 2024-03-11 12:14:56.000000 fine-2.3.5/fine.egg-info/dependency_links.txt
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)        5 2024-03-11 12:14:56.000000 fine-2.3.5/fine.egg-info/top_level.txt
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1890 2024-03-11 09:41:59.000000 fine-2.3.5/pyproject.toml
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      378 2024-02-23 13:39:25.000000 fine-2.3.5/requirements.yml
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)       38 2024-03-11 12:14:56.447958 fine-2.3.5/setup.cfg
-drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-03-11 12:14:56.447958 fine-2.3.5/test/
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3306 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_QPinvest.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1474 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_TSAmultiStage.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    23754 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_balanceLimit.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2399 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_commodityConversionFactors.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    11363 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_commodityConversionFactorsTimeSeries.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3977 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_commodityCostTimeSeries.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    17362 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_conversionPartLoad.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3772 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_conversiondynamic.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      590 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_fixtures.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5335 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_full_load_hours.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5271 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_initTransmission.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     6663 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_leanModel.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1230 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_linkedQuantity.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3228 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_miniSystem.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4809 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_minimumDownTime.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3988 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_minimumPartLoad.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4803 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_minimumUpTime.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      634 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_netPresentValue.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      524 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_operationHeatMap.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1231 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_operationRateMin.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5401 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_rampDownMax.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5393 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_rampUpMax.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3325 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_segmentation.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1239 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_shadowCostOutput.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12335 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_simpleMyopic.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)      270 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_solver.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     9916 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_stochasticOptimization.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15153 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_stock.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     6736 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_storageTimeseriesSetup.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1835 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_updateComponent.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4999 2024-03-07 16:30:37.000000 fine-2.3.5/test/test_utils.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1501 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_warnings.py
--rw-r--r--   0 kknosala  (1000) kknosala  (1000)     7796 2024-02-23 13:39:25.000000 fine-2.3.5/test/test_watersupply.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.279034 fine-2.3.6/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1789 2024-04-11 08:27:35.000000 fine-2.3.6/LICENSE.txt
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)       48 2024-02-23 13:39:25.000000 fine-2.3.6/MANIFEST.in
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15537 2024-04-11 08:36:59.279034 fine-2.3.6/PKG-INFO
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    13641 2024-04-11 08:27:35.000000 fine-2.3.6/README.md
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/IOManagement/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      233 2024-02-23 13:39:25.000000 fine-2.3.6/fine/IOManagement/__init__.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4618 2024-02-23 13:39:25.000000 fine-2.3.6/fine/IOManagement/dictIO.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2088 2024-02-23 13:39:25.000000 fine-2.3.6/fine/IOManagement/exploitOutput.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    44517 2024-04-11 08:27:36.000000 fine-2.3.6/fine/IOManagement/standardIO.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    27777 2024-03-07 16:30:37.000000 fine-2.3.6/fine/IOManagement/utilsIO.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    49003 2024-03-07 16:30:37.000000 fine-2.3.6/fine/IOManagement/xarrayIO.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      453 2024-03-07 16:30:37.000000 fine-2.3.6/fine/__init__.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/aggregations/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      157 2024-02-23 13:39:25.000000 fine-2.3.6/fine/aggregations/__init__.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/aggregations/spatialAggregation/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      218 2024-02-23 13:39:25.000000 fine-2.3.6/fine/aggregations/spatialAggregation/__init__.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    20824 2024-03-07 16:30:37.000000 fine-2.3.6/fine/aggregations/spatialAggregation/aggregation.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12152 2024-03-07 16:30:37.000000 fine-2.3.6/fine/aggregations/spatialAggregation/grouping.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    19659 2024-03-07 16:30:37.000000 fine-2.3.6/fine/aggregations/spatialAggregation/groupingUtils.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15231 2024-03-07 16:30:37.000000 fine-2.3.6/fine/aggregations/spatialAggregation/manager.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4709 2024-02-23 13:39:25.000000 fine-2.3.6/fine/aggregations/spatialAggregation/managerUtils.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/aggregations/technologyAggregation/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      154 2024-02-23 13:39:25.000000 fine-2.3.6/fine/aggregations/technologyAggregation/__init__.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    16319 2024-03-07 16:30:37.000000 fine-2.3.6/fine/aggregations/technologyAggregation/techAggregation.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4926 2024-04-11 08:27:36.000000 fine-2.3.6/fine/aggregations/technologyAggregation/techAggregationUtils.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)   191078 2024-03-07 16:30:37.000000 fine-2.3.6/fine/component.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    60527 2024-03-07 16:30:37.000000 fine-2.3.6/fine/conversion.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)   110346 2024-03-07 16:30:37.000000 fine-2.3.6/fine/energySystemModel.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.259034 fine-2.3.6/fine/expansionModules/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      156 2024-02-23 13:39:25.000000 fine-2.3.6/fine/expansionModules/__init__.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     7984 2024-02-23 13:39:25.000000 fine-2.3.6/fine/expansionModules/optimizeTSAmultiStage.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    10444 2024-02-23 13:39:25.000000 fine-2.3.6/fine/expansionModules/transformationPath.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    62159 2024-03-07 13:57:16.000000 fine-2.3.6/fine/sourceSink.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    98402 2024-03-07 16:30:37.000000 fine-2.3.6/fine/storage.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.269034 fine-2.3.6/fine/subclasses/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      237 2024-03-07 16:30:37.000000 fine-2.3.6/fine/subclasses/__init__.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    22246 2024-03-07 16:30:37.000000 fine-2.3.6/fine/subclasses/conversionDynamic.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    44560 2024-03-07 16:30:37.000000 fine-2.3.6/fine/subclasses/conversionPartLoad.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    16614 2024-03-07 16:30:37.000000 fine-2.3.6/fine/subclasses/lopf.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    50553 2024-03-07 16:30:37.000000 fine-2.3.6/fine/transmission.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)   109028 2024-03-07 16:30:37.000000 fine-2.3.6/fine/utils.py
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.279034 fine-2.3.6/fine.egg-info/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15537 2024-04-11 08:36:59.000000 fine-2.3.6/fine.egg-info/PKG-INFO
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2231 2024-04-11 08:36:59.000000 fine-2.3.6/fine.egg-info/SOURCES.txt
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)        1 2024-04-11 08:36:59.000000 fine-2.3.6/fine.egg-info/dependency_links.txt
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      281 2024-04-11 08:36:59.000000 fine-2.3.6/fine.egg-info/requires.txt
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)        5 2024-04-11 08:36:59.000000 fine-2.3.6/fine.egg-info/top_level.txt
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2382 2024-04-11 08:27:36.000000 fine-2.3.6/pyproject.toml
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      344 2024-04-11 08:27:36.000000 fine-2.3.6/requirements.yml
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)       38 2024-04-11 08:36:59.279034 fine-2.3.6/setup.cfg
+drwxr-xr-x   0 kknosala  (1000) kknosala  (1000)        0 2024-04-11 08:36:59.279034 fine-2.3.6/test/
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3306 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_QPinvest.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1474 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_TSAmultiStage.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    23754 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_balanceLimit.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     2399 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_commodityConversionFactors.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    11363 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_commodityConversionFactorsTimeSeries.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3977 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_commodityCostTimeSeries.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    17362 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_conversionPartLoad.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3772 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_conversiondynamic.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      590 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_fixtures.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5335 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_full_load_hours.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5271 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_initTransmission.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     6663 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_leanModel.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1230 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_linkedQuantity.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3228 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_miniSystem.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4809 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_minimumDownTime.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3988 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_minimumPartLoad.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4803 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_minimumUpTime.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      634 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_netPresentValue.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      524 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_operationHeatMap.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1231 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_operationRateMin.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5401 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_rampDownMax.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     5393 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_rampUpMax.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     3325 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_segmentation.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1239 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_shadowCostOutput.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    12355 2024-04-11 08:27:36.000000 fine-2.3.6/test/test_simpleMyopic.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)      270 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_solver.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     9916 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_stochasticOptimization.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)    15153 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_stock.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     6736 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_storageTimeseriesSetup.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1835 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_updateComponent.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     4999 2024-03-07 16:30:37.000000 fine-2.3.6/test/test_utils.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     1501 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_warnings.py
+-rw-r--r--   0 kknosala  (1000) kknosala  (1000)     7796 2024-02-23 13:39:25.000000 fine-2.3.6/test/test_watersupply.py
```

### Comparing `fine-2.3.5/LICENSE.txt` & `fine-2.3.6/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿MIT License
 
-Copyright (C) 2016-2022 FZJ-IEK-3
+Copyright (C) 2016-2024 FZJ-IEK-3
 
-Active Developers: Theresa Groß, Leander Kotzur, Noah Pflugradt, Julian Belina, Toni Busch, Philipp Dunkel, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Kevin Knosala, Felix Kullmann, Stefan Kraus, Jochen Linßen, Rachel Maier, Peter Markewitz, Lars Nolting, Shruthi Patil, Jan Priesmann, Stanley Risch, Julian Schönau, Bismark Singh, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Christoph Winkler, Michael Zier, Detlef Stolten
+Active Developers: Theresa Groß, Kevin Knosala, Noah Pflugradt, Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, David Franzmann, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Jason Hu, Shitab Ishmam, Sebastian Kebrich, Felix Kullmann, Jochen Linßen, Rachel Maier, Shruthi Patil, Jan Priesmann, Julian Schönau, Maximilian Stargardt, Lovindu Wijesinghe, Christoph Winkler, Detlef Stolten
 
-Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Martin Robinius, Johannes Thürauf, Lara Welder
+Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Leander Kotzur, Stefan Kraus, Peter Markewitz, Lars Nolting,Stanley Risch, Martin Robinius, Bismark Singh, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes Thürauf, Lara Welder, Michael Zier
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fine-2.3.5/PKG-INFO` & `fine-2.3.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fine
-Version: 2.3.5
+Version: 2.3.6
 Summary: Framework for integrated energy systems assessment
 Author-email: Theresa Groß <t.gross@fz-juelich.de>, Kevin Knosala <k.knosala@fz-juelich.de>
 Maintainer-email: Theresa Groß <t.gross@fz-juelich.de>, Kevin Knosala <k.knosala@fz-juelich.de>
 Project-URL: homepage, https://www.fz-juelich.de/de/iek/iek-3/forschung/open-source/fine
 Project-URL: repository, https://github.com/FZJ-IEK3-VSA/FINE
 Project-URL: documentation, https://vsa-fine.readthedocs.io/en/master/
 Keywords: energy assesment,energy system,optimization
@@ -12,183 +12,206 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
+Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: geopandas<1
+Requires-Dist: openpyxl<4
+Requires-Dist: matplotlib<4
+Requires-Dist: xlrd<3
+Requires-Dist: pyomo<7
+Requires-Dist: numpy<2
+Requires-Dist: pandas<3,>=2
+Requires-Dist: scipy<2
+Requires-Dist: scikit-learn<2,>=1.2
+Requires-Dist: xarray<=2024.3
+Requires-Dist: rasterio<2
+Requires-Dist: netcdf4<2
+Requires-Dist: tsam
+Requires-Dist: pwlf<3
+Requires-Dist: psutil<6
+Requires-Dist: gurobi-logtools<4
+Provides-Extra: develop
+Requires-Dist: sphinx<8; extra == "develop"
+Requires-Dist: sphinx_rtd_theme<3; extra == "develop"
+Requires-Dist: myst-parser<3; extra == "develop"
+Requires-Dist: pytest<9; extra == "develop"
+Requires-Dist: pytest-cov<5; extra == "develop"
+Requires-Dist: pytest-xdist<4; extra == "develop"
+Requires-Dist: nbval<1; extra == "develop"
+Requires-Dist: ruff<1; extra == "develop"
+
+<!-- markdownlint-disable line-length no-inline-html -->
+# ETHOS.FINE - Framework for Integrated Energy System Assessment
 
 [![Build Status](https://travis-ci.com/FZJ-IEK3-VSA/FINE.svg?branch=master)](https://travis-ci.com/FZJ-IEK3-VSA/FINE)
 [![Version](https://img.shields.io/pypi/v/FINE.svg)](https://pypi.python.org/pypi/FINE)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/fine.svg)](https://anaconda.org/conda-forge/fine)
 [![Documentation Status](https://readthedocs.org/projects/vsa-fine/badge/?version=latest)](https://vsa-fine.readthedocs.io/en/latest/)
 [![PyPI - License](https://img.shields.io/pypi/l/FINE)](https://github.com/FZJ-IEK3-VSA/FINE/blob/master/LICENSE.txt)
 [![codecov](https://codecov.io/gh/FZJ-IEK3-VSA/FINE/branch/master/graph/badge.svg)](https://codecov.io/gh/FZJ-IEK3-VSA/FINE)
 
-
-<a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/FJZ_IEK-3_logo.svg?raw=True" alt="Forschungszentrum Juelich Logo" width="300px"></a> 
-
-# ETHOS.FINE - Framework for Integrated Energy System Assessment
-
+<a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/FJZ_IEK-3_logo.svg?raw=True" alt="Forschungszentrum Juelich Logo" width="300px"></a>
 
 The ETHOS.FINE python package provides a framework for modeling, optimizing and assessing energy systems. With the provided framework, systems with multiple regions, commodities and time steps can be modeled. Target of the optimization is the minimization of the total annual cost while considering technical and environmental constraints. Besides using the full temporal resolution, an interconnected typical period storage formulation can be applied, that reduces the complexity and computational time of the model.
 
-This readme provides information on the installation of the package. For further information have a look at the [documentation](https://vsa-fine.readthedocs.io/en/latest/).
+This Readme provides information on the installation of the package. For further information have a look at the [documentation](https://vsa-fine.readthedocs.io/en/latest/).
 
 ETHOS.FINE is used for the modelling of a diverse group of optimization problems within the [Energy Transformation PatHway Optimization Suite (ETHOS) at IEK-3](https://www.fz-juelich.de/de/iek/iek-3/leistungen/model-services).  
 
 If you want to use ETHOS.FINE in a published work, please [**kindly cite following publication**](https://www.sciencedirect.com/science/article/pii/S036054421830879X) which gives a description of the first stages of the framework. The python package which provides the time series aggregation module and its corresponding literature can be found [here](https://github.com/FZJ-IEK3-VSA/tsam).
 
-## Content
-<!-- TOC -->
-* [Requirements](#requirements)
-  * [Python package manager](#python-package-manager)
-  * [Mixed Integer Linear Programming (MILP) solver](#mixed-integer-linear-programming-milp-solver)
-* [Installation](#installation)
-  * [Installation via conda-forge](#installation-via-conda-forge)
-  * [Installation from a local folder](#installation-from-a-local-folder)
-  * [Installation for developers](#installation-for-developers)
-* [Installation of an optimization solver](#installation-of-an-optimization-solver)
-  * [Gurobi installation](#gurobi-installation)
-  * [GLPK installation](#glpk-installation)
-  * [CBC](#cbc)
-* [Examples](#examples)
-* [License](#license)
-* [About Us](#about-us-)
-* [Contributions and Users](#contributions-and-users)
-* [Acknowledgement](#acknowledgement)
-<!-- TOC -->
+## Installation from conda-forge
+
+If you would like to run ETHOS.FINE for your analysis we recommend to install it directly from conda-forge into a new Python environment with
 
+```bash
+mamba create --name fine --channel conda-forge fine
+```
 
-## Requirements
+**Note on Mamba vs.Conda:** `mamba` commands can be substitued with `conda`. We highly recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The recommended way to use Mamba on your system is to install the [Miniforge distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In principle, Conda and Mamba are interchangeable. The commands and concepts are the same. The distributions differ in the methodology for determining dependencies when installing Python packages. Mamba relies on a more modern methodology, which (with the same result) leads to very significant time savings during the installation of ETHOS.FINE. Switching to Mamba usually does not lead to any problems, as it is virtually identical to Conda in terms of operation.
 
-### Python package manager
-The installation process uses a Conda-based Python package manager. We highly recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The recommended way to use Mamba on your system is to install the [Miniforge distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In principle, Conda and Mamba are interchangeable. The commands and concepts are the same. The distributions differ in the methodology for determining dependencies when installing Python packages. Mamba relies on a more modern methodology, which (with the same result) leads to very significant time savings during the installation of FINE. Switching to Mamba usually does not lead to any problems, as it is virtually identical to Conda in terms of operation.
+**Note on the solver:** The mamba/conda installation comes with [GLPK](https://www.gnu.org/software/glpk/) [(installation for Windows)](https://sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer Linear Programming (MILP) solver. If you want to solve large problems it is highly recommended to install [GUROBI](http://www.gurobi.com/). See ["Installation of an optimization solver"](#installation-of-an-optimization-solver) for more information.
 
-If you decide to use Conda you have to expect longer installation times for FINE. In this case, we recommend the installation [through our conda-forge package](#installation-via-conda-forge).
+## Installation from pipy
 
-### Mixed Integer Linear Programming (MILP) solver
-The project environment includes [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer Linear Programming (MILP) solver. If you want to solve large problems it is highly recommended to install [GUROBI](http://www.gurobi.com/). See ["Installation of an optimization solver"](#installation-of-an-optimization-solver) for more information.
+The functionality of ETHOS.FINE depends on the following C libraries that need to be installed on your system. If you do not know how to install those, consider installing from conda-forge.
 
-## Installation
+- [GLPK](https://www.gnu.org/software/glpk/)
+- [GDAL](https://gdal.org/index.html)
 
-If you would like to run FINE for your analysis we recommend to install it directly from conda-forge into a new Python environment. Alternatively you can install it from a local folder by using the `requirements.yml` file. If you want to work on the FINE code base choose "Installation for developers". It performs an editable installation of FINE and add some developer tools (e.g. pytest, black) to the environment.
+Create a virtual environment in the ETHOS.FINE folder and activate it
 
-###  Installation via conda-forge
-The simplest way ist to install FINE into a fresh environment from `conda-forge` with:
 ```bash
-mamba create -n fine -c conda-forge fine
+python -m venv .venv
+source .venv/bin/activate
 ```
 
-### Installation from a local folder
-Alternatively you can first clone the content of this repository and perform the installation from there: 
+Install ETHOS.FINE with
 
-1. (Shallow) clone the content of this repository 
-```bash
-git clone --depth 1 https://github.com/FZJ-IEK3-VSA/FINE.git 
-```
-2. Move into the FINE folder with
 ```bash
-cd fine
-```
-3. It is recommended to create a clean environment with conda to use FINE because it requires many dependencies. 
-```bash
-mamba env create -f requirements.yml
-```
-5. Activate the new environment. You should see `(fine)` in front of your command prompt to indicate that you are now in the virtual environment.
-```bash
-mamba activate fine
-```
-6. Install FINE with:
-```bash
-python -m pip install --no-deps .
+python -m pip install fine
 ```
 
-### Installation for developers
-If you want to work on the FINE codebase you need to run. 
-```bash
-git clone https://github.com/FZJ-IEK3-VSA/FINE.git
-```
-to get the whole git history and then
-```bash
-mamba env create -f requirements_dev.yml
-```
-This installs additional dependencies such as `pytest` and installs FINE from the folder in editable mode with `pip -e`. Changes in the folder are then reflected in the package installation.
-Finally, install FINE in editable mode with:
-```bash
-python -m pip install --no-deps --editable .
-```
-Test your installation with the following command in the project root folder:
-```
-pytest
-```
+### Installation of an optimization solver
 
-## Installation of an optimization solver
+ETHOS.FINE requires an MILP solver which can be accessed using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches for the following solvers in this order:
 
-FINE requires an MILP solver which can be accessed using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches for the following solvers in this order:
-- [GUROBI](http://www.gurobi.com/)
-   - Recommended due to better performance but requires license (free academic version available)
-   - Set as standard solver
-- [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
-  - This solver is installed with the FINE environment.
-  - Free version available 
-- [CBC](https://projects.coin-or.org/Cbc)
-  - Free version available
+#### [GUROBI](http://www.gurobi.com/)
+
+This solver is recommended due to better performance but requires license (free academic version available). It is set as the default solver.
 
-### Gurobi installation
 The installation requires the following three components:
+
 - Gurobi Optimizer
-    - In order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) the software you need to create an account and obtain a license.
+  - In order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) the software you need to create an account and obtain a license.
 - Gurobi license
-    - The license needs to be installed according to the instructions in the registration process.
+  - The license needs to be installed according to the instructions in the registration process.
 - Gurobi python api
-    - The python api can be installed according to [this instruction](https://support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-Python-).
+  - The python api can be installed according to [this instruction](https://support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-Python-).
+
+#### [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
+
+This solver is installed with the ETHOS.FINE environment. A complete installation instruction for Windows can be found [here](http://winglpk.sourceforge.net/).
 
-### GLPK installation
-A complete installation instruction for Windows can be found [here](http://winglpk.sourceforge.net/).
+#### [CBC](https://projects.coin-or.org/Cbc)
 
-### CBC
 Installation procedure can be found [here](https://projects.coin-or.org/Cbc).
 
 ## Examples
 
-A number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/master/examples) shows the capabilities of FINE.
+A number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples) shows the capabilities of ETHOS.FINE.
+
+- [00_Tutorial](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/00_Tutorial)
+  - In this application, an energy supply system, consisting of two regions, is modeled and optimized. Recommended as starting point to get to know to ETHOS.FINE.
+- [01_1node_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/01_1node_Energy_System_Workflow)
+  - In this application, a single region energy system is modeled and optimized. The system includes only a few technologies.
+- [02_EnergyLand](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/02_EnergyLand)
+  - In this application, a single region energy system is modeled and optimized. Compared to the previous examples, this example includes a lot more technologies considered in the system.
+- [03_Multi-regional_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/03_Multi-regional_Energy_System_Workflow)
+  - In this application, an energy supply system, consisting of eight regions, is modeled and optimized. The example shows how to model multi-regional energy systems. The example also includes a notebook to get to know the optional performance summary. The summary shows how the optimization performed.
+- [04_Model_Run_from_Excel](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/04_Model_Run_from_Excel)
+  - ETHOS.FINE can also be run by excel. This example shows how to read and run a model using excel files.
+- [05_District_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/05_District_Optimization)
+  - In this application, a small district is modeled and optimized. This example also includes binary decision variables.
+- [06_Water_Supply_System](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/06_Water_Supply_System)
+  - The application cases of ETHOS.FINE are not limited. This application shows how to model the water supply system.
+- [07_NetCDF_to_save_and_set_up_model_instance](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/07_NetCDF_to_save_and_set_up_model_instance)
+  - This example shows how to save the input and optimized results of an energy system Model instance to netCDF files to allow reproducibility.
+- [08_Spatial_and_technology_aggregation](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/08_Spatial_and_technology_aggregation)
+  - These two examples show how to reduce the model complexity. Model regions can be aggregated to reduce the number of regions (spatial aggregation). Input parameters are automatically adapted. Furthermore, technologies can be aggregated to reduce complexity, e.g. reducing the number of different PV components (technology aggregation). Input parameters are automatically adapted.
+- [09_Stochastic_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/9_Stochastic_Optimizatio)
+  - In this application, a stochastic optimization is performed. It is possible to perform the optimization of an energy system model with different input parameter sets to receive a more robust solution.
+- [10_PerfectForesight](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/10_PerfectForesight)
+  - In this application, a transformation pathway of an energy system is modeled and optimized showing how to handle several investment periods with time-dependent assumptions for costs and operation.
+- [11_Partload](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/11_Partload)
+  - In this application, a hydrogen system is modeled and optimized considering partload behavior of the electrolyzer.
+
+## Notes for developers
+
+### Editable install from conda-forge
+
+It is recommended to create a clean environment with conda to use ETHOS.FINE because it requires many dependencies.
+
+```bash
+mamba env create --name fine --file requirements_dev.yml
+mamba activate fine
+```
+
+Install ETHOS.FINE as editable install and without checking the dependencies from pypi with
+
+```bash
+python -m pip install --no-deps --editable .
+```
+
+### Editable install from pypi
+
+If you do not want to use conda-forge consider the steps in section [Installation from pipy](#Installation-from-pipy) and install ETHOS.FINE as editable install and with developer dependencies with
+
+```bash
+python -m pip install --editable .[develop]
+```
 
 ## License
 
 MIT License
 
-Copyright (C) 2016-2023 FZJ-IEK-3
+Copyright (C) 2016-2024 FZJ-IEK-3
 
-Active Developers: Theresa Groß, Kevin Knosala, Noah Pflugradt, Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Shitab Ishmam, Stefan Kraus, Felix Kullmann, Jochen Linßen, Rachel Maier, Peter Markewitz, Lars Nolting, Shruthi Patil, Jan Priesmann, Stanley Risch, Julian Schönau, Bismark Singh, Maximilian Stargardt, Christoph Winkler, Michael Zier, Detlef Stolten
+Active Developers: Theresa Groß, Kevin Knosala, Noah Pflugradt, Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, David Franzmann, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Jason Hu, Shitab Ishmam, Sebastian Kebrich, Felix Kullmann, Jochen Linßen, Rachel Maier, Shruthi Patil, Jan Priesmann, Julian Schönau, Maximilian Stargardt, Lovindu Wijesinghe, Christoph Winkler, Detlef Stolten
 
-Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Leander Kotzur, Martin Robinius, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes Thürauf, Lara Welder
+Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Leander Kotzur, Stefan Kraus, Peter Markewitz, Lars Nolting,Stanley Risch, Martin Robinius, Bismark Singh, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes Thürauf, Lara Welder, Michael Zier
 
 You should have received a copy of the MIT License along with this program.
 If not, see https://opensource.org/licenses/MIT
 
 
 ## About Us 
 
 <a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/iek3-square.png?raw=True" alt="Institute image IEK-3" width="280" align="right" style="margin:0px 10px"/></a>
 
 We are the <a href="https://www.fz-juelich.de/en/iek/iek-3">Institute of Energy and Climate Research - Techno-economic Systems Analysis (IEK-3)</a> belonging to the <a href="https://www.fz-juelich.de/en">Forschungszentrum Jülich</a>. Our interdisciplinary department's research is focusing on energy-related process and systems analyses. Data searches and system simulations are used to determine energy and mass balances, as well as to evaluate performance, emissions and costs of energy systems. The results are used for performing comparative assessment studies between the various systems. Our current priorities include the development of energy strategies, in accordance with the German Federal Government’s greenhouse gas reduction targets, by designing new infrastructures for sustainable and secure energy supply chains and by conducting cost analysis studies for integrating new technologies into future energy market frameworks.
 
-## Contributions and Users
-
-From 2018 to 2022  we developed methods and models for ETHOS.FINE together with the RWTH-Aachen ([Prof. Aaron Praktiknjo](http://www.wiwi.rwth-aachen.de/cms/Wirtschaftswissenschaften/Die-Fakultaet/Institute-und-Lehrstuehle/Professoren/~jgfr/Praktiknjo-Aaron/?allou=1&lidx=1)), the [EDOM Team at FAU](https://www.math.fau.de/wirtschaftsmathematik/) and the [Jülich Supercomputing Centre](http://www.fz-juelich.de/ias/jsc/DE/Home/home_node.html)  within the BMWi funded project [METIS](http://www.metis-platform.net/).
+## Contributions and Support
+Every contributions are welcome:
+- If you have a question, you can start a [Discussion](https://github.com/FZJ-IEK3-VSA/FINE/discussions). You will get a response as soon as possible.
+- If you want to report a bug, please open an [Issue](https://github.com/FZJ-IEK3-VSA/FINE/issues/new). We will then take care of the issue as soon as possible.
+- If you want to contribute with additional features or code improvements, open a [Pull request](https://github.com/FZJ-IEK3-VSA/FINE/pulls).
 
-<p float="left">
-<a href="https://www.rwth-aachen.de/go/id/a/"> <img src="https://upload.wikimedia.org/wikipedia/commons/1/1e/RWTH_Logo_3.svg" width="230" /> </a> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
-<a href="https://www.fau.de/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Friedrich-Alexander-Universit%C3%A4t_Erlangen-N%C3%BCrnberg_logo.svg/2000px-Friedrich-Alexander-Universit%C3%A4t_Erlangen-N%C3%BCrnberg_logo.svg.png" width="230" /> </a>
-</p>
+## Code of Conduct
+Please respect our [code of conduct](CODE_OF_CONDUCT.md).
 
 ## Acknowledgement
+This work was initially supported by the Helmholtz Association under the Joint Initiative ["Energy System 2050   A Contribution of the Research Field Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/). 
+
+The authors also gratefully acknowledge financial support by the Federal Ministry for Economic Affairs and Energy of Germany as part of the project [METIS](http://www.metis-platform.net/) (project number 03ET4064, 2018-2022).
 
-This work was supported by the Helmholtz Association under the Joint Initiative ["Energy System 2050   A Contribution of the Research Field Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/).
+This work was supported by the Helmholtz Association under the program ["Energy System Design"](https://www.helmholtz.de/en/research/research-fields/energy/energy-system-design/).
 
 <p float="left">
 <a href="https://www.helmholtz.de/en/"><img src="https://www.helmholtz.de/fileadmin/user_upload/05_aktuelles/Marke_Design/logos/HG_LOGO_S_ENG_RGB.jpg" alt="Helmholtz Logo" width="200px"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,156 +1,197 @@
-Metadata-Version: 2.1 Name: fine Version: 2.3.5 Summary: Framework for
+Metadata-Version: 2.1 Name: fine Version: 2.3.6 Summary: Framework for
 integrated energy systems assessment Author-email: Theresa GroÃ
 fz-juelich.de>, Kevin Knosala
 fz-juelich.de> Maintainer-email: Theresa GroÃ
 fz-juelich.de>, Kevin Knosala
 fz-juelich.de> Project-URL: homepage, https://www.fz-juelich.de/de/iek/iek-3/
 forschung/open-source/fine Project-URL: repository, https://github.com/FZJ-
 IEK3-VSA/FINE Project-URL: documentation, https://vsa-fine.readthedocs.io/en/
 master/ Keywords: energy assesment,energy system,optimization Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 MIT License Classifier: Natural Language :: English Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
 :: Mathematics Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.txt [![Build Status](https://travis-ci.com/FZJ-IEK3-VSA/
-FINE.svg?branch=master)](https://travis-ci.com/FZJ-IEK3-VSA/FINE) [![Version]
-(https://img.shields.io/pypi/v/FINE.svg)](https://pypi.python.org/pypi/FINE) [!
-[Conda Version](https://img.shields.io/conda/vn/conda-forge/fine.svg)](https://
-anaconda.org/conda-forge/fine) [![Documentation Status](https://
-readthedocs.org/projects/vsa-fine/badge/?version=latest)](https://vsa-
-fine.readthedocs.io/en/latest/) [![PyPI - License](https://img.shields.io/pypi/
-l/FINE)](https://github.com/FZJ-IEK3-VSA/FINE/blob/master/LICENSE.txt) [!
-[codecov](https://codecov.io/gh/FZJ-IEK3-VSA/FINE/branch/master/graph/
-badge.svg)](https://codecov.io/gh/FZJ-IEK3-VSA/FINE) _[_F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_u_e_l_i_c_h
-_L_o_g_o_]# ETHOS.FINE - Framework for Integrated Energy System Assessment The
-ETHOS.FINE python package provides a framework for modeling, optimizing and
-assessing energy systems. With the provided framework, systems with multiple
-regions, commodities and time steps can be modeled. Target of the optimization
-is the minimization of the total annual cost while considering technical and
-environmental constraints. Besides using the full temporal resolution, an
-interconnected typical period storage formulation can be applied, that reduces
-the complexity and computational time of the model. This readme provides
-information on the installation of the package. For further information have a
-look at the [documentation](https://vsa-fine.readthedocs.io/en/latest/).
-ETHOS.FINE is used for the modelling of a diverse group of optimization
-problems within the [Energy Transformation PatHway Optimization Suite (ETHOS)
-at IEK-3](https://www.fz-juelich.de/de/iek/iek-3/leistungen/model-services). If
-you want to use ETHOS.FINE in a published work, please [**kindly cite following
-publication**](https://www.sciencedirect.com/science/article/pii/
-S036054421830879X) which gives a description of the first stages of the
-framework. The python package which provides the time series aggregation module
-and its corresponding literature can be found [here](https://github.com/FZJ-
-IEK3-VSA/tsam). ## Content * [Requirements](#requirements) * [Python package
-manager](#python-package-manager) * [Mixed Integer Linear Programming (MILP)
-solver](#mixed-integer-linear-programming-milp-solver) * [Installation]
-(#installation) * [Installation via conda-forge](#installation-via-conda-forge)
-* [Installation from a local folder](#installation-from-a-local-folder) *
-[Installation for developers](#installation-for-developers) * [Installation of
-an optimization solver](#installation-of-an-optimization-solver) * [Gurobi
-installation](#gurobi-installation) * [GLPK installation](#glpk-installation) *
-[CBC](#cbc) * [Examples](#examples) * [License](#license) * [About Us](#about-
-us-) * [Contributions and Users](#contributions-and-users) * [Acknowledgement]
-(#acknowledgement) ## Requirements ### Python package manager The installation
-process uses a Conda-based Python package manager. We highly recommend using [
-(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The
-recommended way to use Mamba on your system is to install the [Miniforge
-distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer
-installers for Windows, Linux and OS X. In principle, Conda and Mamba are
-interchangeable. The commands and concepts are the same. The distributions
-differ in the methodology for determining dependencies when installing Python
-packages. Mamba relies on a more modern methodology, which (with the same
-result) leads to very significant time savings during the installation of FINE.
-Switching to Mamba usually does not lead to any problems, as it is virtually
-identical to Conda in terms of operation. If you decide to use Conda you have
-to expect longer installation times for FINE. In this case, we recommend the
-installation [through our conda-forge package](#installation-via-conda-forge).
-### Mixed Integer Linear Programming (MILP) solver The project environment
-includes [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
-as Mixed Integer Linear Programming (MILP) solver. If you want to solve large
-problems it is highly recommended to install [GUROBI](http://www.gurobi.com/).
-See ["Installation of an optimization solver"](#installation-of-an-
-optimization-solver) for more information. ## Installation If you would like to
-run FINE for your analysis we recommend to install it directly from conda-forge
-into a new Python environment. Alternatively you can install it from a local
-folder by using the `requirements.yml` file. If you want to work on the FINE
-code base choose "Installation for developers". It performs an editable
-installation of FINE and add some developer tools (e.g. pytest, black) to the
-environment. ### Installation via conda-forge The simplest way ist to install
-FINE into a fresh environment from `conda-forge` with: ```bash mamba create -
-n fine -c conda-forge fine ``` ### Installation from a local folder
-Alternatively you can first clone the content of this repository and perform
-the installation from there: 1. (Shallow) clone the content of this repository
-```bash git clone --depth 1 https://github.com/FZJ-IEK3-VSA/FINE.git ``` 2.
-Move into the FINE folder with ```bash cd fine ``` 3. It is recommended to
-create a clean environment with conda to use FINE because it requires many
-dependencies. ```bash mamba env create -f requirements.yml ``` 5. Activate the
-new environment. You should see `(fine)` in front of your command prompt to
-indicate that you are now in the virtual environment. ```bash mamba activate
-fine ``` 6. Install FINE with: ```bash python -m pip install --no-deps . ```
-### Installation for developers If you want to work on the FINE codebase you
-need to run. ```bash git clone https://github.com/FZJ-IEK3-VSA/FINE.git ``` to
-get the whole git history and then ```bash mamba env create -
-f requirements_dev.yml ``` This installs additional dependencies such as
-`pytest` and installs FINE from the folder in editable mode with `pip -e`.
-Changes in the folder are then reflected in the package installation. Finally,
-install FINE in editable mode with: ```bash python -m pip install --no-deps --
-editable . ``` Test your installation with the following command in the project
-root folder: ``` pytest ``` ## Installation of an optimization solver FINE
-requires an MILP solver which can be accessed using [PYOMO](https://
-pyomo.readthedocs.io/en/stable/index.html). It searches for the following
-solvers in this order: - [GUROBI](http://www.gurobi.com/) - Recommended due to
-better performance but requires license (free academic version available) - Set
-as standard solver - [GLPK](https://sourceforge.net/projects/winglpk/files/
-latest/download) - This solver is installed with the FINE environment. - Free
-version available - [CBC](https://projects.coin-or.org/Cbc) - Free version
-available ### Gurobi installation The installation requires the following three
-components: - Gurobi Optimizer - In order to [download](https://www.gurobi.com/
-downloads/gurobi-optimizer-eula/) the software you need to create an account
-and obtain a license. - Gurobi license - The license needs to be installed
-according to the instructions in the registration process. - Gurobi python api
-- The python api can be installed according to [this instruction](https://
-support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-
-Python-). ### GLPK installation A complete installation instruction for Windows
-can be found [here](http://winglpk.sourceforge.net/). ### CBC Installation
-procedure can be found [here](https://projects.coin-or.org/Cbc). ## Examples A
-number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/master/examples)
-shows the capabilities of FINE. ## License MIT License Copyright (C) 2016-2023
-FZJ-IEK-3 Active Developers: Theresa GroÃ, Kevin Knosala, Noah Pflugradt,
-Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel,
-Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Shitab
-Ishmam, Stefan Kraus, Felix Kullmann, Jochen LinÃen, Rachel Maier, Peter
-Markewitz, Lars Nolting, Shruthi Patil, Jan Priesmann, Stanley Risch, Julian
-SchÃ¶nau, Bismark Singh, Maximilian Stargardt, Christoph Winkler, Michael Zier,
-Detlef Stolten Alumni: Robin Beer, Henrik BÃ¼sing, Dilara Caglayan, Timo
-KannengieÃer, Leander Kotzur, Martin Robinius, Andreas Smolenko, Peter
-Stenzel, Chloi Syranidou, Johannes ThÃ¼rauf, Lara Welder You should have
-received a copy of the MIT License along with this program. If not, see https:/
-/opensource.org/licenses/MIT ## About Us _[_I_n_s_t_i_t_u_t_e_ _i_m_a_g_e_ _I_E_K_-_3_]We are the
-_I_n_s_t_i_t_u_t_e_ _o_f_ _E_n_e_r_g_y_ _a_n_d_ _C_l_i_m_a_t_e_ _R_e_s_e_a_r_c_h_ _-_ _T_e_c_h_n_o_-_e_c_o_n_o_m_i_c_ _S_y_s_t_e_m_s_ _A_n_a_l_y_s_i_s_ 
-_(_I_E_K_-_3_) belonging to the _F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_Ã_¼_l_i_c_h. Our interdisciplinary
-department's research is focusing on energy-related process and systems
-analyses. Data searches and system simulations are used to determine energy and
-mass balances, as well as to evaluate performance, emissions and costs of
-energy systems. The results are used for performing comparative assessment
-studies between the various systems. Our current priorities include the
-development of energy strategies, in accordance with the German Federal
-Governmentâs greenhouse gas reduction targets, by designing new
-infrastructures for sustainable and secure energy supply chains and by
+Modules Requires-Python: <3.13,>=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE.txt Requires-Dist: geopandas<1 Requires-Dist: openpyxl<4
+Requires-Dist: matplotlib<4 Requires-Dist: xlrd<3 Requires-Dist: pyomo<7
+Requires-Dist: numpy<2 Requires-Dist: pandas<3,>=2 Requires-Dist: scipy<2
+Requires-Dist: scikit-learn<2,>=1.2 Requires-Dist: xarray<=2024.3 Requires-
+Dist: rasterio<2 Requires-Dist: netcdf4<2 Requires-Dist: tsam Requires-Dist:
+pwlf<3 Requires-Dist: psutil<6 Requires-Dist: gurobi-logtools<4 Provides-Extra:
+develop Requires-Dist: sphinx<8; extra == "develop" Requires-Dist:
+sphinx_rtd_theme<3; extra == "develop" Requires-Dist: myst-parser<3; extra ==
+"develop" Requires-Dist: pytest<9; extra == "develop" Requires-Dist: pytest-
+cov<5; extra == "develop" Requires-Dist: pytest-xdist<4; extra == "develop"
+Requires-Dist: nbval<1; extra == "develop" Requires-Dist: ruff<1; extra ==
+"develop" # ETHOS.FINE - Framework for Integrated Energy System Assessment [!
+[Build Status](https://travis-ci.com/FZJ-IEK3-VSA/FINE.svg?branch=master)]
+(https://travis-ci.com/FZJ-IEK3-VSA/FINE) [![Version](https://img.shields.io/
+pypi/v/FINE.svg)](https://pypi.python.org/pypi/FINE) [![Conda Version](https://
+img.shields.io/conda/vn/conda-forge/fine.svg)](https://anaconda.org/conda-
+forge/fine) [![Documentation Status](https://readthedocs.org/projects/vsa-fine/
+badge/?version=latest)](https://vsa-fine.readthedocs.io/en/latest/) [![PyPI -
+License](https://img.shields.io/pypi/l/FINE)](https://github.com/FZJ-IEK3-VSA/
+FINE/blob/master/LICENSE.txt) [![codecov](https://codecov.io/gh/FZJ-IEK3-VSA/
+FINE/branch/master/graph/badge.svg)](https://codecov.io/gh/FZJ-IEK3-VSA/FINE)
+_[_F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_u_e_l_i_c_h_ _L_o_g_o_]The ETHOS.FINE python package provides a
+framework for modeling, optimizing and assessing energy systems. With the
+provided framework, systems with multiple regions, commodities and time steps
+can be modeled. Target of the optimization is the minimization of the total
+annual cost while considering technical and environmental constraints. Besides
+using the full temporal resolution, an interconnected typical period storage
+formulation can be applied, that reduces the complexity and computational time
+of the model. This Readme provides information on the installation of the
+package. For further information have a look at the [documentation](https://
+vsa-fine.readthedocs.io/en/latest/). ETHOS.FINE is used for the modelling of a
+diverse group of optimization problems within the [Energy Transformation
+PatHway Optimization Suite (ETHOS) at IEK-3](https://www.fz-juelich.de/de/iek/
+iek-3/leistungen/model-services). If you want to use ETHOS.FINE in a published
+work, please [**kindly cite following publication**](https://
+www.sciencedirect.com/science/article/pii/S036054421830879X) which gives a
+description of the first stages of the framework. The python package which
+provides the time series aggregation module and its corresponding literature
+can be found [here](https://github.com/FZJ-IEK3-VSA/tsam). ## Installation from
+conda-forge If you would like to run ETHOS.FINE for your analysis we recommend
+to install it directly from conda-forge into a new Python environment with
+```bash mamba create --name fine --channel conda-forge fine ``` **Note on Mamba
+vs.Conda:** `mamba` commands can be substitued with `conda`. We highly
+recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/
+) instead of Conda. The recommended way to use Mamba on your system is to
+install the [Miniforge distribution](https://github.com/conda-forge/
+miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In
+principle, Conda and Mamba are interchangeable. The commands and concepts are
+the same. The distributions differ in the methodology for determining
+dependencies when installing Python packages. Mamba relies on a more modern
+methodology, which (with the same result) leads to very significant time
+savings during the installation of ETHOS.FINE. Switching to Mamba usually does
+not lead to any problems, as it is virtually identical to Conda in terms of
+operation. **Note on the solver:** The mamba/conda installation comes with
+[GLPK](https://www.gnu.org/software/glpk/) [(installation for Windows)](https:/
+/sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer
+Linear Programming (MILP) solver. If you want to solve large problems it is
+highly recommended to install [GUROBI](http://www.gurobi.com/). See
+["Installation of an optimization solver"](#installation-of-an-optimization-
+solver) for more information. ## Installation from pipy The functionality of
+ETHOS.FINE depends on the following C libraries that need to be installed on
+your system. If you do not know how to install those, consider installing from
+conda-forge. - [GLPK](https://www.gnu.org/software/glpk/) - [GDAL](https://
+gdal.org/index.html) Create a virtual environment in the ETHOS.FINE folder and
+activate it ```bash python -m venv .venv source .venv/bin/activate ``` Install
+ETHOS.FINE with ```bash python -m pip install fine ``` ### Installation of an
+optimization solver ETHOS.FINE requires an MILP solver which can be accessed
+using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches
+for the following solvers in this order: #### [GUROBI](http://www.gurobi.com/
+) This solver is recommended due to better performance but requires license
+(free academic version available). It is set as the default solver. The
+installation requires the following three components: - Gurobi Optimizer - In
+order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/
+) the software you need to create an account and obtain a license. - Gurobi
+license - The license needs to be installed according to the instructions in
+the registration process. - Gurobi python api - The python api can be installed
+according to [this instruction](https://support.gurobi.com/hc/en-us/articles/
+360044290292-How-do-I-install-Gurobi-for-Python-). #### [GLPK](https://
+sourceforge.net/projects/winglpk/files/latest/download) This solver is
+installed with the ETHOS.FINE environment. A complete installation instruction
+for Windows can be found [here](http://winglpk.sourceforge.net/). #### [CBC]
+(https://projects.coin-or.org/Cbc) Installation procedure can be found [here]
+(https://projects.coin-or.org/Cbc). ## Examples A number of [examples](https://
+github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples) shows the capabilities of
+ETHOS.FINE. - [00_Tutorial](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/00_Tutorial) - In this application, an energy supply system,
+consisting of two regions, is modeled and optimized. Recommended as starting
+point to get to know to ETHOS.FINE. - [01_1node_Energy_System_Workflow](https:/
+/github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/
+01_1node_Energy_System_Workflow) - In this application, a single region energy
+system is modeled and optimized. The system includes only a few technologies. -
+[02_EnergyLand](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/
+02_EnergyLand) - In this application, a single region energy system is modeled
+and optimized. Compared to the previous examples, this example includes a lot
+more technologies considered in the system. - [03_Multi-
+regional_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/
+develop/examples/03_Multi-regional_Energy_System_Workflow) - In this
+application, an energy supply system, consisting of eight regions, is modeled
+and optimized. The example shows how to model multi-regional energy systems.
+The example also includes a notebook to get to know the optional performance
+summary. The summary shows how the optimization performed. -
+[04_Model_Run_from_Excel](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/04_Model_Run_from_Excel) - ETHOS.FINE can also be run by excel. This
+example shows how to read and run a model using excel files. -
+[05_District_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/05_District_Optimization) - In this application, a small district is
+modeled and optimized. This example also includes binary decision variables. -
+[06_Water_Supply_System](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/06_Water_Supply_System) - The application cases of ETHOS.FINE are not
+limited. This application shows how to model the water supply system. -
+[07_NetCDF_to_save_and_set_up_model_instance](https://github.com/FZJ-IEK3-VSA/
+FINE/tree/develop/examples/07_NetCDF_to_save_and_set_up_model_instance) - This
+example shows how to save the input and optimized results of an energy system
+Model instance to netCDF files to allow reproducibility. -
+[08_Spatial_and_technology_aggregation](https://github.com/FZJ-IEK3-VSA/FINE/
+tree/develop/examples/08_Spatial_and_technology_aggregation) - These two
+examples show how to reduce the model complexity. Model regions can be
+aggregated to reduce the number of regions (spatial aggregation). Input
+parameters are automatically adapted. Furthermore, technologies can be
+aggregated to reduce complexity, e.g. reducing the number of different PV
+components (technology aggregation). Input parameters are automatically
+adapted. - [09_Stochastic_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/
+tree/develop/examples/9_Stochastic_Optimizatio) - In this application, a
+stochastic optimization is performed. It is possible to perform the
+optimization of an energy system model with different input parameter sets to
+receive a more robust solution. - [10_PerfectForesight](https://github.com/FZJ-
+IEK3-VSA/FINE/tree/develop/examples/10_PerfectForesight) - In this application,
+a transformation pathway of an energy system is modeled and optimized showing
+how to handle several investment periods with time-dependent assumptions for
+costs and operation. - [11_Partload](https://github.com/FZJ-IEK3-VSA/FINE/tree/
+develop/examples/11_Partload) - In this application, a hydrogen system is
+modeled and optimized considering partload behavior of the electrolyzer. ##
+Notes for developers ### Editable install from conda-forge It is recommended to
+create a clean environment with conda to use ETHOS.FINE because it requires
+many dependencies. ```bash mamba env create --name fine --file
+requirements_dev.yml mamba activate fine ``` Install ETHOS.FINE as editable
+install and without checking the dependencies from pypi with ```bash python -
+m pip install --no-deps --editable . ``` ### Editable install from pypi If you
+do not want to use conda-forge consider the steps in section [Installation from
+pipy](#Installation-from-pipy) and install ETHOS.FINE as editable install and
+with developer dependencies with ```bash python -m pip install --editable .
+[develop] ``` ## License MIT License Copyright (C) 2016-2024 FZJ-IEK-3 Active
+Developers: Theresa GroÃ, Kevin Knosala, Noah Pflugradt, Johannes Behrens,
+Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, David Franzmann,
+Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Jason Hu,
+Shitab Ishmam, Sebastian Kebrich, Felix Kullmann, Jochen LinÃen, Rachel Maier,
+Shruthi Patil, Jan Priesmann, Julian SchÃ¶nau, Maximilian Stargardt, Lovindu
+Wijesinghe, Christoph Winkler, Detlef Stolten Alumni: Robin Beer, Henrik
+BÃ¼sing, Dilara Caglayan, Timo KannengieÃer, Leander Kotzur, Stefan Kraus,
+Peter Markewitz, Lars Nolting,Stanley Risch, Martin Robinius, Bismark Singh,
+Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes ThÃ¼rauf, Lara
+Welder, Michael Zier You should have received a copy of the MIT License along
+with this program. If not, see https://opensource.org/licenses/MIT ## About Us
+_[_I_n_s_t_i_t_u_t_e_ _i_m_a_g_e_ _I_E_K_-_3_]We are the _I_n_s_t_i_t_u_t_e_ _o_f_ _E_n_e_r_g_y_ _a_n_d_ _C_l_i_m_a_t_e_ _R_e_s_e_a_r_c_h_ _-
+_T_e_c_h_n_o_-_e_c_o_n_o_m_i_c_ _S_y_s_t_e_m_s_ _A_n_a_l_y_s_i_s_ _(_I_E_K_-_3_) belonging to the _F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m
+_J_Ã_¼_l_i_c_h. Our interdisciplinary department's research is focusing on energy-
+related process and systems analyses. Data searches and system simulations are
+used to determine energy and mass balances, as well as to evaluate performance,
+emissions and costs of energy systems. The results are used for performing
+comparative assessment studies between the various systems. Our current
+priorities include the development of energy strategies, in accordance with the
+German Federal Governmentâs greenhouse gas reduction targets, by designing
+new infrastructures for sustainable and secure energy supply chains and by
 conducting cost analysis studies for integrating new technologies into future
-energy market frameworks. ## Contributions and Users From 2018 to 2022 we
-developed methods and models for ETHOS.FINE together with the RWTH-Aachen (
-[Prof. Aaron Praktiknjo](http://www.wiwi.rwth-aachen.de/cms/
-Wirtschaftswissenschaften/Die-Fakultaet/Institute-und-Lehrstuehle/Professoren/
-~jgfr/Praktiknjo-Aaron/?allou=1&lidx=1)), the [EDOM Team at FAU](https://
-www.math.fau.de/wirtschaftsmathematik/) and the [JÃ¼lich Supercomputing Centre]
-(http://www.fz-juelich.de/ias/jsc/DE/Home/home_node.html) within the BMWi
-funded project [METIS](http://www.metis-platform.net/).
-_[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_1_/_1_e_/_R_W_T_H___L_o_g_o___3_._s_v_g_]         
- _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_7_/_7_0_/_F_r_i_e_d_r_i_c_h_-
-_A_l_e_x_a_n_d_e_r_-_U_n_i_v_e_r_s_i_t_%_C_3_%_A_4_t___E_r_l_a_n_g_e_n_-_N_%_C_3_%_B_C_r_n_b_e_r_g___l_o_g_o_._s_v_g_/_2_0_0_0_p_x_-_F_r_i_e_d_r_i_c_h_-
-_A_l_e_x_a_n_d_e_r_-_U_n_i_v_e_r_s_i_t_%_C_3_%_A_4_t___E_r_l_a_n_g_e_n_-_N_%_C_3_%_B_C_r_n_b_e_r_g___l_o_g_o_._s_v_g_._p_n_g_]
-## Acknowledgement This work was supported by the Helmholtz Association under
-the Joint Initiative ["Energy System 2050 A Contribution of the Research Field
-Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/).
+energy market frameworks. ## Contributions and Support Every contributions are
+welcome: - If you have a question, you can start a [Discussion](https://
+github.com/FZJ-IEK3-VSA/FINE/discussions). You will get a response as soon as
+possible. - If you want to report a bug, please open an [Issue](https://
+github.com/FZJ-IEK3-VSA/FINE/issues/new). We will then take care of the issue
+as soon as possible. - If you want to contribute with additional features or
+code improvements, open a [Pull request](https://github.com/FZJ-IEK3-VSA/FINE/
+pulls). ## Code of Conduct Please respect our [code of conduct]
+(CODE_OF_CONDUCT.md). ## Acknowledgement This work was initially supported by
+the Helmholtz Association under the Joint Initiative ["Energy System 2050 A
+Contribution of the Research Field Energy"](https://www.helmholtz.de/en/
+research/energy/energy_system_2050/). The authors also gratefully acknowledge
+financial support by the Federal Ministry for Economic Affairs and Energy of
+Germany as part of the project [METIS](http://www.metis-platform.net/) (project
+number 03ET4064, 2018-2022). This work was supported by the Helmholtz
+Association under the program ["Energy System Design"](https://
+www.helmholtz.de/en/research/research-fields/energy/energy-system-design/).
 _[_H_e_l_m_h_o_l_t_z_ _L_o_g_o_]
```

### Comparing `fine-2.3.5/README.md` & `fine-2.3.6/fine.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,217 @@
+Metadata-Version: 2.1
+Name: fine
+Version: 2.3.6
+Summary: Framework for integrated energy systems assessment
+Author-email: Theresa Groß <t.gross@fz-juelich.de>, Kevin Knosala <k.knosala@fz-juelich.de>
+Maintainer-email: Theresa Groß <t.gross@fz-juelich.de>, Kevin Knosala <k.knosala@fz-juelich.de>
+Project-URL: homepage, https://www.fz-juelich.de/de/iek/iek-3/forschung/open-source/fine
+Project-URL: repository, https://github.com/FZJ-IEK3-VSA/FINE
+Project-URL: documentation, https://vsa-fine.readthedocs.io/en/master/
+Keywords: energy assesment,energy system,optimization
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: <3.13,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: geopandas<1
+Requires-Dist: openpyxl<4
+Requires-Dist: matplotlib<4
+Requires-Dist: xlrd<3
+Requires-Dist: pyomo<7
+Requires-Dist: numpy<2
+Requires-Dist: pandas<3,>=2
+Requires-Dist: scipy<2
+Requires-Dist: scikit-learn<2,>=1.2
+Requires-Dist: xarray<=2024.3
+Requires-Dist: rasterio<2
+Requires-Dist: netcdf4<2
+Requires-Dist: tsam
+Requires-Dist: pwlf<3
+Requires-Dist: psutil<6
+Requires-Dist: gurobi-logtools<4
+Provides-Extra: develop
+Requires-Dist: sphinx<8; extra == "develop"
+Requires-Dist: sphinx_rtd_theme<3; extra == "develop"
+Requires-Dist: myst-parser<3; extra == "develop"
+Requires-Dist: pytest<9; extra == "develop"
+Requires-Dist: pytest-cov<5; extra == "develop"
+Requires-Dist: pytest-xdist<4; extra == "develop"
+Requires-Dist: nbval<1; extra == "develop"
+Requires-Dist: ruff<1; extra == "develop"
+
+<!-- markdownlint-disable line-length no-inline-html -->
+# ETHOS.FINE - Framework for Integrated Energy System Assessment
+
 [![Build Status](https://travis-ci.com/FZJ-IEK3-VSA/FINE.svg?branch=master)](https://travis-ci.com/FZJ-IEK3-VSA/FINE)
 [![Version](https://img.shields.io/pypi/v/FINE.svg)](https://pypi.python.org/pypi/FINE)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/fine.svg)](https://anaconda.org/conda-forge/fine)
 [![Documentation Status](https://readthedocs.org/projects/vsa-fine/badge/?version=latest)](https://vsa-fine.readthedocs.io/en/latest/)
 [![PyPI - License](https://img.shields.io/pypi/l/FINE)](https://github.com/FZJ-IEK3-VSA/FINE/blob/master/LICENSE.txt)
 [![codecov](https://codecov.io/gh/FZJ-IEK3-VSA/FINE/branch/master/graph/badge.svg)](https://codecov.io/gh/FZJ-IEK3-VSA/FINE)
 
-
-<a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/FJZ_IEK-3_logo.svg?raw=True" alt="Forschungszentrum Juelich Logo" width="300px"></a> 
-
-# ETHOS.FINE - Framework for Integrated Energy System Assessment
-
+<a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/FJZ_IEK-3_logo.svg?raw=True" alt="Forschungszentrum Juelich Logo" width="300px"></a>
 
 The ETHOS.FINE python package provides a framework for modeling, optimizing and assessing energy systems. With the provided framework, systems with multiple regions, commodities and time steps can be modeled. Target of the optimization is the minimization of the total annual cost while considering technical and environmental constraints. Besides using the full temporal resolution, an interconnected typical period storage formulation can be applied, that reduces the complexity and computational time of the model.
 
-This readme provides information on the installation of the package. For further information have a look at the [documentation](https://vsa-fine.readthedocs.io/en/latest/).
+This Readme provides information on the installation of the package. For further information have a look at the [documentation](https://vsa-fine.readthedocs.io/en/latest/).
 
 ETHOS.FINE is used for the modelling of a diverse group of optimization problems within the [Energy Transformation PatHway Optimization Suite (ETHOS) at IEK-3](https://www.fz-juelich.de/de/iek/iek-3/leistungen/model-services).  
 
 If you want to use ETHOS.FINE in a published work, please [**kindly cite following publication**](https://www.sciencedirect.com/science/article/pii/S036054421830879X) which gives a description of the first stages of the framework. The python package which provides the time series aggregation module and its corresponding literature can be found [here](https://github.com/FZJ-IEK3-VSA/tsam).
 
-## Content
-<!-- TOC -->
-* [Requirements](#requirements)
-  * [Python package manager](#python-package-manager)
-  * [Mixed Integer Linear Programming (MILP) solver](#mixed-integer-linear-programming-milp-solver)
-* [Installation](#installation)
-  * [Installation via conda-forge](#installation-via-conda-forge)
-  * [Installation from a local folder](#installation-from-a-local-folder)
-  * [Installation for developers](#installation-for-developers)
-* [Installation of an optimization solver](#installation-of-an-optimization-solver)
-  * [Gurobi installation](#gurobi-installation)
-  * [GLPK installation](#glpk-installation)
-  * [CBC](#cbc)
-* [Examples](#examples)
-* [License](#license)
-* [About Us](#about-us-)
-* [Contributions and Users](#contributions-and-users)
-* [Acknowledgement](#acknowledgement)
-<!-- TOC -->
+## Installation from conda-forge
 
+If you would like to run ETHOS.FINE for your analysis we recommend to install it directly from conda-forge into a new Python environment with
 
-## Requirements
+```bash
+mamba create --name fine --channel conda-forge fine
+```
 
-### Python package manager
-The installation process uses a Conda-based Python package manager. We highly recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The recommended way to use Mamba on your system is to install the [Miniforge distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In principle, Conda and Mamba are interchangeable. The commands and concepts are the same. The distributions differ in the methodology for determining dependencies when installing Python packages. Mamba relies on a more modern methodology, which (with the same result) leads to very significant time savings during the installation of FINE. Switching to Mamba usually does not lead to any problems, as it is virtually identical to Conda in terms of operation.
+**Note on Mamba vs.Conda:** `mamba` commands can be substitued with `conda`. We highly recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The recommended way to use Mamba on your system is to install the [Miniforge distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In principle, Conda and Mamba are interchangeable. The commands and concepts are the same. The distributions differ in the methodology for determining dependencies when installing Python packages. Mamba relies on a more modern methodology, which (with the same result) leads to very significant time savings during the installation of ETHOS.FINE. Switching to Mamba usually does not lead to any problems, as it is virtually identical to Conda in terms of operation.
 
-If you decide to use Conda you have to expect longer installation times for FINE. In this case, we recommend the installation [through our conda-forge package](#installation-via-conda-forge).
+**Note on the solver:** The mamba/conda installation comes with [GLPK](https://www.gnu.org/software/glpk/) [(installation for Windows)](https://sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer Linear Programming (MILP) solver. If you want to solve large problems it is highly recommended to install [GUROBI](http://www.gurobi.com/). See ["Installation of an optimization solver"](#installation-of-an-optimization-solver) for more information.
 
-### Mixed Integer Linear Programming (MILP) solver
-The project environment includes [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer Linear Programming (MILP) solver. If you want to solve large problems it is highly recommended to install [GUROBI](http://www.gurobi.com/). See ["Installation of an optimization solver"](#installation-of-an-optimization-solver) for more information.
+## Installation from pipy
 
-## Installation
+The functionality of ETHOS.FINE depends on the following C libraries that need to be installed on your system. If you do not know how to install those, consider installing from conda-forge.
 
-If you would like to run FINE for your analysis we recommend to install it directly from conda-forge into a new Python environment. Alternatively you can install it from a local folder by using the `requirements.yml` file. If you want to work on the FINE code base choose "Installation for developers". It performs an editable installation of FINE and add some developer tools (e.g. pytest, black) to the environment.
+- [GLPK](https://www.gnu.org/software/glpk/)
+- [GDAL](https://gdal.org/index.html)
+
+Create a virtual environment in the ETHOS.FINE folder and activate it
 
-###  Installation via conda-forge
-The simplest way ist to install FINE into a fresh environment from `conda-forge` with:
 ```bash
-mamba create -n fine -c conda-forge fine
+python -m venv .venv
+source .venv/bin/activate
 ```
 
-### Installation from a local folder
-Alternatively you can first clone the content of this repository and perform the installation from there: 
+Install ETHOS.FINE with
 
-1. (Shallow) clone the content of this repository 
-```bash
-git clone --depth 1 https://github.com/FZJ-IEK3-VSA/FINE.git 
-```
-2. Move into the FINE folder with
-```bash
-cd fine
-```
-3. It is recommended to create a clean environment with conda to use FINE because it requires many dependencies. 
 ```bash
-mamba env create -f requirements.yml
-```
-5. Activate the new environment. You should see `(fine)` in front of your command prompt to indicate that you are now in the virtual environment.
-```bash
-mamba activate fine
-```
-6. Install FINE with:
-```bash
-python -m pip install --no-deps .
+python -m pip install fine
 ```
 
-### Installation for developers
-If you want to work on the FINE codebase you need to run. 
-```bash
-git clone https://github.com/FZJ-IEK3-VSA/FINE.git
-```
-to get the whole git history and then
-```bash
-mamba env create -f requirements_dev.yml
-```
-This installs additional dependencies such as `pytest` and installs FINE from the folder in editable mode with `pip -e`. Changes in the folder are then reflected in the package installation.
-Finally, install FINE in editable mode with:
-```bash
-python -m pip install --no-deps --editable .
-```
-Test your installation with the following command in the project root folder:
-```
-pytest
-```
+### Installation of an optimization solver
+
+ETHOS.FINE requires an MILP solver which can be accessed using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches for the following solvers in this order:
 
-## Installation of an optimization solver
+#### [GUROBI](http://www.gurobi.com/)
 
-FINE requires an MILP solver which can be accessed using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches for the following solvers in this order:
-- [GUROBI](http://www.gurobi.com/)
-   - Recommended due to better performance but requires license (free academic version available)
-   - Set as standard solver
-- [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
-  - This solver is installed with the FINE environment.
-  - Free version available 
-- [CBC](https://projects.coin-or.org/Cbc)
-  - Free version available
+This solver is recommended due to better performance but requires license (free academic version available). It is set as the default solver.
 
-### Gurobi installation
 The installation requires the following three components:
+
 - Gurobi Optimizer
-    - In order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) the software you need to create an account and obtain a license.
+  - In order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/) the software you need to create an account and obtain a license.
 - Gurobi license
-    - The license needs to be installed according to the instructions in the registration process.
+  - The license needs to be installed according to the instructions in the registration process.
 - Gurobi python api
-    - The python api can be installed according to [this instruction](https://support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-Python-).
+  - The python api can be installed according to [this instruction](https://support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-Python-).
+
+#### [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
 
-### GLPK installation
-A complete installation instruction for Windows can be found [here](http://winglpk.sourceforge.net/).
+This solver is installed with the ETHOS.FINE environment. A complete installation instruction for Windows can be found [here](http://winglpk.sourceforge.net/).
+
+#### [CBC](https://projects.coin-or.org/Cbc)
 
-### CBC
 Installation procedure can be found [here](https://projects.coin-or.org/Cbc).
 
 ## Examples
 
-A number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/master/examples) shows the capabilities of FINE.
+A number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples) shows the capabilities of ETHOS.FINE.
+
+- [00_Tutorial](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/00_Tutorial)
+  - In this application, an energy supply system, consisting of two regions, is modeled and optimized. Recommended as starting point to get to know to ETHOS.FINE.
+- [01_1node_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/01_1node_Energy_System_Workflow)
+  - In this application, a single region energy system is modeled and optimized. The system includes only a few technologies.
+- [02_EnergyLand](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/02_EnergyLand)
+  - In this application, a single region energy system is modeled and optimized. Compared to the previous examples, this example includes a lot more technologies considered in the system.
+- [03_Multi-regional_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/03_Multi-regional_Energy_System_Workflow)
+  - In this application, an energy supply system, consisting of eight regions, is modeled and optimized. The example shows how to model multi-regional energy systems. The example also includes a notebook to get to know the optional performance summary. The summary shows how the optimization performed.
+- [04_Model_Run_from_Excel](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/04_Model_Run_from_Excel)
+  - ETHOS.FINE can also be run by excel. This example shows how to read and run a model using excel files.
+- [05_District_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/05_District_Optimization)
+  - In this application, a small district is modeled and optimized. This example also includes binary decision variables.
+- [06_Water_Supply_System](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/06_Water_Supply_System)
+  - The application cases of ETHOS.FINE are not limited. This application shows how to model the water supply system.
+- [07_NetCDF_to_save_and_set_up_model_instance](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/07_NetCDF_to_save_and_set_up_model_instance)
+  - This example shows how to save the input and optimized results of an energy system Model instance to netCDF files to allow reproducibility.
+- [08_Spatial_and_technology_aggregation](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/08_Spatial_and_technology_aggregation)
+  - These two examples show how to reduce the model complexity. Model regions can be aggregated to reduce the number of regions (spatial aggregation). Input parameters are automatically adapted. Furthermore, technologies can be aggregated to reduce complexity, e.g. reducing the number of different PV components (technology aggregation). Input parameters are automatically adapted.
+- [09_Stochastic_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/9_Stochastic_Optimizatio)
+  - In this application, a stochastic optimization is performed. It is possible to perform the optimization of an energy system model with different input parameter sets to receive a more robust solution.
+- [10_PerfectForesight](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/10_PerfectForesight)
+  - In this application, a transformation pathway of an energy system is modeled and optimized showing how to handle several investment periods with time-dependent assumptions for costs and operation.
+- [11_Partload](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/11_Partload)
+  - In this application, a hydrogen system is modeled and optimized considering partload behavior of the electrolyzer.
+
+## Notes for developers
+
+### Editable install from conda-forge
+
+It is recommended to create a clean environment with conda to use ETHOS.FINE because it requires many dependencies.
+
+```bash
+mamba env create --name fine --file requirements_dev.yml
+mamba activate fine
+```
+
+Install ETHOS.FINE as editable install and without checking the dependencies from pypi with
+
+```bash
+python -m pip install --no-deps --editable .
+```
+
+### Editable install from pypi
+
+If you do not want to use conda-forge consider the steps in section [Installation from pipy](#Installation-from-pipy) and install ETHOS.FINE as editable install and with developer dependencies with
+
+```bash
+python -m pip install --editable .[develop]
+```
 
 ## License
 
 MIT License
 
-Copyright (C) 2016-2023 FZJ-IEK-3
+Copyright (C) 2016-2024 FZJ-IEK-3
 
-Active Developers: Theresa Groß, Kevin Knosala, Noah Pflugradt, Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Shitab Ishmam, Stefan Kraus, Felix Kullmann, Jochen Linßen, Rachel Maier, Peter Markewitz, Lars Nolting, Shruthi Patil, Jan Priesmann, Stanley Risch, Julian Schönau, Bismark Singh, Maximilian Stargardt, Christoph Winkler, Michael Zier, Detlef Stolten
+Active Developers: Theresa Groß, Kevin Knosala, Noah Pflugradt, Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, David Franzmann, Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Jason Hu, Shitab Ishmam, Sebastian Kebrich, Felix Kullmann, Jochen Linßen, Rachel Maier, Shruthi Patil, Jan Priesmann, Julian Schönau, Maximilian Stargardt, Lovindu Wijesinghe, Christoph Winkler, Detlef Stolten
 
-Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Leander Kotzur, Martin Robinius, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes Thürauf, Lara Welder
+Alumni: Robin Beer, Henrik Büsing, Dilara Caglayan, Timo Kannengießer, Leander Kotzur, Stefan Kraus, Peter Markewitz, Lars Nolting,Stanley Risch, Martin Robinius, Bismark Singh, Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes Thürauf, Lara Welder, Michael Zier
 
 You should have received a copy of the MIT License along with this program.
 If not, see https://opensource.org/licenses/MIT
 
 
 ## About Us 
 
 <a href="https://www.fz-juelich.de/en/iek/iek-3"><img src="https://github.com/FZJ-IEK3-VSA/README_assets/blob/main/iek3-square.png?raw=True" alt="Institute image IEK-3" width="280" align="right" style="margin:0px 10px"/></a>
 
 We are the <a href="https://www.fz-juelich.de/en/iek/iek-3">Institute of Energy and Climate Research - Techno-economic Systems Analysis (IEK-3)</a> belonging to the <a href="https://www.fz-juelich.de/en">Forschungszentrum Jülich</a>. Our interdisciplinary department's research is focusing on energy-related process and systems analyses. Data searches and system simulations are used to determine energy and mass balances, as well as to evaluate performance, emissions and costs of energy systems. The results are used for performing comparative assessment studies between the various systems. Our current priorities include the development of energy strategies, in accordance with the German Federal Government’s greenhouse gas reduction targets, by designing new infrastructures for sustainable and secure energy supply chains and by conducting cost analysis studies for integrating new technologies into future energy market frameworks.
 
-## Contributions and Users
-
-From 2018 to 2022  we developed methods and models for ETHOS.FINE together with the RWTH-Aachen ([Prof. Aaron Praktiknjo](http://www.wiwi.rwth-aachen.de/cms/Wirtschaftswissenschaften/Die-Fakultaet/Institute-und-Lehrstuehle/Professoren/~jgfr/Praktiknjo-Aaron/?allou=1&lidx=1)), the [EDOM Team at FAU](https://www.math.fau.de/wirtschaftsmathematik/) and the [Jülich Supercomputing Centre](http://www.fz-juelich.de/ias/jsc/DE/Home/home_node.html)  within the BMWi funded project [METIS](http://www.metis-platform.net/).
+## Contributions and Support
+Every contributions are welcome:
+- If you have a question, you can start a [Discussion](https://github.com/FZJ-IEK3-VSA/FINE/discussions). You will get a response as soon as possible.
+- If you want to report a bug, please open an [Issue](https://github.com/FZJ-IEK3-VSA/FINE/issues/new). We will then take care of the issue as soon as possible.
+- If you want to contribute with additional features or code improvements, open a [Pull request](https://github.com/FZJ-IEK3-VSA/FINE/pulls).
 
-<p float="left">
-<a href="https://www.rwth-aachen.de/go/id/a/"> <img src="https://upload.wikimedia.org/wikipedia/commons/1/1e/RWTH_Logo_3.svg" width="230" /> </a> &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;
-<a href="https://www.fau.de/"> <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/70/Friedrich-Alexander-Universit%C3%A4t_Erlangen-N%C3%BCrnberg_logo.svg/2000px-Friedrich-Alexander-Universit%C3%A4t_Erlangen-N%C3%BCrnberg_logo.svg.png" width="230" /> </a>
-</p>
+## Code of Conduct
+Please respect our [code of conduct](CODE_OF_CONDUCT.md).
 
 ## Acknowledgement
+This work was initially supported by the Helmholtz Association under the Joint Initiative ["Energy System 2050   A Contribution of the Research Field Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/). 
+
+The authors also gratefully acknowledge financial support by the Federal Ministry for Economic Affairs and Energy of Germany as part of the project [METIS](http://www.metis-platform.net/) (project number 03ET4064, 2018-2022).
 
-This work was supported by the Helmholtz Association under the Joint Initiative ["Energy System 2050   A Contribution of the Research Field Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/).
+This work was supported by the Helmholtz Association under the program ["Energy System Design"](https://www.helmholtz.de/en/research/research-fields/energy/energy-system-design/).
 
 <p float="left">
 <a href="https://www.helmholtz.de/en/"><img src="https://www.helmholtz.de/fileadmin/user_upload/05_aktuelles/Marke_Design/logos/HG_LOGO_S_ENG_RGB.jpg" alt="Helmholtz Logo" width="200px"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,141 +1,197 @@
-[![Build Status](https://travis-ci.com/FZJ-IEK3-VSA/FINE.svg?branch=master)]
+Metadata-Version: 2.1 Name: fine Version: 2.3.6 Summary: Framework for
+integrated energy systems assessment Author-email: Theresa GroÃ
+fz-juelich.de>, Kevin Knosala
+fz-juelich.de> Maintainer-email: Theresa GroÃ
+fz-juelich.de>, Kevin Knosala
+fz-juelich.de> Project-URL: homepage, https://www.fz-juelich.de/de/iek/iek-3/
+forschung/open-source/fine Project-URL: repository, https://github.com/FZJ-
+IEK3-VSA/FINE Project-URL: documentation, https://vsa-fine.readthedocs.io/en/
+master/ Keywords: energy assesment,energy system,optimization Classifier:
+Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
+MIT License Classifier: Natural Language :: English Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering
+:: Mathematics Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Python: <3.13,>=3.10 Description-Content-Type: text/markdown
+License-File: LICENSE.txt Requires-Dist: geopandas<1 Requires-Dist: openpyxl<4
+Requires-Dist: matplotlib<4 Requires-Dist: xlrd<3 Requires-Dist: pyomo<7
+Requires-Dist: numpy<2 Requires-Dist: pandas<3,>=2 Requires-Dist: scipy<2
+Requires-Dist: scikit-learn<2,>=1.2 Requires-Dist: xarray<=2024.3 Requires-
+Dist: rasterio<2 Requires-Dist: netcdf4<2 Requires-Dist: tsam Requires-Dist:
+pwlf<3 Requires-Dist: psutil<6 Requires-Dist: gurobi-logtools<4 Provides-Extra:
+develop Requires-Dist: sphinx<8; extra == "develop" Requires-Dist:
+sphinx_rtd_theme<3; extra == "develop" Requires-Dist: myst-parser<3; extra ==
+"develop" Requires-Dist: pytest<9; extra == "develop" Requires-Dist: pytest-
+cov<5; extra == "develop" Requires-Dist: pytest-xdist<4; extra == "develop"
+Requires-Dist: nbval<1; extra == "develop" Requires-Dist: ruff<1; extra ==
+"develop" # ETHOS.FINE - Framework for Integrated Energy System Assessment [!
+[Build Status](https://travis-ci.com/FZJ-IEK3-VSA/FINE.svg?branch=master)]
 (https://travis-ci.com/FZJ-IEK3-VSA/FINE) [![Version](https://img.shields.io/
 pypi/v/FINE.svg)](https://pypi.python.org/pypi/FINE) [![Conda Version](https://
 img.shields.io/conda/vn/conda-forge/fine.svg)](https://anaconda.org/conda-
 forge/fine) [![Documentation Status](https://readthedocs.org/projects/vsa-fine/
 badge/?version=latest)](https://vsa-fine.readthedocs.io/en/latest/) [![PyPI -
 License](https://img.shields.io/pypi/l/FINE)](https://github.com/FZJ-IEK3-VSA/
 FINE/blob/master/LICENSE.txt) [![codecov](https://codecov.io/gh/FZJ-IEK3-VSA/
 FINE/branch/master/graph/badge.svg)](https://codecov.io/gh/FZJ-IEK3-VSA/FINE)
-_[_F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_u_e_l_i_c_h_ _L_o_g_o_]# ETHOS.FINE - Framework for Integrated Energy
-System Assessment The ETHOS.FINE python package provides a framework for
-modeling, optimizing and assessing energy systems. With the provided framework,
-systems with multiple regions, commodities and time steps can be modeled.
-Target of the optimization is the minimization of the total annual cost while
-considering technical and environmental constraints. Besides using the full
-temporal resolution, an interconnected typical period storage formulation can
-be applied, that reduces the complexity and computational time of the model.
-This readme provides information on the installation of the package. For
-further information have a look at the [documentation](https://vsa-
-fine.readthedocs.io/en/latest/). ETHOS.FINE is used for the modelling of a
+_[_F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_u_e_l_i_c_h_ _L_o_g_o_]The ETHOS.FINE python package provides a
+framework for modeling, optimizing and assessing energy systems. With the
+provided framework, systems with multiple regions, commodities and time steps
+can be modeled. Target of the optimization is the minimization of the total
+annual cost while considering technical and environmental constraints. Besides
+using the full temporal resolution, an interconnected typical period storage
+formulation can be applied, that reduces the complexity and computational time
+of the model. This Readme provides information on the installation of the
+package. For further information have a look at the [documentation](https://
+vsa-fine.readthedocs.io/en/latest/). ETHOS.FINE is used for the modelling of a
 diverse group of optimization problems within the [Energy Transformation
 PatHway Optimization Suite (ETHOS) at IEK-3](https://www.fz-juelich.de/de/iek/
 iek-3/leistungen/model-services). If you want to use ETHOS.FINE in a published
 work, please [**kindly cite following publication**](https://
 www.sciencedirect.com/science/article/pii/S036054421830879X) which gives a
 description of the first stages of the framework. The python package which
 provides the time series aggregation module and its corresponding literature
-can be found [here](https://github.com/FZJ-IEK3-VSA/tsam). ## Content *
-[Requirements](#requirements) * [Python package manager](#python-package-
-manager) * [Mixed Integer Linear Programming (MILP) solver](#mixed-integer-
-linear-programming-milp-solver) * [Installation](#installation) * [Installation
-via conda-forge](#installation-via-conda-forge) * [Installation from a local
-folder](#installation-from-a-local-folder) * [Installation for developers]
-(#installation-for-developers) * [Installation of an optimization solver]
-(#installation-of-an-optimization-solver) * [Gurobi installation](#gurobi-
-installation) * [GLPK installation](#glpk-installation) * [CBC](#cbc) *
-[Examples](#examples) * [License](#license) * [About Us](#about-us-) *
-[Contributions and Users](#contributions-and-users) * [Acknowledgement]
-(#acknowledgement) ## Requirements ### Python package manager The installation
-process uses a Conda-based Python package manager. We highly recommend using [
-(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/) instead of Conda. The
-recommended way to use Mamba on your system is to install the [Miniforge
-distribution](https://github.com/conda-forge/miniforge#miniforge3). They offer
-installers for Windows, Linux and OS X. In principle, Conda and Mamba are
-interchangeable. The commands and concepts are the same. The distributions
-differ in the methodology for determining dependencies when installing Python
-packages. Mamba relies on a more modern methodology, which (with the same
-result) leads to very significant time savings during the installation of FINE.
-Switching to Mamba usually does not lead to any problems, as it is virtually
-identical to Conda in terms of operation. If you decide to use Conda you have
-to expect longer installation times for FINE. In this case, we recommend the
-installation [through our conda-forge package](#installation-via-conda-forge).
-### Mixed Integer Linear Programming (MILP) solver The project environment
-includes [GLPK](https://sourceforge.net/projects/winglpk/files/latest/download)
-as Mixed Integer Linear Programming (MILP) solver. If you want to solve large
-problems it is highly recommended to install [GUROBI](http://www.gurobi.com/).
-See ["Installation of an optimization solver"](#installation-of-an-
-optimization-solver) for more information. ## Installation If you would like to
-run FINE for your analysis we recommend to install it directly from conda-forge
-into a new Python environment. Alternatively you can install it from a local
-folder by using the `requirements.yml` file. If you want to work on the FINE
-code base choose "Installation for developers". It performs an editable
-installation of FINE and add some developer tools (e.g. pytest, black) to the
-environment. ### Installation via conda-forge The simplest way ist to install
-FINE into a fresh environment from `conda-forge` with: ```bash mamba create -
-n fine -c conda-forge fine ``` ### Installation from a local folder
-Alternatively you can first clone the content of this repository and perform
-the installation from there: 1. (Shallow) clone the content of this repository
-```bash git clone --depth 1 https://github.com/FZJ-IEK3-VSA/FINE.git ``` 2.
-Move into the FINE folder with ```bash cd fine ``` 3. It is recommended to
-create a clean environment with conda to use FINE because it requires many
-dependencies. ```bash mamba env create -f requirements.yml ``` 5. Activate the
-new environment. You should see `(fine)` in front of your command prompt to
-indicate that you are now in the virtual environment. ```bash mamba activate
-fine ``` 6. Install FINE with: ```bash python -m pip install --no-deps . ```
-### Installation for developers If you want to work on the FINE codebase you
-need to run. ```bash git clone https://github.com/FZJ-IEK3-VSA/FINE.git ``` to
-get the whole git history and then ```bash mamba env create -
-f requirements_dev.yml ``` This installs additional dependencies such as
-`pytest` and installs FINE from the folder in editable mode with `pip -e`.
-Changes in the folder are then reflected in the package installation. Finally,
-install FINE in editable mode with: ```bash python -m pip install --no-deps --
-editable . ``` Test your installation with the following command in the project
-root folder: ``` pytest ``` ## Installation of an optimization solver FINE
-requires an MILP solver which can be accessed using [PYOMO](https://
-pyomo.readthedocs.io/en/stable/index.html). It searches for the following
-solvers in this order: - [GUROBI](http://www.gurobi.com/) - Recommended due to
-better performance but requires license (free academic version available) - Set
-as standard solver - [GLPK](https://sourceforge.net/projects/winglpk/files/
-latest/download) - This solver is installed with the FINE environment. - Free
-version available - [CBC](https://projects.coin-or.org/Cbc) - Free version
-available ### Gurobi installation The installation requires the following three
-components: - Gurobi Optimizer - In order to [download](https://www.gurobi.com/
-downloads/gurobi-optimizer-eula/) the software you need to create an account
-and obtain a license. - Gurobi license - The license needs to be installed
-according to the instructions in the registration process. - Gurobi python api
-- The python api can be installed according to [this instruction](https://
-support.gurobi.com/hc/en-us/articles/360044290292-How-do-I-install-Gurobi-for-
-Python-). ### GLPK installation A complete installation instruction for Windows
-can be found [here](http://winglpk.sourceforge.net/). ### CBC Installation
-procedure can be found [here](https://projects.coin-or.org/Cbc). ## Examples A
-number of [examples](https://github.com/FZJ-IEK3-VSA/FINE/tree/master/examples)
-shows the capabilities of FINE. ## License MIT License Copyright (C) 2016-2023
-FZJ-IEK-3 Active Developers: Theresa GroÃ, Kevin Knosala, Noah Pflugradt,
-Johannes Behrens, Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel,
-Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Shitab
-Ishmam, Stefan Kraus, Felix Kullmann, Jochen LinÃen, Rachel Maier, Peter
-Markewitz, Lars Nolting, Shruthi Patil, Jan Priesmann, Stanley Risch, Julian
-SchÃ¶nau, Bismark Singh, Maximilian Stargardt, Christoph Winkler, Michael Zier,
-Detlef Stolten Alumni: Robin Beer, Henrik BÃ¼sing, Dilara Caglayan, Timo
-KannengieÃer, Leander Kotzur, Martin Robinius, Andreas Smolenko, Peter
-Stenzel, Chloi Syranidou, Johannes ThÃ¼rauf, Lara Welder You should have
-received a copy of the MIT License along with this program. If not, see https:/
-/opensource.org/licenses/MIT ## About Us _[_I_n_s_t_i_t_u_t_e_ _i_m_a_g_e_ _I_E_K_-_3_]We are the
-_I_n_s_t_i_t_u_t_e_ _o_f_ _E_n_e_r_g_y_ _a_n_d_ _C_l_i_m_a_t_e_ _R_e_s_e_a_r_c_h_ _-_ _T_e_c_h_n_o_-_e_c_o_n_o_m_i_c_ _S_y_s_t_e_m_s_ _A_n_a_l_y_s_i_s_ 
-_(_I_E_K_-_3_) belonging to the _F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m_ _J_Ã_¼_l_i_c_h. Our interdisciplinary
-department's research is focusing on energy-related process and systems
-analyses. Data searches and system simulations are used to determine energy and
-mass balances, as well as to evaluate performance, emissions and costs of
-energy systems. The results are used for performing comparative assessment
-studies between the various systems. Our current priorities include the
-development of energy strategies, in accordance with the German Federal
-Governmentâs greenhouse gas reduction targets, by designing new
-infrastructures for sustainable and secure energy supply chains and by
+can be found [here](https://github.com/FZJ-IEK3-VSA/tsam). ## Installation from
+conda-forge If you would like to run ETHOS.FINE for your analysis we recommend
+to install it directly from conda-forge into a new Python environment with
+```bash mamba create --name fine --channel conda-forge fine ``` **Note on Mamba
+vs.Conda:** `mamba` commands can be substitued with `conda`. We highly
+recommend using [(Micro-)Mamba](https://mamba.readthedocs.io/en/latest/
+) instead of Conda. The recommended way to use Mamba on your system is to
+install the [Miniforge distribution](https://github.com/conda-forge/
+miniforge#miniforge3). They offer installers for Windows, Linux and OS X. In
+principle, Conda and Mamba are interchangeable. The commands and concepts are
+the same. The distributions differ in the methodology for determining
+dependencies when installing Python packages. Mamba relies on a more modern
+methodology, which (with the same result) leads to very significant time
+savings during the installation of ETHOS.FINE. Switching to Mamba usually does
+not lead to any problems, as it is virtually identical to Conda in terms of
+operation. **Note on the solver:** The mamba/conda installation comes with
+[GLPK](https://www.gnu.org/software/glpk/) [(installation for Windows)](https:/
+/sourceforge.net/projects/winglpk/files/latest/download) as Mixed Integer
+Linear Programming (MILP) solver. If you want to solve large problems it is
+highly recommended to install [GUROBI](http://www.gurobi.com/). See
+["Installation of an optimization solver"](#installation-of-an-optimization-
+solver) for more information. ## Installation from pipy The functionality of
+ETHOS.FINE depends on the following C libraries that need to be installed on
+your system. If you do not know how to install those, consider installing from
+conda-forge. - [GLPK](https://www.gnu.org/software/glpk/) - [GDAL](https://
+gdal.org/index.html) Create a virtual environment in the ETHOS.FINE folder and
+activate it ```bash python -m venv .venv source .venv/bin/activate ``` Install
+ETHOS.FINE with ```bash python -m pip install fine ``` ### Installation of an
+optimization solver ETHOS.FINE requires an MILP solver which can be accessed
+using [PYOMO](https://pyomo.readthedocs.io/en/stable/index.html). It searches
+for the following solvers in this order: #### [GUROBI](http://www.gurobi.com/
+) This solver is recommended due to better performance but requires license
+(free academic version available). It is set as the default solver. The
+installation requires the following three components: - Gurobi Optimizer - In
+order to [download](https://www.gurobi.com/downloads/gurobi-optimizer-eula/
+) the software you need to create an account and obtain a license. - Gurobi
+license - The license needs to be installed according to the instructions in
+the registration process. - Gurobi python api - The python api can be installed
+according to [this instruction](https://support.gurobi.com/hc/en-us/articles/
+360044290292-How-do-I-install-Gurobi-for-Python-). #### [GLPK](https://
+sourceforge.net/projects/winglpk/files/latest/download) This solver is
+installed with the ETHOS.FINE environment. A complete installation instruction
+for Windows can be found [here](http://winglpk.sourceforge.net/). #### [CBC]
+(https://projects.coin-or.org/Cbc) Installation procedure can be found [here]
+(https://projects.coin-or.org/Cbc). ## Examples A number of [examples](https://
+github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples) shows the capabilities of
+ETHOS.FINE. - [00_Tutorial](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/00_Tutorial) - In this application, an energy supply system,
+consisting of two regions, is modeled and optimized. Recommended as starting
+point to get to know to ETHOS.FINE. - [01_1node_Energy_System_Workflow](https:/
+/github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/
+01_1node_Energy_System_Workflow) - In this application, a single region energy
+system is modeled and optimized. The system includes only a few technologies. -
+[02_EnergyLand](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/examples/
+02_EnergyLand) - In this application, a single region energy system is modeled
+and optimized. Compared to the previous examples, this example includes a lot
+more technologies considered in the system. - [03_Multi-
+regional_Energy_System_Workflow](https://github.com/FZJ-IEK3-VSA/FINE/tree/
+develop/examples/03_Multi-regional_Energy_System_Workflow) - In this
+application, an energy supply system, consisting of eight regions, is modeled
+and optimized. The example shows how to model multi-regional energy systems.
+The example also includes a notebook to get to know the optional performance
+summary. The summary shows how the optimization performed. -
+[04_Model_Run_from_Excel](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/04_Model_Run_from_Excel) - ETHOS.FINE can also be run by excel. This
+example shows how to read and run a model using excel files. -
+[05_District_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/05_District_Optimization) - In this application, a small district is
+modeled and optimized. This example also includes binary decision variables. -
+[06_Water_Supply_System](https://github.com/FZJ-IEK3-VSA/FINE/tree/develop/
+examples/06_Water_Supply_System) - The application cases of ETHOS.FINE are not
+limited. This application shows how to model the water supply system. -
+[07_NetCDF_to_save_and_set_up_model_instance](https://github.com/FZJ-IEK3-VSA/
+FINE/tree/develop/examples/07_NetCDF_to_save_and_set_up_model_instance) - This
+example shows how to save the input and optimized results of an energy system
+Model instance to netCDF files to allow reproducibility. -
+[08_Spatial_and_technology_aggregation](https://github.com/FZJ-IEK3-VSA/FINE/
+tree/develop/examples/08_Spatial_and_technology_aggregation) - These two
+examples show how to reduce the model complexity. Model regions can be
+aggregated to reduce the number of regions (spatial aggregation). Input
+parameters are automatically adapted. Furthermore, technologies can be
+aggregated to reduce complexity, e.g. reducing the number of different PV
+components (technology aggregation). Input parameters are automatically
+adapted. - [09_Stochastic_Optimization](https://github.com/FZJ-IEK3-VSA/FINE/
+tree/develop/examples/9_Stochastic_Optimizatio) - In this application, a
+stochastic optimization is performed. It is possible to perform the
+optimization of an energy system model with different input parameter sets to
+receive a more robust solution. - [10_PerfectForesight](https://github.com/FZJ-
+IEK3-VSA/FINE/tree/develop/examples/10_PerfectForesight) - In this application,
+a transformation pathway of an energy system is modeled and optimized showing
+how to handle several investment periods with time-dependent assumptions for
+costs and operation. - [11_Partload](https://github.com/FZJ-IEK3-VSA/FINE/tree/
+develop/examples/11_Partload) - In this application, a hydrogen system is
+modeled and optimized considering partload behavior of the electrolyzer. ##
+Notes for developers ### Editable install from conda-forge It is recommended to
+create a clean environment with conda to use ETHOS.FINE because it requires
+many dependencies. ```bash mamba env create --name fine --file
+requirements_dev.yml mamba activate fine ``` Install ETHOS.FINE as editable
+install and without checking the dependencies from pypi with ```bash python -
+m pip install --no-deps --editable . ``` ### Editable install from pypi If you
+do not want to use conda-forge consider the steps in section [Installation from
+pipy](#Installation-from-pipy) and install ETHOS.FINE as editable install and
+with developer dependencies with ```bash python -m pip install --editable .
+[develop] ``` ## License MIT License Copyright (C) 2016-2024 FZJ-IEK-3 Active
+Developers: Theresa GroÃ, Kevin Knosala, Noah Pflugradt, Johannes Behrens,
+Julian Belina, Arne Burdack, Toni Busch, Philipp Dunkel, David Franzmann,
+Patrick Freitag, Thomas Grube, Heidi Heinrichs, Maximilian Hoffmann, Jason Hu,
+Shitab Ishmam, Sebastian Kebrich, Felix Kullmann, Jochen LinÃen, Rachel Maier,
+Shruthi Patil, Jan Priesmann, Julian SchÃ¶nau, Maximilian Stargardt, Lovindu
+Wijesinghe, Christoph Winkler, Detlef Stolten Alumni: Robin Beer, Henrik
+BÃ¼sing, Dilara Caglayan, Timo KannengieÃer, Leander Kotzur, Stefan Kraus,
+Peter Markewitz, Lars Nolting,Stanley Risch, Martin Robinius, Bismark Singh,
+Andreas Smolenko, Peter Stenzel, Chloi Syranidou, Johannes ThÃ¼rauf, Lara
+Welder, Michael Zier You should have received a copy of the MIT License along
+with this program. If not, see https://opensource.org/licenses/MIT ## About Us
+_[_I_n_s_t_i_t_u_t_e_ _i_m_a_g_e_ _I_E_K_-_3_]We are the _I_n_s_t_i_t_u_t_e_ _o_f_ _E_n_e_r_g_y_ _a_n_d_ _C_l_i_m_a_t_e_ _R_e_s_e_a_r_c_h_ _-
+_T_e_c_h_n_o_-_e_c_o_n_o_m_i_c_ _S_y_s_t_e_m_s_ _A_n_a_l_y_s_i_s_ _(_I_E_K_-_3_) belonging to the _F_o_r_s_c_h_u_n_g_s_z_e_n_t_r_u_m
+_J_Ã_¼_l_i_c_h. Our interdisciplinary department's research is focusing on energy-
+related process and systems analyses. Data searches and system simulations are
+used to determine energy and mass balances, as well as to evaluate performance,
+emissions and costs of energy systems. The results are used for performing
+comparative assessment studies between the various systems. Our current
+priorities include the development of energy strategies, in accordance with the
+German Federal Governmentâs greenhouse gas reduction targets, by designing
+new infrastructures for sustainable and secure energy supply chains and by
 conducting cost analysis studies for integrating new technologies into future
-energy market frameworks. ## Contributions and Users From 2018 to 2022 we
-developed methods and models for ETHOS.FINE together with the RWTH-Aachen (
-[Prof. Aaron Praktiknjo](http://www.wiwi.rwth-aachen.de/cms/
-Wirtschaftswissenschaften/Die-Fakultaet/Institute-und-Lehrstuehle/Professoren/
-~jgfr/Praktiknjo-Aaron/?allou=1&lidx=1)), the [EDOM Team at FAU](https://
-www.math.fau.de/wirtschaftsmathematik/) and the [JÃ¼lich Supercomputing Centre]
-(http://www.fz-juelich.de/ias/jsc/DE/Home/home_node.html) within the BMWi
-funded project [METIS](http://www.metis-platform.net/).
-_[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_1_/_1_e_/_R_W_T_H___L_o_g_o___3_._s_v_g_]         
- _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_7_/_7_0_/_F_r_i_e_d_r_i_c_h_-
-_A_l_e_x_a_n_d_e_r_-_U_n_i_v_e_r_s_i_t_%_C_3_%_A_4_t___E_r_l_a_n_g_e_n_-_N_%_C_3_%_B_C_r_n_b_e_r_g___l_o_g_o_._s_v_g_/_2_0_0_0_p_x_-_F_r_i_e_d_r_i_c_h_-
-_A_l_e_x_a_n_d_e_r_-_U_n_i_v_e_r_s_i_t_%_C_3_%_A_4_t___E_r_l_a_n_g_e_n_-_N_%_C_3_%_B_C_r_n_b_e_r_g___l_o_g_o_._s_v_g_._p_n_g_]
-## Acknowledgement This work was supported by the Helmholtz Association under
-the Joint Initiative ["Energy System 2050 A Contribution of the Research Field
-Energy"](https://www.helmholtz.de/en/research/energy/energy_system_2050/).
+energy market frameworks. ## Contributions and Support Every contributions are
+welcome: - If you have a question, you can start a [Discussion](https://
+github.com/FZJ-IEK3-VSA/FINE/discussions). You will get a response as soon as
+possible. - If you want to report a bug, please open an [Issue](https://
+github.com/FZJ-IEK3-VSA/FINE/issues/new). We will then take care of the issue
+as soon as possible. - If you want to contribute with additional features or
+code improvements, open a [Pull request](https://github.com/FZJ-IEK3-VSA/FINE/
+pulls). ## Code of Conduct Please respect our [code of conduct]
+(CODE_OF_CONDUCT.md). ## Acknowledgement This work was initially supported by
+the Helmholtz Association under the Joint Initiative ["Energy System 2050 A
+Contribution of the Research Field Energy"](https://www.helmholtz.de/en/
+research/energy/energy_system_2050/). The authors also gratefully acknowledge
+financial support by the Federal Ministry for Economic Affairs and Energy of
+Germany as part of the project [METIS](http://www.metis-platform.net/) (project
+number 03ET4064, 2018-2022). This work was supported by the Helmholtz
+Association under the program ["Energy System Design"](https://
+www.helmholtz.de/en/research/research-fields/energy/energy-system-design/).
 _[_H_e_l_m_h_o_l_t_z_ _L_o_g_o_]
```

### Comparing `fine-2.3.5/fine/IOManagement/dictIO.py` & `fine-2.3.6/fine/IOManagement/dictIO.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/IOManagement/exploitOutput.py` & `fine-2.3.6/fine/IOManagement/exploitOutput.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/IOManagement/standardIO.py` & `fine-2.3.6/fine/IOManagement/standardIO.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,17 @@
         .squeeze("columns")
         .dropna(axis="index", how="all")
     )
     esMData = esMData.apply(
         lambda v: ast.literal_eval(v) if isinstance(v, str) and v[0] == "{" else v
     )
 
+    if not hasattr(inspect, "getargspec"):
+        inspect.getargspec = inspect.getfullargspec
+
     kw = inspect.getargspec(fn.EnergySystemModel.__init__).args
     esM = fn.EnergySystemModel(**esMData[esMData.index.isin(kw)])
 
     for comp in esMData["componentClasses"]:
         data = pd.read_excel(file, sheet_name=comp).dropna(axis="index", how="all")
         dataKeys = set(data["name"].values)
         if comp + "LocSpecs" in file.sheet_names:
@@ -239,15 +242,17 @@
             if dataTS.isnull().any().any():
                 raise ValueError("NaN values in " + comp + "TimeSeries data detected.")
 
         for key, row in data.iterrows():
             temp = row.dropna()
             temp = temp.drop(temp[temp == "None"].index)
             temp = temp.apply(
-                lambda v: ast.literal_eval(v) if isinstance(v, str) and v[0] == "{" else v
+                lambda v: ast.literal_eval(v)
+                if isinstance(v, str) and v[0] == "{"
+                else v
             )
 
             if comp + "LocSpecs" in file.sheet_names:
                 dataLoc_ = dataLoc[dataLoc.index.get_level_values(0) == temp["name"]]
                 for ix in dataLoc_.index.get_level_values(1).unique():
                     temp[ix] = dataLoc.loc[(temp["name"], ix)].squeeze()
```

### Comparing `fine-2.3.5/fine/IOManagement/utilsIO.py` & `fine-2.3.6/fine/IOManagement/utilsIO.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/IOManagement/xarrayIO.py` & `fine-2.3.6/fine/IOManagement/xarrayIO.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/spatialAggregation/aggregation.py` & `fine-2.3.6/fine/aggregations/spatialAggregation/aggregation.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/spatialAggregation/grouping.py` & `fine-2.3.6/fine/aggregations/spatialAggregation/grouping.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/spatialAggregation/groupingUtils.py` & `fine-2.3.6/fine/aggregations/spatialAggregation/groupingUtils.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/spatialAggregation/manager.py` & `fine-2.3.6/fine/aggregations/spatialAggregation/manager.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/spatialAggregation/managerUtils.py` & `fine-2.3.6/fine/aggregations/spatialAggregation/managerUtils.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/technologyAggregation/techAggregation.py` & `fine-2.3.6/fine/aggregations/technologyAggregation/techAggregation.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/aggregations/technologyAggregation/techAggregationUtils.py` & `fine-2.3.6/fine/aggregations/technologyAggregation/techAggregationUtils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 """
 Functions to assist technology aggregation algorithm.
 """
 
-import warnings
 import os
 import numpy as np
 from affine import Affine
 import xarray as xr
-
-try:
-    from rasterio import features
-except ImportError:
-    warnings.warn(
-        "The package rasterio is not installed. Spatial aggregation cannot be used without it."
-    )
-
-try:
-    import geopandas as gpd
-except ImportError:
-    warnings.warn(
-        "The package geopandas is not installed. Spatial aggregation cannot be used without it."
-    )
+from rasterio import features
+import geopandas as gpd
 
 
 def rasterize_geometry(geometry, coords, latitude="y", longitude="x"):
     """
     Given a geometry and geolocations, it masks the geolocations
     such that all the geolocations within the geometry are indicated
     by a 1 and rest are NAs.
```

### Comparing `fine-2.3.5/fine/component.py` & `fine-2.3.6/fine/component.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/conversion.py` & `fine-2.3.6/fine/conversion.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/energySystemModel.py` & `fine-2.3.6/fine/energySystemModel.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/expansionModules/optimizeTSAmultiStage.py` & `fine-2.3.6/fine/expansionModules/optimizeTSAmultiStage.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/expansionModules/transformationPath.py` & `fine-2.3.6/fine/expansionModules/transformationPath.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/sourceSink.py` & `fine-2.3.6/fine/sourceSink.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/storage.py` & `fine-2.3.6/fine/storage.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/subclasses/conversionDynamic.py` & `fine-2.3.6/fine/subclasses/conversionDynamic.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/subclasses/conversionPartLoad.py` & `fine-2.3.6/fine/subclasses/conversionPartLoad.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/subclasses/lopf.py` & `fine-2.3.6/fine/subclasses/lopf.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/transmission.py` & `fine-2.3.6/fine/transmission.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine/utils.py` & `fine-2.3.6/fine/utils.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/fine.egg-info/SOURCES.txt` & `fine-2.3.6/fine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 fine/sourceSink.py
 fine/storage.py
 fine/transmission.py
 fine/utils.py
 fine.egg-info/PKG-INFO
 fine.egg-info/SOURCES.txt
 fine.egg-info/dependency_links.txt
+fine.egg-info/requires.txt
 fine.egg-info/top_level.txt
 fine/IOManagement/__init__.py
 fine/IOManagement/dictIO.py
 fine/IOManagement/exploitOutput.py
 fine/IOManagement/standardIO.py
 fine/IOManagement/utilsIO.py
 fine/IOManagement/xarrayIO.py
```

### Comparing `fine-2.3.5/pyproject.toml` & `fine-2.3.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "fine"
-version = "2.3.5"
+version = "2.3.6"
 description = "Framework for integrated energy systems assessment"
 readme = "README.md"
 authors = [
     { name = "Theresa Groß", email = "t.gross@fz-juelich.de" },
     { name = "Kevin Knosala", email = "k.knosala@fz-juelich.de" },
 ]
 maintainers = [
@@ -25,16 +25,46 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ["energy assesment", "energy system", "optimization"]
-dependencies = []
-requires-python = ">=3.10"
+dependencies = [
+    "geopandas<1",
+    "openpyxl<4",
+    "matplotlib<4",
+    "xlrd<3",
+    "pyomo<7",
+    "numpy<2",
+    "pandas>=2,<3",
+    "scipy<2",
+    "scikit-learn>=1.2,<2",
+    "xarray<=2024.3",
+    "rasterio<2",
+    "netcdf4<2",
+    "tsam",
+    "pwlf<3",
+    "psutil<6",
+    "gurobi-logtools<4",
+]
+
+requires-python = ">=3.10,<3.13"
+
+[project.optional-dependencies]
+develop = [
+    "sphinx<8",
+    "sphinx_rtd_theme<3",
+    "myst-parser<3",
+    "pytest<9",
+    "pytest-cov<5",
+    "pytest-xdist<4",
+    "nbval<1",
+    "ruff<1",
+]
 
 #Configureation options
 # https://docs.pytest.org/en/7.1.x/reference/reference.html#configuration-options
 [tool.pytest.ini_options]
 testpaths = ["test"]
 console_output_style = "progress"
 # How to configure Filterwarning:
@@ -51,9 +81,9 @@
 documentation = "https://vsa-fine.readthedocs.io/en/master/"
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 
 [tool.ruff.lint]
 ignore = [
-    "F403",  # ‘from module import *’ used; unable to detect undefined names
+    "F403", # ‘from module import *’ used; unable to detect undefined names
 ]
```

### Comparing `fine-2.3.5/test/test_QPinvest.py` & `fine-2.3.6/test/test_QPinvest.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_TSAmultiStage.py` & `fine-2.3.6/test/test_TSAmultiStage.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_balanceLimit.py` & `fine-2.3.6/test/test_balanceLimit.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_commodityConversionFactors.py` & `fine-2.3.6/test/test_commodityConversionFactors.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_commodityConversionFactorsTimeSeries.py` & `fine-2.3.6/test/test_commodityConversionFactorsTimeSeries.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_commodityCostTimeSeries.py` & `fine-2.3.6/test/test_commodityCostTimeSeries.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_conversionPartLoad.py` & `fine-2.3.6/test/test_conversionPartLoad.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_conversiondynamic.py` & `fine-2.3.6/test/test_conversiondynamic.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_fixtures.py` & `fine-2.3.6/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_full_load_hours.py` & `fine-2.3.6/test/test_full_load_hours.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_initTransmission.py` & `fine-2.3.6/test/test_initTransmission.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_leanModel.py` & `fine-2.3.6/test/test_leanModel.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_linkedQuantity.py` & `fine-2.3.6/test/test_linkedQuantity.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_miniSystem.py` & `fine-2.3.6/test/test_miniSystem.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_minimumDownTime.py` & `fine-2.3.6/test/test_minimumDownTime.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_minimumPartLoad.py` & `fine-2.3.6/test/test_minimumPartLoad.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_minimumUpTime.py` & `fine-2.3.6/test/test_minimumUpTime.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_netPresentValue.py` & `fine-2.3.6/test/test_netPresentValue.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_operationHeatMap.py` & `fine-2.3.6/test/test_operationHeatMap.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_operationRateMin.py` & `fine-2.3.6/test/test_operationRateMin.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_rampDownMax.py` & `fine-2.3.6/test/test_rampDownMax.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_rampUpMax.py` & `fine-2.3.6/test/test_rampUpMax.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_segmentation.py` & `fine-2.3.6/test/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_shadowCostOutput.py` & `fine-2.3.6/test/test_shadowCostOutput.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_simpleMyopic.py` & `fine-2.3.6/test/test_simpleMyopic.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 np.random.seed(
     42
 )  # Sets a "seed" to produce the same random input data in each model run
 
 
+@pytest.mark.skip()
 def test_CO2ReductionTargets():
     locations = {"regionN", "regionS"}
     commodityUnitDict = {
         "electricity": r"GW$_{el}$",
         "naturalGas": r"GW$_{CH_{4},LHV}$",
         "CO2": r"Mio. t$_{CO_2}$/h",
     }
```

### Comparing `fine-2.3.5/test/test_stochasticOptimization.py` & `fine-2.3.6/test/test_stochasticOptimization.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_stock.py` & `fine-2.3.6/test/test_stock.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_storageTimeseriesSetup.py` & `fine-2.3.6/test/test_storageTimeseriesSetup.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_updateComponent.py` & `fine-2.3.6/test/test_updateComponent.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_utils.py` & `fine-2.3.6/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_warnings.py` & `fine-2.3.6/test/test_warnings.py`

 * *Files identical despite different names*

### Comparing `fine-2.3.5/test/test_watersupply.py` & `fine-2.3.6/test/test_watersupply.py`

 * *Files identical despite different names*

