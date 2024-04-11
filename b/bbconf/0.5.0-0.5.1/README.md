# Comparing `tmp/bbconf-0.5.0.tar.gz` & `tmp/bbconf-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbconf-0.5.0.tar", last modified: Mon Apr  8 17:10:29 2024, max compression
+gzip compressed data, was "bbconf-0.5.1.tar", last modified: Thu Apr 11 16:55:39 2024, max compression
```

## Comparing `bbconf-0.5.0.tar` & `bbconf-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-08 17:10:21.000000 bbconf-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 17:10:21.000000 bbconf-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 17:10:29.360425 bbconf-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-08 17:10:21.000000 bbconf-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.356425 bbconf-0.5.0/bbconf/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/bbagent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.356425 bbconf-0.5.0/bbconf/config_parser/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/bedbaseconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/config_parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf/models/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/base_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/bed_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/bedset_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/models/drs_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/bedfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    15252 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/bedsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-08 17:10:21.000000 bbconf-0.5.0/bbconf/modules/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/bbconf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 17:10:29.000000 bbconf-0.5.0/bbconf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 17:10:21.000000 bbconf-0.5.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:10:29.360425 bbconf-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 17:10:21.000000 bbconf-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:10:29.360425 bbconf-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_bedfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_bedset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-08 17:10:21.000000 bbconf-0.5.0/tests/test_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.300820 bbconf-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-11 16:55:29.000000 bbconf-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 16:55:29.000000 bbconf-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-11 16:55:39.300820 bbconf-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-11 16:55:29.000000 bbconf-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.292820 bbconf-0.5.1/bbconf/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/bbagent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.296820 bbconf-0.5.1/bbconf/config_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/config_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13506 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/config_parser/bedbaseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/config_parser/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/config_parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.296820 bbconf-0.5.1/bbconf/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/models/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/models/bed_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/models/bedset_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/models/drs_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.296820 bbconf-0.5.1/bbconf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/modules/bedfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15122 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/modules/bedsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-11 16:55:29.000000 bbconf-0.5.1/bbconf/modules/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.300820 bbconf-0.5.1/bbconf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-11 16:55:39.000000 bbconf-0.5.1/bbconf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-11 16:55:39.000000 bbconf-0.5.1/bbconf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:55:39.000000 bbconf-0.5.1/bbconf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-11 16:55:39.000000 bbconf-0.5.1/bbconf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 16:55:39.000000 bbconf-0.5.1/bbconf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.296820 bbconf-0.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-11 16:55:29.000000 bbconf-0.5.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:55:29.000000 bbconf-0.5.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-11 16:55:29.000000 bbconf-0.5.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:55:39.300820 bbconf-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-11 16:55:29.000000 bbconf-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:55:39.300820 bbconf-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-11 16:55:29.000000 bbconf-0.5.1/tests/test_bedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-11 16:55:29.000000 bbconf-0.5.1/tests/test_bedset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-11 16:55:29.000000 bbconf-0.5.1/tests/test_objects.py
```

### Comparing `bbconf-0.5.0/LICENSE.txt` & `bbconf-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/PKG-INFO` & `bbconf-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.5.0
+Version: 0.5.1
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk, Oleksandr Khoroshevskyi
 Author-email: khorosh@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bbconf Version: 0.5.0 Summary: Configuration
+Metadata-Version: 2.1 Name: bbconf Version: 0.5.1 Summary: Configuration
 package for bedbase project Home-page: https://databio.org Author: Michal
 Stolarczyk, Oleksandr Khoroshevskyi Author-email: khorosh@virginia.edu License:
 BSD2 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
```

### Comparing `bbconf-0.5.0/README.md` & `bbconf-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/bbagent.py` & `bbconf-0.5.1/bbconf/bbagent.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/config_parser/bedbaseconfig.py` & `bbconf-0.5.1/bbconf/config_parser/bedbaseconfig.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/config_parser/const.py` & `bbconf-0.5.1/bbconf/config_parser/const.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/config_parser/models.py` & `bbconf-0.5.1/bbconf/config_parser/models.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/db_utils.py` & `bbconf-0.5.1/bbconf/db_utils.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/exceptions.py` & `bbconf-0.5.1/bbconf/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,7 +49,13 @@
     pass
 
 
 class BedSetNotFoundError(BedBaseConfError):
     """Error type for missing bedset"""
 
     pass
