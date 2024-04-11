# Comparing `tmp/noisepy_seis_io-0.1.9.tar.gz` & `tmp/noisepy_seis_io-0.1.dev1.tar.gz`

## Comparing `noisepy_seis_io-0.1.9.tar` & `noisepy_seis_io-0.1.dev1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/_version.py
--rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/asdfstore.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/channel_filter_store.py
--rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/channelcatalog.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/constants.py
--rw-r--r--   0        0        0    16699 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/datatypes.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/hierarchicalstores.py
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/numpystore.py
--rw-r--r--   0        0        0    10119 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/scedc_s3store.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/stores.py
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/utils.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/src/noisepy/seis/io/zarrstore.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/LICENSE
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/README.md
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/_version.py
+-rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/asdfstore.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/channel_filter_store.py
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/channelcatalog.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/constants.py
+-rw-r--r--   0        0        0    16699 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/datatypes.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/hierarchicalstores.py
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/numpystore.py
+-rw-r--r--   0        0        0    10776 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/scedc_s3store.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/stores.py
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/utils.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/zarrstore.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/LICENSE
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/README.md
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 noisepy_seis_io-0.1.dev1/PKG-INFO
```

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/asdfstore.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/channel_filter_store.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/channel_filter_store.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from typing import Callable, List
+from typing import List
 
 import obspy
 from datetimerange import DateTimeRange
 
-from noisepy.seis.io.constants import WILD_CARD
 from noisepy.seis.io.datatypes import Channel, ChannelData, Station
 from noisepy.seis.io.stores import RawDataStore
 
-from .constants import WILD_CARD
-
 
 class LocationChannelFilterStore(RawDataStore):
     """
     This 'store' simply wraps another store and filters out duplicate channels that differ only
     by location. It does this by keeping the channel with the 'lowest' (lexicographic) location code.
     """
 
@@ -37,24 +34,7 @@
             if key not in min_chans:
                 min_chans[key] = ch
             # lexicographic comparison of location codes
             #  http://docs.python.org/reference/expressions.html
             elif ch.type.location < min_chans[key].type.location:
                 min_chans[key] = ch
         return list(min_chans.values())
-
-
-def channel_filter(
-    net_list: List[str], sta_list: List[str], cha_list: List[str]
-) -> Callable[[Channel], bool]:
-    stations = set(sta_list)
-    networks = set(net_list)
-    channels = set(cha_list)
-
-    def filter(ch: Channel) -> bool:
-        return (
-            (WILD_CARD in stations or ch.station.name in stations)
-            and (WILD_CARD in networks or ch.station.network in networks)
-            and (WILD_CARD in channels or ch.type.name in channels)
-        )
-
-    return filter
```

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/channelcatalog.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/datatypes.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/hierarchicalstores.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/hierarchicalstores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/numpystore.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/numpystore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/scedc_s3store.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/scedc_s3store.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,32 @@
 
 from .datatypes import Channel, ChannelData, ChannelType, Station
 from .utils import TimeLogger, fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 
 
