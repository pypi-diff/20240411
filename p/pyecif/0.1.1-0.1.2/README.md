# Comparing `tmp/pyecif-0.1.1-py3-none-any.whl.zip` & `tmp/pyecif-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7636 bytes, number of entries: 9
--rw-r--r--  2.0 unx     5648 b- defN 24-Apr-10 03:21 pyecif/ECIFPandasTools.py
+Zip file size: 7779 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     7010 b- defN 24-Apr-11 06:02 pyecif/ECIFPandasTools.py
 -rw-r--r--  2.0 unx       59 b- defN 24-Apr-09 08:05 pyecif/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 08:23 tests/__init__.py
 -rw-r--r--  2.0 unx     3522 b- defN 24-Apr-09 08:05 tests/test_ECIFPandasTools.py
--rw-r--r--  2.0 unx     1067 b- defN 24-Apr-10 03:41 pyecif-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4995 b- defN 24-Apr-10 03:41 pyecif-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-10 03:41 pyecif-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-10 03:41 pyecif-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      693 b- defN 24-Apr-10 03:41 pyecif-0.1.1.dist-info/RECORD
-9 files, 16089 bytes uncompressed, 6444 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     1067 b- defN 24-Apr-11 06:02 pyecif-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5126 b- defN 24-Apr-11 06:02 pyecif-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 06:02 pyecif-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-11 06:02 pyecif-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      693 b- defN 24-Apr-11 06:02 pyecif-0.1.2.dist-info/RECORD
+9 files, 17582 bytes uncompressed, 6587 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_ECIFPandasTools.py
 Comment: 
 
-Filename: pyecif-0.1.1.dist-info/LICENSE
+Filename: pyecif-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyecif-0.1.1.dist-info/METADATA
+Filename: pyecif-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: pyecif-0.1.1.dist-info/WHEEL
+Filename: pyecif-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyecif-0.1.1.dist-info/top_level.txt
+Filename: pyecif-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyecif-0.1.1.dist-info/RECORD
+Filename: pyecif-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyecif/ECIFPandasTools.py

