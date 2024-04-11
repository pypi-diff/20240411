# Comparing `tmp/secrules_parsing-0.2.7.tar.gz` & `tmp/secrules_parsing-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secrules_parsing-0.2.7.tar", max compression
+gzip compressed data, was "secrules_parsing-0.2.8.tar", max compression
```

## Comparing `secrules_parsing-0.2.7.tar` & `secrules_parsing-0.2.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/LICENSE
--rw-r--r--   0        0        0     4926 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/README.md
--rw-r--r--   0        0        0     1223 2024-01-26 15:10:23.638985 secrules_parsing-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       76 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/__init__.py
--rw-r--r--   0        0        0     2655 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/cli.py
--rw-r--r--   0        0        0        0 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/model/__init__.py
--rw-r--r--   0        0        0    11835 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/model/secrules.tx
--rwxr-xr-x   0        0        0     3564 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/parser.py
--rw-r--r--   0        0        0      291 2024-01-26 15:10:07.274883 secrules_parsing-0.2.7/src/secrules_parsing/resources.py
--rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 secrules_parsing-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 20:35:22.470623 secrules_parsing-0.2.8/LICENSE
+-rw-r--r--   0        0        0     4926 2024-04-10 20:35:22.470623 secrules_parsing-0.2.8/README.md
+-rw-r--r--   0        0        0     1223 2024-04-10 20:35:36.918624 secrules_parsing-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/__init__.py
+-rw-r--r--   0        0        0     2655 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/model/__init__.py
+-rw-r--r--   0        0        0    11744 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/model/secrules.tx
+-rwxr-xr-x   0        0        0     3564 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/parser.py
+-rw-r--r--   0        0        0      291 2024-04-10 20:35:22.474623 secrules_parsing-0.2.8/src/secrules_parsing/resources.py
+-rw-r--r--   0        0        0     6122 1970-01-01 00:00:00.000000 secrules_parsing-0.2.8/PKG-INFO
```

### Comparing `secrules_parsing-0.2.7/LICENSE` & `secrules_parsing-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.7/README.md` & `secrules_parsing-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.7/pyproject.toml` & `secrules_parsing-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secrules-parsing"
-version = "v0.2.7"
+version = "v0.2.8"
 description = "ModSecurity DSL Parser package using textX"
 authors = [
     "Felipe Zipitria <felipe.zipitria@owasp.org>"
 ]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/coreruleset/secrules_parsing"
```

### Comparing `secrules_parsing-0.2.7/src/secrules_parsing/cli.py` & `secrules_parsing-0.2.8/src/secrules_parsing/cli.py`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.7/src/secrules_parsing/model/secrules.tx` & `secrules_parsing-0.2.8/src/secrules_parsing/model/secrules.tx`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     idlist+=INT | range=IDRange;
 
 /*
 There is no check against collections existance, or typying between variables and value (e.g: TIME_DAY and its referred value must be equal to some integer)
 FILES is a collection, so it doesn't belong here
 */
 Variable:
