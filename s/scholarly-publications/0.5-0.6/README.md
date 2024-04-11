# Comparing `tmp/scholarly_publications-0.5.tar.gz` & `tmp/scholarly_publications-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scholarly_publications-0.5.tar", last modified: Wed Apr  3 22:27:48 2024, max compression
+gzip compressed data, was "scholarly_publications-0.6.tar", last modified: Thu Apr 11 09:43:33 2024, max compression
```

## Comparing `scholarly_publications-0.5.tar` & `scholarly_publications-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.019787 scholarly_publications-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 22:27:43.000000 scholarly_publications-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:27:48.015787 scholarly_publications-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-03 22:27:43.000000 scholarly_publications-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/scholarly_publications/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 22:27:43.000000 scholarly_publications-0.5/scholarly_publications/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/scholarly_publications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 22:27:48.000000 scholarly_publications-0.5/scholarly_publications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:27:48.019787 scholarly_publications-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 22:27:43.000000 scholarly_publications-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:27:48.015787 scholarly_publications-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 22:27:43.000000 scholarly_publications-0.5/tests/test_scholarly_publications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:43:33.767057 scholarly_publications-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 09:43:26.000000 scholarly_publications-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-11 09:43:33.767057 scholarly_publications-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-11 09:43:26.000000 scholarly_publications-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:43:33.767057 scholarly_publications-0.6/scholarly_publications/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 09:43:26.000000 scholarly_publications-0.6/scholarly_publications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-11 09:43:26.000000 scholarly_publications-0.6/scholarly_publications/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-11 09:43:26.000000 scholarly_publications-0.6/scholarly_publications/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:43:33.767057 scholarly_publications-0.6/scholarly_publications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 09:43:33.000000 scholarly_publications-0.6/scholarly_publications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 09:43:33.767057 scholarly_publications-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-11 09:43:26.000000 scholarly_publications-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 09:43:33.767057 scholarly_publications-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-11 09:43:26.000000 scholarly_publications-0.6/tests/test_scholarly_publications.py
```

### Comparing `scholarly_publications-0.5/LICENSE` & `scholarly_publications-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scholarly_publications-0.5/PKG-INFO` & `scholarly_publications-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scholarly_publications
-Version: 0.5
+Version: 0.6
 Summary: A tool to fetch scholarly publications from Google Scholar by author ID
 Home-page: https://github.com/ezefranca/scholarly_publications
 Author: Ezequiel França
 Author-email: ezequiel.franca@gmail.com
 Project-URL: Bug Reports, https://github.com/ezefranca/scholarly_publications/issues
 Project-URL: Source, https://github.com/ezefranca/scholarly_publications
 Keywords: scholarly publications google scholar fetcher academia
@@ -49,26 +49,34 @@
 ```
 
 Fetch a specific number of publications for a given author ID:
 ```bash
 scholarly_publications <author_id> --max=<number_of_publications>
 ```
 
+Sort results by pubdate/cited:
+```bash
+scholarly_publications <author_id> --sortby=<pubdate/cited>
+```
+
 ### Using as a Python Package
 
 You can also use `scholarly_publications` directly in your Python code. Here's how:
 
 ```python
-from scholarly_publications import fetch_all_publications
+from scholarly_publications import fetch_publications
 
 # Fetch all publications for a given author ID
-publications = fetch_all_publications('<author_id>')
+publications = fetch_publications('<author_id>')
 
 # Fetch a specific number of publications for a given author ID
-publications = fetch_all_publications('<author_id>', max_publications=<number_of_publications>)
+publications = fetch_publications('<author_id>', max_publications=<number_of_publications>)
+
+# Fetch all publications for a given author ID and sort by pubdate/cited
+publications = fetch_publications('<author_id>', sortby='<pubdate/cited>')
 
 print(publications)
 ```
 
 ## Contributing
 
 We welcome contributions to `scholarly_publications`! If you have suggestions for improvements, please open an issue or a pull request.
```

### Comparing `scholarly_publications-0.5/README.md` & `scholarly_publications-0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,34 @@
 ```
 
 Fetch a specific number of publications for a given author ID:
 ```bash
 scholarly_publications <author_id> --max=<number_of_publications>
 ```
 
+Sort results by pubdate/cited:
+```bash
+scholarly_publications <author_id> --sortby=<pubdate/cited>
+```
+
 ### Using as a Python Package
 
 You can also use `scholarly_publications` directly in your Python code. Here's how:
 
 ```python
-from scholarly_publications import fetch_all_publications
+from scholarly_publications import fetch_publications
 
 # Fetch all publications for a given author ID
-publications = fetch_all_publications('<author_id>')
+publications = fetch_publications('<author_id>')
 
 # Fetch a specific number of publications for a given author ID
