# Comparing `tmp/botocore-a-la-carte-location-1.34.82.tar.gz` & `tmp/botocore-a-la-carte-location-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-location-1.34.82.tar", last modified: Thu Apr 11 01:01:02 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-location-1.34.9.tar", last modified: Thu Dec 28 01:06:55 2023, max compression
```

## Comparing `botocore-a-la-carte-location-1.34.82.tar` & `botocore-a-la-carte-location-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.648858 botocore-a-la-carte-location-1.34.82/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 01:01:02.648858 botocore-a-la-carte-location-1.34.82/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.644858 botocore-a-la-carte-location-1.34.82/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.644858 botocore-a-la-carte-location-1.34.82/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.644858 botocore-a-la-carte-location-1.34.82/botocore/data/location/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.648858 botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-11 01:00:33.000000 botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 01:00:33.000000 botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-11 01:00:33.000000 botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   292997 2024-04-11 01:00:33.000000 botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:02.648858 botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:01:02.648858 botocore-a-la-carte-location-1.34.82/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-11 01:01:02.000000 botocore-a-la-carte-location-1.34.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.214385 botocore-a-la-carte-location-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:54.000000 botocore-a-la-carte-location-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:06:55.214385 botocore-a-la-carte-location-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.210385 botocore-a-la-carte-location-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.210385 botocore-a-la-carte-location-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.210385 botocore-a-la-carte-location-1.34.9/botocore/data/location/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.214385 botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2023-12-28 01:06:26.000000 botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-12-28 01:06:26.000000 botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   287133 2023-12-28 01:06:26.000000 botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.214385 botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:06:55.000000 botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2023-12-28 01:06:55.000000 botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:55.000000 botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:55.000000 botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:55.214385 botocore-a-la-carte-location-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-28 01:06:54.000000 botocore-a-la-carte-location-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-location-1.34.82/LICENSE.txt` & `botocore-a-la-carte-location-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.34.82/PKG-INFO` & `botocore-a-la-carte-location-1.34.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-location
-Version: 1.34.82
+Version: 1.34.9
 Summary: location data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/endpoint-rule-set-1.json` & `botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/paginators-1.json` & `botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-location-1.34.82/botocore/data/location/2020-11-19/service-2.json` & `botocore-a-la-carte-location-1.34.9/botocore/data/location/2020-11-19/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993087219058374%*

 * *Differences: {"'shapes'": "{'ApiKeyRestrictions': {'members': {'AllowResources': {'documentation': '<p>A list "*

 * *             'of allowed resource ARNs that a API key bearer can perform actions on.</p> <ul> <li> '*

 * *             '<p>The ARN must be the correct ARN for a map, place, or route ARN. You may include '*

 * *             'wildcards in the resource-id to match multiple resources of the same type.</p> </li> '*

 * *             '<li> <p>The resources must be in the same <code>partition</code>, '*

 * *             '<code>region</co […]*

```diff
@@ -2117,15 +2117,15 @@
                     "shape": "ApiKeyRestrictionsAllowActionsList"
                 },
                 "AllowReferers": {
                     "documentation": "<p>An optional list of allowed HTTP referers for which requests must originate from. Requests using this API key from other domains will not be allowed.</p> <p>Requirements:</p> <ul> <li> <p>Contain only alphanumeric characters (A\u2013Z, a\u2013z, 0\u20139) or any symbols in this list <code>$\\-._+!*`(),;/?:@=&amp;</code> </p> </li> <li> <p>May contain a percent (%) if followed by 2 hexadecimal digits (A-F, a-f, 0-9); this is used for URL encoding purposes.</p> </li> <li> <p>May contain wildcard characters question mark (?) and asterisk (*).</p> <p>Question mark (?) will replace any single character (including hexadecimal digits).</p> <p>Asterisk (*) will replace any multiple characters (including multiple hexadecimal digits).</p> </li> <li> <p>No spaces allowed. For example, <code>https://example.com</code>.</p> </li> </ul>",
                     "shape": "ApiKeyRestrictionsAllowReferersList"
                 },
                 "AllowResources": {
-                    "documentation": "<p>A list of allowed resource ARNs that a API key bearer can perform actions on.</p> <ul> <li> <p>The ARN must be the correct ARN for a map, place, or route ARN. You may include wildcards in the resource-id to match multiple resources of the same type.</p> </li> <li> <p>The resources must be in the same <code>partition</code>, <code>region</code>, and <code>account-id</code> as the key that is being created.</p> </li> <li> <p>Other than wildcards, you must include the full ARN, including the <code>arn</code>, <code>partition</code>, <code>service</code>, <code>region</code>, <code>account-id</code> and <code>resource-id</code> delimited by colons (:).</p> </li> <li> <p>No spaces allowed, even with wildcards. For example, <code>arn:aws:geo:region:<i>account-id</i>:map/ExampleMap*</code>.</p> </li> </ul> <p>For more information about ARN format, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names (ARNs)</a>.</p>",
+                    "documentation": "<p>A list of allowed resource ARNs that a API key bearer can perform actions on.</p> <ul> <li> <p>The ARN must be the correct ARN for a map, place, or route ARN. You may include wildcards in the resource-id to match multiple resources of the same type.</p> </li> <li> <p>The resources must be in the same <code>partition</code>, <code>region</code>, and <code>account-id</code> as the key that is being created.</p> </li> <li> <p>Other than wildcards, you must include the full ARN, including the <code>arn</code>, <code>partition</code>, <code>service</code>, <code>region</code>, <code>account-id</code> and <code>resource-id</code>, delimited by colons (:).</p> </li> <li> <p>No spaces allowed, even with wildcards. For example, <code>arn:aws:geo:region:<i>account-id</i>:map/ExampleMap*</code>.</p> </li> </ul> <p>For more information about ARN format, see <a href=\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\">Amazon Resource Names (ARNs)</a>.</p>",
                     "shape": "ApiKeyRestrictionsAllowResourcesList"
                 }
             },
             "required": [
                 "AllowActions",
                 "AllowResources"
             ],
