# Comparing `tmp/resaid-0.1.5.tar.gz` & `tmp/resaid-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resaid-0.1.5.tar", last modified: Mon Mar 25 21:04:58 2024, max compression
+gzip compressed data, was "resaid-0.1.6.tar", last modified: Wed Apr 10 22:54:40 2024, max compression
```

## Comparing `resaid-0.1.5.tar` & `resaid-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-25 21:04:58.283638 resaid-0.1.5/
--rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.5/LICENSE
--rw-rw-rw-   0        0        0      554 2024-03-25 21:04:58.281629 resaid-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.5/README.md
--rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.5/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-25 21:04:58.255841 resaid-0.1.5/resaid/
--rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.5/resaid/__init__.py
--rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.5/resaid/dca.py
--rw-rw-rw-   0        0        0    19916 2024-03-25 21:02:56.000000 resaid-0.1.5/resaid/econ.py
-drwxrwxrwx   0        0        0        0 2024-03-25 21:04:58.275767 resaid-0.1.5/resaid.egg-info/
--rw-rw-rw-   0        0        0      554 2024-03-25 21:04:58.000000 resaid-0.1.5/resaid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-03-25 21:04:58.000000 resaid-0.1.5/resaid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-25 21:04:58.000000 resaid-0.1.5/resaid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-25 21:04:58.000000 resaid-0.1.5/resaid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-25 21:04:58.000000 resaid-0.1.5/resaid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-25 21:04:58.284635 resaid-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1179 2024-03-25 21:03:25.000000 resaid-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.770402 resaid-0.1.6/
+-rw-rw-rw-   0        0        0     1067 2023-10-05 19:55:40.000000 resaid-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0      704 2024-04-10 22:54:40.762871 resaid-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2022-02-28 19:33:00.000000 resaid-0.1.6/README.md
+-rw-rw-rw-   0        0        0      103 2023-10-09 21:04:28.000000 resaid-0.1.6/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.696797 resaid-0.1.6/resaid/
+-rw-rw-rw-   0        0        0        0 2021-10-06 19:02:31.000000 resaid-0.1.6/resaid/__init__.py
+-rw-rw-rw-   0        0        0    42266 2023-12-01 16:38:17.000000 resaid-0.1.6/resaid/dca.py
+-rw-rw-rw-   0        0        0    19951 2024-03-27 20:04:24.000000 resaid-0.1.6/resaid/econ.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:54:40.756429 resaid-0.1.6/resaid.egg-info/
+-rw-rw-rw-   0        0        0      704 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-10 22:54:40.000000 resaid-0.1.6/resaid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 22:54:40.772404 resaid-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2024-04-08 16:46:50.000000 resaid-0.1.6/setup.py
```

### Comparing `resaid-0.1.5/LICENSE` & `resaid-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `resaid-0.1.5/resaid/dca.py` & `resaid-0.1.6/resaid/dca.py`

 * *Files identical despite different names*

### Comparing `resaid-0.1.5/resaid/econ.py` & `resaid-0.1.6/resaid/econ.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
         #elif discount_rate < 0:
         #    l_npv = 99999
         #else:
         l_npv = np.sum(self._cashflow/ (1+discount_rate)**np.arange(0, len(self._cashflow)))
 
         return l_npv
     
-    def get_irr(self):
-        guess = .5/12
+    def get_irr(self, iterations=50):
+        guess = .1/12
 
         constraint_bounds = ((1e-6, .16),) 
 
         if np.sum(self._cashflow) < 0:
             result = 0
         else:
-            result = newton(self.get_npv, guess)
+            result = newton(self.get_npv, guess, maxiter=iterations)
 
         try:
             result = np.power(1+result,12)-1
         except Exception as e:
             print(result)
             raise e
```

### Comparing `resaid-0.1.5/setup.py` & `resaid-0.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="resaid",
-    version="0.1.5",
+    version="0.1.6",
     author="Greg Easley",
     author_email="greg@easley.dev",
     description="Reservoir engineering tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/geasley-rsc/resaid",
+    url="https://github.com/gregeasley/resaid",
     project_urls={
-        "Bug Tracker": "https://github.com/geasley-rsc/resaid/issues",
+        "Bug Tracker": "https://github.com/gregeasley/resaid/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
```