-publications = fetch_all_publications('<author_id>', max_publications=<number_of_publications>)
+publications = fetch_publications('<author_id>', max_publications=<number_of_publications>)
+
+# Fetch all publications for a given author ID and sort by pubdate/cited
+publications = fetch_publications('<author_id>', sortby='<pubdate/cited>')
 
 print(publications)
 ```
 
 ## Contributing
 
 We welcome contributions to `scholarly_publications`! If you have suggestions for improvements, please open an issue or a pull request.
```

### Comparing `scholarly_publications-0.5/scholarly_publications/cli.py` & `scholarly_publications-0.6/scholarly_publications/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from .fetcher import fetch_all_publications
 import json
 
 def main():
     parser = argparse.ArgumentParser(description="Fetch publications from Google Scholar.")
     parser.add_argument("author_id", help="Google Scholar author ID")
     parser.add_argument("--max", type=int, default=None, help="Maximum number of publications to fetch")
+    parser.add_argument("--sortby", type=str, default=None, help="How to sort publications (cited/pubdate)")
     args = parser.parse_args()
 
-    publications = fetch_all_publications(args.author_id, args.max)
+    publications = fetch_all_publications(args.author_id, args.max, args.sortby)
     print(json.dumps(publications, indent=4))
     print()
 
 if __name__ == "__main__":
     main()
```

### Comparing `scholarly_publications-0.5/scholarly_publications/fetcher.py` & `scholarly_publications-0.6/scholarly_publications/fetcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,30 @@
     'user-agent': 'Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/116.0.0.0 Mobile Safari/537.36',
 }
 
 COOKIES = {
     'CONSENT': 'PENDING+300',
 }
 
-def fetch_all_publications(author_id, max_publications=None):
+def fetch_all_publications(author_id, max_publications=None, sortby='cited'):
     all_publications = []
     start_index = 0
     page_size = 100
     total_fetched = 0
 
     while True:
         if max_publications is not None and total_fetched >= max_publications:
             break
 
         params = {
             'user': author_id,
             'oi': 'ao',
             'cstart': start_index,
             'pagesize': page_size,
+            'sortby': sortby
         }
 
         response = requests.get('https://scholar.google.com/citations', params=params, cookies=COOKIES, headers=HEADERS)
 
         if response.status_code == 200:
             soup = BeautifulSoup(response.text, 'html.parser')
             publications = parse_publications(soup)
```

### Comparing `scholarly_publications-0.5/scholarly_publications.egg-info/PKG-INFO` & `scholarly_publications-0.6/scholarly_publications.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scholarly_publications
-Version: 0.5
+Version: 0.6
 Summary: A tool to fetch scholarly publications from Google Scholar by author ID
 Home-page: https://github.com/ezefranca/scholarly_publications
 Author: Ezequiel França
 Author-email: ezequiel.franca@gmail.com
 Project-URL: Bug Reports, https://github.com/ezefranca/scholarly_publications/issues
 Project-URL: Source, https://github.com/ezefranca/scholarly_publications
 Keywords: scholarly publications google scholar fetcher academia
@@ -49,26 +49,34 @@
 ```
 
 Fetch a specific number of publications for a given author ID:
 ```bash
 scholarly_publications <author_id> --max=<number_of_publications>
 ```
 
+Sort results by pubdate/cited:
+```bash
+scholarly_publications <author_id> --sortby=<pubdate/cited>
+```
+
 ### Using as a Python Package
 
 You can also use `scholarly_publications` directly in your Python code. Here's how:
 
 ```python
-from scholarly_publications import fetch_all_publications
+from scholarly_publications import fetch_publications
 
 # Fetch all publications for a given author ID
-publications = fetch_all_publications('<author_id>')
+publications = fetch_publications('<author_id>')
 
 # Fetch a specific number of publications for a given author ID
-publications = fetch_all_publications('<author_id>', max_publications=<number_of_publications>)
+publications = fetch_publications('<author_id>', max_publications=<number_of_publications>)
+
+# Fetch all publications for a given author ID and sort by pubdate/cited
+publications = fetch_publications('<author_id>', sortby='<pubdate/cited>')
 
 print(publications)
 ```
 
 ## Contributing
 
 We welcome contributions to `scholarly_publications`! If you have suggestions for improvements, please open an issue or a pull request.
```

### Comparing `scholarly_publications-0.5/setup.py` & `scholarly_publications-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from io import open
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-version = '0.5'
+version = '0.6'
 
 setup(
     name='scholarly_publications',
     version=version,
     description='A tool to fetch scholarly publications from Google Scholar by author ID',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `scholarly_publications-0.5/tests/test_scholarly_publications.py` & `scholarly_publications-0.6/tests/test_scholarly_publications.py`

 * *Files identical despite different names*

