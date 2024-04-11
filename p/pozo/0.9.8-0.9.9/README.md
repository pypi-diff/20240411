# Comparing `tmp/pozo-0.9.8.tar.gz` & `tmp/pozo-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pozo-0.9.8.tar", last modified: Sun Feb  4 17:13:00 2024, max compression
+gzip compressed data, was "pozo-0.9.9.tar", last modified: Sat Mar  2 16:07:18 2024, max compression
```

## Comparing `pozo-0.9.8.tar` & `pozo-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-04 17:13:00.366412 pozo-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-04 17:12:48.000000 pozo-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.362412 pozo-0.9.8/pozo/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/pozo/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/renderers/plotly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/renderers/tree_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/pozo/themes/
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/themes/mnemonic_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/themes/theme_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/pozo/units/
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-02-04 17:12:48.000000 pozo-0.9.8/pozo/units/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/pozo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-02-04 17:13:00.000000 pozo-0.9.8/pozo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-04 17:13:00.000000 pozo-0.9.8/pozo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 17:13:00.000000 pozo-0.9.8/pozo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-04 17:13:00.000000 pozo-0.9.8/pozo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-04 17:13:00.000000 pozo-0.9.8/pozo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-04 17:12:48.000000 pozo-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 17:13:00.366412 pozo-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 17:13:00.366412 pozo-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-04 17:12:48.000000 pozo-0.9.8/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-02-04 17:12:48.000000 pozo-0.9.8/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-04 17:12:48.000000 pozo-0.9.8/tests/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-02-04 17:12:48.000000 pozo-0.9.8/tests/test_tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-02 16:07:18.161471 pozo-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-02 16:07:09.000000 pozo-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.157471 pozo-0.9.9/pozo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/pozo/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/renderers/plotly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/renderers/tree_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/pozo/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/themes/mnemonic_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/themes/theme_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/pozo/units/
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-03-02 16:07:09.000000 pozo-0.9.9/pozo/units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/pozo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-02 16:07:18.000000 pozo-0.9.9/pozo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-02 16:07:18.000000 pozo-0.9.9/pozo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 16:07:18.000000 pozo-0.9.9/pozo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-02 16:07:18.000000 pozo-0.9.9/pozo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-02 16:07:18.000000 pozo-0.9.9/pozo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-02 16:07:09.000000 pozo-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 16:07:18.161471 pozo-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 16:07:18.161471 pozo-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-03-02 16:07:09.000000 pozo-0.9.9/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-02 16:07:09.000000 pozo-0.9.9/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-02 16:07:09.000000 pozo-0.9.9/tests/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-02 16:07:09.000000 pozo-0.9.9/tests/test_tracks.py
```

### Comparing `pozo-0.9.8/PKG-INFO` & `pozo-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pozo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Help visualizing well log data - Herramienta para visualizar registros de pozos
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ood>=1.0.6
 Requires-Dist: plotly>=5.18.0
 Requires-Dist: colour>=0.1.5
 Requires-Dist: pint>=0.23
```

### Comparing `pozo-0.9.8/README.md` & `pozo-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/__init__.py` & `pozo-0.9.9/pozo/__init__.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/axes.py` & `pozo-0.9.9/pozo/axes.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/data.py` & `pozo-0.9.9/pozo/data.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/graphs.py` & `pozo-0.9.9/pozo/graphs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import warnings
-
+import numpy as np
 import pozo
 import pozo.units as pzu
 import pozo.renderers as pzr
 import pozo.themes as pzt
 import ood
 import ood.exceptions as ooderr
 
 LAS_TYPE = "<class 'lasio.las.LASFile'>" # TODO this isn't going to work reliably
+WELLY_WELL_TYPE = "<class 'welly.well.Well'>"
+WELLY_PROJECT_TYPE = "<class 'welly.project.Project'>"
 
 class Graph(ood.Observer, pzt.Themeable):
     _type="graph"
     _child_type="track"
 
     def __init__(self, *args, **kwargs):
         self._render = {}
@@ -67,66 +69,126 @@
     def get_render_settings(self):
         return self._render
 
     def process_data(self, *args, **kwargs): # Add ways to add data
         for i, ar in enumerate(args):
             if str(type(ar)) == LAS_TYPE:
                 self.add_las_object(ar, **kwargs)
