# Comparing `tmp/earthdaily-0.0.8.tar.gz` & `tmp/earthdaily-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthdaily-0.0.8.tar", last modified: Wed Feb 28 15:16:48 2024, max compression
+gzip compressed data, was "earthdaily-0.0.9.tar", last modified: Thu Feb 29 09:57:30 2024, max compression
```

## Comparing `earthdaily-0.0.8.tar` & `earthdaily-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.423289 earthdaily-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-28 15:16:47.000000 earthdaily-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-28 15:16:48.423289 earthdaily-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-28 15:16:47.000000 earthdaily-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.415289 earthdaily-0.0.8/earthdaily/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/accessor/
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/accessor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/datasets/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/datasets/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/datasets/data/pivot.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/datasets/data/pivot_corumba.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/earthdatastore/
--rw-r--r--   0 runner    (1001) docker     (127)    37000 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/_scales_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/_zonal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/custom_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/geometry_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/harmonizer/
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.423289 earthdaily-0.0.8/earthdaily/earthdatastore/mask/
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-02-28 15:16:47.000000 earthdaily-0.0.8/earthdaily/earthdatastore/mask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:16:48.419289 earthdaily-0.0.8/earthdaily.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-28 15:16:48.000000 earthdaily-0.0.8/earthdaily.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 15:16:48.423289 earthdaily-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-28 15:16:47.000000 earthdaily-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-29 09:57:29.000000 earthdaily-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-29 09:57:30.363389 earthdaily-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-29 09:57:29.000000 earthdaily-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.359389 earthdaily-0.0.9/earthdaily/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/accessor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/accessor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/datasets/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/pivot.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/datasets/data/pivot_corumba.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/
+-rw-r--r--   0 runner    (1001) docker     (127)    37000 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/_scales_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/_zonal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/custom_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/geometry_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily/earthdatastore/mask/
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-02-29 09:57:29.000000 earthdaily-0.0.9/earthdaily/earthdatastore/mask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:57:30.363389 earthdaily-0.0.9/earthdaily.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-29 09:57:30.000000 earthdaily-0.0.9/earthdaily.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 09:57:30.363389 earthdaily-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-29 09:57:29.000000 earthdaily-0.0.9/setup.py
```

### Comparing `earthdaily-0.0.8/LICENSE` & `earthdaily-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/PKG-INFO` & `earthdaily-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.0.8
+Version: 0.0.9
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_deptr7cn_/tmpxgcy5bvu_TarContainer/0/2", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.0.8 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.0.9 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.0.8/README.md` & `earthdaily-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/accessor/__init__.py` & `earthdaily-0.0.9/earthdaily/accessor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,30 +24,37 @@
 def _typer(raise_mistype=False):
     def decorator(func):
         def force(*args, **kwargs):
             _args = list(args)
             idx = 1
             for key, val in func.__annotations__.items():
                 is_kwargs = key in kwargs.keys()
-                if val not in _SUPPORTED_DTYPE or kwargs.get(key, None) is None and is_kwargs or len(args)==1:
+                if not is_kwargs and idx >= len(args):
                     continue
-                if raise_mistype and (val != type(kwargs.get(key)) if is_kwargs else val != type(args[idx])):
+                input_value = kwargs.get(key, None) if is_kwargs else args[idx]
+                if type(input_value) == val:
+                    continue
+                if raise_mistype and (
+                    val != type(kwargs.get(key))
+                    if is_kwargs
+                    else val != type(args[idx])
+                ):
                     if is_kwargs:
                         expected = f"{type(kwargs[key]).__name__} ({kwargs[key]})"
                     else:
                         expected = f"{type(args[idx]).__name__} ({args[idx]})"
 
                         raise MisType(
-                        f"{key} expected a {val.__name__}, not a {expected}."
-                    )
+                            f"{key} expected a {val.__name__}, not a {expected}."
+                        )
                 if is_kwargs:
                     kwargs[key] = val(kwargs[key]) if val != list else [kwargs[key]]
-                else:
+                elif len(args) >= idx:
                     _args[idx] = val(args[idx]) if val != list else [args[idx]]
-                idx+=1
+                idx += 1
             args = tuple(_args)
             return func(*args, **kwargs)
 
         return force
 
     return decorator
 
@@ -112,44 +119,51 @@
 
     img_weights = img_variance / (np.add(img_variance, overall_variance))
 
     img_output = img_mean + img_weights * (np.subtract(img, img_mean))
     img_output = xr.where(np.isnan(binary_nan), img_, img_output)
     return img_output
 
+
 @xr.register_dataarray_accessor("ed")
 class EarthDailyAccessorDataArray:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
-        
+
     def _max_time_wrap(self, wish=5):
-        return np.min((wish,self._obj['time'].size))
+        return np.min((wish, self._obj["time"].size))
 
     @_typer()
     def plot_band(self, cmap="Greys", col="time", col_wrap=5, **kwargs):
