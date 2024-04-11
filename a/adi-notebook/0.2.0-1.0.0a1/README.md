# Comparing `tmp/adi_notebook-0.2.0-py3-none-manylinux1_x86_64.whl.zip` & `tmp/adi_notebook-1.0.0a1-py3-none-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,11 @@
-Zip file size: 42287 bytes, number of entries: 15
+Zip file size: 13316 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 17:08 adi_notebook/__init__.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Mar-20 22:42 adi_notebook/__main__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-21 22:03 adi_notebook/adi_dataset.py
 -rw-r--r--  2.0 unx      169 b- defN 24-Mar-20 22:48 adi_notebook/adi_notebook.py
--rw-r--r--  2.0 unx    69324 b- defN 24-Mar-29 07:49 adi_notebook/adi_proc.py
--rw-r--r--  2.0 unx    58472 b- defN 24-Mar-24 03:43 adi_notebook/adi_runner.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-05 18:55 adi_notebook/py.typed
--rw-r--r--  2.0 unx    34995 b- defN 24-Apr-11 18:46 adi_notebook/runner.py
--rw-r--r--  2.0 unx     6985 b- defN 24-Mar-29 07:07 adi_notebook/script.py
--rw-r--r--  2.0 unx     2326 b- defN 24-Mar-24 03:43 adi_notebook/script_new.py
--rw-r--r--  2.0 unx      133 b- defN 24-Mar-29 07:07 adi_notebook/custom_package/custom_import.py
--rw-r--r--  2.0 unx      289 b- defN 24-Apr-11 19:16 adi_notebook-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      106 b- defN 24-Apr-11 19:16 adi_notebook-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-11 19:16 adi_notebook-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1224 b- defN 24-Apr-11 19:16 adi_notebook-0.2.0.dist-info/RECORD
-15 files, 174205 bytes uncompressed, 40253 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx    47965 b- defN 24-Mar-21 22:22 adi_notebook/adi_proc.py
+-rw-r--r--  2.0 unx      246 b- defN 24-Mar-21 22:27 adi_notebook-1.0.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx      106 b- defN 24-Mar-21 22:27 adi_notebook-1.0.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Mar-21 22:27 adi_notebook-1.0.0a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      731 b- defN 24-Mar-21 22:27 adi_notebook-1.0.0a1.dist-info/RECORD
+9 files, 49399 bytes uncompressed, 12044 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -9,38 +9,20 @@
 
 Filename: adi_notebook/adi_notebook.py
 Comment: 
 
 Filename: adi_notebook/adi_proc.py
 Comment: 
 
-Filename: adi_notebook/adi_runner.py
+Filename: adi_notebook-1.0.0a1.dist-info/METADATA
 Comment: 
 
-Filename: adi_notebook/py.typed
+Filename: adi_notebook-1.0.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: adi_notebook/runner.py
+Filename: adi_notebook-1.0.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: adi_notebook/script.py
-Comment: 
-
-Filename: adi_notebook/script_new.py
-Comment: 
-
-Filename: adi_notebook/custom_package/custom_import.py
-Comment: 
-
-Filename: adi_notebook-0.2.0.dist-info/METADATA
-Comment: 
-
-Filename: adi_notebook-0.2.0.dist-info/WHEEL
-Comment: 
-
-Filename: adi_notebook-0.2.0.dist-info/top_level.txt
-Comment: 
-
-Filename: adi_notebook-0.2.0.dist-info/RECORD
+Filename: adi_notebook-1.0.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adi_notebook/adi_proc.py

