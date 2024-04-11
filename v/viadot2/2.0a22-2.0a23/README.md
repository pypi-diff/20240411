# Comparing `tmp/viadot2-2.0a22.tar.gz` & `tmp/viadot2-2.0a23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viadot2-2.0a22.tar", last modified: Thu Mar 28 17:09:27 2024, max compression
+gzip compressed data, was "viadot2-2.0a23.tar", last modified: Thu Apr 11 08:31:36 2024, max compression
```

## Comparing `viadot2-2.0a22.tar` & `viadot2-2.0a23.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.011260 viadot2-2.0a22/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-28 17:09:20.000000 viadot2-2.0a22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-28 17:09:27.011260 viadot2-2.0a22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-28 17:09:20.000000 viadot2-2.0a22/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-28 17:09:20.000000 viadot2-2.0a22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 17:09:27.011260 viadot2-2.0a22/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.003260 viadot2-2.0a22/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.007260 viadot2-2.0a22/src/viadot/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.007260 viadot2-2.0a22/src/viadot/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.007260 viadot2-2.0a22/src/viadot/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/azure_data_lake.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10336 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/cloud_for_customers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/exchange_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    21215 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/genesys.py
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/minio.py
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/redshift_spectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/s3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    45347 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/sap_rfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/sharepoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/trino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/sources/uk_carbon_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/task_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23336 2024-03-28 17:09:20.000000 viadot2-2.0a22/src/viadot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:09:27.007260 viadot2-2.0a22/src/viadot2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-03-28 17:09:26.000000 viadot2-2.0a22/src/viadot2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-28 17:09:26.000000 viadot2-2.0a22/src/viadot2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:09:26.000000 viadot2-2.0a22/src/viadot2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-28 17:09:26.000000 viadot2-2.0a22/src/viadot2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 17:09:26.000000 viadot2-2.0a22/src/viadot2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.810063 viadot2-2.0a23/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 08:31:32.000000 viadot2-2.0a23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-11 08:31:36.810063 viadot2-2.0a23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-11 08:31:32.000000 viadot2-2.0a23/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-11 08:31:32.000000 viadot2-2.0a23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 08:31:36.810063 viadot2-2.0a23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.802063 viadot2-2.0a23/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.802063 viadot2-2.0a23/src/viadot/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.806063 viadot2-2.0a23/src/viadot/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.806063 viadot2-2.0a23/src/viadot/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8986 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/azure_data_lake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/cloud_for_customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20681 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/exchange_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21213 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/genesys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/minio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/redshift_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45697 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/sap_rfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/sharepoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/trino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/sources/uk_carbon_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/task_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23220 2024-04-11 08:31:32.000000 viadot2-2.0a23/src/viadot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 08:31:36.806063 viadot2-2.0a23/src/viadot2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-11 08:31:36.000000 viadot2-2.0a23/src/viadot2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 08:31:36.000000 viadot2-2.0a23/src/viadot2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 08:31:36.000000 viadot2-2.0a23/src/viadot2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-11 08:31:36.000000 viadot2-2.0a23/src/viadot2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 08:31:36.000000 viadot2-2.0a23/src/viadot2.egg-info/top_level.txt
```

### Comparing `viadot2-2.0a22/LICENSE` & `viadot2-2.0a23/LICENSE`

 * *Files identical despite different names*

### Comparing `viadot2-2.0a22/PKG-INFO` & `viadot2-2.0a23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viadot2
-Version: 2.0a22
+Version: 2.0a23
 Summary: A simple data ingestion library to guide data flows from some places to other places.
 Author-email: acivitillo <acivitillo@dyvenia.com>, trymzet <mzawadzki@dyvenia.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-core==1.25.0
 Requires-Dist: azure-storage-blob==12.13.1
@@ -29,21 +29,24 @@
 Requires-Dist: pandas-gbq==0.19.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: aiolimiter==1.0.0
 Requires-Dist: trino==0.326.*
 Requires-Dist: sqlalchemy==2.0.*
 Requires-Dist: minio<8.0,>=7.0
-Requires-Dist: databricks-connect==11.3.*
 Requires-Dist: azure-identity>=1.15.0
+Provides-Extra: databricks
+Requires-Dist: databricks-connect==11.3.*; extra == "databricks"
 
 # Viadot
