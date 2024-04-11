# Comparing `tmp/peegee-0.2.2-py3-none-any.whl.zip` & `tmp/peegee-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5702 bytes, number of entries: 6
--rw-r--r--  2.0 unx    19881 b- defN 22-Jun-07 03:49 peegee.py
--rw-rw-rw-  2.0 unx     1064 b- defN 22-Jun-07 03:49 peegee-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx      950 b- defN 22-Jun-07 03:49 peegee-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jun-07 03:49 peegee-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 22-Jun-07 03:49 peegee-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      446 b- defN 22-Jun-07 03:49 peegee-0.2.2.dist-info/RECORD
-6 files, 22440 bytes uncompressed, 4898 bytes compressed:  78.2%
+Zip file size: 5783 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    20216 b- defN 24-Apr-11 09:02 peegee.py
+-rw-rw-rw-  2.0 unx     1064 b- defN 24-Apr-11 09:02 peegee-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      957 b- defN 24-Apr-11 09:02 peegee-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 09:02 peegee-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-11 09:02 peegee-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      446 b- defN 24-Apr-11 09:02 peegee-0.2.3.dist-info/RECORD
+6 files, 22782 bytes uncompressed, 4979 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: peegee.py
 Comment: 
 
-Filename: peegee-0.2.2.dist-info/LICENSE
+Filename: peegee-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: peegee-0.2.2.dist-info/METADATA
+Filename: peegee-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: peegee-0.2.2.dist-info/WHEEL
+Filename: peegee-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: peegee-0.2.2.dist-info/top_level.txt
+Filename: peegee-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: peegee-0.2.2.dist-info/RECORD
+Filename: peegee-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## peegee.py

```diff
@@ -254,18 +254,26 @@
                     ),
                 pk=psysql.Identifier(primary_key_name)
                 )
             )
         if commit:
             self.commit()
 
-    def createUser(self, user, commit=True):
+    def createUser(self, user, password=None, commit=True):
         if not self.isUserExists(user):
-            self.execute(psysql.SQL(
-                'CREATE ROLE {un} LOGIN').format(un=psysql.Identifier(user)))
+            if password:
+                self.execute(psysql.SQL(
+                    'CREATE USER {un} WITH ENCRYPTED PASSWORD {pw}').format(
+                        un=psysql.Identifier(user),
+                        pw=psysql.Literal(password),
+                    ))
+            else:
+                self.execute(psysql.SQL(
+                    'CREATE USER {un}').format(un=psysql.Identifier(user)
+                    ))
             if commit:
                 self.commit()
         else:
             print('The user "{un}" already exists, '\
                   'creation is skipped.'.format(un=user))
 
     def dropTable(self, table, schema=None, commit=True):
```

## Comparing `peegee-0.2.2.dist-info/LICENSE` & `peegee-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `peegee-0.2.2.dist-info/METADATA` & `peegee-0.2.3.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peegee
-Version: 0.2.2
+Version: 0.2.3
 Summary: A PostgreSQL client based on psycopg2
 Home-page: https://gitlab.com/scku208/peegee
 Author: scku
 Author-email: scku208@gmail.com
 License: MIT
 Download-URL: https://gitlab.com/scku208/peegee/-/archive/master/peegee-master.zip
 Keywords: postgresql,psycopg2,database,peegee
@@ -17,11 +17,11 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-Requires-Dist: psycopg2
+Requires-Dist: psycopg2-binary
 
 UNKNOWN
```

