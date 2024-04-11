# Comparing `tmp/responsibleai_vision-0.3.6.tar.gz` & `tmp/responsibleai_vision-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.3.6.tar", last modified: Mon Feb 12 19:36:24 2024, max compression
+gzip compressed data, was "responsibleai_vision-0.3.7.tar", last modified: Thu Apr 11 20:22:11 2024, max compression
```

## Comparing `responsibleai_vision-0.3.6.tar` & `responsibleai_vision-0.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.113860 responsibleai_vision-0.3.6/responsibleai_vision/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/responsibleai_vision/common/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/common/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/responsibleai_vision/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/managers/error_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    29096 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/managers/explainer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/responsibleai_vision/rai_vision_insights/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/rai_vision_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49549 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/responsibleai_vision/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/utils/feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/utils/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/responsibleai_vision/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-12 19:36:24.000000 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-12 19:36:24.000000 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 19:36:24.000000 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-12 19:36:24.000000 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-12 19:36:24.000000 responsibleai_vision-0.3.6/responsibleai_vision.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 19:36:24.117860 responsibleai_vision-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/tests/test_feature_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/tests/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/tests/test_rai_vision_automl_images_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/tests/test_rai_vision_insights.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-02-12 19:32:20.000000 responsibleai_vision-0.3.6/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.993970 responsibleai_vision-0.3.7/responsibleai_vision/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/common/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/error_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29096 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/managers/explainer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49549 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/responsibleai_vision/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 20:22:10.000000 responsibleai_vision-0.3.7/responsibleai_vision.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:22:10.997970 responsibleai_vision-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7035 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_feature_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_automl_images_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_insights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-11 20:18:12.000000 responsibleai_vision-0.3.7/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.3.6/PKG-INFO` & `responsibleai_vision-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.3.6
+Version: 0.3.7
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7"
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
 Requires-Dist: responsibleai>=0.34.1
-Requires-Dist: torchmetrics
+Requires-Dist: torchmetrics[detection]
 Requires-Dist: vision_explanation_methods
 
 # Responsible AI Vision SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8 and 3.9
 
 The Responsible AI Vision SDK enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
```

### Comparing `responsibleai_vision-0.3.6/README.md` & `responsibleai_vision-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.3.7/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.3.7/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.3.7/responsibleai_vision/managers/explainer_manager.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.3.7/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.3.7/responsibleai_vision/utils/feature_extractors.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 
 """Defines the feature extractors."""
 
 import warnings
 from typing import Optional
 
 import pandas as pd
-from PIL import Image
+from PIL import ExifTags, Image
 from PIL.ExifTags import TAGS
+from PIL.TiffImagePlugin import IFDRational
 from tqdm import tqdm
 
 from responsibleai.feature_metadata import FeatureMetadata
 from responsibleai_vision.common.constants import (ExtractedFeatures,
                                                    ImageColumns)
 from responsibleai_vision.utils.image_reader import (
-    get_all_exif_feature_names, get_image_from_path,
+    IFD_CODE_LOOKUP, get_all_exif_feature_names, get_image_from_path,
     get_image_pointer_from_path)
 
 MEAN_PIXEL_VALUE = ExtractedFeatures.MEAN_PIXEL_VALUE.value
 MAX_CUSTOM_LEN = 100
 IMAGE_DETAILS = ImageColumns.IMAGE_DETAILS.value
 
 
@@ -87,39 +88,52 @@
             if has_dropped_features and column_names[j] in dropped_features:
                 continue
             row_feature_values.append(image_dataset.iloc[i, j])
         results.append(row_feature_values)
     return results, feature_names
 
 
