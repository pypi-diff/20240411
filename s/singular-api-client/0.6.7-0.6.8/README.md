# Comparing `tmp/singular_api_client-0.6.7.tar.gz` & `tmp/singular_api_client-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singular_api_client-0.6.7.tar", last modified: Tue Jan 23 13:46:45 2024, max compression
+gzip compressed data, was "singular_api_client-0.6.8.tar", last modified: Thu Apr 11 10:32:12 2024, max compression
```

## Comparing `singular_api_client-0.6.7.tar` & `singular_api_client-0.6.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-01-23 13:46:45.225649 singular_api_client-0.6.7/
--rw-r--r--   0 yonathantzur   (501) staff       (20)      589 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/LICENSE.txt
--rw-r--r--   0 yonathantzur   (501) staff       (20)     1149 2024-01-23 13:46:45.225726 singular_api_client-0.6.7/PKG-INFO
--rw-r--r--   0 yonathantzur   (501) staff       (20)    14082 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/README.md
--rw-r--r--   0 yonathantzur   (501) staff       (20)      109 2024-01-23 13:46:45.225982 singular_api_client-0.6.7/setup.cfg
--rw-r--r--   0 yonathantzur   (501) staff       (20)     1533 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/setup.py
-drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-01-23 13:46:45.224626 singular_api_client-0.6.7/singular_api_client/
--rw-r--r--   0 yonathantzur   (501) staff       (20)       33 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/__init__.py
--rw-r--r--   0 yonathantzur   (501) staff       (20)      584 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/exceptions.py
--rw-r--r--   0 yonathantzur   (501) staff       (20)     6044 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/helpers.py
--rw-r--r--   0 yonathantzur   (501) staff       (20)     3241 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/params.py
--rw-r--r--   0 yonathantzur   (501) staff       (20)    22637 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/singular_client.py
--rw-r--r--   0 yonathantzur   (501) staff       (20)       22 2024-01-23 13:43:34.000000 singular_api_client-0.6.7/singular_api_client/version.py
-drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-01-23 13:46:45.225525 singular_api_client-0.6.7/singular_api_client.egg-info/
--rw-r--r--   0 yonathantzur   (501) staff       (20)     1149 2024-01-23 13:46:45.000000 singular_api_client-0.6.7/singular_api_client.egg-info/PKG-INFO
--rw-r--r--   0 yonathantzur   (501) staff       (20)      451 2024-01-23 13:46:45.000000 singular_api_client-0.6.7/singular_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 yonathantzur   (501) staff       (20)        1 2024-01-23 13:46:45.000000 singular_api_client-0.6.7/singular_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 yonathantzur   (501) staff       (20)       59 2024-01-23 13:46:45.000000 singular_api_client-0.6.7/singular_api_client.egg-info/requires.txt
--rw-r--r--   0 yonathantzur   (501) staff       (20)       20 2024-01-23 13:46:45.000000 singular_api_client-0.6.7/singular_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-04-11 10:32:12.176058 singular_api_client-0.6.8/
+-rw-r--r--   0 yonathantzur   (501) staff       (20)      589 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/LICENSE.txt
+-rw-r--r--   0 yonathantzur   (501) staff       (20)     1246 2024-04-11 10:32:12.175978 singular_api_client-0.6.8/PKG-INFO
+-rw-r--r--   0 yonathantzur   (501) staff       (20)    14082 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/README.md
+-rw-r--r--   0 yonathantzur   (501) staff       (20)      109 2024-04-11 10:32:12.176283 singular_api_client-0.6.8/setup.cfg
+-rw-r--r--   0 yonathantzur   (501) staff       (20)     1533 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/setup.py
+drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-04-11 10:32:12.175007 singular_api_client-0.6.8/singular_api_client/
+-rw-r--r--   0 yonathantzur   (501) staff       (20)       33 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/singular_api_client/__init__.py
+-rw-r--r--   0 yonathantzur   (501) staff       (20)      584 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/singular_api_client/exceptions.py
+-rw-r--r--   0 yonathantzur   (501) staff       (20)     6044 2024-01-23 13:43:34.000000 singular_api_client-0.6.8/singular_api_client/helpers.py
+-rw-r--r--   0 yonathantzur   (501) staff       (20)     3383 2024-04-11 10:30:27.000000 singular_api_client-0.6.8/singular_api_client/params.py
+-rw-r--r--   0 yonathantzur   (501) staff       (20)    25356 2024-04-11 10:30:27.000000 singular_api_client-0.6.8/singular_api_client/singular_client.py
+-rw-r--r--   0 yonathantzur   (501) staff       (20)       22 2024-04-11 10:30:27.000000 singular_api_client-0.6.8/singular_api_client/version.py
+drwxr-xr-x   0 yonathantzur   (501) staff       (20)        0 2024-04-11 10:32:12.175654 singular_api_client-0.6.8/singular_api_client.egg-info/
+-rw-r--r--   0 yonathantzur   (501) staff       (20)     1246 2024-04-11 10:32:12.000000 singular_api_client-0.6.8/singular_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 yonathantzur   (501) staff       (20)      451 2024-04-11 10:32:12.000000 singular_api_client-0.6.8/singular_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 yonathantzur   (501) staff       (20)        1 2024-04-11 10:32:12.000000 singular_api_client-0.6.8/singular_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 yonathantzur   (501) staff       (20)       59 2024-04-11 10:32:12.000000 singular_api_client-0.6.8/singular_api_client.egg-info/requires.txt
+-rw-r--r--   0 yonathantzur   (501) staff       (20)       20 2024-04-11 10:32:12.000000 singular_api_client-0.6.8/singular_api_client.egg-info/top_level.txt
```

### Comparing `singular_api_client-0.6.7/LICENSE.txt` & `singular_api_client-0.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `singular_api_client-0.6.7/PKG-INFO` & `singular_api_client-0.6.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: singular_api_client
-Version: 0.6.7
+Version: 0.6.8
 Summary: Helper Library to use Singular Reporting API
 Home-page: https://github.com/singular-labs/singular_api_client/
+Download-URL: https://github.com/singular-labs/singular_api_client/tarball/0.6.8
 Author: Singular Labs, Inc
 Author-email: devs@singular.net
 License: Apache
-Download-URL: https://github.com/singular-labs/singular_api_client/tarball/0.6.7
 Project-URL: Documentation, https://github.com/singular-labs/singular_api_client
 Project-URL: Source, https://github.com/singular-labs/singular_api_client
 Project-URL: Tracker, https://github.com/singular-labs/singular_api_client/issues
 Keywords: singular
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: pytz
+Requires-Dist: retrying
+Requires-Dist: futures; python_version == "2.7"
 
 This is the official Singular Reporting API Python Library. This library allows easy BI integration of Singular.
 For more information please visit our github repo: https://github.com/singular-labs/singular_api_client/
-
```