```diff
@@ -9,18 +9,17 @@
 import numpy as np
 import sys
 import xarray as xr
 
 import dsproc3 as dsproc
 from adi_py import Process, ADILogger, SkipProcessingIntervalException
 # from .version import __version__
-# import uuid
+import uuid
 import pickle
 import pathlib
-from pathlib import Path
 import os
 
 import requests
 import copy
 import subprocess
 
 import argparse
@@ -30,262 +29,78 @@
 
 from collections.abc import Iterable
 from collections.abc import Mapping
 
 import pandas as pd
 
 from copy import deepcopy
-import dill
+
+# from adi_notebook.adi_dataset import AdiDataset, PrettyXarrayDataset
+
 
     
-class AdiDatasetList(list):
+class AdiDataset(list):
     """
     A data class to wrap the List[Dict[str, xr.Dataset]]
     e.g., self._ds_ins: List[Dict[str, xr.Dataset]] = []  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
     Since xr.Dataset is not very print friendly
     """
-
     def __init__(self, iterable):
-        self.iterable = iterable
-        iterable = [AdiDatasetDict(i) for i in iterable if iterable]
+        # TODO: validation required
+        if iterable:
+            for ds_per_iteration in iterable:
+                for k, v in ds_per_iteration.items():
+                    ds_per_iteration[k] = PrettyXarrayDataset(v)
         super().__init__(iterable)
 
-    def __repr__(self):
-        if self is []:
-            return super().__repr__()
-        
-        iterable = deepcopy(self.iterable)
-        for ds_per_iteration in iterable:
-            # ds_per_iteration = AdiDatasetDict(ds_per_iteration)
-            for k, v in ds_per_iteration.items():
-                ds_per_iteration[k] = PrettyXarrayDataset(v)
-                # ds_per_iteration[k] = xr.Dataset(v)
-        return iterable.__repr__()
-
-
-class AdiDatasetDict(dict):
-    """
-    A data class to wrap the Dict[str, xr.Dataset]
-    e.g., self._ds_ins: Dict[str, xr.Dataset] = {}  # {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}
-    Since xr.Dataset is not very print friendly
-    """
-    def __init__(self, dictionary):
-        self.dictionary = dictionary
-        super().__init__(dictionary)
-
-    def __repr__(self):
-        """
-        EXAMPLE:
-        {'met.b1': <XarrayDataset>({
-            "Coordinates": "['time']",
-            "Data variables": "['alt', 'lat', 'lon', 'met_temperature', 'qc_met_temperature']",
-            "dod_version": "met-b1-7.3"
-        })}
-        """
-        if self is {}:
-            return super().__repr__()
-        
-        dictionary = deepcopy(self.dictionary)
-        for k, v in dictionary.items():
-            dictionary[k] = PrettyXarrayDataset(v)
-            # ds_per_iteration[k] = xr.Dataset(v)
-        return dictionary.__repr__()
-
+# from xarray.core.formatting import *
+# from xarray.core.formatting import _calculate_col_width, _get_boolean_with_default
 DataVars = Mapping[Any, Any]
-class PrettyXarrayDataset:
-    """
-    Pretty printing xr.Dataset
+class PrettyXarrayDataset(xr.Dataset):
     """
+    Pretty printing xr.Dataset"""
     
-    def __init__(self, ds: xr.Dataset):
-        self.ds = ds
+    # def __init__(self, ds: xr.Dataset):
+    #     super().__init__(ds)
 
+    def __init__(self, 
+                 ds: xr.Dataset,                                                                                                                                        
+                 # could make a VariableArgs to use more generally, and refine these
+                 # categories
+                
+    ) -> None:
+        data_vars = ds.data_vars       
+        coords = ds.coords
+        attrs = ds.attrs
+        super().__init__(data_vars = data_vars,      
+                         coords = coords,
+                         attrs = attrs)
+
+    # TODO: got warning 
+    # "FutureWarning: xarray subclass PrettyXarrayDataset should explicitly define __slots__  cls = super().__new__(mcls, name, bases, namespace, **kwargs)"
+    # TODO: check xtending xarray using accessors: https://docs.xarray.dev/en/latest/internals/extending-xarray.html
     def __repr__(self):
         # return self.dataset_repr(self)
         # self.attrs = super().attrs
         # print("super().attrs")
         # print(super().attrs)
-        return f"<XarrayDataset>" + "(" + json.dumps(self.get_xrdataset_info(), indent=4)+ ")"
+        return f"<{str(self.__class__.__name__)}>" + "(" + json.dumps(self.get_xrdataset_info(), indent=4)+ ")"
 
     def get_xrdataset_info(self):
         # TODO: discuss what other fundamental info should be put here
-        ds = self.ds
-        attr_command_line = {"command_line": ds.attrs["command_line"] }
-        attr_dod_version = {"dod_version": ds.attrs["dod_version"] }
+        attr_command_line = {"command_line": self.attrs["command_line"] }
+        attr_dod_version = {"dod_version": self.attrs["dod_version"] }
         xr_dataset_info: dict = {
-            # "time range": (str(ds.time.data[0]).split(".")[0],str(ds.time.data[-1]).split(".")[0]),
-            "time range": f'({str(ds.time.data[0]).split(".")[0]}, {str(ds.time.data[-1]).split(".")[0]})',
-            "Coordinates": str(list(ds.coords)),
-            "Data variables": str(list(ds.data_vars)),            
+            "Coordinates": str(list(self.coords)),
+            "Data variables": str(list(self.data_vars)),            
             } 
         xr_dataset_info.update(attr_dod_version)
         return xr_dataset_info
 
 
-class ProcessStatus:
-    """Basic class representing the final process state."""
-
-    def __init__(self, logs: str=""):
-        self._logs = logs
-
-    @property
-    def succeeded(self) -> bool:
-        if self._logs:
-            final_log_lines = "\n".join(self._logs.splitlines()[-5:])
-        else:
-            final_log_lines = ""
-        return "successful" in final_log_lines
-
-    @property
-    def logs(self) -> str:
-        return self._logs
-    
-    def __repr__(self) -> str:
-        status = "Success" if self.succeeded else "Failed"
-        return f"ProcessStatus={status}"
-
-    def __bool__(self) -> bool:
-        return self.succeeded
-        
-
-class AdiRunner:  # TODO: better name?
-    # TODO: docstring
-
-    def __init__(self, pcm_process: str, site: str, facility: str, begin_date: str, end_date: str):
-        """TODO: write a docstring
-
-        Args:
-            pcm_process (str): The PCM Process name, e.g., 'aosccnsmpskappa'
-            site (str): The site where you want to run the process at.
-            facility (str): The facility you want to run the process at.
-            begin_date (str): The begin date of the process as a YYYYMMDD string.
-            end_date (str): The end date of the process as a YYYYMMDD string.
-        """
-
-        self._adi_process = ADI_Process(
-            pcm_name=pcm_process,
-            site=site,
-            facility=facility,
-            begin_date=begin_date,
-            end_date=end_date
-        )
-        """A wrapper around adi_py.Process which allows for the Process to be run in a jupyter notebook."""
-
-        self._site = site
-        self._facility = facility
-        self._begin_date = begin_date
-        self._end_date = end_date
-        self._pcm_name = pcm_process
-
-    def __repr__(self) -> str:
-        return f"<{self.__class__.__name__}>" + \
-                "(" + json.dumps(self._adi_process.get_pcm_info(), indent=4)+ ")"
-
-    def process(self, cached: bool = False, verbose: bool = True) -> ProcessStatus:
-        """Runs the process and creates retrieved, pre-transformed, post-transformed, and output datasets.
-
-        Args:
-            cached (bool, optional): TODO: write some text for this. Need to indicate how the cache works, limitations, etc. Defaults to False.
-            verbose (bool, optional): Flag to enable logging from ADI. Defaults to True.
-
-        Returns:
-            ProcessStatus: True if the processing succeeded, False if an error occurred.
-        """
-        # TODO: can set log level as well, instead of just one level of verbose
-        # TODO: testing if log properly when using cach
-        logs = self._adi_process.process(cached=cached)
-        status = ProcessStatus(logs)
-        if verbose:
-            print(status.logs)
-        return status        
-
-    @property
-    def input_datasets(self) -> list[dict[str, xr.Dataset]]:
-        # TODO: docstring
-        filepath = Path(self._adi_process.ds_ins_full_path)
-        if not filepath.is_file():
-            ADILogger.debug(f"{filepath} does not exist. ", 2)
-            raise OSError(f"Data not available. Run process() first.")    
-        data = self._adi_process._pickle_load_ds(filepath)
-        return AdiDatasetList(data)
-    
-    @property
-    def output_datasets(self) -> list[dict[str, xr.Dataset]]:
-        # TODO: docstring
-        filepath = Path(self._adi_process.ds_outs_full_path)
-        if not filepath.is_file():
-            ADILogger.debug(f"{filepath} does not exist. ", 2)
-            raise OSError(f"Data not available. Run process() first.")    
-        data = self._adi_process._pickle_load_ds(filepath)
-        return AdiDatasetList(data)
-    
-    @property
-    def transformed_datasets(self) -> list[dict[str, xr.Dataset]]:
-        # TODO: docstring
-        filepath = Path(self._adi_process.ds_transforms_full_path)
-        if not filepath.is_file():
-            ADILogger.debug(f"{filepath} does not exist. ", 2)
-            raise OSError(f"Data not available. Run process() first.")            
-        data = self._adi_process._pickle_load_ds(filepath)
-        return AdiDatasetList(data)
-
-    @property
-    def transform_pairs(self) -> list[tuple[str, str]]:
-        return self._adi_process._transform_pairs
-
-    def set_transform_pair(self, input_datastream: str, coordinate: str):
-        """
-        TODO: doc string
-        """
-        self._adi_process.set_transform_pair(input_datastream, coordinate)
-
-    def get_valid_transform_mappings(self, display_like_str: bool=False):    
-        """
-        return available input_datastream--coordinate pairs for transformation.
-        display_like in ["tuple", "str", "string"]
-        
-        EXAMPLE:
-        get_valid_transform_mappings()
-        >>
-        [('ceil.b1', 'half_min_grid'), ('ceil.b1', 'mapped'),
-        ('ceil.b1', 'half_min_grid'), ('met.b1', 'half_min_grid'),
-        ('sirs.b1', 'mapped'), ('1twrmr.c1', 'mapped')]
-
-        EXAMPLE:
-        get_valid_transform_mappings(display_like="str")
-        >>        
-        ['ceil.b1 +=> half_min_grid', 'ceil.b1+=>mapped',
-        'ceil.b1 +=> half_min_grid', 'met.b1+=>half_min_grid',
-        'sirs.b1 +=> mapped', '1twrmr.c1+=>mapped']
-        """
-        return self._adi_process.get_valid_transform_mappings(display_like_str)
-
-    def clear_transform_pairs(self):
-        """
-        Clear out all the transform paris. Note: Doesn't support target delete at the moment.
-        """
-        self._adi_process.clear_transform_pairs()
-
-    def set_custom_adi_hooks(self, hook_type: str, injected_func: callable, arg_mapping: Dict[str, str]):
-        """
-        mimic Adi_Process set_custom_adi_hooks
-        For custom adi hook
-        hook_type in ["injected_pre_transform_hook", "injected_process_data_hook"]
-        TODO: doc string
-        """
-        self._adi_process.set_custom_adi_hooks(hook_type, injected_func, arg_mapping)
-
-    def set_local_package_path(self, abs_path: str):
-        """
-        Add local package to path, e.g., to make local package resolvable.
-        """
-        self._adi_process.set_local_package_path(abs_path)
-        
-
-
 class ADI_Process(Process):
     """-----------------------------------------------------------------------------------------------------------------
     This class implements the pblhtdlrf_training_validation process using the new, XArray-based ADI library.  Please see
     https://adi-python.readthedocs.io/en/latest/examples.html for more examples on how to use this API.
     -----------------------------------------------------------------------------------------------------------------"""
 
     MISSING_VALUE = -9999
@@ -330,15 +145,15 @@
         # get process info
         self.process_info: dict = self.retrieve_process(self._pcm_name) 
         # get input datastream name(s)
         self.ds_in_names = self.get_input_datastreams(self.process_info)
         # get output datastream name(s)
         self.ds_out_names = self.get_output_datastreams(self.process_info)
         # get transform name(s)
-        self.coord_names = self.get_coordinate_systems(self.process_info)
+        self.ds_coord_names = self.get_coordinate_systems(self.process_info)
         
         self._ds_ins: List[Dict[str, xr.Dataset]] = []  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
         self._ds_transforms: List[Dict[str, xr.Dataset]] = []  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
         self._ds_outs: List[Dict[str, xr.Dataset]] =  []  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
         
         # self._ds_ins: AdiDataset = AdiDataset([])  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
         # self._ds_transforms: AdiDataset = AdiDataset([])  # [{'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}, {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2},]
@@ -347,298 +162,134 @@
         # TODO: make the structure of self.ds_ins and self.ds_outs more readable, 
         # proposing adding processing interval in-front
         # {
         #   {"HH:mm:ss-HH:mm:ss": {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}},
         #   {"HH:mm:ss-HH:mm:ss": {'co2flx25m.b1': ds1, 'dlprofwstats4news.c1': ds2}},
         #   ...
         # }
-        # TODO: discuss the path connection: <userhome>/.adi_tmp/<pcm-name>/ 
+        # TODO: discuss the path conention: <userhome>/.adi_tmp/<pcm-name>/ 
         # and file convention: <process_name>_<site>_<facility>_<begin_date>_<end_date>.pickle
         self.pickle_path = pathlib.Path(f'{self.ADI_TMP_DIR}/{self._pcm_name}')
         # self.ds_ins_pickle_name = f"ds_ins_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
         # self.ds_outs_pickle_name = f"ds_outs_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
 
         # environment variables
         self._adi_env_vars = {}
         self.config_adi_env_vars()
 
         # # transformation plan
         # transform_pairs = self._get_all_transformation_pairs()
-        self._transform_pairs: List[Tuple[str,str]] = []  # e.g., [('1twrmr.c1', 'mapped'), ('ceil.b1', 'half_min_grid')]
-
-        # For custom adi hooks
-        # self._custom_adi_hooks: Dict[str, callable] = {}
-        self._custom_adi_hooks: Dict[str, tuple] = {}  # keys: ["instance_id", "injected_pre_transform_hook", "injected_process_data_hook"]
-
-        # For dynamic import
-        # TODO: only support import xx.yy.zz now as a lib, will support from xx.yy import zz, as zz_2, from a file, etc.
-        self._dynamic_import_libs = []
-
-        # dump whatever needs to be dumped _persisted_dict
-        self._persisted_dict: dict = {}
-
-        # flag to tell whether run from command line/subprocess
-        self._run_from_command_line = None
-
-        # add local package to the path (assume from the script where load this package)
-        self.__package_path = None
-        
-
-    def _save_persisted_dict(self):
-        """
-        TODO: clean up: dump whatever needs to be dumped in a subprocess workflow
-        """
-        # mkdir to pickle path
-        self._mkdir(self.pickle_path)
-        # save ds_ins as pickle
-        persisted_dict = deepcopy(self._persisted_dict)
-        persisted_dict["instance_id"] = str(id(self))
-        self._dill_dump_var(self._persisted_dict_full_path, persisted_dict)
-
-    def _load_persisted_dict(self):
-        """
-        load persisted persisted_dict variables
-        """
-        if os.path.isfile(self._persisted_dict_full_path):
-            return self._dill_load_var(self._persisted_dict_full_path)
-        
+        self._transform_pairs: Dict[str, Tuple[str,str]]  # e.g., {'1twrmr.c1--mapped': ('1twrmr.c1', 'mapped'), 'ceil.b1--half_min_grid': ('ceil.b1', 'half_min_grid'),
 
     def get_pcm_info(self):
         # TODO: discuss what other fundamental info should be put here
-        # TODO: get PCM version !!!
         pcm_info: dict = {
             "pcm_name": self._pcm_name,
             "input_datastreams": self.ds_in_names,
             "output_datastreams": self.ds_out_names,
-            "coordinates": self.coord_names,
-            # "datastream_flags": list(self.ds_str_flags),
-            "valid_transformation_pairs": self.get_valid_transform_mappings(display_like_str=True)
+            "coordinates": self.ds_coord_names,
+            "datastream_flags": list(self.ds_str_flags),
+            "transformation_pairs": list(self._get_all_transformation_pairs().keys())
         } 
         # pcm_info.update({"ENV-VARS": self._adi_env_vars})
         return pcm_info
-
-    def get_pcm_info_as_table(self) ->pd.DataFrame:
-        """
-        Get a tabular formatted PCM info
-        EXAMPLE:
-              group          shape             out_ds                 out_var  \
-        0   ceil_b1  half_min_grid  adiregulargrid.c1        ceil_backscatter   
-        1   ceil_b1         mapped                                              
-        2   ceil_b1  half_min_grid  adiregulargrid.c1  ceil_laser_temperature   
-        3    met_b1  half_min_grid  adiregulargrid.c1         met_temperature   
-        4  twrmr_c1         mapped   adimappedgrid.c1       twrmr_temperature   
-
-                             name           dims                 in_ds  
-        0        ceil_backscatter  [time, range]             {ceil.b1}  
-        1          ceil_first_cbh         [time]             {ceil.b1}  
-        2  ceil_laser_temperature         [time]             {ceil.b1}  
-        3         met_temperature         [time]              {met.b1}  
-        4       twrmr_temperature         [time]  {sirs.b1, 1twrmr.c1}  
-        """
-        df = self._get_process_info_ret_field()
-        return df[["group", "shape", "out_ds", "out_var", "name", "dims", "in_ds"]]
-
-    def get_valid_transform_mappings(self, display_like_str: bool=False):
-        """
-        return available input_datastream--coordinate pairs for transformation.
-        display_like in ["tuple", "str", "string"]
-        
-        EXAMPLE:
-        get_valid_transform_mappings()
-        >>
-        [('ceil.b1', 'half_min_grid'), ('ceil.b1', 'mapped'),
-        ('ceil.b1', 'half_min_grid'), ('met.b1', 'half_min_grid'),
-        ('sirs.b1', 'mapped'), ('1twrmr.c1', 'mapped')]
-
-        EXAMPLE:
-        get_valid_transform_mappings(display_like="str")
-        >>        
-        ['ceil.b1 +=> half_min_grid', 'ceil.b1+=>mapped',
-        'ceil.b1 +=> half_min_grid', 'met.b1+=>half_min_grid',
-        'sirs.b1 +=> mapped', '1twrmr.c1+=>mapped']
-        """
-        df = self.get_pcm_info_as_table()
-        df_in_coord_pairs = df[["in_ds", "shape"]].explode("in_ds").drop_duplicates().reset_index(drop=True)
-        if display_like_str:
-            return (df_in_coord_pairs["in_ds"] + " +=> " + df_in_coord_pairs["shape"]).values.tolist()
-        else:
-            return df_in_coord_pairs.apply(lambda x: (x["in_ds"], x["shape"]), axis=1).values.tolist()
-
-    def get_transform_pairs(self, display_like_str: bool=False):
-        """
-        Get a list of transformation pairs
-
-        Note: since transformation is expensive, we ask the user to set transformation pairs manually
-
-        EXAMPLE:
-
-        """
-        if not self._transform_pairs:
-            return []
-        if display_like_str:
-            return [(ds_name + " +=> " + coord) for (ds_name, coord) in self._transform_pairs]
-        else:
-            return self._transform_pairs
-
-    def set_transform_pair(self, input_datastream: str, coordinate: str):
-        """
-        Set transform pair (one pair at a time)
-        Note: use clear_transform_pairs to delete. Doesn't support target delete at the moment.
-        """
-        # TODO: check if should log this. use print for now
-        # TODO: at 3 test scenario for the following three cases.
-        trans_pair = (input_datastream, coordinate)
-        if trans_pair not in self.get_valid_transform_mappings():
-            print(f"Transformation_pair: {trans_pair} is not a valid transformation pairs in {self.get_valid_transform_mappings()}.")
-            print("Cannot set transform pair")        
-        elif trans_pair in self._transform_pairs:
-            print(f"Transformation_pair: {trans_pair} already exists in {self._transform_pairs}.")
-            print("No transform pair added.")            
-        else:
-            self._transform_pairs.append(trans_pair)
-            print(f"Added transformation_pair: {trans_pair} to the list.")
-            print(f"Current Transformation_pair: {self._transform_pairs}.")
-
-        
-
-
-
-    def clear_transform_pairs(self):
-        """
-        Clear out all the transform paris. Note: Doesn't support target delete at the moment.
-        """
-        self._transform_pairs = []
-        print(f"Cleared all the transform pairs.")
-
-        
     
     def _group_2_dsname(self, group_name: str) -> str:
         """
         Helper function to map group name in pcm to datastream name, e.g., ceil_b1 -> ceil.b1
         """
         queries = self.process_info['ret']['queries']
         group_2_dsname: dict = {}
         for group, rules in queries.items():
             for rule in rules:
                 datastream_name = f"{rule['class']}.{rule['level']}"
-                if group_2_dsname.get(group):
-                    if datastream_name not in group_2_dsname.get(group):  # keep unique
-                        group_2_dsname[group].append(datastream_name)
-                else:
-                    group_2_dsname[group] = [datastream_name]
+                group_2_dsname[group] = datastream_name
         return group_2_dsname[group_name]
     
     def _get_process_info_ret_field_raw(self) -> pd.DataFrame:
         """
-        Helper function to get tabular formatted data of the process_info["ret"]["fields"]
+        Helper function to get tablular formatted data of the process_info["ret"]["fields"]
         """
         json_field = self.process_info["ret"]["fields"]
         return pd.DataFrame(json_field)
 
     def _get_process_info_ret_field(self) -> pd.DataFrame:
         """
-        Helper function to get processed tabular formatted data of the process_info["ret"]["fields"]
+        Helper function to get processed tablular formatted data of the process_info["ret"]["fields"]
         """
         ds = self._get_process_info_ret_field_raw()
         df_fields_2 = ds.copy()
         df_fields_2["out_str"] = df_fields_2.out.apply(lambda x: str(x)) 
         df_fields_2["out_dict"] = df_fields_2.out.apply(lambda x: x[0] if x else {})
         df_fields_2["out_ds"] = df_fields_2["out_dict"].apply(lambda x: x.get("d") if x else "")
         df_fields_2["out_var"] = df_fields_2["out_dict"].apply(lambda x: x.get("f") if x else "")
         df_fields_2["in_ds"] = df_fields_2["group"].apply(lambda x: self._group_2_dsname(x))
 
         return df_fields_2
         
     def get_transform_plan(self) -> pd.DataFrame:
         """
         Get information about the transformation plan based on
-        its associated input_datastream, coordinates/shape, and output_datastream
+        its associated input_datastream, coordiates/shape, and output_datasream
 
         EXAMPLE: 
                    in_ds          shape             out_ds                                       out_var  
             0  1twrmr.c1         mapped   adimappedgrid.c1                           [twrmr_temperature] 
             1    ceil.b1  half_min_grid  adiregulargrid.c1    [ceil_backscatter, ceil_laser_temperature] 
             2    ceil.b1         mapped                                                               [] 
             3     met.b1  half_min_grid  adiregulargrid.c1                             [met_temperature] 
         """
         df = self._get_process_info_ret_field()
         df_copy = df.copy()
         return df_copy.groupby(["in_ds", "shape", "out_ds"])["out_var"].apply(lambda x: list(x)).reset_index()
 
-    @property
-    def _package_path(self):
-        """
-        Used to resolve local import package
-        Side effect: set self._persisted_dict["package_path"]
+    def _get_all_transformation_pairs(self) -> dict:
         """
-        # TODO: this logic is too messy. needs clean up.
-        if not self._run_from_command_line:
-            if not self.__package_path:
-                package_path = os.path.dirname(__file__)
-            else:
-                package_path = self.__package_path
-            # self._persisted_dict["package_path"] = package_path
-            return package_path
-        else:
-            return self._persisted_dict.get("package_path")
+        Helper function to get all the transformed pairs defined by PCM, 
+        i.e., datastream names and the coordinate system that apply transformation accordingly
 
-    def set_local_package_path(self, abs_path: str):
-        """
-        Add local package to path, e.g., to make local package resolvable.
-        """
-        if not os.path.exists(abs_path):
-            raise FileNotFoundError(f"{abs_path} does not exists.")
-        self.__package_path = abs_path
-        self._persisted_dict["package_path"] = abs_path
-        sys.path.append(abs_path)
+        EXAMPLE:
+        {'1twrmr.c1--mapped': ('1twrmr.c1', 'mapped'),
+        'ceil.b1--half_min_grid': ('ceil.b1', 'half_min_grid'),
+        'ceil.b1--mapped': ('ceil.b1', 'mapped'),
+        'met.b1--half_min_grid': ('met.b1', 'half_min_grid')}
+        """
+        df = self.get_transform_plan()
+        transform_pair: dict = {}
+        for plan in df[["in_ds", "shape"]].values:
+            ds_name = plan[0]
+            corrd = plan[1]
+            transform_pair[ds_name + "--" + corrd] = tuple(plan)
+        return transform_pair
 
-    def _load_local_package_path(self):
-        """
-        Load and add local package
-        """
-        sys.path.append(self._package_path)
 
     @property
     def adi_env_vars(self):
         return self._adi_env_vars
 
     def __repr__(self):
         return self.__module__ + "." +\
               self.__class__.__name__ + "(" + json.dumps(self.get_pcm_info(), indent=4)+ ")"
 
     @property
     def ds_ins_full_path(self):
-        # TODO: discuss if ds_ins_full_path and other similar attributes should be hidden from the user and not defined as property
-        # Maybe rename it as _ds_ins_full_path but still keep as property, since the calculation can be encapsulated still
         ds_ins_pickle_name = f"ds_ins_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
         return os.path.join(self.pickle_path, ds_ins_pickle_name)     
 
     @property
     def ds_transforms_full_path(self):
         ds_transforms_pickle_name = f"ds_transforms_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
         return os.path.join(self.pickle_path, ds_transforms_pickle_name)   
     
     @property
     def ds_outs_full_path(self):
         ds_outs_pickle_name = f"ds_outs_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
         return os.path.join(self.pickle_path, ds_outs_pickle_name)     
-    
-    @property
-    def _custom_adi_hooks_full_path(self):
-        # ds_outs_pickle_name = f"ds_outs_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
-        custom_adi_hooks = "custom_adi_hooks.pickle"
-        return os.path.join(self.pickle_path, custom_adi_hooks)     
-
-    @property
-    def _persisted_dict_full_path(self):
-        # ds_outs_pickle_name = f"ds_outs_{self._pcm_name}_{self._site}_{self._facility}_{self._begin_date}_{self._end_date}.pickle"
-        persisted_dict = "persisted_dict.pickle"
-        return os.path.join(self.pickle_path, persisted_dict)     
 
-    def set_datastream_str_flag(self, ds_name: str, ds_str_flag: str):
+    def set_datasteam_str_flag(self, ds_name: str, ds_str_flag: str):
         """
         Wrapper on adi_py.process def set_datastream_flags(dsid: int, flags: int)
 
         The original allowed flags are
         identified below:
 
         - dsproc.DS_STANDARD_QC     = Apply standard QC before storing a dataset.
@@ -666,38 +317,38 @@
                                       variables when mapped to the output datasets.
     
         - dsproc.DS_SCAN_MODE       = Enable scan mode for datastream that are not
                                       expected to be continuous. This prevents warning
                                       messages from being generated when data is not
                                       found within a processing interval. Instead, a
                                       message will be written to the log file indicating
-                                      that the processing interval was skipped.
+                                      that the procesing interval was skipped.
     
         - dsproc.DS_OBS_LOOP        = Loop over observations instead of time intervals.
                                       This also sets the DS_PRESERVE_OBS flag.
     
         - dsproc.DS_FILTER_VERSIONED_FILES = Check for files with .v# version extensions
                                              and filter out lower versioned files. Files
                                              without a version extension take precedence.
 
         """
-        # TODO: make this method more user-friendly and pythonic and flexible (e.g., )
+        # TODO: make this method more user-friedly and pythonic and flexible (e.g., )
         # mechanism: set datastream-flag pair one at a time, and store at a dict-like self.ds_flags attribute,
         # then have the init_process_hook read through self.ds_flags then call the original def set_datastream_flags(dsid: int, flags: int)
         # note: def set_datastream_flags(dsid: int, flags: int) should be "private"
 
         # TODO: write value check for input. (i.e., ds_name, Q: can ds_name be output_datastream name?, flag)
-        # TODO: discuss naming, note: even it is set one-at-a-time, it should not be called add_datastream_flag, since it can take out flag as well.
+        
 
         if not self._ds_str_flags.get(ds_name):
             self._ds_str_flags[ds_name] = set([ds_str_flag]) # Note: make sure unique
         else:
             self._ds_str_flags[ds_name].add(ds_str_flag)
 
-    def set_datastream_int_flag(self, ds_name: str, ds_int_flag: int):
+    def set_datasteam_int_flag(self, ds_name: str, ds_int_flag: int):
         """
 
         """
         # TODO: make this method more user-friedly and pythonic and flexible (e.g., )
         # mechanism: set datastream-flag pair one at a time, and store at a dict-like self.ds_flags attribute,
         # then have the init_process_hook read through self.ds_flags then call the original def set_datastream_flags(dsid: int, flags: int)
         # note: def set_datastream_flags(dsid: int, flags: int) should be "private"
@@ -747,57 +398,20 @@
         "DS_ROLLUP_TRANS_QC": dsproc.DS_ROLLUP_TRANS_QC, # 64
         "DS_SCAN_MODE": dsproc.DS_SCAN_MODE, # 128
         "DS_OBS_LOOP": dsproc.DS_OBS_LOOP, #256
         # "DS_FILTER_VERSIONED_FILES": dsproc.DS_FILTER_VERSIONED_FILES  module 'dsproc3' has no attribute 'DS_FILTER_VERSIONED_FILES'
         }
         return ds_flag_str_2_int[str_flag]
 
-    # def set_sub_input_dataset(self):
-    #     pass
-
-
-    def set_custom_adi_hooks(self, hook_type: str, injected_func: callable, arg_mapping: Dict[str, str], 
-                             import_list: List = None, **kwargs):
-        """
-        For custom adi hook
-        hook_type in ["injected_pre_transform_hook", "injected_process_data_hook"]
-
-        TODO: need to handle dynamic import in a more elegant way (import list: only demo lib import here. Will support file import later)
-        TODO: need to handle user_data in a more elegant way
-        """
-        valid_injected_custom_hooks = ["injected_pre_transform_hook", "injected_process_data_hook"]
-        if hook_type not in valid_injected_custom_hooks:
-            raise Exception(f"hook_type {hook_type} not in valid injected hooks {valid_injected_custom_hooks}")
-        elif hook_type == "injected_pre_transform_hook":
-            self._custom_adi_hooks["injected_pre_transform_hook"] = (injected_func, arg_mapping)
-        else:
-            self._custom_adi_hooks["injected_process_data_hook"] = (injected_func, arg_mapping)
-
-        if import_list:
-            self._dynamic_import_libs += import_list
-            
-
-
-    def _instantiate_dynamic_import_libs(self):
+    def set_transform_rule(input_datastream_name: str, coordinate: str, how=None):
         """
-        TODO: only support import xx.yy.zz now as a lib, will support from xx.yy import zz, as zz_2, from a file, etc.
+        TODO: method to configure self._transform_pairs, then pass to the post_transform_hook
         TODO: add validation
         """
-        for lib in self._dynamic_import_libs:
-            try:
-                __import__(lib)
-            except ImportError as e:
-                print(e)
-            raise ImportError(e)
-
-
-
-
-
-
+        pass
 
     def init_process_hook(self):        
 
         # TODO: make an API entry point for the custom DSPROC redefinition 
         # custom DSPROC redefinition
         # self.pblhtsonde_dsid = self.get_dsid(self.DS_IN_PBLHTSONDE1MCFARL_C1)        
         # if self.pblhtsonde_dsid is None:            # This will terminate the process and also log an error to the process log            
@@ -813,65 +427,26 @@
     # def init_process_hook(self):
     #     """-------------------------------------------------------------------------------------------------------------
     #     This hook will will be called once just before the main data processing loop begins and before the initial
     #     database connection is closed.
     #     -------------------------------------------------------------------------------------------------------------"""
         
     #     # Here is an example of setting obs-based processing, which is controlled by ADI flags.  (Delete this stubbed
-    #     # out code if you do not need obs-based processing.)
+    #     # out code if you do not need obs-based procesing.)
 
     #     # Get the ADI dsid for one of your input datastreams
     #     # dsid = self.get_dsid(self.DS_IN_CO2FLX25M_B1)
 
     #     # dsid will be None if the datastream does not exist in ADI
     #     # if dsid is None:
     #         # This will terminate the process and also log an error to the process log
     #         # raise Exception(f'Could not find input dsid for { self.DS_IN_CO2FLX25M_B1 }')
 
     #     # Set the obs loop control flag for that input datastream
     #     # self.set_datastream_flags(dsid, dsproc.DS_OBS_LOOP)
-                
-    def _injected_adi_hook(self, hook_type: str):
-        """
-        To inject something like the following and call it.
-
-        hook_type in ["injected_pre_transform_hook", "injected_process_data_hook"]
-
-        def sub_input_dataset(arg1: xr.dataset, arg2: xr.dataset):
-            arg1[var1].data = arg1[var1].data * 2
-
-        sub_input_dataset(arg1=ds_1, arg2=ds2)
-
-        where injected_pre_transform_hook = self._custom_adi_hooks["injected_pre_transform_hook"]
-        injected_pre_transform_hook: tuple[callable, dict] == (<callable>, {"arg1": "ds_1_name", "arg2": "ds_2_name"})
-
-        Note: preferred a well-defined API, than a too flexible one: do not support arg other than valid datastream names.
-        """
-
-        if hook_type in ["injected_pre_transform_hook", "injected_process_data_hook"] and self._custom_adi_hooks.get(hook_type):
-            injected_custom_adi_hook = self._custom_adi_hooks[hook_type]
-        else:
-            return
-
-        callable_symbol: callable = injected_custom_adi_hook[0]
-        arg_mapping: Dict[str, str] = injected_custom_adi_hook[1]  # e.g., {"arg1": "ds_1", "arg2": "ds_2"}
-        # TODO validation here to check if the feed in datastream/datastream names are valid
-        
-        ds_combined_per_run = {}
-        ds_combined_per_run.update(self.ds_ins_per_run)
-        if hook_type == "injected_process_data_hook":
-            ds_combined_per_run.update(self.ds_transforms_per_run)
-            ds_combined_per_run.update(self.ds_outs_per_run)
-        if arg_mapping:
-            actual_arg_mapping: Dict[str, xr.Dataset] = {arg: ds_combined_per_run[ds_name] 
-                                                        for arg, ds_name in arg_mapping.items()}
-        else:
-            actual_arg_mapping = {}
-        
-        callable_symbol(**actual_arg_mapping)
         
 
     def pre_transform_hook(self, begin_date: int, end_date: int):
         """-------------------------------------------------------------------------------------------------------------
         This hook will be called once per processing interval just prior to data transformation,and after the retrieved
         observations are merged and QC is applied.
 
@@ -885,52 +460,42 @@
         # OR you can get the dataset by dsid (see init_process_hook example above) by calling
         # self.get_retrieved_dataset_by_dsid())
         # ds = self.get_retrieved_dataset(self.DS_IN_CO2FLX25M_B1)
 
         # Automatically get all the PCM-defined input datasets
         # TODO: need to handle get_retrieved_dataset vs. get_retrieved_datasets
         # TODO: need to handle observed dataset cannot be retrieved without setting set_datastream_flags
-        self.ds_ins_per_run: dict = {}  # all the input datastreams per process run
+        ds_ins_per_run: dict = {}  # all the input datastreams per process run
         for ds_in_name in self.ds_in_names:
-            # TODO: verify the retrieve rules, i.e., to make it more general/flexible, should we use get_retrieved_dataset or get_retrieved_datasets
+            # TODO: verify the retrive rules, i.e., to make it more general/flexible, should we use get_retrieved_dataset or get_retrieved_datasets
             ds = self.get_retrieved_dataset(ds_in_name)  
+            # ds = PrettyXarrayDataset(ds)
             # ds_ins_per_run[ds_in_name] = ds
             if ds:
                 ds_copy = ds.copy()  # note: it is important to have a deep-copy of it
             else:
                 ds_copy = ds
-            self.ds_ins_per_run[ds_in_name] = ds_copy
-        self._ds_ins.append(self.ds_ins_per_run)
+            ds_ins_per_run[ds_in_name] = ds_copy
+        self._ds_ins.append(ds_ins_per_run)
 
         # Dataset will be None if the datastream does not exist in ADI
         # if ds is None:
         #     # This will terminate the process and also log an error to the process log.  Only do this if this particular
         #     # datastream is required
         #     raise Exception(f'Could not find input datastream for { self.DS_IN_CO2FLX25M_B1 }')
 
         #     # As an alternative, you can throw SkipProcessingIntervalException to skip to the next processing interval
         #     # You can decide if this skip should be logged as a warning or an info to the log
         #     # ADILogger.info(f'Skipping processing interval because { self.DS_IN_CO2FLX25M_B1 } not found.')
         #     # raise SkipProcessingIntervalException(f'Could not find input datastream for { self.DS_IN_CO2FLX25M_B1 }')
 
         # Perform your work here...
 
-        # Inject custom hook
-        self._injected_adi_hook("injected_pre_transform_hook")
-        
-
-
         # Now you need to push any changes you made back to ADI
         # self.sync_datasets(ds)
-        for ds_name, ds in self.ds_ins_per_run.items():
-            self.sync_datasets(ds)
-          
-
-        x = 1
-        # self._custom_adi_hooks["pre_transformed_hook"]()
         
 
         # This is an example of adding a level 3 debug log via ADILogger (levels 1-4 are supported)
         ADILogger.debug("This is a micro debug statement, often used for printing values of variables.", 3)
         ADILogger.debug("I don't need to debug when hooks start and stop because this is done for me by the parent class!!", 3)
 
     def post_transform_hook(self, begin_date: int, end_date: int):
@@ -938,34 +503,36 @@
         This hook will be called once per processing interval just after data transformation, but before the output
         datasets are created.
 
         Args:
           begin_date (int): the begin time of the current processing interval
           end_date (int):   the end time of the current processing interval
         -------------------------------------------------------------------------------------------------------------"""
+        
+       
+        # ds_tranforms_per_run: dict = {}  # all the input datastreams per process run
+        # for ds_in_name in self.ds_in_names:
+        #     ds_tranforms_per_run[ds_in_name] = self.get_transformed_dataset(ds_in_name, self.ds_coord_names[0])
+        # self.ds_transforms.append(ds_tranforms_per_run)
+
+        # TODO: perform full cross paired transform is very expensive, consider use deafult transform method,
+        # transform how: all (all the paire), None (no transform), customer specified
 
-        self.ds_transforms_per_run: dict = {}  # all the input datastreams per process run
+        ds_transforms_per_run: dict = {}  # all the input datastreams per process run
         if not self._transform_pairs:
-            # raise SkipProcessingIntervalException("Skip post_transform_hook")
             return
-        for pair in self._transform_pairs:
+        for plan, pair in self._transform_pairs.items():
             ds = self.get_transformed_dataset(pair[0], pair[1])  # TODO: handle edge case of get_transformed_datasets later
+            # ds = PrettyXarrayDataset(ds)
             if ds:
                 ds_copy = ds.copy()  # note: it is important to have a deep-copy of it
             else:
-                ds_copy = ds     
-            plan_name = pair[0] + " +=> " + pair[1]
-            self.ds_transforms_per_run[plan_name] = ds_copy
-        self._ds_transforms.append(self.ds_transforms_per_run)
-
-        # # Now you need to push any changes you made back to ADI
-        # # self.sync_datasets(ds)
-        # # TODO: explore how transform data behaves. The sync_datasets for transform data might not be needed.
-        # for ds_name, ds in self.ds_transforms_per_run.items():
-        #     self.sync_datasets(ds)
+                ds_copy = ds        
+            ds_transforms_per_run[plan] = ds_copy
+        self._ds_transforms.append(ds_transforms_per_run)
 
         # This is an example of adding a level 3 debug log via ADILogger (levels 1-4 are supported)
         ADILogger.debug("This is a micro debug statement, often used for printing values of variables.", 3)
         ADILogger.debug("I don't need to debug when hooks start and stop because this is done for me by the parent class!!", 3)
 
     def process_data_hook(self, begin_date: int, end_date: int):
         """-------------------------------------------------------------------------------------------------------------
@@ -980,25 +547,26 @@
         # First get any output datasets that we need to modify (as an XArray dataset)
         # (Note that you can get the dataset by datastream_name by calling self.get_output_dataset(),
         # OR you can get the dataset by dsid (see init_process_hook example above) by calling
         # self.get_output_dataset_by_dsid())
         # ds = self.get_output_dataset(self.DS_OUT_KMPBLHTDLRF_C1)
 
         # Automatically get all the PCM-defined input datasets
-        self.ds_outs_per_run: dict = {}  # all the input datastreams per process run
+        ds_outs_per_run: dict = {}  # all the input datastreams per process run
         for ds_out_name in self.ds_out_names:
             ds = self.get_output_dataset(ds_out_name)
+            # ds = PrettyXarrayDataset(ds)
             # self.sync_datasets(ds)
             # ds_outs_per_run[ds_out_name] = ds
             if ds:
                 ds_copy = copy.deepcopy(ds)  # note: it is important to have a deep-copy of it
             else:
                 ds_copy = ds
-            self.ds_outs_per_run[ds_out_name] = ds_copy
-        self._ds_outs.append(self.ds_outs_per_run)
+            ds_outs_per_run[ds_out_name] = ds_copy
+        self._ds_outs.append(ds_outs_per_run)
 
         # Dataset will be None if the datastream does not exist in ADI
         
         # if ds is None:
         #     # This will terminate the process and also log an error to the process log.  Only do this if this particular
         #     # datastream is required
         #     raise Exception(f'Could not find output datastream for { self.DS_OUT_KMPBLHTDLRF_C1 }')
@@ -1006,36 +574,31 @@
         #     # As an alternative, you can throw SkipProcessingIntervalException to skip to the next processing interval
         #     # You can decide if this skip should be logged as a warning or an info to the log
         #     # ADILogger.info(f'Skipping processing interval because { self.DS_OUT_KMPBLHTDLRF_C1 } not found.')
         #     # raise SkipProcessingIntervalException(f'Could not find output datastream for { self.DS_OUT_KMPBLHTDLRF_C1 }')
         
         # Perform your work here...
 
-        # Inject custom hook
-        self._injected_adi_hook("injected_process_data_hook")
-
         # Now you need to push any changes you made back to ADI
         # self.sync_datasets(ds)
-        for ds_name, ds in self.ds_outs_per_run.items():
-            self.sync_datasets(ds)
         
 
         # This is an example of adding a level 3 debug log via ADILogger (levels 1-4 are supported) (levels 1-4 are supported)
         ADILogger.debug("This is a micro debug statement, often used for printing values of variables.", 3)
         ADILogger.debug("I don't need to debug when hooks start and stop because this is done for me by the parent class!!", 3)
         
     def finish_process_hook(self):
         """-----------------------------------------------------------------------
         This hook will be called once just after the main data processing loop finishes.  This function should be used
         to clean up any temporary files used.
 
         -----------------------------------------------------------------------"""
         pass
 
-        # Note: this hook is not per process-vise, but after all the process intervals are finished.
+        # Note: this hook is not per process-vise, but after all the process inverals are finished.
         # self.ds_ins
         # self.ds_outs
         self._save_ds()    
     
 
     def quicklook_hook(self, begin_date: int, end_date: int):
         """-------------------------------------------------------------------------------------------------------------
@@ -1045,15 +608,15 @@
             begin_date (int): the begin timestamp of the current processing interval
             end_date (int): the end timestamp of the current processing interval
         -------------------------------------------------------------------------------------------------------------"""
         # see adi_example1_py_newapi for an example implementation
         pass
 
     def run(self):
-        """override the parent method to prevent calling it directly."""
+        """overide the parent method to prevent calling it directly."""
         print("Warning. This method should not be called, especially from a Notebook environment")
 
     def _run(self) -> int:
         """-----------------------------------------------------------------------
         mimic the parent class def run method
         Returns:
             int: The processing status:
@@ -1099,99 +662,59 @@
         """
         Persist self.ds_ins and self.ds_outs based as pickle on certain naming convention
         """
         # mkdir to pickle path
         self._mkdir(self.pickle_path)
         # save ds_ins as pickle
         self._pickle_dump_ds(self.ds_ins_full_path, self._ds_ins)
-        # save ds_transforms as pickle
+        # save ds_trnasforms as pickle
         self._pickle_dump_ds(self.ds_transforms_full_path, self._ds_transforms) 
         # save ds_outs as pickle
         self._pickle_dump_ds(self.ds_outs_full_path, self._ds_outs)
 
-    def _save_custom_adi_hooks(self):
-        """
-        Persist self._custom_adi_hooks on certain naming convention
-        """
-        # mkdir to pickle path
-        self._mkdir(self.pickle_path)
-        # save ds_ins as pickle
-        custom_adi_hooks_w_id = deepcopy(self._custom_adi_hooks)
-        custom_adi_hooks_w_id["instance_id"] = str(id(self))
-        self._dill_dump_var(self._custom_adi_hooks_full_path, custom_adi_hooks_w_id)
-
     @staticmethod
     def _mkdir(path: pathlib.Path) -> bool:
         """
         Helper function to make dir, if exists skip. 
-        Return True if success."""
+        Return True if sucess."""
         try:
             path.mkdir(parents=True, exist_ok=True)
             return True
         except Exception as e:
             print(e)
             return False
 
-    def _pickle_dump_var(self, abs_file, var):
-        """
-        TODO: reuse _pickle_dump_ds to not breaking code. Unit test later"""
-        self._pickle_dump_ds(abs_file, var)
-
-    def _dill_dump_var(self, abs_file, var):
-        """
-        Note dill works better wth function object serialization than pickle"""
-        with open(abs_file, 'wb+') as f:
-                dill.dump(var, f) 
-                # dill.dump_session(var, f)            
-
-
-    def _pickle_load_var(self, abs_file):
-        # TODO: reuse _pickle_dump_ds to not breaking code. Unit test later"""
-        return self._pickle_load_ds(abs_file)
-    
-    def _dill_load_var(self, abs_file):
-        """
-        Note dill works better wth function object serialization than pickle"""
-        try:
-            with open(abs_file, 'rb+') as f:
-                var = dill.load(f)             
-            return var  
-        except Exception as e:
-            print(e)
-            # Don't skip silently
-            raise e
-
     @staticmethod
     def _pickle_dump_ds(abs_file, var):
         """
         TODO: this method needs to clean up. And bug exists."""
         # try:
         #     if not os.path.isfile(abs_file):
         #         f = open(abs_file, "x")
         #         f.close()
         #     # with open(abs_file, 'ab+') as f:
         #     #     pickle.dump(var, f)               
         #     with open(abs_file, 'wb+') as f:
         #         pickle.dump(var, f)               
         # except Exception as e:
         #     print(e)
-        #     # Don't skip silently
+        #     # Don't skep silently
         #     raise e
         with open(abs_file, 'wb+') as f:
                 pickle.dump(var, f)            
 
     @staticmethod
     def _pickle_load_ds(abs_file):
         try:
             with open(abs_file, 'rb+') as f:
                 var = pickle.load(f)             
             return var  
         except Exception as e:
             print(e)
-            # Don't skip silently
+            # Don't skep silently
             raise e
     
     @staticmethod
     def retrieve_process(proc_name):
         """
         Mimic create_adi
         ...
@@ -1304,115 +827,82 @@
         # TODO: try to return the exit value from _run() and feed to process()
         # TODO: explore with the idea to use dummy class rather than subprocess to invoke the async process.
         #  (maybe it is cleaner. e.g., --set_datastream_flags is too recursive)
         """
 
         # if cached==True and pickle dump files exist, then skip 
         if cached and os.path.isfile(self.ds_ins_full_path) and os.path.isfile(self.ds_outs_full_path) and os.path.isfile(self.ds_transforms_full_path):
-            return "process successful. (Cached==True)"
+            return
             
         # TODO: currently use `python <script_name>` style, consider to encapsulate into package in the future
         this_file_path = os.path.dirname(__file__)
         this_file_name = os.path.basename(__file__)
         this_file_absolute_path = os.path.join(this_file_path, this_file_name)
         command = f"python {this_file_absolute_path} " +\
                     f"-n {self._pcm_name} " +\
                     f"-s {self._site} " +\
                     f"-f {self._facility} " +\
                     f"-b {self._begin_date} " +\
                     f"-e {self._end_date} "
         command_split = command.split()  
-        # feed in datastream_flag info
         if self.ds_int_flags:
-            # command_pair = '"'
+            command_pair = '"'
             command_pair = ''
             for ds_name, int_flag in self.ds_int_flags.items():
                 command_pair = command_pair + ds_name+ " " 
                 command_pair = command_pair+ str(int_flag) + " " 
             # command_pair = command_pair + '"'
             command_split += ["--set_datastream_flags"]
             command_split += [command_pair]
-        # feed in transformation_pair info
-        if self._transform_pairs:
-            command_pair = ''
-            for ds_name, coord_name in self._transform_pairs:
-                command_pair = command_pair + ds_name+ " " 
-                command_pair = command_pair+ coord_name + " " 
-            command_split += ["--set_transform_pairs"]
-            command_split += [command_pair]
-
-        # feed in instance id
-        command_split += ["--instance_id"]
-        command_split += [str(id(self))]    
-
-        # dump custom_adi_hooks
-        # TODO: dump other info, e.g., user_data: dict
-        self._save_custom_adi_hooks()   
-
-        # add local package to path, if no explicitly added, add this file
-        
-        self._persisted_dict["package_path"] = self._package_path
-
-
-        # persist the dict for whatever needs to be dumped there (TODO: clean up)
-        self._save_persisted_dict()
-        # dynamic import
-
-        
-
 
         # feed in env-vars
         my_env = os.environ.copy()
+        my_env["testing_env_var"] = "tesing-env-var"  # testing
         
-        output = subprocess.run(command_split, env=my_env, capture_output=True)
-        return output.stdout.decode()
+        # Note: use subprocess.run to wait for the whole process to end, 
+        # adi output should print out on the terminal
+        # print("=============================")
+        # print("=============================")
+        # print(command_split)
+        # print("=============================")
+        # print("=============================")
+        subprocess.run(command_split, env=my_env) 
 
     def dry_run(pcm_name, site, facility):
         """
         TODO: method to check if the the process is valid with the associated parameters 
         """
         pass
 
     def get_ds_ins(self):
         """
         Get persisted ds_ins variables
         """
         if not os.path.isfile(self.ds_ins_full_path):
             raise Exception(f"{self.ds_ins_full_path} NOT exist. Run process() first.")
         # return self._pickle_load_ds(self.ds_ins_full_path)
-        return AdiDatasetList(self._pickle_load_ds(self.ds_ins_full_path))
+        return AdiDataset(self._pickle_load_ds(self.ds_ins_full_path))
 
     def get_ds_transforms(self):
         """
         Get persisted ds_transform variables
         """
         if not os.path.isfile(self.ds_transforms_full_path):  
             raise Exception(f"{self.ds_transforms_full_path} NOT exist. Run process() first.") 
-        # return self._pickle_load_ds(self.ds_transforms_full_path)
-        return AdiDatasetList(self._pickle_load_ds(self.ds_transforms_full_path))
+        return self._pickle_load_ds(self.ds_transforms_full_path)
+        # return AdiDataset(self._pickle_load_ds(self.ds_transforms_full_path))
 
     def get_ds_outs(self):
         """
         Get persisted ds_outs variables
         """
         if not os.path.isfile(self.ds_outs_full_path):
             raise Exception(f"{self.ds_outs_full_path} NOT exist. Run process() first.")
-        # return self._pickle_load_ds(self.ds_outs_full_path)
-        return AdiDatasetList(self._pickle_load_ds(self.ds_outs_full_path))
-
-    def get_custom_adi_hooks(self):
-        pass
-
-    def _load_custom_adi_hooks(self):
-        """
-        load persisted custom_adi_hooks variables
-        """
-        if os.path.isfile(self._custom_adi_hooks_full_path):
-            return self._dill_load_var(self._custom_adi_hooks_full_path)
-
+        return self._pickle_load_ds(self.ds_outs_full_path)
+        # return AdiDataset(self._pickle_load_ds(self.ds_outs_full_path))
 
     def  _get_retrieved_dataset(self):
         pass
         # TODO: just like run, get_retrieved_dataset cannot be called outside the run process/from init_hook to finish_hook, 
         # otherwise the cbind part will complain. (connection issue?) 
         # use a run_on_flag to control whether such methods can be called. 
         # (basically, it is method like dsproc.get_retrieved_dataset() causes the problem)
@@ -1424,15 +914,15 @@
                             LOGS_DATA="default",
                             CONF_DATA="default",
                             ADI_PY_MODE="development",
                             **kwargs
                         ):
         """
         TODO: develop validation check, e.g., figure out available options for ADI_PY_MODE
-        TODO: discuss if use "default" or None for signature default value
+        TODO: discuss if use "default" or None for signature deafult value
         """
         
         if DATASTREAM_DATA_OUT == "default":
             DATASTREAM_DATA_OUT = os.path.join(self.ADI_DATA_DIR, "datastream/")
         if QUICKLOOK_DATA == "default":
             QUICKLOOK_DATA = os.path.join(self.ADI_DATA_DIR, "quicklook/")
         if LOGS_DATA == "default":
@@ -1489,21 +979,15 @@
                         metavar="<BEGIN_DATE>",
                         help="begin date, e.g., 20100101")
     parser.add_argument("-e", "--end_date", action="store", type=str, required=True,
                         metavar="<END_DATE>",
                         help="end date, e.g., 20100102")
     parser.add_argument("--set_datastream_flags", action="store", type=str,
                         metavar="<list of datastream-flag pairs>",
-                        help="list of datastream-flag pairs, separate with space, e.g., ds-name-1 10 ds-name-2 8 ")
-    parser.add_argument("--set_transform_pairs", action="store", type=str,
-                        metavar="<list of datastream-coordinate pairs for transformation>",
-                        help="list of datastream-coordinate pairs for transformation, separate with space, e.g., met.b1 half_min_grid sirs.b1 mapped")
-    parser.add_argument("--instance_id", action="store", type=str,
-                        metavar="<instance id>",
-                        help="instance id. Way to make auth check")
+                        help="list of datastream-flag pairs, seperate with space, e.g., ds-name-1 10 ds-namee-2 8 ")
 
     args = parser.parse_args()
 
     return args
 
 def pairwise(iterable):
     """ use to organize ds_name ds_flag pair on command line
@@ -1536,42 +1020,15 @@
     # set environment variable
 
 
     # set flags
     flag_command = args.set_datastream_flags  # e.g., 'pblhtsonde1mcfarl.c1 258 pblhtsonde1mcfarl.c1xx 2 '
     if flag_command:
         for ds_name, int_flag in pairwise(flag_command.split()):
-            adi_process.set_datastream_int_flag(ds_name, int(int_flag))
-
-    # set transformation pairs
-    transform_pair_command = args.set_transform_pairs
-    if transform_pair_command:
-        for ds_name, coord in pairwise(transform_pair_command.split()):
-            adi_process.set_transform_pair(ds_name, coord)
-
-    # use instance id check to load pickles
-    instance_id_referenced = args.instance_id
-    # _load_custom_adi_hooks
-    pickled_custom_adi_hooks = adi_process._load_custom_adi_hooks()
-    if instance_id_referenced == pickled_custom_adi_hooks.get("instance_id"):
-        pickled_custom_adi_hooks.pop('instance_id', None)
-        adi_process._custom_adi_hooks = pickled_custom_adi_hooks
-    # _load_persisted_dict
-    pickled_persisted_dict = adi_process._load_persisted_dict()
-    if instance_id_referenced == pickled_persisted_dict.get("instance_id"):
-        pickled_persisted_dict.pop('instance_id', None)
-        adi_process._persisted_dict = pickled_persisted_dict
-
-    # pre init (based on whether or not running from command line)
-    adi_process._run_from_command_line = True
-
-    # load and add local package to path
-    adi_process._load_local_package_path()
-    
-
+            adi_process.set_datasteam_int_flag(ds_name, int(int_flag))
 
     adi_process._run()
 
 
 if __name__ == '__main__':
 
     main()
```