-def append_exif_features(image, row_feature_values, feature_names,
-                         blacklisted_tags, feature_metadata):
+def process_data(data,
+                 tag,
+                 feature_names,
+                 feature_metadata,
+                 row_feature_values,
+                 blacklisted_tags):
+    if isinstance(data, IFDRational):
+        data = data.numerator / data.denominator
+    if isinstance(data, (str, int, float)):
+        if tag in feature_names:
+            if tag not in feature_metadata.categorical_features:
+                feature_metadata.categorical_features.append(tag)
+            row_feature_values[feature_names.index(tag)] = data
+        elif tag not in blacklisted_tags:
+            blacklisted_tags.add(tag)
+            warnings.warn(
+                f'Exif tag {tag} could not be found '
+                'in the feature names. Ignoring tag '
+                'from extracted metadata.')
+
+
+def append_exif_features(image,
+                         row_feature_values,
+                         feature_names,
+                         blacklisted_tags,
+                         feature_metadata):
     if isinstance(image, str):
         image_pointer_path = get_image_pointer_from_path(image)
         with Image.open(image_pointer_path) as im:
             exifdata = im.getexif()
             for tag_id in exifdata:
-                # get the tag name, instead of human unreadable tag id
-                tag = str(TAGS.get(tag_id, tag_id))
-                data = exifdata.get(tag_id)
-                # decode bytes
-                if isinstance(data, bytes):
-                    data = data.decode()
-                    if len(data) > MAX_CUSTOM_LEN:
-                        data = data[:MAX_CUSTOM_LEN] + '...'
-                if isinstance(data, str):
-                    if tag in feature_names:
-                        if tag not in feature_metadata.categorical_features:
-                            feature_metadata.categorical_features.append(tag)
-                        tag_index = feature_names.index(tag)
-                        row_feature_values[tag_index] = data
-                    else:
-                        # in theory this should now never happen with
-                        # latest code, but adding this check for safety
-                        if tag not in blacklisted_tags:
-                            blacklisted_tags.add(tag)
-                            warnings.warn(
-                                f'Exif tag {tag} could not be found '
-                                'in the feature names. Ignoring tag '
-                                'from extracted metadata.')
-                elif isinstance(data, int) or isinstance(data, float):
-                    row_feature_values[feature_names.index(tag)] = data
+                if tag_id in IFD_CODE_LOOKUP:
+                    ifd_data = exifdata.get_ifd(tag_id)
+                    for nested_tag_id, data in ifd_data.items():
+                        tag = ExifTags.GPSTAGS.get(nested_tag_id, None) \
+                            or ExifTags.TAGS.get(nested_tag_id, None) \
+                            or nested_tag_id
+                        process_data(data, tag, feature_names,
+                                     feature_metadata, row_feature_values,
+                                     blacklisted_tags)
+                else:
+                    tag = str(TAGS.get(tag_id, tag_id))
+                    data = exifdata.get(tag_id)
+                    process_data(data, tag, feature_names, feature_metadata,
+                                 row_feature_values, blacklisted_tags)
```

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.3.7/responsibleai_vision/utils/image_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 import base64
 from io import BytesIO
 from typing import Any, Tuple, Union
 from urllib.parse import urlparse
 
 import requests
 from numpy import asarray
-from PIL import Image
+from PIL import ExifTags, Image
 from PIL.ExifTags import TAGS
 from requests.adapters import HTTPAdapter, Retry
 
 from responsibleai_vision.common.constants import (AutoMLImagesModelIdentifier,
                                                    CommonTags)
 
 # domain mapped session for reuse
 _requests_sessions = {}
 
+IFD_CODE_LOOKUP = {t.value: t.name for t in ExifTags.IFD}
+
 
 def _get_retry_session(url):
     domain = urlparse(url.lower()).netloc
     if domain in _requests_sessions:
         return _requests_sessions[domain]
 
     session = requests.Session()
@@ -84,23 +86,30 @@
     for i in range(image_dataset.shape[0]):
         image = image_dataset.iloc[i, 0]
         if isinstance(image, str):
             image_pointer_path = get_image_pointer_from_path(image)
             with Image.open(image_pointer_path) as im:
                 exifdata = im.getexif()
                 for tag_id in exifdata:
-                    # get the tag name, instead of human unreadable tag id
-                    tag = TAGS.get(tag_id, tag_id)
-                    if tag not in image_dataset.columns:
-                        data = exifdata.get(tag_id)
-                        if isinstance(data, str) or \
-                           isinstance(data, int) or \
-                           isinstance(data, float) or \
-                           isinstance(data, bytes):
+                    # nesting for IFD block tags
+                    if tag_id in IFD_CODE_LOOKUP:
+                        ifd_data = exifdata.get_ifd(tag_id)
+
+                        for nested_tag_id in ifd_data:
+                            nested_tag = ExifTags.GPSTAGS.get(nested_tag_id,
+                                                              None) \
+                                or ExifTags.TAGS.get(nested_tag_id, None) \
+                                or nested_tag_id
+                            exif_feature_names.add(nested_tag)
+                    else:
+                        # get the tag name, instead of human unreadable tag id
+                        tag = TAGS.get(tag_id, tag_id)
+                        if tag not in image_dataset.columns:
                             exif_feature_names.add(tag)
+
     return list(exif_feature_names)
 
 
 def get_base64_string_from_path(
     img_path: str, return_image_size: bool = False
 ) -> Union[str, Tuple[str, Tuple[int, int]]]:
     """Load and convert pillow image to base64-encoded image
```

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.3.7/responsibleai_vision/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.3.7/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.3.6
+Version: 0.3.7
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: Pillow>=10.0.0; python_version > "3.7"
 Requires-Dist: Pillow<10.0.0; python_version <= "3.7"
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: semver~=2.13.0
 Requires-Dist: responsibleai>=0.34.1
