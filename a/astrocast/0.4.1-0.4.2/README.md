# Comparing `tmp/astrocast-0.4.1.tar.gz` & `tmp/astrocast-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrocast-0.4.1.tar", max compression
+gzip compressed data, was "astrocast-0.4.2.tar", max compression
```

## Comparing `astrocast-0.4.1.tar` & `astrocast-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    35149 2024-02-19 12:18:59.762777 astrocast-0.4.1/LICENSE
--rw-r--r--   0        0        0        0 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/__init__.py
--rw-r--r--   0        0        0    91719 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/analysis.py
--rw-r--r--   0        0        0   160370 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/app_analysis.py
--rw-r--r--   0        0        0    34330 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/app_preparation.py
--rw-r--r--   0        0        0    39836 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/autoencoders.py
--rw-r--r--   0        0        0    65743 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/cli_interfaces.py
--rw-r--r--   0        0        0    65798 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/clustering.py
--rw-r--r--   0        0        0   100976 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/denoising.py
--rw-r--r--   0        0        0    67139 2024-02-19 12:18:59.762777 astrocast-0.4.1/astrocast/detection.py
--rw-r--r--   0        0        0    40447 2024-02-19 12:18:59.766777 astrocast-0.4.1/astrocast/helper.py
--rw-r--r--   0        0        0   121134 2024-02-19 12:18:59.766777 astrocast-0.4.1/astrocast/preparation.py
--rw-r--r--   0        0        0    17428 2024-02-19 12:18:59.766777 astrocast-0.4.1/astrocast/reduction.py
--rw-r--r--   0        0        0     3014 2024-02-19 12:18:59.858776 astrocast-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 astrocast-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 13:38:56.649018 astrocast-0.4.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/__init__.py
+-rw-r--r--   0        0        0   111566 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/analysis.py
+-rw-r--r--   0        0        0   160370 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/app_analysis.py
+-rw-r--r--   0        0        0    34330 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/app_preparation.py
+-rw-r--r--   0        0        0    44410 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/autoencoders.py
+-rw-r--r--   0        0        0    66413 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/cli_interfaces.py
+-rw-r--r--   0        0        0    74538 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/clustering.py
+-rw-r--r--   0        0        0   102072 2024-04-11 13:38:56.649018 astrocast-0.4.2/astrocast/denoising.py
+-rw-r--r--   0        0        0    67564 2024-04-11 13:38:56.653018 astrocast-0.4.2/astrocast/detection.py
+-rw-r--r--   0        0        0    34641 2024-04-11 13:38:56.653018 astrocast-0.4.2/astrocast/experiments.py
+-rw-r--r--   0        0        0    68378 2024-04-11 13:38:56.653018 astrocast-0.4.2/astrocast/helper.py
+-rw-r--r--   0        0        0   121844 2024-04-11 13:38:56.653018 astrocast-0.4.2/astrocast/preparation.py
+-rw-r--r--   0        0        0    23425 2024-04-11 13:38:56.653018 astrocast-0.4.2/astrocast/reduction.py
+-rw-r--r--   0        0        0     3014 2024-04-11 13:38:56.761018 astrocast-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3749 1970-01-01 00:00:00.000000 astrocast-0.4.2/PKG-INFO
```

### Comparing `astrocast-0.4.1/LICENSE` & `astrocast-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `astrocast-0.4.1/astrocast/analysis.py` & `astrocast-0.4.2/astrocast/analysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import traceback
 from collections import defaultdict
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Literal, Tuple, Union
 
 import dask.array as da
+import humanize
+from sklearn.preprocessing import LabelEncoder
 
 try:
     import napari
 except ImportError:
     logging.warning(
             f"napari is not installed, some of functionality regarding visualization will not work."
             f"Consider reinstalling astrocast with the 'video-player' extras activated or install napari"
@@ -89,14 +91,23 @@
         
         else:
             raise ValueError(f"please provide data as either np.ndarray or dask.array")
     
     def __len__(self):
         return self.Z
     
+    def __sizeof__(self):
+        
+        data = self.data
+        if isinstance(data, da.Array):
+            logging.warning(f"data represented as da.Array. Not sure about size!")
+            return 0
+        else:
+            return data.size * data.itemsize
+    
     def get_data(self, in_memory=False):
         
         if in_memory and isinstance(self.data, da.Array):
             return self.data.compute()
         
         else:
             return self.data
@@ -252,192 +263,194 @@
         axx["D"].set_xlabel("Frame number")
         axx["D"].set_ylabel("Average signal (AU)")
         
         return fig
 
 
 class Events(CachedClass):
-    """
-        The Events class manages and processes astrocytic events detected in timeseries calcium recordings. It provides
-        various functionalities such as loading, extending, filtering, and analyzing events.
+    
+    def __init__(
+            self, event_dir: Union[str, Path] = None, lazy: bool = True,
+            data: Union[np.ndarray, da.Array, str, Path, Video] = None,
+            loc: str = None, group: Union[str, int] = None, subject_id: Union[str, int] = None,
+            z_slice: Tuple[int, int] = None, index_prefix: str = None,
+            custom_columns: Union[list, Tuple, Literal['v_area_norm', 'v_ara_footprint', 'cx', 'cy']] = (
+                    "v_area_norm", "cx", "cy"), frame_to_time_mapping: Union[dict, list] = None,
+            frame_to_time_function: Callable = None, cache_path: Union[str, Path] = None, seed: int = 1
+            ):
+        """
+        Manages and processes astrocytic events detected in timeseries calcium recordings. This class offers
+        functionalities for loading, extending, filtering, and analyzing astrocytic event data, providing a comprehensive
+        interface for the examination of calcium imaging data.
+
+        This class interacts with event data primarily through a DataFrame that contains a variety of calculated properties
+        for each detected event. These properties facilitate detailed analysis and characterization of the events.
 
         Args:
-            event_dir: The directory or list of directories where event data is stored after event detection.
-            lazy: Flag to indicate if data should be loaded lazily.
-            data: The associated video data or path to it. If set to `infer`, attempts to automatically determine the video path.
-            loc: Location specification for loading data, applicable when data is a .h5 file.
-            group: Identifier for the group or condition to which the events belong.
+            event_dir: Directory or list of directories containing event data post-detection.
+            lazy: If set to True, loads data lazily.
+            data: Associated video data or path to it. Automatically determines the path if set to `infer`.
+            loc: Location specification for loading data, applicable for .h5 files.
+            group: Identifier for the group or condition of the events.
             subject_id: Identifier for the subject associated with the events.
-            z_slice: The frame range to consider for processing.
-            index_prefix: Prefix for indexing events. Useful in multi-file scenarios.
-            custom_columns: Additional columns to compute and include in the events DataFrame.
-            frame_to_time_mapping: Mapping from frame numbers to absolute time.
-            frame_to_time_function: Function to convert frame numbers to absolute time.
+            z_slice: Frame range for processing, specified as a tuple (start, end).
+            index_prefix: Prefix for event indexing in multi-file scenarios.
+            custom_columns: Additional columns to compute and include in the DataFrame.
+            frame_to_time_mapping: Maps frame numbers to absolute time.
+            frame_to_time_function Function to convert frame numbers to absolute time.
             cache_path: Path for caching processed data.
-            seed: Seed value for hash generation. Needs to stay consistent between runs of analysis for caching to work.
+            seed: Seed for hash generation, ensuring consistency between runs for cache usage.
 
         Features:
             - Load and preprocess event data from specified directories.
-            - Supports both single and multiple file loading.
-            - Extend event traces in time by their mean or edge footprint.
+            - Extend event traces temporally by mean or edge footprint.
             - Normalize and filter events based on specified criteria.
-            - Generate and visualize summary statistics, frequency distributions, and clustering results.
-
-        Example::
+            - Generate and visualize summary statistics and frequency distributions.
+            - Perform clustering analysis on event data.
 
-            from astrocast.analysis import Events
-            event_obj = Events('/your/event/dir')
+            DataFrame Columns:
+                - `z0`, `z1`: Start and end indices in the z-dimension, defining the Z-index bounds of the event.
+                - `x0`, `x1`, `y0`, `y1`: Coordinates that define the event's bounding box in the XY plane.
+                - `dz`, `dx`, `dy`: Dimensions of the bounding box, indicating depth (dz), width (dx), and height (dy).
+                - `v_length`: Length of the event in the z-dimension, calculated as z1 - z0.
+                - `v_diameter`: Diameter of the event, derived as sqrt(dx^2 + dy^2).
+                - `v_area`: Total area covered by the event, calculated from the count of z-indices where the event_id is present.
+                - `v_bbox_pix_num`: Total number of pixels within the bounding box, computed as dz * dx * dy.
+                - `mask`: Binary mask indicating the presence (1) or absence (0) of the event.
+                - `v_mask_centroid_local`: Local centroid coordinates of the event mask, normalized by the bounding box size in each dimension.
+                - `v_mask_axis_major_length`, `v_mask_axis_minor_length`: Lengths of the major and minor axes of the ellipse equivalent to the event mask.
+                - `v_mask_extent`: Ratio of pixels in the region to pixels in the total bounding box.
+                - `v_mask_solidity`: Proportion of the pixels in the convex hull that are also in the region, indicating the solidity of the event.
+                - `v_mask_area`: Number of pixels in the region, representing the event's area.
+                - `v_mask_equivalent_diameter_area`: Diameter of a circle with the same area as the region.
+                - `contours`: Contours extracted from each frame of the event, detailing the event's shape.
+                - `footprint`: 2D representation of the event, capturing its extent in the XY plane.
+                - `v_fp_<property>`: Properties such as centroid, eccentricity, perimeter calculated from the 2D footprint.
+                - `trace`: Average signal intensity of the event across the z-dimension.
+                - `v_max_height`: Peak signal intensity in the trace.
+                - `v_max_gradient`: Steepest gradient in the trace, indicating rapid changes in intensity.
+                - `noise_mask_trace`: Trace calculated from the noise mask area, helping to differentiate signal from noise.
+                - `v_noise_mask_mean`, `v_noise_mask_std`: Mean and standard deviation of the noise mask trace, characterizing noise.
+                - `v_signal_to_noise_ratio`, `v_signal_to_noise_ratio_fold`: Metrics assessing the quality of the signal relative to noise.
+                - `error`: Flag indicating any computational errors during property calculation..
 
+        Example:
+            >>> from astrocast.analysis import Events
+            >>> event_obj = Events('/your/event/dir')
         """
-    
-    def __init__(
-            self, event_dir: Union[str, Path, List[str]] = None, lazy: bool = True,
-            data: Union[np.ndarray, da.Array, str, Path, Video] = None,
-            loc: str = None, group: Union[str, int] = None, subject_id: Union[str, int] = None,
-            z_slice: Tuple[int, int] = None, index_prefix: str = None,
-            custom_columns: Union[list, Tuple, Literal['v_area_norm', 'v_ara_footprint', 'cx', 'cy']] = (
-                    "v_area_norm", "cx", "cy"), frame_to_time_mapping: Union[dict, list] = None,
-            frame_to_time_function: Union[Callable, list] = None, cache_path: Union[str, Path] = None, seed: int = 1
-            ):
         
         super().__init__(cache_path=cache_path)
         
         self.seed = seed
         self.z_slice = z_slice
         
-        if not isinstance(event_dir, list):  # single file support
+        if event_dir is None:
+            logging.warning("event_dir is None. Creating empty Events instance!")
+            self.event_map = None
+            self.num_frames, self.X, self.Y = None, None, None
+            self.events = None
+        
+        else:
             
-            if event_dir is None:
-                logging.warning("event_dir is None. Creating empty Events instance!")
-                self.event_map = None
-                self.num_frames, self.X, self.Y = None, None, None
-                self.events = None
+            event_dir = Path(event_dir)
+            self.event_dir = event_dir
+            if not event_dir.is_dir():
+                raise FileNotFoundError(f"cannot find provided event directory: {event_dir}")
             
-            else:
+            # load event map
+            event_map, event_map_shape, event_map_dtype = self.get_event_map(event_dir, lazy=lazy, z_slice=z_slice)
+            self.event_map = event_map
+            self.num_frames, self.X, self.Y = event_map_shape
+            
+            # create time map
+            # time_map, events_start_frame, events_end_frame = self.get_time_map(event_dir=event_dir, event_map=event_map)
+            
+            # load events
+            self.events = self._load_events(
+                    event_dir, z_slice=z_slice, index_prefix=index_prefix, custom_columns=custom_columns
+                    )
+            
+            # z slicing
+            if z_slice is not None:
+                z_min, z_max = z_slice
+                self.events = self.events[(self.events.z0 >= z_min) & (self.events.z1 <= z_max)]
                 
-                event_dir = Path(event_dir)
-                self.event_dir = event_dir
-                if not event_dir.is_dir():
-                    raise FileNotFoundError(f"cannot find provided event directory: {event_dir}")
-                
-                # load event map
-                event_map, event_map_shape, event_map_dtype = self.get_event_map(event_dir, lazy=lazy, z_slice=z_slice)
-                self.event_map = event_map
-                self.num_frames, self.X, self.Y = event_map_shape
-                
-                # create time map
-                # time_map, events_start_frame, events_end_frame = self.get_time_map(event_dir=event_dir, event_map=event_map)
-                
-                # load events
-                self.events = self._load_events(
-                        event_dir, z_slice=z_slice, index_prefix=index_prefix, custom_columns=custom_columns
+                # TODO how does this effect:  # - time_map, events_start_frame, events_end_frame  # - data  # - indices in the self.events dataframe
+            
+            self.z_range = (self.events.z0.min(), self.events.z1.max())
+            
+            # align time
+            if frame_to_time_mapping is not None or frame_to_time_function is not None:
+                self.events["t0"] = self._convert_frame_to_time(
+                        self.events.z0.tolist(), mapping=frame_to_time_mapping, function=frame_to_time_function
                         )
                 
-                # z slicing
-                if z_slice is not None:
-                    z_min, z_max = z_slice
-                    self.events = self.events[(self.events.z0 >= z_min) & (self.events.z1 <= z_max)]
-                    
-                    # TODO how does this effect:  # - time_map, events_start_frame, events_end_frame  # - data  # - indices in the self.events dataframe
-                
-                self.z_range = (self.events.z0.min(), self.events.z1.max())
-                
-                # align time
-                if frame_to_time_mapping is not None or frame_to_time_function is not None:
-                    self.events["t0"] = self._convert_frame_to_time(
-                            self.events.z0.tolist(), mapping=frame_to_time_mapping, function=frame_to_time_function
-                            )
-                    
-                    self.events["t1"] = self._convert_frame_to_time(
-                            self.events.z1.tolist(), mapping=frame_to_time_mapping, function=frame_to_time_function
-                            )
-                    
-                    self.events.dt = self.events.t1 - self.events.t0
-                
-                # add group columns
-                self.events["group"] = group
-                self.events["subject_id"] = subject_id
-                self.events["file_name"] = event_dir.stem
-            
-            # get data
-            if isinstance(data, (str, Path)):
-                
-                if data == "infer":
-                    parent = self.event_dir.parent
-                    root_guess = parent.joinpath(f"{self.event_dir.stem}")
-                    for suffix in (".h5", ".hdf5", ".tiff", ".tif", ".tdb"):
-                        
-                        video_path_guess = root_guess.with_suffix(suffix)
-                        if video_path_guess.exists():
-                            logging.info(f"inferring video file as: {video_path_guess}")
-                            data = video_path_guess
-                            break
-                    
-                    if data is None:
-                        logging.warning(f"unable to infer video path with {root_guess}.tiff/h5/tdb")
-                
-                if data is not None:
-                    self.data = Video(data, z_slice=z_slice, loc=loc)
-            
-            elif isinstance(data, (np.ndarray, da.Array)):
-                print("data instance is an np array")
-                if z_slice is not None:
-                    logging.warning("'data'::array > Please ensure array was not sliced before providing data flag")
+                self.events["t1"] = self._convert_frame_to_time(
+                        self.events.z1.tolist(), mapping=frame_to_time_mapping, function=frame_to_time_function
+                        )
                 
-                self.data = Video(data, z_slice=z_slice)
+                self.events.dt = self.events.t1 - self.events.t0
             
-            elif isinstance(data, Video):
-                
-                if z_slice is not None:
-                    logging.warning("'data'::Video > Slice manually during Video object initialization")
+            # add group columns
+            self.events["group"] = group
+            self.events["subject_id"] = subject_id
+            self.events["file_name"] = event_dir.stem
+        
+        # get data
+        if isinstance(data, (str, Path)):
+            
+            if data == "infer":
+                parent = self.event_dir.parent
+                root_guess = parent.joinpath(f"{self.event_dir.stem}")
+                for suffix in (".h5", ".hdf5", ".tiff", ".tif", ".tdb"):
+                    
+                    video_path_guess = root_guess.with_suffix(suffix)
+                    if video_path_guess.exists():
+                        logging.info(f"inferring video file as: {video_path_guess}")
+                        data = video_path_guess
+                        break
                 
-                self.data: Video = data
+                if data is None:
+                    logging.warning(f"unable to infer video path with {root_guess}.tiff/h5/tdb")
             
-            elif data is None:
-                self.data = None
+            if data is not None:
+                self.data = Video(data, z_slice=z_slice, loc=loc, lazy=lazy)
+        
+        elif isinstance(data, (np.ndarray, da.Array)):
+            print("data instance is an np array")
+            if z_slice is not None:
+                logging.warning("'data'::array > Please ensure array was not sliced before providing data flag")
             
-            else:
-                logging.warning(f"data is not a valid type ({type(data)}). Defaulting to None")
-                self.data = None
+            self.data = Video(data, z_slice=z_slice, lazy=lazy)
         
-        else:  # multi file support
+        elif isinstance(data, Video):
             
-            event_objects = []
-            for i in range(len(event_dir)):
-                event = Events(
-                        event_dir[i], data=data if not isinstance(data, list) else data[i],
-                        loc=loc if not isinstance(loc, list) else loc[i],
-                        z_slice=z_slice if not isinstance(z_slice, list) else z_slice[i],
-                        group=group if not isinstance(group, list) else group[i], lazy=lazy, index_prefix=f"{i}x",
-                        subject_id=i, custom_columns=custom_columns,
-                        frame_to_time_mapping=frame_to_time_mapping if not isinstance(frame_to_time_mapping, list) else
-                        frame_to_time_mapping[i],
-                        frame_to_time_function=frame_to_time_function if not isinstance(frame_to_time_function,
-                                                                                        list) else
-                        frame_to_time_function[i]
-                        )
-                
-                event_objects.append(event)
+            if z_slice is not None:
+                logging.warning("'data'::Video > Slice manually during Video object initialization")
             
-            self.event_objects = event_objects
-            self.events = pd.concat([ev.events for ev in event_objects])
-            self.events.reset_index(drop=False, inplace=True, names="idx")
-            self.z_slice = z_slice
+            self.data: Video = data
+        
+        elif data is None:
+            self.data = None
+        
+        else:
+            logging.warning(f"data is not a valid type ({type(data)}). Defaulting to None")
+            self.data = None
         
         if self.events is not None:
             # make categorical
             for col in ('file_name', 'subject_id', 'group'):
                 if col in self.events.columns:
                     self.events[col] = self.events[col].astype("category")
     
     def __len__(self):
         return len(self.events)
     
     def __getitem__(self, item):
-        return self.events.iloc[item]
+        return self.events[self.events.index == item].iloc[0]
     
     def __hash__(self):
         
         traces = self.events.trace
         
         hashed_traces = traces.apply(lambda x: xxhash.xxh64_intdigest(np.array(x), seed=self.seed))
         hash_ = xxhash.xxh64_intdigest(hashed_traces.values, seed=self.seed)
@@ -452,20 +465,14 @@
     #     dump(self, path)
     #
     # @staticmethod
     # def load(path):
     #     from joblib import load
     #     return load(path)
     
-    def _is_multi_subject(self):
-        if len(self.events.subject_id.unique()) > 1:
-            return True
-        else:
-            return False
-    
     def _is_ragged(self):
         return is_ragged(self.events.trace.tolist())
     
     def add_clustering(self, cluster_lookup_table: dict, column_name: str = "cluster") -> None:
         """
                 Adds a clustering column to the events DataFrame based on a provided lookup table.
 
@@ -515,54 +522,67 @@
         selected_metrics = [metrics.adjusted_rand_score, metrics.adjusted_mutual_info_score,
                             metrics.normalized_mutual_info_score, metrics.homogeneity_score, metrics.completeness_score,
                             metrics.v_measure_score, metrics.fowlkes_mallows_score]
         
         results = {f.__name__: np.round(f(groups, pred_groups), 2) for f in selected_metrics}
         return results
     
-    def get_counts_per_cluster(self, cluster_col: str, group_col: str = None) -> pd.DataFrame:
+    @wrapper_local_cache
+    def get_counts_per_cluster(self, cluster_col: str, group_col: str = None, z_slice: Tuple[int, int] = None,
+                               transpose: bool = False) -> (pd.DataFrame):
         """
                 Computes the counts of events per cluster, optionally grouped by an additional column.
 
                 This method calculates the frequency of events in each cluster. If a group column is provided, it calculates
                 the frequency of events in each cluster for each group.
 
                 Args:
                     cluster_col: The name of the column in the events DataFrame that contains cluster labels.
                     group_col: The name of the column by which to group counts. If provided, the method
                         returns counts per cluster for each group. If None, the method returns overall counts per cluster.
-
+                    z_slice: Frames to select for counting
+                    transpose: Flag to return transposed matrix
                 Returns:
                     pd.DataFrame: A DataFrame with counts of events. Each row represents a cluster. If group_col is provided, each column represents a group, otherwise there is a single column with total counts.
 
                 .. note::
 
                     This method is particularly useful for analyzing the distribution of events across different clusters and groups.
 
                 """
+        
+        events = self.events.copy()
+        
+        if z_slice is not None:
+            z0, z1 = z_slice
+            events = events[(events.z0 >= z0) & (events.z1 < z1)]
+        
         if group_col is None:
-            counts = self.events[cluster_col].value_counts()
+            counts = events[cluster_col].value_counts()
         
         else:
             
-            unique_clusters = self.events[cluster_col].unique()
+            unique_clusters = events[cluster_col].unique()
             lut_cluster = {c: i for i, c in enumerate(unique_clusters)}
             
-            unique_groups = self.events[group_col].unique()
+            unique_groups = events[group_col].unique()
             lut_groups = {g: i for i, g in enumerate(unique_groups)}
             
             counts = np.zeros(shape=(len(unique_clusters), len(unique_groups)), dtype=int)
             
-            for _, row in self.events.iterrows():
+            for _, row in events.iterrows():
                 x = lut_cluster[row[cluster_col]]
                 y = lut_groups[row[group_col]]
                 counts[x, y] += 1
             
             counts = pd.DataFrame(data=counts, index=unique_clusters, columns=unique_groups)
         
+        if transpose:
+            counts = counts.transpose()
+        
         return counts
     
     def plot_cluster_counts(
             self, counts: pd.DataFrame, normalize_instructions: dict = None, method: str = "average",
             metric: str = "euclidean", z_score: Literal[0, 1, None] = 0, center: Union[int, float] = 0,
             transpose: bool = False, color_palette: str = "viridis",
             group_cmap: Union[str, dict, Literal['auto']] = None, cmap: str = "vlag"
@@ -840,14 +860,44 @@
         events_start_frame = np.argmax(time_map, axis=0)
         
         # 1D array (num_events x frames) of event stop
         events_end_frame = time_map.shape[0] - np.argmax(time_map[::-1, :], axis=0)
         
         return time_map, events_start_frame, events_end_frame
     
+    @wrapper_local_cache
+    def get_time_map_by_cluster(self, cluster_column: str, show_progress: bool = True):
+        
+        events = self.events.copy()
+        
+        z1_max = events.z1.max()
+        unique_clusters = events[cluster_column].unique().tolist()
+        cluster_num = len(unique_clusters)
+        
+        if isinstance(events[cluster_column].tolist()[0], str):
+            label_encoder = LabelEncoder()
+            int_category = label_encoder.fit_transform(events[cluster_column])
+            unique_clusters = int_category.tolist()
+            cluster_column = "dummy_cluster_column"
+            events[cluster_column] = int_category
+        
+        time_map = np.zeros((z1_max, cluster_num), dtype=int)
+        iterator = tqdm(range(z1_max)) if show_progress else range(z1_max)
+        for z in iterator:
+            
+            selected = events[(events.z0 <= z) & (events.z1 > z)]
+            counts = selected[[cluster_column, "z0"]].groupby(cluster_column).count()
+            
+            for idx, row in counts.iterrows():
+                
+                tm_idx = unique_clusters.index(idx)
+                time_map[z, tm_idx] += row.z0
+        
+        return time_map
+    
     @staticmethod
     def _load_events(event_dir: Path, z_slice=None, index_prefix=None, custom_columns=("v_area_norm", "cx", "cy")):
         
         """
         Load events from the specified directory and perform optional preprocessing.
 
         Args:
@@ -938,20 +988,38 @@
             events = self.events
         
         if ragged:
             return np.array(events.trace.tolist())
         
         arr = np.zeros((len(events), self.num_frames))
         
-        for i, (z0, z1, trace) in enumerate(zip(events.z0, events.z1, events.trace)):
-            arr[i, z0:z1] = trace
+        for i, (idx, row) in enumerate(events.iterrows()):
+            z0, z1 = row.z0, row.z1
+            dz = z1 - z0
+            
+            trace = row.trace
+            dtrace = len(trace)
+            
+            if dz != dtrace:
+                logging.warning(f"z boundaries ({z0}, {z1}) does match trace length: {dtrace}. Skipping {idx}.")
+                continue
+            
+            if z0 < 0:
+                logging.warning(f"Encountered event with negative z0: {z0}. Skipping {idx}.")
+                continue
+            
+            try:
+                arr[i, z0:z1] = trace
+            except ValueError as err:
+                logging.warning(f"Encountered broadcast issue at {idx}. Skipping value. \n {err}")
         
-        # todo this should actually be a mask instead then; np.nan creates weird behavior
         if empty_as_nan:
-            arr[arr == 0] = np.nan
+            mask = np.ones(arr.shape)
+            mask[np.where(arr == 0)] = 0
+            arr = np.ma.array(arr, mask=mask)
         
         return arr
     
     @lru_cache
     def to_tsfresh(self, show_progress: bool = False) -> pd.DataFrame:
         """
         Converts the events trace data into a format suitable for tsfresh, a library for time series feature extraction.
@@ -988,18 +1056,17 @@
             ids = ids + [id_] * len(trace)
             times = times + list(range(len(trace)))
             dim_0s = dim_0s + list(trace)
         
         X = pd.DataFrame({"id": ids, "time": times, "dim_0": dim_0s})
         return X
     
-    @wrapper_local_cache
     def get_average_event_trace(
             self, events: pd.DataFrame = None, empty_as_nan: bool = True, agg_func: Callable = np.nanmean,
-            index: List[int] = None, gradient: bool = False, smooth: int = None
+            index: List[int] = None, gradient: bool = False, smooth: int = None, ragged: bool = False,
             ) -> pd.Series:
         """
         Computes the average trace of events, optionally applying smoothing and gradient calculation.
 
         This method processes a DataFrame of event data to calculate an average trace. It can handle NaN values,
         apply a custom aggregation function, and optionally compute the gradient or smooth the resulting trace.
         The method is useful for summarizing event data into a single representative trace. The result will be similar
@@ -1011,28 +1078,29 @@
                 events DataFrame.
             empty_as_nan: If True, treats empty values in the trace as NaN for the purpose of calculations. Helps to
                 boost the signal-to-noise ratio, especially when dealing with sparse events.
             agg_func: A function to aggregate the event traces. Defaults to numpy's nanmean, which ignores NaN values.
             index: The index values for the resulting pd.Series. If None, defaults to a range based on trace length.
             gradient: If True, calculates the gradient of the average trace.
             smooth: Specifies the window size for smoothing the average trace. If None, no smoothing is applied.
-
+            ragged: Flag whether data is ragged or not
+            
         Returns:
             pd.Series: A pandas Series representing the average event trace, indexed as specified by the 'index' argument.
 
         Raises:
             ValueError: If the provided 'agg_func' is not a callable function.
 
         Example:
             # Assuming `events` is an instance of the Events class with event data
             avg_trace = events.get_average_event_trace(smooth=5, gradient=True)
         """
         
         # Convert events DataFrame to a numpy array representation
-        arr = self.to_numpy(events=events, empty_as_nan=empty_as_nan)
+        arr = self.to_numpy(events=events, empty_as_nan=empty_as_nan, ragged=ragged)
         
         # Check if agg_func is callable
         if not callable(agg_func):
             raise ValueError("Please provide a callable function for the 'agg_func' argument.")
         
         # Calculate the average event trace using the provided agg_func
         avg_trace = agg_func(arr, axis=0)
@@ -1362,14 +1430,15 @@
     
     @wrapper_local_cache
     def get_extended_events(
             self, events: pd.DataFrame = None, video: Union[np.ndarray, da.Array, Video] = None, dtype: type = float,
             use_footprint: bool = False, extend: Union[int, Tuple[int, int]] = -1, ensure_min: int = None,
             ensure_max: int = None, pad_borders: bool = False, return_array: bool = False, in_place: bool = False,
             normalization_instructions: Dict[int, List[Union[str, Dict[str, str]]]] = None, show_progress: bool = True,
+            load_to_memory: bool = False,
             memmap_path: Union[str, Path] = None, save_path: Union[str, Path] = None, save_param: Dict[str, Any] = None
             ) -> Union[pd.DataFrame, Tuple[np.ndarray, List[int], List[int]]]:
         """
                 Extends the footprint of individual events either over the entire z-range or a fixed number of bordering
                 frames of a time series recording.
 
                 This method extends the event signals by applying the event's footprint or mask over a specified range in the
@@ -1423,30 +1492,36 @@
             events = events.copy()
         
         n_events = len(events)
         
         # load data
         if video is not None:
             
-            if isinstance(video, Video):
+            if isinstance(video, (Video, astrocast.analysis.Video)):
                 video = video.get_data()
             elif not isinstance(video, (da.Array, np.ndarray)):
-                raise ValueError(f"'video' must be a astrocast.Video, numpy or dask array")
+                raise ValueError(f"'video' must be a astrocast.Video, numpy or dask array NOT {type(video)}")
         
         elif self.data is not None:
             video = self.data.get_data()
         else:
             raise ValueError(
                     "to extend the event traces you either have to provide the 'video' argument "
                     "when calling this function or the 'data' argument during Event creation."
                     )
         
         # get video dimensions
         n_frames, X, Y = video.shape
         
+        if load_to_memory and isinstance(video, da.Array):
+            logging.warning(f"attempting to load data to RAM "
+                            f"({humanize.naturalsize(video.size * video.itemsize)}).")
+            video = video.compute()
+            logging.warning(f"loaded!")
+        
         # create container to save extended events in
         arr_ext, extended = None, None
         if return_array:
             
             # create array
             if memmap_path:
                 memmap_path = Path(memmap_path).with_suffix(
@@ -1802,15 +1877,15 @@
 
         Returns:
           None if 'inplace' is True; otherwise, returns a numpy array of normalized traces.
 
         Example::
 
           # Assuming a class instance 'event_obj'
-          norm_instr = { 0: ["subtract", {"mode":"min"}], 1: ["divide", {"mode": "max"}]
+          norm_instr = { 0: ["subtract", {"mode":"min"}], 1: ["divide", {"mode": "max"}]}
           normalized_traces = event_obj.normalize(norm_instr, inplace=False)
           print(normalized_traces)
         """
         
         traces = self.events.trace
         
         norm = Normalization(traces)
@@ -1853,23 +1928,279 @@
         """
         cluster_lookup_table = defaultdict(lambda: default_cluster)
         cluster_lookup_table.update({k: label for k, label in list(zip(self.events.index.tolist(), labels.tolist()))})
         
         return cluster_lookup_table
 
 
+class MultiEvents(Events):
+    
+    def __init__(self, event_dirs: List[Union[str, Path, Events]] = None, lazy: bool = True,
+                 data: Union[List[Union[np.ndarray, da.Array, str, Path, Video]], Literal['infer']] = None,
+                 loc: Union[str, List[str]] = None,
+                 group: Union[str, int, List[Union[str, int]]] = None,
+                 subject_id: Union[str, int, List[Union[str, int]]] = None,
+                 z_slice: Union[Tuple[int, int], List[Tuple[int, int]]] = None,
+                 custom_columns: Union[list, Tuple, Literal['v_area_norm', 'v_ara_footprint', 'cx', 'cy']] = (
+                         "v_area_norm", "cx", "cy"), frame_to_time_mapping: Union[dict, list] = None,
+                 frame_to_time_function: Union[Callable, List[Callable]] = None, cache_path: Union[str, Path] = None,
+                 seed: int = 1):
+        
+        if cache_path is not None:
+            
+            if isinstance(cache_path, str):
+                cache_path = Path(cache_path)
+            
+            if not cache_path.is_dir():
+                cache_path.mkdir()
+                assert cache_path.exists(), f"failed to create cache_path: {cache_path}"
+                logging.info(f"created cache_path at {cache_path}")
+            
+            self.cache_path = cache_path
+        
+        super().__init__()
+        
+        self.seed = seed
+        self.z_slice = z_slice
+        self.num_event_objects = len(event_dirs)
+        self.event_dirs = event_dirs
+        
+        # data
+        if data == "infer" or data is None:
+            self.data = [data for _ in range(self.num_event_objects)]
+        elif isinstance(data, list):
+            if len(data) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#data {len(data)} != #events {self.num_event_objects}")
+            self.data = data
+        else:
+            raise ValueError(f"'data' must be either list, 'infer' or None NOT {data}")
+        
+        # loc
+        if isinstance(loc, list):
+            if len(loc) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#loc {len(loc)} != #events {self.num_event_objects}")
+            self.loc = loc
+        else:
+            self.loc = [loc for _ in range(self.num_event_objects)]
+        
+        # z_slice
+        if isinstance(z_slice, list):
+            if len(z_slice) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#z_slice {len(z_slice)} != #events {self.num_event_objects}")
+            self.z_slice = z_slice
+        else:
+            self.z_slice = [z_slice for _ in range(self.num_event_objects)]
+        
+        # group
+        if isinstance(group, list):
+            if len(group) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#group {len(group)} != #events {self.num_event_objects}")
+            self.group = group
+        else:
+            self.group = [group for _ in range(self.num_event_objects)]
+        
+        # subject_id
+        if isinstance(subject_id, list):
+            if len(subject_id) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#subject_id {len(subject_id)} != #events {self.num_event_objects}")
+            self.subject_id = subject_id
+        elif subject_id is None:
+            self.subject_id = range(self.num_event_objects)
+        else:
+            self.subject_id = [subject_id for _ in range(self.num_event_objects)]
+        
+        # frame_to_time_mapping
+        if isinstance(frame_to_time_mapping, list):
+            if len(frame_to_time_mapping) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#frame_to_time_mapping {len(frame_to_time_mapping)} != #events {self.num_event_objects}")
+            self.frame_to_time_mapping = frame_to_time_mapping
+        else:
+            self.frame_to_time_mapping = [frame_to_time_mapping for _ in range(self.num_event_objects)]
+        
+        # frame_to_time_function
+        if isinstance(frame_to_time_function, list):
+            if len(frame_to_time_function) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#frame_to_time_function {len(frame_to_time_function)} != #events {self.num_event_objects}")
+            self.frame_to_time_function = frame_to_time_function
+        else:
+            self.frame_to_time_function = [frame_to_time_function for _ in range(self.num_event_objects)]
+        
+        # cache
+        if isinstance(cache_path, list):
+            if len(cache_path) != self.num_event_objects:
+                raise ValueError(f"Length of events and data is unequal: "
+                                 f"#cache_path {len(cache_path)} != #events {self.num_event_objects}")
+            self.cache_path = cache_path
+        else:
+            self.cache_path = [cache_path for _ in range(self.num_event_objects)]
+        
+        # create events
+        self.event_objects = []
+        for i in range(self.num_event_objects):
+            
+            idx = self.subject_id[i]
+            
+            event_dir = self.event_dirs[i]
+            
+            if isinstance(event_dir, Events):
+                event = event_dir
+            
+            else:
+                event = Events(event_dir=event_dir,
+                               data=self.data[i], loc=self.loc[i], z_slice=self.z_slice[i], group=self.group[i],
+                               lazy=lazy, index_prefix=f"{idx}x", subject_id=idx,
+                               frame_to_time_mapping=self.frame_to_time_mapping[i],
+                               frame_to_time_function=self.frame_to_time_function[i],
+                               custom_columns=custom_columns, seed=self.seed, cache_path=self.cache_path[i])
+            
+            self.event_objects.append(event)
+        
+        self.events = self.combine_events()
+    
+    def combine_events(self):
+        events = pd.concat([ev.events for ev in self.event_objects])
+        events.reset_index(drop=False, inplace=True, names="subject_idx")
+        
+        # make categorical
+        for col in ('file_name', 'subject_id', 'group'):
+            if col in events.columns:
+                events[col] = events[col].astype("category")
+        
+        return events
+    
+    # def __hash__(self):
+    #     raise NotImplementedError
+    
+    # def add_clustering(self, cluster_lookup_table: dict, column_name: str = "cluster") -> None:
+    #
+    #     for event in self.event_objects:
+    #         event.add_clustering(cluster_lookup_table=cluster_lookup_table, column_name=column_name)
+    #
+    #     self.events = self.combine_events()
+    
+    # def filter(self, filters: dict, inplace: bool = True) -> None:
+    #
+    #     if not inplace:
+    #         raise NotImplementedError("currently MultiEvent objects can only be changed inplace.")
+    #
+    #     for event in self.event_objects:
+    #         event.filter(filters=filters, inplace=inplace)
+    #
+    #     self.combine_events()
+    
+    # def to_numpy(self, events: pd.DataFrame = None, empty_as_nan: bool = True, ragged: bool = False) -> np.ndarray:
+    #     raise NotImplementedError("currently MultiEvent objects does not implement this function.")
+    #
+    def show_event_map(
+            self, video: Union[Path, str] = None, loc: str = None, z_slice: Tuple[int, int] = None, lazy: bool = True
+            ):
+        raise NotImplementedError("currently MultiEvent objects does not implement this function.")
+    
+    # def get_trials(
+    #         self, trial_timings: Union[np.ndarray, da.Array], trial_length: int = 30,
+    #         multi_timing_behavior: Literal['first', 'expand', 'exclude'] = "first",
+    #         output_format: Literal['array', 'dataframe'] = "array"
+    #         ) -> Union[np.ndarray, pd.DataFrame]:
+    #     raise NotImplementedError("currently MultiEvent objects does not implement this function.")
+    
+    @wrapper_local_cache
+    def get_extended_events(
+            self, events: pd.DataFrame = None, video: Union[np.ndarray, da.Array, Video] = None, dtype: type = float,
+            use_footprint: bool = False, extend: Union[int, Tuple[int, int]] = -1, ensure_min: int = None,
+            ensure_max: int = None, pad_borders: bool = False, return_array: bool = False, in_place: bool = False,
+            normalization_instructions: Dict[int, List[Union[str, Dict[str, str]]]] = None, show_progress: bool = True,
+            load_to_memory: bool = False,
+            memmap_path: Union[str, Path] = None, save_path: Union[str, Path] = None, save_param: Dict[str, Any] = None
+            ):
+        
+        if not in_place:
+            raise NotImplementedError("currently MultiEvent objects can only be changed inplace.")
+        
+        if return_array:
+            raise NotImplementedError("currently MultiEvent objects cannot return arrays.")
+        
+        if save_path is not None:
+            raise NotImplementedError("currently MultiEvent objects cannot save results.")
+        
+        if show_progress:
+            iterator = tqdm(self.event_objects)
+        else:
+            iterator = self.event_objects
+        
+        for event in iterator:
+            event.get_extended_events(events=events, video=video, dtype=dtype,
+                                      use_footprint=use_footprint, extend=extend, ensure_min=ensure_min,
+                                      ensure_max=ensure_max, pad_borders=pad_borders, return_array=return_array,
+                                      in_place=in_place, normalization_instructions=normalization_instructions,
+                                      show_progress=show_progress, memmap_path=memmap_path, save_path=save_path,
+                                      save_param=save_param, load_to_memory=load_to_memory
+                                      )
+        
+        self.combine_events()
+    
+    def enforce_length(
+            self, min_length: Union[int, None] = None, pad_mode: str = "edge", max_length: Union[int, None] = None,
+            inplace: bool = False
+            ) -> pd.DataFrame:
+        raise NotImplementedError("currently MultiEvent objects does not implement this function.")
+    
+    # def normalize(self, normalize_instructions: dict, inplace: bool = True):
+    #
+    #     if not inplace:
+    #         raise NotImplementedError("currently MultiEvent objects can only be changed inplace.")
+    #
+    #     for event in self.event_objects:
+    #         event.normalize(normalize_instructions=normalize_instructions, inplace=inplace)
+    #
+    #     self.combine_events()
+
+
 class Plotting:
     
-    def __init__(self, events: Events = None):
+    def __init__(self, events: Union[Events, pd.DataFrame] = None):
         
-        if events is not None:
+        if isinstance(events, (Events, astrocast.analysis.Events)):
             self.events = events.events
+        elif isinstance(events, pd.DataFrame):
+            self.events = events
         else:
             self.events = events
     
+    def plot_events(self, idx: int, show_noise: bool = False, figsize=(10, 3)):
+        
+        # get event row
+        row = self.events[self.events.index == idx].iloc[0]
+        if len(row) == 0:
+            raise ValueError(f"can't find idx {idx}")
+        
+        # create figure
+        fig, axx = plt.subplot_mosaic(mosaic="AAB", figsize=figsize)
+        
+        # collect data
+        raw_trace = row.trace
+        noise_trace = row.noise_mask_trace
+        footprint = row.footprint
+        footprint = np.reshape(footprint, newshape=(row.dx, row.dy))
+        
+        # plot traces
+        ax = axx['A']
+        ax.plot(raw_trace, color="darkblue")
+        if show_noise:
+            ax.plot(noise_trace, color="gray")
+        
+        ax = axx['B']
+        ax.imshow(footprint)
+    
     @staticmethod
     def _get_factorials(nr):
         """
         Returns the factors of a number.
 
         Args:
             nr (int): Number.
@@ -1967,31 +2298,38 @@
                 new_axx.append(ax)
         
         # Adjust the spacing between subplots
         fig.tight_layout()
         
         return fig, new_axx
     
-    def _get_random_sample(self, num_samples):
+    def _get_random_sample(self, num_samples: int, by: str = None):
         """
-        Get a random sample of traces from the events.
+        Get a random sample of traces from the events, optionally grouped by a specified column.
 
         Args:
             num_samples (int): Number of samples to retrieve.
+            by (str, optional): Column name to group and sample traces by. Defaults to None.
 
         Returns:
-            list: List of sampled traces.
+            dict or list: If 'by' is specified, returns a dictionary of lists of sampled traces grouped by unique column values.
+                          Otherwise, returns a list of sampled traces.
 
         Raises:
             ValueError: If the events data type is not one of pandas.DataFrame, numpy.ndarray, or list.
-
         """
         
         events = self.events
         
+        if by is not None and isinstance(events, pd.DataFrame):
+            unique_values = events[by].unique()
+            sampled_traces = {val: events[events[by] == val].sample(min(num_samples, len(events[events[by] == val])))
+                              for val in unique_values}
+            return {val: sampled_traces[val]['trace'].values for val in unique_values}
+        
         if num_samples == -1:
             return events
         
         if isinstance(events, pd.DataFrame):
             # If events is a pandas DataFrame, sample num_samples rows and retrieve the trace values
             sel = events.sample(num_samples)
             traces = sel.trace.values
@@ -2011,29 +2349,57 @@
             raise ValueError(
                     "Please provide one of the following data types: pandas.DataFrame, numpy.ndarray, or list. "
                     f"Instead of {type(events)}"
                     )
         
         return traces
     
-    # todo clustering
-    def plot_traces(self, num_samples=-1, ax=None, figsize=(5, 5)):
+    def plot_traces(self, num_samples=-1, by=None, ax=None, figsize=(5, 5), alpha=1, linestyle='-',
+                    title: str = None):
+        """
+        Plot sampled traces, optionally grouped and color-coded by a specified column.
+
+        Args:
+            num_samples (int): Number of samples to plot. Defaults to -1.
+            by (str, optional): Column name to group and sample traces by. Also used for color coding. Defaults to None.
+            ax (matplotlib.axes.Axes, optional): Axes object to plot on. If None, a new figure is created. Defaults to None.
+            figsize (tuple, optional): Figure size. Defaults to (5, 5).
+
+        Returns:
+            matplotlib.figure.Figure: The figure object containing the plot.
+        """
         
-        traces = self._get_random_sample(num_samples=num_samples)
+        traces = self._get_random_sample(num_samples=num_samples, by=by)
         
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = ax.get_figure()
         
-        for i, trace in enumerate(traces):
-            ax.plot(trace, label=i)
+        if by is not None and isinstance(traces, dict):
+            
+            colors = sns.color_palette("husl", len(traces))
+            
+            for i, (val, selected_traces) in enumerate(traces.items()):
+                for trace in selected_traces:
+                    ax.plot(trace, color=colors[i], alpha=alpha, linestyle=linestyle,
+                            label=f"group {i}")
+            
+            handles, labels = ax.get_legend_handles_labels()
+            by_label = dict(zip(labels, handles))
+            ax.legend(by_label.values(), by_label.keys())
         
-        plt.tight_layout()
+        else:
+            for i, trace in enumerate(traces):
+                ax.plot(trace, label=i, alpha=alpha, linestyle=linestyle)
+        
+        if title is not None:
+            ax.set_title(title)
         
+        plt.tight_layout()
         return fig
     
     def plot_distribution(
             self, column, plot_func=sns.violinplot, outlier_deviation=None, axx=None, figsize=(8, 3), title=None
             ):
         
         values = self.events[column]
@@ -2150,7 +2516,50 @@
         if title_2 is not None:
             axx[letters_right[0]].set_title(title_2)
         
         axx[letters_left[-1]].set_xlabel("frames")
         axx[letters_right[-1]].set_xlabel("frames")
         
         return fig, axx
+    
+    def get_color_mapping(self, group_column: str = "group", index_column: str = "subject_id"):
+        
+        unique_groups = self.events[group_column].unique()
+        colors = sns.color_palette("husl", len(unique_groups))
+        
+        temp = self.events[[group_column, index_column]].drop_duplicates()
+        temp.index = temp.subject_id
+        
+        lut = dict(zip(unique_groups, colors))
+        
+        col_colors = temp[group_column].astype(str).map(lut)
+        return col_colors.to_dict()
+    
+    @staticmethod
+    def plot_trial_alignment(trials: Union[pd.DataFrame, List[pd.DataFrame]],
+                             labels: List[str] = None,
+                             colors: List = None,
+                             figsize=(5, 5), ax=None):
+        
+        if ax is None:
+            fig, ax = plt.subplots(1, 1, figsize=figsize)
+        
+        if isinstance(trials, pd.DataFrame):
+            trials = [trials]
+        
+        if labels is not None and isinstance(labels, str):
+            labels = [labels]
+        
+        if labels is not None and len(labels) != len(trials):
+            logging.warning(f"Length of labels ({len(labels)} != length of trials ({len(trials)}).")
+            labels = None
+        
+        if colors is None:
+            colors = sns.color_palette("husl", len(trials))
+        elif len(colors) != len(trials):
+            raise ValueError(f"length of colors ({len(colors)}) does not match length of trials ({len(trials)})")
+        
+        for i, trial in enumerate(trials):
+            label = labels[i] if labels is not None else None
+            sns.lineplot(x="timepoint", y="value", data=trial, ax=ax, color=colors[i], label=label,
+                         # **arg
+                         )
```

