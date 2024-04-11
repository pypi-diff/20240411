# Comparing `tmp/VLCDA-1.0.8.tar.gz` & `tmp/VLCDA-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VLCDA-1.0.8.tar", last modified: Wed Apr 10 22:30:03 2024, max compression
+gzip compressed data, was "VLCDA-1.0.9.tar", last modified: Thu Apr 11 04:31:21 2024, max compression
```

## Comparing `VLCDA-1.0.8.tar` & `VLCDA-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:30:03.123537 VLCDA-1.0.8/
--rw-rw-rw-   0        0        0     1077 2023-11-28 23:29:37.000000 VLCDA-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2043 2024-04-10 22:30:03.122551 VLCDA-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-11-28 23:29:37.000000 VLCDA-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 22:30:03.077529 VLCDA-1.0.8/VLCDA/
--rw-rw-rw-   0        0        0    32053 2024-04-10 22:28:39.000000 VLCDA-1.0.8/VLCDA/Logic_Circuits_Evolution.py
--rw-rw-rw-   0        0        0        0 2023-11-28 23:29:37.000000 VLCDA-1.0.8/VLCDA/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:30:03.095691 VLCDA-1.0.8/VLCDA.egg-info/
--rw-rw-rw-   0        0        0     2043 2024-04-10 22:30:02.000000 VLCDA-1.0.8/VLCDA.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2024-04-10 22:30:02.000000 VLCDA-1.0.8/VLCDA.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:30:02.000000 VLCDA-1.0.8/VLCDA.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-10 22:30:02.000000 VLCDA-1.0.8/VLCDA.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-10 22:30:03.120544 VLCDA-1.0.8/dist/
--rw-rw-rw-   0        0        0     7475 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.0-py3-none-any.whl
--rw-rw-rw-   0        0        0     7746 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.0.tar.gz
--rw-rw-rw-   0        0        0     7472 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.1-py3-none-any.whl
--rw-rw-rw-   0        0        0     7531 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.1.tar.gz
--rw-rw-rw-   0        0        0     8172 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.2-py3-none-any.whl
--rw-rw-rw-   0        0        0     8301 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.2.tar.gz
--rw-rw-rw-   0        0        0     8181 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.3-py3-none-any.whl
--rw-rw-rw-   0        0        0    50423 2023-11-28 23:29:37.000000 VLCDA-1.0.8/dist/VLCDA-1.0.3.tar.gz
--rw-rw-rw-   0        0        0       42 2024-04-10 22:30:03.124534 VLCDA-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      884 2024-04-10 22:26:38.000000 VLCDA-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 04:31:21.094808 VLCDA-1.0.9/
+-rw-rw-rw-   0        0        0     1077 2023-11-28 23:29:37.000000 VLCDA-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5257 2024-04-11 04:31:21.093808 VLCDA-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4620 2024-04-11 04:31:09.000000 VLCDA-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 04:31:20.987803 VLCDA-1.0.9/VLCDA/
+-rw-rw-rw-   0        0        0    28212 2024-04-11 04:31:08.000000 VLCDA-1.0.9/VLCDA/Logic_Circuits_Evolution.py
+-rw-rw-rw-   0        0        0     3312 2024-04-11 04:24:13.000000 VLCDA-1.0.9/VLCDA/PGs_Collection.py
+-rw-rw-rw-   0        0        0        0 2023-11-28 23:29:37.000000 VLCDA-1.0.9/VLCDA/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 04:31:21.013979 VLCDA-1.0.9/VLCDA.egg-info/
+-rw-rw-rw-   0        0        0     5257 2024-04-11 04:31:20.000000 VLCDA-1.0.9/VLCDA.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2024-04-11 04:31:20.000000 VLCDA-1.0.9/VLCDA.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 04:31:20.000000 VLCDA-1.0.9/VLCDA.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-11 04:31:20.000000 VLCDA-1.0.9/VLCDA.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 04:31:21.090808 VLCDA-1.0.9/dist/
+-rw-rw-rw-   0        0        0     7475 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.0-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7746 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.0.tar.gz
+-rw-rw-rw-   0        0        0     7472 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0     7531 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.1.tar.gz
+-rw-rw-rw-   0        0        0     8172 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.2-py3-none-any.whl
+-rw-rw-rw-   0        0        0     8301 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     8181 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.3-py3-none-any.whl
+-rw-rw-rw-   0        0        0    50423 2023-11-28 23:29:37.000000 VLCDA-1.0.9/dist/VLCDA-1.0.3.tar.gz
+-rw-rw-rw-   0        0        0       42 2024-04-11 04:31:21.094808 VLCDA-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      884 2024-04-11 04:31:06.000000 VLCDA-1.0.9/setup.py
```

### Comparing `VLCDA-1.0.8/LICENSE.txt` & `VLCDA-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/VLCDA/Logic_Circuits_Evolution.py` & `VLCDA-1.0.9/VLCDA/Logic_Circuits_Evolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,52 +3,14 @@
 import datetime
 import bisect
 import matplotlib.pyplot as plt
 import numpy as np
 from multiprocessing.sharedctypes import copy
 from quopri import decodestring
 