-Requires-Dist: torchmetrics
+Requires-Dist: torchmetrics[detection]
 Requires-Dist: vision_explanation_methods
 
 # Responsible AI Vision SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8 and 3.9
 
 The Responsible AI Vision SDK enables users to analyze their machine learning models for computer vision in one API. Users will be able to analyze errors, explain the most important features, and understand their data using a single API.
```

### Comparing `responsibleai_vision-0.3.6/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.3.7/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/setup.py` & `responsibleai_vision-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/tests/test_image_utils.py` & `responsibleai_vision-0.3.7/tests/test_image_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from collections import Counter
 from http.client import HTTPMessage
 from math import isclose
 from unittest.mock import Mock, patch
 from urllib.parse import urlparse
 
 import numpy as np
-from common_vision_utils import load_fridge_object_detection_dataset
+from common_vision_utils import (load_clearsight_object_detection_dataset,
+                                 load_fridge_object_detection_dataset)
 
 from responsibleai_vision.common.constants import ImageColumns
 from responsibleai_vision.utils.image_reader import \
     _get_retry_session as image_reader_get_retry_session
 from responsibleai_vision.utils.image_reader import \
     _requests_sessions as image_reader_requests_sessions
 from responsibleai_vision.utils.image_reader import get_all_exif_feature_names
@@ -91,19 +92,20 @@
         session = image_reader_get_retry_session(url)
 
         assert session.get(url).status_code == 200
 
     def test_get_all_exif_feature_names(self):
         image_dataset = load_fridge_object_detection_dataset().head(2)
         exif_feature_names = get_all_exif_feature_names(image_dataset)
-        assert len(exif_feature_names) == 11
-        assert set(exif_feature_names) == \
-            set(['Orientation', 'ExifOffset', 'ImageWidth', 'GPSInfo',
-                 'Model', 'DateTime', 'YCbCrPositioning', 'ImageLength',
-                 'ResolutionUnit', 'Software', 'Make'])
+        assert len(exif_feature_names) == 60
+
+    def test_get_all_clearsight_feature_names(self):
+        image_dataset = load_clearsight_object_detection_dataset().head(2)
+        exif_feature_names = get_all_exif_feature_names(image_dataset)
+        assert len(exif_feature_names) == 64
 
     def test_generate_od_error_labels(self):
         true_y = np.array([[[3, 142, 257, 395, 463, 0]],
                            [[3, 107, 272, 240, 501, 0],
                             [1, 261, 274, 393, 449, 0]],
                            [[4, 139, 253, 339, 506, 0]],
                            [[2, 100, 173, 233, 521, 0]],
```

### Comparing `responsibleai_vision-0.3.6/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.3.7/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.3.7/tests/test_rai_vision_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.3.6/tests/test_rai_vision_insights_save_and_load_scenarios.py` & `responsibleai_vision-0.3.7/tests/test_rai_vision_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*

