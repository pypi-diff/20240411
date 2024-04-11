# Comparing `tmp/doh-tools-1.1.tar.gz` & `tmp/doh-tools-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doh-tools-1.1.tar", last modified: Wed Mar 13 16:21:41 2024, max compression
+gzip compressed data, was "doh-tools-1.2.tar", last modified: Thu Apr 11 19:41:59 2024, max compression
```

## Comparing `doh-tools-1.1.tar` & `doh-tools-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 16:21:41.505841 doh-tools-1.1/
--rw-rw-rw-   0        0        0       54 2024-03-13 16:21:41.504847 doh-tools-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      123 2024-01-03 18:28:13.000000 doh-tools-1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-13 16:21:41.478733 doh-tools-1.1/doh_tools/
--rw-rw-rw-   0        0        0       65 2024-01-03 17:36:43.000000 doh-tools-1.1/doh_tools/__init__.py
--rw-rw-rw-   0        0        0     3153 2024-01-03 20:58:42.000000 doh-tools-1.1/doh_tools/custom_logging.py
--rw-rw-rw-   0        0        0     3312 2024-02-05 16:59:05.000000 doh-tools-1.1/doh_tools/google_helpers.py
--rw-rw-rw-   0        0        0     3706 2024-03-13 16:17:23.000000 doh-tools-1.1/doh_tools/idis_processing.py
--rw-rw-rw-   0        0        0     2674 2024-02-05 16:58:44.000000 doh-tools-1.1/doh_tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-13 16:21:41.500823 doh-tools-1.1/doh_tools.egg-info/
--rw-rw-rw-   0        0        0       54 2024-03-13 16:21:41.000000 doh-tools-1.1/doh_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-03-13 16:21:41.000000 doh-tools-1.1/doh_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 16:21:41.000000 doh-tools-1.1/doh_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-03-13 16:21:41.000000 doh-tools-1.1/doh_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-13 16:21:41.506839 doh-tools-1.1/setup.cfg
--rw-rw-rw-   0        0        0      118 2024-03-13 16:20:16.000000 doh-tools-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:41:59.060927 doh-tools-1.2/
+-rw-rw-rw-   0        0        0       54 2024-04-11 19:41:59.059043 doh-tools-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2506 2024-03-13 16:22:31.000000 doh-tools-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 19:41:59.032202 doh-tools-1.2/doh_tools/
+-rw-rw-rw-   0        0        0       65 2024-01-03 17:36:43.000000 doh-tools-1.2/doh_tools/__init__.py
+-rw-rw-rw-   0        0        0     3153 2024-01-03 20:58:42.000000 doh-tools-1.2/doh_tools/custom_logging.py
+-rw-rw-rw-   0        0        0     3312 2024-02-05 16:59:05.000000 doh-tools-1.2/doh_tools/google_helpers.py
+-rw-rw-rw-   0        0        0     4798 2024-04-11 16:57:54.000000 doh-tools-1.2/doh_tools/idis_processing.py
+-rw-rw-rw-   0        0        0     2674 2024-02-05 16:58:44.000000 doh-tools-1.2/doh_tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:41:59.053892 doh-tools-1.2/doh_tools.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-04-11 19:41:58.000000 doh-tools-1.2/doh_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-11 19:41:58.000000 doh-tools-1.2/doh_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 19:41:58.000000 doh-tools-1.2/doh_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 19:41:58.000000 doh-tools-1.2/doh_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 19:41:59.061926 doh-tools-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      118 2024-04-11 19:41:30.000000 doh-tools-1.2/setup.py
```

### Comparing `doh-tools-1.1/doh_tools/custom_logging.py` & `doh-tools-1.2/doh_tools/custom_logging.py`

 * *Files identical despite different names*

### Comparing `doh-tools-1.1/doh_tools/google_helpers.py` & `doh-tools-1.2/doh_tools/google_helpers.py`

 * *Files identical despite different names*

### Comparing `doh-tools-1.1/doh_tools/idis_processing.py` & `doh-tools-1.2/doh_tools/idis_processing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-#%%
 import pandas as pd
 import os
 import zipfile
+import re
 
 def process_idis_fwf(filename):
     '''
     Process the IDIS FWF Export from HUD.
 
-    This function takes a fixed-width IDIS file, and coverts it to a pandas df. 
+    This function takes a fixed-width IDIS file, and converts it to a pandas DataFrame.
 
     Parameters:
         - filename: Path to the fixed-width IDIS file
 
     Returns:
-        - Pandas df
+        - Pandas DataFrame
     '''
     # Define an empty list to store column specifications
     col_specs = []
 
     # Read the fixed-width file
     with open(filename, 'r') as file:
