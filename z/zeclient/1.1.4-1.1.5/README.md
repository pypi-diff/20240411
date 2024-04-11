# Comparing `tmp/zeclient-1.1.4.tar.gz` & `tmp/zeclient-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\python-client\dist\.tmp-al6mc44h\zeclient-1.1.4.tar", last modified: Fri Oct  6 06:45:37 2023, max compression
+gzip compressed data, was "zeclient-1.1.5.tar", last modified: Thu Apr 11 04:07:00 2024, max compression
```

## Comparing `zeclient-1.1.4.tar` & `zeclient-1.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-10-06 06:45:37.000000 zeclient-1.1.4/
--rw-rw-rw-   0        0        0      969 2023-10-06 06:11:53.000000 zeclient-1.1.4/CHANGES.txt
--rw-rw-rw-   0        0        0       32 2023-10-06 06:11:53.000000 zeclient-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0       46 2023-10-06 06:11:53.000000 zeclient-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1181 2023-10-06 06:45:36.000000 zeclient-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-10-06 06:11:53.000000 zeclient-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-10-06 06:45:36.000000 zeclient-1.1.4/docs/
--rw-rw-rw-   0        0        0     9575 2023-10-06 06:11:53.000000 zeclient-1.1.4/docs/odata_user_guide.md
--rw-rw-rw-   0        0        0     7401 2023-10-06 06:11:54.000000 zeclient-1.1.4/docs/rest_user_guide.md
--rw-rw-rw-   0        0        0     6322 2023-10-06 06:11:54.000000 zeclient-1.1.4/docs/soap_proxy_user_guide.md
--rw-rw-rw-   0        0        0     5573 2023-10-06 06:11:54.000000 zeclient-1.1.4/docs/soap_user_guide.md
--rw-rw-rw-   0        0        0     3021 2023-10-06 06:11:54.000000 zeclient-1.1.4/docs/sso_user_guide.md
--rw-rw-rw-   0        0        0    15927 2023-10-06 06:11:54.000000 zeclient-1.1.4/docs/zema_user_guide.md
--rw-rw-rw-   0        0        0      450 2023-10-06 06:11:54.000000 zeclient-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-06 06:45:37.000000 zeclient-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-10-06 06:11:54.000000 zeclient-1.1.4/setup.py
--rw-rw-rw-   0        0        0        1 2023-10-06 06:11:54.000000 zeclient-1.1.4/test.txt
-drwxrwxrwx   0        0        0        0 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient/
--rw-rw-rw-   0        0        0        0 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/__init__.py
--rw-rw-rw-   0        0        0     4976 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/http_client.py
-drwxrwxrwx   0        0        0        0 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient/oauth2/
--rw-rw-rw-   0        0        0        0 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/__init__.py
--rw-rw-rw-   0        0        0      972 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/adfs_authorization_code.py
--rw-rw-rw-   0        0        0     1842 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/adfs_bearer_token.py
--rw-rw-rw-   0        0        0     1310 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/generic_resource_owner_password_flow.py
--rw-rw-rw-   0        0        0     1172 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/keycloak_resource_owner_password.py
--rw-rw-rw-   0        0        0      174 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/oauth2_flow.py
--rw-rw-rw-   0        0        0     1789 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/okta_authorization_code.py
--rw-rw-rw-   0        0        0     1338 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/okta_resource_owner_password.py
--rw-rw-rw-   0        0        0     1290 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/oauth2/ping_authorization_code.py
--rw-rw-rw-   0        0        0     1514 2023-10-06 06:11:53.000000 zeclient-1.1.4/zeclient/oauth2/ping_resource_owner_password.py
--rw-rw-rw-   0        0        0    10567 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/odata_client.py
--rw-rw-rw-   0        0        0    12894 2023-10-06 06:11:53.000000 zeclient-1.1.4/zeclient/rest_client.py
--rw-rw-rw-   0        0        0     7759 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/soap_client.py
--rw-rw-rw-   0        0        0     7423 2023-10-06 06:11:53.000000 zeclient-1.1.4/zeclient/soap_proxy.py
--rw-rw-rw-   0        0        0    11475 2023-10-06 06:11:54.000000 zeclient-1.1.4/zeclient/soap_util.py
--rw-rw-rw-   0        0        0     6301 2023-10-06 06:11:55.000000 zeclient-1.1.4/zeclient/zema_auth.py
--rw-rw-rw-   0        0        0     6988 2023-10-06 06:11:55.000000 zeclient-1.1.4/zeclient/zema_client.py
-drwxrwxrwx   0        0        0        0 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/
--rw-rw-rw-   0        0        0     1181 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-06 06:45:36.000000 zeclient-1.1.4/zeclient.egg-info/top_level.txt
+drwxr-xr-x   0 jingxingguo   (501) staff       (20)        0 2024-04-11 04:07:00.937905 zeclient-1.1.5/
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1057 2024-03-10 22:05:42.000000 zeclient-1.1.5/CHANGES.txt
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)       32 2024-03-10 22:05:40.000000 zeclient-1.1.5/LICENSE.txt
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)       46 2024-03-10 22:05:40.000000 zeclient-1.1.5/MANIFEST.in
+-rw-r--r--   0 jingxingguo   (501) staff       (20)     1523 2024-04-11 04:07:00.937728 zeclient-1.1.5/PKG-INFO
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      848 2024-03-10 22:05:42.000000 zeclient-1.1.5/README.md
+drwxr-xr-x   0 jingxingguo   (501) staff       (20)        0 2024-04-11 04:07:00.933107 zeclient-1.1.5/docs/
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     9575 2024-03-10 22:05:40.000000 zeclient-1.1.5/docs/odata_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     7401 2024-03-10 22:05:40.000000 zeclient-1.1.5/docs/rest_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     6322 2024-03-10 22:05:40.000000 zeclient-1.1.5/docs/soap_proxy_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     5573 2024-03-10 22:05:42.000000 zeclient-1.1.5/docs/soap_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     3021 2024-03-10 22:05:40.000000 zeclient-1.1.5/docs/sso_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)    15927 2024-03-10 22:05:40.000000 zeclient-1.1.5/docs/zema_user_guide.md
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      487 2024-04-11 01:26:34.000000 zeclient-1.1.5/pyproject.toml
+-rw-r--r--   0 jingxingguo   (501) staff       (20)       38 2024-04-11 04:07:00.937943 zeclient-1.1.5/setup.cfg
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      911 2024-04-11 01:26:34.000000 zeclient-1.1.5/setup.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)        1 2024-03-10 22:05:40.000000 zeclient-1.1.5/test.txt
+drwxr-xr-x   0 jingxingguo   (501) staff       (20)        0 2024-04-11 04:07:00.934804 zeclient-1.1.5/zeclient/
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)        0 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/__init__.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     4976 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/http_client.py
+drwxr-xr-x   0 jingxingguo   (501) staff       (20)        0 2024-04-11 04:07:00.937104 zeclient-1.1.5/zeclient/oauth2/
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)        0 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/oauth2/__init__.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      972 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/oauth2/adfs_authorization_code.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1842 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/oauth2/adfs_bearer_token.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1310 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/oauth2/generic_resource_owner_password_flow.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1172 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/oauth2/keycloak_resource_owner_password.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      174 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/oauth2/oauth2_flow.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1789 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/oauth2/okta_authorization_code.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1338 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/oauth2/okta_resource_owner_password.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1290 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/oauth2/ping_authorization_code.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1514 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/oauth2/ping_resource_owner_password.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)    10567 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/odata_client.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)    12894 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/rest_client.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     7759 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/soap_client.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     7423 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/soap_proxy.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)    12149 2024-03-10 22:05:40.000000 zeclient-1.1.5/zeclient/soap_util.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     6301 2024-03-10 22:05:42.000000 zeclient-1.1.5/zeclient/zema_auth.py
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     6988 2024-03-10 22:05:44.000000 zeclient-1.1.5/zeclient/zema_client.py
+drwxr-xr-x   0 jingxingguo   (501) staff       (20)        0 2024-04-11 04:07:00.937288 zeclient-1.1.5/zeclient.egg-info/
+-rw-r--r--   0 jingxingguo   (501) staff       (20)     1523 2024-04-11 04:07:00.000000 zeclient-1.1.5/zeclient.egg-info/PKG-INFO
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)     1025 2024-04-11 04:07:00.000000 zeclient-1.1.5/zeclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)        1 2024-04-11 04:07:00.000000 zeclient-1.1.5/zeclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)      120 2024-04-11 04:07:00.000000 zeclient-1.1.5/zeclient.egg-info/requires.txt
+-rw-rw-r--   0 jingxingguo   (501) staff       (20)        9 2024-04-11 04:07:00.000000 zeclient-1.1.5/zeclient.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `zeclient-1.1.4/CHANGES.txt` & `zeclient-1.1.5/CHANGES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,9 +33,12 @@
 2022-06-02
     1.1.2 added support for generic Resource Owner Password OAuth2 Flow
 
 2023-03-08
     1.1.3 added upload curve data services for REST
           made it available in PyPI - https://pypi.org/project/zeclient
 
-2023-04-11
+2023-11-04
     1.1.4 added "effective_date" parameter for getting profile data
+
+2023-11-22
+    1.1.5 allow soap client method find_curves to return external curves
```