### Comparing `astrocast-0.4.1/astrocast/app_analysis.py` & `astrocast-0.4.2/astrocast/app_analysis.py`

 * *Files identical despite different names*

### Comparing `astrocast-0.4.1/astrocast/app_preparation.py` & `astrocast-0.4.2/astrocast/app_preparation.py`

 * *Files identical despite different names*

### Comparing `astrocast-0.4.1/astrocast/autoencoders.py` & `astrocast-0.4.2/astrocast/autoencoders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import logging
+import time
 from pathlib import Path
-from typing import Union
+from typing import Literal, Union
 
+import humanize
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from matplotlib import pyplot as plt
 from sklearn.model_selection import train_test_split
 from torch.nn.utils.rnn import pad_packed_sequence, pack_padded_sequence, pad_sequence
@@ -16,17 +19,17 @@
 # ----------------------------------------
 class EarlyStopper:
     def __init__(self, patience: int = 1, min_delta: Union[int, float] = 0):
         self.patience = patience
         self.min_delta = min_delta
         self.counter = 0
         self.min_loss = float('inf')
-
+    
     def __call__(self, loss):
-
+        
         if loss < self.min_loss:
             self.min_loss = loss
             self.counter = 0
         elif loss - self.min_loss <= self.min_delta:
             self.counter += 1
             if self.counter >= self.patience:
                 return True