-        return self._obj.plot.imshow(cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs)
+        return self._obj.plot.imshow(
+            cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs
+        )
 
     @_typer()
     def plot_index(
         self, cmap="RdYlGn", vmin=-1, vmax=1, col="time", col_wrap=5, **kwargs
     ):
         return self._obj.plot.imshow(
-            vmin=vmin, vmax=vmax, cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs
+            vmin=vmin,
+            vmax=vmax,
+            cmap=cmap,
+            col=col,
+            col_wrap=self._max_time_wrap(col_wrap),
+            **kwargs,
         )
 
 
 @xr.register_dataset_accessor("ed")
 class EarthDailyAccessorDataset:
     def __init__(self, xarray_obj):
         self._obj = xarray_obj
 
     def _max_time_wrap(self, wish=5):
-        return np.min((wish,self._obj['time'].size))
-        
-    
+        return np.min((wish, self._obj["time"].size))
+
     @_typer()
     def plot_rgb(
         self,
         red: str = "red",
         green: str = "green",
         blue: str = "blue",
         col="time",
@@ -169,15 +183,20 @@
         )
 
     @_typer()
     def plot_index(
         self, index, cmap="RdYlGn", vmin=-1, vmax=1, col="time", col_wrap=5, **kwargs
     ):
         return self._obj[index].plot.imshow(
-            vmin=vmin, vmax=vmax, cmap=cmap, col=col, col_wrap=self._max_time_wrap(col_wrap), **kwargs
+            vmin=vmin,
+            vmax=vmax,
+            cmap=cmap,
+            col=col,
+            col_wrap=self._max_time_wrap(col_wrap),
+            **kwargs,
         )
 
     @_typer()
     def lee_filter(self, window_size: int = 7):
         return xr.apply_ufunc(
             _lee_filter,
             self._obj,
@@ -231,28 +250,31 @@
             ).data_vars
         )
         for v in data_vars:
             if v in _BAND_MAPPING.keys():
                 params[_BAND_MAPPING[v]] = self._obj[v]
         return params
 
-    def available_index(self, details=False):
+    def available_indices(self, details=False):
         mapper = list(self._auto_mapper().keys())
         indices = spyndex.indices
         available_indices = []
         for k, v in indices.items():
             needed_bands = v.bands
+            missing_bands = False
             for needed_band in needed_bands:
                 if needed_band not in mapper:
+                    missing_bands = True
                     break
+            if missing_bands is False:
                 available_indices.append(spyndex.indices[k] if details else k)
         return available_indices
 
     @_typer()
-    def add_index(self, index: list, **kwargs):
+    def add_indices(self, index: list, **kwargs):
         """
         Uses spyndex to compute and add index.
 
         For list of indices, see https://github.com/awesome-spectral-indices/awesome-spectral-indices.
 
 
         Parameters
```

### Comparing `earthdaily-0.0.8/earthdaily/datasets/__init__.py` & `earthdaily-0.0.9/earthdaily/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/datasets/data/pivot.geojson` & `earthdaily-0.0.9/earthdaily/datasets/data/pivot.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/datasets/data/pivot_corumba.geojson` & `earthdaily-0.0.9/earthdaily/datasets/data/pivot_corumba.geojson`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/__init__.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/_scales_collections.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/_scales_collections.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/__init__.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/_zonal.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/_zonal.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/__update_asset_mapper_config_json.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/asset_mapper/asset_mapper_config.json`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/custom_operations.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/custom_operations.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/geometry_manager.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/geometry_manager.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/harmonizer/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/cube_utils/preprocessing.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/cube_utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily/earthdatastore/mask/__init__.py` & `earthdaily-0.0.9/earthdaily/earthdatastore/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/earthdaily.egg-info/PKG-INFO` & `earthdaily-0.0.9/earthdaily.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthdaily
-Version: 0.0.8
+Version: 0.0.9
 Summary: earthdaily: easy authentication, search and retrieval of Earth Data Store collections data
 Home-page: UNKNOWN
 Author: EarthDaily Agro
 License: MIT
 Keywords: Earth Data Store,earthdaily,earthdailyagro,stac
 Platform: UNKNOWN
 Requires-Python: >=3.10
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_deptr7cn_/tmpxgcy5bvu_TarContainer/0/32", line 25, column 36: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: earthdaily Version: 0.0.8 Summary: earthdaily: easy
+Metadata-Version: 2.1 Name: earthdaily Version: 0.0.9 Summary: earthdaily: easy
 authentication, search and retrieval of Earth Data Store collections data Home-
 page: UNKNOWN Author: EarthDaily Agro License: MIT Keywords: Earth Data
 Store,earthdaily,earthdailyagro,stac Platform: UNKNOWN Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
 
 ************ EEaarrtthhDDaaiillyy PPyytthhoonn CClliieenntt ************
 Your gateway to the Earth Data Store STAC Catalog.
```

### Comparing `earthdaily-0.0.8/earthdaily.egg-info/SOURCES.txt` & `earthdaily-0.0.9/earthdaily.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthdaily-0.0.8/setup.py` & `earthdaily-0.0.9/setup.py`

 * *Files identical despite different names*