### Comparing `zeclient-1.1.4/README.md` & `zeclient-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/odata_user_guide.md` & `zeclient-1.1.5/docs/odata_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/rest_user_guide.md` & `zeclient-1.1.5/docs/rest_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/soap_proxy_user_guide.md` & `zeclient-1.1.5/docs/soap_proxy_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/soap_user_guide.md` & `zeclient-1.1.5/docs/soap_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/sso_user_guide.md` & `zeclient-1.1.5/docs/sso_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/docs/zema_user_guide.md` & `zeclient-1.1.5/docs/zema_user_guide.md`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/setup.py` & `zeclient-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         'numpy',
         'tabulate',
         'validate_email'
 ]
 
 setup(
     name='zeclient',
-    version='1.1.4',
+    version='1.1.5',
     author='ZE',
     author_email='support@ze.com',
     packages=['zeclient', 'zeclient.oauth2'],
     url='http://www.ze.com',
     license='LICENSE.txt',
     description='Python APIs for ZE Web Services.',
     long_description=open('README.md').read(),
```

### Comparing `zeclient-1.1.4/zeclient/http_client.py` & `zeclient-1.1.5/zeclient/http_client.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/adfs_authorization_code.py` & `zeclient-1.1.5/zeclient/oauth2/adfs_authorization_code.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/adfs_bearer_token.py` & `zeclient-1.1.5/zeclient/oauth2/adfs_bearer_token.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/generic_resource_owner_password_flow.py` & `zeclient-1.1.5/zeclient/oauth2/generic_resource_owner_password_flow.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/keycloak_resource_owner_password.py` & `zeclient-1.1.5/zeclient/oauth2/keycloak_resource_owner_password.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/okta_authorization_code.py` & `zeclient-1.1.5/zeclient/oauth2/okta_authorization_code.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/okta_resource_owner_password.py` & `zeclient-1.1.5/zeclient/oauth2/okta_resource_owner_password.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/ping_authorization_code.py` & `zeclient-1.1.5/zeclient/oauth2/ping_authorization_code.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/oauth2/ping_resource_owner_password.py` & `zeclient-1.1.5/zeclient/oauth2/ping_resource_owner_password.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/odata_client.py` & `zeclient-1.1.5/zeclient/odata_client.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/rest_client.py` & `zeclient-1.1.5/zeclient/rest_client.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/soap_client.py` & `zeclient-1.1.5/zeclient/soap_client.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/soap_proxy.py` & `zeclient-1.1.5/zeclient/soap_proxy.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/soap_util.py` & `zeclient-1.1.5/zeclient/soap_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,37 +99,49 @@
     for c in columns:
         df[c] = []
     
     names = {}
     
     for b in result:                
         for p in b.profiles:
-            if len(p.observations) == 0:
+            if p is None:
                 df[columns[0]].append(b.owner)
                 df[columns[1]].append(b.groupName)
                 df[columns[2]].append(b.name)
                 df[columns[3]].append(b.id)
                 df[columns[4]].append(b.dataType)
-                df[columns[5]].append(p.profileName)
-                df[columns[6]].append(p.configName)
+                df[columns[5]].append(None)
+                df[columns[6]].append(None)
                 df[columns[7]].append('')
                 df[columns[8]].append(b.granularity)
                 df[columns[9]].append('')
             else:
-                for o in p.observations:
+                if len(p.observations) == 0:
                     df[columns[0]].append(b.owner)
                     df[columns[1]].append(b.groupName)
                     df[columns[2]].append(b.name)
                     df[columns[3]].append(b.id)
                     df[columns[4]].append(b.dataType)
                     df[columns[5]].append(p.profileName)
                     df[columns[6]].append(p.configName)
-                    df[columns[7]].append(o.curveType)
-                    df[columns[8]].append(o.granularity)
-                    df[columns[9]].append(o.dataType)
+                    df[columns[7]].append('')
+                    df[columns[8]].append(b.granularity)
+                    df[columns[9]].append('')
+                else:
+                    for o in p.observations:
+                        df[columns[0]].append(b.owner)
+                        df[columns[1]].append(b.groupName)
+                        df[columns[2]].append(b.name)
+                        df[columns[3]].append(b.id)
+                        df[columns[4]].append(b.dataType)
+                        df[columns[5]].append(p.profileName)
+                        df[columns[6]].append(p.configName)
+                        df[columns[7]].append(o.curveType)
+                        df[columns[8]].append(o.granularity)
+                        df[columns[9]].append(o.dataType)
         
         if len(b.properties) > 0:
             for pp in b.properties:
                 if pp.label in names:
                     names[pp.label] += 1
                 else:
                     names[pp.label] = 1
@@ -143,19 +155,20 @@
     
     # only include properties assigned to all available curves
     if len(valid_names) > 0:
         for b in result:
             for pp in b.properties:
                 if pp.label in valid_names:
                     for p in b.profiles:
-                        if len(p.observations) == 0:
-                            df[pp.label].append(pp.value)
-                        else:
-                            for o in p.observations:
+                        if p is not None:
+                            if len(p.observations) == 0:
                                 df[pp.label].append(pp.value)
+                            else:
+                                for o in p.observations:
+                                    df[pp.label].append(pp.value)
         
     return pd.DataFrame.from_dict(df)
     
 def print_curve_data_bean(result):
     for r in result:
         print('Curve name: %s' % r.curveName)
         print('Opr date: %s' % r.oprDate)
```

### Comparing `zeclient-1.1.4/zeclient/zema_auth.py` & `zeclient-1.1.5/zeclient/zema_auth.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient/zema_client.py` & `zeclient-1.1.5/zeclient/zema_client.py`

 * *Files identical despite different names*

### Comparing `zeclient-1.1.4/zeclient.egg-info/SOURCES.txt` & `zeclient-1.1.5/zeclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

