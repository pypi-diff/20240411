# Comparing `tmp/xesmf-0.8.4.tar.gz` & `tmp/xesmf-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xesmf-0.8.4.tar", last modified: Fri Feb 23 21:57:53 2024, max compression
+gzip compressed data, was "xesmf-0.8.5.tar", last modified: Thu Apr 11 21:00:38 2024, max compression
```

## Comparing `xesmf-0.8.4.tar` & `xesmf-0.8.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:57:53.471840 xesmf-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-02-23 21:57:44.000000 xesmf-0.8.4/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-23 21:57:44.000000 xesmf-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-23 21:57:44.000000 xesmf-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-02-23 21:57:53.471840 xesmf-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-02-23 21:57:44.000000 xesmf-0.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-23 21:57:44.000000 xesmf-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-23 21:57:44.000000 xesmf-0.8.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 21:57:53.471840 xesmf-0.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:57:53.467840 xesmf-0.8.4/xesmf/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20144 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    52494 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/smm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:57:53.471840 xesmf-0.8.4/xesmf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    35542 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/test_frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/test_oceanmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/test_smm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-02-23 21:57:44.000000 xesmf-0.8.4/xesmf/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 21:57:53.471840 xesmf-0.8.4/xesmf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-23 21:57:53.000000 xesmf-0.8.4/xesmf.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:38.880843 xesmf-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-04-11 21:00:33.000000 xesmf-0.8.5/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-11 21:00:33.000000 xesmf-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 21:00:33.000000 xesmf-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-11 21:00:38.880843 xesmf-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-11 21:00:33.000000 xesmf-0.8.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-11 21:00:33.000000 xesmf-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-11 21:00:33.000000 xesmf-0.8.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 21:00:38.880843 xesmf-0.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:38.876843 xesmf-0.8.5/xesmf/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20144 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53829 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9605 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/smm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:38.880843 xesmf-0.8.5/xesmf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36379 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/test_oceanmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/test_smm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-04-11 21:00:33.000000 xesmf-0.8.5/xesmf/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:00:38.880843 xesmf-0.8.5/xesmf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-11 21:00:38.000000 xesmf-0.8.5/xesmf.egg-info/SOURCES.txt
```

### Comparing `xesmf-0.8.4/CHANGES.rst` & `xesmf-0.8.5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 What's new
 ==========
 
