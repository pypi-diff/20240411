# Comparing `tmp/bitrix24-rest-motexc-1.1.4b1.tar.gz` & `tmp/bitrix24-rest-motexc-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitrix24-rest-motexc-1.1.4b1.tar", last modified: Thu Jan 25 10:27:47 2024, max compression
+gzip compressed data, was "bitrix24-rest-motexc-1.1.5.tar", last modified: Thu Apr 11 13:53:11 2024, max compression
```

## Comparing `bitrix24-rest-motexc-1.1.4b1.tar` & `bitrix24-rest-motexc-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 10:27:47.732384 bitrix24-rest-motexc-1.1.4b1/
--rw-rw-rw-   0        0        0     1093 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/LICENSE
--rw-rw-rw-   0        0        0       54 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/MANIFEST.in
--rw-rw-rw-   0        0        0     2850 2024-01-25 10:27:47.730386 bitrix24-rest-motexc-1.1.4b1/PKG-INFO
--rw-rw-rw-   0        0        0     1373 2024-01-19 08:31:37.000000 bitrix24-rest-motexc-1.1.4b1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 10:27:47.702377 bitrix24-rest-motexc-1.1.4b1/bitrix24/
--rw-rw-rw-   0        0        0      965 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24/__init__.py
--rw-rw-rw-   0        0        0     4689 2024-01-25 10:26:59.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24/bitrix24.py
--rw-rw-rw-   0        0        0      353 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-25 10:27:47.727394 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/
--rw-rw-rw-   0        0        0     2850 2024-01-25 10:27:47.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-01-25 10:27:47.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 10:27:47.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-25 10:27:47.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-01-25 10:27:47.000000 bitrix24-rest-motexc-1.1.4b1/bitrix24_rest_motexc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 10:27:47.732384 bitrix24-rest-motexc-1.1.4b1/setup.cfg
--rw-rw-rw-   0        0        0     2820 2024-01-25 10:25:56.000000 bitrix24-rest-motexc-1.1.4b1/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-25 10:27:47.723378 bitrix24-rest-motexc-1.1.4b1/tests/
--rw-rw-rw-   0        0        0        0 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/tests/__init__.py
--rw-rw-rw-   0        0        0     2994 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.4b1/tests/test_bitrix24.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:53:11.114243 bitrix24-rest-motexc-1.1.5/
+-rw-rw-rw-   0        0        0     1093 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       54 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2184 2024-04-11 13:53:11.112241 bitrix24-rest-motexc-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1373 2024-01-19 08:31:37.000000 bitrix24-rest-motexc-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 13:53:11.069680 bitrix24-rest-motexc-1.1.5/bitrix24/
+-rw-rw-rw-   0        0        0      965 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/bitrix24/__init__.py
+-rw-rw-rw-   0        0        0     4696 2024-04-11 13:51:26.000000 bitrix24-rest-motexc-1.1.5/bitrix24/bitrix24.py
+-rw-rw-rw-   0        0        0      353 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/bitrix24/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:53:11.110240 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/
+-rw-rw-rw-   0        0        0     2184 2024-04-11 13:53:10.000000 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-04-11 13:53:10.000000 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 13:53:10.000000 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 13:53:10.000000 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-11 13:53:10.000000 bitrix24-rest-motexc-1.1.5/bitrix24_rest_motexc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 13:53:11.114243 bitrix24-rest-motexc-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2163 2024-04-11 13:52:25.000000 bitrix24-rest-motexc-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 13:53:11.107236 bitrix24-rest-motexc-1.1.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     2994 2024-01-19 08:19:53.000000 bitrix24-rest-motexc-1.1.5/tests/test_bitrix24.py
```

### Comparing `bitrix24-rest-motexc-1.1.4b1/LICENSE` & `bitrix24-rest-motexc-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitrix24-rest-motexc-1.1.4b1/README.md` & `bitrix24-rest-motexc-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bitrix24-rest-motexc-1.1.4b1/bitrix24/__init__.py` & `bitrix24-rest-motexc-1.1.5/bitrix24/__init__.py`

 * *Files identical despite different names*

### Comparing `bitrix24-rest-motexc-1.1.4b1/bitrix24/bitrix24.py` & `bitrix24-rest-motexc-1.1.5/bitrix24/bitrix24.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
         try:
             url = '{0}/{1}.json'.format(self.domain, method)
 
             p = self._prepare_params(params)
             m = method.rsplit('.', 1)[1]
 
-            if m not in ['add', 'update', 'delete', 'set']:
+            if m not in ['add', 'update', 'delete', 'set', 'get']:
                 h = {'Content-Type': 'text/text; charset=utf-8'}
                 try:
                     params = params['fields']
                 except:
                     pass
                 r = requests.post(url, data=params, timeout=self.timeout, verify=self.safe, headers=h).json()
             else:
```

### Comparing `bitrix24-rest-motexc-1.1.4b1/tests/test_bitrix24.py` & `bitrix24-rest-motexc-1.1.5/tests/test_bitrix24.py`

 * *Files identical despite different names*