@@ -34,27 +37,27 @@
 
 
 class GaussianNoise(nn.Module):
     def __init__(self, mean=0., std=0.1):
         super(GaussianNoise, self).__init__()
         self.mean = mean
         self.std = std
-
+    
     def forward(self, x):
         if self.training:
             noise = torch.randn_like(x) * self.std + self.mean
             return x + noise
         return x
 
 
 class CustomUpsample(nn.Module):
     def __init__(self, target_length):
         super(CustomUpsample, self).__init__()
         self.target_length = target_length
-
+    
     def forward(self, x):
         current_length = x.shape[-1]
         diff = self.target_length - current_length
         zeros = torch.zeros((x.shape[0], x.shape[1], diff)).to(x.device)
         return torch.cat([x, zeros], dim=-1)
 
 
@@ -67,467 +70,504 @@
 
     Parameters:
         target_length (int): trace lenght.
     
     Example:
         autoencoder = CNN_Autoencoder(target_length=18, dropout=0.2, latent_size=128, add_noise=0.1)
     """
-
+    
     def __init__(
-            self, target_length: int, dropout: float = 0.15, l1_reg: float = 0.0001, latent_size=64 * 6, add_noise=None
-    ):
+            self, target_length: int, dropout: float = 0.15, l1_reg: float = 0.0001, latent_size=64 * 6, add_noise=None,
+            use_cuda: bool = False
+            ):
         super(CNN_Autoencoder, self).__init__()
-
+        
+        self.use_cuda = use_cuda
         self.losses = None
         self.l1_reg = l1_reg
         self.latent_size = latent_size
-
+        
         self.encoder, self.decoder = self.define_layers(
-            dropout=dropout, add_noise=add_noise, target_length=target_length
-        )
-
+                dropout=dropout, add_noise=add_noise, target_length=target_length
+                )
+        
+        if self.use_cuda and torch.cuda.is_available():
+            self.cuda()  # Move the model to GPU if CUDA is enabled and available
+        
         # Manually defining a linear layer to serve as the dense layer for the encoder output
         self.latent_size = latent_size
         self.dense_layer = None
         self.dense_layer_out = None
         self.add_noise = add_noise
-
+    
     @staticmethod
     def define_layers(dropout=None, add_noise=None, target_length=18):
-
+        
         encoder_layers = []
         if dropout is not None:
             encoder_layers += [nn.Dropout(dropout)]
         if add_noise is not None:
             encoder_layers += [GaussianNoise(std=add_noise)]
         encoder_layers += [nn.Conv1d(1, 128, 3, padding=1), ]
         encoder_layers += [nn.ReLU(), ]
         encoder_layers += [nn.MaxPool1d(2), ]
         encoder_layers += [nn.Conv1d(128, 64, 3, padding=1), ]
         encoder_layers += [nn.ReLU(), ]
         encoder_layers += [nn.MaxPool1d(2), ]
         encoder = nn.Sequential(*encoder_layers)
-
+        
         decoder = nn.Sequential(
-            nn.Conv1d(64, 64, 3, padding=1), nn.ReLU(), nn.Upsample(scale_factor=2), nn.Conv1d(64, 128, 3, padding=1),
-            nn.ReLU(), nn.Upsample(scale_factor=2), CustomUpsample(target_length=target_length),
-            nn.Conv1d(128, 1, 3, padding=1), nn.Sigmoid()
-        )
-
+                nn.Conv1d(64, 64, 3, padding=1), nn.ReLU(), nn.Upsample(scale_factor=2),
+                nn.Conv1d(64, 128, 3, padding=1),
+                nn.ReLU(), nn.Upsample(scale_factor=2), CustomUpsample(target_length=target_length),
+                nn.Conv1d(128, 1, 3, padding=1), nn.Sigmoid()
+                )
+        
         return encoder, decoder
-
+    
     def forward(self, x):
+        
+        if self.use_cuda:
+            x = x.cuda()  # Ensure input data is moved to GPU
+        
         x = self.encoder(x)
-
+        
         shape_before_flatten = x.shape[1:]
         flattened_dim = torch.prod(torch.tensor(shape_before_flatten))
-
+        
         if self.dense_layer is None:
             self.dense_layer = nn.Linear(flattened_dim.item(), self.latent_size).to(x.device)
             self.dense_layer_out = nn.Linear(self.latent_size, flattened_dim.item()).to(x.device)
-
+        
         x = x.view(-1, flattened_dim)
-
+        
         # Apply the dense layer
         x = self.dense_layer(x)
-
+        
         # Make the output binary
         x = torch.sigmoid(x)
         x = torch.round(x)
-
+        
         # Save the encoder output for later use
         encoder_output = x
-
+        
         # go back to initial size
         x = self.dense_layer_out(x)
-
+        
         # Add L1 regularization to the encoder output
         l1_loss = self.l1_reg * torch.norm(x, 1)
-
+        
         x = x.view(-1, *shape_before_flatten)
         x = self.decoder(x)
-
+        
         return x, l1_loss, encoder_output
-
+    
     @staticmethod
     def split_dataset(data, val_split=0.1, train_split=0.8, seed=None):
-
+        
         from torch.utils.data import random_split
-
+        
         # Assuming you have a PyTorch Dataset object `full_dataset`
         # This could be an instance of a custom dataset class, or one of the built-in classes like `torchvision.datasets.MNIST`
-
+        
         if seed is not None:
             torch.manual_seed(seed)
-
+        
         # ensure equal length input
         unique_length = np.unique([len(data[i, :]) for i in range(len(data))])
         if len(unique_length) > 1:
             raise ValueError(f"input contains unequal length sequences: {unique_length}! aborting.")
-
+        
         # Define the proportions
         total_size = len(data)
         train_size = int(train_split * total_size)
         val_size = int(val_split * total_size)
         test_size = total_size - train_size - val_size
-
+        
         # Split the dataset
         train_dataset, val_dataset, test_dataset = random_split(data, [train_size, val_size, test_size])
         return train_dataset, val_dataset, test_dataset
-
+    
     def train_autoencoder(
             self, X_train, X_val=None, X_test=None, patience=5, min_delta=0.0005, epochs=100, learning_rate=0.001,
             batch_size=32
-    ):
-
+            ):
+        
         # ensure equal length input
         for X in [X_train, X_val, X_test]:
             if X is not None:
                 unique_length = np.unique([len(X_train[i]) for i in range(len(X))])
                 if len(unique_length) > 1:
                     raise ValueError(f"input contains unequal length sequences: {unique_length}! aborting.")
-
+        
         # Create DataLoader
         train_data = torch.FloatTensor(X_train)
+        if self.use_cuda:
+            train_data = train_data.cuda()
         train_dataset = TensorDataset(train_data, train_data)  # autoencoders use same data for input and output
         train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
-
+        
         if X_val is not None:
             val_data = torch.FloatTensor(X_val)
+            if self.use_cuda:
+                val_data = val_data.cuda()
             val_dataset = TensorDataset(val_data, val_data)
             val_loader = DataLoader(val_dataset, batch_size=batch_size, shuffle=False)
+        
         else:
             val_loader = None
-
+        
         if X_test is not None:
             test_data = torch.FloatTensor(X_test)
+            if self.use_cuda:
+                test_data = test_data.cuda()
             test_dataset = TensorDataset(test_data, test_data)
             test_loader = DataLoader(test_dataset, batch_size=batch_size, shuffle=False)
+        
         else:
             test_loader = None
-
+        
         # Initialize model
         model = self
         criterion = nn.MSELoss()  # Mean Squared Error Loss
         optimizer = optim.Adam(model.parameters(), lr=learning_rate)
-
+        
         # Training loop
-
+        
         losses = []
         early_stopper = EarlyStopper(patience=patience, min_delta=min_delta)
         pbar = tqdm(total=epochs)
         for epoch in range(epochs):
             model.train()
             train_loss = 0
-
+            
             for batch_data, _ in train_loader:  # autoencoders don't use labels
                 batch_data = batch_data.unsqueeze(1)  # add channel dimension
-
+                
                 # Forward pass
                 outputs, l1_loss, encoded = model(batch_data)
-
+                
                 # Compute loss
                 reconstruction_loss = criterion(outputs, batch_data)
                 loss = reconstruction_loss + l1_loss
-
+                
                 # Backward pass and optimization
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
-
+                
                 train_loss += loss.item()
-
+            
             # Validation
             if val_loader is not None:
                 model.eval()
                 val_loss = 0
                 with torch.no_grad():
                     for batch_data, _ in val_loader:
                         batch_data = batch_data.unsqueeze(1)  # add channel dimension
                         outputs, l1_loss, encoded = model(batch_data)
-
+                        
                         reconstruction_loss = criterion(outputs, batch_data)
                         loss = reconstruction_loss + l1_loss
                         val_loss += loss.item()
-
+                
                 model.train()
             else:
                 val_loss = None
-
+            
             losses.append((train_loss, val_loss))
-
+            
             # Early stopping logic
             if early_stopper(val_loss):
                 print("Early stopping!")
                 break
-
+            
             pbar.set_description(
-                f"train_Loss:{train_loss / len(train_loader):.4f}, val_loss:{val_loss / len(val_loader):.4f}"
-            )
+                    f"train_Loss:{train_loss / len(train_loader):.4f}, val_loss:{val_loss / len(val_loader):.4f}"
+                    )
             pbar.update()
         pbar.close()
-
+        
         # Evaluation
         if test_loader is not None:
             model.eval()
             with torch.no_grad():
                 test_loss = 0
                 for batch_data, _ in test_loader:
                     batch_data = batch_data.unsqueeze(1)  # add channel dimension
                     outputs, l1_loss, encoded = model(batch_data)
-
+                    
                     reconstruction_loss = criterion(outputs, batch_data)
                     loss = reconstruction_loss + l1_loss
                     test_loss += loss.item()
-
+                
                 print(f"Test Loss: {test_loss / len(test_loader):.4f}")
             model.train()
-
+        
         self.losses = losses
         return losses
-
+    
     def embed(self, data, batch_size=64):
-
-        # Create DataLoader
-        train_data = torch.FloatTensor(data)
-        train_dataset = TensorDataset(train_data, train_data)  # autoencoders use same data for input and output
-        train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True)
-
-        # Initialize model
-        model = self
-        encoded_traces = []
-        for batch_data, _ in train_loader:
-            batch_data = batch_data.unsqueeze(1)
-            _, _, encoded = model(batch_data)
-            encoded = encoded.detach().numpy()
-
-            encoded_traces.append(encoded)
-
-        encoded_traces = np.vstack(encoded_traces)
-
+        
+        with torch.no_grad():
+            # Create DataLoader
+            train_data = torch.FloatTensor(data)
+            if self.use_cuda:
+                train_data = train_data.cuda()
+            train_dataset = TensorDataset(train_data, train_data)  # autoencoders use same data for input and output
+            train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=False)
+            
+            # Initialize model
+            model = self
+            encoded_traces = []
+            for batch_data, _ in train_loader:
+                batch_data = batch_data.unsqueeze(1)
+                if self.use_cuda and torch.cuda.is_available():
+                    batch_data = batch_data.cuda()  # Ensure batch data is on GPU
+                
+                _, _, encoded = model(batch_data)
+                
+                if self.use_cuda:
+                    encoded = encoded.cpu()  # Move encoded data back to CPU before converting to numpy
+                
+                encoded = encoded.detach().numpy()
+                encoded_traces.append(encoded)
+            
+            encoded_traces = np.vstack(encoded_traces)
+        
         return encoded_traces
-
+    
     @staticmethod
     def reshape_to_square_matrix(vector):
         """
         Reshapes a 1D vector to a square-ish 2D matrix.
         """
-
+        
         import math
-
+        
         length = len(vector)
         # Find the closest integer square root of the length
         sqrt_length = int(math.sqrt(length))
-
+        
         # Find the dimensions of the reshaped matrix
         rows = sqrt_length
         while length % rows != 0:
             rows -= 1
         cols = length // rows
-
+        
         # Reshape the vector
         reshaped_matrix = np.reshape(vector, (rows, cols))
-
+        
         return reshaped_matrix
-
-    def plot_examples_pytorch(
-            self, X_test, Y_test=None, show_diff=False, num_samples=9, figsize=(10, 6)
-    ):
-
+    
+    def plot_examples_pytorch(self, X_test, Y_test=None,
+                              show_diff=False, trim_zeros=True,
+                              num_samples=9, figsize=(10, 6)
+                              ):
+        
         model = self
-
+        
         # Convert PyTorch tensor to numpy
         X_test = np.array(list(X_test))
-
+        
         # Make predictions if Y_test is not provided
         if Y_test is None:
             model.eval()
             with torch.no_grad():
                 input_tensor = torch.FloatTensor(X_test).unsqueeze(1)  # add channel dimension
                 output_tensor, l1_loss, encoder_output = model(input_tensor)
+            if self.use_cuda:
+                output_tensor = output_tensor.cpu()  # Move encoded data back to CPU before converting to numpy
+                encoder_output = encoder_output.cpu()
             Y_test = output_tensor.numpy().squeeze()
             encoder_output = encoder_output.numpy().squeeze()
-
+        
         else:
             encoder_output = Y_test
-
+        
         if show_diff and Y_test is not None:
             consensus = np.mean(encoder_output, axis=0)
             encoder_output = encoder_output - consensus
         else:
             if not isinstance(Y_test, np.ndarray):
                 Y_test = Y_test.numpy().squeeze()
             else:
                 Y_test = np.squeeze(Y_test)
-
+        
         num_rounds = 1
-        if not isinstance(num_samples, int):
+        if isinstance(num_samples, tuple):
             num_rounds, num_samples = num_samples
-
+        
         fig = None
         for nr in range(num_rounds):
             fig, axx = plt.subplots(3, num_samples, figsize=figsize)
-
+            
             for i, idx in enumerate(np.random.randint(0, len(X_test) - 1, size=num_samples)):
                 inp = X_test[idx, :]
                 out = Y_test[idx, :]
-
-                inp = np.trim_zeros(inp, trim="b")
-                out = out[0:len(inp)]
-
+                
+                if trim_zeros:
+                    inp = np.trim_zeros(inp, trim="b")
+                    out = out[0:len(inp)]
+                
                 axx[0, i].plot(inp, alpha=0.75, color="black")
                 axx[0, i].plot(out, alpha=0.75, linestyle="--", color="darkgreen")
                 axx[1, i].plot(inp - out)
-
+                
                 axx[0, i].sharey(axx[1, i])
-
+                
                 latent_output = encoder_output[idx, :]
                 latent_output = self.reshape_to_square_matrix(latent_output)
-
+                
                 cmap = 'binary' if not show_diff else 'bwr'
                 min_value = 0 if not show_diff else -1
                 axx[2, i].imshow(
-                    latent_output, cmap=cmap, interpolation='nearest', aspect='auto', vmin=min_value, vmax=1
-                )
+                        latent_output, cmap=cmap, interpolation='nearest', aspect='auto', vmin=min_value, vmax=1
+                        )
                 axx[2, i].get_xaxis().set_visible(False)
                 axx[2, i].get_yaxis().set_visible(False)
-
+                
                 axx[0, i].get_xaxis().set_visible(False)
                 axx[1, i].get_xaxis().set_visible(False)
-
+                
                 if i != 0:
                     axx[0, i].get_yaxis().set_visible(False)
                     axx[1, i].get_yaxis().set_visible(False)
-
+            
             axx[0, 0].set_ylabel("IN/OUT", fontweight=600)
             axx[1, 0].set_ylabel("error", fontweight=600)
-
+        
         return fig
-
+    
     def save(self, filepath: Union[str, Path]):
         """
         Save the model parameters to a file.
 
         Parameters:
         - filepath (str): The location where the model parameters should be saved.
 
         Example usage:
             model = CNN_Autoencoder(target_length=18)
             model.save("path/to/save/model.pth")
         """
-
+        
         if isinstance(filepath, Path):
             filepath = filepath.as_posix()
-
+        
         torch.save(self.state_dict(), filepath)
-
+    
     @classmethod
     def load(cls, filepath: Union[str, Path], *args, **kwargs):
         """
         Load the model parameters from a file and return an instance of the model.
 
         Parameters:
         - filepath (str): The location from where the model parameters should be loaded.
 
         Returns:
         - CNN_Autoencoder: An instance of the CNN_Autoencoder model with loaded parameters.
 
         Example usage:
             loaded_model = CNN_Autoencoder.load("path/to/save/model.pth", target_length=18)
         """
-
+        
         if isinstance(filepath, Path):
             filepath = filepath.as_posix()
-
+        
         model = cls(*args, **kwargs)  # Create a new instance of the model
         model.load_state_dict(torch.load(filepath))
         model.eval()  # Set the model to evaluation mode
         return model
 
 
 # Recurrent Neural Network Autoencoder
 # ------------------------------------
 
 class PaddedSequenceDataset(Dataset):
     def __init__(self, data):
         self.data = data
         self.lengths = [len(seq) for seq in data]
-
+    
     def __len__(self):
         return len(self.data)
-
+    
     def __getitem__(self, index):
         return self.data[index], self.lengths[index]
 
 
 class PaddedDataLoader:
-
+    
     def __init__(self, data):
         self.data = data
-
+    
     def __len__(self):
         return len(self.data)
-
+    
     def get_dataloader(self, data, batch_size, shuffle):
-
+        
         ds = [torch.tensor(x, dtype=torch.float32) for x in data]
         ds = PaddedSequenceDataset(ds)
-
+        
         dl = DataLoader(ds, batch_size=batch_size, shuffle=shuffle, collate_fn=self.collate_fn)
         return dl
-
+    
     def get_datasets(
             self, batch_size=(32, "auto", "auto"), val_size=0.15, test_size=0.15, shuffle=(True, False, False)
-    ):
-
+            ):
+        
         # First, split into training and temp sets
         train_data, temp_data = train_test_split(self.data, test_size=(val_size + test_size))
         # Then split the temp_data into validation and test sets
         val_data, test_data = train_test_split(temp_data, test_size=(test_size / (val_size + test_size)))
-
+        
         if isinstance(batch_size, int):
             batch_size = (batch_size, batch_size, batch_size)
         elif isinstance(batch_size, (list, tuple)):
             if len(batch_size) != 3:
                 raise ValueError(f"please provide batch_size as int or list of length 3.")
-
+        
         datasets = []
         for i, ds in enumerate([train_data, val_data, test_data]):
-
+            
             bs = batch_size[i]
             if bs == "auto":
                 bs = len(ds)
-
+            
             dl = self.get_dataloader(ds, batch_size=bs, shuffle=shuffle[i])
-
+            
             datasets.append(dl)
-
+        
+        logging.info(
+                f"train #{len(datasets[0])}, "
+                f"val #{len(datasets[1])}, "
+                f"test #{len(datasets[2])}")
+        
         return datasets
-
+    
     @staticmethod
     def collate_fn(batch):
         # Sort sequences by length in descending order
         batch.sort(key=lambda x: x[1], reverse=True)  # x[1] is the length
-
+        
         # Separate sequence lengths and sequences
         sequences = [x[0] for x in batch]  # x[0] is the data
         lengths = [x[1] for x in batch]  # x[1] is the length
-
+        
         # Pad sequences
         sequences = pad_sequence(sequences, batch_first=True)
-
+        
         return sequences, lengths
 
 
 class TimeSeriesRnnAE:
-
+    
     def __init__(
             self, num_features=1, rnn_hidden_dim=32, num_layers=2, encoder_lr=0.001, decoder_lr=0.001, clip=0.5,
             dropout=0, initialize_repeat=True, num_directions=1, use_cuda=False
-    ):
+            ):
         """
         Initialize the TimeSeriesRnnAE model.
 
         Parameters:
         - num_features (int): Dimensionality of the input time-series data.
         - rnn_hidden_dim (int): Number of hidden units in the LSTM layers.
         - num_layers (int): Number of LSTM layers.
