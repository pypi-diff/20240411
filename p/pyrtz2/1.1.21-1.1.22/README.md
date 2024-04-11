# Comparing `tmp/pyrtz2-1.1.21.tar.gz` & `tmp/pyrtz2-1.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.21.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.22.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.21.tar` & `pyrtz2-1.1.22.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.21/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.21/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.21/LICENSE
--rw-r--r--   0        0        0      455 2024-04-05 17:28:24.205830 pyrtz2-1.1.21/README.md
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.21/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.21/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   331740 2024-04-04 23:26:50.939244 pyrtz2-1.1.21/example/con050_curves.pdf
--rw-r--r--   0        0        0     1749 2024-04-04 23:26:34.450692 pyrtz2-1.1.21/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.21/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.21/example/test.py
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.21/pyproject.toml
--rw-r--r--   0        0        0       62 2024-04-06 22:49:29.492506 pyrtz2-1.1.21/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.21/pyrtz2/afm.py
--rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.21/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.21/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     5106 2024-04-06 15:47:56.375397 pyrtz2-1.1.21/pyrtz2/asylum.py
--rw-r--r--   0        0        0    17569 2024-04-06 21:25:58.646302 pyrtz2-1.1.21/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-02 14:59:14.529838 pyrtz2-1.1.21/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.21/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.21/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.21/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.21/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.1.21/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     2826 2024-04-06 15:45:15.625467 pyrtz2-1.1.21/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     2874 2024-04-06 15:44:47.448540 pyrtz2-1.1.21/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.21/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1186 2024-04-06 15:49:10.935231 pyrtz2-1.1.21/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1321 2024-04-06 21:53:03.543206 pyrtz2-1.1.21/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1707 2024-04-06 15:49:56.149071 pyrtz2-1.1.21/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3230 2024-04-06 15:49:27.361168 pyrtz2-1.1.21/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.21/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.21/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3275 2024-04-06 15:49:11.334196 pyrtz2-1.1.21/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.21/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.21/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.21/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.21/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.21/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 pyrtz2-1.1.21/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.22/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.22/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.22/LICENSE
+-rw-r--r--   0        0        0      770 2024-04-10 14:20:28.536754 pyrtz2-1.1.22/README.md
+-rw-r--r--   0        0        0   108151 2024-04-09 18:10:30.442428 pyrtz2-1.1.22/example/con050.PNG
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.22/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.22/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.1.22/example/con050_curves.pdf
+-rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.1.22/example/con050_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.22/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.22/example/test.py
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.22/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-04-11 17:11:34.850059 pyrtz2-1.1.22/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.22/pyrtz2/afm.py
+-rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.22/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.22/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     5106 2024-04-06 15:47:56.375397 pyrtz2-1.1.22/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    17629 2024-04-11 17:08:54.848531 pyrtz2-1.1.22/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-04-09 18:06:56.894949 pyrtz2-1.1.22/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.22/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.22/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.22/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.22/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.1.22/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     2826 2024-04-06 15:45:15.625467 pyrtz2-1.1.22/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     2874 2024-04-06 15:44:47.448540 pyrtz2-1.1.22/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.22/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1186 2024-04-06 15:49:10.935231 pyrtz2-1.1.22/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1718 2024-04-08 16:35:01.806773 pyrtz2-1.1.22/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1707 2024-04-06 15:49:56.149071 pyrtz2-1.1.22/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3230 2024-04-06 15:49:27.361168 pyrtz2-1.1.22/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.22/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.22/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3275 2024-04-06 15:49:11.334196 pyrtz2-1.1.22/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.22/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.22/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.22/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.22/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.22/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1501 1970-01-01 00:00:00.000000 pyrtz2-1.1.22/PKG-INFO
```

### Comparing `pyrtz2-1.1.21/LICENSE` & `pyrtz2-1.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.1.22/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.1.22/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.1.22/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.1.22/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.1.22/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.1.22/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.1.22/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.1.22/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.1.22/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.1.22/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyproject.toml` & `pyrtz2-1.1.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/afm.py` & `pyrtz2-1.1.22/pyrtz2/afm.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/assets/style.css` & `pyrtz2-1.1.22/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/asylum.py` & `pyrtz2-1.1.22/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/curves.py` & `pyrtz2-1.1.22/pyrtz2/curves.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
         if self.contact_values is None:
             self.contact_values = self.data.iloc[self.contact_index].copy()
         return self.contact_values
 
     def adjust_to_contact(self) -> None:
         self.data -= self.get_contact_values()
 
-    def get_data_between(self, start: int, last: int) -> pd.DataFrame:
-        return self.data.iloc[start:last].reset_index(drop=True)
+    def get_data_between(self, first: int, last: int) -> pd.DataFrame:
+        return self.data.iloc[first:last].reset_index(drop=True)
 
     def get_approach(self) -> pd.DataFrame:
         return self.get_data_between(0, self.dwell_range[0])
 
     def get_preapproach(self) -> pd.DataFrame:
         return self.get_data_between(0, self.contact_index)
 
@@ -104,19 +104,20 @@
         return self.get_data_between(self.contact_index, self.dwell_range[0])
 
     def get_indent_until(self, ind: float) -> pd.DataFrame:
         indent = self.get_indent()
         ind_index = (np.abs(indent['ind'].to_numpy() - ind)).argmin()
         return indent.iloc[:ind_index].reset_index(drop=True)
 
