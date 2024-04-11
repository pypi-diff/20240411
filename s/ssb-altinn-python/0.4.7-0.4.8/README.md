# Comparing `tmp/ssb_altinn_python-0.4.7.tar.gz` & `tmp/ssb_altinn_python-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.4.7.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.4.8.tar", max compression
```

## Comparing `ssb_altinn_python-0.4.7.tar` & `ssb_altinn_python-0.4.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/LICENSE
--rw-r--r--   0        0        0     8257 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/README.md
--rw-r--r--   0        0        0     4351 2024-03-18 13:46:40.358244 ssb_altinn_python-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      325 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/__init__.py
--rw-r--r--   0        0        0      198 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/__main__.py
--rw-r--r--   0        0        0     2207 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/file.py
--rw-r--r--   0        0        0    12279 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/flatten.py
--rw-r--r--   0        0        0     4276 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/parser.py
--rw-r--r--   0        0        0        0 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/py.typed
--rw-r--r--   0        0        0     1378 2024-03-18 13:46:28.462329 ssb_altinn_python-0.4.7/src/altinn/utils.py
--rw-r--r--   0        0        0     9334 1970-01-01 00:00:00.000000 ssb_altinn_python-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 08:17:12.838420 ssb_altinn_python-0.4.8/LICENSE
+-rw-r--r--   0        0        0     9093 2024-04-11 08:17:12.838420 ssb_altinn_python-0.4.8/README.md
+-rw-r--r--   0        0        0     4352 2024-04-11 08:17:22.990492 ssb_altinn_python-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      325 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/__init__.py
+-rw-r--r--   0        0        0      198 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/__main__.py
+-rw-r--r--   0        0        0     2207 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/file.py
+-rw-r--r--   0        0        0    12654 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/flatten.py
+-rw-r--r--   0        0        0     4245 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/py.typed
+-rw-r--r--   0        0        0     1378 2024-04-11 08:17:12.842420 ssb_altinn_python-0.4.8/src/altinn/utils.py
+-rw-r--r--   0        0        0    10170 1970-01-01 00:00:00.000000 ssb_altinn_python-0.4.8/PKG-INFO
```

### Comparing `ssb_altinn_python-0.4.7/LICENSE` & `ssb_altinn_python-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.7/README.md` & `ssb_altinn_python-0.4.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,32 @@
 
 mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
            'kontAmbulForeDispAnt':'ISEE_VAR2',
            'kontAmbulForeDriftAnt':'ISEE_VAR3',}
 
 isee_transform(file, mapping)
 ```
+
+If you need to flatten more than 'SkjemaData' from the XML, you can make a list of the tags in the XML you need to flatten, and add this list as an argument (tag_list) when running the function isee_transform(file, taglist=taglist). The default value is 'SkjemaData', so if you only need to flatten this, its not needed to pass the argument tag_list.
+
+```python
+from altinn import isee_transform
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
+
+mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
+           'kontAmbulForeDispAnt':'ISEE_VAR2',
+           'kontAmbulForeDriftAnt':'ISEE_VAR3',
+           'kontaktPersonNavn'; 'ISEE_KONTAKTPERSON',}
+
+tags = ['SkjemaData', 'Kontakt']
+
+isee_transform(file, mapping, tag_list=tags)
+```
+
 The function handles flat structures and 'tables' in the XML. If the XML contains repeating values, it puts a suffix containig a number at the end of the FELTNAVN-column. If the XML-contains more complex structures as 'table in table' if will give a warning with a list of which values in FELTNAVN that needs to be further processed before it can be used in ISEE.
 
 The XML needs to contain certain fields in the 'InternInfo'-block, The required filds are:
 - 'enhetsIdent'
 - 'enhetsType'
 - 'delregNr'
```