@@ -537,79 +577,80 @@
         - dropout (float): Dropout rate for LSTM layers.
         - initialize_repeat (bool): Whether to initialize the repeat vector in the decoder.
         - num_directions (int): Number of directions for the LSTM layers.
         - use_cuda (bool): Whether to use GPU acceleration if available.
 
         """
         super(TimeSeriesRnnAE, self).__init__()
-
+        
         # set device
         if torch.cuda.is_available() and use_cuda:
             device = torch.device("cuda:0")
         else:
             device = "cpu"
-
+        
         self.device = device
         self.criterion = nn.MSELoss()
         self.clip = clip
-
+        
         # Create encoder rnn and decoder rnn module
         self.encoder = Encoder(
-            device=device, num_features=num_features, rnn_hidden_dim=rnn_hidden_dim, num_layers=num_layers,
-            dropout=dropout, num_directions=num_directions
-        )
+                device=device, num_features=num_features, rnn_hidden_dim=rnn_hidden_dim, num_layers=num_layers,
+                dropout=dropout, num_directions=num_directions
+                )
         self.decoder = Decoder(
-            device=self.device, criterion=self.criterion, initialize_repeat=initialize_repeat,
-            rnn_hidden_dim=rnn_hidden_dim, num_layers=num_layers, num_features=num_features,
-            num_directions=num_directions, dropout=dropout
-        )
+                device=self.device, criterion=self.criterion, initialize_repeat=initialize_repeat,
+                rnn_hidden_dim=rnn_hidden_dim, num_layers=num_layers, num_features=num_features,
+                num_directions=num_directions, dropout=dropout
+                )
         self.encoder.to(device)
         self.decoder.to(device)
         # Create optimizers for encoder and decoder
         self.encoder_lr = encoder_lr
         self.decoder_lr = decoder_lr
         self.encoder_optimizer = optim.Adam(self.encoder.parameters(), lr=encoder_lr)
         self.decoder_optimizer = optim.Adam(self.decoder.parameters(), lr=decoder_lr)
-
+        
         # initialize historical variables
         self.learning_rates = None
         self.val_losses = None
         self.train_losses = None
-
+    
     def update_learning_rates(self, encoder_factor, decoder_factor):
         self.encoder_lr = self.encoder_lr * encoder_factor
         self.decoder_lr = self.decoder_lr * decoder_factor
         self.set_learning_rates(self.encoder_lr, self.decoder_lr)
-
+    
     def set_learning_rates(self, encoder_lr, decoder_lr):
         self.encoder_lr = encoder_lr
         self.decoder_lr = decoder_lr
         for param_group in self.encoder_optimizer.param_groups:
             param_group['lr'] = encoder_lr
         for param_group in self.decoder_optimizer.param_groups:
             param_group['lr'] = decoder_lr
-
+    
     def train(self):
         self.encoder.train()
         self.decoder.train()
-
+    
     def eval(self):
         self.encoder.eval()
         self.decoder.eval()
-
+    
     @staticmethod
     def are_equal_tensors(a, b):
         if torch.all(torch.eq(a, b)).data.cpu().numpy() == 0:
             return False
         return True
-
-    def train_epochs(
-            self, dataloader_train, dataloader_val=None, num_epochs=10, diminish_learning_rate=0.99, patience=5,
-            min_delta=0.001, smooth_loss_len=3, safe_after_epoch=None, show_mode=None
-    ):
+    
+    def train_epochs(self, dataloader_train: PaddedSequenceDataset,
+                     dataloader_val: PaddedSequenceDataset = None, num_epochs=10,
+                     diminish_learning_rate=0.99, patience=5, min_delta=0.001, smooth_loss_len=3,
+                     safe_after_epoch=None, show_mode: Literal['progress', 'notebook'] = None
+                     ):
         """
         Train the TimeSeriesRnnAE model for multiple epochs.
 
         Parameters:
         - dataloader_train (DataLoader): DataLoader object for the training data.
         - dataloader_val (DataLoader): DataLoader object for the validation data (optional).
         - num_epochs (int): Maximum number of epochs to train the model.
@@ -620,400 +661,409 @@
         - safe_after_epoch (str, Path): Path to save the final encoder and decoder models to.
         - show_mode (str): Mode for displaying training progress ('progress', 'notebook', or None).
 
         Returns:
         - epoch_loss (float): The total loss for the last epoch.
 
         """
-
+        
         self.train()
-
+        
         patience_counter = 0
         losses = None
-
+        train_length = len(dataloader_train)
+        val_length = 1 if dataloader_val is None else len(dataloader_val)
+        
         if show_mode == "progress":
             iterator = tqdm(range(num_epochs), total=num_epochs)
         elif show_mode == "notebook":
             from IPython.display import clear_output
             from IPython.core.display_functions import display
             iterator = range(num_epochs)
         else:
             iterator = range(num_epochs)
-
+        
         train_losses = []
         val_losses = []
         learning_rates = []
         for epoch in iterator:
-
+            
+            t0 = time.time()
+            
             batch_losses = []
             for batch_data, batch_lengths in dataloader_train:
                 batch_data = batch_data.unsqueeze(-1)
                 batch_data = batch_data.to(dtype=torch.float32).to(self.device)  # Move to device and ensure it's float
                 batch_lengths = torch.tensor(batch_lengths, dtype=torch.float32, device=self.device)
-
+                
                 # Pack the batch
                 packed_batch_data = pack_padded_sequence(
-                    batch_data, batch_lengths.cpu().numpy(), batch_first=True
-                )  # .to(self.device)
-
+                        batch_data, batch_lengths.cpu().numpy(), batch_first=True
+                        )  # .to(self.device)
+                
                 # Your existing code for training on a single batch
                 batch_loss = self.train_batch(packed_batch_data, batch_lengths)
                 batch_losses.append(batch_loss)
-
+            
             epoch_loss = np.mean(batch_losses)
             train_losses.append(epoch_loss)
-
+            
             if diminish_learning_rate is not None:
                 self.update_learning_rates(diminish_learning_rate, diminish_learning_rate)
             learning_rates.append([self.encoder_lr, self.decoder_lr])
-
+            
             # model saving
             if safe_after_epoch is not None:
-
+                
                 if not isinstance(safe_after_epoch, (str, Path)):
                     raise ValueError(f"please provide 'safe_after_epoch' as string or pathlib.Path")
-
+                
                 if isinstance(safe_after_epoch, str):
                     safe_after_epoch = Path(safe_after_epoch)
-
+                
                 encoder_file_name = safe_after_epoch.joinpath("_encoder.model")
                 decoder_file_name = safe_after_epoch.joinpath("_decoder.model")
-
+                
                 self.save_models(encoder_file_name, decoder_file_name)
-
+            
             if dataloader_val is not None:
                 val_loss = self.evaluate_batch(dataloader_val)
                 val_losses.append(val_loss)
-
+            
             # progress
             if show_mode == "progress":
-
+                
                 descr = f"tloss>{epoch_loss:.2E} "
-
+                
                 if dataloader_val is not None:
                     descr += f"vloss>{val_losses[-1]:.2E} "
-
+                
                 if self.encoder_lr == self.decoder_lr:
                     descr += f"lr>{self.encoder_lr:.2E} "
                 else:
                     descr += f"lr>({self.encoder_lr:.2E}, {self.decoder_lr:.2E}) "
-
+                
                 descr += f"P{patience_counter}"
-
+                
                 iterator.set_description(descr)
                 iterator.update()
-
+            
             elif show_mode == "notebook":
-
+                
                 from IPython.core.display_functions import clear_output, display
-
+                
                 plt.clf()
                 clear_output(wait=True)
-
+                
                 fig, axx = plt.subplots(1, 2, figsize=(9, 4))
-
-                axx[0].plot(train_losses, color="black", label="training")
+                
+                tloss = [t / train_length for t in train_losses]
+                axx[0].plot(tloss, color="black", label="training")
                 if dataloader_val is not None:
-                    axx[0].plot(np.array(val_losses).flatten(), color="green", label="validation")
-
+                    vloss = np.array(val_losses).flatten() / val_length
+                    axx[0].twinx().plot(vloss, color="green", label="validation")
+                
                 axx[0].set_title(f"losses")
                 axx[0].set_yscale("log")
                 axx[0].legend()
-
+                
                 lrates = np.array(learning_rates)
                 axx[1].plot(lrates[:, 0], color="green", label="encoder")
                 axx[1].plot(lrates[:, 1], color="red", label="decoder")
                 axx[1].set_title(f"learning rates")
                 axx[1].legend()
-
-                fig.suptitle(f"Epoch {epoch}/{num_epochs}; Patience {patience_counter}/{patience}")
-
+                
+                fig.suptitle(f"Epoch {epoch}/{num_epochs} "
+                             f"Patience {patience_counter}/{patience} "
+                             f"runtime {humanize.naturaldelta(time.time() - t0)}")
+                
                 plt.tight_layout()
-
+                
                 display(fig)
-
+            
             # Early stopping
             if dataloader_val is not None:
                 losses = val_losses
             else:
                 losses = train_losses
-
+            
             smoothed_loss = np.median(np.array(losses[-smooth_loss_len - 1:-1]))
             if smoothed_loss - losses[-1] > min_delta:
                 patience_counter = 0
             else:
                 patience_counter += 1
-
+            
             # Check for early stopping
             if patience_counter >= patience:
                 print("Early stopping triggered.")
                 break
-
+        
         self.eval()
-
+        
         self.train_losses = train_losses
         self.val_losses = val_losses
         self.learning_rates = learning_rates
-
+        
         return losses
-
+    
     def train_batch(self, packed_inputs, lengths):
         """
         Train a single batch for the TimeSeriesRnnAE model.
 
         Parameters:
         - packed_inputs (PackedSequence): The packed input time-series data for this batch.
 
         Returns:
         - loss (float): The normalized loss for this batch.
         """
         # Get batch size and number of time steps
         batch_size = packed_inputs.batch_sizes[0]  # The first element contains the batch size
         num_steps = packed_inputs.data.size(0)  # Total number of time steps across all sequences
-
+        
         # Zero the gradients
         self.encoder_optimizer.zero_grad()
         self.decoder_optimizer.zero_grad()
-
+        
         # Forward pass through the encoder and decoder
         initial_hidden = self.encoder.init_hidden(batch_size)
-
+        
         z, new_hidden = self.encoder(packed_inputs, initial_hidden)
-
+        
         loss = self.decoder(packed_inputs, z, lengths)
-
+        
         # Backpropagation
         loss.backward()
-
+        
         # Gradient clipping
         torch.nn.utils.clip_grad_norm_(self.encoder.parameters(), self.clip)
         torch.nn.utils.clip_grad_norm_(self.decoder.parameters(), self.clip)
-
+        
         # Update parameters
         self.encoder_optimizer.step()
         self.decoder_optimizer.step()
-
+        
         return loss.item() / num_steps  # Normalized loss
-
+    
     def evaluate_batch(self, dataloader, return_outputs=False):
-
+        
         losses = []
         outputs = []
         for batch_data, batch_lengths in dataloader:
-
+            
             batch_data = batch_data.unsqueeze(-1)
             batch_data = batch_data.to(dtype=torch.float32).to(self.device)  # Move to device and ensure it's float
             batch_lengths = torch.tensor(batch_lengths, dtype=torch.float32, device=self.device)
-
+            
             # Pack the batch
             packed_batch_data = pack_padded_sequence(
-                batch_data, batch_lengths.cpu().numpy(), batch_first=True
-            )  # .to(self.device)
-
+                    batch_data, batch_lengths.cpu().numpy(), batch_first=True
+                    )  # .to(self.device)
+            
             batch_size = packed_batch_data.batch_sizes[0]  # The first element contains the batch size
-
+            
             # encode
             initial_hidden = self.encoder.init_hidden(batch_size)
             z, new_hidden = self.encoder(packed_batch_data, initial_hidden)
-
+            
             # decode
             res = self.decoder(packed_batch_data, z, batch_lengths, return_outputs=return_outputs)
-
+            
             if return_outputs:
                 loss, output = res
-                outputs.append(output)
+                outputs.append(output.cpu().detach().numpy())
             else:
                 loss = res
-            losses.append(loss.detach().numpy())
-
+            losses.append(loss.cpu().detach().numpy())
+        
         losses = np.mean(np.array(losses))
-
+        
         if return_outputs:
             return losses, outputs
         else:
             return losses
-
+    
     def save_models(self, encoder_file_name, decoder_file_name):
         torch.save(self.encoder.state_dict(), encoder_file_name)
         torch.save(self.decoder.state_dict(), decoder_file_name)
-
+    
     def load_models(self, encoder_file_name, decoder_file_name):
         self.encoder.load_state_dict(torch.load(encoder_file_name))
         self.decoder.load_state_dict(torch.load(decoder_file_name))
-
+    
     def embedd(self, dataloader: DataLoader):
         """
             Embeds the data using the trained encoder-decoder model.
 
             Args:
                 dataloader (torch.utils.data.DataLoader): The data loader for the input data.
 
             Returns:
                 Tuple: A tuple containing the embedded input data, the decoded output data, the latent representation, and the losses.
 
         """
         self.eval()
-
+        
         x_val = []
         y_val = []
         latent = []
         losses = []
         for batch_data, batch_lengths in tqdm(dataloader):
             batch_data = batch_data.unsqueeze(-1)
             batch_data = batch_data.to(
-                dtype=torch.float32
-            )  # .to(self.device)  # Move to device and ensure it is a float
+                    dtype=torch.float32
+                    ).to(self.device)  # Move to device and ensure it is a float
             batch_lengths = torch.tensor(batch_lengths, dtype=torch.float32)  # , device=self.device)
-
+            
             # Pack the batch
             packed_batch_data = pack_padded_sequence(
-                batch_data, batch_lengths.cpu().numpy(), batch_first=True
-            )  # .to(self.device)
+                    batch_data, batch_lengths.cpu().numpy(), batch_first=True
+                    )  # .to(self.device)
             batch_size = packed_batch_data.batch_sizes[0]  # The first element contains the batch size
-
+            
             # encode
             encoder = self.encoder
             initial_hidden = encoder.init_hidden(batch_size)
             encoded, _ = encoder(packed_batch_data, initial_hidden)
-
+            
             # decode
             decoder = self.decoder
             loss, decoded = decoder(packed_batch_data, encoded, batch_lengths, return_outputs=True)
-
+            
             # Convert batch_data and decoded data to numpy
             x_np = batch_data.cpu().numpy()
             y_np = decoded.cpu().detach().numpy()
             encoded_np = encoded.cpu().detach().numpy()
-
+            
             # Remove zero padding based on batch_lengths
             x_np = [x_np[i, :int(batch_lengths[i]), :] for i in range(len(batch_lengths))]
             y_np = [y_np[i, :int(batch_lengths[i]), :] for i in range(len(batch_lengths))]
-
+            
             x_val.extend(x_np)
             y_val.extend(y_np)
             latent.extend(encoded_np)
             losses.append(loss.item())
-
+        
         return x_val, y_val, latent, losses
-
+    
     def plot_traces(self, dataloader, figsize=(10, 10), n_samples=16, sharex=False):
-
+        
         self.eval()
-
+        
         x_val, y_val, latent, losses = self.embedd(dataloader)
-
+        
         n_samples = min(len(x_val), n_samples)
         fig, axx = plt.subplots(n_samples, 2, figsize=figsize, sharex=sharex)
-
+        
         for i, idx in enumerate(np.random.randint(0, len(x_val), size=n_samples)):
             x = np.squeeze(x_val[idx])
             y = np.squeeze(y_val[idx])
-
+            
             axx[i, 0].plot(x, color="gray", linestyle="--")
             axx[i, 0].plot(y, color="red", linestyle="-")
             axx[i, 0].set_ylabel(f"idx: {idx}")
-
+            
             if i != 0:
                 axx[i, 0].sharex(axx[0, 0])
-
+            
             latent_vector = latent[i]
             latent_vector = np.reshape(latent_vector, (len(latent_vector), 1)).transpose()
             axx[i, 1].imshow(latent_vector, aspect="auto", cmap="viridis")
             axx[i, 1].axis("off")
-
+        
         plt.tight_layout()
-
+        
         return fig, x_val, y_val, latent, losses
 
 
 class Encoder(nn.Module):
-
+    
     def __init__(self, device="cpu", num_features=1, rnn_hidden_dim=32, num_layers=2, dropout=0, num_directions=1):
         """ Initializes the Encoder object.
         Parameters:
             device (str): The device to use for computations, default is “cpu”.
             num_features (int): The number of input features, default is 1.
             rnn_hidden_dim (int): The number of hidden units in the RNN, default is 32.
             num_layers (int): The number of layers in the RNN, default is 2.
             dropout (float): The dropout rate, default is 0.
         """
         super(Encoder, self).__init__()
-
+        
         self.device = device
         self.num_hidden_states = 2
         rnn = nn.LSTM
-
+        
         self.num_features = num_features
         self.rnn_hidden_dim = rnn_hidden_dim
         self.num_layers = num_layers
         self.dropout = dropout
         self.num_directions = num_directions
-
+        
         self.rnn = rnn(
-            num_features, rnn_hidden_dim, num_layers=num_layers, bidirectional=False, dropout=dropout, batch_first=True
-        )
-
+                num_features, rnn_hidden_dim, num_layers=num_layers, bidirectional=False, dropout=dropout,
+                batch_first=True
+                )
+        
         # Initialize hidden state
         self.hidden = None
         self._init_weights()
-
+    
     def init_hidden(self, batch_size):
         return (torch.zeros(self.num_layers * self.num_directions, batch_size, self.rnn_hidden_dim).to(
-            self.device
-        ), torch.zeros(self.num_layers * self.num_directions, batch_size, self.rnn_hidden_dim).to(
-            self.device
-        ))
-
+                self.device
+                ), torch.zeros(self.num_layers * self.num_directions, batch_size, self.rnn_hidden_dim).to(
+                self.device
+                ))
+    
     def forward(self, packed_inputs, initial_hidden=None):
-
+        
         # Initialize hidden state based on the current batch size
         batch_size = packed_inputs.batch_sizes[0]
-
+        
         if initial_hidden is None:
             initial_hidden = self.init_hidden(batch_size)
-
+        
         # Forward pass through RNN
         _, new_hidden = self.rnn(packed_inputs, initial_hidden)
-
+        
         # Flatten the hidden state
         last_embedding_layer = self._flatten_hidden(new_hidden)
-
+        
         return last_embedding_layer, new_hidden  # Return the new hidden state
-
+    
     @staticmethod
     def _flatten_hidden(h):
-
+        
         if h is None:
             return None
-
+        
         return h[0][-1]  # Take the last hidden state from the last layer
-
+    
     @staticmethod
     def _flatten(h, batch_size):
         # (num_layers*num_directions, batch_size, hidden_dim)  ==>
         # (batch_size, num_directions*num_layers, hidden_dim)  ==>
         # (batch_size, num_directions*num_layers*hidden_dim)
         return h.transpose(0, 1).contiguous().view(batch_size, -1)
-
+    
     def _init_weights(self):
         for m in self.modules():
             if isinstance(m, nn.Embedding):
                 torch.nn.init.uniform_(m.weight, -0.001, 0.001)
             elif isinstance(m, nn.Linear):
                 torch.nn.init.xavier_uniform_(m.weight)
                 m.bias.data.fill_(0.01)
 
 
 class Decoder(nn.Module):
-
+    
     def __init__(
             self, criterion=nn.MSELoss(), device="cpu", initialize_repeat=True, rnn_hidden_dim=32, num_layers=2,
             num_features=1, num_directions=1, dropout=0,
-
-    ):
+            
+            ):
         """ Initializes the Decoder object.
             Parameters:
                 criterion (nn.Module): The loss function to use, default is nn.MSELoss().
                 device (str): The device to use for computations, default is “cpu”.
                 initialize_repeat (bool): Whether to initialize the repeat, default is True.
                 rnn_hidden_dim (int): The number of hidden units in the RNN, default is 32.
                 num_layers (int): The number of layers in the RNN, default is 2.
