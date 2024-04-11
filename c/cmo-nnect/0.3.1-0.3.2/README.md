# Comparing `tmp/cmo_nnect-0.3.1.tar.gz` & `tmp/cmo_nnect-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cmo_nnect-0.3.1.tar", last modified: Thu Nov 30 14:06:33 2023, max compression
+gzip compressed data, was "dist\cmo_nnect-0.3.2.tar", last modified: Thu Apr 11 13:58:36 2024, max compression
```

## Comparing `cmo_nnect-0.3.1.tar` & `cmo_nnect-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/
--rw-rw-rw-   0        0        0    35129 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    23355 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    19025 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/cmo_nnect/
--rw-rw-rw-   0        0        0      589 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/__init__.py
--rw-rw-rw-   0        0        0     4718 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/afasprofit.py
--rw-rw-rw-   0        0        0     2476 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/braze.py
--rw-rw-rw-   0        0        0     9852 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/businesscentral.py
--rw-rw-rw-   0        0        0     3301 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/dynamics365.py
--rw-rw-rw-   0        0        0     7252 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/exact.py
--rw-rw-rw-   0        0        0     3597 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/freshdesk.py
--rw-rw-rw-   0        0        0     3898 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/freshsales.py
--rw-rw-rw-   0        0        0     4716 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/ga4.py
--rw-rw-rw-   0        0        0     4575 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/helpers.py
--rw-rw-rw-   0        0        0     2380 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/kadaster.py
--rw-rw-rw-   0        0        0      899 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/knmi.py
--rw-rw-rw-   0        0        0     4517 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/mautic.py
--rw-rw-rw-   0        0        0     4416 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/notion.py
--rw-rw-rw-   0        0        0     5678 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/piano.py
--rw-rw-rw-   0        0        0     3869 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/recruitee.py
--rw-rw-rw-   0        0        0     4543 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/sfmc.py
--rw-rw-rw-   0        0        0     1569 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_afasprofit.py
--rw-rw-rw-   0        0        0     1927 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_braze.py
--rw-rw-rw-   0        0        0     2966 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_businesscentral.py
--rw-rw-rw-   0        0        0     4364 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_exact.py
--rw-rw-rw-   0        0        0     1732 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_freshdesk.py
--rw-rw-rw-   0        0        0     1665 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_freshsales.py
--rw-rw-rw-   0        0        0     1655 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/cmo_nnect/test_kadaster.py
--rw-rw-rw-   0        0        0      619 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_knmi.py
--rw-rw-rw-   0        0        0     2600 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_mautic.py
--rw-rw-rw-   0        0        0     2592 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_notion.py
--rw-rw-rw-   0        0        0     1919 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_piano.py
--rw-rw-rw-   0        0        0     2509 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_recruitee.py
--rw-rw-rw-   0        0        0     3358 2023-11-30 14:05:21.000000 cmo_nnect-0.3.1/cmo_nnect/test_sfmc.py
-drwxrwxrwx   0        0        0        0 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/
--rw-rw-rw-   0        0        0    23355 2023-11-30 14:06:32.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      896 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-30 14:06:32.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2023-11-30 14:06:32.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-11-30 14:06:32.000000 cmo_nnect-0.3.1/cmo_nnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-30 14:06:33.000000 cmo_nnect-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-11-30 14:05:20.000000 cmo_nnect-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/
+-rw-rw-rw-   0        0        0    35129 2024-04-11 13:58:02.000000 cmo_nnect-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    23355 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19025 2024-04-11 13:58:03.000000 cmo_nnect-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect/
+-rw-rw-rw-   0        0        0      589 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/__init__.py
+-rw-rw-rw-   0        0        0     4772 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/afasprofit.py
+-rw-rw-rw-   0        0        0     2476 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/braze.py
+-rw-rw-rw-   0        0        0     9852 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/businesscentral.py
+-rw-rw-rw-   0        0        0     3301 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/dynamics365.py
+-rw-rw-rw-   0        0        0     7252 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/exact.py
+-rw-rw-rw-   0        0        0     3597 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/freshdesk.py
+-rw-rw-rw-   0        0        0     3898 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/freshsales.py
+-rw-rw-rw-   0        0        0     4716 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/ga4.py
+-rw-rw-rw-   0        0        0     4575 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/helpers.py
+-rw-rw-rw-   0        0        0     2380 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/kadaster.py
+-rw-rw-rw-   0        0        0      899 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/knmi.py
+-rw-rw-rw-   0        0        0     4517 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/mautic.py
+-rw-rw-rw-   0        0        0     4416 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/notion.py
+-rw-rw-rw-   0        0        0     5678 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/piano.py
+-rw-rw-rw-   0        0        0     3869 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/recruitee.py
+-rw-rw-rw-   0        0        0     4543 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/sfmc.py
+-rw-rw-rw-   0        0        0     1569 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_afasprofit.py
+-rw-rw-rw-   0        0        0     1927 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_braze.py
+-rw-rw-rw-   0        0        0     2966 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_businesscentral.py
+-rw-rw-rw-   0        0        0     4364 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_exact.py
+-rw-rw-rw-   0        0        0     1732 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_freshdesk.py
+-rw-rw-rw-   0        0        0     1665 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_freshsales.py
+-rw-rw-rw-   0        0        0     1655 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_kadaster.py
+-rw-rw-rw-   0        0        0      619 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_knmi.py
+-rw-rw-rw-   0        0        0     2600 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_mautic.py
+-rw-rw-rw-   0        0        0     2592 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_notion.py
+-rw-rw-rw-   0        0        0     1919 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_piano.py
+-rw-rw-rw-   0        0        0     2509 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_recruitee.py
+-rw-rw-rw-   0        0        0     3358 2024-04-11 13:58:04.000000 cmo_nnect-0.3.2/cmo_nnect/test_sfmc.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/
+-rw-rw-rw-   0        0        0    23355 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      183 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/cmo_nnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:58:36.000000 cmo_nnect-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2024-04-11 13:58:03.000000 cmo_nnect-0.3.2/setup.py
```

### Comparing `cmo_nnect-0.3.1/LICENSE` & `cmo_nnect-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/PKG-INFO` & `cmo_nnect-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmo_nnect
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connect with a variety of API's with ease.
 Home-page: https://dev.azure.com/Cmotions/Packages/_git/cmo_nnect
 Author: Thijs van der Velden, Koen Leijsten
 Author-email: service@cmotions.nl
 License: UNKNOWN
 Description: # Cmotions Nnect (Cmo-Nnect)