```diff
@@ -1,27 +1,38 @@
 import os
 import re
 
 import numpy as np
 import pandas as pd
 from pymatgen.core.structure import Structure
 from pymatgen.io.cif import CifParser, CifWriter
+from multiprocessing import Pool
+import gemmi
+from tqdm import tqdm
 
 
 def WriteEcif(df, out, idName='ID', cifColName='CIF', properties=None):
     """
     Write a pandas dataframe to an ECIF file
     """
-
+    
     if cifColName not in df.columns:
         raise ValueError("No column named %s in dataframe" % cifColName)
     
+    cifblock = CifBlock()
+
     for cif in df[cifColName]:
-        if not isinstance(cif, Structure):
-            raise ValueError("Column %s is not a list of pymatgen Structures" % cifColName)
+        if isinstance(cif, gemmi.SmallStructure):
+            processStructure = cifblock.SetCifFromGemmicif
+            break
+        elif isinstance(cif, Structure):
+            processStructure = cifblock.SetCifFromPymatgen
+            break
+        else:
+            raise ValueError("CIF column must contain either pymatgen or gemmi structures")
     
     if properties is None:
         properties = []
     else:
         properties = list(properties)
 
     if cifColName in properties:
@@ -31,23 +42,23 @@
 
     if os.path.exists(out):
         print("Warning: %s already exists. Overwriting." % out)
     
     with open(out, 'w') as file:
 
         for num, row in enumerate(df.iterrows()):
-            cifblock = CifBlock()
+            
             if idName is not None:
                 if idName == 'ID':
                     cifblock.SetProp('_Name', str(row[0]))
                 else:
                     cifblock.SetProp('_Name', str(row[1][idName]))
 
             structure = row[1][cifColName]
-            cifblock.AddCifFromPymatgen(structure)
+            processStructure(structure)
 
             for prop in properties:
                 cell_value = row[1][prop]
                 # Make sure float does not get formatted in E notation
                 if np.issubdtype(type(cell_value), np.floating):
                     s = '{:f}'.format(cell_value).rstrip("0")  # "f" will show 7.0 as 7.00000
                     if s[-1] == ".":
@@ -56,122 +67,148 @@
                 else:
                     cifblock.SetProp(prop, str(cell_value))
 
             cif_block = cifblock.GetBlock(cifColName)
             num_cif_block = re.sub(r'(<.*?>)(.*?)(?=\s|$)', fr'\1 ({num})', cif_block)
             file.write(num_cif_block)
             file.write('\n\n$$$$\n\n')
-        
-
 
-def LoadEcif(ecif_file, idName='ID', cifColName='CIF'):
+def LoadEcif(ecif_file, idName='ID', cifColName='CIF', type='gemmi'):
     """
     Load ECIF file into a pandas dataframe
     """
         
     with open(ecif_file, 'r') as file:
         lines = file.readlines()
     
     df = pd.DataFrame()
     block = []
+    rows = []
+    cifblocks = []
     for line in lines:
-        if line.strip() == '$$$$':
-            cifblock = CifBlock()
-            cifblock.AddBlock('\n'.join(block), cifColName=cifColName)
+        if line.strip() == '$$$$':   
+            cifblock = CifBlock()   
+            cifblock.SetBlock('\n'.join(block), cifColName=cifColName)
             block = []
-            row = _CifBlockToRow(cifblock, cifColName)
-            df = df._append(row, ignore_index=True)
-
+            cifblocks.append(cifblock)
+            row = _CifBlockToRow(cifblock, cifColName, type=type)
+            rows.append(row)
         else:
             block.append(line)
+
+    df = pd.DataFrame(rows)
+
     if idName in df.columns:
         df.set_index(idName, inplace=True)
 
     for col in df.columns:
         if col != cifColName:
             df[col] = pd.to_numeric(df[col], errors='ignore')
 
     return df
 
-def _CifBlockToRow(cifblock, cifColName):
+def _CifBlockToRow(cifblock, cifColName, type='gemmi'):
     row = {}
     for key, value in cifblock._props.items():
         row[key] = value
-    row[cifColName] = cifblock.GetPymatgenStructure()
+    if type == 'gemmi':
+        row[cifColName] = cifblock.GetGemmicif()
+    elif type == 'pymatgen':
+        row[cifColName] = cifblock.GetPymatgenStructure()
     return row
 
 class CifBlock:
     def __init__(self):
         self._props = {}
         self._cif = []
+        self.pattern = re.compile(r'<(.*?)>\s\(\d+\)\n(.*?)(?=<|$)', re.DOTALL)
     
     def SetProp(self, key, value):
         self._props[key] = value
     
     def GetProp(self, key):
         return self._props[key]
     
-    def AddCifLine(self, line):
-        self._cif.append(line)
-    
-    def AddCifFromPymatgen(self, structure):
-        cif_writer = CifWriter(structure)
-        cif_string = cif_writer.__str__()
-        cif_string = cif_string.split('\n')
-        for line in cif_string:
-            self._cif.append(line)   
+    def SetCifFromString(self, string):
+        self._cif = string.split('\n')
 
     def GetCif(self):
         return self._cif
-    
+
+    def SetBlock(self, block, cifColName='CIF'):
+        
+        matches = self.pattern.findall(block)
+
+        block_dict = {key: value.strip() for key, value in matches}
+
+        self._cif = block_dict[cifColName].split('\n')
+        for key, value in block_dict.items():
+            if key != cifColName:
+                self._props[key] = value
+
     def GetBlock(self, cifColName='CIF'):
         block = []
         block.append('<ID>\n%s\n' % self._props['_Name'])
         block.append(f'<{cifColName}>')
         for line in self._cif:
             block.append(line)
         for key, value in self._props.items():
             if key != '_Name':
                 block.append('<%s>\n%s' % (key, value))
         block_str = '\n'.join(block)
         return block_str
-    
+
+    def SetCifFromPymatgen(self, structure):
+        cif_writer = CifWriter(structure)
+        cif_string = cif_writer.__str__()
+        cif_string = cif_string.split('\n')
+        self._cif = []
+        for line in cif_string:
+            self._cif.append(line)   
+
+    def SetCifFromGemmicif(self, structure):
+        cif_string = structure.make_cif_block().as_string()
+        cif_string = cif_string.split('\n')
+        self._cif = []
+        for line in cif_string:
+            self._cif.append(line)
+
     def GetPymatgenStructure(self):
         cif_str = '\n'.join(self._cif)
         cif_parser = CifParser.from_str(cif_str)
         return cif_parser.get_structures(on_error='ignore')[0]
-
-    def AddBlock(self, block, cifColName='CIF'):
-        pattern = re.compile(r'<(.*?)>\s\(\d+\)\n(.*?)(?=<|$)', re.DOTALL)
-        matches = pattern.findall(block)
-
-        # 创建一个字典来存储key-value对
-        block_dict = {key: value.strip() for key, value in matches}
-
-        self._cif = block_dict[cifColName].split('\n')
-        for key, value in block_dict.items():
-            if key != cifColName:
-                self._props[key] = value
+    
+    def GetGemmicif(self):
+        cif_str = '\n'.join(self._cif)
+        cif_parser = gemmi.cif.read_string(cif_str)
+        return gemmi.make_small_structure_from_block(cif_parser.sole_block())
 
     def WriteCif(self, filename):
         with open(filename, 'w') as f:
             for key, value in self._props.items():
                 f.write('_%s\n%s\n' % (key, value))
             f.write('\n')
             for line in self._cif:
                 f.write(line + '\n')
 
 if __name__ == '__main__':
     #df = LoadEcif('example/mb-jdft2d.ecif')
     #WriteEcif(df, 'output.ecif', properties=df.columns)
-    from pymatgen.core import Lattice
-    df = pd.DataFrame({
-        'ID': ['test1', 'test2'],
-        'CIF': [Structure(Lattice.cubic(4.225), ["Na"], [[0, 0, 0]]),
-                Structure(Lattice.cubic(3.61), ["Cu", "Cu", "Cu", "Cu"], [[0, 0, 0], [0.5, 0.5, 0], [0.5, 0, 0.5], [0, 0.5, 0.5]])
-                ],
-        'prop1': [1, 2],
-        'prop2': [3, 4]
-    })
-
-    WriteEcif(df, 'test.ecif', properties=['prop1', 'prop2'])
-    df = LoadEcif('test.ecif')
+    #from pymatgen.core import Lattice
+    #df = pd.DataFrame({
+    #    'ID': ['test1', 'test2'],
+    #    'CIF': [Structure(Lattice.cubic(4.225), ["Na"], [[0, 0, 0]]),
+    #            Structure(Lattice.cubic(3.61), ["Cu", "Cu", "Cu", "Cu"], [[0, 0, 0], [0.5, 0.5, 0], [0.5, 0, 0.5], [0, 0.5, #0.5]])
+    #            ],
+    #    'prop1': [1, 2],
+    #    'prop2': [3, 4]
+    #})
+    #WriteEcif(df, 'test.ecif', properties=['prop1', 'prop2'])
+    #df = LoadEcif('test.ecif')
+    #WriteEcif(df, 'test2.ecif', properties=df.columns)
+
+    #import cProfile
+    #cProfile.run('df = LoadEcif("matbench/matbench_jdft2d/test_fold_0.ecif", cifColName="structure")')
+    #df = LoadEcif("matbench/matbench_mp_e_form/train_fold_0.ecif", cifColName="structure", type='gemmi')
+    df = LoadEcif("matbench/matbench_jdft2d/train_fold_0.ecif", cifColName="structure", type='gemmi')
+    print(df)
+    #df
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `pyecif-0.1.1.dist-info/LICENSE` & `pyecif-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyecif-0.1.1.dist-info/METADATA` & `pyecif-0.1.2.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecif
-Version: 0.1.1
+Version: 0.1.2
 Summary: ECIF file format tools for Python.
 Home-page: https://github.com/emotionor/ecif
 Author: Cui Yaning
 Author-email: emotionor@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -61,28 +61,36 @@
 
 Note that both of these functions accept some optional parameters for specifying the names of certain columns in the dataframe, as well as additional properties to be included in the ECIF file.
 
 Below is a snapshot of our data frame (`df`). It contains the fields ID, exfoliation energy (exfoliation_en) and crystal structure (CIF).
 
 | ID | exfoliation_en | CIF |
 | --- | --- | --- |