-PG_collection = {}
-
-x = "2-3 2-0 0-0 2-5 5-1 8-6 1-3 9-1 4-2 11-10 4-11 5-0 4-14 10-8 3-9 15-7 14-14 13-17 8-3 11-3 11-0 21-13 3-1 26-25 5-5 25-8 6-13 0-4 8-10 32-16 23-16 15-17 23-26 34-26 19-26 7-37 30-24 23-5 16-12 22-37 31-15 29-27 27-34 26-43 43-9 23-34 3-16 47-0 27-3 5-52 44-45 19-47 16-32 41-14 9-54 39-38 31-44 23-10 50-42 59-55"
-lx = x.split(" ")
-PG_collection["PG1"] = lx
-
-x = "1-2 4-2 1-5 0-0 7-6 8-8 5-6 8-3 3-7 4-10 3-11 2-6 7-9 0-11 6-1 4-10 13-19 18-11 10-10 6-21 17-17 7-13 12-17 6-20 10-0 20-8 19-3 26-20 5-0 9-21 14-8 29-26 22-28 34-18 30-31 6-7 17-35 40-13 14-39 30-28 38-11 40-3 16-29 36-28 40-2 42-17 12-43 15-8 22-9 23-9 49-6 0-44 3-47 13-35 38-26 58-20 42-47 34-29 11-10 59-41"
-lx = x.split(" ")
-PG_collection["PG2"] = lx
-
-x = "2-0 2-3 3-5 5-6 1-0 2-5 6-9 2-10 0-8 8-9 1-8 14-12 5-10 5-6 2-12 17-9 13-16 6-15 17-7 22-7 16-20 11-18 22-7 11-12 13-3 18-13 24-15 5-28 21-16 7-8 6-14 10-5 0-18 21-32 11-11 3-28 8-2 2-11 11-5 16-5 29-39 13-6 29-22 4-37 29-11 4-48 24-44 10-2 51-35 32-30 8-46 22-0 53-23 42-35 31-1 4-32 42-39 5-11 48-38 53-26"
-lx = x.split(" ")
-PG_collection["PG3"] = lx
-
-x = "2-0 2-0 3-3 1-6 7-1 2-5 3-8 5-9 8-1 6-10 1-6 12-10 1-7 10-5 3-14 4-7 0-5 16-19 11-17 20-3 3-23 8-16 0-9 25-12 8-6 9-20 15-29 24-18 27-18 4-27 29-29 15-30 11-34 12-33 36-14 27-25 23-33 25-25 2-39 30-29 6-19 12-10 23-19 29-39 14-20 13-32 15-28 2-9 12-14 43-17 41-47 36-42 22-29 28-26 40-2 57-2 3-10 5-60 22-14 43-35"
-lx = x.split(" ")
-PG_collection["PG4"] = lx
-
-x = "1-3 3-1 1-5 3-3 1-2 2-6 2-4 2-2 6-8 1-10 11-5 5-3 0-11 15-15 7-6 1-6 8-1 2-15 18-5 1-3 6-15 13-7 15-22 11-21 24-27 25-21 2-15 0-22 26-0 25-4 22-31 4-29 24-30 34-32 23-2 0-3 23-10 28-8 41-28 39-5 17-29 4-11 28-37 32-7 13-20 44-43 39-46 50-32 42-41 44-13 3-5 7-11 10-20 56-51 19-0 39-53 2-37 1-28 11-46 60-62"
-lx = x.split(" ")
-PG_collection["PG5"] = lx
-
-x = "3-0 0-1 5-1 4-6 5-0 4-2 6-7 5-3 7-2 11-8 5-10 3-9 6-3 3-0 17-3 7-12 12-7 6-9 11-3 18-8 2-12 24-20 17-22 9-23 25-23 13-25 13-0 10-16 21-29 29-25 21-28 20-8 15-30 29-2 20-15 30-11 30-31 38-4 34-41 1-34 38-25 13-1 45-19 23-20 27-25 7-4 6-15 29-37 34-11 1-19 43-37 29-13 35-5 5-36 35-30 53-15 59-48 13-44 37-20 55-33"
-lx = x.split(" ")
-PG_collection["PG6"] = lx
-
-x = "2-0 4-4 0-3 6-0 6-3 8-7 2-9 10-9 1-1 12-10 4-5 6-12 3-8 2-10 14-15 8-14 11-17 12-12 1-4 15-20 23-4 2-16 7-17 23-21 16-23 6-28 9-26 3-10 27-25 32-32 22-31 34-18 33-5 1-10 27-26 12-20 2-8 2-29 10-40 39-0 17-4 23-19 14-19 0-24 11-4 6-48 43-4 12-47 47-7 17-9 27-39 30-5 10-39 47-33 9-11 52-2 53-3 5-21 48-30 39-27"
-lx = x.split(" ")
-PG_collection["PG7"] = lx
-
-x = "2-2 0-3 5-0 4-6 1-2 1-4 3-5 10-6 3-4 2-4 12-2 12-4 2-8 9-16 10-17 18-2 13-17 1-20 19-17 13-1 2-23 1-0 17-0 22-22 11-27 7-27 13-18 9-4 7-7 30-22 26-32 25-27 31-12 21-6 31-2 15-21 1-28 4-10 11-20 6-30 39-27 5-12 1-11 16-13 18-6 43-23 27-24 20-46 32-2 47-6 37-45 44-10 5-43 41-44 56-13 26-1 8-29 44-54 55-34 42-43"
-lx = x.split(" ")
-PG_collection["PG8"] = lx
-
-x = "0-1 1-4 3-1 6-3 0-0 4-0 1-1 9-5 4-8 3-11 10-6 7-5 8-9 2-5 1-4 13-3 13-12 18-1 11-13 0-10 22-19 15-16 3-23 2-24 22-14 22-21 14-29 29-6 27-2 8-16 33-6 28-6 23-3 5-21 7-37 30-30 39-5 9-39 30-10 27-2 15-32 44-11 22-41 33-31 6-31 24-29 14-25 29-6 35-10 23-41 9-36 12-29 27-24 47-16 8-42 47-24 16-16 2-41 29-58 56-32"
-lx = x.split(" ")
-PG_collection["PG9"] = lx
-
 class Genoma:
     def __init__(self, numberOfGenes = 60, nInputs = 4,nOutputs = 1, rateMutation = 0.10):
         self.genotipo = []
         self.copyGenotipo = []
         self.numberOfGenes = numberOfGenes
         self.faultChance = 0
         self.nInputs = nInputs