```

### Comparing `cmo_nnect-0.3.1/README.md` & `cmo_nnect-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/__init__.py` & `cmo_nnect-0.3.2/cmo_nnect/__init__.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/afasprofit.py` & `cmo_nnect-0.3.2/cmo_nnect/afasprofit.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
         # creating an empty list and fill it with data first the api call of max 20.000 rows.
         all_rows = []
         all_rows += response_object.json()["rows"]
 
         # Loop through additional pages of data if any, and append to 'rows'-list.
         while response_object.json()["rows"]:
-            params["skip"] += 100
-            params["take"] += 100
+            params["skip"] += take
+            params["take"] += take
             response_object = requests.get(
                 url=url, headers=self.authorization, params=params
             )
 
             entity_data = response_object.json()["rows"]
             all_rows += entity_data
 
@@ -74,19 +74,19 @@
         # Set-up url to get-connector
         url = f"https://{str(self.company_id)}.rest.afas.online/ProfitRestServices/connectors/{connector_name}"
 
         # Format parameters
         base_params = {
             "skip": skip,
             "take": take,
-            "orderbyfieldids": order_by
-            if order_type == "asc"
-            else f"-{order_by}"
-            if order_by is not None
-            else None,  # Default descending, unless specifically ascending is requested
+            "orderbyfieldids": (
+                order_by
+                if order_type == "asc"
+                else f"-{order_by}" if order_by is not None else None
+            ),  # Default descending, unless specifically ascending is requested
             "filterfieldids": filter_fields,
             "filtervalues": filter_values,
             "operatortypes": operator_types,
         }
 
         # Eliminate None values
         params = {key: value for key, value in base_params.items() if value is not None}
