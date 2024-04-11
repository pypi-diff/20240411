# Comparing `tmp/dump_github-0.1.1-py3-none-any.whl.zip` & `tmp/dump_github-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4480 bytes, number of entries: 10
+Zip file size: 4481 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       43 b- defN 24-Apr-10 18:26 dump_github/__init__.py
 -rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/lib.py
--rw-rw-r--  2.0 unx     1486 b- defN 24-Apr-10 18:32 dump_github/main.py
+-rw-rw-r--  2.0 unx     1490 b- defN 24-Apr-10 19:17 dump_github/main.py
 -rw-rw-r--  2.0 unx      715 b- defN 24-Apr-10 17:24 dump_github/mylib.py
--rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       12 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      809 b- defN 24-Apr-10 19:03 dump_github-0.1.1.dist-info/RECORD
-10 files, 6148 bytes uncompressed, 3092 bytes compressed:  49.7%
+-rw-rw-r--  2.0 unx     1064 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       12 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      809 b- defN 24-Apr-10 19:18 dump_github-0.1.2.dist-info/RECORD
+10 files, 6152 bytes uncompressed, 3093 bytes compressed:  49.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: dump_github/main.py
 Comment: 
 
 Filename: dump_github/mylib.py
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/LICENSE
+Filename: dump_github-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/METADATA
+Filename: dump_github-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/WHEEL
+Filename: dump_github-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/entry_points.txt
+Filename: dump_github-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/top_level.txt
+Filename: dump_github-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: dump_github-0.1.1.dist-info/RECORD
+Filename: dump_github-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dump_github/main.py

```diff
@@ -40,14 +40,14 @@
 def main():
     # print(args)
     repos = serach_user_repos(args.username, args.token)
     for repo in repos:
         if args.print == True:
             print(repo["clone_url"])
         elif args.download_zip == True:
-            download_zip(user_name, repo["name"])
+            download_zip(args.username, repo["name"])
         else:
             clone_repo(repo)
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `dump_github-0.1.1.dist-info/LICENSE` & `dump_github-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dump_github-0.1.1.dist-info/METADATA` & `dump_github-0.1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dump-github
-Version: 0.1.1
+Version: 0.1.2
 Summary: This tool can be used to back up users' GitHub repositories in case they need them later.
 Home-page: https://github.com/core2002/dump_github
 Author: core2002
 Author-email: core2002@aliyun.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `dump_github-0.1.1.dist-info/RECORD` & `dump_github-0.1.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dump_github/__init__.py,sha256=3XLRrchVn7g3TYWiQpv3u2lKdTO-jDqg4_0-lpmRuRs,43
 dump_github/lib.py,sha256=pHONzAjGbXkmAUvCGn8HkHWS7fyY2qu9R17to6jD1TU,715
-dump_github/main.py,sha256=tZ3yPdcljCobzIGk2_Exwnb2ao-1JPAflwTVe--BnZg,1486
+dump_github/main.py,sha256=OJE08ZVbv1-TZvSUvmz6smjYYWoqSiDhE1XYyKynHBQ,1490
 dump_github/mylib.py,sha256=pHONzAjGbXkmAUvCGn8HkHWS7fyY2qu9R17to6jD1TU,715
-dump_github-0.1.1.dist-info/LICENSE,sha256=5tQa-lQLqvLhjTuELEk4bm70I5hcdjUeOn4qf3MK84E,1064
-dump_github-0.1.1.dist-info/METADATA,sha256=PMjLrIl4bxKIH5eedQ2IiUX9P54u58rym8a3hsvPjA0,1162
-dump_github-0.1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dump_github-0.1.1.dist-info/entry_points.txt,sha256=bHSMsd4MLHu5N-1Vomjq7P_VLmFWN5VabwMVyJEJurA,50
-dump_github-0.1.1.dist-info/top_level.txt,sha256=6oWfdkP2U1AN9zL6AUIUTxe6hYIeo_Nf8M8SWBxElUw,12
-dump_github-0.1.1.dist-info/RECORD,,
+dump_github-0.1.2.dist-info/LICENSE,sha256=5tQa-lQLqvLhjTuELEk4bm70I5hcdjUeOn4qf3MK84E,1064
+dump_github-0.1.2.dist-info/METADATA,sha256=rtzv-7udXjyD7EOPqhWPt7sSlVh1E7FArBd82gfKaK0,1162
+dump_github-0.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dump_github-0.1.2.dist-info/entry_points.txt,sha256=bHSMsd4MLHu5N-1Vomjq7P_VLmFWN5VabwMVyJEJurA,50
+dump_github-0.1.2.dist-info/top_level.txt,sha256=6oWfdkP2U1AN9zL6AUIUTxe6hYIeo_Nf8M8SWBxElUw,12
+dump_github-0.1.2.dist-info/RECORD,,
```