### Comparing `singular_api_client-0.6.7/README.md` & `singular_api_client-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `singular_api_client-0.6.7/setup.py` & `singular_api_client-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `singular_api_client-0.6.7/singular_api_client/exceptions.py` & `singular_api_client-0.6.8/singular_api_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `singular_api_client-0.6.7/singular_api_client/helpers.py` & `singular_api_client-0.6.8/singular_api_client/helpers.py`

 * *Files identical despite different names*

### Comparing `singular_api_client-0.6.7/singular_api_client/params.py` & `singular_api_client-0.6.8/singular_api_client/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     ADN_IMPRESSIONS = "adn_impressions"
     ADN_COST = "adn_cost"
     ADN_ORIGINAL_COST = "adn_original_cost"
     ADN_ESTIMATED_TOTAL_CONVERSIONS = "adn_estimated_total_conversions"
     CUSTOM_CLICKS = "custom_clicks"
     CUSTOM_INSTALLS = "custom_installs"
     SKAN_INSTALLS = "skan_installs"
+    UNIFIED_INSTALLS = "unified_installs"
+    UNIFIED_ECPI = "unified_ecpi"
+    UNIFIED_CVR = "unified_cvr"
+    UNIFIED_OCVR = "unified_ocvr"
     CTR = "ctr"
     CVR = "cvr"
     ECPI = "ecpi"
     OCVR = "ocvr"
     ECPM = "ecpm"
     ECPC = "ecpc"