@@ -169,36 +131,43 @@
         count = 0
         n = len(l)
         if(l[n] + l[n-1] == 1):
           return 1
         else :
           return 0
 
-    def gpiNand(self, l):
+    def gpiNand(self, l, nOutputs=1):
         count = 0
         n = len(l)
         for i in range(0,n):
           if(l[i] == 1):
             count+=1
 
         if(count%2 == 0):
             return "0"
         else: 
             return "1"
 
-    def fullAdderNand(self,l):
-      middle = int(len(l)/2)
-
-      input1 = [str(x) for x in l[0:middle]]
+    def fullAdderNand(self, l, nOutputs):
+    # Preparing
+      middle = int(len(l)/2) + 1
+      input1 = [str(x) for x in l[1:middle]]
       input2 = [str(x) for x in l[middle:]]
+      cIn = [str(l[0])]
       input1s = ''.join(input1) 
       input2s = ''.join(input2)
-      sum_bits = bin(int(input1s, 2) + int(input2s, 2) + int(str(l[0]),2))[2:]
-      sum_bits_string = sum_bits.zfill(self.nOutputs)
-
+      cIns = ''.join(cIn)
+      #print(input1s, input2s, cIns)
+      # Logical Expressions
+      sum = bin(int(input1s, 2) ^ int(input2s, 2) ^ int(cIns, 2))[2:]
+      cOut = bin((int(input1s, 2) & int(input2s, 2)) | (int(input2s, 2) & int(cIns, 2)) | (int(input1s, 2) & int(cIns, 2)))[2:]
+      sum_bits =str(sum) + str(cOut) 
+      sum_bits_string = sum_bits.zfill(nOutputs)
+      #print(sum_bits_string)
+      # Returning
       return sum_bits_string
 
     def NAND(self,a,b):  ### NAND 1 1 1 0
         output = 1
         if a == 1 and b == 1:
             output = 0
         return output
