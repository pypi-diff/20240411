# Comparing `tmp/SQLDataModel-0.3.6.tar.gz` & `tmp/SQLDataModel-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLDataModel-0.3.6.tar", last modified: Tue Apr  9 21:48:25 2024, max compression
+gzip compressed data, was "SQLDataModel-0.3.7.tar", last modified: Thu Apr 11 00:31:03 2024, max compression
```

## Comparing `SQLDataModel-0.3.6.tar` & `SQLDataModel-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.930335 SQLDataModel-0.3.6/
--rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.6/LICENSE
--rw-rw-rw-   0        0        0    27185 2024-04-09 21:48:25.915556 SQLDataModel-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.6/README.md
--rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 21:48:25.931336 SQLDataModel-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     2312 2024-04-09 21:45:20.000000 SQLDataModel-0.3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:21.317626 SQLDataModel-0.3.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:24.602173 SQLDataModel-0.3.6/src/SQLDataModel/
--rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.6/src/SQLDataModel/ANSIColor.py
--rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.6/src/SQLDataModel/HTMLParser.py
--rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.6/src/SQLDataModel/JSONEncoder.py
--rw-rw-rw-   0        0        0   559275 2024-04-09 21:46:29.000000 SQLDataModel-0.3.6/src/SQLDataModel/SQLDataModel.py
--rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.6/src/SQLDataModel/StandardDeviation.py
--rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.6/src/SQLDataModel/__init__.py
--rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.6/src/SQLDataModel/converters.py
--rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.6/src/SQLDataModel/demo.py
--rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.6/src/SQLDataModel/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.038923 SQLDataModel-0.3.6/src/SQLDataModel/extensions/
--rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.6/src/SQLDataModel/extensions/__init__.py
--rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.6/src/SQLDataModel/extensions/str_utils.c
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.906552 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/
--rw-rw-rw-   0        0        0    27185 2024-04-09 21:48:20.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-09 21:48:21.000000 SQLDataModel-0.3.6/src/SQLDataModel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-09 21:48:25.795861 SQLDataModel-0.3.6/tests/
--rw-rw-rw-   0        0        0    48353 2024-04-08 16:22:48.000000 SQLDataModel-0.3.6/tests/test_Future.py
--rw-rw-rw-   0        0        0    48356 2024-04-08 16:22:46.000000 SQLDataModel-0.3.6/tests/test_SQLDataModel.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.315938 SQLDataModel-0.3.7/
+-rw-rw-rw-   0        0        0     1095 2024-03-19 13:42:59.000000 SQLDataModel-0.3.7/LICENSE
+-rw-rw-rw-   0        0        0    27185 2024-04-11 00:31:03.309870 SQLDataModel-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0    25313 2024-04-01 18:33:13.000000 SQLDataModel-0.3.7/README.md
+-rw-rw-rw-   0        0        0       86 2023-12-16 01:14:43.000000 SQLDataModel-0.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 00:31:03.316454 SQLDataModel-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     2400 2024-04-11 00:20:07.000000 SQLDataModel-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:01.955320 SQLDataModel-0.3.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.110437 SQLDataModel-0.3.7/src/SQLDataModel/
+-rw-rw-rw-   0        0        0     6899 2024-03-19 22:34:49.000000 SQLDataModel-0.3.7/src/SQLDataModel/ANSIColor.py
+-rw-rw-rw-   0        0        0     9146 2024-03-20 22:08:53.000000 SQLDataModel-0.3.7/src/SQLDataModel/HTMLParser.py
+-rw-rw-rw-   0        0        0     1267 2024-03-19 22:36:01.000000 SQLDataModel-0.3.7/src/SQLDataModel/JSONEncoder.py
+-rw-rw-rw-   0        0        0   563580 2024-04-11 00:29:49.000000 SQLDataModel-0.3.7/src/SQLDataModel/SQLDataModel.py
+-rw-rw-rw-   0        0        0     2286 2024-03-19 22:36:42.000000 SQLDataModel-0.3.7/src/SQLDataModel/StandardDeviation.py
+-rw-rw-rw-   0        0        0      173 2024-03-05 04:16:05.000000 SQLDataModel-0.3.7/src/SQLDataModel/__init__.py
+-rw-rw-rw-   0        0        0     1501 2024-03-19 22:35:10.000000 SQLDataModel-0.3.7/src/SQLDataModel/converters.py
+-rw-rw-rw-   0        0        0     1269 2024-03-19 22:35:23.000000 SQLDataModel-0.3.7/src/SQLDataModel/demo.py
+-rw-rw-rw-   0        0        0     2826 2024-03-19 22:35:37.000000 SQLDataModel-0.3.7/src/SQLDataModel/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.250402 SQLDataModel-0.3.7/src/SQLDataModel/extensions/
+-rw-rw-rw-   0        0        0        0 2024-01-21 21:36:40.000000 SQLDataModel-0.3.7/src/SQLDataModel/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1355 2024-01-21 21:24:09.000000 SQLDataModel-0.3.7/src/SQLDataModel/extensions/str_utils.c
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.304171 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/
+-rw-rw-rw-   0        0        0    27185 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 00:31:01.000000 SQLDataModel-0.3.7/src/SQLDataModel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 00:31:03.262889 SQLDataModel-0.3.7/tests/
+-rw-rw-rw-   0        0        0    50768 2024-04-11 00:17:44.000000 SQLDataModel-0.3.7/tests/test_Future.py
+-rw-rw-rw-   0        0        0    50763 2024-04-11 00:17:45.000000 SQLDataModel-0.3.7/tests/test_SQLDataModel.py
```

### Comparing `SQLDataModel-0.3.6/LICENSE` & `SQLDataModel-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/PKG-INFO` & `SQLDataModel-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.6
+Version: 0.3.7
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.6/README.md` & `SQLDataModel-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/setup.py` & `SQLDataModel-0.3.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='SQLDataModel',  
-     version='0.3.6',
+     version='0.3.7',
      scripts=['src/SQLDataModel/SQLDataModel.py'] ,
      author='Ante Tonkovic-Capin',
      author_email='antetc@icloud.com',
      description='SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.',