@@ -3419,28 +3419,14 @@
             "required": [
                 "CreateTime",
                 "TrackerArn",
                 "TrackerName"
             ],
             "type": "structure"
         },
-        "CustomLayer": {
-            "max": 100,
-            "min": 1,
-            "pattern": "^[-._\\w]+$",
-            "type": "string"
-        },
-        "CustomLayerList": {
-            "max": 10,
-            "member": {
-                "shape": "CustomLayer"
-            },
-            "min": 0,
-            "type": "list"
-        },
         "DataSourceConfiguration": {
             "documentation": "<p>Specifies the data storage option chosen for requesting Places.</p> <important> <p>When using Amazon Location Places:</p> <ul> <li> <p>If using HERE Technologies as a data provider, you can't store results for locations in Japan by setting <code>IntendedUse</code> to <code>Storage</code>. parameter.</p> </li> <li> <p>Under the <code>MobileAssetTracking</code> or <code>MobilAssetManagement</code> pricing plan, you can't store results from your place index resources by setting <code>IntendedUse</code> to <code>Storage</code>. This returns a validation exception error.</p> </li> </ul> <p>For more information, see the <a href=\"https://aws.amazon.com/service-terms/\">AWS Service Terms</a> for Amazon Location Service.</p> </important>",
             "members": {
                 "IntendedUse": {
                     "documentation": "<p>Specifies how the results of an operation will be stored by the caller. </p> <p>Valid values include:</p> <ul> <li> <p> <code>SingleUse</code> specifies that the results won't be stored. </p> </li> <li> <p> <code>Storage</code> specifies that the result can be cached or stored in a database.</p> </li> </ul> <p>Default value: <code>SingleUse</code> </p>",
                     "shape": "IntendedUse"
                 }
@@ -3463,20 +3449,14 @@
         },
         "DeleteGeofenceCollectionResponse": {
             "members": {},
             "type": "structure"
         },
         "DeleteKeyRequest": {
             "members": {
-                "ForceDelete": {
-                    "documentation": "<p>ForceDelete bypasses an API key's expiry conditions and deletes the key. Set the parameter <code>true</code> to delete the key or to <code>false</code> to not preemptively delete the API key.</p> <p>Valid values: <code>true</code>, or <code>false</code>.</p> <p>Required: No</p> <note> <p>This action is irreversible. Only use ForceDelete if you are certain the key is no longer in use.</p> </note>",
-                    "location": "querystring",
-                    "locationName": "forceDelete",
-                    "shape": "Boolean"
-                },
                 "KeyName": {
                     "documentation": "<p>The name of the API key to delete.</p>",
                     "location": "uri",
                     "locationName": "KeyName",
                     "shape": "ResourceName"
                 }
             },
@@ -4283,15 +4263,15 @@
                 "UpdateTime"
             ],
             "type": "structure"
         },
         "GetMapGlyphsRequest": {
             "members": {
                 "FontStack": {
-                    "documentation": "<p>A comma-separated list of fonts to load glyphs from in order of preference. For example, <code>Noto Sans Regular, Arial Unicode</code>.</p> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri</a> styles: </p> <ul> <li> <p>VectorEsriDarkGrayCanvas \u2013 <code>Ubuntu Medium Italic</code> | <code>Ubuntu Medium</code> | <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriLightGrayCanvas \u2013 <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Light</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriTopographic \u2013 <code>Noto Sans Italic</code> | <code>Noto Sans Regular</code> | <code>Noto Sans Bold</code> | <code>Noto Serif Regular</code> | <code>Roboto Condensed Light Italic</code> </p> </li> <li> <p>VectorEsriStreets \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> <li> <p>VectorEsriNavigation \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> | <code>Arial Unicode MS Bold</code> | <code>Arial Unicode MS Regular</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies</a> styles:</p> <ul> <li> <p>VectorHereContrast \u2013 <code>Fira GO Regular</code> | <code>Fira GO Bold</code> </p> </li> <li> <p>VectorHereExplore, VectorHereExploreTruck, HybridHereExploreSatellite \u2013 <code>Fira GO Italic</code> | <code>Fira GO Map</code> | <code>Fira GO Map Bold</code> | <code>Noto Sans CJK JP Bold</code> | <code>Noto Sans CJK JP Light</code> | <code>Noto Sans CJK JP Regular</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps</a> styles:</p> <ul> <li> <p>VectorGrabStandardLight, VectorGrabStandardDark \u2013 <code>Noto Sans Regular</code> | <code>Noto Sans Medium</code> | <code>Noto Sans Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data</a> styles:</p> <ul> <li> <p>VectorOpenDataStandardLight, VectorOpenDataStandardDark, VectorOpenDataVisualizationLight, VectorOpenDataVisualizationDark \u2013 <code>Amazon Ember Regular,Noto Sans Regular</code> | <code>Amazon Ember Bold,Noto Sans Bold</code> | <code>Amazon Ember Medium,Noto Sans Medium</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold</code> | <code>Amazon Ember Regular,Noto Sans Regular,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold,Noto Sans Arabic Condensed Bold</code> | <code>Amazon Ember Bold,Noto Sans Bold,Noto Sans Arabic Bold</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular,Noto Sans Arabic Condensed Regular</code> | <code>Amazon Ember Medium,Noto Sans Medium,Noto Sans Arabic Medium</code> </p> </li> </ul> <note> <p>The fonts used by the Open Data map styles are combined fonts that use <code>Amazon Ember</code> for most glyphs but <code>Noto Sans</code> for glyphs unsupported by <code>Amazon Ember</code>.</p> </note>",
+                    "documentation": "<p>A comma-separated list of fonts to load glyphs from in order of preference. For example, <code>Noto Sans Regular, Arial Unicode</code>.</p> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri</a> styles: </p> <ul> <li> <p>VectorEsriDarkGrayCanvas \u2013 <code>Ubuntu Medium Italic</code> | <code>Ubuntu Medium</code> | <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriLightGrayCanvas \u2013 <code>Ubuntu Italic</code> | <code>Ubuntu Regular</code> | <code>Ubuntu Light</code> | <code>Ubuntu Bold</code> </p> </li> <li> <p>VectorEsriTopographic \u2013 <code>Noto Sans Italic</code> | <code>Noto Sans Regular</code> | <code>Noto Sans Bold</code> | <code>Noto Serif Regular</code> | <code>Roboto Condensed Light Italic</code> </p> </li> <li> <p>VectorEsriStreets \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> <li> <p>VectorEsriNavigation \u2013 <code>Arial Regular</code> | <code>Arial Italic</code> | <code>Arial Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies</a> styles:</p> <ul> <li> <p>VectorHereContrast \u2013 <code>Fira GO Regular</code> | <code>Fira GO Bold</code> </p> </li> <li> <p>VectorHereExplore, VectorHereExploreTruck, HybridHereExploreSatellite \u2013 <code>Fira GO Italic</code> | <code>Fira GO Map</code> | <code>Fira GO Map Bold</code> | <code>Noto Sans CJK JP Bold</code> | <code>Noto Sans CJK JP Light</code> | <code>Noto Sans CJK JP Regular</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps</a> styles:</p> <ul> <li> <p>VectorGrabStandardLight, VectorGrabStandardDark \u2013 <code>Noto Sans Regular</code> | <code>Noto Sans Medium</code> | <code>Noto Sans Bold</code> </p> </li> </ul> <p>Valid font stacks for <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data</a> styles:</p> <ul> <li> <p>VectorOpenDataStandardLight, VectorOpenDataStandardDark, VectorOpenDataVisualizationLight, VectorOpenDataVisualizationDark \u2013 <code>Amazon Ember Regular,Noto Sans Regular</code> | <code>Amazon Ember Bold,Noto Sans Bold</code> | <code>Amazon Ember Medium,Noto Sans Medium</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold</code> | <code>Amazon Ember Regular,Noto Sans Regular,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Bold,Noto Sans Bold,Noto Sans Arabic Condensed Bold</code> | <code>Amazon Ember Bold,Noto Sans Bold,Noto Sans Arabic Bold</code> | <code>Amazon Ember Regular Italic,Noto Sans Italic,Noto Sans Arabic Regular</code> | <code>Amazon Ember Condensed RC Regular,Noto Sans Regular,Noto Sans Arabic Condensed Regular</code> | <code>Amazon Ember Medium,Noto Sans Medium,Noto Sans Arabic Medium</code> </p> </li> </ul> <note> <p>The fonts used by the Open Data map styles are combined fonts that use <code>Amazon Ember</code> for most glyphs but <code>Noto Sans</code> for glyphs unsupported by <code>Amazon Ember</code>.</p> </note>",
                     "location": "uri",
                     "locationName": "FontStack",
                     "shape": "String"
                 },
                 "FontUnicodeRange": {
                     "documentation": "<p>A Unicode range of characters to download glyphs for. Each response will contain 256 characters. For example, 0\u2013255 includes all characters from range <code>U+0000</code> to <code>00FF</code>. Must be aligned to multiples of 256.</p>",
                     "location": "uri",
@@ -4531,15 +4511,15 @@
                 "Language": {
                     "documentation": "<p>The preferred language used to return results. The value must be a valid <a href=\"https://tools.ietf.org/search/bcp47\">BCP 47</a> language tag, for example, <code>en</code> for English.</p> <p>This setting affects the languages used in the results, but not the results themselves. If no language is specified, or not supported for a particular result, the partner automatically chooses a language for the result.</p> <p>For an example, we'll use the Greek language. You search for a location around Athens, Greece, with the <code>language</code> parameter set to <code>en</code>. The <code>city</code> in the results will most likely be returned as <code>Athens</code>.</p> <p>If you set the <code>language</code> parameter to <code>el</code>, for Greek, then the <code>city</code> in the results will more likely be returned as <code>\u0391\u03b8\u03ae\u03bd\u03b1</code>.</p> <p>If the data provider does not have a value for Greek, the result will be in a language that the provider does support.</p>",
                     "location": "querystring",
                     "locationName": "language",
                     "shape": "LanguageTag"
                 },
                 "PlaceId": {
-                    "documentation": "<p>The identifier of the place to find.</p> <p>While you can use PlaceID in subsequent requests, PlaceID is not intended to be a permanent identifier and the ID can change between consecutive API calls. Please see the following PlaceID behaviour for each data provider:</p> <ul> <li> <p>Esri: Place IDs will change every quarter at a minimum. The typical time period for these changes would be March, June, September, and December. Place IDs might also change between the typical quarterly change but that will be much less frequent.</p> </li> <li> <p>HERE: We recommend that you cache data for no longer than a week to keep your data data fresh. You can assume that less than 1% ID shifts will release over release which is approximately 1 - 2 times per week.</p> </li> <li> <p>Grab: Place IDs can expire or become invalid in the following situations.</p> <ul> <li> <p>Data operations: The POI may be removed from Grab POI database by Grab Map Ops based on the ground-truth, such as being closed in the real world, being detected as a duplicate POI, or having incorrect information. Grab will synchronize data to the Waypoint environment on weekly basis.</p> </li> <li> <p>Interpolated POI: Interpolated POI is a temporary POI generated in real time when serving a request, and it will be marked as derived in the <code>place.result_type</code> field in the response. The information of interpolated POIs will be retained for at least 30 days, which means that within 30 days, you are able to obtain POI details by Place ID from Place Details API. After 30 days, the interpolated POIs(both Place ID and details) may expire and inaccessible from the Places Details API.</p> </li> </ul> </li> </ul>",
+                    "documentation": "<p>The identifier of the place to find.</p>",
                     "location": "uri",
                     "locationName": "PlaceId",
                     "shape": "PlaceId"
                 }
             },
             "required": [
                 "IndexName",
@@ -5412,39 +5392,31 @@
                 "shape": "ListTrackersResponseEntry"
             },
             "type": "list"
         },
         "MapConfiguration": {
             "documentation": "<p>Specifies the map tile style selected from an available provider.</p>",
             "members": {
-                "CustomLayers": {
-                    "documentation": "<p>Specifies the custom layers for the style. Leave unset to not enable any custom layer, or, for styles that support custom layers, you can enable layer(s), such as <code>POI</code> layer for the VectorEsriNavigation style. Default is <code>unset</code>.</p> <note> <p>Currenlty only <code>VectorEsriNavigation</code> supports CustomLayers. For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#map-custom-layers\">Custom Layers</a>.</p> </note>",
-                    "shape": "CustomLayerList"
-                },
                 "PoliticalView": {
                     "documentation": "<p>Specifies the political view for the style. Leave unset to not use a political view, or, for styles that support specific political views, you can choose a view, such as <code>IND</code> for the Indian view.</p> <p>Default is unset.</p> <note> <p>Not all map resources or styles support political view styles. See <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#political-views\">Political views</a> for more information.</p> </note>",
                     "shape": "CountryCode3"
                 },
                 "Style": {
-                    "documentation": "<p>Specifies the map style selected from an available data provider.</p> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri map styles</a>:</p> <ul> <li> <p> <code>VectorEsriNavigation</code> \u2013 The Esri Navigation map style, which provides a detailed basemap for the world symbolized with a custom navigation map style that's designed for use during the day in mobile devices. It also includes a richer set of places, such as shops, services, restaurants, attractions, and other points of interest. Enable the <code>POI</code> layer by setting it in CustomLayers to leverage the additional places data.</p> <p/> </li> <li> <p> <code>RasterEsriImagery</code> \u2013 The Esri Imagery map style. A raster basemap that provides one meter or better satellite and aerial imagery in many parts of the world and lower resolution satellite imagery worldwide. </p> </li> <li> <p> <code>VectorEsriLightGrayCanvas</code> \u2013 The Esri Light Gray Canvas map style, which provides a detailed vector basemap with a light gray, neutral background style with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>VectorEsriTopographic</code> \u2013 The Esri Light map style, which provides a detailed vector basemap with a classic Esri map style.</p> </li> <li> <p> <code>VectorEsriStreets</code> \u2013 The Esri Street Map style, which provides a detailed vector basemap for the world symbolized with a classic Esri street map style. The vector tile layer is similar in content and style to the World Street Map raster map.</p> </li> <li> <p> <code>VectorEsriDarkGrayCanvas</code> \u2013 The Esri Dark Gray Canvas map style. A vector basemap with a dark gray, neutral background with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies map styles</a>:</p> <ul> <li> <p> <code>VectorHereExplore</code> \u2013 A default HERE map style containing a neutral, global map and its features including roads, buildings, landmarks, and water features. It also now includes a fully designed map of Japan.</p> </li> <li> <p> <code>RasterHereExploreSatellite</code> \u2013 A global map containing high resolution satellite imagery.</p> </li> <li> <p> <code>HybridHereExploreSatellite</code> \u2013 A global map displaying the road network, street names, and city labels over satellite imagery. This style will automatically retrieve both raster and vector tiles, and your charges will be based on total tiles retrieved.</p> <note> <p>Hybrid styles use both vector and raster tiles when rendering the map that you see. This means that more tiles are retrieved than when using either vector or raster tiles alone. Your charges will include all tiles retrieved.</p> </note> </li> <li> <p> <code>VectorHereContrast</code> \u2013 The HERE Contrast (Berlin) map style is a high contrast detailed base map of the world that blends 3D and 2D rendering.</p> <note> <p>The <code>VectorHereContrast</code> style has been renamed from <code>VectorHereBerlin</code>. <code>VectorHereBerlin</code> has been deprecated, but will continue to work in applications that use it.</p> </note> </li> <li> <p> <code>VectorHereExploreTruck</code> \u2013 A global map containing truck restrictions and attributes (e.g. width / height / HAZMAT) symbolized with highlighted segments and icons on top of HERE Explore to support use cases within transport and logistics.</p> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps map styles</a>:</p> <ul> <li> <p> <code>VectorGrabStandardLight</code> \u2013 The Grab Standard Light map style provides a basemap with detailed land use coloring, area names, roads, landmarks, and points of interest covering Southeast Asia.</p> </li> <li> <p> <code>VectorGrabStandardDark</code> \u2013 The Grab Standard Dark map style provides a dark variation of the standard basemap covering Southeast Asia.</p> </li> </ul> <note> <p>Grab provides maps only for countries in Southeast Asia, and is only available in the Asia Pacific (Singapore) Region (<code>ap-southeast-1</code>). For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html#grab-coverage-area\">GrabMaps countries and area covered</a>.</p> </note> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data map styles</a>:</p> <ul> <li> <p> <code>VectorOpenDataStandardLight</code> \u2013 The Open Data Standard Light map style provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataStandardDark</code> \u2013 Open Data Standard Dark is a dark-themed map style that provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataVisualizationLight</code> \u2013 The Open Data Visualization Light map style is a light-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> <li> <p> <code>VectorOpenDataVisualizationDark</code> \u2013 The Open Data Visualization Dark map style is a dark-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> </ul>",
+                    "documentation": "<p>Specifies the map style selected from an available data provider.</p> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/esri.html\">Esri map styles</a>:</p> <ul> <li> <p> <code>VectorEsriDarkGrayCanvas</code> \u2013 The Esri Dark Gray Canvas map style. A vector basemap with a dark gray, neutral background with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>RasterEsriImagery</code> \u2013 The Esri Imagery map style. A raster basemap that provides one meter or better satellite and aerial imagery in many parts of the world and lower resolution satellite imagery worldwide. </p> </li> <li> <p> <code>VectorEsriLightGrayCanvas</code> \u2013 The Esri Light Gray Canvas map style, which provides a detailed vector basemap with a light gray, neutral background style with minimal colors, labels, and features that's designed to draw attention to your thematic content. </p> </li> <li> <p> <code>VectorEsriTopographic</code> \u2013 The Esri Light map style, which provides a detailed vector basemap with a classic Esri map style.</p> </li> <li> <p> <code>VectorEsriStreets</code> \u2013 The Esri Street Map style, which provides a detailed vector basemap for the world symbolized with a classic Esri street map style. The vector tile layer is similar in content and style to the World Street Map raster map.</p> </li> <li> <p> <code>VectorEsriNavigation</code> \u2013 The Esri Navigation map style, which provides a detailed basemap for the world symbolized with a custom navigation map style that's designed for use during the day in mobile devices.</p> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/HERE.html\">HERE Technologies map styles</a>:</p> <ul> <li> <p> <code>VectorHereContrast</code> \u2013 The HERE Contrast (Berlin) map style is a high contrast detailed base map of the world that blends 3D and 2D rendering.</p> <note> <p>The <code>VectorHereContrast</code> style has been renamed from <code>VectorHereBerlin</code>. <code>VectorHereBerlin</code> has been deprecated, but will continue to work in applications that use it.</p> </note> </li> <li> <p> <code>VectorHereExplore</code> \u2013 A default HERE map style containing a neutral, global map and its features including roads, buildings, landmarks, and water features. It also now includes a fully designed map of Japan.</p> </li> <li> <p> <code>VectorHereExploreTruck</code> \u2013 A global map containing truck restrictions and attributes (e.g. width / height / HAZMAT) symbolized with highlighted segments and icons on top of HERE Explore to support use cases within transport and logistics.</p> </li> <li> <p> <code>RasterHereExploreSatellite</code> \u2013 A global map containing high resolution satellite imagery.</p> </li> <li> <p> <code>HybridHereExploreSatellite</code> \u2013 A global map displaying the road network, street names, and city labels over satellite imagery. This style will automatically retrieve both raster and vector tiles, and your charges will be based on total tiles retrieved.</p> <note> <p>Hybrid styles use both vector and raster tiles when rendering the map that you see. This means that more tiles are retrieved than when using either vector or raster tiles alone. Your charges will include all tiles retrieved.</p> </note> </li> </ul> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html\">GrabMaps map styles</a>:</p> <ul> <li> <p> <code>VectorGrabStandardLight</code> \u2013 The Grab Standard Light map style provides a basemap with detailed land use coloring, area names, roads, landmarks, and points of interest covering Southeast Asia.</p> </li> <li> <p> <code>VectorGrabStandardDark</code> \u2013 The Grab Standard Dark map style provides a dark variation of the standard basemap covering Southeast Asia.</p> </li> </ul> <note> <p>Grab provides maps only for countries in Southeast Asia, and is only available in the Asia Pacific (Singapore) Region (<code>ap-southeast-1</code>). For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/grab.html#grab-coverage-area\">GrabMaps countries and area covered</a>.</p> </note> <p>Valid <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/open-data.html\">Open Data map styles</a>:</p> <ul> <li> <p> <code>VectorOpenDataStandardLight</code> \u2013 The Open Data Standard Light map style provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataStandardDark</code> \u2013 Open Data Standard Dark is a dark-themed map style that provides a detailed basemap for the world suitable for website and mobile application use. The map includes highways major roads, minor roads, railways, water features, cities, parks, landmarks, building footprints, and administrative boundaries.</p> </li> <li> <p> <code>VectorOpenDataVisualizationLight</code> \u2013 The Open Data Visualization Light map style is a light-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> <li> <p> <code>VectorOpenDataVisualizationDark</code> \u2013 The Open Data Visualization Dark map style is a dark-themed style with muted colors and fewer features that aids in understanding overlaid data.</p> </li> </ul>",
                     "shape": "MapStyle"
                 }
             },
             "required": [
                 "Style"
             ],
             "type": "structure"
         },
         "MapConfigurationUpdate": {
             "documentation": "<p>Specifies the political view for the style.</p>",
             "members": {
-                "CustomLayers": {
-                    "documentation": "<p>Specifies the custom layers for the style. Leave unset to not enable any custom layer, or, for styles that support custom layers, you can enable layer(s), such as <code>POI</code> layer for the VectorEsriNavigation style. Default is <code>unset</code>.</p> <note> <p>Currenlty only <code>VectorEsriNavigation</code> supports CustomLayers. For more information, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#map-custom-layers\">Custom Layers</a>.</p> </note>",
-                    "shape": "CustomLayerList"
-                },
                 "PoliticalView": {
                     "documentation": "<p>Specifies the political view for the style. Set to an empty string to not use a political view, or, for styles that support specific political views, you can choose a view, such as <code>IND</code> for the Indian view.</p> <note> <p>Not all map resources or styles support political view styles. See <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/map-concepts.html#political-views\">Political views</a> for more information.</p> </note>",
                     "shape": "CountryCode3OrEmpty"
                 }
             },
             "type": "structure"
         },
@@ -5504,15 +5476,15 @@
                     "shape": "String"
                 },
                 "Street": {
                     "documentation": "<p>The name for a street or a road to identify a location. For example, <code>Main Street</code>.</p>",
                     "shape": "String"
                 },
                 "SubMunicipality": {
-                    "documentation": "<p>An area that's part of a larger municipality. For example, <code>Blissville</code> is a submunicipality in the Queen County in New York.</p> <note> <p>This property is only returned for a place index that uses Esri as a data provider. The property is represented as a <code>district</code>.</p> </note> <p>For more information about data providers, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/what-is-data-provider.html\">Amazon Location Service data providers</a>.</p>",
+                    "documentation": "<p>An area that's part of a larger municipality. For example, <code>Blissville </code> is a submunicipality in the Queen County in New York.</p> <note> <p>This property supported by Esri and OpenData. The Esri property is <code>district</code>, and the OpenData property is <code>borough</code>.</p> </note>",
                     "shape": "String"
                 },
                 "SubRegion": {
                     "documentation": "<p>A county, or an area that's part of a larger region. For example, <code>Metro Vancouver</code>.</p>",
                     "shape": "String"
                 },
                 "SupplementalCategories": {
@@ -5520,19 +5492,19 @@
                     "shape": "PlaceSupplementalCategoryList"
                 },
                 "TimeZone": {
                     "documentation": "<p>The time zone in which the <code>Place</code> is located. Returned only when using HERE or Grab as the selected partner.</p>",
                     "shape": "TimeZone"
                 },
                 "UnitNumber": {
-                    "documentation": "<p>For addresses with multiple units, the unit identifier. Can include numbers and letters, for example <code>3B</code> or <code>Unit 123</code>.</p> <note> <p>This property is returned only for a place index that uses Esri or Grab as a data provider. It is not returned for <code>SearchPlaceIndexForPosition</code>.</p> </note>",
+                    "documentation": "<p>For addresses with multiple units, the unit identifier. Can include numbers and letters, for example <code>3B</code> or <code>Unit 123</code>.</p> <note> <p>Returned only for a place index that uses Esri or Grab as a data provider. Is not returned for <code>SearchPlaceIndexForPosition</code>.</p> </note>",
                     "shape": "String"
                 },
                 "UnitType": {
-                    "documentation": "<p>For addresses with a <code>UnitNumber</code>, the type of unit. For example, <code>Apartment</code>.</p> <note> <p>This property is returned only for a place index that uses Esri as a data provider.</p> </note>",
+                    "documentation": "<p>For addresses with a <code>UnitNumber</code>, the type of unit. For example, <code>Apartment</code>.</p> <note> <p>Returned only for a place index that uses Esri as a data provider.</p> </note>",
                     "shape": "String"
                 }
             },
             "required": [
                 "Geometry"
             ],
             "type": "structure"