-    '!'? ('ARGS_COMBINED_SIZE' | 'ARGS_GET_NAMES' | 'ARGS_NAMES' | 'ARGS_POST_NAMES' |
+    '!'? '&'? ('ARGS_COMBINED_SIZE' | 'ARGS_GET_NAMES' | 'ARGS_NAMES' | 'ARGS_POST_NAMES' |
     'AUTH_TYPE' | 'DURATION' | 'FILES_COMBINED_SIZE' | 'FILES_NAMES' | 'FILES' | 
     'FULL_REQUEST' | 'FULL_REQUEST_LENGTH' | 'FILES_SIZES' | 'FILES_TMPNAMES' | 
     'FILES_TMP_CONTENT' | 'HIGHEST_SEVERITY' | 'INBOUND_DATA_ERROR' | 'MATCHED_VAR_NAME' |
     'MODSEC_BUILD' | 'MULTIPART_CRLF_LF_LINES' | 'MULTIPART_FILENAME' | 'MULTIPART_NAME' |
     'MULTIPART_STRICT_ERROR' | 'MULTIPART_UNMATCHED_BOUNDARY' | 'OUTBOUND_DATA_ERROR' | 
     'PATH_INFO' | 'PERF_ALL' | 'PERF_COMBINED' | 'PERF_GC' | 'PERF_LOGGING' | 'PERF_PHASE1' |
     'PERF_PHASE2' | 'PERF_PHASE3' | 'PERF_PHASE4' | 'PERF_PHASE5' | 'PERF_SREAD' | 'PERF_SWRITE' |
@@ -65,19 +65,17 @@
     'RESPONSE_BODY' | 'RESPONSE_CONTENT_LENGTH' | 'RESPONSE_CONTENT_TYPE' |
     'RESPONSE_PROTOCOL' | 'RESPONSE_STATUS' | 'RULE' | 'SCRIPT_BASENAME' | 'SCRIPT_FILENAME' |
     'SCRIPT_GID' | 'SCRIPT_GROUPNAME' | 'SCRIPT_MODE' | 'SCRIPT_UID' | 'SCRIPT_USERNAME' |
     'SDBM_DELETE_ERROR' | 'SERVER_ADDR' | 'SERVER_NAME' | 'SERVER_PORT' | 'SESSION' | 'SESSIONID' |
     'STATUS_LINE' | 'STREAM_INPUT_BODY' | 'STREAM_OUTPUT_BODY' | 'TIME' | 'TIME_DAY' | 'TIME_EPOCH' |
     'TIME_HOUR' | 'TIME_MIN' | 'TIME_MON' | 'TIME_SEC' | 'TIME_WDAY' | 'TIME_YEAR' | 'UNIQUE_ID' |
     'URLENCODED_ERROR' | 'USERID' | 'USERAGENT_IP' | 'WEBAPPID' | 'WEBSERVER_ERROR_LOG' |
-    count=Count? collection=CollectionName ':'? collectionArg=CollectionArgument?) |
+    collection=CollectionName ':'? collectionArg=CollectionArgument?) |
     SpecialCollection | 'MATCHED_VAR';
 
-CollectionCount: '&' collection=CollectionName ':' VariableName;
-    
 VariableOrCollection: Variable | CollectionName;
     
 //    CollectionArgument: AnythingBetweenSlashes | "'"? '/' SlashedRegExp '/' "'"? | VariableName;
 CollectionArgument: AnythingBetweenSingleQuotes | '/' SlashedRegExp '/' | VariableName;
     
 /* Collections */
 CollectionName:
@@ -90,16 +88,14 @@
 SpecialCollection: 'XML' ':' XPathExpression;
 
 XPathExpression: /(\/\*|\/\/@\*)/;
 
 AnythingBetweenSlashes: /(\*|\\\/)+/;
 AnythingBetweenSingleQuotes: /\'.+\'/;
     
-Count: '&';
-
 //- pattern match (pm/pmf)    
 Operator:
     ('beginsWith' beginswith=PathOrMacro | 'contains' contains=PatternMatch | 'containsWord' containsWord=STRING |
     detectsqli ?= 'detectSQLi' | detectxss ?= 'detectXSS' | 'endsWith' endswith=ExtendedMacro |
     'fuzzyHash' fuzzyhash=STRING | 'eq' eq=INT | 'ge' ge=Macro | geolookup ?= 'geoLookup'  |
     'gsbLookup' gsblookup=INT | 'gt' gt=Macro | 'inspectFile' inspectfile=URI | 'ipMatch' ipmatch+=IPCIDR[','] |
     'ipMatchF' ipmatchf=STRING | 'ipMatchFromFile' ipmatchfromfile=STRING | 'le' le=INT | 'lt' lt=Macro |
```

### Comparing `secrules_parsing-0.2.7/src/secrules_parsing/parser.py` & `secrules_parsing-0.2.8/src/secrules_parsing/parser.py`

 * *Files identical despite different names*

### Comparing `secrules_parsing-0.2.7/PKG-INFO` & `secrules_parsing-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secrules-parsing
-Version: 0.2.7
+Version: 0.2.8
 Summary: ModSecurity DSL Parser package using textX
 Home-page: https://github.com/coreruleset/secrules_parsing
 License: Apache-2.0
 Keywords: secrule,modsecurity,parser,textX
 Author: Felipe Zipitria
 Author-email: felipe.zipitria@owasp.org
 Requires-Python: >=3.7,<4.0
```