@@ -1021,84 +1071,84 @@
                 num_directions (int): The number of directions in the RNN, default is 1.
                 dropout (float): The dropout rate, default is 0.
 
         """
         super(Decoder, self).__init__()
         self.device = device
         self.criterion = criterion
-
+        
         self.initialize_repeat = initialize_repeat
         self.rnn_hidden_dim = rnn_hidden_dim
         self.num_layers = num_layers
         self.num_features = num_features
         self.num_directions = num_directions
         self.dropout = dropout
-
+        
         if not self.initialize_repeat:
             self.transformation_layer = nn.Linear(
-                self.rnn_hidden_dim, self.rnn_hidden_dim * self.num_layers
-            )
-
+                    self.rnn_hidden_dim, self.rnn_hidden_dim * self.num_layers
+                    )
+        
         # RNN layer
         self.num_hidden_states = 2
         rnn = nn.LSTM
-
+        
         self.rnn = rnn(
-            self.num_features, self.rnn_hidden_dim * self.num_directions, num_layers=self.num_layers,
-            dropout=self.dropout, batch_first=True
-        )
-
+                self.num_features, self.rnn_hidden_dim * self.num_directions, num_layers=self.num_layers,
+                dropout=self.dropout, batch_first=True
+                )
+        
         self.out = nn.Linear(self.rnn_hidden_dim * self.num_directions, self.num_features)
-
+        
         self._init_weights()
-
+    
     def forward(self, sequence, z, lengths, return_outputs=False):
         # Unpack the sequence
         padded_sequence, _ = pad_packed_sequence(sequence, batch_first=True)
-
+        
         # Now padded_sequence is a tensor, and you can get its shape
         batch_size, num_steps = padded_sequence.shape[0], padded_sequence.shape[1]
-
+        
         # Initialize with the embedding
         hidden = (z.repeat(self.num_layers, 1, 1), z.repeat(self.num_layers, 1, 1))
-
+        
         # Initialize recovered_sequence with zeros
         recovered_sequence = torch.zeros(padded_sequence.shape, dtype=torch.float32).to(self.device)
-
+        
         # Initialize prediction with zeros
         prediction = torch.zeros((batch_size, 1), dtype=torch.float32).to(self.device)
-
+        
         # Loop through each time step
         for i in range(num_steps):
             prediction, hidden = self._step(prediction, hidden)
             recovered_sequence[:, i] = prediction.squeeze() if batch_size == 1 else prediction
-
+        
         # Compute loss
         loss = self.criterion(padded_sequence, recovered_sequence)
-
+        
         if return_outputs:
             return loss, recovered_sequence
         else:
             return loss
-
+    
     def _step(self, input_, hidden):
-
+        
         # Ensure the input is 3D: [batch_size, 1, input_dim]
         if len(input_.shape) == 2:
             input_ = input_.unsqueeze(1)
-
+        
         # Push input through RNN layer with current hidden state
         prediction, hidden = self.rnn(input_, hidden)
-
+        
         # print("hidden.shape: ", hidden[0].shape, hidden[1].shape)
-
+        
         prediction = self.out(prediction)[:, :, 0]  # .squeeze(0)
-
+        
         return prediction, hidden
-
+    
     def _init_weights(self):
         for m in self.modules():
             if isinstance(m, nn.Embedding):
                 torch.nn.init.uniform_(m.weight, -0.001, 0.001)
             elif isinstance(m, nn.Linear):
                 torch.nn.init.xavier_uniform_(m.weight)
                 m.bias.data.fill_(0.01)
```

### Comparing `astrocast-0.4.1/astrocast/cli_interfaces.py` & `astrocast-0.4.2/astrocast/cli_interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,56 +696,64 @@
 @click_custom_option('--in-memory', type=click.BOOL, default=False, help='Whether to store data in memory.')
 @click_custom_option('--logging-level', type=click.INT, default=logging.INFO, help='Logging level for messages.')
 @click_custom_option(
         '--loc-out', type=click.STRING, default=None,
         help='Location in the output file where the results will be saved.'
         )
 @click_custom_option(
-        '--dtype', type=click.STRING, default="same",
+        '--dtype', type=click.STRING, default="float32",
         help='Data type for the output. If "same", the data type of the input will be used.'
         )
 @click_custom_option(
         '--chunk-strategy', type=click.Choice(["None", 'balanced', 'XY', 'Z']), default="balanced",
         help='Infer chunks size.'
         )
 @click_custom_option(
         '--chunks', type=(click.INT, click.INT, click.INT), default=None,
         help='Chunk size to use when saving to HDF5 or TileDB.'
         )
+@click_custom_option(
+        '--compression', type=click.STRING, default="gzip",
+        help='Compression algorithm to use.'
+        )
 @click_custom_option('--rescale', type=click.BOOL, default=True, help='Whether to rescale the output values.')
 def denoise(
         input_path, batch_size, input_size, pre_post_frames, gap_frames, z_select, logging_level, model, loc_out, dtype,
-        chunk_strategy, chunks, rescale, overlap, padding, normalize, loc_in, in_memory, output_file
+        chunk_strategy, chunks, rescale, overlap, padding, normalize, loc_in, in_memory, output_file, compression
         ):
     """
     Denoise the input data using the SubFrameGenerator class and infer method.
     """
     
     if model is None:
         raise ValueError(f"Please provide a model with '--model'")
     
     if output_file is None:
         output_file = input_path
         logging.warning(f"No output_file provided. Choosing input_file: {input_path}")
     
-    from astrocast.denoising import SubFrameGenerator
+    from astrocast.denoising import SubFrameDataset, PyTorchNetwork
     
-    with (UserFeedback(params=locals(), logging_level=logging_level)):
+    with ((UserFeedback(params=locals(), logging_level=logging_level))):
+        
         # Initializing the SubFrameGenerator instance
-        sub_frame_generator = SubFrameGenerator(paths=input_path, batch_size=batch_size, input_size=input_size,
-                                                pre_post_frames=pre_post_frames, gap_frames=gap_frames,
-                                                z_select=z_select, allowed_rotation=[0], allowed_flip=[-1],
-                                                overlap=overlap, padding=padding, shuffle=False, normalize=normalize,
-                                                loc=loc_in, in_memory=in_memory, save_global_descriptive=False,
-                                                logging_level=logging_level)
+        infer_dataset = SubFrameDataset(paths=input_path, loc=loc_in, input_size=input_size,
+                                        pre_post_frames=pre_post_frames, gap_frames=gap_frames,
+                                        z_select=z_select, allowed_rotation=[0], allowed_flip=[-1],
+                                        overlap=overlap, padding=padding, shuffle=False, normalize=normalize,
+                                        in_memory=in_memory, save_global_descriptive=False,
+                                        logging_level=logging_level)
+        
+        # Load model
+        net = PyTorchNetwork(infer_dataset, load_model=model, batch_size=batch_size)
         
         # Running the infer method
-        result = sub_frame_generator.infer(
-                model=model, output=output_file, out_loc=loc_out, dtype=dtype,
-                chunks=chunks, chunk_strategy=chunk_strategy, rescale=rescale)
+        net.infer(dataset=infer_dataset, output=output_file, out_loc=loc_out, dtype=dtype, chunks=chunks,
+                  chunk_strategy=chunk_strategy, compression=compression,
+                  rescale=rescale)
         
         logging.info(f"saved inference to: {output_file}")
 
 
 @cli.command()
 @click.argument('input-path', type=click.Path())
 @click_custom_option('--loc', type=click.STRING, default=None, help='Specific dataset to run the process on.')
@@ -1297,67 +1305,86 @@
                 k = dict_["key"]
                 print(f"\tchecking: {k}")
                 
                 base_name = f.name.replace(".h5", "")
                 log_name = log_path.joinpath(f"slurm-%A-{base_name}-{k}.out").as_posix()
                 job_name = f"{k}_{base_name}"
                 
-                if (k == "roi" and "df" in file and not f.with_suffix(".roi").exists()) or (k not in file):
-                    
-                    cmd += f"astrocast --config {cfg_path} {dict_['script']} {f};"
-                    print(f"\tcmd {k}>{base_name}:\n {cmd}")
-                    
-                    dependency = dict(afterok=last_jobid) if last_jobid is not None else None
+                # roi output exists
+                skip_step = True
+                if k == "roi":
                     
-                    slurm = Slurm()
-                    slurm.add_arguments(A=account)
-                    slurm.add_arguments(c=dict_["cores"])
-                    
-                    # set time dynamically
-                    req_time = dict_["time"]
-                    if "/" in req_time:
-                        
-                        # split requirement into parts
-                        req_time, per_pixel = req_time.split("/")
-                        numbers = req_time.split(":")
-                        
-                        # calculate multiplier
-                        if "data" not in file:
-                            Z, X, Y = 10000, 512, 512
-                            logging.warning(f"couldn't find data size. Assuming {(Z, X, Y)}!")
-                        else:
-                            for data_key in file["data"].keys():
-                                Z, X, Y = file[f"data/{data_key}"].shape
+                    roi_output = f.with_suffix(".roi")
+                    if roi_output.exists():
                         
-                        multiplier = (Z * X * Y) / int(float(per_pixel))
+                        expected_files = ["event_map.tiff", "events.npy"]
                         
-                        req_time = ""
-                        for num in numbers:
-                            num = f"{int(int(num) * multiplier)}"
-                            
-                            if num == "0":
-                                num = "00"
-                            
-                            req_time += f"{num}:"
-                        
-                        req_time = req_time[:-1]
-                        logging.warning(f"choosing dynamic runtime: {req_time}")
+                        for exp in expected_files:
+                            if not roi_output.joinpath(exp).exists():
+                                skip_step = False
+                
+                # other outputs exist
+                elif k not in file:
+                    skip_step = False
+                
+                if skip_step:
+                    continue
+                
+                # push command
+                cmd += f"astrocast --config {cfg_path} {dict_['script']} {f};"
+                print(f"\tcmd {k}>{base_name}:\n {cmd}")
+                
+                dependency = dict(afterok=last_jobid) if last_jobid is not None else None
+                
+                slurm = Slurm()
+                slurm.add_arguments(A=account)
+                slurm.add_arguments(c=dict_["cores"])
+                
+                # set time dynamically
+                req_time = dict_["time"]
+                if "/" in req_time:
                     
-                    slurm.add_arguments(time=str(req_time))
+                    # split requirement into parts
+                    req_time, per_pixel = req_time.split("/")
+                    numbers = req_time.split(":")
                     
-                    if job_name is not None:
-                        slurm.add_arguments(J=job_name)
+                    # calculate multiplier
+                    if "data" not in file:
+                        Z, X, Y = 10000, 512, 512
+                        logging.warning(f"couldn't find data size. Assuming {(Z, X, Y)}!")
+                    else:
+                        for data_key in file["data"].keys():
+                            Z, X, Y = file[f"data/{data_key}"].shape
                     
-                    if log_path is not None:
-                        slurm.add_arguments(output=log_name)
+                    multiplier = (Z * X * Y) / int(float(per_pixel))
                     
-                    if dependency is not None:
-                        slurm.add_arguments(dependency=dependency)
+                    req_time = ""
+                    for num in numbers:
+                        num = f"{int(int(num) * multiplier)}"
+                        
+                        if num == "0":
+                            num = "00"
+                        
+                        req_time += f"{num}:"
                     
-                    last_jobid = slurm.sbatch(cmd)
+                    req_time = req_time[:-1]
+                    logging.warning(f"choosing dynamic runtime: {req_time}")
+                
+                slurm.add_arguments(time=str(req_time))
+                
+                if job_name is not None:
+                    slurm.add_arguments(J=job_name)
+                
+                if log_path is not None:
+                    slurm.add_arguments(output=log_name)
+                
+                if dependency is not None:
+                    slurm.add_arguments(dependency=dependency)
+                
+                last_jobid = slurm.sbatch(cmd)
 
 
 def save_projection(input_path_: Union[Path, str], loc: str, output_path_: Union[Path, str] = None,
                     lazy=True, overwrite=False) -> None:
     
     import h5py
     from astrocast.analysis import Video
```

### Comparing `astrocast-0.4.1/astrocast/clustering.py` & `astrocast-0.4.2/astrocast/clustering.py`

 * *Files 10% similar despite different names*

```diff
@@ -122,17 +122,18 @@
     
     def __init__(self, cache_path=None, logging_level=logging.INFO):
         super().__init__(logging_level=logging_level, cache_path=cache_path)
         
         self.Z = None
     
     def get_barycenters(
-            self, events, cutoff, criterion="distance", default_cluster=-1, distance_matrix=None,
-            distance_type="pearson", param_distance={}, return_linkage_matrix=False, param_linkage={},
-            param_clustering={}, param_barycenter={}
+            self, events, cutoff, criterion="distance", default_cluster=-1,
+            distance_matrix=None, distance_type: Literal['pearson', 'dtw', 'dtw_parallel'] = "pearson",
+            param_distance={}, return_linkage_matrix=False,
+            param_linkage={}, param_clustering={}, param_barycenter={}
             ):
         
         """
 
         :param events:
         :param cutoff: maximum cluster distance (criterion='distance') or number of clusters (criterion='maxclust')
         :param criterion: one of 'inconsistent', 'distance', 'monocrit', 'maxclust' or 'maxclust_monocrit'
@@ -258,16 +259,19 @@
     def calculate_barycenters(
             self, clusters, cluster_labels, events, init_fraction=0.1, max_it=100, thr=1e-5, penalty=0, psi=None,
             show_progress=True
             ):
         
         """ Calculate consensus trace (barycenter) for each cluster"""
         
-        traces = events.events.trace.tolist()
-        indices = events.events.index.tolist()
+        if not isinstance(events, pd.DataFrame):
+            events = events.events
+        
+        traces = events.trace.tolist()
+        indices = events.index.tolist()
         
         c_idx_, c_bc, c_num, c_cluster = list(), list(), list(), list()
         iterator = tqdm(
                 enumerate(clusters.index), total=len(clusters), desc="barycenters:"
                 ) if show_progress else enumerate(clusters.index)
         for i, cl in iterator:
             idx_ = np.where(cluster_labels == cl)[0]
@@ -441,15 +445,17 @@
             corr = np.corrcoef(events).astype(dtype)
             corr = np.tril(corr)
         
         return corr
     
     @wrapper_local_cache
     def get_dtw_correlation(
-            self, events: Events, use_mmap: bool = False, block: int = 10000, show_progress: bool = True
+            self, events: Events, use_mmap: bool = False, block: int = 10000,
+            parallel: bool = True, compact: bool = False, only_triu: bool = False,
+            return_similarity: bool = True, show_progress: bool = True
             ):
         """
                     Computes the dynamic time warping (DTW) correlation matrix for a set of time series.
 
                     This function calculates the pairwise DTW distances between time series data,
                     represented by the `events` object. It uses a fast DTW computation method and can handle
                     large datasets by optionally utilizing memory mapping (mmap).
@@ -475,20 +481,24 @@
                     Returns:
                         np.ndarray
                             A 1-D array representing the upper triangular part of the computed DTW distance matrix.
                             The matrix is compacted into a 1-D array where each entry represents the distance between
                             a pair of time series.
 
                     """
-        traces = [np.array(t) for t in events.events.trace.tolist()]
+        
+        if not isinstance(events, pd.DataFrame):
+            events = events.events
+        
+        traces = [np.array(t) for t in events.trace.tolist()]
         N = len(traces)
         
         if not use_mmap:
             distance_matrix = dtw.distance_matrix_fast(
-                    traces, use_pruning=False, parallel=True, compact=True, only_triu=True
+                    traces, use_pruning=False, parallel=parallel, compact=compact, only_triu=only_triu
                     )
             
             distance_matrix = np.array(distance_matrix)
         
         else:
             
             logging.info("creating mmap of shape ({}, 1)".format(int((N * N - N) / 2)))
@@ -499,26 +509,104 @@
             iterator = range(0, N, block) if not show_progress else tqdm(range(0, N, block), desc="distance matrix:")
             
             i = 0
             for x0 in iterator:
                 x1 = min(x0 + block, N)
                 
                 dm_ = dtw.distance_matrix_fast(
-                        traces, block=((x0, x1), (0, N)), use_pruning=False, parallel=True, compact=True, only_triu=True
+                        traces, block=((x0, x1), (0, N)), use_pruning=False, parallel=parallel, compact=compact,
+                        only_triu=only_triu
                         )
                 
                 distance_matrix[i:i + len(dm_)] = dm_
                 distance_matrix.flush()
                 
                 i = i + len(dm_)
                 
                 del dm_
         