-    def get_indent_between(self, start: float, last: float) -> pd.DataFrame:
+    def get_indent_between(self, first: float, last: float) -> pd.DataFrame:
         indent = self.get_indent()
-        start_index = int(start * len(indent))
-        last_index = int(last * len(indent))
-        return indent.iloc[start_index:last_index].reset_index(drop=True)
+        f = indent['f'].to_numpy()
+        first_index = np.argmin(np.abs(f - f[-1] * first))
+        last_index = np.argmin(np.abs(f - f[-1] * last))
+        return indent.iloc[first_index:last_index].reset_index(drop=True)
 
     def get_dwell(self) -> pd.DataFrame:
         return self.get_data_between(self.dwell_range[0], self.dwell_range[1])
 
     def get_repulsion(self) -> pd.DataFrame:
         dwell = self.get_dwell()
         max_ind = dwell['ind'].argmax()
```

### Comparing `pyrtz2-1.1.21/pyrtz2/fit.py` & `pyrtz2-1.1.22/pyrtz2/fit.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,23 +103,23 @@
 
 def biexponential_fit(x, y, bound=False):
     if bound:
         def bnd_wrapper(t, c, tau1, tau2):
             return biexponential(t, y[0], c, tau1, tau2, y[-1])
 
         bounds = ([0, 0, 0], [1, np.inf, np.inf])
-        p0 = [0.5, 0.1, 1]
+        p0 = [0.4, 1, 0.1]
         popt, _ = curve_fit(bnd_wrapper, x, y,
                             bounds=bounds, p0=p0, jac='3-point')
         args = [y[0], *popt, y[-1]]
     else:
         def ubnd_wrapper(t, c, tau1, tau2, y_f):
             return biexponential(t, y[0], c, tau1, tau2, y_f)
 
-        p0 = [0.5, 0.1, 1, 0]
+        p0 = [0.4, 1, 0.1, 0]
         bounds = ([0, 0, 0, -np.inf], [1, np.inf, np.inf, np.inf])
         popt, _ = curve_fit(ubnd_wrapper, x, y,
                             bounds=bounds, p0=p0, jac='3-point')
         args = [y[0], *popt]
 
     y_pred = biexponential(x, *args)
     r2_score = r2(y, y_pred)
@@ -128,23 +128,23 @@
 
 def poroelastic_fit(x, y, bound=False):
     if bound:
         def bnd_wrapper(t, c, tau1, tau2):
             return poroelastic(t, y[0], c, tau1, tau2, y[-1])
 
         bounds = ([0, 0, 0], [1, np.inf, np.inf])
-        p0 = [0.5, 0.1, 1]
+        p0 = [0.4, 1, 0.1]
         popt, _ = curve_fit(bnd_wrapper, x, y,
                             bounds=bounds, p0=p0, jac='3-point')
         args = [y[0], *popt, y[-1]]
     else:
         def ubnd_wrapper(t, c, tau1, tau2, y_f):
             return poroelastic(t, y[0], c, tau1, tau2, y_f)
 
-        p0 = [0.5, 0.1, 1, 0]
+        p0 = [0.4, 1, 0.1, 0]
         bounds = ([0, 0, 0, -np.inf], [1, np.inf, np.inf, np.inf])
         popt, _ = curve_fit(ubnd_wrapper, x, y,
                             bounds=bounds, p0=p0, jac='3-point')
         args = [y[0], *popt]
 
     y_pred = poroelastic(x, *args)
     r2_score = r2(y, y_pred)
```

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.22/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.22/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.22/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.22/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.22/pyrtz2/src/components/fig_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.22/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.22/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.22/pyrtz2/src/components/image_frame.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,15 +25,27 @@
         # THIS ONLY SHOWS THE FIRST IMAGE IF THERE IS ONE
         if images.get(new_key):
             image_path = images[new_key][0]
             image_src = load_image(image_path)
             return image_src
         else:
             return ''
-
+    '''
+    @app.callback(
+        Output('click-data', 'children'),
+        Input('image-graph', 'clickData')
+    )
+    def store_cell_position(clickData):
+        if clickData is None:
+            return []
+        else:
+            # Extract coordinates from the clickData
+            x, y = clickData['points'][0]['x'], clickData['points'][0]['y']
+            return [x, y]
+    '''
     return html.Div(
         className='image',
         children=[
             html.Img(
                 id=ids.IMAGE_FRAME,
                 style={
                     'display': 'flex',
```

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.22/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.22/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.22/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.22/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.22/pyrtz2/src/data/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.22/pyrtz2/src/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.22/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.22/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.21/PKG-INFO` & `pyrtz2-1.1.22/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.21
+Version: 1.1.22
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
@@ -37,13 +37,18 @@
 
 Please see the example folder. To run the HTML dash app interface simply use:
 
 ```
 from pyrtz2 import app
 app.run()
 ```
+You should see this interface:
+
+![pyrtz2.app](./example/con050.PNG)
+
+You can select the contact point interactively. It will perform fits for approach and dwell parts of the curves using Hertzian and biexponential equations. After downloading the `csv` of fits, you can download those curves in one pdf files.
 
 These options are under development:
 - Show Fits
 - Download Image Data
 - Download Experiment
```