+            elif str(type(ar)) == WELLY_PROJECT_TYPE:
+                if len(ar.get_wells()) != 1:
+                    raise ValueError(f"If you use welly, you must supply a well (or a project that has exactly one well). This project has {len(ar.get_wells())} wells.")
+                else:
+                    self.add_welly_object(ar[0], **kwargs)
+            elif str(type(ar)) == WELLY_WELL_TYPE:
+                self.add_welly_object(ar, **kwargs)
             elif isinstance(ar, (pozo.Data, pozo.Axis, pozo.Track)):
                 self.add_tracks(ar)
             else:
-                warnings.warn("Unknown argument type passed: argument {i}, {type(ar)}. Ignored")
+                warnings.warn(f"Unknown argument type passed: argument {i}, {type(ar)}. Ignored")
 
     def add_las_object(self, ar, **kwargs):
         include = kwargs.get('include', [])
         exclude = kwargs.get('exclude', [])
         yaxis = kwargs.get('yaxis', None)
         yaxis_name = kwargs.get('yaxis_name',"DEPTH")
         yaxis_unit = None
         if yaxis is not None: # this is a manually added y axis, don't parse it with LAS
-            yaxis_name = None
+            if yaxis_name is None and hasattr(yaxis, "mnemonic"): yaxis_name = yaxis.mnemonic
             if hasattr(yaxis, "unit"):
                 yaxis_unit = yaxis.unit
             else:
-                warnings.warn("Not sure what yaxis units are.") # TODO
+                warnings.warn("Not sure what yaxis units are.")
+            if hasattr(yaxis, "data"):
+                yaxis = yaxis.data
             if len(yaxis) != len(ar.index):
                 raise ValueError(f"Length of supplied yaxis ({len(yaxis)}) does not match length of LAS File index ({len(ar.index)})")
         elif yaxis_name in ar.curves.keys():
             yaxis = ar.curves[yaxis_name].data
             yaxis_unit = pzu.parse_unit_from_curve(ar.curves[yaxis_name])
         else:
             warnings.warn("No yaxis specified and 'DEPTH' not found: using index. Set explicitly with yaxis= OR yaxis_name=. Not sure what y-axis units are.")
-            yaxis = ar.index
-            yaxis_name = None
+            yaxis = ar.depth_m
+            yaxis_unit = pzu.registry.parse_units("meter")
 
 
         for curve in ar.curves:
-            if yaxis_name is not None and curve.mnemonic == yaxis_name:
-                continue
+            if yaxis_name is not None and curve.mnemonic == yaxis_name: continue
 
             mnemonic = pozo.deLASio(curve.mnemonic)
             if include and len(include) != 0 and curve.mnemonic not in include:
                 continue
             elif exclude and len(exclude) != 0 and curve.mnemonic in exclude:
                 continue
-
+            unit = None
             if curve.unit is None:
                 warnings.warn(f"No units found for mnemonic {mnemonic}") # TODO Handle percentages/lookup mnemonics
-            unit = pzu.parse_unit_from_curve(curve)
+            else: unit = pzu.parse_unit_from_curve(curve)
 
             if ooderr.NameConflictException(level=self._name_conflict) is None:
                 name = mnemonic
             else:
                 name = curve.mnemonic
 
             data = pozo.Data(curve.data, depth=yaxis, mnemonic=mnemonic, name=name, unit=unit, depth_unit=yaxis_unit)
             self.add_tracks(data)
         if include and len(include) != 0:
             self.reorder_all_tracks(include)
 