+        if return_similarity:
+            distance_matrix = self.distance_to_similarity(distance_matrix)
+        
         return distance_matrix
     
+    @staticmethod
+    def distance_to_similarity(D, r=None, a=None, method='exponential', return_params=False, cover_quantile=False):
+        """Transform a distance matrix to a similarity matrix.
+
+        The available methods are:
+        - Exponential: e^(-D / r)
+          r is max(D) if not given
+        - Gaussian: e^(-D^2 / r^2)
+          r is max(D) if not given
+        - Reciprocal: 1 / (r + D*a)
+          r is 1 if not given
+        - Reverse: r - D
+          r is min(D) + max(D) if not given
+
+        All of these methods are monotonically decreasing transformations. The order of the
+        distances thus remains unchanged (only the direction).
+
+        Example usage::
+
+            dist_matrix = dtw.distance_matrix(series)
+            sim_matrix = distance_to_similarity(dist_matrix)
+
+
+        :param D: The distance matrix
+        :param r: A scaling or smoothing parameter.
+        :param method: One of 'exponential', 'gaussian', 'reciprocal', 'reverse'
+        :param return_params: Return the value used for parameter r
+        :param cover_quantile: Compute r such that the function covers the `cover_quantile` fraction of the data.
+            Expects a value in [0,1]. If a tuple (quantile, value) is given, then r (and a) are set such that
+            at the quantile the given value is reached (if not given, value is 1-quantile).
+        :return: Similarity matrix S
+        """
+        if cover_quantile is not False:
+            if type(cover_quantile) in [tuple, list]:
+                cover_quantile, cover_quantile_target = cover_quantile
+            else:
+                cover_quantile_target = 1 - cover_quantile
+        else:
+            cover_quantile_target = None
+        method = method.lower()
+        if method == 'exponential':
+            if r is None:
+                if cover_quantile is False:
+                    r = np.max(D)
+                else:
+                    r = -np.quantile(D, cover_quantile) / np.log(cover_quantile_target)
+            S = np.exp(-D / r)
+        elif method == 'gaussian':
+            if r is None:
+                if cover_quantile is False:
+                    r = np.max(D)
+                else:
+                    r = np.sqrt(-np.quantile(D, cover_quantile) ** 2 / np.log(cover_quantile_target))
+            S = np.exp(-np.power(D, 2) / r ** 2)
+        elif method == 'reciprocal':
+            if r is None:
+                r = 1
+            if a is None:
+                if cover_quantile is False:
+                    a = 1
+                else:
+                    a = (1 - cover_quantile_target * r) / (cover_quantile_target * np.quantile(D, cover_quantile))
+            S = 1 / (r + D * a)
+        elif method == 'reverse':
+            if r is None:
+                r = np.min(D) + np.max(D)
+            S = (r - D) / r
+        else:
+            raise ValueError("method={} is not supported".format(method))
+        if return_params:
+            return S, r
+        else:
+            return S
+    
     @wrapper_local_cache
     def get_dtw_parallel_correlation(
             self, events: Events, local_dissimilarity: Literal[
                 "square_euclidean_distance", "gower", "norm1", "norm2", "braycurtis", "canberra", "chebyshev", "cityblock", "correlation", "cosine", "euclidean", "jensenshannon", "minkowski", "sqeuclidean"] = "norm1",
             type_dtw: Literal["d", "i"] = "d", constrained_path_search: Literal["itakura", "sakoe_chiba"] = None,
             itakura_max_slope: float = None, sakoe_chiba_radius: int = None, sigma_kernel: int = 1,
             dtw_to_kernel: bool = False, multivariate: bool = True, use_mmap: bool = False
@@ -948,15 +1036,15 @@
             ev0 = ev0[0]
             ev1 = ev1[0]
         
         # Choose z range
         trace_0 = events[ev0]
         trace_1 = events[ev1]
         
-        if not isinstance(trace_0, np.ndarray):
+        if isinstance(trace_0, da.Array):
             trace_0 = trace_0.compute()
             trace_1 = trace_1.compute()
         
         trace_0 = np.squeeze(trace_0).astype(float)
         trace_1 = np.squeeze(trace_1).astype(float)
         
         if z_range is not None:
@@ -1161,20 +1249,22 @@
             for name, obj in inspect.getmembers(module):
                 if inspect.isclass(obj):
                     available_models.append(name)
         
         return available_models
     
     def train_classifier(
-            self, embedding=None, category_vector=None, split=0.8, classifier="RandomForestClassifier", **kwargs
+            self, embedding=None, category_vector=None, indices=None, split=0.8, classifier="RandomForestClassifier",
+            balance_training_set: bool = False, balance_test_set: bool = False, **kwargs
             ):
         
         # split into training and validation dataset
         if self.X_train is None or self.Y_train is None:
-            self.split_dataset(embedding, category_vector, split=split)
+            self.split_dataset(embedding, category_vector, split=split, indices=indices,
+                               balance_training_set=balance_training_set, balance_test_set=balance_test_set)
         
         # available models
         available_models = self.get_available_models()
         if classifier not in available_models:
             raise ValueError(f"unknown classifier {classifier}. Choose one of {available_models}")
         
         # fit model
@@ -1203,40 +1293,105 @@
         
         if normalization_instructions is not None:
             norm = Normalization(X, inplace=True)
             norm.run(normalization_instructions)
         
         return self.clf.predict(X)
     
-    def evaluate(self, regression=False, cutoff=0.5, normalize=None):
+    @staticmethod
+    def compute_scores(true_labels, predicted_labels, scoring: Literal['classification', 'clustering'] =
+    'classification'):
+        """Compute performance metrics between true and predicted labels.
+
+        Args:
+          true_labels: Ground truth (correct) labels.
+          predicted_labels: Predicted labels, as returned by a classifier.
+          scoring: type of scoring
+
+        Returns:
+          A dictionary with accuracy, precision, recall, and F1 score.
+        """
         
-        evaluations = []
-        for X, Y, lbl in [(self.X_train, self.Y_train, "train"), (self.X_test, self.Y_test, "test")]:
+        if scoring == 'classification':
             
+            from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
+            
+            return {
+                'accuracy':  accuracy_score(true_labels, predicted_labels),
+                'precision': precision_score(true_labels, predicted_labels, average='macro'),
+                'recall':    recall_score(true_labels, predicted_labels, average='macro'),
+                'f1':        f1_score(true_labels, predicted_labels, average='macro')
+                }
+        
+        elif scoring == 'clustering':
+            
+            from sklearn.metrics import adjusted_mutual_info_score, adjusted_rand_score, homogeneity_score, rand_score
+            
+            return {
+                'adjusted_mutual_info_score': adjusted_mutual_info_score(true_labels, predicted_labels),
+                'adjusted_rand_score':        adjusted_rand_score(true_labels, predicted_labels),
+                'homogeneity_score':          homogeneity_score(true_labels, predicted_labels),
+                'rand_score':                 rand_score(true_labels, predicted_labels)
+                }
+        
+        else:
+            raise ValueError(f"for scoring choose one of: classifcation, clustering")
+    
+    def evaluate(self, regression=False, cutoff=0.5, normalize=None, show_plot: bool = True,
+                 title: str = None, figsize=(10, 5), axx=None):
+        
+        fig = None
+        if show_plot and axx is None:
+            fig, axx = plt.subplots(1, 2, figsize=figsize)
+        
+        evaluations = {}
+        for i, (X, Y, lbl) in enumerate([(self.X_train, self.Y_train, "train"), (self.X_test, self.Y_test, "test")]):
+            
+            results = {}
             pred = np.squeeze(self.clf.predict(X))
             
             if pred.dtype != int and not regression and cutoff is not None:
                 logging.warning(f"assuming probability prediction. thresholding at {cutoff}")
                 Y = Y >= cutoff
             
             if regression:
                 score = self.clf.score(X, Y)
-                evaluations.append(score)
+                evaluations[lbl] = {"score": score}
             
             else:
                 
+                # create confusion matrix
                 cm = confusion_matrix(pred, Y, normalize=normalize)
-                evaluations.append(cm)
+                results["cm"] = cm
+                
+                # create score
+                for k, v in self.compute_scores(Y, pred).items():
+                    results[k] = v
+                
+                # plot result
+                if show_plot:
+                    ax = axx[i]
+                    sns.heatmap(cm, annot=True, fmt=".2f", cmap="Blues", cbar=False, ax=ax)
+                    ax.set_xlabel("Predicted")
+                    ax.set_ylabel("True")
+                    ax.set_title(f"Confusion Matrix ({lbl.capitalize()})")
+                
+                evaluations[lbl] = results
+        
+        if show_plot and title is not None:
+            if fig is None:
+                fig = axx[0].get_figure()
+            fig.suptitle(title)
         
         return evaluations
     
-    def split_dataset(
-            self, embedding, category_vector, split=0.8, balance_training_set=False, balance_test_set=False,
-            encode_category=None, normalization_instructions=None
-            ):
+    def split_dataset(self, embedding, category_vector, indices=None,
+                      split=0.8, balance_training_set=False, balance_test_set=False,
+                      encode_category=None, normalization_instructions=None
+                      ):
         
         # get data
         X = embedding
         
         if isinstance(X, pd.DataFrame):
             X = X.values
         
@@ -1274,17 +1429,24 @@
             norm.run(normalization_instructions)
         
         # split X and Y
         split_idx = int(len(X) * split)
         X_train, X_test = X[:split_idx], X[split_idx:]
         Y_train, Y_test = Y[:split_idx], Y[split_idx:]
         
-        indices = self.events.events.index.tolist()
+        # ensure correct length of indices
+        if indices is None:
+            logging.warning(f"Assuming indices from event dataframe.")
+            indices = self.events.events.index.tolist()
+        elif len(indices) != len(X):
+            raise ValueError(f"length of indices ({len(indices)}) does not match length of embedding ({len(X)})")
+        
         indices_train, indices_test = indices[:split_idx], indices[split_idx:]
         
+        # todo: this is too late, because sometimes Y_test is missing values due to the split in the section before
         # balancing
         if balance_training_set:
             X_train, Y_train, indices_train = self._balance_set(X_train, Y_train, indices_train)
         
         if balance_test_set:
             X_test, Y_test, indices_test = self._balance_set(X_test, Y_test, indices_test)
         
@@ -1292,36 +1454,72 @@
         self.X_train = X_train
         self.Y_train = Y_train
         self.X_test = X_test
         self.Y_test = Y_test
         self.indices_train = indices_train
         self.indices_test = indices_test
     
+    # @staticmethod
+    # def _balance_set(X, Y, indices):
+    #
+    #     # identify the category with the fewest members
+    #     count_category_members = pd.Series(Y).value_counts()
+    #     min_category_count = count_category_members.min()
+    #
+    #     # choose random indices
+    #     rand_indices = list()
+    #     for category in count_category_members.index.unique():
+    #         rand_indices.append(np.random.choice(np.where(Y == category)[0], size=min_category_count, replace=False))
+    #
+    #     rand_indices = np.array(rand_indices).astype(int)
+    #     rand_indices = rand_indices.flatten()
+    #
+    #     # select randomly chosen rows
+    #     X = X[rand_indices]
+    #     Y = Y[rand_indices]
+    #
+    #     indices = np.array(indices)[rand_indices]
+    #
+    #     return X, Y, indices
+    
     @staticmethod
     def _balance_set(X, Y, indices):
         
-        # identify the category with the fewest members
-        count_category_members = pd.Series(Y).value_counts()
-        min_category_count = count_category_members.min()
+        X = np.array(X)
+        Y = np.array(Y)
         
-        # choose random indices
-        rand_indices = list()
-        for category in count_category_members.index.unique():
-            rand_indices.append(np.random.choice(np.where(Y == category)[0], size=min_category_count, replace=False))
+        unique_classes = np.unique(Y)
+        min_class_samples = np.inf
         
-        rand_indices = np.array(rand_indices).astype(int)
-        rand_indices = rand_indices.flatten()
+        for cls in unique_classes:
+            class_count = np.sum(Y == cls)
+            if class_count < min_class_samples:
+                min_class_samples = class_count
+        
+        if min_class_samples == np.inf or min_class_samples == 0:
+            # Balancing is not feasible; you could raise an error or skip.
+            raise ValueError("Balancing not feasible: One or more classes have zero samples.")
+        
+        balanced_X, balanced_Y, balanced_indices = [], [], []
+        for cls in unique_classes:
+            cls_indices = np.where(Y == cls)[0]
+            chosen_indices = np.random.choice(cls_indices, min_class_samples, replace=False)
+            chosen_indices = np.array(chosen_indices).flatten()
+            
+            balanced_X.append(X[chosen_indices])
+            balanced_Y.append(Y[chosen_indices])
+            balanced_indices.extend([indices[i] for i in chosen_indices])
+        
+        # Flattening the lists
+        balanced_X = np.vstack(balanced_X)
+        balanced_Y = np.concatenate(balanced_Y)
+        # Ensure indices match the order of the balanced dataset
+        balanced_indices = [indices[i] for i in np.argsort(balanced_Y)]
         
-        # select randomly chosen rows
-        X = X[rand_indices]
-        Y = Y[rand_indices]
-        
-        indices = np.array(indices)[rand_indices]
-        
-        return X, Y, indices
+        return balanced_X, balanced_Y, balanced_indices
 
 
 class CoincidenceDetection:
     
     def __init__(
             self, events, incidences, embedding, train_split=0.8, balance_training_set=False, balance_test_set=False,
             encode_category=None, normalization_instructions=None
@@ -1340,17 +1538,17 @@
         self.train_split = train_split
         self.balance_training_set = balance_training_set
         self.balance_test_set = balance_test_set
         self.encode_category = encode_category
         self.normalization_instructions = normalization_instructions
         
         # align incidences
-        self.aligned = self.align_events_and_incidences()
+        self.aligned = self._align_events_and_incidences()
     
-    def align_events_and_incidences(self):
+    def _align_events_and_incidences(self):
         
         id_event_ = []
         num_events_ = []
         incidence_location_ = []
         incidence_location_relative_ = []
         for i, (idx, row) in enumerate(self.events.events.iterrows()):
             
@@ -1374,36 +1572,39 @@
                  "incidence_location":          incidence_location_,
                  "incidence_location_relative": incidence_location_relative_}
                 )
         
         return aligned
     
     def _train(
-            self, embedding, category_vector, classifier, regression=False, normalize_confusion_matrix=False, **kwargs
+            self, embedding, category_vector, classifier, regression=False, normalize_confusion_matrix=False,
+            show_plot: bool = False,
+            **kwargs
             ):
         
         discr = Discriminator(self.events)
         
         discr.split_dataset(
                 embedding, category_vector, split=self.train_split, balance_training_set=self.balance_training_set,
                 balance_test_set=self.balance_test_set, encode_category=self.encode_category,
                 normalization_instructions=self.normalization_instructions
                 )
         
         clf = discr.train_classifier(
                 self, embedding, split=None, classifier=classifier, **kwargs
                 )
         
-        evaluation = discr.evaluate(cutoff=0.5, normalize=normalize_confusion_matrix, regression=regression)
+        evaluation = discr.evaluate(cutoff=0.5, normalize=normalize_confusion_matrix, regression=regression,
+                                    show_plot=show_plot)
         
         return clf, evaluation
     
     def predict_coincidence(
-            self, binary_classification=True, classifier="RandomForestClassifier", normalize_confusion_matrix=False,
-            **kwargs
+            self, binary_classification=True, classifier="RandomForestClassifier", normalize_confusion_matrix=None,
+            show_plot: bool = False, **kwargs
             ):
         
         aligned = self.aligned.copy()
         aligned = aligned.reset_index()
         
         embedding = self.embedding.copy()
         
@@ -1414,20 +1615,22 @@
         
         else:
             category_vector = aligned.num_incidences
             category_vector = category_vector.astype(int).values
         
         clf, confusion_matrix = self._train(
                 embedding, category_vector, classifier, regression=False,
-                normalize_confusion_matrix=normalize_confusion_matrix, **kwargs
+                normalize_confusion_matrix=normalize_confusion_matrix, show_plot=show_plot,
+                **kwargs
                 )
         
         return clf, confusion_matrix
     
-    def predict_incidence_location(self, classifier="RandomForestRegressor", single_event_prediction=True, **kwargs):
+    def predict_incidence_location(self, classifier="RandomForestRegressor", single_event_prediction=True,
+                                   show_plot: bool = False, **kwargs):
         
         aligned = self.aligned.copy()
         aligned = aligned.reset_index()
         
         embedding = self.embedding.copy()
         
         # select event with coincidence
@@ -1442,11 +1645,12 @@
         
         if single_event_prediction:
             category_vector = selected.incidence_location_relative.apply(lambda x: x[0]).values
         else:
             raise ValueError(f"currently multi event prediction is not implemented.")
         
         clf, score = self._train(
-                embedding, category_vector, classifier=classifier, regression=True, **kwargs
+                embedding, category_vector, classifier=classifier, regression=True,
+                show_plot=False, **kwargs
                 )
         
         return clf, score
```

### Comparing `astrocast-0.4.1/astrocast/denoising.py` & `astrocast-0.4.2/astrocast/denoising.py`

 * *Files 1% similar despite different names*

```diff
@@ -1587,15 +1587,15 @@
 
 
 class PyTorchNetwork:
     def __init__(
             self, train_dataset: SubFrameDataset, val_dataset: SubFrameDataset = None,
             test_dataset: SubFrameDataset = None, batch_size: int = 32, shuffle: bool = True, num_workers: int = 4,
             learning_rate: float = 0.0001, momentum: float = 0.9, decay_rate: float = 0.1, decay_steps: int = 30,
-            n_stacks: int = 3, kernels: int = 64, kernel_size: int = 3, batch_normalize: bool = False,
+            n_stacks: int = None, kernels: int = None, kernel_size: int = None, batch_normalize: bool = False,
             loss: PyTorchLoss = "annealed_loss",
             load_model: Union[str, Path] = None, use_cpu: bool = False):
         
         # define attributes
         self.t0 = None
         self.optimizer = None
         self.iterator = None
@@ -1603,14 +1603,26 @@
         self.kernels = kernels
         self.kernel_size = kernel_size
         self.batch_normalize = batch_normalize
         self.item_size = train_dataset.item_size
         self.input_size = train_dataset.input_size
         self.history = None
         
+        # check input
+        if load_model is None:
+            if n_stacks is None:
+                raise ValueError(f"Please provide 'n_stacks' parameter or provide pretrained model with 'load_model'.")
+            
+            if kernels is None:
+                raise ValueError(f"Please provide 'kernels' parameter or provide pretrained model with 'load_model'.")
+            
+            if kernel_size is None:
+                raise ValueError(
+                        f"Please provide 'kernel_size' parameter or provide pretrained model with 'load_model'.")
+        
         # define generators
         self.train_dataloader = DataLoader(train_dataset, batch_size=batch_size, shuffle=shuffle,
                                            num_workers=num_workers)
         
         if val_dataset is not None:
             self.val_dataloader = DataLoader(val_dataset, batch_size=batch_size, shuffle=shuffle,
                                              num_workers=num_workers)
@@ -1619,22 +1631,21 @@
         
         if test_dataset is not None:
             self.test_dataloader = DataLoader(test_dataset, batch_size=batch_size, shuffle=False,
                                               num_workers=num_workers)
         else:
             self.test_dataloader = None
         
-        # Create fresh UNet
-        self.model = UNet(item_size=self.item_size, n_stacks=n_stacks,
-                          batch_normalize=batch_normalize,
-                          kernels=kernels, kernel_size=kernel_size)
-        
-        # load model
+        # Create model
         if load_model is not None:
             self._load_model(model_path=load_model)
+        else:
+            self.model = UNet(item_size=self.item_size, n_stacks=n_stacks,
+                              batch_normalize=batch_normalize,
+                              kernels=kernels, kernel_size=kernel_size)
         
         # Define loss
         self.loss = loss
         
         # define decay rate
         self.learning_rate = learning_rate
         self.momentum = momentum