@@ -110,15 +110,15 @@
                         skip,
                         take,
                     )
                 else:
                     profit_data = DataFrame(profit_response.json()["rows"])
             else:
                 raise ValueError(
-                    f"Received a response with statuscode {profit_response.status_code}."
+                    f"Received a response with statuscode {profit_response.status_code} with message {profit_response.text}."
                 )
 
             return profit_data
         elif connector_names:
             profit_data = self.execute_parallel(
                 get_data_function=self.get_data,
                 entity_list=connector_names,
```

### Comparing `cmo_nnect-0.3.1/cmo_nnect/braze.py` & `cmo_nnect-0.3.2/cmo_nnect/braze.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/businesscentral.py` & `cmo_nnect-0.3.2/cmo_nnect/businesscentral.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/dynamics365.py` & `cmo_nnect-0.3.2/cmo_nnect/dynamics365.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/exact.py` & `cmo_nnect-0.3.2/cmo_nnect/exact.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/freshdesk.py` & `cmo_nnect-0.3.2/cmo_nnect/freshdesk.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/freshsales.py` & `cmo_nnect-0.3.2/cmo_nnect/freshsales.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/ga4.py` & `cmo_nnect-0.3.2/cmo_nnect/ga4.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/helpers.py` & `cmo_nnect-0.3.2/cmo_nnect/helpers.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/kadaster.py` & `cmo_nnect-0.3.2/cmo_nnect/kadaster.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/knmi.py` & `cmo_nnect-0.3.2/cmo_nnect/knmi.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/mautic.py` & `cmo_nnect-0.3.2/cmo_nnect/mautic.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/notion.py` & `cmo_nnect-0.3.2/cmo_nnect/notion.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/piano.py` & `cmo_nnect-0.3.2/cmo_nnect/piano.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/recruitee.py` & `cmo_nnect-0.3.2/cmo_nnect/recruitee.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/sfmc.py` & `cmo_nnect-0.3.2/cmo_nnect/sfmc.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_afasprofit.py` & `cmo_nnect-0.3.2/cmo_nnect/test_afasprofit.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_braze.py` & `cmo_nnect-0.3.2/cmo_nnect/test_braze.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_businesscentral.py` & `cmo_nnect-0.3.2/cmo_nnect/test_businesscentral.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_exact.py` & `cmo_nnect-0.3.2/cmo_nnect/test_exact.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_freshdesk.py` & `cmo_nnect-0.3.2/cmo_nnect/test_freshdesk.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_freshsales.py` & `cmo_nnect-0.3.2/cmo_nnect/test_freshsales.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_kadaster.py` & `cmo_nnect-0.3.2/cmo_nnect/test_kadaster.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_knmi.py` & `cmo_nnect-0.3.2/cmo_nnect/test_knmi.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_mautic.py` & `cmo_nnect-0.3.2/cmo_nnect/test_mautic.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_notion.py` & `cmo_nnect-0.3.2/cmo_nnect/test_notion.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_piano.py` & `cmo_nnect-0.3.2/cmo_nnect/test_piano.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_recruitee.py` & `cmo_nnect-0.3.2/cmo_nnect/test_recruitee.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect/test_sfmc.py` & `cmo_nnect-0.3.2/cmo_nnect/test_sfmc.py`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/cmo_nnect.egg-info/PKG-INFO` & `cmo_nnect-0.3.2/cmo_nnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmo-nnect
-Version: 0.3.1
+Version: 0.3.2
 Summary: Connect with a variety of API's with ease.
 Home-page: https://dev.azure.com/Cmotions/Packages/_git/cmo_nnect
 Author: Thijs van der Velden, Koen Leijsten
 Author-email: service@cmotions.nl
 License: UNKNOWN
 Description: # Cmotions Nnect (Cmo-Nnect)
```

### Comparing `cmo_nnect-0.3.1/cmo_nnect.egg-info/SOURCES.txt` & `cmo_nnect-0.3.2/cmo_nnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmo_nnect-0.3.1/setup.py` & `cmo_nnect-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="cmo_nnect",
-    version="0.3.1",
+    version="0.3.2",
     python_requires=">=3.8",
     description="Connect with a variety of API's with ease.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Thijs van der Velden, Koen Leijsten",
     author_email="service@cmotions.nl",
     keyword=[
```

