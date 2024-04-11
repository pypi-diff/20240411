# Comparing `tmp/software_development_project_team1-0.1.3.tar.gz` & `tmp/software_development_project_team1-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "software_development_project_team1-0.1.3.tar", last modified: Thu Apr 11 18:50:39 2024, max compression
+gzip compressed data, was "software_development_project_team1-0.1.4.tar", last modified: Thu Apr 11 18:56:32 2024, max compression
```

## Comparing `software_development_project_team1-0.1.3.tar` & `software_development_project_team1-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 18:50:39.692883 software_development_project_team1-0.1.3/
--rw-rw-rw-   0        0        0     1086 2024-02-19 08:02:42.000000 software_development_project_team1-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      620 2024-04-11 18:50:39.692883 software_development_project_team1-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5226 2024-04-11 16:58:15.000000 software_development_project_team1-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 18:50:39.692883 software_development_project_team1-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      833 2024-04-11 18:50:33.000000 software_development_project_team1-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:50:39.672529 software_development_project_team1-0.1.3/software_development_project_team1/
--rw-rw-rw-   0        0        0        0 2024-04-10 17:43:52.000000 software_development_project_team1-0.1.3/software_development_project_team1/__init__.py
--rw-rw-rw-   0        0        0    11922 2024-04-11 16:55:28.000000 software_development_project_team1-0.1.3/software_development_project_team1/autoencoder.py
--rw-rw-rw-   0        0        0    17650 2024-04-11 16:54:24.000000 software_development_project_team1-0.1.3/software_development_project_team1/genetic_algorithm.py
--rw-rw-rw-   0        0        0    10170 2024-04-11 16:54:24.000000 software_development_project_team1-0.1.3/software_development_project_team1/identify_attacker.py
--rw-rw-rw-   0        0        0    37373 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.3/software_development_project_team1/projet_interface_class.py
--rw-rw-rw-   0        0        0    15234 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.3/software_development_project_team1/ui.py
-drwxrwxrwx   0        0        0        0 2024-04-11 18:50:39.691410 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/
--rw-rw-rw-   0        0        0      620 2024-04-11 18:50:39.000000 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2024-04-11 18:50:39.000000 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 18:50:39.000000 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-04-11 18:50:39.000000 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-04-11 18:50:39.000000 software_development_project_team1-0.1.3/software_development_project_team1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 18:56:32.537979 software_development_project_team1-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2024-02-19 08:02:42.000000 software_development_project_team1-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      620 2024-04-11 18:56:32.536677 software_development_project_team1-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5226 2024-04-11 16:58:15.000000 software_development_project_team1-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 18:56:32.537979 software_development_project_team1-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      833 2024-04-11 18:56:26.000000 software_development_project_team1-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:56:32.520113 software_development_project_team1-0.1.4/software_development_project_team1/
+-rw-rw-rw-   0        0        0        0 2024-04-10 17:43:52.000000 software_development_project_team1-0.1.4/software_development_project_team1/__init__.py
+-rw-rw-rw-   0        0        0    11922 2024-04-11 16:55:28.000000 software_development_project_team1-0.1.4/software_development_project_team1/autoencoder.py
+-rw-rw-rw-   0        0        0    17650 2024-04-11 16:54:24.000000 software_development_project_team1-0.1.4/software_development_project_team1/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    10170 2024-04-11 18:55:37.000000 software_development_project_team1-0.1.4/software_development_project_team1/identify_attacker.py
+-rw-rw-rw-   0        0        0    37373 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.4/software_development_project_team1/projet_interface_class.py
+-rw-rw-rw-   0        0        0    15234 2024-04-10 17:43:54.000000 software_development_project_team1-0.1.4/software_development_project_team1/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-11 18:56:32.535364 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/
+-rw-rw-rw-   0        0        0      620 2024-04-11 18:56:32.000000 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2024-04-11 18:56:32.000000 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 18:56:32.000000 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-11 18:56:32.000000 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-04-11 18:56:32.000000 software_development_project_team1-0.1.4/software_development_project_team1.egg-info/top_level.txt
```

### Comparing `software_development_project_team1-0.1.3/LICENSE` & `software_development_project_team1-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/PKG-INFO` & `software_development_project_team1-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software_development_project_team1
-Version: 0.1.3
+Version: 0.1.4
 Summary: Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm
 Author: Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes
 Author-email: laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `software_development_project_team1-0.1.3/README.md` & `software_development_project_team1-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/setup.py` & `software_development_project_team1-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
 name='software_development_project_team1',
-version='0.1.3',
+version='0.1.4',
 author='Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes',
 author_email='laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr',
 description='Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1/autoencoder.py` & `software_development_project_team1-0.1.4/software_development_project_team1/autoencoder.py`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1/genetic_algorithm.py` & `software_development_project_team1-0.1.4/software_development_project_team1/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1/identify_attacker.py` & `software_development_project_team1-0.1.4/software_development_project_team1/identify_attacker.py`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1/projet_interface_class.py` & `software_development_project_team1-0.1.4/software_development_project_team1/projet_interface_class.py`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1/ui.py` & `software_development_project_team1-0.1.4/software_development_project_team1/ui.py`

 * *Files identical despite different names*

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1.egg-info/PKG-INFO` & `software_development_project_team1-0.1.4/software_development_project_team1.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: software-development-project-team1
-Version: 0.1.3
+Version: 0.1.4
 Summary: Software to help victims portray a culprit using an autoencoder model trained on the CelebA dataset and a genetic algorithm
 Author: Laetitia Guérout, Théo Berthet, Lucas Bodelle & Synne Trettenes
 Author-email: laetitia.guerout@insa-lyon.fr, theo.berthet@insa-lyon.fr, lucas.bodelle@insa-lyon.fr, synne-moe.trettenes@insa-lyon.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `software_development_project_team1-0.1.3/software_development_project_team1.egg-info/SOURCES.txt` & `software_development_project_team1-0.1.4/software_development_project_team1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

