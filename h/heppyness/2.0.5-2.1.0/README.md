# Comparing `tmp/heppyness-2.0.5.tar.gz` & `tmp/heppyness-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heppyness-2.0.5.tar", last modified: Tue Sep  5 14:08:04 2023, max compression
+gzip compressed data, was "heppyness-2.1.0.tar", last modified: Thu Apr 11 09:23:13 2024, max compression
```

## Comparing `heppyness-2.0.5.tar` & `heppyness-2.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-09-05 14:08:04.603774 heppyness-2.0.5/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1071 2022-03-22 10:30:20.000000 heppyness-2.0.5/LICENSE
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1587 2023-09-05 14:08:04.603600 heppyness-2.0.5/PKG-INFO
--rw-r--r--   0 stefanrichter   (501) staff       (20)      933 2023-09-05 14:05:48.000000 heppyness-2.0.5/README.md
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-09-05 14:08:04.601173 heppyness-2.0.5/heppy/
--rw-r--r--   0 stefanrichter   (501) staff       (20)      321 2023-02-24 11:27:11.000000 heppyness-2.0.5/heppy/__init__.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    14124 2022-03-22 10:30:20.000000 heppyness-2.0.5/heppy/heatmap.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    70541 2023-09-05 13:41:51.000000 heppyness-2.0.5/heppy/histogram.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2832 2023-02-20 18:47:17.000000 heppyness-2.0.5/heppy/panel.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    17681 2023-08-29 08:11:40.000000 heppyness-2.0.5/heppy/plot.py
--rwxr-xr-x   0 stefanrichter   (501) staff       (20)     2761 2023-04-17 19:41:29.000000 heppyness-2.0.5/heppy/readroot.py
--rwxr-xr-x   0 stefanrichter   (501) staff       (20)    13157 2023-04-17 19:28:50.000000 heppyness-2.0.5/heppy/readroot_legacy.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2184 2023-02-24 20:20:26.000000 heppyness-2.0.5/heppy/readtrex.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2081 2022-04-21 09:18:03.000000 heppyness-2.0.5/heppy/readyoda.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1478 2022-03-22 10:30:20.000000 heppyness-2.0.5/heppy/scanroot.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    26748 2023-02-24 20:07:11.000000 heppyness-2.0.5/heppy/uncertainty.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     5810 2022-03-22 10:30:20.000000 heppyness-2.0.5/heppy/value.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     6170 2022-03-22 10:30:20.000000 heppyness-2.0.5/heppy/yodarun.py
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-09-05 14:08:04.602090 heppyness-2.0.5/heppyness.egg-info/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1587 2023-09-05 14:08:04.000000 heppyness-2.0.5/heppyness.egg-info/PKG-INFO
--rw-r--r--   0 stefanrichter   (501) staff       (20)      516 2023-09-05 14:08:04.000000 heppyness-2.0.5/heppyness.egg-info/SOURCES.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)        1 2023-09-05 14:08:04.000000 heppyness-2.0.5/heppyness.egg-info/dependency_links.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)       78 2023-09-05 14:08:04.000000 heppyness-2.0.5/heppyness.egg-info/requires.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)        6 2023-09-05 14:08:04.000000 heppyness-2.0.5/heppyness.egg-info/top_level.txt
--rw-r--r--   0 stefanrichter   (501) staff       (20)       38 2023-09-05 14:08:04.603831 heppyness-2.0.5/setup.cfg
--rw-r--r--   0 stefanrichter   (501) staff       (20)     1091 2023-09-05 14:07:17.000000 heppyness-2.0.5/setup.py
-drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2023-09-05 14:08:04.603228 heppyness-2.0.5/test/
--rw-r--r--   0 stefanrichter   (501) staff       (20)     3030 2022-03-22 10:30:20.000000 heppyness-2.0.5/test/test_heatmap.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    15789 2022-03-22 10:30:20.000000 heppyness-2.0.5/test/test_histogram1d.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)    10062 2022-03-22 10:30:20.000000 heppyness-2.0.5/test/test_histogram2d.py
--rw-r--r--   0 stefanrichter   (501) staff       (20)     2949 2023-04-17 19:48:25.000000 heppyness-2.0.5/test/test_readroot.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2024-04-11 09:23:13.317681 heppyness-2.1.0/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1071 2022-03-22 10:30:20.000000 heppyness-2.1.0/LICENSE
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1785 2024-04-11 09:23:13.317466 heppyness-2.1.0/PKG-INFO
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      933 2023-09-05 14:05:48.000000 heppyness-2.1.0/README.md
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2024-04-11 09:23:13.314713 heppyness-2.1.0/heppy/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      333 2024-04-11 09:18:01.000000 heppyness-2.1.0/heppy/__init__.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    14124 2022-03-22 10:30:20.000000 heppyness-2.1.0/heppy/heatmap.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    69972 2023-12-14 10:23:41.000000 heppyness-2.1.0/heppy/histogram.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2832 2023-02-20 18:47:17.000000 heppyness-2.1.0/heppy/panel.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    17832 2023-12-12 16:56:50.000000 heppyness-2.1.0/heppy/plot.py
+-rwxr-xr-x   0 stefanrichter   (501) staff       (20)     2761 2023-04-17 19:41:29.000000 heppyness-2.1.0/heppy/readroot.py
+-rwxr-xr-x   0 stefanrichter   (501) staff       (20)    13157 2023-04-17 19:28:50.000000 heppyness-2.1.0/heppy/readroot_legacy.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2184 2023-02-24 20:20:26.000000 heppyness-2.1.0/heppy/readtrex.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2081 2022-04-21 09:18:03.000000 heppyness-2.1.0/heppy/readyoda.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1485 2024-04-11 09:17:25.000000 heppyness-2.1.0/heppy/scanroot.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    26748 2023-02-24 20:07:11.000000 heppyness-2.1.0/heppy/uncertainty.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     5810 2022-03-22 10:30:20.000000 heppyness-2.1.0/heppy/value.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1140 2023-10-24 14:51:21.000000 heppyness-2.1.0/heppy/writeroot_helpers.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     6170 2022-03-22 10:30:20.000000 heppyness-2.1.0/heppy/yodarun.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2024-04-11 09:23:13.317225 heppyness-2.1.0/heppyness.egg-info/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1785 2024-04-11 09:23:13.000000 heppyness-2.1.0/heppyness.egg-info/PKG-INFO
+-rw-r--r--   0 stefanrichter   (501) staff       (20)      543 2024-04-11 09:23:13.000000 heppyness-2.1.0/heppyness.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)        1 2024-04-11 09:23:13.000000 heppyness-2.1.0/heppyness.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)       78 2024-04-11 09:23:13.000000 heppyness-2.1.0/heppyness.egg-info/requires.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)        6 2024-04-11 09:23:13.000000 heppyness-2.1.0/heppyness.egg-info/top_level.txt
+-rw-r--r--   0 stefanrichter   (501) staff       (20)       38 2024-04-11 09:23:13.317726 heppyness-2.1.0/setup.cfg
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     1091 2024-04-11 09:19:51.000000 heppyness-2.1.0/setup.py
+drwxr-xr-x   0 stefanrichter   (501) staff       (20)        0 2024-04-11 09:23:13.316735 heppyness-2.1.0/test/
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     3030 2022-03-22 10:30:20.000000 heppyness-2.1.0/test/test_heatmap.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    15789 2022-03-22 10:30:20.000000 heppyness-2.1.0/test/test_histogram1d.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)    10062 2022-03-22 10:30:20.000000 heppyness-2.1.0/test/test_histogram2d.py
+-rw-r--r--   0 stefanrichter   (501) staff       (20)     2949 2023-04-17 19:48:25.000000 heppyness-2.1.0/test/test_readroot.py
```

### Comparing `heppyness-2.0.5/LICENSE` & `heppyness-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/PKG-INFO` & `heppyness-2.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heppyness
-Version: 2.0.5
+Version: 2.1.0
 Home-page: https://gitlab.cern.ch/strichte/heppy
 Author: Stefan Richter
 Author-email: stefan.richter@cern.ch
 Maintainer: Stefan Richter
 Maintainer-email: stefan.richter@cern.ch
 License: HEP license, based on MIT license
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: uproot
+Requires-Dist: uproot-methods
+Requires-Dist: awkward
+Requires-Dist: pandas
+Requires-Dist: pyyaml
+Requires-Dist: sphinx_rtd_theme
 
 # Heppy
 
 Heppy provides pythonic data structures and a few high-level tools for high-energy physics. In particular, it provides very useful histogram classes that neatly integrate systematic variations (which, to my knowledge, no other histogram class that's widely used in HEP does) and support common operations such as addition, division, rebinning, slicing, projecting, integrating. It also provides flexible matplotlib-based plotting.
 
 The documentation can be found [here](https://heppy.readthedocs.io).
```

### Comparing `heppyness-2.0.5/README.md` & `heppyness-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/heatmap.py` & `heppyness-2.1.0/heppy/heatmap.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/histogram.py` & `heppyness-2.1.0/heppy/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,44 +282,49 @@
             return np.nan_to_num((self_signs + other_signs) / (np.abs(self_signs) + np.abs(other_signs)))
 
 
 
     def _modify_areas(self, other, operation, symbol):
         '''
         Backend function that internally implements the mathematical operations between two histograms
-        Alternatively, @other may be a scalar (float or int)
+        Alternatively, @other may be a scalar (float or int) or a numpy array of the same dimension as the histogram areas
 
         NOTE: if @operation is truediv, the bin heights rather than areas are set.
 
         Behaviour for combining UNCORRELATED uncertainties:
 
         '''
-        scalar = False
+        scalar_or_array = False
         if isinstance(other, (int, float)):
-            scalar = True
+            scalar_or_array = True
             other = type(self)(self.binedges, np.zeros_like(self.areas) + other, areas=True, name='{0}'.format(other))
+        elif isinstance(other, np.ndarray):
+            scalar_or_array = True
+            if not other.shape == self.areas.shape:
+                raise ValueError(f'Cannot perform mathematical operation of histogram and numpy array, shapes differ:\n{self.areas.shape}\n{other.shape}')
+            other = type(self)(self.binedges, other, areas=True, name='{0}'.format(other))
         # NB: array_equal also works for a tuple of Numpy arrays, as we have for a 2D histogram!
         if isinstance(self.binedges, np.ndarray):
             if not np.allclose(self.binedges, other.binedges):
-                raise RuntimeError('Cannot perform mathematical operation on histograms, binegdes differ:\n{a}\n{b}'.format(a=self.binedges, b=other.binedges))
+                raise ValueError('Cannot perform mathematical operation on histograms, binegdes differ:\n{a}\n{b}'.format(a=self.binedges, b=other.binedges))
         else:
             if not np.allclose(self.binedges[0], other.binedges[0]) or not np.allclose(self.binedges[1], other.binedges[1]):
-                raise RuntimeError('Cannot perform mathematical operation on histograms, binegdes differ:\n{a}\n{b}'.format(a=self.binedges, b=other.binedges))
+                raise ValueError('Cannot perform mathematical operation on histograms, binegdes differ:\n{a}\n{b}'.format(a=self.binedges, b=other.binedges))
         selfname = '({0})'.format(self.name) if ' ' in self.name else self.name
         othername = '({0})'.format(other.name) if ' ' in other.name else other.name
         resultname = '{0} {1} {2}'.format(selfname, symbol, othername)
         attributes = {**other.attributes, **self.attributes}
         plot_attributes = {**other.plot_attributes, **self.plot_attributes}
         binedges = self.binedges
         with warnings.catch_warnings():
             warnings.simplefilter('ignore', RuntimeWarning) # do not warn about NaNs in the division in the following line
             areas = operation(self.areas, other.areas)
         # Constructing uncorrelated variations of the new histogram
         uncorr_variations = {}
-        if scalar:
+        if scalar_or_array:
             # for name, array in self.uncorr_variations.items():
             #     print(name, array, other.areas, operation(array, other.areas))
             uncorr_variations = {name : operation(array, other.areas) for name, array in self.uncorr_variations.items()}
         elif not operation in [operator.add, operator.sub, operator.truediv]:
             # CAUTION: calculation of uncorrelated uncertainty is not implemented in this case
             pass
         else:
@@ -344,15 +349,15 @@
                         uncorr_variations[name] = areas + shift_directions * np.sqrt((self_shifts / other.areas)**2 + (self.areas * other_shifts / other.areas**2)**2)
                 else:
                     uncorr_variations[name] = areas + shift_directions * np.sqrt((self_shifts**2 + other_shifts**2))
 
 
         # Constructing correlated variations of the new histogram
         corr_variations = {}
-        if scalar:
+        if scalar_or_array:
             corr_variations = {name : operation(array, other.areas) for name, array in self.corr_variations.items()}
         else:
             # TODO: factor this else clause into a separate method!
             all_corr_variations = list(set(list(self.corr_variations.keys()) + list(other.corr_variations.keys())))
             for name in all_corr_variations:
                 try:
                     self_var = self.corr_variations[name]
@@ -372,51 +377,51 @@
         #print('TODO: add support for combining variations in histogram manipulation')
         return type(self)(binedges, areas, name=resultname, areas=True, uncorr_variations=uncorr_variations, corr_variations=corr_variations, attributes=attributes, plot_attributes=plot_attributes)
 
 
 
     def __add__(self, other):
         '''
-        Add another histogram or a scalar to this histogram.
+        Add another histogram or a scalar/numpy array to this histogram.
 
         Returns the result of the addition as a histogram.
 
         Correlated variations are treated as fully correlated among the two histograms if they have the same
         name, otherwise they are treated as uncorrelated. Uncorrelated variations are treated as uncorrelated
         between the two histograms.
         '''
         return self._modify_areas(other, operator.add, '+')
 
     def __sub__(self, other):
         '''
-        Subtract another histogram or a scalar from this histogram.
+        Subtract another histogram or a scalar/numpy array from this histogram.
 
         Returns the result of the subtraction as a histogram.
 
         Correlated variations are treated as fully correlated among the two histograms if they have the same
         name, otherwise they are treated as uncorrelated. Uncorrelated variations are treated as uncorrelated
         between the two histograms.
         '''
         return self._modify_areas(other, operator.sub, '-')
 
     def __mul__(self, other):
         '''
-        Multiply another histogram or a scalar binwise with this histogram.
+        Multiply another histogram or a scalar/numpy array binwise with this histogram.
 
         Returns the result of the binwise multiplication as a histogram.
 
         Correlated variations are treated as fully correlated among the two histograms if they have the same
         name, otherwise they are treated as uncorrelated. Uncorrelated variations are treated as uncorrelated
         between the two histograms.
         '''
         return self._modify_areas(other, operator.mul, '*')
 
     def __truediv__(self, other):
         '''
-        Divide by another histogram or a scalar binwise.
+        Divide by another histogram or a scalar/numpy array binwise.
 
         Returns the result of the binwise division as a histogram.
 
         Correlated variations are treated as fully correlated among the two histograms if they have the same
         name, otherwise they are treated as uncorrelated.
 
         CAUTION: Uncorrelated variations are treated as uncorrelated between the two histograms. If the
@@ -522,19 +527,17 @@
 
         Similar to ``numpy.clip`` (see `here <https://numpy.org/doc/stable/reference/generated/numpy.clip.html>`_).
 
         Both the nominals and all correlated and uncorrelated variations of the histogram are clipped.
         *Note that the net variation of multiple individual variations considered together may still lie
         outside of the clip range!*
 
-        :param minimum: minimum accepted value; areas below this value will be set to the value.
-        If ``None``, no minimum is imposed.
+        :param minimum: minimum accepted value; areas below this value will be set to the value. If ``None``, no minimum is imposed.
         :type minimum: ``float`` or ``None``
-        :param maximum: maximum accepted value; areas above this value will be set to the value.
-        If ``None``, no maximum is imposed.
+        :param maximum: maximum accepted value; areas above this value will be set to the value. If ``None``, no maximum is imposed.
         :type maximum: ``float`` or ``None``
 
         The behaviour is like that of ``numpy.clip``, e.g. with regards to what happens if ``minimum`` is
         greater than ``maximum``.
 
         **"Undocumented" feature:** you can actually pass a Numpy ``array_like`` as ``minimum`` or ``maximum``,
         not just a single ``float``!
@@ -932,31 +935,22 @@
         :type errors: ``np.array`` or ``None``
 
         :returns: dictionary of ROOT histograms (values) mapped by variation
             name (keys)
         :rtype: ``dict`` of ``str`` and ``ROOT.TH1D``
         """
         import ROOT
-        from array import array
-        def array2hist(areas, th1, errors=None):
-            for bin_index in range(self.nbins):
-                th1.SetBinContent(bin_index+1, self.areas[bin_index])
-                if errors is not None:
-                    th1.SetBinError(bin_index+1, errors[bin_index])
-        def to_th1(name, binedges, areas):
-            th1 = ROOT.TH1D(name, name, len(binedges)-1, array('d', [b for b in binedges]))
-            array2hist(areas, th1, errors=errors)
-            return th1
+        from . import writeroot_helpers as wrh
         th1s = {}
         # Add nominal
         key = key_form.format(name=self.name, variation=nominal_label)
-        th1s[key] = to_th1(key, self.binedges, self.areas)
+        th1s[key] = wrh.to_th1(key, self.binedges, self.areas, self.nbins)
         for variation, areas in {**self.uncorr_variations, **self.corr_variations}.items():
             key = key_form.format(name=self.name, variation=variation)
-            th1s[key] = to_th1(key, self.binedges, areas)
+            th1s[key] = wrh.to_th1(key, self.binedges, areas, self.nbins)
         return th1s
 
 
 
     def to_root_file(self, filename, recreate=False, **kwargs):
         """Writes this histogram to a ROOT file as a set of TH1D's.
 
@@ -973,14 +967,15 @@
         mode = 'RECREATE' if recreate else 'UPDATE'
         rootfile = ROOT.TFile(filename, mode)
         if not rootfile.IsOpen():
             raise OSError(f'Cannot open ROOT file "{filepath}"')
         th1s = self.to_root(**kwargs)
         for key, th1 in th1s.items():
             th1.Write(key)
+        rootfile.Close()
 
 
 
 
 
 def zeros_like(a, name=None):
     '''
@@ -1439,33 +1434,22 @@
 
 
         :returns: dictionary of ROOT histograms (values) mapped by variation
             name (keys)
         :rtype: ``dict`` of ``str`` and ``ROOT.TH2D``
         """
         import ROOT
-        from array import array
-        def array2hist(areas, th2, errors=None):
-            nbins_x, nbins_y = self.nbins
-            for bin_index_x in range(nbins_x):
-                for bin_index_y in range(nbins_y):
-                    th2.SetBinContent(bin_index_x+1, bin_index_y+1, areas[bin_index_x, bin_index_y])
-                    if errors is not None:
-                        th2.SetBinError(bin_index_x+1, bin_index_y+1, errors[bin_index_x, bin_index_y])
-        def to_th2(name, binedges, areas):
-            th2 = ROOT.TH2D(name, name, len(binedges[0])-1, array('d', [b for b in binedges[0]]), len(binedges[1])-1, array('d', [b for b in binedges[1]]))
-            array2hist(areas, th2, errors=errors)
-            return th2
+        from . import writeroot_helpers as wrh
         th2s = {}
         # Add nominal
         key = key_form.format(name=self.name, variation=nominal_label)
-        th2s[key] = to_th2(key, self.binedges, self.areas)
+        th2s[key] = wrh.to_th2(key, self.binedges, self.areas, self.nbins)
         for variation, areas in {**self.uncorr_variations, **self.corr_variations}.items():
             key = key_form.format(name=self.name, variation=variation)
-            th2s[key] = to_th2(key, self.binedges, areas)
+            th2s[key] = wrh.to_th2(key, self.binedges, areas, self.nbins)
         return th2s
 
 
 
     def to_root_file(self, filename, recreate=False, **kwargs):
         """Writes this histogram to a ROOT file as a set of TH2D's.
```

### Comparing `heppyness-2.0.5/heppy/panel.py` & `heppyness-2.1.0/heppy/panel.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/plot.py` & `heppyness-2.1.0/heppy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,18 @@
         if p.xlabel: axes[i].set_xlabel(p.xlabel, ha='right', x=1., size='x-large')
         if p.ylabel: axes[i].set_ylabel(p.ylabel, ha='right', y=1., size='x-large')
         if p.logx: axes[i].set_xscale('log', nonpositive='clip')
         if p.logy: axes[i].set_yscale('log', nonpositive='clip')
         if p.ylims: axes[i].set_ylim(*p.ylims)
 
         axes[i].tick_params(which='both', bottom=True, top=True, left=True, right=True, direction='in')
+        try:
+            axes[i].ticklabel_format(useMathText=True, useOffset=False)
+        except AttributeError:
+            pass
         axes[i].set_xlim((min(x), max(x)))
         if xmax:
             axes[i].set_xlim((min(x), xmax))
         if xlims:
             axes[i].set_xlim(xlims)
         legend_handles, legend_labels = axes[i].get_legend_handles_labels()
         try:
@@ -241,23 +245,23 @@
         if not p.nolegend:
             # print('Updating plot legend.')
             if legend_outside:
                 # Also wraps the legend labels to make the legend high and narrow --- fits well on the side of the plot
                 #legend_labels = [textwrap.fill(label, width=30) for label in legend_labels]
                 # Attempt to make this work better with LaTeX-rendered labels by only
                 # line-breaking such labels that do not contain LaTeX math:
-                legend_labels = [label if '$' in label else textwrap.fill(label, width=30) for label in legend_labels]
+                legend_labels = [label if '$' in label or '\n' in label else textwrap.fill(label, width=30) for label in legend_labels]
                 axes[i].legend(legend_handles, legend_labels, bbox_to_anchor=(1.01, 1.0), fontsize='small', frameon=False, title=p.legend_title, loc=p.legend_loc)
             else:
                 axes[i].legend(legend_handles, legend_labels, title=p.legend_title, loc=p.legend_loc)
 
 
 
     if title: axes[0].set_title(title, x=0., ha='left', size='x-large')
-    fig.subplots_adjust(top=0.9, hspace=0.02)
+    fig.subplots_adjust(top=0.85, hspace=0.02)
     # fig.subplots_adjust(left=0.15, right=0.95, top=0.95, bottom=0.1, hspace=0.02)
     if legend_outside:
         fig.subplots_adjust(right=0.7)
 
     # Align y-labels horizontally
     fig.align_ylabels()
```

### Comparing `heppyness-2.0.5/heppy/readroot.py` & `heppyness-2.1.0/heppy/readroot.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/readroot_legacy.py` & `heppyness-2.1.0/heppy/readroot_legacy.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/readtrex.py` & `heppyness-2.1.0/heppy/readtrex.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/readyoda.py` & `heppyness-2.1.0/heppy/readyoda.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/scanroot.py` & `heppyness-2.1.0/heppy/scanroot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import ROOT
-ROOT.PyConfig.IgnoreCommandLineOptions = True
-
 # Generator of all paths to non-directories in the file
 # Copied from Andy Buckley, http://pastebin.com/GebcyHY9
 def path_generator(d, basepath='/'):
     for key in d.GetListOfKeys():
         kname = key.GetName()
         if key.IsFolder() and 'TDirectory' in key.GetClassName():
             for i in path_generator(d.Get(kname), basepath+kname+'/'):
@@ -40,14 +37,16 @@
 
 
 
 # Get list of all histogram paths in a ROOT file that pass filters:
 # @param include     list of strings that paths need to contain to be considered
 # @param exclude     list of strings that paths may not contain to be considered  
 def get_keys(fpath, all=[], some=[], none=[]):
+    import ROOT
+    ROOT.PyConfig.IgnoreCommandLineOptions = True
     rootfile = ROOT.TFile(fpath, 'r')
     rootfile.cd()
     paths = []
     for path in path_generator(rootfile):
         if string_contains_all(path, all) and string_contains_some(path, some) and string_contains_none(path, none):
             paths.append(path)
     return paths
```

### Comparing `heppyness-2.0.5/heppy/uncertainty.py` & `heppyness-2.1.0/heppy/uncertainty.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/value.py` & `heppyness-2.1.0/heppy/value.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppy/yodarun.py` & `heppyness-2.1.0/heppy/yodarun.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/heppyness.egg-info/PKG-INFO` & `heppyness-2.1.0/heppyness.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heppyness
-Version: 2.0.5
+Version: 2.1.0
 Home-page: https://gitlab.cern.ch/strichte/heppy
 Author: Stefan Richter
 Author-email: stefan.richter@cern.ch
 Maintainer: Stefan Richter
 Maintainer-email: stefan.richter@cern.ch
 License: HEP license, based on MIT license
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: uproot
+Requires-Dist: uproot-methods
+Requires-Dist: awkward
+Requires-Dist: pandas
+Requires-Dist: pyyaml
+Requires-Dist: sphinx_rtd_theme
 
 # Heppy
 
 Heppy provides pythonic data structures and a few high-level tools for high-energy physics. In particular, it provides very useful histogram classes that neatly integrate systematic variations (which, to my knowledge, no other histogram class that's widely used in HEP does) and support common operations such as addition, division, rebinning, slicing, projecting, integrating. It also provides flexible matplotlib-based plotting.
 
 The documentation can be found [here](https://heppy.readthedocs.io).
```

### Comparing `heppyness-2.0.5/heppyness.egg-info/SOURCES.txt` & `heppyness-2.1.0/heppyness.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 heppy/readroot.py
 heppy/readroot_legacy.py
 heppy/readtrex.py
 heppy/readyoda.py
 heppy/scanroot.py
 heppy/uncertainty.py
 heppy/value.py
+heppy/writeroot_helpers.py
 heppy/yodarun.py
 heppyness.egg-info/PKG-INFO
 heppyness.egg-info/SOURCES.txt
 heppyness.egg-info/dependency_links.txt
 heppyness.egg-info/requires.txt
 heppyness.egg-info/top_level.txt
 test/test_heatmap.py
```

### Comparing `heppyness-2.0.5/setup.py` & `heppyness-2.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='heppyness',
     license='HEP license, based on MIT license',
-    version='2.0.5',
+    version='2.1.0',
     author='Stefan Richter',
     author_email='stefan.richter@cern.ch',
     maintainer='Stefan Richter',
     maintainer_email='stefan.richter@cern.ch',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `heppyness-2.0.5/test/test_heatmap.py` & `heppyness-2.1.0/test/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/test/test_histogram1d.py` & `heppyness-2.1.0/test/test_histogram1d.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/test/test_histogram2d.py` & `heppyness-2.1.0/test/test_histogram2d.py`

 * *Files identical despite different names*

### Comparing `heppyness-2.0.5/test/test_readroot.py` & `heppyness-2.1.0/test/test_readroot.py`

 * *Files identical despite different names*