-        # Skip the first 5 lines
-        for _ in range(5):
-            next(file)
+        # Skip line 1
+        next(file)
+        
+        # Read in line 2
+        table_name1 = file.readline().strip()
+
+        # Skip Line 3
+        next(file)
+
+        # Read in line 4 as table name
+        table_name2 = file.readline().strip()
+
+        # Skip line 5
+        next(file)
 
         # Read the file line by line
         for line in file:
             line = line.strip()
             if line:  # If the line is not empty
                 # Extract column position, name, and type
                 col_spec_parts = line.split()
@@ -45,14 +56,21 @@
             else:
                 # Break if a blank line is encountered
                 break
 
         # Read the data into a DataFrame using the extracted column specifications
         df = pd.read_fwf(file, colspecs=[(spec[0]-1, spec[1]) for spec in col_specs], names=[spec[2] for spec in col_specs])
 
+        # Add the TABLE_NAME column to the DataFrame
+        table_name = table_name1 + ' ' + table_name2
+        table_name = table_name.replace('*', '')
+        table_name = re.sub(r'\s+', ' ', table_name).strip()
+        table_name = table_name.replace(' ', '_').lower()
+        df['TABLE_NAME'] = table_name
+
     return df
 
 
 
 def extract_zip(zip_path):
     '''
     Extracts zipped folder contents to regular folder, deletes zipped folder after.
@@ -69,41 +87,47 @@
         zip_ref.extractall(extract_dir)
 
     # Remove the zip file after extraction
     os.remove(zip_path)
 
 
 
-def idis_fwf_to_csv(input_path, output_folder_path):
+def idis_fwf_to_file(input_path, output_folder_path, output_format='csv'):
     '''
     Process the IDIS FWF Export from HUD.
 
-    This function takes a path to a folder with FWF IDIS files or zipped folders with said files, and writes them out as CSVs to a defined output folder. 
+    This function takes a path to a folder with FWF IDIS files or zipped folders with said files, and writes them out as CSVs or Parquet files to a defined output folder.
 
     Parameters:
         - input_path: Path to the fixed-width IDIS files and/or zipped folders
-        - output_folder_path: Path to the folder you want the csvs written out to
+        - output_folder_path: Path to the folder you want the files written out to
+        - output_format: Output format, either 'csv' or 'parquet'. Default is 'csv'.
 
     Returns:
-        - All content that was fwfs as csvs
+        - All content that was fwfs as csvs or parquet files
     '''
     if not os.path.exists(input_path):
         print("The path does not exist.")
         return
 
     for item in os.listdir(input_path):
         item_path = os.path.join(input_path, item)
         if os.path.isfile(item_path):
             if item.lower().endswith('.txt'):
                 df = process_idis_fwf(item_path)
-                out_item = os.path.splitext(item)[0] + '.csv'
-                out_path = os.path.join(output_folder_path, out_item)
-                df.to_csv(out_path, index=False)
+                out_item = df['TABLE_NAME'][0]
+                if output_format == 'csv':
+                    out_path = os.path.join(output_folder_path, out_item + '.csv')
+                    df.to_csv(out_path, index=False)
+                elif output_format == 'parquet':
+                    out_path = os.path.join(output_folder_path, out_item + '.parquet')
+                    df.to_parquet(out_path, index=False)
+                else:
+                    print("Unsupported output format. Please choose either 'csv' or 'parquet'.")
             elif zipfile.is_zipfile(item_path):
                 extract_zip(item_path)
                 extract_path = os.path.join(input_path, os.path.splitext(item)[0])
-                idis_fwf_to_csv(extract_path, output_folder_path)
+                idis_fwf_to_file(extract_path, output_folder_path, output_format)
             else:
                 print(f"{item} is not a text file or zipped folder, skipping.")
         elif os.path.isdir(item_path):
-            idis_fwf_to_csv(item_path, output_folder_path)
-
+            idis_fwf_to_file(item_path, output_folder_path, output_format)
```

### Comparing `doh-tools-1.1/doh_tools/utils.py` & `doh-tools-1.2/doh_tools/utils.py`

 * *Files identical despite different names*