```

### Comparing `singular_api_client-0.6.7/singular_api_client/singular_client.py` & `singular_api_client-0.6.8/singular_api_client/singular_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,14 +132,57 @@
                                                       app, source, time_breakdown, country_code_format,
                                                       filters, skadnetwork_date_type, **kwargs)
 
         response = self._api_post("v2.0/create_async_skadnetwork_raw_report", data=query_dict)
         parsed_response = response.json()
         return parsed_response["value"]["report_id"]
 
+    def create_async_unified_report(self, start_date, end_date,
+                                    format=Format.JSON,
+                                    dimensions=(Dimensions.APP, Dimensions.SOURCE),
+                                    metrics=(Metrics.UNIFIED_INSTALLS,),
+                                    cohort_metrics=None,
+                                    cohort_periods=None,
+                                    source=None,
+                                    app=None,
+                                    time_breakdown=TimeBreakdown.ALL,
+                                    country_code_format=CountryCodeFormat.ISO3,
+                                    filters=None,
+                                    **kwargs
+                                    ):
+        """
+        Use this endpoint to run custom queries in the Singular platform for aggregated unified data without
+         keeping a live connection throughout the request
+
+        :param start_date: "YYYY-mm-dd" format date
+        :param end_date: "YYYY-mm-dd" format date
+        :param format: Format for returned results, for example Format.JSON
+        :param dimensions: A list of dimensions, for example [Dimensions.APP, Dimensions.Source]
+        :param metrics: A list of metrics, for example [Metrics.UNIFIED_INSTALLS]
+        :param cohort_metrics: List of cohorted metrics by name or ID
+        :param cohort_periods: List of cohorted periods
+        :param source: optional List of source names to filter by
+        :param app: optional List of app names to filter by
+        :param time_breakdown: Break results by the requested time period, for example TimeBreakdown.DAY
+        :param country_code_format: Country code formatting option, for example CountryCodeFormat.ISO3
+        :param filters: A JSON encoded list of filters. Can be used to apply more complex filters than simply filtering
+          by app or source. The relation between different elements of the list is an AND relation.
+          A full list of the dimensions you can filter by and potential values can be retrieved from the
+          `get_reporting_filters` endpoint.
+        :return: report_id
+        """
+        query_dict = self._build_reporting_query(start_date, end_date, format, dimensions, metrics,
+                                                 None, cohort_metrics, cohort_periods, app, source,
+                                                 None, time_breakdown, country_code_format, filters,
+                                                 **kwargs)
+
+        response = self._api_post("v2.0/create_async_unified_report", data=query_dict)
+        parsed_response = response.json()
+        return parsed_response["value"]["report_id"]
+
     def create_async_skadnetwork_report(self, start_date, end_date,
                                         format=Format.JSON,
                                         dimensions=(Dimensions.APP, Dimensions.SOURCE,
                                                     Dimensions.SKAN_CAMPAIGN_ID, Dimensions.SKAN_CONVERSION_VALUE),
                                         metrics=(Metrics.SKAN_INSTALLS,),
                                         discrepancy_metrics=None,
                                         source=None,
```

### Comparing `singular_api_client-0.6.7/singular_api_client.egg-info/PKG-INFO` & `singular_api_client-0.6.8/singular_api_client.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: singular-api-client
-Version: 0.6.7
+Version: 0.6.8
 Summary: Helper Library to use Singular Reporting API
 Home-page: https://github.com/singular-labs/singular_api_client/
+Download-URL: https://github.com/singular-labs/singular_api_client/tarball/0.6.8
 Author: Singular Labs, Inc
 Author-email: devs@singular.net
 License: Apache
-Download-URL: https://github.com/singular-labs/singular_api_client/tarball/0.6.7
 Project-URL: Documentation, https://github.com/singular-labs/singular_api_client
 Project-URL: Source, https://github.com/singular-labs/singular_api_client
 Project-URL: Tracker, https://github.com/singular-labs/singular_api_client/issues
 Keywords: singular
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: pytz
+Requires-Dist: retrying
+Requires-Dist: futures; python_version == "2.7"
 
 This is the official Singular Reporting API Python Library. This library allows easy BI integration of Singular.
 For more information please visit our github repo: https://github.com/singular-labs/singular_api_client/
-
```