+0.8.5 (2024-04-11)
+------------------
+* Reverted to the chunking behaviour of xESMF 0.7 for cases where the spatial dimensions are not chunked on the source data. (:pull:`348`) By `Pascal Bourgault <https://github.com/aulemahal>`_.
+
 0.8.4 (2024-02-26)
 ------------------
 * Fix regression from :pull:`332` that made ``Regridder`` fail with rectilinear datasets and ``parallel=True``. (:issue:`343`, :pull:`344`).
 * Allow Python 3.12 (and higher) again. (:pull:`345).
 
 0.8.3 (2024-02-20)
 ------------------
 * Remove usage of private method of xarray that was removed in its 2024.02.0 version (:issue:`338`, :issue:`340`) By `Pascal Bourgault <https://github.com/aulemahal>`_.
 
 Internal changes
-----------------
+~~~~~~~~~~~~~~~~
 * Test against ESMF 8.6
 
+
 0.8.2 (2023-09-18)
 ------------------
 
 Bug fixes
 ~~~~~~~~~
 * Raise a meaningful error messages when the output grid has no chunks with `parallel=True` (:issue:`299`, :pull:`304`). By `Pascal Bourgault <https://github.com/aulemahal>`_.
 * Correct guess of output chunks for ``SpatialAverager``.
```

### Comparing `xesmf-0.8.4/LICENSE` & `xesmf-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/PKG-INFO` & `xesmf-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xesmf
-Version: 0.8.4
+Version: 0.8.5
 Summary: Universal Regridder for Geospatial Data
 Author-email: Jiawei Zhuang <jiaweizhuang@g.harvard.edu>
 License: MIT
 Project-URL: documentation, https://xesmf.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/pangeo-data/xESMF
 Project-URL: repository, https://github.com/pangeo-data/xESMF
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xesmf-0.8.4/README.rst` & `xesmf-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/pyproject.toml` & `xesmf-0.8.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/backend.py` & `xesmf-0.8.5/xesmf/backend.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/data.py` & `xesmf-0.8.5/xesmf/data.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/frontend.py` & `xesmf-0.8.5/xesmf/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,19 +493,22 @@
             the output value is set to NaN. For instance, if `na_thres` is set
             to 0, the output value is NaN if a single NaN is found in the input
             values that are used to compute the output value; similarly,
             if `na_thres` is set to 1, all input values must be missing to
             mask the output value.
 
         output_chunks: dict or tuple, optional
-            If indata is a dask_array_type, the desired chunks to have on the
-            output data along the spatial axes. Other non-spatial axes inherit
-            the same chunks as indata as those are not affected by the application
-            of the weights. Default behavior is to have the outdata chunks be like
-            the indata chunks. Chunks have to be specified for all spatial dimensions
+            The desired chunks to have on the output along the spatial axes, if indata is a dask array.
+            Other non-spatial axes inherit the same chunks as indata.
+            Default behavior depends on the chunking of indata. If it is not chunked along
+            the spatial dimension, the output will also not be chunked,
+            equivalent to passing ``output_chunks=(-1, -1)``.
+            If it is chunked, the output will preserve the chunk sizes,
+            equivalent to passing ``output_chunks=ìndata.chunks``.
+            Chunks have to be specified for all spatial dimensions
             of the output data otherwise regridding will fail. output_chunks can
             either be a tuple the same size as the spatial axes of outdata or it
             can be a dict with defined dims. If output_chunks is a dict, the
             keys must match the dims of the output grid passed when initializing this Regridder.
 
         Returns
         -------
@@ -589,17 +592,36 @@
         check_shapes(indata, weights, **kwargs)
 
         kwargs.update(skipna=skipna, na_thres=na_thres)
 
         weights = self.weights.data.reshape(self.shape_out + self.shape_in)
         if isinstance(indata, dask_array_type):  # dask
             if output_chunks is None:
+                # Default : same chunk size as the input to preserve chunksize
+                # Unless the input is not chunked along the dimension (shape_in == in_chunk_size), in which case we do not chunk along the dimension
+                # This preserves the pre-0.8 behaviour.
                 output_chunks = tuple(
-                    [min(shp, inchnk) for shp, inchnk in zip(self.shape_out, indata.chunksize[-2:])]
+                    min(chnkin, shpout) if shpin != chnkin else shpout
+                    for shpout, shpin, chnkin in zip(
+                        self.shape_out, self.shape_in, indata.chunksize[-2:]
+                    )
                 )
+                fac = np.prod(
+                    [np.ceil(shp / chnk) for shp, chnk in zip(self.shape_out, output_chunks)]
+                )
+                if fac > 4:  # Dask's built-in threshold is 10
+                    warnings.warn(
+                        (
+                            f'Regridding is increasing the number of chunks by a factor of {fac}, '
+                            'you might want to specify sizes in `output_chunks` in the regridder call. '
+                            f'Default behaviour is to preserve the chunk sizes from the input {indata.chunksize[-2:]}.'
+                        ),
+                        da.core.PerformanceWarning,
+                        stacklevel=3,
+                    )
             if len(output_chunks) != len(self.shape_out):
                 if len(output_chunks) == 1 and self.sequence_out:
                     output_chunks = (1, output_chunks[0])
                 else:
                     raise ValueError(
                         f'output_chunks must have same dimension as ds_out,'
                         f' output_chunks dimension ({len(output_chunks)}) does not '
```

### Comparing `xesmf-0.8.4/xesmf/smm.py` & `xesmf-0.8.5/xesmf/smm.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/tests/conftest.py` & `xesmf-0.8.5/xesmf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/tests/test_backend.py` & `xesmf-0.8.5/xesmf/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/tests/test_frontend.py` & `xesmf-0.8.5/xesmf/tests/test_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,31 +503,54 @@
 
 @pytest.mark.parametrize('scheduler', dask_schedulers)
 def test_regrid_dask(request, scheduler):
     # chunked dask array (no xarray metadata)
     scheduler = request.getfixturevalue(scheduler)
     regridder = xe.Regridder(ds_in, ds_out, 'conservative')
 
-    indata = ds_in_chunked['data4D'].data
-    # Use ridiculous small chunk size value to be sure it _isn't_ impacting computation.
-    with dask.config.set({'array.chunk-size': '1MiB'}):
-        outdata = regridder(indata)
+    indata = ds_in_chunked['data'].data
+    outdata = regridder(indata)
 
     assert dask.is_dask_collection(outdata)
 
     # lazy dask arrays have incorrect shape attribute due to last chunk
     assert outdata.shape == indata.shape[:-2] + horiz_shape_out
-    assert outdata.chunksize == indata.chunksize
 
-    # Check that the number of tasks hasn't exploded.
+    # Check that the number of tasks is as predicted
+    # ds_in has 1 chunk
+    # thus output also has 1 chunk (output is not chunked if input isn't)
+    # regridding adds 3 tasks, wrapping the weights adds 2
+    n_task_out = len(outdata.__dask_graph__().keys())
     n_task_in = len(indata.__dask_graph__().keys())
+    assert n_task_out == n_task_in + 5
+
+    # Use very small chunks
+    indata_chunked = indata.rechunk((5, 6))  # Now has 9 chunks (5, 6)
+    outdata = regridder(indata_chunked)
+    # This is the case where we preserve chunk size
+    assert outdata.chunksize == indata_chunked.chunksize
     n_task_out = len(outdata.__dask_graph__().keys())
-    assert (n_task_out / n_task_in) < 15
+    n_task_in = len(indata_chunked.__dask_graph__().keys())
+    # input has 9 chunks
+    # output has 16
+    # Regridding adds 2 * 9 * 16 + 16 + 64 (I'm not sure I fully understand how dasks sums at the end)
+    # Wrapping the weights adds 9 * 16 + 1
+    assert n_task_out == n_task_in + 513
+
+    # Prescribe chunks
+    outdata = regridder(indata, output_chunks=(-1, 12))
+    n_task_out = len(outdata.__dask_graph__().keys())
+    n_task_in = len(indata.__dask_graph__().keys())
+    # input has 1 chunks
+    # output has 2
+    # Regridding adds 2 * 1 * 2 + 2
+    # Wrapping the weights adds 1 * 2 + 1
+    assert n_task_out == n_task_in + 9
 
-    outdata_ref = ds_out['data4D_ref'].values
+    outdata_ref = ds_out['data_ref'].values
     rel_err = (outdata.compute() - outdata_ref) / outdata_ref
     assert np.max(np.abs(rel_err)) < 0.05
 
 
 @pytest.mark.parametrize('scheduler', dask_schedulers)
 def test_regrid_dask_to_locstream(request, scheduler):
     # chunked dask array (no xarray metadata)
@@ -558,15 +581,14 @@
     regridder = xe.Regridder(ds_in, ds_out, 'conservative')
 
     dr_in = ds_in_chunked['data4D']
     dr_out = regridder(dr_in)
     assert dask.is_dask_collection(dr_out)
 
     assert dr_out.data.shape == dr_in.data.shape[:-2] + horiz_shape_out
-    assert dr_out.data.chunksize == dr_in.data.chunksize
 
     # data over broadcasting dimensions should agree
     assert_almost_equal(dr_in.values.mean(axis=(2, 3)), dr_out.values.mean(axis=(2, 3)), decimal=10)
 
     # check metadata
     xr.testing.assert_identical(dr_out['time'], dr_in['time'])
     xr.testing.assert_identical(dr_out['lev'], dr_in['lev'])
```

### Comparing `xesmf-0.8.4/xesmf/tests/test_oceanmodels.py` & `xesmf-0.8.5/xesmf/tests/test_oceanmodels.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/tests/test_smm.py` & `xesmf-0.8.5/xesmf/tests/test_smm.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/tests/test_util.py` & `xesmf-0.8.5/xesmf/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `xesmf-0.8.4/xesmf/util.py` & `xesmf-0.8.5/xesmf/util.py`

 * *Files identical despite different names*

