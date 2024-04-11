# Comparing `tmp/veetility-0.3.8.tar.gz` & `tmp/veetility-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.3.8.tar", last modified: Mon Oct 16 13:21:34 2023, max compression
+gzip compressed data, was "veetility-0.3.9.tar", last modified: Thu Oct 19 10:07:09 2023, max compression
```

## Comparing `veetility-0.3.8.tar` & `veetility-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-16 13:21:34.015217 veetility-0.3.8/
--rw-r--r--   0 willbutler   (502) staff       (20)     3518 2023-10-16 13:21:34.015032 veetility-0.3.8/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.3.8/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-10-16 13:21:34.015281 veetility-0.3.8/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1437 2023-10-16 13:21:30.000000 veetility-0.3.8/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-16 13:21:34.008304 veetility-0.3.8/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.3.8/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.3.8/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.3.8/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-16 13:21:34.013777 veetility-0.3.8/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.3.8/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    18855 2023-09-28 09:44:10.000000 veetility-0.3.8/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     4797 2023-09-28 11:08:39.000000 veetility-0.3.8/veetility/email_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     4397 2023-08-18 12:05:15.000000 veetility-0.3.8/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)    31373 2023-09-29 08:54:16.000000 veetility-0.3.8/veetility/linkedin_api.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.3.8/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    38337 2023-10-16 13:18:26.000000 veetility-0.3.8/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    14531 2023-09-28 08:09:20.000000 veetility-0.3.8/veetility/rivaliq_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2340 2023-09-27 20:16:46.000000 veetility-0.3.8/veetility/s3_bucket.py
--rw-r--r--   0 willbutler   (502) staff       (20)     8976 2023-09-28 10:53:28.000000 veetility-0.3.8/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    56254 2023-10-09 10:43:22.000000 veetility-0.3.8/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2850 2023-09-27 16:57:08.000000 veetility-0.3.8/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11238 2023-09-28 09:20:07.000000 veetility-0.3.8/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-16 13:21:34.014800 veetility-0.3.8/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3518 2023-10-16 13:21:33.000000 veetility-0.3.8/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      666 2023-10-16 13:21:33.000000 veetility-0.3.8/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-10-16 13:21:33.000000 veetility-0.3.8/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-10-16 13:21:33.000000 veetility-0.3.8/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-10-16 13:21:33.000000 veetility-0.3.8/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-19 10:07:09.378087 veetility-0.3.9/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3518 2023-10-19 10:07:09.377876 veetility-0.3.9/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.3.9/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-10-19 10:07:09.378151 veetility-0.3.9/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1437 2023-10-19 10:07:01.000000 veetility-0.3.9/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-19 10:07:09.371032 veetility-0.3.9/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.3.9/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.3.9/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.3.9/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-19 10:07:09.376556 veetility-0.3.9/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.3.9/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    18855 2023-09-28 09:44:10.000000 veetility-0.3.9/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     4797 2023-09-28 11:08:39.000000 veetility-0.3.9/veetility/email_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     4397 2023-08-18 12:05:15.000000 veetility-0.3.9/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    31373 2023-09-29 08:54:16.000000 veetility-0.3.9/veetility/linkedin_api.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.3.9/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    38418 2023-10-19 10:01:42.000000 veetility-0.3.9/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    14531 2023-09-28 08:09:20.000000 veetility-0.3.9/veetility/rivaliq_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2340 2023-09-27 20:16:46.000000 veetility-0.3.9/veetility/s3_bucket.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     8976 2023-09-28 10:53:28.000000 veetility-0.3.9/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    56254 2023-10-09 10:43:22.000000 veetility-0.3.9/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2850 2023-09-27 16:57:08.000000 veetility-0.3.9/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11238 2023-09-28 09:20:07.000000 veetility-0.3.9/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-10-19 10:07:09.377620 veetility-0.3.9/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3518 2023-10-19 10:07:09.000000 veetility-0.3.9/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      666 2023-10-19 10:07:09.000000 veetility-0.3.9/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-10-19 10:07:09.000000 veetility-0.3.9/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-10-19 10:07:09.000000 veetility-0.3.9/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-10-19 10:07:09.000000 veetility-0.3.9/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.3.8/PKG-INFO` & `veetility-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.3.8
+Version: 0.3.9
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `veetility-0.3.8/README.md` & `veetility-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/setup.py` & `veetility-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.3.8",
+    version="0.3.9",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.3.8/tests/test_best_fuzzy_match_dict.py` & `veetility-0.3.9/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/tests/test_identify_match_multi_cols.py` & `veetility-0.3.9/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/tests/test_prepare_string_matching.py` & `veetility-0.3.9/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/cleaning_functions.py` & `veetility-0.3.9/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/email_functions.py` & `veetility-0.3.9/veetility/email_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/generic_functions.py` & `veetility-0.3.9/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/linkedin_api.py` & `veetility-0.3.9/veetility/linkedin_api.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/point_to_point_regressor.py` & `veetility-0.3.9/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/quality_assessments.py` & `veetility-0.3.9/veetility/quality_assessments.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,29 +315,30 @@
                 error_message = error_message + '  ' + f'The total of {key} has increased by more than\n'\
                                     f'{perc_increase_threshold}% from last time\n'\
                                         f' Prev Value = {old_dict[key]}, New Value = {new_dict[key]}\n'
                 
         # If cols_to_group is specified, then group by those columns and store the info in the dict
         if cols_to_group != None:
             new_dict['info'] = df.groupby(cols_to_group)[cols_to_check].sum().reset_index().to_json(orient='records')
+            print(f"Groupby of latest {name_of_df} = {new_dict['info']}")
         
         #The "Columns" and the "info" columns take up a low of space, so we only keep the last 5 entries in the db
         if check_cols_set == True: 
             cols_to_reduce_data = ['info','columns']
         else:
             cols_to_reduce_data = ['info']
 
         # If manual override is set to False, then add a new row to the historic db with the new values
         if not manual_override:
             if error_occured:
                 error_message = f'Comparison with historic df {name_of_df}: ' + error_message + '\n'
                 logger.info('ERROR' + error_message) # If error messages has been added to then log it
             if raise_exceptions and error_occured:
                 if 'num_unique_ids' in old_dict:
-                    error_message = error_message + f'\n Unique values count, {old_dict["num_unique_ids"]} -> {new_dict["num_unique_ids"]}'
+                    error_message = error_message + f'\n Unique values count change: {old_dict["num_unique_ids"]} -> {new_dict["num_unique_ids"]}'
                 raise Exception(error_message)
             if not error_occured:
                 new_dict['manual_override'] = False
                 db_with_new_row = pd.concat([historic_db, pd.DataFrame([new_dict])], ignore_index=True)
                 db_with_new_row.loc[db_with_new_row.iloc[:-5].index,cols_to_reduce_data] = np.nan
                 self.util.write_to_postgresql(db_with_new_row, name_of_table, if_exists='replace')
```

### Comparing `veetility-0.3.8/veetility/rivaliq_functions.py` & `veetility-0.3.9/veetility/rivaliq_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/s3_bucket.py` & `veetility-0.3.9/veetility/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/snowflake.py` & `veetility-0.3.9/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/utility_functions.py` & `veetility-0.3.9/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/v_lift.py` & `veetility-0.3.9/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility/view_through_rate.py` & `veetility-0.3.9/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.3.8/veetility.egg-info/PKG-INFO` & `veetility-0.3.9/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.3.8
+Version: 0.3.9
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `veetility-0.3.8/veetility.egg-info/SOURCES.txt` & `veetility-0.3.9/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