+
 [![build status](https://github.com/dyvenia/viadot/actions/workflows/build.yml/badge.svg)](https://github.com/dyvenia/viadot/actions/workflows/build.yml)
 [![formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/Trymzet/dyvenia/branch/main/graph/badge.svg?token=k40ALkXbNq)](https://codecov.io/gh/Trymzet/dyvenia)
+
 ---
 
 **Documentation**: <a href="https://dyvenia.github.io/viadot/" target="_blank">https://dyvenia.github.io/viadot/</a>
 
 **Source Code**: <a href="https://github.com/dyvenia/viadot" target="_blank">https://github.com/dyvenia/viadot</a>
 
 ---
@@ -61,35 +64,42 @@
 ukci.query("/intensity")
 df = ukci.to_df()
 
 print(df)
 ```
 
 **Output:**
-|      | from              | to                | forecast | actual | index    |
+| | from | to | forecast | actual | index |
 | ---: | :---------------- | :---------------- | -------: | -----: | :------- |
-|    0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z |      211 |    216 | moderate |
+| 0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z | 211 | 216 | moderate |
 
 The above `df` is a pandas `DataFrame` object. It contains data downloaded by `viadot` from the Carbon Intensity UK API.
 
 ## Loading Data to a Source
-Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
+Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
 ## Getting started
+
 ### Prerequisites
-We assume that you have [Docker](https://www.docker.com/) installed.
+
+We assume that you have [Rye](https://rye-up.com/) installed:
+
+```console
+curl -sSf https://rye-up.com/get | bash
+```
 
 ### Installation
+
 Clone the `2.0` branch, and set up and run the environment:
-  ```sh
-  git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-    cd viadot/docker && \
-    sh update.sh  && \
-    sh run.sh && \
-    cd ../
-  ```
+
+```console
+git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
+  cd viadot && \
+  rye sync
+```
 
 ### Configuration
+
 In order to start using sources, you must configure them with required credentials. Credentials can be specified either in the viadot config file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to each source's `credentials` parameter.
 
 You can find specific information about each source's credentials in [the documentation](https://dyvenia.github.io/viadot/references/sql_sources/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viadot2 Version: 2.0a22 Summary: A simple data
+Metadata-Version: 2.1 Name: viadot2 Version: 2.0a23 Summary: A simple data
 ingestion library to guide data flows from some places to other places. Author-
 email: acivitillo
 dyvenia.com>, trymzet
 dyvenia.com> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: azure-core==1.25.0 Requires-Dist: azure-
 storage-blob==12.13.1 Requires-Dist: awswrangler==2.19.0 Requires-Dist:
 s3fs==2022.11.0 Requires-Dist: boto3==1.24.59 Requires-Dist: pandas==1.4.4
@@ -11,40 +11,40 @@
 matplotlib>=3.8.3 Requires-Dist: adlfs==2022.9.1 Requires-Dist: Shapely==1.8.0
 Requires-Dist: imagehash==4.2.1 Requires-Dist: visions==0.7.5 Requires-Dist:
 sharepy<2.1.0,>=2.0.0 Requires-Dist: simple_salesforce==1.11.5 Requires-Dist:
 sql-metadata==2.3.0 Requires-Dist: duckdb==0.5.1 Requires-Dist: sendgrid==6.9.7
 Requires-Dist: pandas-gbq==0.19.1 Requires-Dist: pyyaml>=6.0.1 Requires-Dist:
 pydantic==1.10.11 Requires-Dist: aiolimiter==1.0.0 Requires-Dist:
 trino==0.326.* Requires-Dist: sqlalchemy==2.0.* Requires-Dist: minio<8.0,>=7.0
-Requires-Dist: databricks-connect==11.3.* Requires-Dist: azure-identity>=1.15.0
-# Viadot [![build status](https://github.com/dyvenia/viadot/actions/workflows/
-build.yml/badge.svg)](https://github.com/dyvenia/viadot/actions/workflows/
-build.yml) [![formatting](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) [![codecov](https://codecov.io/gh/
-Trymzet/dyvenia/branch/main/graph/badge.svg?token=k40ALkXbNq)](https://
-codecov.io/gh/Trymzet/dyvenia) --- **Documentation**: _h_t_t_p_s_:_/_/
-_d_y_v_e_n_i_a_._g_i_t_h_u_b_._i_o_/_v_i_a_d_o_t_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_y_v_e_n_i_a_/_v_i_a_d_o_t --
-- A simple data ingestion library to guide data flows from some places to other
-places. ## Getting Data from a Source Viadot supports several API and RDBMS
-sources, private and public. Currently, we support the UK Carbon Intensity
-public API and base the examples on it. ```python from
-viadot.sources.uk_carbon_intensity import UKCarbonIntensity ukci =
-UKCarbonIntensity() ukci.query("/intensity") df = ukci.to_df() print(df) ```
+Requires-Dist: azure-identity>=1.15.0 Provides-Extra: databricks Requires-Dist:
+databricks-connect==11.3.*; extra == "databricks" # Viadot [![build status]
+(https://github.com/dyvenia/viadot/actions/workflows/build.yml/badge.svg)]
+(https://github.com/dyvenia/viadot/actions/workflows/build.yml) [![formatting]
+(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) [![codecov](https://codecov.io/gh/Trymzet/dyvenia/branch/
+main/graph/badge.svg?token=k40ALkXbNq)](https://codecov.io/gh/Trymzet/dyvenia)
+--- **Documentation**: _h_t_t_p_s_:_/_/_d_y_v_e_n_i_a_._g_i_t_h_u_b_._i_o_/_v_i_a_d_o_t_/ **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_y_v_e_n_i_a_/_v_i_a_d_o_t --- A simple data ingestion library to guide
+data flows from some places to other places. ## Getting Data from a Source
+Viadot supports several API and RDBMS sources, private and public. Currently,
+we support the UK Carbon Intensity public API and base the examples on it.
+```python from viadot.sources.uk_carbon_intensity import UKCarbonIntensity ukci
+= UKCarbonIntensity() ukci.query("/intensity") df = ukci.to_df() print(df) ```
 **Output:** | | from | to | forecast | actual | index | | ---: | :-------------
 --- | :---------------- | -------: | -----: | :------- | | 0 | 2021-08-10T11:
 00Z | 2021-08-10T11:30Z | 211 | 216 | moderate | The above `df` is a pandas
 `DataFrame` object. It contains data downloaded by `viadot` from the Carbon
 Intensity UK API. ## Loading Data to a Source Depending on the source, `viadot`
 provides different methods of uploading data. For instance, for SQL sources,
 this would be bulk inserts. For data lake sources, it would be a file upload.
 For ready-made pipelines including data validation steps using `dbt`, see
 [prefect-viadot](https://github.com/dyvenia/prefect-viadot). ## Getting started
-### Prerequisites We assume that you have [Docker](https://www.docker.com/
-) installed. ### Installation Clone the `2.0` branch, and set up and run the
-environment: ```sh git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-cd viadot/docker && \ sh update.sh && \ sh run.sh && \ cd ../ ``` ###
-Configuration In order to start using sources, you must configure them with
+### Prerequisites We assume that you have [Rye](https://rye-up.com/) installed:
+```console curl -sSf https://rye-up.com/get | bash ``` ### Installation Clone
+the `2.0` branch, and set up and run the environment: ```console git clone
+https://github.com/dyvenia/viadot.git -b 2.0 && \ cd viadot && \ rye sync ```
+### Configuration In order to start using sources, you must configure them with
 required credentials. Credentials can be specified either in the viadot config
 file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to
 each source's `credentials` parameter. You can find specific information about
 each source's credentials in [the documentation](https://dyvenia.github.io/
 viadot/references/sql_sources/).
```

### Comparing `viadot2-2.0a22/README.md` & `viadot2-2.0a23/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Viadot
+
 [![build status](https://github.com/dyvenia/viadot/actions/workflows/build.yml/badge.svg)](https://github.com/dyvenia/viadot/actions/workflows/build.yml)
 [![formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/Trymzet/dyvenia/branch/main/graph/badge.svg?token=k40ALkXbNq)](https://codecov.io/gh/Trymzet/dyvenia)
+
 ---
 
 **Documentation**: <a href="https://dyvenia.github.io/viadot/" target="_blank">https://dyvenia.github.io/viadot/</a>
 
 **Source Code**: <a href="https://github.com/dyvenia/viadot" target="_blank">https://github.com/dyvenia/viadot</a>
 
 ---
@@ -23,35 +25,42 @@
 ukci.query("/intensity")
 df = ukci.to_df()
 
 print(df)
 ```
 
 **Output:**
-|      | from              | to                | forecast | actual | index    |
+| | from | to | forecast | actual | index |
 | ---: | :---------------- | :---------------- | -------: | -----: | :------- |
-|    0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z |      211 |    216 | moderate |
+| 0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z | 211 | 216 | moderate |
 
 The above `df` is a pandas `DataFrame` object. It contains data downloaded by `viadot` from the Carbon Intensity UK API.
 
 ## Loading Data to a Source
-Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
+Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
 ## Getting started
+
 ### Prerequisites
-We assume that you have [Docker](https://www.docker.com/) installed.
+
+We assume that you have [Rye](https://rye-up.com/) installed:
+
+```console
+curl -sSf https://rye-up.com/get | bash
+```
 
 ### Installation
+
 Clone the `2.0` branch, and set up and run the environment:
-  ```sh
-  git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-    cd viadot/docker && \
-    sh update.sh  && \
-    sh run.sh && \
-    cd ../
-  ```
+
+```console
+git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
+  cd viadot && \
+  rye sync
+```
 
 ### Configuration
+
 In order to start using sources, you must configure them with required credentials. Credentials can be specified either in the viadot config file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to each source's `credentials` parameter.
 
-You can find specific information about each source's credentials in [the documentation](https://dyvenia.github.io/viadot/references/sql_sources/).
+You can find specific information about each source's credentials in [the documentation](https://dyvenia.github.io/viadot/references/sql_sources/).
```

#### html2text {}

```diff
@@ -16,17 +16,17 @@
 00Z | 2021-08-10T11:30Z | 211 | 216 | moderate | The above `df` is a pandas
 `DataFrame` object. It contains data downloaded by `viadot` from the Carbon
 Intensity UK API. ## Loading Data to a Source Depending on the source, `viadot`
 provides different methods of uploading data. For instance, for SQL sources,
 this would be bulk inserts. For data lake sources, it would be a file upload.
 For ready-made pipelines including data validation steps using `dbt`, see
 [prefect-viadot](https://github.com/dyvenia/prefect-viadot). ## Getting started
-### Prerequisites We assume that you have [Docker](https://www.docker.com/
-) installed. ### Installation Clone the `2.0` branch, and set up and run the
-environment: ```sh git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-cd viadot/docker && \ sh update.sh && \ sh run.sh && \ cd ../ ``` ###
-Configuration In order to start using sources, you must configure them with
+### Prerequisites We assume that you have [Rye](https://rye-up.com/) installed:
+```console curl -sSf https://rye-up.com/get | bash ``` ### Installation Clone
+the `2.0` branch, and set up and run the environment: ```console git clone
+https://github.com/dyvenia/viadot.git -b 2.0 && \ cd viadot && \ rye sync ```
+### Configuration In order to start using sources, you must configure them with
 required credentials. Credentials can be specified either in the viadot config
 file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to
 each source's `credentials` parameter. You can find specific information about
 each source's credentials in [the documentation](https://dyvenia.github.io/
 viadot/references/sql_sources/).
```

### Comparing `viadot2-2.0a22/pyproject.toml` & `viadot2-2.0a23/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "viadot2"
-version = "2.0a22"
+version = "2.0a23"
 description = "A simple data ingestion library to guide data flows from some places to other places."
 authors = [
     { name = "acivitillo", email = "acivitillo@dyvenia.com" },
     { name = "trymzet", email = "mzawadzki@dyvenia.com" },
 ]
 dependencies = [
     "azure-core==1.25.0",
@@ -30,39 +30,37 @@
     "pandas-gbq==0.19.1",
     "pyyaml>=6.0.1",
     "pydantic==1.10.11",
     "aiolimiter==1.0.0",
     "trino==0.326.*",
     "sqlalchemy==2.0.*",
     "minio>=7.0, <8.0",
-    "databricks-connect==11.3.*",
     "azure-identity>=1.15.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
+[project.optional-dependencies]
+databricks = [
+    "databricks-connect==11.3.*",
+]
+
 [tool.rye]
 dev-dependencies = [
     "black==22.6.0",
     "pytest==8.1.1",
     "pytest-cov==3.0.0",
     "mkdocs-autorefs==0.4.1",
     "mkdocs-material-extensions==1.0.3",
     "mkdocs-material==8.4.3",
     "mkdocs==1.3.1",
     "mkdocstrings==0.19.0",
     "Faker==13.12.1",
     "python-dotenv>=1.0.1",
-]
-
-[tool.coverage.run]
-omit = [
-    "viadot/flows/azure_sql_transform_dbt.py",
-    "viadot/flows/supermetrics_to_adls.py",
-    "viadot/flows/supermetrics_to_azure_sql_v2.py",
+    "coverage>=7.4.4",
 ]
 
 [tool.pytest.ini_options]
 log_format = "%(asctime)s %(levelname)s %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 log_cli = true
 log_level = "WARNING"
```

### Comparing `viadot2-2.0a22/src/viadot/config.py` & `viadot2-2.0a23/src/viadot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 
 class Config(dict):
     @classmethod
     def _get_configuration(
         cls, config: dict, key: Optional[str] = None
     ) -> Optional[dict]:
-
         # Empty config.
         if not config:
             return
 
         # Config key does not exist or has no values.
         if key:
             config = config.get(key)
```

### Comparing `viadot2-2.0a22/src/viadot/exceptions.py` & `viadot2-2.0a23/src/viadot/exceptions.py`

 * *Files identical despite different names*

### Comparing `viadot2-2.0a22/src/viadot/sources/azure_data_lake.py` & `viadot2-2.0a23/src/viadot/sources/azure_data_lake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from typing import Any, Dict, List
 
 import pandas as pd
 from adlfs import AzureBlobFileSystem, AzureDatalakeFileSystem
 
-from ..config import get_source_credentials
-from ..exceptions import CredentialError
-from .base import Source
-from ..utils import add_viadot_metadata_columns
+from viadot.config import get_source_credentials
+from viadot.exceptions import CredentialError
+from viadot.sources.base import Source
+from viadot.utils import add_viadot_metadata_columns
 
 
 class AzureDataLake(Source):
     """
     A class for pulling data from the Azure Data Lakes (gen1 and gen2).
 
     You can either connect to the lake in general
@@ -31,15 +31,14 @@
         path: str = None,
         gen: int = 2,
         credentials: Dict[str, Any] = None,
         config_key: str = None,
         *args,
         **kwargs,
     ):
-
         credentials = credentials or get_source_credentials(config_key)
         required_credentials = (
             "account_name",
             "tenant_id",
             "client_id",
             "client_secret",
         )
@@ -78,15 +77,15 @@
             self.storage_options["account_name"] = storage_account_name
             self.fs = AzureBlobFileSystem(
                 account_name=storage_account_name,
                 tenant_id=tenant_id,
                 client_id=client_id,
                 client_secret=client_secret,
             )
-            self.base_url = f"az://"
+            self.base_url = "az://"
 
     def upload(
         self,
         from_path: str,
         to_path: str = None,
         recursive: bool = False,
         overwrite: bool = False,
@@ -106,15 +105,15 @@
 
         lake = AzureDataLake()
         lake.upload(from_path='tests/test.csv', to_path="sandbox/test.csv")
         ```
         """
 
         if self.gen == 1:
-            raise NotImplemented(
+            raise NotImplementedError(
                 "Azure Data Lake Gen1 does not support simple file upload."
             )
 
         to_path = to_path or self.path
 
         self.logger.info(f"Uploading file(s) from '{from_path}' to '{to_path}'...")
 
@@ -161,17 +160,16 @@
     def download(
         self,
         to_path: str,
         from_path: str = None,
         recursive: bool = False,
         overwrite: bool = True,
     ) -> None:
-
         if overwrite is False:
-            raise NotImplemented(
+            raise NotImplementedError(
                 "Currently, only the default behavior (overwrite) is available."
             )
 
         from_path = from_path or self.path
         self.fs.download(rpath=from_path, lpath=to_path, recursive=recursive)
 
     @add_viadot_metadata_columns
```

### Comparing `viadot2-2.0a22/src/viadot/sources/base.py` & `viadot2-2.0a23/src/viadot/sources/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from abc import abstractmethod
 from typing import Any, Dict, List, Literal, NoReturn, Tuple, Union
 
 import pandas as pd
 import pyarrow as pa
 import pyodbc
 
-from ..config import get_source_credentials
-from ..signals import SKIP
+from viadot.config import get_source_credentials
+from viadot.signals import SKIP
 
 logger = logging.getLogger(__name__)
 
 Record = Tuple[Any]
 
 
 class Source:
```

### Comparing `viadot2-2.0a22/src/viadot/sources/cloud_for_customers.py` & `viadot2-2.0a23/src/viadot/sources/cloud_for_customers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from typing import Any, Dict, List, Optional
 from urllib.parse import urljoin
 
 import pandas as pd
 import requests
 from pydantic import BaseModel, SecretStr, root_validator
 
+from viadot.config import get_source_credentials
 from viadot.exceptions import CredentialError
-
-from ..config import get_source_credentials
-from ..utils import handle_api_response, validate
-from .base import Source
+from viadot.sources.base import Source
+from viadot.utils import handle_api_response, validate
 
 
 class CloudForCustomersCredentials(BaseModel):
     username: str  # eg. username@{tenant_name}.com
     password: SecretStr
     url: Optional[str] = None  # The URL to extract records from.
     report_url: Optional[str] = None  # The URL of a prepared report.
```

### Comparing `viadot2-2.0a22/src/viadot/sources/databricks.py` & `viadot2-2.0a23/src/viadot/sources/databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import json
 import os
 from typing import Literal, Optional, Union
 
 import pandas as pd
-import pyspark.sql.dataframe as spark
-from delta.tables import *
-from pydantic import BaseModel, root_validator
 
-from viadot.exceptions import CredentialError
+try:
+    import pyspark.sql.dataframe as spark
+    from delta.tables import *  # noqa
+except ModuleNotFoundError:
+    raise ImportError("pyspark.sql.dataframe is required to use Databricks source.")
+
+from pydantic import BaseModel, root_validator
 
-from ..config import get_source_credentials
-from ..exceptions import TableAlreadyExists, TableDoesNotExist
-from ..utils import (
+from viadot.config import get_source_credentials
+from viadot.exceptions import CredentialError, TableAlreadyExists, TableDoesNotExist
+from viadot.sources.base import Source
+from viadot.utils import (
+    _cast_df_cols,
     add_viadot_metadata_columns,
     build_merge_query,
     df_snakecase_column_names,
-    _cast_df_cols,
 )
-from .base import Source
 
 
 class DatabricksCredentials(BaseModel):
     host: str  # The host address of the Databricks cluster.
     port: str = "15001"  # The port on which the cluster is exposed. By default '15001'. For Spark Connect, use the port 443 by default.
     cluster_id: str  # The ID of the Databricks cluster to which to connect.
     org_id: Optional[
@@ -80,15 +83,15 @@
 
     def __exit__(self, exc_type, exc_value, traceback):
         if self._session:
             self._session.stop()
             self._session = None
 
     @property
-    def session(self) -> Union[SparkSession, "DatabricksSession"]:
+    def session(self) -> Union[SparkSession, "DatabricksSession"]:  # noqa
         if self._session is None:
             session = self._create_spark_session()
             self._session = session
             return session
         return self._session
 
     def _create_spark_session(self):
@@ -106,15 +109,15 @@
             org_id=self.credentials.get("org_id"),
             port=self.credentials.get("port"),
         )
 
         with open(os.path.expanduser("~/.databricks-connect"), "w") as f:
             json.dump(db_connect_config, f)
 
-        spark = SparkSession.builder.getOrCreate()
+        spark = SparkSession.builder.getOrCreate()  # noqa
         return spark
 
     def _create_spark_connect_session(self):
         """
         Establish a connection to a Databricks cluster.
 
         Returns:
```

### Comparing `viadot2-2.0a22/src/viadot/sources/exchange_rates.py` & `viadot2-2.0a23/src/viadot/sources/exchange_rates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import json
 from datetime import datetime
 from typing import Any, Dict, List, Literal
 
 import pandas as pd
 import requests
 
+from viadot.config import get_source_credentials
 from viadot.exceptions import CredentialError
+from viadot.sources.base import Source
 from viadot.utils import add_viadot_metadata_columns, cleanup_df, validate
 
-from ..config import get_source_credentials
-from .base import Source
-
 Currency = Literal[
     "USD", "EUR", "GBP", "CHF", "PLN", "DKK", "COP", "CZK", "SEK", "NOK", "ISK"
 ]
 
 
 class ExchangeRates(Source):
-
     URL = "https://api.apilayer.com/exchangerates_data/timeseries"
 
     def __init__(
         self,
         currency: Currency = "USD",
         start_date: str = datetime.today().strftime("%Y-%m-%d"),
         end_date: str = datetime.today().strftime("%Y-%m-%d"),
@@ -108,15 +106,14 @@
             )
         except ConnectionError as e:
             raise e
 
         return json.loads(response.text)
 
     def to_records(self) -> List[tuple]:
-
         data = self.get_data()
         records = []
 
         for j in data["rates"]:
             records.append(j)
             records.append(data["base"])
 
@@ -124,21 +121,19 @@
                 records.append(data["rates"][j][i])
 
         records = [x for x in zip(*[iter(records)] * (2 + len(self.symbols)))]
 
         return records
 
     def get_columns(self) -> List[str]:
-
         columns = ["Date", "Base"] + self.symbols
 
         return columns
 
     def to_json(self) -> Dict[str, Any]:
-
         records = self.to_records()
         columns = self.get_columns()
         records = [dict(zip(columns, records[i])) for i in range(len(records))]
         json = {}
         json["currencies"] = records
 
         return json
```

### Comparing `viadot2-2.0a22/src/viadot/sources/genesys.py` & `viadot2-2.0a23/src/viadot/sources/genesys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import os
-import json
+import asyncio
 import base64
+import json
+import os
 import warnings
-import asyncio
-from typing import Any, Dict, List, Literal, Optional
 from io import StringIO
+from typing import Any, Dict, List, Literal, Optional
 
 import aiohttp
 import pandas as pd
 from aiolimiter import AsyncLimiter
 
-from ..config import get_source_credentials
-from .base import Source
-from ..exceptions import CredentialError, APIError
-from ..utils import handle_api_response, validate
-from ..signals import SKIP
+from viadot.config import get_source_credentials
+from viadot.exceptions import APIError, CredentialError
+from viadot.signals import SKIP
+from viadot.sources.base import Source
+from viadot.utils import handle_api_response, validate
 
 warnings.simplefilter("ignore")
 
 
 class Genesys(Source):
     def __init__(
         self,
@@ -85,15 +85,15 @@
 
         if self.environment is None:
             self.environment = self.credentials.get("ENVIRONMENT", None)
 
         if self.ids_mapping is None:
             self.ids_mapping = self.credentials.get("IDS_MAPPING", None)
 
-            if type(self.ids_mapping) is dict and self.ids_mapping is not None:
+            if isinstance(self.ids_mapping, dict) and self.ids_mapping is not None:
                 self.logger.info("IDS_MAPPING loaded from local credential.")
             else:
                 self.logger.warning(
                     "IDS_MAPPING is not provided in you credentials or is not a dictionary."
                 )
 
         self.report_data = []
@@ -231,15 +231,15 @@
         Returns:
             None
         """
         request_json = self.load_reporting_exports()
 
         if request_json is not None:
             entities = request_json.get("entities")
-            assert type(entities) == list
+            assert isinstance(entities, list)
             if len(entities) != 0:
                 for entity in entities:
                     tmp = [
                         entity.get("id"),
                         entity.get("downloadUrl"),
                         entity.get("filter").get("queueIds", [-1])[0],
                         entity.get("filter").get("mediaTypes", [-1])[0],
@@ -278,18 +278,19 @@
             url=f"{report_url}", headers=self.authorization_token
         )
         if output_file_name is None:
             final_file_name = f"Genesys_Queue_Metrics_Interval_Export.{file_extension}"
         else:
             final_file_name = f"{output_file_name}.{file_extension}"
 
-        response_data = response_file.content
         df = pd.read_csv(StringIO(response_file.content.decode("utf-8")))
+
         if drop_duplicates is True:
             df.drop_duplicates(inplace=True, ignore_index=True)
+
         df.to_csv(os.path.join(path, final_file_name), index=False, sep=sep)
 
     def download_all_reporting_exports(
         self, store_file_names: bool = True, path: str = ""
     ) -> List[str]:
         """
         Get information form data report and download all files.
```

### Comparing `viadot2-2.0a22/src/viadot/sources/minio.py` & `viadot2-2.0a23/src/viadot/sources/minio.py`

 * *Files identical despite different names*

### Comparing `viadot2-2.0a22/src/viadot/sources/redshift_spectrum.py` & `viadot2-2.0a23/src/viadot/sources/redshift_spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             schema (str): The name of the schema.
             description (str, optional): The description of the schema. Defaults to None.
         """
         self._create_glue_database(
             database=schema, description=description, exist_ok=True
         )
         create_schema_query = f"""
-create external schema if not exists "{schema}" from data catalog 
+create external schema if not exists "{schema}" from data catalog
 database '{schema}'
 iam_role '{self.credentials.get("iam_role")}'
 region '{self.credentials.get("region_name")}'
 CREATE EXTERNAL DATABASE IF NOT EXISTS;
 """
         with self.con.cursor() as cursor:
             cursor.execute(create_schema_query)
```

### Comparing `viadot2-2.0a22/src/viadot/sources/s3.py` & `viadot2-2.0a23/src/viadot/sources/s3.py`

 * *Files identical despite different names*

### Comparing `viadot2-2.0a22/src/viadot/sources/sap_rfc.py` & `viadot2-2.0a23/src/viadot/sources/sap_rfc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import logging
 import re
 from collections import OrderedDict
 from typing import (
     Any,
     Dict,
+    Iterable,
+    Iterator,
     List,
-    OrderedDict as OrderedDictType,
     Literal,
     Tuple,
     Union,
-    Iterable,
-    Iterator,
 )
-
+from typing import (
+    OrderedDict as OrderedDictType,
+)
 
 import numpy as np
 import pandas as pd
 
 try:
     import pyrfc
     from pyrfc._exception import ABAPApplicationError
 except ModuleNotFoundError:
     raise ImportError("pyfrc is required to use the SAPRFC source.")
 from sql_metadata import Parser
 
 from viadot.config import get_source_credentials
-from ..utils import validate, add_viadot_metadata_columns
 from viadot.exceptions import CredentialError, DataBufferExceeded
 from viadot.sources.base import Source
+from viadot.utils import add_viadot_metadata_columns, validate
 
 logger = logging.getLogger()
 
 
 def remove_whitespaces(text):
     return " ".join(text.split())
 
@@ -119,15 +120,15 @@
             logger.warning(
                 f"Empty output was generated for chunk {chunk} in columns {fields}."
             )
             start = True
     elif data_raw.shape[0] != row_index:
         data_raw = data_raw[:row_index]
         logger.warning(
-            f"New rows were generated during the execution of the script. The table is truncated to the number of rows for the first chunk."
+            "New rows were generated during the execution of the script. The table is truncated to the number of rows for the first chunk."
         )
 
     return row_index, data_raw, start
 
 
 def replace_separator_in_data(
     data_raw: np.array,
@@ -154,15 +155,15 @@
     for no_sep in no_sep_index:
         logger.warning(
             "A separator character was found and replaced inside a string text that could produce future errors:"
         )
         logger.warning("\n" + data_raw[no_sep][record_key])
         split_array = np.array([*data_raw[no_sep][record_key]])
         position = np.where(split_array == f"{sep}")[0]
-        index_sep_index = np.argwhere(np.in1d(position, pos_sep_index) == False)
+        index_sep_index = np.argwhere(np.in1d(position, pos_sep_index) == False)  # noqa
         index_sep_index = index_sep_index.reshape(
             len(index_sep_index),
         )
         split_array[position[index_sep_index]] = replacement
         data_raw[no_sep][record_key] = "".join(split_array)
         logger.warning("\n" + data_raw[no_sep][record_key])
 
@@ -407,15 +408,15 @@
                     "WHERE conditions after the 75 character limit can only be combined with the AND keyword."
                 )
             else:
                 filters_pretty = list(client_side_filters.items())
                 self.logger.warning(
                     f"Trimmed conditions ({filters_pretty}) will be applied client-side."
                 )
-                self.logger.warning(f"See the documentation for caveats.")
+                self.logger.warning("See the documentation for caveats.")
 
         self.client_side_filters = client_side_filters
         return where_trimmed
 
     @staticmethod
     def _get_table_name(sql: str) -> str:
         parsed = Parser(sql)
@@ -866,15 +867,15 @@
                     "WHERE conditions after the 75 character limit can only be combined with the AND keyword."
                 )
             else:
                 filters_pretty = list(client_side_filters.items())
                 self.logger.warning(
                     f"Trimmed conditions ({filters_pretty}) will be applied client-side."
                 )
-                self.logger.warning(f"See the documentation for caveats.")
+                self.logger.warning("See the documentation for caveats.")
 
         self.client_side_filters = client_side_filters
         return where_trimmed
 
     @staticmethod
     def _get_table_name(sql: str) -> str:
         parsed = Parser(sql)
@@ -1157,47 +1158,51 @@
                 except ABAPApplicationError as e:
                     if e.key == "DATA_BUFFER_EXCEEDED":
                         raise DataBufferExceeded(
                             "Character limit per row exceeded. Please select fewer columns."
                         )
                     else:
                         raise e
-                record_key = "WA"
-                data_raw = np.array(response["DATA"])
-                del response
-
-                # if the reference columns are provided not necessary to remove any extra row.
-                if not isinstance(self.rfc_unique_id[0], str):
-                    row_index, data_raw, start = detect_extra_rows(
-                        row_index, data_raw, chunk, fields
-                    )
-                else:
-                    start = False
+                # Check and skip if there is no data returned
+                if response["DATA"]:
+                    record_key = "WA"
+                    data_raw = np.array(response["DATA"])
+                    del response
+
+                    # if the reference columns are provided not necessary to remove any extra row.
+                    if not isinstance(self.rfc_unique_id[0], str):
+                        row_index, data_raw, start = detect_extra_rows(
+                            row_index, data_raw, chunk, fields
+                        )
+                    else:
+                        start = False
 
-                records = [row for row in gen_split(data_raw, sep, record_key)]
-                del data_raw
+                    records = [row for row in gen_split(data_raw, sep, record_key)]
+                    del data_raw
 
-                if (
-                    isinstance(self.rfc_unique_id[0], str)
-                    and not list(df.columns) == fields
-                ):
-                    df_tmp = pd.DataFrame(columns=fields)
-                    df_tmp[fields] = records
-                    # SAP adds whitespaces to the first extracted column value
-                    # If whitespace is in unique column it must be removed to make a proper merge
-                    for col in self.rfc_unique_id:
-                        df_tmp[col] = df_tmp[col].str.strip()
-                        df[col] = df[col].str.strip()
-                    df = pd.merge(df, df_tmp, on=self.rfc_unique_id, how="outer")
-                else:
-                    if not start:
-                        df[fields] = records
+                    if (
+                        isinstance(self.rfc_unique_id[0], str)
+                        and not list(df.columns) == fields
+                    ):
+                        df_tmp = pd.DataFrame(columns=fields)
+                        df_tmp[fields] = records
+                        # SAP adds whitespaces to the first extracted column value
+                        # If whitespace is in unique column it must be removed to make a proper merge
+                        for col in self.rfc_unique_id:
+                            df_tmp[col] = df_tmp[col].str.strip()
+                            df[col] = df[col].str.strip()
+                        df = pd.merge(df, df_tmp, on=self.rfc_unique_id, how="outer")
                     else:
-                        df[fields] = np.nan
-                chunk += 1
+                        if not start:
+                            df[fields] = records
+                        else:
+                            df[fields] = np.nan
+                    chunk += 1
+                elif not response["DATA"]:
+                    print("No data returned from SAP.")
         df.columns = columns
 
         if self.client_side_filters:
             filter_query = self._build_pandas_filter_query(self.client_side_filters)
             df.query(filter_query, inplace=True)
             client_side_filter_cols_aliased = [
                 self._get_alias(col) for col in self._get_client_side_filter_cols()
```

### Comparing `viadot2-2.0a22/src/viadot/sources/sharepoint.py` & `viadot2-2.0a23/src/viadot/sources/sharepoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from typing import Optional, Union
 
 import pandas as pd
 import sharepy
 from pydantic import BaseModel, root_validator
 from sharepy.errors import AuthError
 
+from viadot.config import get_source_credentials
 from viadot.exceptions import CredentialError
-
-from ..config import get_source_credentials
-from ..signals import SKIP
-from ..utils import add_viadot_metadata_columns, cleanup_df, validate
-from .base import Source
+from viadot.signals import SKIP
+from viadot.sources.base import Source
+from viadot.utils import add_viadot_metadata_columns, cleanup_df, validate
 
 
 class SharepointCredentials(BaseModel):
     site: str  # Path to sharepoint website (e.g : {tenant_name}.sharepoint.com)
     username: str  # Sharepoint username (e.g username@{tenant_name}.com)
     password: str  # Sharepoint password
```

### Comparing `viadot2-2.0a22/src/viadot/sources/sqlite.py` & `viadot2-2.0a23/src/viadot/sources/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .base import SQL
+from viadot.sources.base import SQL
 
 
 class SQLite(SQL):
     """A SQLite source
 
     Args:
         server (str): server string, usually localhost
```

### Comparing `viadot2-2.0a22/src/viadot/sources/trino.py` & `viadot2-2.0a23/src/viadot/sources/trino.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 WHERE TABLE_SCHEMA = '{schema_name}'
 AND TABLE_NAME = '{table_name}'"""
         with self.get_connection() as connection:
             results = list(self.run(query, connection=connection))
         return len(results) > 0
 
     def get_schemas(self) -> list[str]:
-        query = f"SHOW SCHEMAS"
+        query = "SHOW SCHEMAS"
         with self.get_connection() as connection:
             return list(self.run(query, connection=connection))
 
     def _check_if_schema_exists(self, schema_name: str) -> None:
         query = f"SELECT * FROM INFORMATION_SCHEMA.SCHEMATA WHERE SCHEMA_NAME = '{schema_name}'"
         with self.get_connection() as connection:
             results = list(self.run(query, connection=connection))
@@ -271,15 +271,15 @@
             for partition in result.partitions():
                 yield from partition
 
         self.logger.debug("Executing SQL:\n" + sql)
 
         try:
             # Execute with server-side cursor of size 5000.
-            result = connection.execution_options(yield_per=5000,).execute(text(sql))
+            result = connection.execution_options(yield_per=5000).execute(text(sql))
         except Exception as e:
             raise ValueError(f"Failed executing SQL:\n{sql}") from e
 
         query_keywords = ["SELECT", "SHOW", "PRAGMA", "WITH"]
         is_query = any(sql.strip().upper().startswith(word) for word in query_keywords)
 
         if is_query:
```

### Comparing `viadot2-2.0a22/src/viadot/sources/uk_carbon_intensity.py` & `viadot2-2.0a23/src/viadot/sources/uk_carbon_intensity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import requests
 
-from .base import Source
-from ..utils import add_viadot_metadata_columns
+from viadot.sources.base import Source
+from viadot.utils import add_viadot_metadata_columns
 
 
 class UKCarbonIntensity(Source):
     """Fetches data of Carbon Intensity of the UK Power Grid.
 
     Documentation for this source API is located
     at: https://carbon-intensity.github.io/api-definitions/#carbon-intensity-api-v2-0-0
```

### Comparing `viadot2-2.0a22/src/viadot/task_utils.py` & `viadot2-2.0a23/src/viadot/task_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,15 @@
     given a list of paths in that directory. Such list can be obtained using the
     `AzureDataLakeList` task. This task is useful for working with immutable data lakes as
     the data is often written in the format /path/table_name/TIMESTAMP.parquet.
     """
 
     logger = prefect.context.get("logger")
 
-    extract_fname = (
-        lambda f: os.path.basename(f).replace(".csv", "").replace(".parquet", "")
-    )
-    file_names = [extract_fname(file) for file in files]
+    file_names = [Path(file).stem for file in files]
     latest_file_name = max(file_names, key=lambda d: datetime.fromisoformat(d))
     latest_file = files[file_names.index(latest_file_name)]
 
     logger.debug(f"Latest file: {latest_file}")
 
     return latest_file
 
@@ -196,15 +193,14 @@
 def df_to_csv(
     df: pd.DataFrame,
     path: str,
     sep="\t",
     if_exists: Literal["append", "replace", "skip"] = "replace",
     **kwargs,
 ) -> None:
-
     """
     Task to create csv file based on pandas DataFrame.
     Args:
     df (pd.DataFrame): Input pandas DataFrame.
     path (str): Path to output csv file.
     sep (str, optional): The separator to use in the CSV. Defaults to "\t".
     if_exists (Literal["append", "replace", "skip"], optional): What to do if the table exists. Defaults to "replace".
@@ -222,15 +218,15 @@
         out_df = df
 
     # create directories if they don't exist
     try:
         if not os.path.isfile(path):
             directory = os.path.dirname(path)
             os.makedirs(directory, exist_ok=True)
-    except:
+    except Exception:
         pass
 
     out_df.to_csv(path, index=False, sep=sep)
 
 
 @task
 def df_to_parquet(
@@ -258,15 +254,15 @@
         out_df = df
 
     # create directories if they don't exist
     try:
         if not os.path.isfile(path):
             directory = os.path.dirname(path)
             os.makedirs(directory, exist_ok=True)
-    except:
+    except Exception:
         pass
 
     out_df.to_parquet(path, index=False, **kwargs)
 
 
 @task
 def union_dfs_task(dfs: List[pd.DataFrame]):
@@ -307,15 +303,15 @@
     shutil.rmtree(ge_project_path)
 
 
 @task
 def df_converts_bytes_to_int(df: pd.DataFrame) -> pd.DataFrame:
     logger = prefect.context.get("logger")
     logger.info("Converting bytes in dataframe columns to list of integers")
-    return df.applymap(lambda x: list(map(int, x)) if isinstance(x, bytes) else x)
+    return df.applymap(lambda x: list(map(int, x)) if isinstance(x, bytes) else x)  # noqa
 
 
 @task(
     max_retries=3,
     retry_delay=timedelta(seconds=10),
 )
 def df_to_dataset(
@@ -360,15 +356,14 @@
     only_states: list = [Failed],
     local_api_key: str = None,
     credentials_secret: str = None,
     vault_name: str = None,
     from_email: str = None,
     to_emails: str = None,
 ) -> prefect.engine.state.State:
-
     """
     Custom state handler configured to work with sendgrid.
     Works as a standalone state handler, or can be called from within a custom state handler.
     Args:
         tracked_obj (Task or Flow): Task or Flow object the handler is registered with.
         old_state (State): previous state of tracked object.
         new_state (State): new state of tracked object.
@@ -413,16 +408,16 @@
         from_email=from_email,
         to_emails=to_emails,
         subject=f"The flow {tracked_obj.name} - Status {new_state}",
         html_content=f"<strong>The flow {cast(str,tracked_obj.name)} FAILED at {curr_dt}. \
     <p>More details here: {url}</p></strong>",
     )
     try:
-        send_grid = SendGridAPIClient(api_key)
-        response = send_grid.send(message)
+        sendgrid = SendGridAPIClient(api_key)
+        sendgrid.send(message)
     except Exception as e:
         raise e
 
     return new_state
 
 
 @task
```

### Comparing `viadot2-2.0a22/src/viadot/utils.py` & `viadot2-2.0a23/src/viadot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import functools
 import logging
 import re
 import subprocess
 from datetime import datetime, timezone
-from typing import Any, Callable, Dict, List, Literal, Union, Optional
+from typing import Any, Callable, Dict, List, Literal, Optional
 
 import pandas as pd
 import pyodbc
-import pyspark.sql.dataframe as spark
 import requests
 
 # from prefect.utilities.graphql import EnumValue, with_args
 from requests.adapters import HTTPAdapter
 from requests.exceptions import ConnectionError, HTTPError, ReadTimeout, Timeout
 from requests.packages.urllib3.util.retry import Retry
 from urllib3.exceptions import ProtocolError
 
-from .exceptions import APIError
-from .exceptions import ValidationError
-from .signals import SKIP
+from viadot.exceptions import APIError, ValidationError
+from viadot.signals import SKIP
+
+try:
+    import pyspark.sql.dataframe as spark
+except ImportError:
+    pass
 
 
 def slugify(name: str) -> str:
     return name.replace(" ", "_").lower()
 
 
 def handle_api_request(
@@ -85,24 +88,24 @@
     url = response.url
     try:
         response.raise_for_status()
     except ReadTimeout as e:
         msg = "The connection was successful, "
         msg += f"however the API call to {url} timed out after {timeout[1]}s "
         msg += "while waiting for the server to return data."
-        raise APIError(msg)
+        raise APIError(msg) from e
     except HTTPError as e:
         raise APIError(
             f"The API call to {url} failed. "
             "Perhaps your account credentials need to be refreshed?",
         ) from e
     except (ConnectionError, Timeout) as e:
         raise APIError(f"The API call to {url} failed due to connection issues.") from e
-    except ProtocolError as e:
-        raise APIError(f"Did not receive any reponse for the API call to {url}.")
+    except ProtocolError:
+        raise APIError(f"Did not receive any response for the API call to {url}.")
     except Exception as e:
         raise APIError("Unknown error.") from e
 
     return response
 
 
 def handle_api_response(
@@ -167,15 +170,15 @@
             to None.
 
     Returns:
         dict: A dictionary of the form {column_name: dtype, ...}.
     """
 
     query = f"""
-    SELECT 
+    SELECT
         col.name,
         t.name,
         col.max_length
     FROM sys.tables AS tab
         INNER JOIN sys.columns AS col
             ON tab.object_id = col.object_id
         LEFT JOIN sys.types AS t
@@ -242,31 +245,30 @@
 
     return df
 
 
 def build_merge_query(
     table: str,
     primary_key: str,
-    source: Union[pyodbc.Connection, "Databricks"],
+    source,
     stg_schema: str = None,
     stg_table: str = "stg",
     schema: str = None,
-    df: spark.DataFrame = None,
+    df: Optional["spark.DataFrame"] = None,
 ) -> str:
     """
     Build a merge query for the simplest possible upsert scenario:
     - updating and inserting all fields
     - merging on a single column, which has the same name in both tables
 
     Args:
         table (str): The table to merge into.
         primary_key (str): The column on which to merge.
-        source (pyodbc.Connection or Databricks): Either the connection to the database
-            or the Databricks object used to connect to the Spark cluster on which
-            the query will be executed.
+        source (Source): The Databricks object used to connect to the Spark cluster on
+            which the query will be executed.
         stg_schema (str, Optional): The schema where the staging table is located.
         stg_table (str, Optional): The table with new/updated data.
         schema (str, Optional): The schema where the table is located.
         df (spark.DataFrame, Optional): A Spark DataFrame whose data will be upserted
             to a table.
     """
     fqn = f"{schema}.{table}"
@@ -296,36 +298,33 @@
         WHEN NOT MATCHED
             THEN INSERT({", ".join(columns)})
             VALUES({", ".join(columns_stg_fqn)});
     """
     return merge_query
 
 
-def _get_table_columns(
-    schema: str, table: str, source: Union[pyodbc.Connection, "Databricks"]
-) -> str:
-    if isinstance(source, pyodbc.Connection):
+def _get_table_columns(schema: str, table: str, source) -> str:
+    if source.__class__.__name__ == "Databricks":
+        result = source.run(f"SHOW COLUMNS IN {schema}.{table}", "pandas")
+        columns_query_result = result["col_name"].values
+    else:
         columns_query = f"""
-        SELECT 
+        SELECT
             col.name
         FROM sys.tables AS tab
             INNER JOIN sys.columns AS col
                 ON tab.object_id = col.object_id
         WHERE tab.name = '{table}'
         AND schema_name(tab.schema_id) = '{schema}'
         ORDER BY column_id;
         """
-        cursor = source.cursor()
+        cursor = source.con.cursor()
         columns_query_result = cursor.execute(columns_query).fetchall()
         cursor.close()
 
-    else:
-        result = source.run(f"SHOW COLUMNS IN {schema}.{table}", "pandas")
-        columns_query_result = result["col_name"].values
-
     return columns_query_result
 
 
 def gen_bulk_insert_query_from_df(
     df: pd.DataFrame, table_fqn: str, chunksize=1000, **kwargs
 ) -> str:
     """
@@ -356,15 +355,14 @@
     """
     if df.shape[1] == 1:
         raise NotImplementedError(
             "Currently, this function only handles DataFrames with at least two columns."
         )
 
     def _gen_insert_query_from_records(records: List[tuple]) -> str:
-
         tuples = map(str, tuple(records))
 
         # Change Nones to NULLs
         none_nan_pattern = r"(?<=\W)(nan|None)(?=\W)"
         values = re.sub(none_nan_pattern, "NULL", (",\n" + " " * 7).join(tuples))
 
         # Change the double quotes into single quotes, as explained above.
@@ -387,15 +385,15 @@
     # Escape values with single quotes inside by adding another single quote
     # ("val'ue" -> "val''ue").
     # As Python wraps such strings in double quotes, which are interpreted as
     # column names by SQL Server, we later also replace the double quotes with
     # single quotes.
     tuples_escaped = [
         tuple(
-            f"""{value.replace("'", "''")}""" if type(value) == str else value
+            f"""{value.replace("'", "''")}""" if isinstance(value, str) else value
             for value in row
         )
         for row in tuples_raw
     ]
 
     if len(tuples_escaped) > chunksize:
         insert_query = ""
@@ -497,21 +495,21 @@
             )
             try:
                 if v == column_max_length[k]:
                     logger.log(level=stream_level, msg="[column_size] for {k} passed.")
                 else:
                     logger.log(
                         level=stream_level,
-                        msg=f"[column_size] test for {k} failed. field lenght is different than {v}",
+                        msg=f"[column_size] test for {k} failed. field length is different than {v}",
                     )
                     failed_tests += 1
                     failed_tests_list.append("column_size error")
             except Exception as e:
                 logger.log(level=stream_level, msg=f"{e}")
-    except TypeError as e:
+    except TypeError:
         logger.log(
             level=stream_level,
             msg=f"Please provide `column_size` parameter as dictionary {'columns': value}.",
         )
 
 
 def validate_column_unique_values(
@@ -533,15 +531,15 @@
             )
 
 
 def validate_column_list_to_match(
     df, tests, logger, stream_level, failed_tests, failed_tests_list
 ):
     if set(tests["column_list_to_match"]) == set(df.columns):
-        logger.log(level=stream_level, msg=f"[column_list_to_match] passed.")
+        logger.log(level=stream_level, msg=f"{tests['column_list_to_match']} passed.")
     else:
         failed_tests += 1
         failed_tests_list.append("column_list_to_match error")
         logger.log(
             level=stream_level,
             msg="[column_list_to_match] failed. Columns are different than expected.",
         )
```

### Comparing `viadot2-2.0a22/src/viadot2.egg-info/PKG-INFO` & `viadot2-2.0a23/src/viadot2.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viadot2
-Version: 2.0a22
+Version: 2.0a23
 Summary: A simple data ingestion library to guide data flows from some places to other places.
 Author-email: acivitillo <acivitillo@dyvenia.com>, trymzet <mzawadzki@dyvenia.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: azure-core==1.25.0
 Requires-Dist: azure-storage-blob==12.13.1
@@ -29,21 +29,24 @@
 Requires-Dist: pandas-gbq==0.19.1
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: pydantic==1.10.11
 Requires-Dist: aiolimiter==1.0.0
 Requires-Dist: trino==0.326.*
 Requires-Dist: sqlalchemy==2.0.*
 Requires-Dist: minio<8.0,>=7.0
-Requires-Dist: databricks-connect==11.3.*
 Requires-Dist: azure-identity>=1.15.0
+Provides-Extra: databricks
+Requires-Dist: databricks-connect==11.3.*; extra == "databricks"
 
 # Viadot
+
 [![build status](https://github.com/dyvenia/viadot/actions/workflows/build.yml/badge.svg)](https://github.com/dyvenia/viadot/actions/workflows/build.yml)
 [![formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/Trymzet/dyvenia/branch/main/graph/badge.svg?token=k40ALkXbNq)](https://codecov.io/gh/Trymzet/dyvenia)
+
 ---
 
 **Documentation**: <a href="https://dyvenia.github.io/viadot/" target="_blank">https://dyvenia.github.io/viadot/</a>
 
 **Source Code**: <a href="https://github.com/dyvenia/viadot" target="_blank">https://github.com/dyvenia/viadot</a>
 
 ---
@@ -61,35 +64,42 @@
 ukci.query("/intensity")
 df = ukci.to_df()
 
 print(df)
 ```
 
 **Output:**
-|      | from              | to                | forecast | actual | index    |
+| | from | to | forecast | actual | index |
 | ---: | :---------------- | :---------------- | -------: | -----: | :------- |
-|    0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z |      211 |    216 | moderate |
+| 0 | 2021-08-10T11:00Z | 2021-08-10T11:30Z | 211 | 216 | moderate |
 
 The above `df` is a pandas `DataFrame` object. It contains data downloaded by `viadot` from the Carbon Intensity UK API.
 
 ## Loading Data to a Source
-Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
+Depending on the source, `viadot` provides different methods of uploading data. For instance, for SQL sources, this would be bulk inserts. For data lake sources, it would be a file upload. For ready-made pipelines including data validation steps using `dbt`, see [prefect-viadot](https://github.com/dyvenia/prefect-viadot).
 
 ## Getting started
+
 ### Prerequisites
-We assume that you have [Docker](https://www.docker.com/) installed.
+
+We assume that you have [Rye](https://rye-up.com/) installed:
+
+```console
+curl -sSf https://rye-up.com/get | bash
+```
 
 ### Installation
+
 Clone the `2.0` branch, and set up and run the environment:
-  ```sh
-  git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-    cd viadot/docker && \
-    sh update.sh  && \
-    sh run.sh && \
-    cd ../
-  ```
+
+```console
+git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
+  cd viadot && \
+  rye sync
+```
 
 ### Configuration
+
 In order to start using sources, you must configure them with required credentials. Credentials can be specified either in the viadot config file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to each source's `credentials` parameter.
 
 You can find specific information about each source's credentials in [the documentation](https://dyvenia.github.io/viadot/references/sql_sources/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viadot2 Version: 2.0a22 Summary: A simple data
+Metadata-Version: 2.1 Name: viadot2 Version: 2.0a23 Summary: A simple data
 ingestion library to guide data flows from some places to other places. Author-
 email: acivitillo
 dyvenia.com>, trymzet
 dyvenia.com> Requires-Python: >=3.10 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: azure-core==1.25.0 Requires-Dist: azure-
 storage-blob==12.13.1 Requires-Dist: awswrangler==2.19.0 Requires-Dist:
 s3fs==2022.11.0 Requires-Dist: boto3==1.24.59 Requires-Dist: pandas==1.4.4
@@ -11,40 +11,40 @@
 matplotlib>=3.8.3 Requires-Dist: adlfs==2022.9.1 Requires-Dist: Shapely==1.8.0
 Requires-Dist: imagehash==4.2.1 Requires-Dist: visions==0.7.5 Requires-Dist:
 sharepy<2.1.0,>=2.0.0 Requires-Dist: simple_salesforce==1.11.5 Requires-Dist:
 sql-metadata==2.3.0 Requires-Dist: duckdb==0.5.1 Requires-Dist: sendgrid==6.9.7
 Requires-Dist: pandas-gbq==0.19.1 Requires-Dist: pyyaml>=6.0.1 Requires-Dist:
 pydantic==1.10.11 Requires-Dist: aiolimiter==1.0.0 Requires-Dist:
 trino==0.326.* Requires-Dist: sqlalchemy==2.0.* Requires-Dist: minio<8.0,>=7.0
-Requires-Dist: databricks-connect==11.3.* Requires-Dist: azure-identity>=1.15.0
-# Viadot [![build status](https://github.com/dyvenia/viadot/actions/workflows/
-build.yml/badge.svg)](https://github.com/dyvenia/viadot/actions/workflows/
-build.yml) [![formatting](https://img.shields.io/badge/code%20style-black-
-000000.svg)](https://github.com/psf/black) [![codecov](https://codecov.io/gh/
-Trymzet/dyvenia/branch/main/graph/badge.svg?token=k40ALkXbNq)](https://
-codecov.io/gh/Trymzet/dyvenia) --- **Documentation**: _h_t_t_p_s_:_/_/
-_d_y_v_e_n_i_a_._g_i_t_h_u_b_._i_o_/_v_i_a_d_o_t_/ **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_y_v_e_n_i_a_/_v_i_a_d_o_t --
-- A simple data ingestion library to guide data flows from some places to other
-places. ## Getting Data from a Source Viadot supports several API and RDBMS
-sources, private and public. Currently, we support the UK Carbon Intensity
-public API and base the examples on it. ```python from
-viadot.sources.uk_carbon_intensity import UKCarbonIntensity ukci =
-UKCarbonIntensity() ukci.query("/intensity") df = ukci.to_df() print(df) ```
+Requires-Dist: azure-identity>=1.15.0 Provides-Extra: databricks Requires-Dist:
+databricks-connect==11.3.*; extra == "databricks" # Viadot [![build status]
+(https://github.com/dyvenia/viadot/actions/workflows/build.yml/badge.svg)]
+(https://github.com/dyvenia/viadot/actions/workflows/build.yml) [![formatting]
+(https://img.shields.io/badge/code%20style-black-000000.svg)](https://
+github.com/psf/black) [![codecov](https://codecov.io/gh/Trymzet/dyvenia/branch/
+main/graph/badge.svg?token=k40ALkXbNq)](https://codecov.io/gh/Trymzet/dyvenia)
+--- **Documentation**: _h_t_t_p_s_:_/_/_d_y_v_e_n_i_a_._g_i_t_h_u_b_._i_o_/_v_i_a_d_o_t_/ **Source Code**:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_y_v_e_n_i_a_/_v_i_a_d_o_t --- A simple data ingestion library to guide
+data flows from some places to other places. ## Getting Data from a Source
+Viadot supports several API and RDBMS sources, private and public. Currently,
+we support the UK Carbon Intensity public API and base the examples on it.
+```python from viadot.sources.uk_carbon_intensity import UKCarbonIntensity ukci
+= UKCarbonIntensity() ukci.query("/intensity") df = ukci.to_df() print(df) ```
 **Output:** | | from | to | forecast | actual | index | | ---: | :-------------
 --- | :---------------- | -------: | -----: | :------- | | 0 | 2021-08-10T11:
 00Z | 2021-08-10T11:30Z | 211 | 216 | moderate | The above `df` is a pandas
 `DataFrame` object. It contains data downloaded by `viadot` from the Carbon
 Intensity UK API. ## Loading Data to a Source Depending on the source, `viadot`
 provides different methods of uploading data. For instance, for SQL sources,
 this would be bulk inserts. For data lake sources, it would be a file upload.
 For ready-made pipelines including data validation steps using `dbt`, see
 [prefect-viadot](https://github.com/dyvenia/prefect-viadot). ## Getting started
-### Prerequisites We assume that you have [Docker](https://www.docker.com/
-) installed. ### Installation Clone the `2.0` branch, and set up and run the
-environment: ```sh git clone https://github.com/dyvenia/viadot.git -b 2.0 && \
-cd viadot/docker && \ sh update.sh && \ sh run.sh && \ cd ../ ``` ###
-Configuration In order to start using sources, you must configure them with
+### Prerequisites We assume that you have [Rye](https://rye-up.com/) installed:
+```console curl -sSf https://rye-up.com/get | bash ``` ### Installation Clone
+the `2.0` branch, and set up and run the environment: ```console git clone
+https://github.com/dyvenia/viadot.git -b 2.0 && \ cd viadot && \ rye sync ```
+### Configuration In order to start using sources, you must configure them with
 required credentials. Credentials can be specified either in the viadot config
 file (by default, `$HOME/.config/viadot/config.yaml`), or passed directly to
 each source's `credentials` parameter. You can find specific information about
 each source's credentials in [the documentation](https://dyvenia.github.io/
 viadot/references/sql_sources/).
```

### Comparing `viadot2-2.0a22/src/viadot2.egg-info/SOURCES.txt` & `viadot2-2.0a23/src/viadot2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `viadot2-2.0a22/src/viadot2.egg-info/requires.txt` & `viadot2-2.0a23/src/viadot2.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,11 @@
 pandas-gbq==0.19.1
 pyyaml>=6.0.1
 pydantic==1.10.11
 aiolimiter==1.0.0
 trino==0.326.*
 sqlalchemy==2.0.*
 minio<8.0,>=7.0
-databricks-connect==11.3.*
 azure-identity>=1.15.0
+
+[databricks]
+databricks-connect==11.3.*
```