@@ -1764,15 +1775,17 @@
         
         # Run unfrozen epochs
         self.run(num_epochs=unfrozen_epochs, patience=patience, min_delta=min_delta, save_model=save_model,
                  model_prefix=model_prefix, show_mode=show_mode)
     
     def infer(self, dataset: SubFrameDataset, output: Union[str, Path] = None,
               out_loc: str = None, batch_size: int = 16, num_workers: int = 4,
-              dtype: Union[Literal["same"], np.dtype] = "same", chunk_size: Union[str, Tuple[int, int, int]] = None,
+              dtype: Union[Literal["same"], np.dtype] = "same", chunks: Union[str, Tuple[int, int, int]] = None,
+              compression: str = None,
+              chunk_strategy: Literal['Z', 'XY', 'balanced'] = 'Z',
               rescale: bool = True, overwrite: bool = False,
               ) -> Union[np.ndarray, Path, None]:
         """
         Performs inference on video data using a provided model and generates output in specified format.
 
         This method applies a deep learning model to the video data to perform tasks such as denoising or segmentation.
         It supports different input and output formats, including .h5 and .tif files. The method also allows for optional
@@ -1828,28 +1841,28 @@
             output = Path(output)
         
         if output is not None and output.suffix in (".h5", ".hdf5"):
             
             if out_loc is None:
                 raise ValueError(f"when exporting results to .h5 file please provide 'out_loc' flag")
             
-            if chunk_size is None:
+            if chunks is None:
                 io = IO()
-                chunk_size = io.infer_chunks(output_shape, dtype, strategy="Z")
+                chunks = io.infer_chunks(output_shape, dtype, strategy=chunk_strategy)
             
             f = h5.File(output, "a")
             
             if out_loc in f:
                 if overwrite:
                     del f[out_loc]
                 else:
                     raise FileExistsError(f"Dataset {out_loc} already exists in {output}. "
                                           f"Choose a different output file or set 'overwrite' to True.")
             
-            rec = f.create_dataset(out_loc, shape=output_shape, chunks=chunk_size, dtype=dtype)
+            rec = f.create_dataset(out_loc, shape=output_shape, chunks=chunks, dtype=dtype, compression=compression)
         else:
             rec = np.zeros(output_shape, dtype=dtype)
         
         # infer frames
         dataloader = DataLoader(dataset, batch_size=batch_size, shuffle=False, num_workers=num_workers)
         
         for i, (inputs, _) in tqdm(enumerate(dataloader), total=len(dataloader)):
@@ -1916,17 +1929,21 @@
         elif output.suffix in (".h5", ".hdf5"):
             f.close()
             return output
     
     def save(self, path, extras: dict = None):
         
         model_dict = {'model_state_dict':     self.model.state_dict(),
-                      'optimizer_state_dict': self.optimizer.state_dict(), 'item_size': self.item_size,
-                      'n_stacks':             self.n_stacks, 'kernels': self.kernels, 'kernel_size': self.kernel_size,
-                      'batch_normalize':      self.batch_normalize, 'input_size': self.input_size}
+                      'optimizer_state_dict': self.optimizer.state_dict(),
+                      'item_size':            self.item_size,
+                      'n_stacks':             self.n_stacks,
+                      'kernels':              self.kernels,
+                      'kernel_size':          self.kernel_size,
+                      'batch_normalize':      self.batch_normalize,
+                      'input_size':           self.input_size}
         
         if extras is not None:
             model_dict.update(extras)
         
         if path.suffix != ".pth":
             path = path.with_suffix(".pth")
             logging.warning(f"changed path suffix to {path}")
@@ -1958,18 +1975,23 @@
         item_size = load_dict['item_size']
         input_size = load_dict['input_size']
         
         if self.item_size != item_size:
             raise ValueError(f"loaded module expects a stack length of {item_size}, got {self.item_size}."
                              f"Stack length is defined by the pre and post frames during dataset initiation.")
         
-        if self.input_size != input_size:
+        if self.input_size is not None and self.input_size != input_size:
             raise ValueError(f"loaded module expects an input_size of {input_size}, got {self.input_size}."
                              f"Input size is defined during dataset initiation.")
         
+        # Create fresh model
+        self.model = UNet(item_size=item_size, n_stacks=n_stacks,
+                          batch_normalize=batch_normalize,
+                          kernels=kernels, kernel_size=kernel_size)
+        
         # Load the saved model weights
         if 'model_state_dict' in load_dict:
             self.model.load_state_dict(load_dict['model_state_dict'])
         else:
             raise KeyError("The loaded dictionary does not have a 'model_state_dict' key.")
         
         # update the class attributes
```

### Comparing `astrocast-0.4.1/astrocast/detection.py` & `astrocast-0.4.2/astrocast/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,19 +323,28 @@
                     io.save(self.output_directory.joinpath("debug_smoothed_input.tiff"), data=data)
             
             # Threshold
             if use_spatial:
                 active_pixels_spatial = self._spatial_threshold(
                         data, min_ratio=spatial_min_ratio, threshold_z_depth=spatial_z_depth
                         )
+                
+                if debug:
+                    io.save(self.output_directory.joinpath("debug_active_pixels_spatial.tiff"),
+                            data=active_pixels_spatial)
+            
             if use_temporal:
                 active_pixels_temporal = self._temporal_threshold(
                         data, prominence=temporal_prominence, width=temporal_width, rel_height=temporal_rel_height,
                         wlen=temporal_wlen, plateau_size=temporal_plateau_size
                         )
+                
+                if debug:
+                    io.save(self.output_directory.joinpath("debug_active_pixels_temporal.tiff"),
+                            data=active_pixels_temporal)
             
             if use_spatial and use_temporal:
                 
                 if comb_type == "&":
                     active_pixels = np.minimum(active_pixels_spatial, active_pixels_temporal)
                 elif comb_type == "|":
                     active_pixels = np.maximum(active_pixels_spatial, active_pixels_temporal)
@@ -1207,15 +1216,15 @@
                 
                 # signal-to-noise characteristics
                 if temp_v_noise_mask_mean == 0:
                     SNR = None
                 else:
                     SNR = abs(temp_v_max_height / temp_v_noise_mask_mean)
                 
-                if np.isinf(SNR):
+                if SNR is not None and np.isinf(SNR):
                     SNR = None
                 
                 res[event_id_key]["v_signal_to_noise_ratio"] = SNR
                 
                 if temp_v_noise_mask_std != 0 and SNR is not None:
                     res[event_id_key]["v_signal_to_noise_ratio_fold"] = abs(SNR / temp_v_noise_mask_std)
                 else:
```

### Comparing `astrocast-0.4.1/astrocast/helper.py` & `astrocast-0.4.2/astrocast/helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import glob
+import inspect
 import logging
 import pickle
 import platform
+import random
 import shutil
 import tempfile
 import time
 import types
+from functools import lru_cache
 from pathlib import Path
-from typing import Tuple, Union
+from typing import List, Literal, Tuple, Union
 
 import awkward as ak
 import dask.array as da
 import h5py
 import numpy as np
 import pandas as pd
 import py.path
 import tifffile
 import tiledb
 import xxhash
 import yaml
 from skimage.util import img_as_uint
+from sklearn.preprocessing import LabelEncoder
+from tqdm import tqdm
 
 
 def closest_power_of_two(value):
     """
     Check if the value is a power of two, and if not, find the closest power of two.
 
     Args:
@@ -209,15 +214,15 @@
         else:
             
             try:
                 # last saving attempt
                 with open(path + ".p", "wb") as f:
                     pickle.dump(value, f)
             except:
-                print("saving failed because datatype is unknown: ", type(value))
+                logging.warning("saving failed because datatype is unknown: ", type(value))
                 return False
         
         return True
     
     def load_value(path):
         
         # convert file path
@@ -234,15 +239,15 @@
             result = np.load(path)
         
         elif suffix == "p":
             with open(path, "rb") as f:
                 result = pickle.load(f)
         
         else:
-            print("loading failed because filetype not recognized: ", path)
+            logging.warning("loading failed because filetype not recognized: ", path)
             result = None
         
         return result
     
     def inner_function(*args, **kwargs):
         
         if isinstance(f, types.FunctionType) and "cache_path" in list(kwargs.keys()):
@@ -254,15 +259,23 @@
                 self_ = args[0]
                 cache_path = self_.cache_path
             
             except:
                 logging.warning(f"trying to cache static method or class without 'cache_path': {f.__name__}")
                 cache_path = None
         
-        if cache_path is not None:
+        if cache_path == "lru_cache":
+            
+            @lru_cache
+            def temp(args_, kwargs_):
+                return f(*args_, **kwargs_)
+            
+            return temp(args, kwargs)
+        
+        elif cache_path is not None and isinstance(cache_path, (str, Path)):
             
             hash_string = get_string_from_args(f, args, kwargs)
             cache_path = cache_path.joinpath(hash_string)
             
             # find file with regex matching from hash_value
             files = glob.glob(cache_path.as_posix() + ".*")
             
@@ -381,40 +394,398 @@
     
     if return_dtype:
         return shape, chunksize, dtype
     else:
         return shape, chunksize
 
 
+class SignalGenerator:
+    
+    def __init__(self, parameter_fluctuations: float = 0,
+                 signal_amplitude: float = None, noise_amplitude: float = 0.05, abort_amplitude=None,
+                 allow_negative_values: bool = False, trace_length: Union[int, List[int], Tuple[int, int]] = None,
+                 offset: Union[int, Tuple[int, int], Tuple[float, float], Tuple[None]] = None,
+                 ragged_allowed: bool = True,
+                 oscillation_frequency: int = 4, oscillation_amplitude: float = 1, plateau_duration: int = 1,
+                 a: float = 0, k: float = 1, b: float = 1, v: float = 1, m_0: float = 0,
+                 leaky_k: float = 0.1, leaky_n: float = 1, show_progress: bool = False,
+                 ):
+        """
+        Initializes the SignalGenerator with parameters for the signal phases and noise level.
+
+        Args:
+            a: Left horizontal asymptote, representing the curve's minimum value.
+            k: Right horizontal asymptote, representing the curve's maximum value.
+            b: Growth rate; negative for inverted behavior.
+            v: Shape parameter, biases the slope of the maximum growth rate.
+            m_0: The value of `t` at which the maximum growth rate occurs; adjusts the curve's position along the x-axis.
+            plateau_duration: Duration of the plateau phase in arbitrary units.
+            oscillation_frequency: Frequency of oscillation within the plateau.
+            oscillation_amplitude: Amplitude of the oscillations within the plateau.
+            leaky_k: A constant controlling the rate of the leak.
+            leaky_n: The exponent controlling how the leak rate scales with the state's value.
+        """
+        self.signal_amplitude = signal_amplitude
+        self.noise_amplitude = noise_amplitude
+        self.abort_amplitude = abort_amplitude
+        self.allow_negative_values = allow_negative_values
+        
+        self.oscillation_frequency = oscillation_frequency
+        self.oscillation_amplitude = oscillation_amplitude
+        self.plateau_duration = plateau_duration
+        
+        self.leaky_k = leaky_k
+        self.leaky_n = leaky_n
+        
+        self.trace_length = trace_length
+        self.offset = offset
+        self.ragged_allowed = ragged_allowed
+        
+        self.m_0 = m_0
+        self.v = v
+        self.b = b
+        self.c = 1
+        self.k = k
+        self.a = a
+        
+        self.parameter_fluctuations = parameter_fluctuations
+        self.show_progress = show_progress
+        
+        self.identifier = self.get_hash()
+    
+    def get_hash(self):
+        
+        if isinstance(self.trace_length, (int, float)):
+            tl = self.trace_length
+        elif isinstance(self.trace_length, (List, Tuple)):
+            tl = sum(self.trace_length)
+        else:
+            tl = 1
+        
+        h = xxhash.xxh128(np.array([self.signal_amplitude, self.noise_amplitude, self.abort_amplitude,
+                                    self.oscillation_frequency, self.oscillation_amplitude, self.plateau_duration,
+                                    self.leaky_k, self.leaky_n, tl, self.offset, self.ragged_allowed,
+                                    self.m_0, self.v, self.b, self.k, self.a]))
+        
+        return h.intdigest()
+    
+    @staticmethod
+    def _richards_curve(t: Union[float, np.ndarray, int] = None, a: float = 0, k: float = 1,
+                        c: float = 1, b: float = 1, v: float = 1, m_0: float = 6):
+        """
+        Calculate the first derivative of the Richards curve at time t or returns the derivative function of the Richards curve.
+
+        The derivative of the Richards curve represents the rate of change of the growth process at time t.
+
+        Args:
+            t: Time point(s) at which the curve's derivative is evaluated. If None, returns the derivative function itself.
+            a: Left horizontal asymptote, representing the curve's minimum value.
+            k: Right horizontal asymptote, representing the curve's maximum value.
+            c: Affects the rate of growth; often set to 1.
+            b: Growth rate; negative for inverted behavior.
+            v: Shape parameter, biases the slope of the maximum growth rate.
+            m_0: The value of `t` at which the maximum growth rate occurs; adjusts the curve's position along the x-axis.
+
+        Raises:
+            ValueError: If `v` is not greater than 0.
+
+        Returns:
+            The first derivative of the Richards curve value(s) at time t, or the derivative function if t is None.
+        """
+        
+        if v <= 0:
+            raise ValueError(f"v={v} must be greater than 0.")
+        
+        def func(x):
+            exponent = np.exp(-b * (x - m_0))
+            return ((k - a) * b * exponent) / (v * (c + exponent) ** ((1 / v) + 1))
+        
+        if t is None:
+            return func
+        
+        elif isinstance(t, (float, int, np.ndarray)):
+            return func(t)
+        
+        else:
+            raise ValueError(f"t must be float, int, np.ndarray or None")
+    
+    @staticmethod
+    def _oscillatory_plateau(t: Union[float, np.ndarray, int] = None, a=1, plateau_duration: float = 4,
+                             oscillation_frequency: float = 1.0, oscillation_amplitude: float = 0.1):
+        """
+        Generates an oscillatory plateau based on given parameters.
+    
+        Args:
+            t: Time point(s) to calculate the oscillation. If None, returns the oscillatory function itself.
+            plateau_duration: Duration of the plateau phase in arbitrary units.
+            oscillation_frequency: Frequency of oscillation within the plateau.
+            oscillation_amplitude: Amplitude of the oscillations within the plateau.
+    
+        Returns:
+            The oscillatory plateau value(s) at time t, or the oscillatory function if t is None.
+        """
+        
+        def func(x):
+            
+            if x > plateau_duration or plateau_duration == 0:
+                return 0
+            else:
+                plateau = a + np.cos(2 * np.pi * oscillation_frequency * x) * oscillation_amplitude
+                return plateau
+        
+        if t is None:
+            return func
+        
+        elif isinstance(t, (float, int, np.ndarray)):
+            return func(t)
+        
+        else:
+            raise ValueError(f"t must be float, int, np.ndarray or None")
+    
+    @staticmethod
+    def leaky_integrator(k: float = 0.1, n: float = 1):
+        """
+        Calculate the next state of a leaky integrator system where the leak rate increases with the state's value.
+
+        Args:
+            y: The current state of the system.
+            k: A constant controlling the rate of the leak.
+            n: The exponent controlling how the leak rate scales with the state's value.
+
+        Returns:
+            dy: the change in signal
+
+        """
+        
+        # Calculate the rate of change of Y
+        def func(x, reduce: float = 1):
+            return -k * x ** n * reduce
+        
+        return func
+    
+    def noise_floor(self):
+        noise = np.random.normal() * self.noise_amplitude
+        return noise
+    
+    def _fluctuate_parameter(self, param):
+        
+        if param in [0, 1]:
+            return param
+        else:
+            return np.random.normal(loc=param, scale=self.parameter_fluctuations)
+    
+    def generate_signal(self) -> Union[np.ndarray, None]:
+        """
+        Generates a calcium burst signal with added Gaussian noise.
+
+        Returns:
+          A numpy array representing the generated signal.
+        """
+        
+        # rise parameters
+        a = self._fluctuate_parameter(self.a)
+        k = self._fluctuate_parameter(self.k)
+        c = self._fluctuate_parameter(self.c)
+        b = self._fluctuate_parameter(self.b)
+        v = self._fluctuate_parameter(self.v)
+        m_0 = self._fluctuate_parameter(self.m_0)
+        
+        # plateau parameters
+        plateau_duration = self._fluctuate_parameter(self.plateau_duration)
+        oscillation_frequency = self._fluctuate_parameter(self.oscillation_frequency)
+        oscillation_amplitude = self._fluctuate_parameter(self.oscillation_amplitude)
+        
+        # define functions
+        rise = self._richards_curve(a=a, k=k, c=c, b=b, v=v, m_0=m_0)
+        leaky_integrator = self.leaky_integrator(k=self._fluctuate_parameter(self.leaky_k),
+                                                 n=self._fluctuate_parameter(self.leaky_n))
+        plateau = self._oscillatory_plateau(plateau_duration=plateau_duration,
+                                            oscillation_frequency=oscillation_frequency,
+                                            oscillation_amplitude=oscillation_amplitude)
+        
+        # define trace length
+        length = self.trace_length
+        if self.ragged_allowed:
+            min_length, max_length = length if isinstance(length, (tuple, list)) else (1, length)
+        else:
+            min_length, max_length = length if isinstance(length, (tuple, list)) else (length, length)
+            
+            if max_length is not None and min_length != max_length:
+                raise ValueError(f"min_length != max_length although ragged is not allowed:"
+                                 f" {min_length} vs. {max_length}")
+        
+        if min_length is None:
+            min_length = 1
+        
+        abort_amplitude = self.abort_amplitude if self.abort_amplitude is not None else self.noise_amplitude * 4
+        
+        # define offset
+        offset_0, offset_1 = self.offset if isinstance(self.offset, (tuple, list)) else (self.offset, self.offset)
+        
+        # generate signal
+        signal = []
+        event_occurred = False
+        v = 0
+        t = 0
+        plateau_start = 0
+        phase = 0
+        while True:
+            
+            # add noise
+            v += self.noise_floor()
+            
+            # burst up
+            r = rise(t)
+            v += r
+            
+            # plateau
+            if phase == 2 and plateau_duration > 0:
+                v += plateau(t - plateau_start)
+                v += leaky_integrator(v, reduce=abs(t - plateau_duration) / plateau_duration)
+            
+            # subtract leak
+            else:
+                v += leaky_integrator(v)
+            
+            # deal with negative values
+            if not self.allow_negative_values and v < 0:
+                v = 0
+            
+            # wait for burst to pick up speed
+            if phase == 0 and v > k / 4:
+                phase += 1
+            
+            # wait for burst to lose speed
+            if phase == 1 and len(signal) > 1 and signal[-1] > v + self.noise_amplitude:
+                phase += 1
+                plateau_start = t
+            
+            # wait for plateau to end
+            if phase == 2 and t > plateau_start + plateau_duration:
+                phase += 1
+            
+            # abort conditions
+            if max_length is not None and len(signal) >= max_length:
+                break
+            
+            if phase >= 3 and abs(v) < abort_amplitude:
+                break
+            
+            # save value
+            signal.append(v)
+            t += 1
+        
+        signal = np.array(signal)
+        
+        # add offset
+        if offset_0 is not None:
+            offset_0 = np.array([abs(self.noise_floor()) for _ in range(offset_0)])
+            signal = np.concatenate((offset_0, signal), axis=0)
+        
+        if offset_1 is not None:
+            offset_1 = np.array([abs(self.noise_floor()) for _ in range(offset_1)])
+            signal = np.concatenate((signal, offset_1), axis=0)
+        
+        # enforce signal length
+        if len(signal) < min_length:
+            diff = min_length - len(signal)
+            diff_0, diff_1 = int(diff / 2) + diff % 2, int(diff / 2)
+            
+            diff_0 = np.array([abs(self.noise_floor()) for _ in range(diff_0)])
+            diff_1 = np.array([abs(self.noise_floor()) for _ in range(diff_1)])
+            signal = np.concatenate((diff_0, signal, diff_1), axis=0)
+        
+        if max_length is not None and len(signal) > max_length:
+            logging.warning(f"Generated signal is too long: {len(signal)} !<=  {max_length}")
+            return signal[:max_length]
+        
+        # scale to signal amplitude
+        if self.signal_amplitude is not None:
+            signal = (signal / np.max(signal) * self._fluctuate_parameter(self.signal_amplitude))
+        
+        return signal
+    
+    def generate_signal_population(self, num_signals: int = 1) -> List[np.ndarray]:
+        """
+        Generates a population of signals with unique identifiers.
+
+        Args:
+          num_signals: Number of signals to generate.
+
+        Returns:
+          A list of generated signals.
+        """
+        signals = []
+        iterator = tqdm(range(num_signals)) if self.show_progress else range(num_signals)
+        for _ in iterator:
+            signal = self.generate_signal()
+            
+            if signal is not None:
+                
+                if self.trace_length is None:
+                    signals.append(signal)
+                
+                elif isinstance(self.trace_length, (int, float)):
+                    if len(signal) <= self.trace_length:
+                        signals.append(signal)
+                
+                elif isinstance(self.trace_length, (tuple, list)):
+                    min_, max_ = self.trace_length
+                    if len(signal) >= min_ and len(signal) <= max_:
+                        signals.append(signal)
+        
+        return signals
+
+
 class DummyTensorFlow:
     class keras:
         class utils:
             class Sequence:
                 def __init__(self, *args, **kwargs):
                     pass
 
 
 class DummyGenerator:
     
     def __init__(
-            self, num_rows=25, trace_length=12, ragged=False, offset=0, min_length=2, n_groups=None, n_clusters=None
+            self, num_rows=25, trace_length=12, ragged=False, offset=0, min_length=2,
+            n_groups: Union[int, List[str]] = 1, n_clusters: int = 1, n_subjects: Union[int, List[str]] = 1,
+            timings: List[List[int]] = None, timing_jitter: Union[int, Tuple[float, float]] = None,
+            timing_offset: Union[int, Literal['max']] = 0,
+            z_range: Tuple[int, int] = None,
+            generators: Union[SignalGenerator, List[SignalGenerator]] = None, ratios: List[float] = None
             ):
         