+    def add_welly_object(self, ar, **kwargs):
+        include = kwargs.get('include', [])
+        exclude = kwargs.get('exclude', [])
+        yaxis = kwargs.get('yaxis', None)
+        yaxis_name = kwargs.get('yaxis_name',"DEPTH")
+        yaxis_unit = kwargs.get('yaxis_unit', None)
+
+        if yaxis is not None:
+            if yaxis_name and hasattr(yaxis, "mnemonic"): yaxis_name = yaxis.mnemonic
+            if hasattr(yaxis, "units"):
+                yaxis_unit = pzu.registry.parse_unit_from_context(pozo.deLASio(yaxis.mnemonic), yaxis.units, yaxis.values)
+            else:
+                warnings.warn("Not sure what yaxis units are.") # TODO
+            if hasattr(yaxis, "values"): yaxis = yaxis.values
+        elif yaxis_name in ar.data.keys():
+            yaxis = ar.data[yaxis_name]
+            yaxis_unit = pzu.registry.parse_unit_from_context(pozo.deLASio(yaxis.mnemonic), yaxis.units, yaxis.values)
+        else:
+            raise ValueError("No yaxis specified and 'DEPTH' not found. Set explicitly with yaxis= OR yaxis_name=.")
+        for curve in ar.data.values():
+            if yaxis_name is not None and curve.mnemonic == yaxis_name: continue
+
+            mnemonic = pozo.deLASio(curve.mnemonic)
+            if include and len(include) != 0 and curve.mnemonic not in include:
+                continue
+            elif exclude and len(exclude) != 0 and curve.mnemonic in exclude:
+                continue
+
+            unit = None
+            if curve.units is None:
+                warnings.warn(f"No units found for mnemonic {mnemonic}")
+            else: unit = pzu.registry.parse_unit_from_context(mnemonic, curve.units, curve.values) # TODO is curve correct?
+
+            if ooderr.NameConflictException(level=self._name_conflict) is None:
+                name = mnemonic
+            else:
+                name = curve.mnemonic
+            depth = None
+            depth_unit = None
+            if yaxis is not None:
+                depth = yaxis
+                depth_unit = yaxis_unit
+            else:
+                depth = curve.index
+                depth_unit = pzu.parse_unit_from_context(pozo.deLASio(curve.index_name), curve.index_name, curve.index)
+
+            data = pozo.Data(curve.values, depth=depth, mnemonic=mnemonic, name=name, unit=unit, depth_unit=depth_unit)
+            self.add_tracks(data)
+        if include and len(include) != 0:
+            self.reorder_all_tracks(include)
+
+
     def _check_types(self, *tracks):
         accepted_types = (pozo.Axis, pozo.Data, pozo.Track)
         raw_return = []
         for track in tracks:
             if isinstance(track, (list)):
                 raw_return.extend(self._check_types(*tracks))
             elif not isinstance(track, accepted_types):
```

### Comparing `pozo-0.9.8/pozo/renderers/plotly.py` & `pozo-0.9.9/pozo/renderers/plotly.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/renderers/tree_table.py` & `pozo-0.9.9/pozo/renderers/tree_table.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/themes/__init__.py` & `pozo-0.9.9/pozo/themes/__init__.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/themes/mnemonic_tables.py` & `pozo-0.9.9/pozo/themes/mnemonic_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,12 +52,12 @@
     },
     "RHOB" : {
         "color" : "red",
         "range": [1.95, 2.95],
         "range_unit": "gram/centimeter**3",
     },
     "DT" : {
-        "color" : "black",
+        "color" : "red",
         "range": [30, 200],
         "range_unit": "microsecond/foot",
     },
 }
```

### Comparing `pozo-0.9.8/pozo/themes/theme_tools.py` & `pozo-0.9.9/pozo/themes/theme_tools.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/tracks.py` & `pozo-0.9.9/pozo/tracks.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pozo/units/__init__.py` & `pozo-0.9.9/pozo/units/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -44,41 +44,45 @@
 # TODO: Beginning of a database, has to go online
 # mnemonics, synonyms (resolve- matching in theme,
 # matching in recipe, matching for unit determination)
 # relationships between mnemonics? tolerances? tools?
 # annotating reg files w/ corrections that the file doesn't support
 # versioning, searching
 # also want it to point to posts
+import re
+desc_wo_num = re.compile(r'^(?:\s*\d+\s+)?(.*)$')
 
 def check_las(las, registry=registry):
     def n0(s): # If None, convert to ""
         return "" if s is None else str(s)
     d = chr(0X1e) # delimiter
     result = [f"mnemonic{d}las unit{d}pozo mapping{d}confidence{d}parsed{d}description"]
     for curve in las.curves:
         resolved = None
         pozo_match = None
         confidence = None
         try:
-            resolved = registry.resolve_las_unit(curve)
+            resolved = registry.resolve_las_unit(curve.mnemonic, curve.unit, curve.data)
             if resolved is not None:
                 pozo_match = resolved.unit
                 confidence = resolved.confidence
-            parsed = registry.parse_unit_from_curve(curve)
+            parsed = registry.parse_unit_from_context(curve.mnemonic, curve.unit, curve.data)
         except (pint.UndefinedUnitError, MissingRangeError) as e:
             confidence = " - " + str(e) + " - NONE"