-| mb-jdft2d-001 | 63.593833 | [[1.49323138 3.32688405 7.26257785] Hf, [3.326... |
-| mb-jdft2d-002 | 134.86375 | [[1.85068084 4.37698238 6.93015769] As, [-1.63... |
-| mb-jdft2d-003 | 43.114667 | [[-1.23770919e-16  2.02133251e+00  1.19727954e... |
-| mb-jdft2d-004 | 240.715488 | [[2.39882726 2.39882726 2.53701553] In, [0.054... |
-| mb-jdft2d-005 | 67.442833 | [[ -1.50082215  -0.86650009 -19.85028757] Nb, ... |
+| mb-jdft2d-001 | 63.593833 |  <gemmi.SmallStructure: SrSbSe2F> |
+| mb-jdft2d-002 | 134.86375 |       <gemmi.SmallStructure: AgI> |
+| mb-jdft2d-003 | 43.114667 | <gemmi.SmallStructure: Mg(ReO4)2> |
+| mb-jdft2d-004 | 240.715488 |     <gemmi.SmallStructure: Si3H> |
+| mb-jdft2d-005 | 67.442833 |      <gemmi.SmallStructure: CoO2> |
 | ... | ... | ... |
-| mb-jdft2d-632 | 26.426545 | [[ -2.38592122   1.37751225 -13.178104  ] Co, ... |
-| mb-jdft2d-633 | 43.574286 | [[1.92920996 1.92920997 4.57868062] Ca, [1.929... |
-| mb-jdft2d-634 | 88.808659 | [[4.53578337 0.         3.14900225] Pd, [ 9.07... |
-| mb-jdft2d-635 | 132.26525 | [[4.41728901 2.2026463  1.81895292] Hg, [6.631... |
-| mb-jdft2d-636 | 63.564333 | [[ 0.70613488 -1.21109143  1.03195663] Co, [ 2... |
+| mb-jdft2d-632 | 26.426545 |    <gemmi.SmallStructure: HgBr2 |
+| mb-jdft2d-633 | 43.574286 |    <gemmi.SmallStructure: FeCl3 |
+| mb-jdft2d-634 | 88.808659 |    <gemmi.SmallStructure: HoBrO |
+| mb-jdft2d-635 | 132.26525 |    <gemmi.SmallStructure: GaHO2 |
+| mb-jdft2d-636 | 63.564333 |  <gemmi.SmallStructure: TaCoTe2 |
 
 
-To better understand the contents of the CIF field, we can look at the details of `df['CIF'][0]`. This is an example describing the position of the elements Hf, Si and Te in the crystal structure, which is the `pymatgen.core.Structure` class:
+The default is to use `gimmi` to load the data, one can also choose `pymatgen` to load the data.
+
+```python
+from pyecif import LoadEcif
+
+df = LoadEcif('output.ecif', cifColName='CIF', type='pymatgen')
+```
+
+To better understand the contents of the CIF field, the details of `df['CIF'][0]` is as below with `pymatgen`. This is an example describing the position of the elements Hf, Si and Te in the crystal structure, which is the `pymatgen.core.Structure` class:
 
 ```python
 Structure Summary
 Lattice
     abc : 3.66730534 3.66730534 27.311209
  angles : 90.0 90.0 90.0
  volume : 367.31195815130786
@@ -98,7 +106,10 @@
 PeriodicSite: Te5 (Te) (1.493, 3.327, 1.652) [0.4072, 0.9072, 0.06049]
 ```
 
 # Matbench
 
 Matbench is a benchmark dataset for materials science. You can easily obtain the ECIF format of the Matbench dataset using the example script `scripts/get_matbench_jdft2d.py`.
 
+# Time cost
+Total time: 27.1109 s for 106201 structure (matbench_mp_e_form:train)
+
```

## Comparing `pyecif-0.1.1.dist-info/RECORD` & `pyecif-0.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyecif/ECIFPandasTools.py,sha256=AlEi25g_xiyT3jWK6-85Egj_M89Yq4YK1054yyuKYw0,5648
+pyecif/ECIFPandasTools.py,sha256=RBCqV2NJgSOedhKpROLhJUYWqBV49sBSkTCXZzB_ke0,7010
 pyecif/__init__.py,sha256=jL-BaYNsrAJhOiCzGaYRrPHVcNHfQbI-YRXC3IWNThQ,59
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_ECIFPandasTools.py,sha256=Jgp35kiH4k-ZKWLHWrhzNgmVRs7pTerMUy8ixRR7xSg,3522
-pyecif-0.1.1.dist-info/LICENSE,sha256=YERY5Sni2zmI2BXmMscBH4tbImOr8a-cazWbo0Vqn6E,1067
-pyecif-0.1.1.dist-info/METADATA,sha256=pdfczfVEHzyeg2T7QkM9NKIgi1x9DESMlWXS4KqTFG4,4995
-pyecif-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyecif-0.1.1.dist-info/top_level.txt,sha256=QjrGpiTVAxnKH-qt9S2Em5DcuXxDBa3gwau0JQRO2rY,13
-pyecif-0.1.1.dist-info/RECORD,,
+pyecif-0.1.2.dist-info/LICENSE,sha256=YERY5Sni2zmI2BXmMscBH4tbImOr8a-cazWbo0Vqn6E,1067
+pyecif-0.1.2.dist-info/METADATA,sha256=GbhizumD7817R2tTayaGN2mUVraWj9ROqbrrALnkOJA,5126
+pyecif-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyecif-0.1.2.dist-info/top_level.txt,sha256=QjrGpiTVAxnKH-qt9S2Em5DcuXxDBa3gwau0JQRO2rY,13
+pyecif-0.1.2.dist-info/RECORD,,
```