-        self.data = self.get_data(
-                num_rows=num_rows, trace_length=trace_length, ragged=ragged, offset=offset, min_length=min_length
-                )
+        self.generators = [generators] if isinstance(generators, SignalGenerator) else generators
+        self.ratios = ratios
+        self.ragged = True if (isinstance(ragged, str) and ragged == "ragged") else ragged
+        self.n_groups = n_groups
+        self.n_subjects = n_subjects
+        self.identifiers = None
+        
+        self.timings = timings
+        self.z_range = z_range
+        self.timing_jitter = timing_jitter
+        self.timing_offset = timing_offset
+        
+        # random traces
+        if self.generators is None:
+            self.data = self._get_random_data(num_rows=num_rows, trace_length=trace_length,
+                                              ragged=self.ragged, min_length=min_length, offset=offset)
+            
+            self.identifiers = np.random.randint(0, n_clusters, size=len(self.data), dtype=int)
         
-        self.groups = None if n_groups is None else np.random.randint(0, n_groups, size=len(self.data), dtype=int)
-        self.clusters = None if n_clusters is None else np.random.randint(0, n_clusters, size=len(self.data), dtype=int)
+        # signal populations
+        else:
+            self.data, self.identifiers = self._get_signal_population(generators=self.generators,
+                                                                      num_rows=num_rows,
+                                                                      ratios=self.ratios)
     
     @staticmethod
-    def get_data(num_rows, trace_length, ragged, offset, min_length):
-        
-        if isinstance(ragged, str):
-            ragged = True if ragged == "ragged" else False
+    def _get_random_data(num_rows, trace_length, ragged, min_length, offset):
         
         if ragged:
             
             data = []
             for _ in range(num_rows):
                 random_length = max(
                         min_length, trace_length + np.random.randint(low=-trace_length, high=trace_length) + offset
@@ -422,35 +793,165 @@
                 data.append(np.random.random(size=(random_length)))
         
         else:
             data = np.random.random(size=(num_rows, trace_length)) + offset
         
         return data
     
+    @staticmethod
+    def _get_signal_population(generators, num_rows, ratios: List[Tuple] = None,
+                               shuffle: bool = True):
+        """
+        Generates a population of signals according to specified ratios for each generator.
+
+        Args:
+          num_rows: Total size of the population to generate.
+          ratios: List of ratios for each generator. Must sum to 1.
+          shuffle: randomize the population after generation
+
+        Returns:
+          A tuple of two lists: the generated signals and their identifiers.
+        """
+        
+        # calculate ratios
+        if ratios is None:
+            equal_ratio = 1 / len(generators)
+            ratios = [equal_ratio for _ in range(len(generators))]
+        
+        elif sum(ratios) != 1:
+            diff = 1 - sum(ratios)
+            ratios = list(ratios)
+            ratios[-1] += diff
+            logging.warning(f"ratios did not add up to 1; adjusted last entry to {ratios[-1]:.2f} by {diff:.2f}.")
+        
+        assert np.allclose(sum(ratios), 1, rtol=0.01), f"Ratios must sum to 1, not {sum(ratios)} > {ratios}."
+        
+        # generate population
+        population = []
+        identifiers = []
+        for gen_idx, gen in enumerate(generators):
+            
+            num_signals = int(num_rows * ratios[gen_idx])
+            signals = gen.generate_signal_population(num_signals)
+            population.extend(signals)
+            identifiers.extend([gen.identifier] * num_signals)
+        
+        # shuffle
+        if shuffle:
+            indices = list(range(len(population)))
+            random.shuffle(indices)
+            
+            population = [population[i] for i in indices]
+            identifiers = [identifiers[i] for i in indices]
+        
+        return population, identifiers
+    
+    def _create_z_boundaries(self, df: pd.DataFrame) -> pd.DataFrame:
+        
+        timings = self.timings
+        timing_jitter = self.timing_jitter
+        timing_offset = self.timing_offset
+        
+        # create event length column
+        df["dz"] = df.trace.apply(lambda x: len(x))
+        
+        # calculate z_range
+        if self.z_range is None:
+            z_range = (0, max(df.dz.sum() / 2, 1))
+        else:
+            z_range = self.z_range
+        
+        if timings is None:
+            logging.info(f"Creating random z boundaries.")
+            
+            # create random boundaries
+            dz_sum = int(df.dz.sum() / 2)
+            df["z0"] = [np.random.randint(low=z_range[0], high=z_range[1]) for _ in range(len(df))]
+            df["z1"] = df.z0 + df.dz
+        
+        else:
+            
+            num_groups = len(df.group.unique())
+            if len(timings) < num_groups:
+                raise ValueError(f"Length of timings ({len(timings)}) does not equal "
+                                 f"unique group ({num_groups})")
+            elif len(timings) > num_groups:
+                logging.warning(f"Number of timings ({len(timings)}) exceeds number of groups ({num_groups}).")
+            
+            def apply_timings(row):
+                
+                # select timings associated with group
+                group = int(row.group)
+                timing = timings[group]
+                
+                if timing is None:
+                    z0 = np.random.randint(low=z_range[0], high=z_range[1])
+                else:
+                    
+                    if isinstance(timing_jitter, int):
+                        jitter = np.random.randint(low=0, high=timing_jitter)
+                    elif isinstance(timing_jitter, Tuple):
+                        jitter = int(np.random.normal(loc=timing_jitter[0], scale=timing_jitter[1]))
+                    else:
+                        jitter = 0
+                    
+                    if timing_offset == 'max':
+                        chosen_timing = np.random.choice(timing)
+                        idx_max = np.argmax(row.trace)
+                        z0 = chosen_timing + jitter - idx_max
+                    else:
+                        z0 = np.random.choice(timing) + jitter - timing_offset
+                
+                return z0
+            
+            # create boundaries
+            df["z0"] = df.apply(func=apply_timings, axis='columns')
+            df["z1"] = df.z0 + df.dz
+        
+        # create fake index
+        df["idx"] = df.index
+        
+        return df
+    
     def get_dataframe(self):
         
         data = self.data
         
-        if type(data) == list:
+        if isinstance(data, list):
             df = pd.DataFrame(dict(trace=data))
         
-        elif type(data) == np.ndarray:
+        elif isinstance(data, np.ndarray):
             df = pd.DataFrame(dict(trace=data.tolist()))
         else:
-            raise TypeError
+            raise TypeError(f"unknown data type: {type(data)}")
         
-        # create dz, z0 and z1
-        df["dz"] = df.trace.apply(lambda x: len(x))
+        # add a group
+        if self.n_groups is not None:
+            
+            if isinstance(self.n_groups, int):
+                df["group"] = np.random.randint(0, self.n_groups, size=len(self.data), dtype=int)
+            elif isinstance(self.n_groups, List):
+                df["group"] = [np.random.choice(self.n_groups) for _ in range(len(self.data))]
+            else:
+                raise ValueError(f"n_groups has to be of type int or list, not: {type(self.n_groups)}")
+        
+        # add subject id
+        if self.n_subjects is not None:
+            
+            if isinstance(self.n_subjects, int):
+                df["subject_id"] = np.random.randint(0, self.n_subjects, size=len(self.data), dtype=int)
+            elif isinstance(self.n_subjects, list):
+                df["subject_id"] = [np.random.choice(self.n_subjects) for _ in range(len(self.data))]
+            else:
+                raise ValueError(f"n_subjects has to be of type int or list, not: {type(self.n_subjects)}")
         
-        dz_sum = int(df.dz.sum() / 2)
-        df["z0"] = [np.random.randint(low=0, high=max(dz_sum, 1)) for _ in range(len(df))]
-        df["z1"] = df.z0 + df.dz
+        # add a cluster
+        df["cluster"] = self.identifiers
         
-        # create fake index
-        df["idx"] = df.index
+        df = self._create_z_boundaries(df=df)
         
         return df
     
     def get_list(self):
         
         data = self.data
         
@@ -494,27 +995,21 @@
                 chunks = (1, -1) if chunks is None else chunks
                 
                 return da.from_array(data, chunks=chunks)
         
         else:
             return da.from_array(data, chunks="auto")
     
-    def get_events(self):
+    def get_events(self, cache_path=None):
         
         from astrocast.analysis import Events
         
-        ev = Events(event_dir=None)
+        ev = Events(event_dir=None, cache_path=cache_path)
         df = self.get_dataframe()
         
-        if self.groups is not None:
-            df["group"] = self.groups
-        
-        if self.clusters is not None:
-            df["clusters"] = self.clusters
-        
         ev.events = df
         ev.seed = 1
         
         return ev
     
     def get_by_name(self, name, param={}):
         
@@ -523,14 +1018,76 @@
         
         if name not in options.keys():
             raise ValueError(f"unknown attribute: {name}")
         
         return options[name]
 
 
+class DummyMultiGenerator:
+    
+    def __init__(self):
+        pass
+    
+    @staticmethod
+    def get_multi_event(group_names: List[str], num_rows: int, subject_ids: Union[List[str], int],
+                        z_range: Tuple[int, int] = None, ragged=True,
+                        signal_generators: Union[int, List[SignalGenerator]] = 1,
+                        signal_offset: float = 1, encode_clusters: bool = True,
+                        timings: List[List[int]] = None, timing_jitter: Union[int, Tuple[float, float]] = None,
+                        timing_offset: Union[int, Literal['max']] = None,
+                        cache_path: str = "lru_cache", shuffle: bool = True, **kwargs):
+        from astrocast.analysis import MultiEvents
+        
+        offset = 1
+        eObjects = []
+        for idx_g, group_name in enumerate(group_names):
+            
+            if isinstance(signal_generators, int):
+                signal_generators_ = [SignalGenerator(
+                        b=np.random.normal(loc=1.5, scale=0.5) * offset,
+                        plateau_duration=np.random.normal(loc=5, scale=2) * offset,
+                        signal_amplitude=np.random.normal(loc=1, scale=0.5) * offset,
+                        **kwargs
+                        ) for _ in range(signal_generators)]
+            else:
+                signal_generators_ = signal_generators[idx_g]
+            
+            if isinstance(subject_ids, List):
+                subject_ids_ = [f"{sid}_{group_name}" for sid in subject_ids]
+            elif isinstance(subject_ids, int):
+                subject_ids_ = [f"{idx_g * subject_ids + i}" for i in range(subject_ids)]
+            else:
+                raise ValueError(f"unknown type for subject_ids: {type(subject_ids)}")
+            
+            timings_ = timings[idx_g] if timings is not None else None
+            timing_jitter_ = timing_jitter[idx_g] if timing_jitter is not None else None
+            timing_offset_ = timing_offset[idx_g] if timing_offset is not None else None
+            
+            dg = DummyGenerator(num_rows=num_rows, generators=signal_generators_, n_subjects=subject_ids_,
+                                timings=timings_, timing_jitter=timing_jitter_, timing_offset=timing_offset_,
+                                z_range=z_range, ragged=ragged)
+            eObj = dg.get_events()
+            eObj.events["group"] = group_name
+            
+            eObjects.append(eObj)
+            offset *= signal_offset
+        
+        eObj_multi = MultiEvents(event_dirs=eObjects, cache_path=cache_path)
+        
+        if encode_clusters:
+            
+            le = LabelEncoder()
+            eObj_multi.events.cluster = le.fit_transform(eObj_multi.events.cluster.tolist())
+        
+        if shuffle:
+            eObj_multi.events = eObj_multi.events.sample(frac=1).reset_index(drop=True)
+        
+        return eObj_multi
+
+
 class EventSim:
     
     def __init__(self):
         pass
     
     @staticmethod
     def split_3d_array_indices(arr, cz, cx, cy, skip_n):
@@ -947,28 +1504,144 @@
     
     def mean_std(self):
         
         instructions = {0: ["subtract", {"mode": "mean"}], 1: ["divide", {"mode": "std"}]}
         return self.run(instructions)
     
     @staticmethod
-    def get_value(data, mode, population_wide=False, axis=1):
+    def _first(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the first value along the specified axis."""
+        if population_wide:
+            values = np.mean(x[:, 0] if summary_axis else x[0, :])
+        else:
+            values = x[:, 0] if summary_axis else x[0, :]
+        
+        if not population_wide:
+            values = values[:, None]  # broadcasting for downstream calculation
+        
+        return values
+    
+    @staticmethod
+    def _mean(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the mean value along the specified axis."""
+        values = np.mean(x, axis=summary_axis)
+        
+        if not population_wide:
+            values = values[:, None]  # broadcasting for downstream calculation
+        
+        return values
+    
+    @staticmethod
+    def _median(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the median value along the specified axis."""
+        values = np.median(x, axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+        return values
+    
+    @staticmethod
+    def _min(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the minimum value along the specified axis."""
+        values = np.min(x, axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+        return values
+    
+    @staticmethod
+    def _min_abs(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the minimum of absolute values along the specified axis."""
+        values = np.min(np.abs(x), axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+        return values
+    
+    @staticmethod
+    def _max(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the maximum value along the specified axis."""
+        values = np.max(x, axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+        return values
+    
+    @staticmethod
+    def _max_abs(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the maximum of absolute values along the specified axis."""
+        values = np.max(np.abs(x), axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+        return values
+    
+    @staticmethod
+    def _std(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the standard deviation along the specified axis."""
+        values = np.std(x, axis=summary_axis)
+        if not population_wide:
+            values = values[:, None]  # Broadcasting for downstream calculation
+    
+    @staticmethod
+    def _std_mean(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the standard deviation along the specified axis."""
+        
+        if not population_wide:
+            logging.warning(f"'_std_mean' can only be calculated for population wide characteristic; ignoring flag.")
+        
+        if summary_axis is None:
+            summary_axis = 1
+        
+        values = np.std(x, axis=summary_axis)
+        values = np.mean(values)
+        
+        return values
+    
+    @staticmethod
+    def _std_median(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the standard deviation along the specified axis."""
+        
+        if not population_wide:
+            logging.warning(f"'_std_mean' can only be calculated for population wide characteristic; ignoring flag.")
+        
+        if summary_axis is None:
+            summary_axis = 1
         
+        values = np.std(x, axis=summary_axis)
+        values = np.median(values)
+        
+        return values
+    
+    @staticmethod
+    def _std_max(x: Union[da.Array, np.ndarray, ak.Array], population_wide: bool = False, summary_axis: int = None):
+        """Calculate the standard deviation along the specified axis."""
+        
+        if not population_wide:
+            logging.warning(f"'_std_mean' can only be calculated for population wide characteristic; ignoring flag.")
+        
+        if summary_axis is None:
+            summary_axis = 1
+        
+        values = np.std(x, axis=summary_axis)
+        values = np.max(values)
+        
+        return values
+    
+    @staticmethod
+    def get_value(data, mode, population_wide=False, axis=1):
         summary_axis = None if population_wide else axis
         
+        # Dynamically create the mode_options dictionary from methods
         mode_options = {
-            "first":   lambda x: np.mean(x[:, 0] if axis else x[0, :]) if population_wide else x[:, 0] if axis else x[0,
-                                                                                                                    :],
-            "mean":    lambda x: np.mean(x, axis=summary_axis), "min": lambda x: np.min(x, axis=summary_axis),
-            "min_abs": lambda x: np.min(np.abs(x), axis=summary_axis), "max": lambda x: np.max(x, axis=summary_axis),
-            "max_abs": lambda x: np.max(np.abs(x), axis=summary_axis), "std": lambda x: np.std(x, axis=summary_axis)}
-        assert mode in mode_options.keys(), f"please provide valid mode: {mode_options.keys()}"
+            method_name[1:]: method
+            for method_name, method in inspect.getmembers(Normalization, predicate=inspect.isfunction)
+            if method_name.startswith("_")
+            }
+        
+        assert mode in mode_options.keys(), f"please provide valid mode: {list(mode_options.keys())}"
+        
+        ret = mode_options[mode](data, population_wide, summary_axis)
         
-        ret = mode_options[mode](data)
-        return ret if population_wide else ret[:, None]  # broadcasting for downstream calculation
+        return ret
     
     def subtract(self, data, mode="min", population_wide=False, rows=True):
         
         value = self.get_value(data, mode, population_wide, axis=int(rows))
         
         # transpose result if subtracting by columns
         if not rows:
@@ -1100,14 +1773,16 @@
         if cache_path is not None:
             
             if isinstance(cache_path, str):
                 cache_path = Path(cache_path)
             
             if not cache_path.is_dir():
                 cache_path.mkdir()
+                assert cache_path.exists(), f"failed to create cache_path: {cache_path}"
+                logging.info(f"created cache_path at {cache_path}")
         
         self.cache_path = cache_path
         
         # set logging level
         logging.basicConfig(level=logging_level)
     
     @wrapper_local_cache
```

### Comparing `astrocast-0.4.1/astrocast/preparation.py` & `astrocast-0.4.2/astrocast/preparation.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
         if z_slice is not None:
             z0, z1 = z_slice
         
         if lazy:
             data = h5py.File(path.as_posix(), "r")
             
             if loc not in data:
-                raise ValueError(f"cannot find dataset in file ({path}): {list(data.keys())}")
+                raise ValueError(f"cannot find dataset ({loc}) in file ({path}): {list(data.keys())}")
             
             data = data[loc]
             
             if z_slice is not None:
                 data = data[z0:z1]
             
             chunks = self.infer_chunks_from_array(arr=data, strategy=infer_strategy, chunks=chunks)
@@ -781,24 +781,41 @@
                         f"dimensions incorrect: {len(stack.shape)}. Currently not implemented for dim != 3D"
                         )
         
         elif path.is_file():
             # If the path is a file, load a single TIFF file
             
             if lazy:
-                stack = tifffile.imread(path.as_posix())
                 
-                chunks = self.infer_chunks_from_array(stack, strategy=infer_strategy, chunks=chunks)
-                stack = da.from_array(stack, chunks=chunks)
+                (Z, X, Y), _, dtype = get_data_dimensions(path, return_dtype=True)
+                
+                if z_slice is not None:
+                    z_range = range(z0, z1)
+                    Z = z1 - z0
+                else:
+                    z_range = range(Z)
+                
+                chunks = self.infer_chunks((Z, X, Y), dtype=dtype, strategy=infer_strategy,
+                                           chunks=chunks)
+                
+                def imread(key):
+                    return tifffile.imread(path.as_posix(), key=key)
+                
+                stack = [dask.delayed(imread)(z) for z in z_range]
+                stack = [da.from_delayed(x, shape=(X, Y), dtype=dtype) for x in stack]
+                stack = da.stack(stack)
+                
+                stack = da.rechunk(stack, chunks=chunks)
             
             else:
-                stack = tifffile.imread(path.as_posix())
-            
-            if z_slice is not None:
-                stack = stack[z0:z1]
+                
+                if z_slice is not None:
+                    stack = tifffile.imread(path.as_posix(), key=(z0, z1))
+                else:
+                    stack = tifffile.imread(path.as_posix())
         
         else:
             raise FileNotFoundError(f"cannot find directory or file: {path}")
         
         return stack
     
     def save(
```

### Comparing `astrocast-0.4.1/pyproject.toml` & `astrocast-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astrocast"
-version = "0.4.1"
+version = "0.4.2"
 description = "Package to analyze calcium fluorescence events in astrocytes"
 authors = ["Jan Philipp Reising <jan.reising@ki.se>", "Ana Cristina González"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 h5py = "^3.9.0"
 hdbscan = "^0.8.33"
@@ -70,15 +70,15 @@
 pytest = { extras = ["testing"], version = "^7.4.3", optional = true }
 sphinx = { version = "^7.2.6", optional = true }
 sphinx-rtd-theme = { version = "^1.3.0", optional = true }
 sphinx-autodoc-typehints = { version = "^1.25.2", optional = true }
 tensorflow = "*"
 tensorflow-io-gcs-filesystem = { version = "0.31.0", platform = "windows" }
 pyqt5-qt5 = { version = "5.15.2", optional = true }
-build = "^1.0.3"
+build = "0.10.0"
 
 [tool.poetry.scripts]
 astrocast = 'astrocast.cli_interfaces:cli'
 
 [tool.poetry.extras]
 video_player = ["napari", "pyqt5-qt5", "napari-plot", "napari-time-series-plotter", "pydantic"]
 testing = ["pytest", "pytest-cov", "pytest-xdist", "pytest-rerunfailures"]
```

### Comparing `astrocast-0.4.1/PKG-INFO` & `astrocast-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: astrocast
-Version: 0.4.1
+Version: 0.4.2
 Summary: Package to analyze calcium fluorescence events in astrocytes
 Author: Jan Philipp Reising
 Author-email: jan.reising@ki.se
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
 Provides-Extra: doc
 Provides-Extra: testing
 Provides-Extra: video-player
 Requires-Dist: awkward (>=2.4.2,<3.0.0)
-Requires-Dist: build (>=1.0.3,<2.0.0)
+Requires-Dist: build (==0.10.0)
 Requires-Dist: climage (>=0.2.0,<0.3.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colorcet (>=3.0.1,<4.0.0)
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
 Requires-Dist: dask (>=2023.9.2,<2024.0.0)
 Requires-Dist: dask-image (>=2023.8.1,<2024.0.0)
 Requires-Dist: datashader (>=0.15.2,<0.16.0)
```

