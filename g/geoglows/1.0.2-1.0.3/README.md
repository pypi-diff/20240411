# Comparing `tmp/geoglows-1.0.2.tar.gz` & `tmp/geoglows-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoglows-1.0.2.tar", last modified: Tue Apr  9 21:02:08 2024, max compression
+gzip compressed data, was "geoglows-1.0.3.tar", last modified: Wed Apr 10 19:57:58 2024, max compression
```

## Comparing `geoglows-1.0.2.tar` & `geoglows-1.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.709809 geoglows-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-09 21:02:04.000000 geoglows-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-09 21:02:04.000000 geoglows-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 21:02:08.705809 geoglows-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-09 21:02:04.000000 geoglows-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows/_plots/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/format_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_bias_corrected.py
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_forecasts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plotly_retrospective.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/_plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/bias.py
--rw-r--r--   0 runner    (1001) docker     (127)    13365 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-09 21:02:04.000000 geoglows-1.0.2/geoglows/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 21:02:08.705809 geoglows-1.0.2/geoglows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 21:02:08.000000 geoglows-1.0.2/geoglows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 21:02:04.000000 geoglows-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 21:02:08.709809 geoglows-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 21:02:04.000000 geoglows-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:57:58.529936 geoglows-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-10 19:57:54.000000 geoglows-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-10 19:57:54.000000 geoglows-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 19:57:58.525936 geoglows-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-10 19:57:54.000000 geoglows-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:57:58.525936 geoglows-1.0.3/geoglows/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:57:58.525936 geoglows-1.0.3/geoglows/_plots/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/format_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/plotly_bias_corrected.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/plotly_forecasts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/plotly_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/plotly_retrospective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/_plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7939 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/bias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-10 19:57:54.000000 geoglows-1.0.3/geoglows/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:57:58.525936 geoglows-1.0.3/geoglows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 19:57:58.000000 geoglows-1.0.3/geoglows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-10 19:57:58.000000 geoglows-1.0.3/geoglows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:57:58.000000 geoglows-1.0.3/geoglows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-10 19:57:58.000000 geoglows-1.0.3/geoglows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 19:57:58.000000 geoglows-1.0.3/geoglows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-10 19:57:54.000000 geoglows-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:57:58.529936 geoglows-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-10 19:57:54.000000 geoglows-1.0.3/setup.py
```

### Comparing `geoglows-1.0.2/LICENSE` & `geoglows-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/PKG-INFO` & `geoglows-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.2/README.md` & `geoglows-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/format_tools.py` & `geoglows-1.0.3/geoglows/_plots/format_tools.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/plotly_bias_corrected.py` & `geoglows-1.0.3/geoglows/_plots/plotly_bias_corrected.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/plotly_forecasts.py` & `geoglows-1.0.3/geoglows/_plots/plotly_forecasts.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/plotly_helpers.py` & `geoglows-1.0.3/geoglows/_plots/plotly_helpers.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/plotly_retrospective.py` & `geoglows-1.0.3/geoglows/_plots/plotly_retrospective.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/_plots/plots.py` & `geoglows-1.0.3/geoglows/_plots/plots.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/analyze.py` & `geoglows-1.0.3/geoglows/analyze.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/bias.py` & `geoglows-1.0.3/geoglows/bias.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/data.py` & `geoglows-1.0.3/geoglows/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,17 +56,19 @@
             if len(date) == 8:
                 date = f'{date}00.zarr'
             elif len(date) == 10:
                 date = f'{date}.zarr'
             else:
                 raise ValueError('Date must be YYYYMMDD or YYYYMMDDHH format. Use dates() to view available data.')
         else:
-            dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)])
+            dates = sorted([x.split('/')[-1] for x in s3.ls(ODP_FORECAST_S3_BUCKET_URI)], reverse=True)
+            dates = [x.split('.')[0] for x in dates if x.endswith('.zarr')]  # ignore the index.html file
+            dates = [x.replace('00.zarr', '') for x in dates]
             if product_name == 'dates':
-                return dates
+                return pd.DataFrame(dict(dates=dates))
             date = dates[-1]
         s3store = s3fs.S3Map(root=f'{ODP_FORECAST_S3_BUCKET_URI}/{date}', s3=s3, check=False)
 
         df = xr.open_zarr(s3store).sel(rivid=reach_id).to_dataframe().round(2).reset_index()
 
         # rename columns to match the REST API
         if isinstance(reach_id, list):
```

### Comparing `geoglows-1.0.2/geoglows/streams.py` & `geoglows-1.0.3/geoglows/streams.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows/tables.py` & `geoglows-1.0.3/geoglows/tables.py`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/geoglows.egg-info/PKG-INFO` & `geoglows-1.0.3/geoglows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoglows
-Version: 1.0.2
+Version: 1.0.3
 Summary: Package for accessing data from the GEOGLOWS Hydrological Model
 Home-page: https://data.geoglows.org
 Author: Riley Hales PhD
 License: BSD 3-Clause Clear License
 Project-URL: Homepage, https://data.geoglows.org
 Project-URL: Documentation, https://geoglows.readthedocs.io
 Project-URL: Source, https://github.com/geoglows/pygeoglows
```

### Comparing `geoglows-1.0.2/geoglows.egg-info/SOURCES.txt` & `geoglows-1.0.3/geoglows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoglows-1.0.2/setup.py` & `geoglows-1.0.3/setup.py`

 * *Files identical despite different names*