@@ -694,39 +663,8 @@
                     bestParent.calculateFitness(logicFunction)
                     bestParent.calculateNoiseFitness()
                     print("Recalculating fitness without faults...")
                     self.display(bestParent.genotipo,bestParent.fitness,bestParent.noiseFitness,self.totalGeneration)
 
                     break
         timeDiff = datetime.datetime.now() - self.startTime
-        print("The end in: ",str(timeDiff))
-
-def gpinand(l,nOutputs = 1):
-  count = 0
-  n = len(l)
-  for i in range(0,n):
-    if(l[i] == 1):
-      count+=1
-
-  if(count%2 == 0):
-      return "0"
-  else: 
-      return "1"
-
-def fullAdderNand(l, nOutputs):
-    # Preparing
-    middle = int(len(l)/2) + 1
-    input1 = [str(x) for x in l[1:middle]]
-    input2 = [str(x) for x in l[middle:]]
-    cIn = [str(l[0])]
-    input1s = ''.join(input1) 
-    input2s = ''.join(input2)
-    cIns = ''.join(cIn)
-    #print(input1s, input2s, cIns)
-    # Logical Expressions
-    sum = bin(int(input1s, 2) ^ int(input2s, 2) ^ int(cIns, 2))[2:]
-    cOut = bin((int(input1s, 2) & int(input2s, 2)) | (int(input2s, 2) & int(cIns, 2)) | (int(input1s, 2) & int(cIns, 2)))[2:]
-    sum_bits =str(sum) + str(cOut) 
-    sum_bits_string = sum_bits.zfill(nOutputs)
-    #print(sum_bits_string)
-    # Returning
-    return sum_bits_string
+        print("The end in: ",str(timeDiff))
```

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.0-py3-none-any.whl` & `VLCDA-1.0.9/dist/VLCDA-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.0.tar.gz` & `VLCDA-1.0.9/dist/VLCDA-1.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.1-py3-none-any.whl` & `VLCDA-1.0.9/dist/VLCDA-1.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.1.tar.gz` & `VLCDA-1.0.9/dist/VLCDA-1.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.2-py3-none-any.whl` & `VLCDA-1.0.9/dist/VLCDA-1.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.2.tar.gz` & `VLCDA-1.0.9/dist/VLCDA-1.0.2.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.3-py3-none-any.whl` & `VLCDA-1.0.9/dist/VLCDA-1.0.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/dist/VLCDA-1.0.3.tar.gz` & `VLCDA-1.0.9/dist/VLCDA-1.0.3.tar.gz`

 * *Files identical despite different names*

### Comparing `VLCDA-1.0.8/setup.py` & `VLCDA-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as rm:
     long_description = rm.read()
 
 setup(
     name = "VLCDA",
-    version = "1.0.8",
+    version = "1.0.9",
     license='MIT',
     description = "Modulo Python dedicado a evolução de circuitos lógicos através de algoritmos genéticos",
     author = "Humberto Távora, Stefan Blawid, Yasmin Maria",
     author_email = 'humbertocctg@gmail.com',
     long_description=long_description,
     long_description_content_type = "text/markdown",
     url = 'https://github.com/HumbertoTavora/Logic-Circuits-Evolution',
```