+
+
+class BedSetExistsError(BedBaseConfError):
+    """Error type for existing bedset"""
+
+    pass
```

### Comparing `bbconf-0.5.0/bbconf/helpers.py` & `bbconf-0.5.1/bbconf/helpers.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/models/base_models.py` & `bbconf-0.5.1/bbconf/models/base_models.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/models/bed_models.py` & `bbconf-0.5.1/bbconf/models/bed_models.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/models/bedset_models.py` & `bbconf-0.5.1/bbconf/models/bedset_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,10 +32,8 @@
     limit: int
     offset: int
     results: List[BedSetMetadata]
 
 
 class BedSetBedFiles(BaseModel):
     count: int
-    limit: int
-    offset: int
     results: List[BedMetadata]
```

### Comparing `bbconf-0.5.0/bbconf/models/drs_models.py` & `bbconf-0.5.1/bbconf/models/drs_models.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf/modules/bedfiles.py` & `bbconf-0.5.1/bbconf/modules/bedfiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,18 +380,23 @@
                 )
                 if not nofail:
                     raise e
         else:
             _LOGGER.info("upload_pephub set to false. Skipping pephub..")
 
         if upload_qdrant:
-            self.upload_file_qdrant(
-                identifier, files.bed_file.path, {"bed_id": identifier}
-            )
-            _LOGGER.info(f"File uploaded to qdrant. {identifier}")
+            if classification.genome_alias == "hg38":
+                self.upload_file_qdrant(
+                    identifier, files.bed_file.path, {"bed_id": identifier}
+                )
+                _LOGGER.info(f"File uploaded to qdrant. {identifier}")
+            else:
+                _LOGGER.warning(
+                    f"Could not upload to qdrant. Genome: {classification.genome_alias} is not supported."
+                )
         else:
             _LOGGER.info("upload_qdrant set to false. Skipping qdrant..")
 
         # Upload files to s3
         if upload_s3:
             if files:
                 files = self._config.upload_files_s3(
```

### Comparing `bbconf-0.5.0/bbconf/modules/bedsets.py` & `bbconf-0.5.1/bbconf/modules/bedsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import logging
 
-# TODO: will be available in the next geniml release
-# from geniml.io.utils import compute_md5sum_bedset
-from hashlib import md5
+from geniml.io.utils import compute_md5sum_bedset
 from typing import Dict, List
 
 from sqlalchemy import Float, Numeric, func, or_, select
 from sqlalchemy.orm import Session
 
 from bbconf.config_parser import BedBaseConfig
 from bbconf.const import PKG_NAME
 from bbconf.db_utils import BedFileBedSetRelation, BedSets, BedStats, Files
-from bbconf.exceptions import BEDFileNotFoundError, BedSetNotFoundError
+from bbconf.exceptions import (
+    BedSetNotFoundError,
+    BedSetExistsError,
+)
 from bbconf.models.bed_models import BedStatsModel
 from bbconf.models.bedset_models import (
     BedSetBedFiles,
     BedSetListResult,
     BedSetMetadata,
     BedSetPlots,
     BedSetStats,
     FileModel,
+    BedMetadata,
 )
-from bbconf.modules.bedfiles import BedAgentBedFile
 
 _LOGGER = logging.getLogger(PKG_NAME)
 
 
 class BedAgentBedSet:
     """
     Class that represents Bedset in Database.
@@ -162,36 +163,42 @@
         description: str = None,
         statistics: bool = False,
         plots: dict = None,
         upload_pephub: bool = False,
         upload_s3: bool = False,
         local_path: str = "",
         no_fail: bool = False,
+        overwrite: bool = False,
     ) -> None:
         """
         Create bedset in the database.
 
         :param identifier: bedset identifier
         :param name: bedset name
         :param description: bedset description
         :param bedid_list: list of bed file identifiers
         :param statistics: calculate statistics for bedset
         :param plots: dictionary with plots
         :param upload_pephub: upload bedset to pephub (create view in pephub)
         :param upload_s3: upload bedset to s3
         :param local_path: local path to the output files
         :param no_fail: do not raise an error if bedset already exists
+        :param overwrite: overwrite the record in the database
         :return: None
         """
         _LOGGER.info(f"Creating bedset '{identifier}'")
 
         if statistics:
             stats = self._calculate_statistics(bedid_list)
         else:
             stats = None
+        if self.exists(identifier):
+            if not overwrite and not no_fail:
+                raise BedSetExistsError(identifier)
+            self.delete(identifier)
 
         if upload_pephub:
             try:
                 self._create_pephub_view(identifier, description, bedid_list, no_fail)
             except Exception as e:
                 _LOGGER.error(f"Failed to create view in pephub: {e}")
                 if not no_fail:
@@ -199,42 +206,48 @@
 
         new_bedset = BedSets(
             id=identifier,
             name=name,
             description=description,
             bedset_means=stats.mean.model_dump() if stats else None,
             bedset_standard_deviation=stats.sd.model_dump() if stats else None,
-            # md5sum=compute_md5sum_bedset(bedid_list),
-            md5sum=md5("".join(bedid_list).encode()).hexdigest(),
+            md5sum=compute_md5sum_bedset(bedid_list),
         )
 
         if upload_s3:
             plots = BedSetPlots(**plots)
             plots = self.config.upload_files_s3(
                 identifier, files=plots, base_path=local_path, type="bedsets"
             )
 
-        with Session(self._db_engine.engine) as session:
-            session.add(new_bedset)
+        try:
+            with Session(self._db_engine.engine) as session:
+                session.add(new_bedset)
 
-            for bedfile in bedid_list:
-                session.add(
-                    BedFileBedSetRelation(bedset_id=identifier, bedfile_id=bedfile)
-                )
-            if upload_s3:
-                for k, v in plots:
-                    if v:
-                        new_file = Files(
-                            **v.model_dump(exclude_none=True, exclude_unset=True),
-                            bedset_id=identifier,
-                            type="plot",
-                        )
-                        session.add(new_file)
+                if no_fail:
+                    bedid_list = list(set(bedid_list))
+                for bedfile in bedid_list:
+                    session.add(
+                        BedFileBedSetRelation(bedset_id=identifier, bedfile_id=bedfile)
+                    )
+                if upload_s3:
+                    for k, v in plots:
+                        if v:
+                            new_file = Files(
+                                **v.model_dump(exclude_none=True, exclude_unset=True),
+                                bedset_id=identifier,
+                                type="plot",
+                            )
+                            session.add(new_file)
 
-            session.commit()
+                session.commit()
+        except Exception as e:
+            _LOGGER.error(f"Failed to create bedset: {e}")
+            if not no_fail:
+                raise e
 
         _LOGGER.info(f"Bedset '{identifier}' was created successfully")
         return None
 
     def _calculate_statistics(self, bed_ids: List[str]) -> BedSetStats:
         """
         Calculate statistics for bedset.
@@ -259,16 +272,18 @@
                 sd_bedset_statement = select(
                     func.round(
                         func.stddev(getattr(BedStats, column_name)).cast(Numeric),
                         4,
                     ).cast(Float)
                 ).where(BedStats.id.in_(bed_ids))
 
-                bedset_sd[column_name] = session.execute(mean_bedset_statement).one()[0]
-                bedset_mean[column_name] = session.execute(sd_bedset_statement).one()[0]
+                bedset_sd[column_name] = session.execute(sd_bedset_statement).one()[0]
+                bedset_mean[column_name] = session.execute(mean_bedset_statement).one()[
+                    0
+                ]
 
             bedset_stats = BedSetStats(
                 mean=bedset_mean,
                 sd=bedset_sd,
             )
 
         _LOGGER.info("Bedset statistics were calculated successfully")
@@ -337,49 +352,34 @@
         return BedSetListResult(
             count=len(result_list),
             limit=limit,
             offset=offset,
             results=result_list,
         )
 
-    def get_bedset_bedfiles(
-        self, identifier: str, full: bool = False, limit: int = 100, offset: int = 0
-    ) -> BedSetBedFiles:
+    def get_bedset_bedfiles(self, identifier: str) -> BedSetBedFiles:
         """
         Get list of bedfiles in bedset.
 
         :param identifier: bedset identifier
-        :param full: return full records with stats, plots, files and metadata
-        :param limit: limit of results
-        :param offset: offset of results
 
         :return: list of bedfiles
         """
-        bed_object = BedAgentBedFile(self.config)
-
-        statement = (
-            select(BedFileBedSetRelation)
-            .where(BedFileBedSetRelation.bedset_id == identifier)
-            .limit(limit)
-            .offset(offset)
-        )
+        statement = select(BedSets).where(BedSets.id == identifier)
 
         with Session(self._db_engine.engine) as session:
-            bedfiles = session.execute(statement).all()
-        results = []
-        for bedfile in bedfiles:
-            try:
-                results.append(bed_object.get(bedfile[0].bedfile_id, full=full))
-            except BEDFileNotFoundError as _:
-                _LOGGER.error(f"Bedfile {bedfile[0].bedfile_id} not found")
+            bedset_obj = session.scalar(statement)
+            bedfiles_list = bedset_obj.bedfiles
+
+            results = [
+                BedMetadata(**bedfile.bedfile.__dict__) for bedfile in bedfiles_list
+            ]
 
         return BedSetBedFiles(
             count=len(results),
-            limit=limit,
-            offset=offset,
             results=results,
         )
 
     def delete(self, identifier: str) -> None:
         """
         Delete bed file from the database.
```

### Comparing `bbconf-0.5.0/bbconf/modules/objects.py` & `bbconf-0.5.1/bbconf/modules/objects.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/bbconf.egg-info/PKG-INFO` & `bbconf-0.5.1/bbconf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbconf
-Version: 0.5.0
+Version: 0.5.1
 Summary: Configuration package for bedbase project
 Home-page: https://databio.org
 Author: Michal Stolarczyk, Oleksandr Khoroshevskyi
 Author-email: khorosh@virginia.edu
 License: BSD2
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bbconf Version: 0.5.0 Summary: Configuration
+Metadata-Version: 2.1 Name: bbconf Version: 0.5.1 Summary: Configuration
 package for bedbase project Home-page: https://databio.org Author: Michal
 Stolarczyk, Oleksandr Khoroshevskyi Author-email: khorosh@virginia.edu License:
 BSD2 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics Description-
```

### Comparing `bbconf-0.5.0/bbconf.egg-info/SOURCES.txt` & `bbconf-0.5.1/bbconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/setup.py` & `bbconf-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/tests/test_bedfile.py` & `bbconf-0.5.1/tests/test_bedfile.py`

 * *Files identical despite different names*

### Comparing `bbconf-0.5.0/tests/test_bedset.py` & `bbconf-0.5.1/tests/test_bedset.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,14 @@
     def test_get_get_bedset_bedfiles(self, bbagent_obj):
         with ContextManagerDBTesting(
             config=bbagent_obj.config, add_data=True, bedset=True
         ):
             result = bbagent_obj.bedset.get_bedset_bedfiles(BEDSET_TEST_ID)
 
             assert result.count == 1
-            assert result.limit == 100
-            assert result.offset == 0
             assert len(result.results) == 1
 
     def test_delete(self, bbagent_obj, mocker):
         with ContextManagerDBTesting(
             config=bbagent_obj.config, add_data=True, bedset=True
         ):
             mocker.patch(
```

### Comparing `bbconf-0.5.0/tests/test_objects.py` & `bbconf-0.5.1/tests/test_objects.py`

 * *Files identical despite different names*