+def channel_filter(stations: List[str], ch_prefixes: str) -> Callable[[Channel], bool]:
+    """
+    Helper function for creating a channel filter to be used in the constructor of the store.
+    This filter uses a list of allowed station name along with a channel filter prefix.
+    """
+    sta_set = set(stations)
+
+    def filter(ch: Channel) -> bool:
+        if sta_set == {"*"}:
+            return ch.type.name.lower().startswith(tuple(ch_prefixes.lower().split(",")))
+        else:
+            return ch.station.name in sta_set and ch.type.name.lower().startswith(
+                tuple(ch_prefixes.lower().split(","))
+            )
+
+    return filter
+
+
 class MiniSeedS3DataStore(RawDataStore):
     """
     A data store implementation to read from a directory of miniSEED (.ms) files from an S3 bucket.
     Every directory is a a day and each .ms file contains the data for a channel.
     """
 
     def __init__(
```

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/stores.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/utils.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,26 @@
 import psutil
 from tqdm.autonotebook import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 
 from noisepy.seis.io.constants import AWS_EXECUTION_ENV
 
 S3_SCHEME = "s3"
-HTTPS_SCHEME = "https"
 FIND_RETRIES = 5
 FIND_RETRY_SLEEP = 0.1  # (100ms)
 utils_logger = logging.getLogger(__name__)
 
 
 def get_filesystem(path: str, storage_options: dict = {}) -> fsspec.AbstractFileSystem:
     """Construct an fsspec filesystem for the given path"""
     url = urlparse(path)
     # The storage_options coming from the ConfigParameters is keyed by protocol
     storage_options = storage_options.get(url.scheme, storage_options)
     if url.scheme == S3_SCHEME:
         return fsspec.filesystem(url.scheme, **storage_options)
-    elif url.scheme == HTTPS_SCHEME:
-        return fsspec.filesystem(url.scheme)
     else:
         return fsspec.filesystem("file", **storage_options)
 
 
 def fs_join(path1: str, path2: str) -> str:
     """Helper for joining two paths that can handle both S3 URLs and local file system paths"""
     url = urlparse(path1)
@@ -43,16 +40,18 @@
     else:
         return os.path.join(path1, path2)
 
 
 def get_fs_sep(path1: str) -> str:
     """Helper for getting a path separator that can handle both S3 URLs and local file system paths"""
     url = urlparse(path1)
-    fs = fsspec.filesystem(url.scheme)
-    return fs.sep
+    if url.scheme == S3_SCHEME:
+        return posixpath.sep
+    else:
+        return os.sep
 
 
 def io_retry(func: Callable, *args, **kwargs) -> Any:
     """
     Retry the given function up to FIND_RETRIES times if an OSError(EBUSY) is raised, sleeping between retries.
     If the function still fails, the exception is raised.
     """
```

### Comparing `noisepy_seis_io-0.1.9/src/noisepy/seis/io/zarrstore.py` & `noisepy_seis_io-0.1.dev1/src/noisepy/seis/io/zarrstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/.gitignore` & `noisepy_seis_io-0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/LICENSE` & `noisepy_seis_io-0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/README.md` & `noisepy_seis_io-0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis_io-0.1.9/pyproject.toml` & `noisepy_seis_io-0.1.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
     "fsspec>=2023.4.0,<2024.0.0",
     "s3fs==2023.4.0,<2024.0.0",
     "zarr==2.14.2",
     "pydantic==2.3.0",
     "PyYAML==6.0",
     "pydantic-yaml==1.0",
     "psutil>=5.9.5,<6.0.0",
-    "tqdm",
-    "diskcache",
 ]
 # On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
```

### Comparing `noisepy_seis_io-0.1.9/PKG-INFO` & `noisepy_seis_io-0.1.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis-io
-Version: 0.1.9
+Version: 0.1.dev1
 Project-URL: Homepage, https://github.com/noisepy/noisepy-io
 Author-email: Marine Denolle <mdenolle@uw.edu>, Carlos Suarez <carlosg@uw.edu>, Ishika Khandelwal <ishikakhandelwal02@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ishika Khandelwal
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,25 +28,23 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Dist: datetimerange<3.0.0,>=2.0.0
-Requires-Dist: diskcache
 Requires-Dist: fsspec<2024.0.0,>=2023.4.0
 Requires-Dist: numpy<2.0.0,>=1.22.0
 Requires-Dist: pandas<2.0.0,>=1.5.3
 Requires-Dist: psutil<6.0.0,>=5.9.5
 Requires-Dist: pyasdf<1.0.0,>=0.7.5
 Requires-Dist: pydantic-yaml==1.0
 Requires-Dist: pydantic==2.3.0
 Requires-Dist: pyyaml==6.0
 Requires-Dist: s3fs<2024.0.0,==2023.4.0
-Requires-Dist: tqdm
 Requires-Dist: zarr==2.14.2
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
 Requires-Dist: matplotlib; extra == 'dev'
 Requires-Dist: nbconvert; extra == 'dev'
 Requires-Dist: nbsphinx; extra == 'dev'
```

