# Comparing `tmp/bohr-0.2.3.tar.gz` & `tmp/bohr-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bohr-0.2.3.tar", last modified: Wed Nov 29 10:42:59 2023, max compression
+gzip compressed data, was "bohr-0.2.4.tar", last modified: Thu Apr 11 13:10:52 2024, max compression
```

## Comparing `bohr-0.2.3.tar` & `bohr-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-11-29 10:42:59.618121 bohr-0.2.3/
--rw-rw-rw-   0        0        0      107 2023-11-29 10:42:59.616119 bohr-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-11-22 08:39:01.000000 bohr-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-11-29 10:42:59.579271 bohr-0.2.3/bohr/
--rw-rw-rw-   0        0        0      129 2023-11-29 10:42:37.000000 bohr-0.2.3/bohr/__init__.py
--rw-rw-rw-   0        0        0     2619 2023-09-21 15:23:25.000000 bohr-0.2.3/bohr/database.py
--rw-rw-rw-   0        0        0     2822 2023-11-29 10:42:15.000000 bohr-0.2.3/bohr/forecast.py
--rw-rw-rw-   0        0        0     4077 2023-11-29 10:40:07.000000 bohr-0.2.3/bohr/mdm.py
--rw-rw-rw-   0        0        0     2832 2023-11-29 10:41:21.000000 bohr-0.2.3/bohr/ms.py
--rw-rw-rw-   0        0        0      229 2023-10-31 14:28:53.000000 bohr-0.2.3/bohr/test.py
-drwxrwxrwx   0        0        0        0 2023-11-29 10:42:59.614155 bohr-0.2.3/bohr.egg-info/
--rw-rw-rw-   0        0        0      107 2023-11-29 10:42:59.000000 bohr-0.2.3/bohr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-11-29 10:42:59.000000 bohr-0.2.3/bohr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-29 10:42:59.000000 bohr-0.2.3/bohr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-11-29 10:42:59.000000 bohr-0.2.3/bohr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-11-29 10:42:59.000000 bohr-0.2.3/bohr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-29 10:42:59.618121 bohr-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-11-29 10:42:44.000000 bohr-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:10:52.722223 bohr-0.2.4/
+-rw-rw-rw-   0        0        0      107 2024-04-11 13:10:52.720225 bohr-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-11-22 08:39:01.000000 bohr-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 13:10:52.659225 bohr-0.2.4/bohr/
+-rw-rw-rw-   0        0        0      129 2023-11-29 10:42:37.000000 bohr-0.2.4/bohr/__init__.py
+-rw-rw-rw-   0        0        0     3004 2024-04-11 13:10:24.000000 bohr-0.2.4/bohr/database.py
+-rw-rw-rw-   0        0        0     2822 2023-11-29 10:42:15.000000 bohr-0.2.4/bohr/forecast.py
+-rw-rw-rw-   0        0        0     4077 2023-11-29 10:40:07.000000 bohr-0.2.4/bohr/mdm.py
+-rw-rw-rw-   0        0        0     2832 2023-11-29 10:41:21.000000 bohr-0.2.4/bohr/ms.py
+-rw-rw-rw-   0        0        0      229 2023-10-31 14:28:53.000000 bohr-0.2.4/bohr/test.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:10:52.717227 bohr-0.2.4/bohr.egg-info/
+-rw-rw-rw-   0        0        0      107 2024-04-11 13:10:52.000000 bohr-0.2.4/bohr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-04-11 13:10:52.000000 bohr-0.2.4/bohr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:10:52.000000 bohr-0.2.4/bohr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-11 13:10:52.000000 bohr-0.2.4/bohr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 13:10:52.000000 bohr-0.2.4/bohr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:10:52.723226 bohr-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      293 2024-04-11 13:10:35.000000 bohr-0.2.4/setup.py
```

### Comparing `bohr-0.2.3/bohr/database.py` & `bohr-0.2.4/bohr/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,20 +57,26 @@
         except Exception as e:
             print(f"SQL execution error: {e}")
         finally:
             conn.close()
 
 
 
-    def insert(self,table, df,onConflict=''):
-        if self.multiple :
-            for db in ['research','trading'] : 
-                self.batch_insert(db,table, df,onConflict)
-        else :
-            self.batch_insert(self.database,table, df,onConflict)
+    def insert(self, table, df, onConflict=''):
+        if self.multiple:
+            if "research_dev" in self.database or 'trading_dev' in self.database:
+                for db in ['research_dev', 'trading_dev']:
+                    self.batch_insert(db, table, df, onConflict)
+            elif self.database=="research" or self.database=='trading':
+                for db in ['research', 'trading']:
+                    self.batch_insert(db, table, df, onConflict)
+            else:
+                self.batch_insert(self.database, table, df, onConflict)
+        else:
+            self.batch_insert(self.database, table, df, onConflict)
 
 
     def batch_insert(self,db,table, df,onConflict=''):
         try:
             conn, cur = self.connect(db)
             if conn is None or cur is None:
                 return
```

### Comparing `bohr-0.2.3/bohr/forecast.py` & `bohr-0.2.4/bohr/forecast.py`

 * *Files identical despite different names*

### Comparing `bohr-0.2.3/bohr/mdm.py` & `bohr-0.2.4/bohr/mdm.py`

 * *Files identical despite different names*

### Comparing `bohr-0.2.3/bohr/ms.py` & `bohr-0.2.4/bohr/ms.py`

 * *Files identical despite different names*