-     keywords='SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package',
+     keywords=['SQL','ETL','dataframe','terminal tables','pretty print tables','sql2sql','data analysis','data science','data model','extract','transform','load','web scraping tables','data mining','html','html table parsing','apache arrow','pyarrow','pyarrow conversion','pyarrow to table','pyarrow to sql','pyarrow to csv','parquet file parsing','csv','csv parsing','markdown','markdown table parsing','latex','latex table parsing','delimited','delimited data parsing','file conversion','format conversion','terminal styling','table styling','from sqlite','to sqlite','from postgresql','to postgresql','sql to sql','excel','xlsx file','excel to sql','DataFrame package'],
      license_file='LICENSE',
      long_description=long_description,
      long_description_content_type='text/markdown',
      url='https://github.com/AnteT/SQLDataModel',
      project_urls = {
         'Documentation':'https://sqldatamodel.readthedocs.io/en/latest/',
         'Source': 'https://github.com/AnteT/SQLDataModel.git'
```

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/ANSIColor.py` & `SQLDataModel-0.3.7/src/SQLDataModel/ANSIColor.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/HTMLParser.py` & `SQLDataModel-0.3.7/src/SQLDataModel/HTMLParser.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/JSONEncoder.py` & `SQLDataModel-0.3.7/src/SQLDataModel/JSONEncoder.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/SQLDataModel.py` & `SQLDataModel-0.3.7/src/SQLDataModel/SQLDataModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -8047,16 +8047,16 @@
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: insufficient model count '{len(other)}', at least 1 additional 'SQLDataModel' is required to horizontally stack against")
             )
         if not all(isinstance(sdm, SQLDataModel) for sdm in other):
             raise TypeError(
                 SQLDataModel.ErrorFormat(f"TypeError: invalid type encountered in '{[type(other[n]).__name__ for n in other]}', arguments for `other` must all be of type 'SQLDataModel' to horizontally stack")
             )
-        other_headers, other_dtypes = zip(*[(col[0], col[1]) for sdm in other for col in sdm.get_column_dtypes().items()])
-        other_headers, other_dtypes = list(SQLDataModel.alias_duplicates([*self.headers,*other_headers])), [*self.get_column_dtypes().values(), *other_dtypes]
+        other_headers, other_dtypes = zip(*[(col[0], col[1]) for sdm in other for col in sdm.dtypes.items()])
+        other_headers, other_dtypes = list(SQLDataModel.alias_duplicates([*self.headers,*other_headers])), [*self.dtypes.values(), *other_dtypes]
         other_data = [(sdm[:self.row_count].data() if sdm.row_count > 1 else [sdm[:self.row_count].data()]) + [tuple(None for _ in range(sdm.column_count)) for _ in range(self.row_count - sdm.row_count)] for sdm in other]
         other_data = [tuple(item for sublist in row for item in sublist) for row in list(zip(*other_data))]
         if inplace:
             other_headers = other_headers[self.column_count:] # since in place remove current model's headers
             other_dtypes = other_dtypes[self.column_count:] # since in place remove current model's dtypes
             update_sql_script = ";".join([f"""alter table "{self.sql_model}" add column "{col_name}" {self.static_py_to_sql_map_dict.get(col_type, 'TEXT')}""" for col_name, col_type in zip(other_headers, other_dtypes)])
             col_val_param = ','.join([f""" "{col}" = {SQLDataModel.sqlite_cast_type_format(param='?', dtype=dtype)} """ for col,dtype in zip(other_headers, other_dtypes)])
@@ -8142,14 +8142,83 @@
         except ValueError as e:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f'ValueError: {e}, rename header or use `normalize_headers()` method to fix')
             ) from None
         res = self.sql_db_conn.execute(self._generate_sql_stmt(index=include_idx_col))
         yield from (Row(*x) for x in res.fetchall())
     
+    def mean(self) -> SQLDataModel:
+        """
+        Returns a new ``SQLDataModel`` containing the mean value of all viable columns in the current model. Calculated by ``sum(x_i, ..., x_n) * (1 / N)``
+
+        Returns:
+            ``SQLDataModel``: A new SQLDataModel containing the mean values of each column.
+
+        Example::
+        
+            from SQLDataModel import SQLDataModel
+
+            # Sample data
+            headers = ['Name', 'Age', 'Birthday', 'Height', 'Date of Hire']
+            data = [
+                ('John', 30, '1994-06-15', 175.3, '2018-03-03 11:20:19'), 
+                ('Alice', 28, '1996-11-20', 162.0, '2023-04-24 08:45:30'), 
+                ('Travis', 37, '1987-01-07', 185.8, '2012-10-06 15:30:40')
+            ]
+
+            # Create the model and infer correct types
+            sdm = SQLDataModel(data, headers, infer_dtypes=True)
+
+            # View full model
+            print(sdm)
+        
+        This will output the sample model we'll be using to calculate mean values for:
+
+        ```shell
+            ┌────────┬─────┬────────────┬─────────┬─────────────────────┐
+            │ Name   │ Age │ Birthday   │  Height │ Date of Hire        │
+            ├────────┼─────┼────────────┼─────────┼─────────────────────┤
+            │ John   │  30 │ 1994-06-15 │  175.30 │ 2018-03-03 11:20:19 │
+            │ Alice  │  28 │ 1996-11-20 │  162.00 │ 2023-04-24 08:45:30 │
+            │ Travis │  37 │ 1987-01-07 │  185.80 │ 2012-10-06 15:30:40 │
+            └────────┴─────┴────────────┴─────────┴─────────────────────┘
+            [3 rows x 5 columns]        
+        ```
+
+        Now let's find the mean values:
+
+        ```python
+            # Calculate the mean values
+            sdm_mean = sdm.mean()
+
+            # View result
+            print(sdm_mean)
+        ```
+
+        This will output the mean values for the "Age", "Birthday", "Height" and "Date of Hire" columns:
+
+        ```shell
+            ┌──────┬────────┬────────────┬─────────┬─────────────────────┐
+            │ Name │    Age │ Birthday   │  Height │ Date of Hire        │
+            ├──────┼────────┼────────────┼─────────┼─────────────────────┤
+            │ NaN  │  31.67 │ 1992-10-14 │  174.37 │ 2018-01-30 11:52:09 │
+            └──────┴────────┴────────────┴─────────┴─────────────────────┘
+            [1 rows x 5 columns]
+        ```
+
+        Note:
+            - Only non-null values are included in the calculation of the sum and the total number of values in the column, use :meth:`SQLDataModel.fillna()` to fill null values.
+            - For ``date`` and ``datetime`` columns values are converted to julian days prior to calculation and recast into original data type, some imprecision may occur as a result.
+            - See :meth:`SQLDataModel.min()` for returning the minimum value, :meth:`SQLDataModel.max()` for maximum value, and :meth:`SQLDataModel.describe()` for descriptive statical values.
+        """
+        fetch_stmt = ",".join([f"""avg("{col}") as "{col}" """ if dtype in ('int', 'float','bool') else f"""{dtype}(avg(julianday("{col}"))) as "{col}" """ if dtype in ('date','datetime') else f"""'NaN' as "{col}" """ for col,dtype in self.dtypes.items()])
+        fetch_stmt = " ".join(["select", fetch_stmt, f"""from "{self.sql_model}" """])
+        dtypes = {col:dtype if dtype not in ('int','bytes') else 'float' if dtype == 'int' else 'str' for col,dtype in self.dtypes.items()}
+        return self.execute_fetch(fetch_stmt, dtypes=dtypes)
+
     def min(self) -> SQLDataModel:
         """
         Returns a new ``SQLDataModel`` containing the minimum value of all non-null values for each column in a row-wise orientation.
 
         Returns:
             ``SQLDataModel``: A new SQLDataModel containing the minimum non-null value for each column.
 
@@ -8929,15 +8998,15 @@
                 raise SQLProgrammingError(
                     SQLDataModel.ErrorFormat(f"SQLProgrammingError: invalid update values, SQL execution failed with '{e}'")
                 ) from None            
             self._update_model_metadata(update_row_meta=True)
             return
         else:
             other_data = (*self.data(index=False, include_headers=False),*other_data)
-            return type(self)(data=other_data, headers=self.headers, dtypes=self.get_column_dtypes(), **self._get_display_args())
+            return type(self)(data=other_data, headers=self.headers, dtypes=self.dtypes, **self._get_display_args())
 
     def where(self, predicate:str) -> SQLDataModel:
         """
         Filters the rows of the current ``SQLDataModel`` object based on the specified SQL predicate and returns a
         new ``SQLDataModel`` containing only the rows that satisfy the condition. Only the predicates are needed as the statement prepends the select clause as "select [current model columns] where [`predicate`]", see below for detailed examples.
 
         Parameters:
@@ -9393,17 +9462,17 @@
         fetch_result = res.fetchall()
         fetch_headers = [x[0] for x in res.description]
         if (rows_returned := len(fetch_result)) < 1:
             raise ValueError(
                 SQLDataModel.ErrorFormat(f"ValueError: nothing to return, provided query returned '{rows_returned}' rows which is insufficient to return or generate a new model from")
             )
         if not kwargs:
-            return type(self)(fetch_result, headers=fetch_headers, dtypes=self.get_column_dtypes(), display_max_rows=self.display_max_rows, min_column_width=self.min_column_width, max_column_width=self.max_column_width, column_alignment=self.column_alignment, display_color=self.display_color, display_index=self.display_index, display_float_precision=self.display_float_precision)
+            return type(self)(fetch_result, headers=fetch_headers, dtypes=self.dtypes, display_max_rows=self.display_max_rows, min_column_width=self.min_column_width, max_column_width=self.max_column_width, column_alignment=self.column_alignment, display_color=self.display_color, display_index=self.display_index, display_float_precision=self.display_float_precision)
         else:
-            params = {"dtypes":self.get_column_dtypes(),"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision}
+            params = {"dtypes":self.dtypes,"display_max_rows":self.display_max_rows, "min_column_width":self.min_column_width, "max_column_width":self.max_column_width, "column_alignment":self.column_alignment, "display_color":self.display_color, "display_index":self.display_index, "display_float_precision":self.display_float_precision}
             params.update({k:v for k,v in kwargs.items()})
             return type(self)(fetch_result, headers=fetch_headers, **params)
 
     def execute_statement(self, sql_stmt:str) -> None:
         """
         Executes an arbitrary SQL query against the current model without the expectation of selection or returned rows.
```

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/StandardDeviation.py` & `SQLDataModel-0.3.7/src/SQLDataModel/StandardDeviation.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/converters.py` & `SQLDataModel-0.3.7/src/SQLDataModel/converters.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/demo.py` & `SQLDataModel-0.3.7/src/SQLDataModel/demo.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/exceptions.py` & `SQLDataModel-0.3.7/src/SQLDataModel/exceptions.py`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel/extensions/str_utils.c` & `SQLDataModel-0.3.7/src/SQLDataModel/extensions/str_utils.c`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel.egg-info/PKG-INFO` & `SQLDataModel-0.3.7/src/SQLDataModel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SQLDataModel
-Version: 0.3.6
+Version: 0.3.7
 Summary: SQLDataModel is a lightweight dataframe library designed for efficient data extraction, transformation, and loading (ETL) across various sources and destinations, providing an efficient alternative to common setups like pandas, numpy, and sqlalchemy while also providing additional features without the overhead of external dependencies.
 Home-page: https://github.com/AnteT/SQLDataModel
 Author: Ante Tonkovic-Capin
 Author-email: antetc@icloud.com
 Project-URL: Documentation, https://sqldatamodel.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/AnteT/SQLDataModel.git
 Keywords: SQL,ETL,dataframe,terminal tables,pretty print tables,sql2sql,data analysis,data science,data model,extract,transform,load,web scraping tables,data mining,html,html table parsing,apache arrow,pyarrow,pyarrow conversion,pyarrow to table,pyarrow to sql,pyarrow to csv,parquet file parsing,csv,csv parsing,markdown,markdown table parsing,latex,latex table parsing,delimited,delimited data parsing,file conversion,format conversion,terminal styling,table styling,from sqlite,to sqlite,from postgresql,to postgresql,sql to sql,excel,xlsx file,excel to sql,DataFrame package
```

### Comparing `SQLDataModel-0.3.6/src/SQLDataModel.egg-info/SOURCES.txt` & `SQLDataModel-0.3.7/src/SQLDataModel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SQLDataModel-0.3.6/tests/test_Future.py` & `SQLDataModel-0.3.7/tests/test_Future.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from future.SQLDataModel_future import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
+@pytest.fixture
+def sample_data_parameterized() -> tuple[list[list], list[str]]:
+    """Returns sample data from data_generator function with pass through parameters for customizing output for testing."""
+    def _data_generator(num_rows=12, float_precision=2, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='separate', exclude_nonetype=True):
+        return data_generator(num_rows=num_rows, float_precision=float_precision, num_columns=num_columns, seed=seed, return_header_type=return_header_type, return_row_type=return_row_type, return_format=return_format, exclude_nonetype=exclude_nonetype)
+    return _data_generator
+
 @pytest.mark.core
 def test_init(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     input_rows, input_cols = len(input_data), len(input_data[0])
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     assert sdm.row_count == input_rows and sdm.column_count == input_cols
     assert sdm.headers == input_headers
@@ -768,8 +775,30 @@
     assert output_data == expected_data    
 
 @pytest.mark.core
 def test_transpose():
     num_rows, num_cols = 10, 5
     input_data = [tuple(f"{i},{j}" for j in range(num_cols)) for i in range(num_rows)]
     output_data = SQLDataModel(input_data).transpose(infer_types=True,include_headers=False).transpose(infer_types=True,include_headers=False).data()
-    assert output_data == input_data
+    assert output_data == input_data
+
+@pytest.mark.core
+def test_min(sample_data_parameterized):
+    data, headers = sample_data_parameterized(exclude_nonetype=True)
+    expected_data = tuple(min([row[j] for row in data]) for j in range(len(data[0])))
+    output_data = SQLDataModel(data, headers).min().data()
+    assert output_data == expected_data
+
+@pytest.mark.core
+def test_max(sample_data_parameterized):
+    data, headers = sample_data_parameterized(exclude_nonetype=True)
+    expected_data = tuple(max([row[j] for row in data]) for j in range(len(data[0])))
+    output_data = SQLDataModel(data, headers).max().data()
+    assert output_data == expected_data    
+
+@pytest.mark.core
+def test_mean():
+    data = [('QNkrwWcsJnL', -633, 996.8432, 1, datetime.date(1962, 6, 7), b'3S7Z8ZcCeSc', datetime.datetime(1948, 10, 13, 9, 42, 47), 'waRB660S'), ('C5', -380, -585.4195, 1, datetime.date(1944, 9, 6), b'VceF78VXuWI', datetime.datetime(2020, 4, 23, 20, 14, 56), 'rABpuXdI'), ('FfeWNVq', -378, 575.8778, 0, datetime.date(1998, 3, 3), b'YyPoUKrPK', datetime.datetime(1958, 4, 18, 3, 11, 46), 'j2lb'), ('Xx', -744, 972.1331, 1, datetime.date(1994, 1, 19), b'PJyDr', datetime.datetime(2022, 12, 17, 14, 49, 10), 'KpWirYfv'), ('SuzgO', -627, 332.6614, 1, datetime.date(2011, 9, 14), b'b9', datetime.datetime(1922, 2, 25, 23, 23, 58), 'WM1VHoJ25zf'), ('69UEuh0', -954, -906.1676, 1, datetime.date(1980, 7, 26), b'PYesip__', datetime.datetime(1954, 8, 5, 4, 38, 33), 'jUWRBAyJXV')]    
+    expected_data = ('NaN', -619.3333333333334, 230.98806666666667, 0.8333333333333334, datetime.date(1981, 12, 7), 'NaN', datetime.datetime(1971, 3, 8, 16, 40, 11), 'NaN')
+    output_data = SQLDataModel(data).mean().data()
+    assert output_data == expected_data
+
```

### Comparing `SQLDataModel-0.3.6/tests/test_SQLDataModel.py` & `SQLDataModel-0.3.7/tests/test_SQLDataModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from src.SQLDataModel.SQLDataModel import SQLDataModel
 
 @pytest.fixture
 def sample_data() -> tuple[list[list], list[str]]:
     """Returns sample data in format `(data, headers)` to use for testing."""
     return data_generator(num_rows=120, float_precision=4, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='combined')
 
+@pytest.fixture
+def sample_data_parameterized() -> tuple[list[list], list[str]]:
+    """Returns sample data from data_generator function with pass through parameters for customizing output for testing."""
+    def _data_generator(num_rows=12, float_precision=2, num_columns=8, seed=42, return_header_type='list', return_row_type='tuple', return_format='separate', exclude_nonetype=True):
+        return data_generator(num_rows=num_rows, float_precision=float_precision, num_columns=num_columns, seed=seed, return_header_type=return_header_type, return_row_type=return_row_type, return_format=return_format, exclude_nonetype=exclude_nonetype)
+    return _data_generator
+
 @pytest.mark.core
 def test_init(sample_data):
     input_data, input_headers = sample_data[1:], sample_data[0]
     input_rows, input_cols = len(input_data), len(input_data[0])
     sdm = SQLDataModel(data=input_data, headers=input_headers)
     assert sdm.row_count == input_rows and sdm.column_count == input_cols
     assert sdm.headers == input_headers
@@ -768,8 +775,29 @@
     assert output_data == expected_data    
 
 @pytest.mark.core
 def test_transpose():
     num_rows, num_cols = 10, 5
     input_data = [tuple(f"{i},{j}" for j in range(num_cols)) for i in range(num_rows)]
     output_data = SQLDataModel(input_data).transpose(infer_types=True,include_headers=False).transpose(infer_types=True,include_headers=False).data()
-    assert output_data == input_data
+    assert output_data == input_data
+
+@pytest.mark.core
+def test_min(sample_data_parameterized):
+    data, headers = sample_data_parameterized(exclude_nonetype=True)
+    expected_data = tuple(min([row[j] for row in data]) for j in range(len(data[0])))
+    output_data = SQLDataModel(data, headers).min().data()
+    assert output_data == expected_data
+
+@pytest.mark.core
+def test_max(sample_data_parameterized):
+    data, headers = sample_data_parameterized(exclude_nonetype=True)
+    expected_data = tuple(max([row[j] for row in data]) for j in range(len(data[0])))
+    output_data = SQLDataModel(data, headers).max().data()
+    assert output_data == expected_data    
+
+@pytest.mark.core
+def test_mean():
+    data = [('QNkrwWcsJnL', -633, 996.8432, 1, datetime.date(1962, 6, 7), b'3S7Z8ZcCeSc', datetime.datetime(1948, 10, 13, 9, 42, 47), 'waRB660S'), ('C5', -380, -585.4195, 1, datetime.date(1944, 9, 6), b'VceF78VXuWI', datetime.datetime(2020, 4, 23, 20, 14, 56), 'rABpuXdI'), ('FfeWNVq', -378, 575.8778, 0, datetime.date(1998, 3, 3), b'YyPoUKrPK', datetime.datetime(1958, 4, 18, 3, 11, 46), 'j2lb'), ('Xx', -744, 972.1331, 1, datetime.date(1994, 1, 19), b'PJyDr', datetime.datetime(2022, 12, 17, 14, 49, 10), 'KpWirYfv'), ('SuzgO', -627, 332.6614, 1, datetime.date(2011, 9, 14), b'b9', datetime.datetime(1922, 2, 25, 23, 23, 58), 'WM1VHoJ25zf'), ('69UEuh0', -954, -906.1676, 1, datetime.date(1980, 7, 26), b'PYesip__', datetime.datetime(1954, 8, 5, 4, 38, 33), 'jUWRBAyJXV')]    
+    expected_data = ('NaN', -619.3333333333334, 230.98806666666667, 0.8333333333333334, datetime.date(1981, 12, 7), 'NaN', datetime.datetime(1971, 3, 8, 16, 40, 11), 'NaN')
+    output_data = SQLDataModel(data).mean().data()
+    assert output_data == expected_data
```

