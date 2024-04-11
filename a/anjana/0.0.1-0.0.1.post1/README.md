# Comparing `tmp/anjana-0.0.1.tar.gz` & `tmp/anjana-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anjana-0.0.1.tar", max compression
+gzip compressed data, was "anjana-0.0.1.post1.tar", max compression
```

## Comparing `anjana-0.0.1.tar` & `anjana-0.0.1.post1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11353 2024-03-19 16:33:35.335622 anjana-0.0.1/LICENSE
--rw-r--r--   0        0        0     4690 2024-03-19 19:54:09.811315 anjana-0.0.1/README.md
--rw-r--r--   0        0        0      743 2024-03-19 16:40:51.972587 anjana-0.0.1/anjana/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/__init__.py
--rw-r--r--   0        0        0     6416 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/_beta_likeness.py
--rw-r--r--   0        0        0     3629 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/_delta_disclosure.py
--rw-r--r--   0        0        0    10095 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/_k_anonymity.py
--rw-r--r--   0        0        0    13419 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/_l_diversity.py
--rw-r--r--   0        0        0     3501 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/_t_closeness.py
--rw-r--r--   0        0        0      784 2024-03-19 20:55:50.632954 anjana-0.0.1/anjana/anonymity/utils/__init__.py
--rw-r--r--   0        0        0     3552 2024-04-11 06:37:38.765784 anjana-0.0.1/anjana/anonymity/utils/utils.py
--rw-r--r--   0        0        0     2048 2024-04-11 06:41:04.099859 anjana-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6179 1970-01-01 00:00:00.000000 anjana-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11353 2024-03-19 16:17:26.810719 anjana-0.0.1.post1/LICENSE
+-rw-r--r--   0        0        0     4711 2024-04-11 07:00:56.429436 anjana-0.0.1.post1/README.md
+-rw-r--r--   0        0        0      749 2024-04-11 07:42:52.316264 anjana-0.0.1.post1/anjana/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/__init__.py
+-rw-r--r--   0        0        0     6416 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_beta_likeness.py
+-rw-r--r--   0        0        0     3629 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_delta_disclosure.py
+-rw-r--r--   0        0        0    10095 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_k_anonymity.py
+-rw-r--r--   0        0        0    13419 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_l_diversity.py
+-rw-r--r--   0        0        0     3501 2024-04-10 10:21:10.035760 anjana-0.0.1.post1/anjana/anonymity/_t_closeness.py
+-rw-r--r--   0        0        0      784 2024-03-20 08:17:01.773369 anjana-0.0.1.post1/anjana/anonymity/utils/__init__.py
+-rw-r--r--   0        0        0     3552 2024-04-10 10:40:59.006301 anjana-0.0.1.post1/anjana/anonymity/utils/utils.py
+-rw-r--r--   0        0        0     2054 2024-04-11 08:17:33.117704 anjana-0.0.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 anjana-0.0.1.post1/PKG-INFO
```

### Comparing `anjana-0.0.1/LICENSE` & `anjana-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/README.md` & `anjana-0.0.1.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 * The **level of anonymity to be applied**, e.g. _k_ (for _k-anonymity_), _ℓ_ (for _ℓ-diversity_), _t_ (for _t-closeness_), _β_ (for _basic or enhanced β-likeness_), etc.
 * Maximum **level of record suppression** allowed (from 0 to 100).
 * Dictionary containing one dictionary for each quasi-identifier with the **hierarchies** and the levels.
 
 ### Example: apply _k-anonymity_, _ℓ-diversity_ and _t-closeness_ to the [adult dataset](https://archive.ics.uci.edu/dataset/2/adult) with some predefined hierarchies:
 ```python
 import pandas as pd
-from anonymity import k_anonymity, l_diversity, t_closeness
+import anjana
+from anjana.anonymity import k_anonymity, l_diversity, t_closeness
 
 # Read and process the data
 data = pd.read_csv("adult.csv") 
 data.columns = data.columns.str.strip()
 cols = [
     "workclass",
     "education",
```

### Comparing `anjana-0.0.1/anjana/__init__.py` & `anjana-0.0.1.post1/anjana/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """ANJANA is an open source framework for anonymizing data with different techniques."""
 
-__version__ = "0.0.1"
+__version__ = "0.0.1.post1"
```

### Comparing `anjana-0.0.1/anjana/anonymity/__init__.py` & `anjana-0.0.1.post1/anjana/anonymity/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/_beta_likeness.py` & `anjana-0.0.1.post1/anjana/anonymity/_beta_likeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/_delta_disclosure.py` & `anjana-0.0.1.post1/anjana/anonymity/_delta_disclosure.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/_k_anonymity.py` & `anjana-0.0.1.post1/anjana/anonymity/_k_anonymity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/_l_diversity.py` & `anjana-0.0.1.post1/anjana/anonymity/_l_diversity.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/_t_closeness.py` & `anjana-0.0.1.post1/anjana/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/utils/__init__.py` & `anjana-0.0.1.post1/anjana/anonymity/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/anjana/anonymity/utils/utils.py` & `anjana-0.0.1.post1/anjana/anonymity/utils/utils.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.1/pyproject.toml` & `anjana-0.0.1.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anjana"
-version = "0.0.1"
+version = "0.0.1.post1"
 description = "ANJANA is an open source framework for applying different anonymity techniques."
 authors = [
     "Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>",
     "Álvaro López García <aloga@ifca.unican.es>"
 ]
 maintainers = ["Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>"]
 license = "Apache License 2.0"
```

### Comparing `anjana-0.0.1/PKG-INFO` & `anjana-0.0.1.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anjana
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: ANJANA is an open source framework for applying different anonymity techniques.
 Home-page: https://gitlab.ifca.es/privacy-security/anjana
 License: Apache-2.0
 Keywords: anonymity,privacy
 Author: Judith Sáinz-Pardo Díaz
 Author-email: sainzpardo@ifca.unican.es
 Maintainer: Judith Sáinz-Pardo Díaz
@@ -66,15 +66,16 @@
 * The **level of anonymity to be applied**, e.g. _k_ (for _k-anonymity_), _ℓ_ (for _ℓ-diversity_), _t_ (for _t-closeness_), _β_ (for _basic or enhanced β-likeness_), etc.
 * Maximum **level of record suppression** allowed (from 0 to 100).
 * Dictionary containing one dictionary for each quasi-identifier with the **hierarchies** and the levels.
 
 ### Example: apply _k-anonymity_, _ℓ-diversity_ and _t-closeness_ to the [adult dataset](https://archive.ics.uci.edu/dataset/2/adult) with some predefined hierarchies:
 ```python
 import pandas as pd
-from anonymity import k_anonymity, l_diversity, t_closeness
+import anjana
+from anjana.anonymity import k_anonymity, l_diversity, t_closeness
 
 # Read and process the data
 data = pd.read_csv("adult.csv") 
 data.columns = data.columns.str.strip()
 cols = [
     "workclass",
     "education",
```

