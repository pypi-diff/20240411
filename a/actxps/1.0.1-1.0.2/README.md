# Comparing `tmp/actxps-1.0.1.tar.gz` & `tmp/actxps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actxps-1.0.1.tar", max compression
+gzip compressed data, was "actxps-1.0.2.tar", max compression
```

## Comparing `actxps-1.0.1.tar` & `actxps-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      293 2024-03-03 02:54:55.921744 actxps-1.0.1/actxps/__init__.py
--rw-r--r--   0        0        0        1 2023-03-19 11:56:28.947050 actxps-1.0.1/actxps/actxpspy.egg-info/dependency_links.txt
--rw-r--r--   0        0        0     9704 2023-03-19 11:56:28.946053 actxps-1.0.1/actxps/actxpspy.egg-info/PKG-INFO
--rw-r--r--   0        0        0       13 2023-03-19 11:56:28.949043 actxps-1.0.1/actxps/actxpspy.egg-info/requires.txt
--rw-r--r--   0        0        0      242 2023-03-19 11:56:28.971984 actxps-1.0.1/actxps/actxpspy.egg-info/SOURCES.txt
--rw-r--r--   0        0        0       17 2023-03-19 11:56:28.950044 actxps-1.0.1/actxps/actxpspy.egg-info/top_level.txt
--rw-r--r--   0        0        0     1811 2024-03-03 02:54:55.922743 actxps-1.0.1/actxps/col_select.py
--rw-r--r--   0        0        0   465054 2024-03-03 02:54:55.928726 actxps-1.0.1/actxps/data/account_vals
--rw-r--r--   0        0        0     9818 2024-03-03 02:54:55.929723 actxps-1.0.1/actxps/data/agg_sim_dat
--rw-r--r--   0        0        0   207333 2024-03-03 02:54:55.932714 actxps-1.0.1/actxps/data/census_dat
--rw-r--r--   0        0        0      502 2024-03-03 02:54:55.933712 actxps-1.0.1/actxps/data/create_data.py
--rw-r--r--   0        0        0     4368 2024-03-03 02:54:55.934711 actxps-1.0.1/actxps/data/qx_iamb.csv
--rw-r--r--   0        0        0     3667 2024-03-03 02:54:55.935706 actxps-1.0.1/actxps/data/scaleG2.csv
--rw-r--r--   0        0        0      125 2024-03-03 02:54:55.936704 actxps-1.0.1/actxps/data/toy_census.csv
--rw-r--r--   0        0        0   493948 2024-03-03 02:54:55.941690 actxps-1.0.1/actxps/data/withdrawals
--rw-r--r--   0        0        0     6765 2024-03-03 02:54:55.942689 actxps-1.0.1/actxps/datasets.py
--rw-r--r--   0        0        0    11237 2024-03-03 02:54:55.944683 actxps-1.0.1/actxps/dates.py
--rw-r--r--   0        0        0    45750 2024-03-03 02:54:55.945680 actxps-1.0.1/actxps/exp_shiny.py
--rw-r--r--   0        0        0    43502 2024-03-03 02:54:55.947675 actxps-1.0.1/actxps/exp_stats.py
--rw-r--r--   0        0        0    49143 2024-03-03 02:54:55.948673 actxps-1.0.1/actxps/expose.py
--rw-r--r--   0        0        0    10233 2024-03-03 02:54:55.950668 actxps-1.0.1/actxps/expose_split.py
--rw-r--r--   0        0        0    12039 2024-03-03 02:54:55.951665 actxps-1.0.1/actxps/tools.py
--rw-r--r--   0        0        0    40102 2024-03-03 02:54:55.952663 actxps-1.0.1/actxps/trx_stats.py
--rw-r--r--   0        0        0     1092 2024-03-03 02:54:55.915760 actxps-1.0.1/LICENSE
--rw-r--r--   0        0        0     1787 2024-03-03 13:35:26.714934 actxps-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    14719 2024-03-03 13:12:08.589673 actxps-1.0.1/README.md
--rw-r--r--   0        0        0    15762 1970-01-01 00:00:00.000000 actxps-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      293 2024-03-03 02:54:55.921744 actxps-1.0.2/actxps/__init__.py
+-rw-r--r--   0        0        0        1 2023-03-19 11:56:28.947050 actxps-1.0.2/actxps/actxpspy.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0     9704 2023-03-19 11:56:28.946053 actxps-1.0.2/actxps/actxpspy.egg-info/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-03-19 11:56:28.949043 actxps-1.0.2/actxps/actxpspy.egg-info/requires.txt
+-rw-r--r--   0        0        0      242 2023-03-19 11:56:28.971984 actxps-1.0.2/actxps/actxpspy.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0       17 2023-03-19 11:56:28.950044 actxps-1.0.2/actxps/actxpspy.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1811 2024-03-03 02:54:55.922743 actxps-1.0.2/actxps/col_select.py
+-rw-r--r--   0        0        0   465054 2024-03-03 02:54:55.928726 actxps-1.0.2/actxps/data/account_vals
+-rw-r--r--   0        0        0     9818 2024-03-03 02:54:55.929723 actxps-1.0.2/actxps/data/agg_sim_dat
+-rw-r--r--   0        0        0   207333 2024-03-03 02:54:55.932714 actxps-1.0.2/actxps/data/census_dat
+-rw-r--r--   0        0        0      502 2024-03-03 02:54:55.933712 actxps-1.0.2/actxps/data/create_data.py
+-rw-r--r--   0        0        0     4368 2024-03-03 02:54:55.934711 actxps-1.0.2/actxps/data/qx_iamb.csv
+-rw-r--r--   0        0        0     3667 2024-03-03 02:54:55.935706 actxps-1.0.2/actxps/data/scaleG2.csv
+-rw-r--r--   0        0        0      125 2024-03-03 02:54:55.936704 actxps-1.0.2/actxps/data/toy_census.csv
+-rw-r--r--   0        0        0   493948 2024-03-03 02:54:55.941690 actxps-1.0.2/actxps/data/withdrawals
+-rw-r--r--   0        0        0     6765 2024-03-03 02:54:55.942689 actxps-1.0.2/actxps/datasets.py
+-rw-r--r--   0        0        0    11237 2024-03-03 02:54:55.944683 actxps-1.0.2/actxps/dates.py
+-rw-r--r--   0        0        0    45750 2024-03-03 02:54:55.945680 actxps-1.0.2/actxps/exp_shiny.py
+-rw-r--r--   0        0        0    43502 2024-03-03 02:54:55.947675 actxps-1.0.2/actxps/exp_stats.py
+-rw-r--r--   0        0        0    49333 2024-04-11 14:30:29.355944 actxps-1.0.2/actxps/expose.py
+-rw-r--r--   0        0        0    10233 2024-03-03 02:54:55.950668 actxps-1.0.2/actxps/expose_split.py
+-rw-r--r--   0        0        0    12039 2024-03-03 02:54:55.951665 actxps-1.0.2/actxps/tools.py
+-rw-r--r--   0        0        0    40102 2024-03-03 02:54:55.952663 actxps-1.0.2/actxps/trx_stats.py
+-rw-r--r--   0        0        0     1092 2024-03-03 02:54:55.915760 actxps-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1727 2024-04-11 14:30:29.356943 actxps-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    14719 2024-03-03 14:37:45.472541 actxps-1.0.2/README.md
+-rw-r--r--   0        0        0    15762 1970-01-01 00:00:00.000000 actxps-1.0.2/PKG-INFO
```

### Comparing `actxps-1.0.1/actxps/actxpspy.egg-info/PKG-INFO` & `actxps-1.0.2/actxps/actxpspy.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/col_select.py` & `actxps-1.0.2/actxps/col_select.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/account_vals` & `actxps-1.0.2/actxps/data/account_vals`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/agg_sim_dat` & `actxps-1.0.2/actxps/data/agg_sim_dat`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/census_dat` & `actxps-1.0.2/actxps/data/census_dat`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/qx_iamb.csv` & `actxps-1.0.2/actxps/data/qx_iamb.csv`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/scaleG2.csv` & `actxps-1.0.2/actxps/data/scaleG2.csv`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/data/withdrawals` & `actxps-1.0.2/actxps/data/withdrawals`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/datasets.py` & `actxps-1.0.2/actxps/datasets.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/dates.py` & `actxps-1.0.2/actxps/dates.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/exp_shiny.py` & `actxps-1.0.2/actxps/exp_shiny.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/exp_stats.py` & `actxps-1.0.2/actxps/exp_stats.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/expose.py` & `actxps-1.0.2/actxps/expose.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,23 +348,28 @@
                  'cal_e': rename_col('cal', '_end')})
 
         else:
 
             data = data.with_columns(
                 cal_b=add_per(pl.col('issue_date'), pl.col('time') - 1),
                 cal_e=(add_per(pl.col('issue_date'), pl.col('time')).
-                       dt.offset_by('-1d')),
-                exposure=(pl.when(pl.col('last_per') & ~pl.col('status').
-                                  is_in(pl.Series(target_status,
-                                                  dtype=status_levels))).
-                          then(pl.col('tot_per') % 1).
-                          otherwise(1).
-                          # exposure = 0 is possible if exactly 1 period
-                          # has elapsed. replace these with 1's.
-                          replace(0, 1))
+                       dt.offset_by('-1d'))
+            ).with_columns(
+                exposure=(
+                    pl.when(pl.col('last_per') & ~pl.col('status').
+                            is_in(pl.Series(target_status,
+                                            dtype=status_levels))).
+                    then(((pl.col('last_date') -
+                           pl.col('cal_b')).dt.total_days() + 1) /
+                         ((pl.col('cal_e') -
+                           pl.col('cal_b')).dt.total_days() + 1)).
+                    otherwise(1).
+                    # exposure = 0 is possible if exactly 1 period
+                    # has elapsed. replace these with 1's.
+                    replace(0, 1))
             ).drop(
                 ['last_per', 'last_date', 'tot_per', 'rep_n']
             ).filter(
                 pl.col('cal_b') >= start_date,
                 pl.col('cal_b') <= end_date
             ).rename(
                 {'time': rename_col('pol'),
```

### Comparing `actxps-1.0.1/actxps/expose_split.py` & `actxps-1.0.2/actxps/expose_split.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/tools.py` & `actxps-1.0.2/actxps/tools.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/actxps/trx_stats.py` & `actxps-1.0.2/actxps/trx_stats.py`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/LICENSE` & `actxps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/pyproject.toml` & `actxps-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "actxps"
-version = "1.0.1"
+version = "1.0.2"
 description = "Create Actuarial Experience Studies: Prepare Data, Summarize Results, and Create Reports"
 authors = [
   "Matt Heaphy <mattrmattrs@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mattheaphy/actxpspy"
@@ -14,21 +14,21 @@
 python = ">=3.10"
 numpy = ">=1.26.2"
 pandas = ">=2.1.4"
 plotnine = ">=0.12.4"
 joblib = ">=1.3.2"
 scipy = ">=1.11.4"
 matplotlib = ">=3.8.2"
-shiny = {version = ">=0.7.0"}
+shiny = ">=0.7.0"
 great-tables = ">=0.3.1"
-shinyswatch = {version = ">=0.4.2"}
-faicons = {version = ">=0.2.2"}
-scikit-misc = {version = ">=0.3.1"}
+shinyswatch = ">=0.4.2"
+faicons = ">=0.2.2"
+scikit-misc = ">=0.3.1"
 polars = ">=0.20.9"
-selenium = {version = "^4.18.1"}
+selenium = "^4.18.1"
 pyarrow = ">=15.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3"
 pytest-cov = ">=4.1.0"
```

### Comparing `actxps-1.0.1/README.md` & `actxps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `actxps-1.0.1/PKG-INFO` & `actxps-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actxps
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create Actuarial Experience Studies: Prepare Data, Summarize Results, and Create Reports
 Home-page: https://github.com/mattheaphy/actxpspy
 License: MIT
 Author: Matt Heaphy
 Author-email: mattrmattrs@gmail.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: actxps Version: 1.0.1 Summary: Create Actuarial
+Metadata-Version: 2.1 Name: actxps Version: 1.0.2 Summary: Create Actuarial
 Experience Studies: Prepare Data, Summarize Results, and Create Reports Home-
 page: https://github.com/mattheaphy/actxpspy License: MIT Author: Matt Heaphy
 Author-email: mattrmattrs@gmail.com Requires-Python: >=3.10 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: faicons (>=0.2.2) Requires-Dist: great-tables (>=0.3.1)
```

