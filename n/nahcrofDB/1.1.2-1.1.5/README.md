# Comparing `tmp/nahcrofDB-1.1.2.tar.gz` & `tmp/nahcrofDB-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nahcrofDB-1.1.2.tar", last modified: Tue Mar 19 03:51:20 2024, max compression
+gzip compressed data, was "nahcrofDB-1.1.5.tar", last modified: Thu Apr 11 02:49:10 2024, max compression
```

## Comparing `nahcrofDB-1.1.2.tar` & `nahcrofDB-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 03:51:20.610000 nahcrofDB-1.1.2/
--rw-rw-rw-   0        0        0      460 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-19 03:51:20.620000 nahcrofDB-1.1.2/nahcrofDB.egg-info/
--rw-rw-rw-   0        0        0      460 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/nahcrofDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/nahcrofDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/nahcrofDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/nahcrofDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/nahcrofDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3220 2024-03-19 03:35:04.000000 nahcrofDB-1.1.2/nahcrofDB.py
--rw-rw-rw-   0        0        0       42 2024-03-19 03:51:22.000000 nahcrofDB-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      601 2024-03-19 03:40:18.000000 nahcrofDB-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 02:49:10.300000 nahcrofDB-1.1.5/
+-rw-rw-rw-   0        0        0      460 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-11 02:49:10.310000 nahcrofDB-1.1.5/nahcrofDB.egg-info/
+-rw-rw-rw-   0        0        0      460 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/nahcrofDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3771 2024-04-11 02:41:50.000000 nahcrofDB-1.1.5/nahcrofDB.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 02:49:12.000000 nahcrofDB-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      601 2024-04-11 02:49:02.000000 nahcrofDB-1.1.5/setup.py
```

### Comparing `nahcrofDB-1.1.2/nahcrofDB.py` & `nahcrofDB-1.1.5/nahcrofDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,27 @@
         templist.append(keydata)
     keynamenum = str(len(keynames)) 
     result = "".join(templist)
     r = requests.get(url=f"https://database.nahcrof.com/getKeys/?location={quote(username[0])}&token={quote(token[0])}&keynamenum={quote(keynamenum)}" + result)
     data = r.json()
     return data
 
+# returns multiple requested keys with a list input value 
+def getKeysList(keynames: list):
+    templist = []
+    for keyname in keynames:
+        listnum = len(templist)
+        keydata = f"&key_{listnum}={quote(keyname)}"
+        templist.append(keydata)
+    keynamenum = str(len(keynames))
+    result = "".join(templist)
+    r = requests.get(url=f"https://database.nahcrof.com/getKeys/?location={quote(username[0])}&token={quote(token[0])}&keynamenum={quote(keynamenum)}" + result)
+    data = r.json()
+    return data
+
 # creates a key in the defined database
 def makeKey(keyname: str, keycontent):
     if token[0] == 0:
         print("token parameter not set")
     elif username[0] == 0:
         print("username/location parameter not set")
     else:
@@ -73,14 +86,15 @@
     else:
         payload = {"location": username[0], "keyname": keyname, "token": token[0]}
         r1 = requests.post('https://database.nahcrof.com/delKey', json=payload)
         return r1
 
 
 # this will reset the defined database to have 0 keys, no backup will be made, DO NOT use this unless you know what you are doing def resetDB():
+def resetDB():
     if token[0] == 0:
         print("token parameter not set")
     elif username[0] == 0:
         print("username/location parameter not set")
     else:
         payload = {"location": username[0], "token": token[0]}
         r1 = requests.post('https://database.nahcrof.com/resetDB', json=payload)
```

### Comparing `nahcrofDB-1.1.2/setup.py` & `nahcrofDB-1.1.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nahcrofDB',
-    version='1.1.2',
+    version='1.1.5',
     py_modules=['nahcrofDB'],
     author='Tyrae Paul',
     author_email='tyraepaul@gmail.com',
     install_requires=["requests"],
     description='nahcrofDB is a simple key-value database solution allowing for fast and easy data storage',
     classifiers=[
         "Programming Language :: Python :: 3",
```

