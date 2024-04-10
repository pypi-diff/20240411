# Comparing `tmp/VLCDA-1.0.6.tar.gz` & `tmp/VLCDA-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.6.tar", last modified: Wed Apr 10 22:03:08 2024, max compression
+gzip compressed data, was "VLCDA-1.0.7.tar", last modified: Wed Apr 10 22:16:27 2024, max compression
```

## Comparing `VLCDA-1.0.6.tar` & `VLCDA-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:03:08.684787 VLCDA-1.0.6/
--rw-rw-rw-   0        0        0     1077 2023-11-28 23:29:37.000000 VLCDA-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     2043 2024-04-10 22:03:08.684787 VLCDA-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-11-28 23:29:37.000000 VLCDA-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 22:03:08.647931 VLCDA-1.0.6/VLCDA/
--rw-rw-rw-   0        0        0    35446 2024-04-10 21:37:51.000000 VLCDA-1.0.6/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-11-28 23:29:37.000000 VLCDA-1.0.6/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:03:08.664634 VLCDA-1.0.6/VLCDA.egg-info/
--rw-rw-rw-   0        0        0     2043 2024-04-10 22:03:08.000000 VLCDA-1.0.6/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2024-04-10 22:03:08.000000 VLCDA-1.0.6/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:03:08.000000 VLCDA-1.0.6/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 22:03:08.000000 VLCDA-1.0.6/VLCDA.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 22:03:08.682779 VLCDA-1.0.6/dist/
--rw-rw-rw-   0        0        0     7475 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.0-py3-none-any.whl
--rw-rw-rw-   0        0        0     7746 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.0.tar.gz
--rw-rw-rw-   0        0        0     7472 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     7531 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.1.tar.gz
--rw-rw-rw-   0        0        0     8172 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.2-py3-none-any.whl
--rw-rw-rw-   0        0        0     8301 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.2.tar.gz
--rw-rw-rw-   0        0        0     8181 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.3-py3-none-any.whl
--rw-rw-rw-   0        0        0    50423 2023-11-28 23:29:37.000000 VLCDA-1.0.6/dist/VLCDA-1.0.3.tar.gz
--rw-rw-rw-   0        0        0       42 2024-04-10 22:03:08.685794 VLCDA-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-04-10 22:03:05.000000 VLCDA-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:16:27.744579 VLCDA-1.0.7/
+-rw-rw-rw-   0        0        0     1077 2023-11-28 23:29:37.000000 VLCDA-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     2043 2024-04-10 22:16:27.743582 VLCDA-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1406 2023-11-28 23:29:37.000000 VLCDA-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-10 22:16:27.697261 VLCDA-1.0.7/VLCDA/
+-rw-rw-rw-   0        0        0    35397 2024-04-10 22:13:20.000000 VLCDA-1.0.7/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0        0 2023-11-28 23:29:37.000000 VLCDA-1.0.7/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:16:27.713951 VLCDA-1.0.7/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0     2043 2024-04-10 22:16:27.000000 VLCDA-1.0.7/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2024-04-10 22:16:27.000000 VLCDA-1.0.7/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 22:16:27.000000 VLCDA-1.0.7/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-10 22:16:27.000000 VLCDA-1.0.7/VLCDA.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 22:16:27.740535 VLCDA-1.0.7/dist/
+-rw-rw-rw-   0        0        0     7475 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7746 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.0.tar.gz
+-rw-rw-rw-   0        0        0     7472 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7531 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.1.tar.gz
+-rw-rw-rw-   0        0        0     8172 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0     8301 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     8181 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.3-py3-none-any.whl
+-rw-rw-rw-   0        0        0    50423 2023-11-28 23:29:37.000000 VLCDA-1.0.7/dist/VLCDA-1.0.3.tar.gz
+-rw-rw-rw-   0        0        0       42 2024-04-10 22:16:27.744579 VLCDA-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-04-10 22:16:22.000000 VLCDA-1.0.7/setup.py
```

### Comparing `VLCDA-1.0.6/LICENSE.txt` & `VLCDA-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/PKG-INFO` & `VLCDA-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.6
+Version: 1.0.7
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
```

### Comparing `VLCDA-1.0.6/README.md` & `VLCDA-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/VLCDA/Logic_Circuits_Evolution.py` & `VLCDA-1.0.7/VLCDA/Logic_Circuits_Evolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,15 +674,15 @@
                 child.calculateFitness(logicFunction)
                 child.calculateNoiseFitness()
                 
                 listGenomes.append(child)
 
                        
             self.getBestGenome(listGenomes).copyGene(bestParent)
-            self.makeHistgram(bestParent.fitness)
+            self.addToFitnessList(bestParent.fitness)
 
             if(self.totalGeneration % 1000 == 0):
               self.display(bestParent.genotipo, bestParent.fitness,bestParent.noiseFitness,self.totalGeneration)
             
             if(self.totalGeneration>=self.maxGeneration):
                 break
             
@@ -695,16 +695,14 @@
                     bestParent.calculateNoiseFitness()
                     print("Recalculating fitness without faults...")
                     self.display(bestParent.genotipo,bestParent.fitness,bestParent.noiseFitness,self.totalGeneration)
 
                     break
         timeDiff = datetime.datetime.now() - self.startTime
         print("The end in: ",str(timeDiff))
-
-    def evolutionTest(self,genome,logicFunction):
         
         bestParent = Genoma(genome.numberOfGenes,genome.nInputs,genome.nOutputs)
         genome.copyGene(bestParent)
       
         bestParent.generate_parent() # Generate the first generation (The first Parent)
         bestParent.calculateFitness(logicFunction)  # Get the first generation fitness
         bestParent.calculateNoiseFitness()
```

### Comparing `VLCDA-1.0.6/VLCDA.egg-info/PKG-INFO` & `VLCDA-1.0.7/VLCDA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VLCDA
-Version: 1.0.6
+Version: 1.0.7
 Summary: Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos
 Home-page: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Download-URL: https://github.com/HumbertoTavora/Logic-Circuits-Evolution
 Author: Humberto Távora, Stefan Blawid, Yasmin Maria
 Author-email: humbertocctg@gmail.com
 License: MIT
 Keywords: Genetic,Algorithm,Logic Circuits,Evolution,Optimization
```

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.0-py3-none-any.whl` & `VLCDA-1.0.7/dist/VLCDA-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.0.tar.gz` & `VLCDA-1.0.7/dist/VLCDA-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.1-py3-none-any.whl` & `VLCDA-1.0.7/dist/VLCDA-1.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.1.tar.gz` & `VLCDA-1.0.7/dist/VLCDA-1.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.2-py3-none-any.whl` & `VLCDA-1.0.7/dist/VLCDA-1.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.2.tar.gz` & `VLCDA-1.0.7/dist/VLCDA-1.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.3-py3-none-any.whl` & `VLCDA-1.0.7/dist/VLCDA-1.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/dist/VLCDA-1.0.3.tar.gz` & `VLCDA-1.0.7/dist/VLCDA-1.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.6/setup.py` & `VLCDA-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup(
     name = "VLCDA",
-    version = "1.0.6",
+    version = "1.0.7",
     license='MIT',
     description = "Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos",
     author = "Humberto Távora, Stefan Blawid, Yasmin Maria",
     author_email = 'humbertocctg@gmail.com',
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
```