@@ -5840,15 +5812,15 @@
             "documentation": "<p>Contains a place suggestion resulting from a place suggestion query that is run on a place index resource.</p>",
             "members": {
                 "Categories": {
                     "documentation": "<p>The Amazon Location categories that describe the Place.</p> <p>For more information about using categories, including a list of Amazon Location categories, see <a href=\"https://docs.aws.amazon.com/location/latest/developerguide/category-filtering.html\">Categories and filtering</a>, in the <i>Amazon Location Service Developer Guide</i>.</p>",
                     "shape": "PlaceCategoryList"
                 },
                 "PlaceId": {
-                    "documentation": "<p>The unique identifier of the Place. You can use this with the <code>GetPlace</code> operation to find the place again later, or to get full information for the Place.</p> <p>The <code>GetPlace</code> request must use the same <code>PlaceIndex</code> resource as the <code>SearchPlaceIndexForSuggestions</code> that generated the Place ID.</p> <note> <p>For <code>SearchPlaceIndexForSuggestions</code> operations, the <code>PlaceId</code> is returned by place indexes that use Esri, Grab, or HERE as data providers.</p> </note> <p>While you can use PlaceID in subsequent requests, PlaceID is not intended to be a permanent identifier and the ID can change between consecutive API calls. Please see the following PlaceID behaviour for each data provider:</p> <ul> <li> <p>Esri: Place IDs will change every quarter at a minimum. The typical time period for these changes would be March, June, September, and December. Place IDs might also change between the typical quarterly change but that will be much less frequent.</p> </li> <li> <p>HERE: We recommend that you cache data for no longer than a week to keep your data data fresh. You can assume that less than 1% ID shifts will release over release which is approximately 1 - 2 times per week.</p> </li> <li> <p>Grab: Place IDs can expire or become invalid in the following situations.</p> <ul> <li> <p>Data operations: The POI may be removed from Grab POI database by Grab Map Ops based on the ground-truth, such as being closed in the real world, being detected as a duplicate POI, or having incorrect information. Grab will synchronize data to the Waypoint environment on weekly basis.</p> </li> <li> <p>Interpolated POI: Interpolated POI is a temporary POI generated in real time when serving a request, and it will be marked as derived in the <code>place.result_type</code> field in the response. The information of interpolated POIs will be retained for at least 30 days, which means that within 30 days, you are able to obtain POI details by Place ID from Place Details API. After 30 days, the interpolated POIs(both Place ID and details) may expire and inaccessible from the Places Details API.</p> </li> </ul> </li> </ul>",
+                    "documentation": "<p>The unique identifier of the Place. You can use this with the <code>GetPlace</code> operation to find the place again later, or to get full information for the Place.</p> <p>The <code>GetPlace</code> request must use the same <code>PlaceIndex</code> resource as the <code>SearchPlaceIndexForSuggestions</code> that generated the Place ID.</p> <note> <p>For <code>SearchPlaceIndexForSuggestions</code> operations, the <code>PlaceId</code> is returned by place indexes that use Esri, Grab, or HERE as data providers.</p> </note>",
                     "shape": "PlaceId"
                 },
                 "SupplementalCategories": {
                     "documentation": "<p>Categories from the data provider that describe the Place that are not mapped to any Amazon Location categories.</p>",
                     "shape": "PlaceSupplementalCategoryList"
                 },
                 "Text": {
```

### Comparing `botocore-a-la-carte-location-1.34.82/botocore_a_la_carte_location.egg-info/PKG-INFO` & `botocore-a-la-carte-location-1.34.9/botocore_a_la_carte_location.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-location
-Version: 1.34.82
+Version: 1.34.9
 Summary: location data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-location-1.34.82/setup.py` & `botocore-a-la-carte-location-1.34.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-location',
-    version="1.34.82",
+    version="1.34.9",
     description='location data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/location/*/*.json'],
```