+        find_desc = desc_wo_num.findall(curve.descr)
+        desc = find_desc[0] if len(find_desc) > 0 else curve.descr
         result.append(d.join([n0(x) for x in [pozo.deLASio(curve.mnemonic),
                                              curve.unit,
                                              pozo_match,
                                              confidence,
                                              parsed,
-                                             curve.descr]
+                                             desc]
                               ]))
     try:
         display(HTML(pd.read_csv(StringIO("\n".join(result)), delimiter=d, na_filter=False).to_html()))
     except Exception as e:
         display(str(e))
         display(HTML("<br>".join(result)))
 
 # Just a shorcut to make the API nice
 def parse_unit_from_curve(curve, registry=registry):
-    return registry.parse_unit_from_curve(curve)
+    return registry.parse_unit_from_context(curve.mnemonic, curve.unit, curve.data)
```

### Comparing `pozo-0.9.8/pozo/units/units.py` & `pozo-0.9.9/pozo/units/units.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,36 +46,36 @@
             if not isinstance(ra, LasMapEntry):
                 raise TypeError("Improperly formated map for LasMap, should be type LasMapEntry")
             self.parse_units(ra.unit) # Can't check in LasMapEntry because don't have registry
         if mnemonic not in self._mnemonic_units:
             self._mnemonic_units[mnemonic] = {}
         self._mnemonic_units[mnemonic][unit] = ranges
 
-    def resolve_las_unit(self, curve):
-        mnemonic = pozo.deLASio(curve.mnemonic)
-        unit = curve.unit
-        max_val = np.nanmax(curve.data)
-        min_val = np.nanmin(curve.data)
+    def resolve_las_unit(self, mnemonic, unit, data):
+        mnemonic = pozo.deLASio(mnemonic)
+        unit = unit
+        max_val = np.nanmax(data)
+        min_val = np.nanmin(data)
         if mnemonic in self._mnemonic_units and unit in self._mnemonic_units[mnemonic]:
             ranges = self._mnemonic_units[mnemonic][unit]
             for ra in ranges:
                 if ra.check(min_val, max_val):
                     return ra
             raise MissingRangeError(f"{unit} for {mnemonic} found but not in range: {ranges}.")
         return None
 
-    def parse_unit_from_curve(self, curve): # this just gives you a result
+    def parse_unit_from_context(self, mnemonic, unit, data): # this just gives you a result
         resolved = None
         try:
-            resolved = self.resolve_las_unit(curve)
+            resolved = self.resolve_las_unit(mnemonic, unit, data)
         except MissingRangeError as e:
             warnings.warn(str(e))
         if resolved is not None:
             return self.parse_units(resolved.unit)
         else:
             try:
-                if not curve.unit or curve.unit == "": raise pint.UndefinedUnitError("Empty unit not allowed- please map it")
-                return self.parse_units(curve.unit)
+                if not unit or unit == "": raise pint.UndefinedUnitError("Empty unit not allowed- please map it")
+                return self.parse_units(unit)
             except pint.UndefinedUnitError as e:
-                raise pint.UndefinedUnitError(f"{curve.unit} for {pozo.deLASio(curve.mnemonic)} not found. {str(e)}")
+                raise pint.UndefinedUnitError(f"{unit} for {pozo.deLASio(mnemonic)} not found. {str(e)}")
 
 # we now don't get confidence from string
```

### Comparing `pozo-0.9.8/pozo.egg-info/PKG-INFO` & `pozo-0.9.9/pozo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pozo
-Version: 0.9.8
+Version: 0.9.9
 Summary: Help visualizing well log data - Herramienta para visualizar registros de pozos
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: ood>=1.0.6
 Requires-Dist: plotly>=5.18.0
 Requires-Dist: colour>=0.1.5
 Requires-Dist: pint>=0.23
```

### Comparing `pozo-0.9.8/pozo.egg-info/SOURCES.txt` & `pozo-0.9.9/pozo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/pyproject.toml` & `pozo-0.9.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 find = {namespaces = false}
 
 [project]
 name = "pozo"
 description = "Help visualizing well log data - Herramienta para visualizar registros de pozos"
 readme = "README.md"
 requires-python = ">=3.9"
-version = "0.9.8"
+version = "0.9.9"
 dependencies = [
  "ood >=1.0.6",
  "plotly >=5.18.0",
  "colour >= 0.1.5",
  "pint >= 0.23",
  "pandas >= 2.0.0",
  "numpy >= 1.26.0",
```

### Comparing `pozo-0.9.8/tests/test_axes.py` & `pozo-0.9.9/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/tests/test_data.py` & `pozo-0.9.9/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pozo-0.9.8/tests/test_tracks.py` & `pozo-0.9.9/tests/test_tracks.py`

 * *Files identical despite different names*