### Comparing `ssb_altinn_python-0.4.7/pyproject.toml` & `ssb_altinn_python-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.4.7"
+version = "0.4.8"
 description = "SSB Altinn Python"
 authors = ["Vidar Strandseter <vidar.strandseter@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-altinn-python"
 repository = "https://github.com/statisticsnorway/ssb-altinn-python"
 documentation = "https://statisticsnorway.github.io/ssb-altinn-python"
@@ -74,15 +74,15 @@
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 force-exclude = true  # Apply excludes to pre-commit
 show-fixes = true
 src = ["src", "tests"]
-target-version = "py39"  # Minimum Python version supported
+target-version = "py310"  # Minimum Python version supported
 include = ["*.py", "*.pyi", "**/pyproject.toml", "*.ipynb"]
 extend-exclude = [
     "__pycache__",
     "old",
     ".ipynb_checkpoints",
     "noxfile.py",
     "docs/conf.py",
```

### Comparing `ssb_altinn_python-0.4.7/src/altinn/file.py` & `ssb_altinn_python-0.4.8/src/altinn/file.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.7/src/altinn/flatten.py` & `ssb_altinn_python-0.4.8/src/altinn/flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 of Altinn3. This is done in a separate file.
 """
 
 import re
 import xml.etree.ElementTree as ET
 from collections.abc import MutableMapping
 from typing import Any
-from typing import Optional
 
 import pandas as pd
 import xmltodict
 from dapla import FileClient
 
 from altinn import utils
 
@@ -227,50 +226,61 @@
 
     df = df.drop(["COUNTER", "LEVELS"], axis=1)
 
     return df
 
 
 def isee_transform(
-    file_path: str, mapping: Optional[dict[str, str]] = None
+    file_path: str,
+    mapping: dict[str, str] | None = None,
+    tag_list: list[str] | None = None,
 ) -> pd.DataFrame:
     """Transforms a XML to ISEE-format using xmltodict.
 
     Transforms the XML to ISEE-format by using xmltodict to transform the XML
     to a dictionary. Traverses/scans the key/values in dictionary for lists,
     dicts and simple values.
     Stores the results in a list of dictionaries, that converts to a DataFrame
 
     Args:
         file_path: The path to the XML file.
         mapping: The mapping dictionary to map variable names in the
             'feltnavn' column. The default value is an empty dictionary
             (if mapping is not needed).
+        tag_list: A list containing the tags in the XML that will be flatten
+            The default value is ['SkjemaData']
 
     Returns:
         pandas.DataFrame: A transformed DataFrame which aligns with the
         ISEE dynarev format.
 
     Raises:
         ValueError: If invalid gcs-file or xml-file.
     """
     if utils.is_valid_xml(file_path):
         if _validate_interninfo(file_path):
             if mapping is None:
                 mapping = {}
 
+            if tag_list is None:
+                tag_list = ["SkjemaData"]
+
             xml_dict = _read_single_xml_to_dict(file_path)
             root_element = next(iter(xml_dict.keys()))
-            input_dict = xml_dict[root_element]["SkjemaData"]
 
-            final_dict = _flatten_dict(input_dict)
+            final_df = pd.DataFrame()
 
-            final_df = pd.DataFrame(
-                list(final_dict.items()), columns=["FELTNAVN", "FELTVERDI"]
-            )
+            for tag in tag_list:
+                input_dict = xml_dict[root_element][tag]
+                tag_dict = _flatten_dict(input_dict)
+                tag_df = pd.DataFrame(
+                    list(tag_dict.items()), columns=["FELTNAVN", "FELTVERDI"]
+                )
+
+                final_df = pd.concat([final_df, tag_df], axis=0, ignore_index=True)
 
             final_df["IDENT_NR"] = xml_dict[root_element]["InternInfo"]["enhetsIdent"]
             final_df["VERSION_NR"] = _extract_angiver_id(file_path)
             final_df["DELREG_NR"] = xml_dict[root_element]["InternInfo"]["delregNr"]
             final_df["ENHETS_TYPE"] = xml_dict[root_element]["InternInfo"]["enhetsType"]
             final_df["SKJEMA_ID"] = (
                 xml_dict[root_element]["InternInfo"]["raNummer"] + "A3"
```

### Comparing `ssb_altinn_python-0.4.7/src/altinn/parser.py` & `ssb_altinn_python-0.4.8/src/altinn/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """This module contains the main function for running the Altinn application."""
 
 import os
 from typing import Any
-from typing import Optional
 from xml.etree.ElementTree import Element
 
 import pandas as pd
 from dapla import FileClient
 from defusedxml import ElementTree
 
 from .utils import is_gcs
@@ -35,15 +34,15 @@
         if not is_valid_xml(self.file_path):
             print("""File is not a valid XML-file.""")
 
     def traverse_xml(
         self,
         element: Element,
         column_counter: int = 1,
-        data: Optional[dict[str, Any]] = None,
+        data: dict[str, Any] | None = None,
     ) -> dict[str, Any]:
         """Recursively traverse an XML element and extract data.
 
         Args:
             element: The XML element to traverse.
             column_counter (int): The counter for generating unique column names.
             data (dict or None): The dictionary to store the extracted data.
```

### Comparing `ssb_altinn_python-0.4.7/src/altinn/utils.py` & `ssb_altinn_python-0.4.8/src/altinn/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.4.7/PKG-INFO` & `ssb_altinn_python-0.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.4.7
+Version: 0.4.8
 Summary: SSB Altinn Python
 Home-page: https://github.com/statisticsnorway/ssb-altinn-python
 License: MIT
 Author: Vidar Strandseter
 Author-email: vidar.strandseter@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -76,14 +76,32 @@
 
 mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
            'kontAmbulForeDispAnt':'ISEE_VAR2',
            'kontAmbulForeDriftAnt':'ISEE_VAR3',}
 
 isee_transform(file, mapping)
 ```
+
+If you need to flatten more than 'SkjemaData' from the XML, you can make a list of the tags in the XML you need to flatten, and add this list as an argument (tag_list) when running the function isee_transform(file, taglist=taglist). The default value is 'SkjemaData', so if you only need to flatten this, its not needed to pass the argument tag_list.
+
+```python
+from altinn import isee_transform
+
+file = "gs://ssb-prod-dapla-felles-data-delt/altinn3/RA-0595/2023/2/6/810409282_460784f978a2_ebc7af7e-4ebe-4883-b844-66ee6292a93a/form_460784f978a2.xml"
+
+mapping = {'kontAmbulForeDispJaNei':'ISEE_VAR1',
+           'kontAmbulForeDispAnt':'ISEE_VAR2',
+           'kontAmbulForeDriftAnt':'ISEE_VAR3',
+           'kontaktPersonNavn'; 'ISEE_KONTAKTPERSON',}
+
+tags = ['SkjemaData', 'Kontakt']
+
+isee_transform(file, mapping, tag_list=tags)
+```
+
 The function handles flat structures and 'tables' in the XML. If the XML contains repeating values, it puts a suffix containig a number at the end of the FELTNAVN-column. If the XML-contains more complex structures as 'table in table' if will give a warning with a list of which values in FELTNAVN that needs to be further processed before it can be used in ISEE.
 
 The XML needs to contain certain fields in the 'InternInfo'-block, The required filds are:
 - 'enhetsIdent'
 - 'enhetsType'
 - 'delregNr'
```

