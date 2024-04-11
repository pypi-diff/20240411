# Comparing `tmp/mpcontribs-client-5.8.2.tar.gz` & `tmp/mpcontribs-client-5.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.8.2.tar", last modified: Tue Apr  9 23:44:44 2024, max compression
+gzip compressed data, was "mpcontribs-client-5.8.3.tar", last modified: Thu Apr 11 01:19:56 2024, max compression
```

## Comparing `mpcontribs-client-5.8.2.tar` & `mpcontribs-client-5.8.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.145999 mpcontribs-client-5.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.137999 mpcontribs-client-5.8.2/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    96696 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-09 23:44:44.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-09 23:44:43.000000 mpcontribs-client-5.8.2/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:44:44.145999 mpcontribs-client-5.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:44:44.141999 mpcontribs-client-5.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-09 23:44:33.000000 mpcontribs-client-5.8.2/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.264024 mpcontribs-client-5.8.3/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.264024 mpcontribs-client-5.8.3/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    96703 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-11 01:19:55.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-11 01:19:56.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:19:55.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:19:55.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 01:19:55.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 01:19:55.000000 mpcontribs-client-5.8.3/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:19:56.268024 mpcontribs-client-5.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-11 01:19:46.000000 mpcontribs-client-5.8.3/tests/test_client.py
```

### Comparing `mpcontribs-client-5.8.2/LICENSE` & `mpcontribs-client-5.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/PKG-INFO` & `mpcontribs-client-5.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.8.2
+Version: 5.8.3
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.8.2/README.md` & `mpcontribs-client-5.8.3/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/mpcontribs/client/__init__.py` & `mpcontribs-client-5.8.3/mpcontribs/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 MAX_PAYLOAD = 15 * MEGABYTES
 MAX_COLUMNS = 160
 DEFAULT_HOST = "contribs-api.materialsproject.org"
 BULMA = "is-narrow is-fullwidth has-background-light"
 PROVIDERS = {"github", "google", "facebook", "microsoft", "amazon"}
 COMPONENTS = ["structures", "tables", "attachments"]  # using list to maintain order
 SUBDOMAINS = ["contribs", "ml", "micro"]
-PORTS = [5000, 5002, 5003, 5005, 10000, 10002, 10003, 10005, 20000]
+PORTS = [5000, 5002, 5003, 5005, 10000, 10002, 10003, 10005, 20000, 20005]
 HOSTS = ["localhost", "contribs-apis"]
 HOSTS += [f"192.168.0.{i}" for i in range(36, 47)]  # PrivateSubnetOne
 HOSTS += [f"192.168.0.{i}" for i in range(52, 63)]  # PrivateSubnetTwo
 VALID_URLS = {f"http://{h}:{p}" for p in PORTS for h in HOSTS}
 VALID_URLS |= {
     f"https://{n}-api{m}.materialsproject.org"
     for n in SUBDOMAINS
```

### Comparing `mpcontribs-client-5.8.2/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.8.3/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.8.2
+Version: 5.8.3
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.8.2/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.8.3/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,13 +7,15 @@
 mpcontribs_client.egg-info/dependency_links.txt
 mpcontribs_client.egg-info/not-zip-safe
 mpcontribs_client.egg-info/requires.txt
 mpcontribs_client.egg-info/top_level.txt
 requirements/deployment.txt
 requirements/ubuntu-latest_py3.10.txt
 requirements/ubuntu-latest_py3.10_extras.txt
+requirements/ubuntu-latest_py3.11.txt
+requirements/ubuntu-latest_py3.11_extras.txt
 requirements/ubuntu-latest_py3.8.txt
 requirements/ubuntu-latest_py3.8_extras.txt
 requirements/ubuntu-latest_py3.9.txt
 requirements/ubuntu-latest_py3.9_extras.txt
 tests/conftest.py
 tests/test_client.py
```

### Comparing `mpcontribs-client-5.8.2/requirements/deployment.txt` & `mpcontribs-client-5.8.3/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.10.txt`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     #   requests
 ipython==8.23.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
@@ -86,15 +86,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
```

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     # via pytest
 ipython==8.23.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.19.1
     # via ipython
-joblib==1.3.2
+joblib==1.4.0
     # via pymatgen
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
 jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
@@ -98,15 +98,15 @@
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.8
     # via
     #   bravado
     #   bravado-core
-networkx==3.2.1
+networkx==3.3
     # via pymatgen
 numpy==1.26.4
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
```

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.8.3/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/setup.py` & `mpcontribs-client-5.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.8.2/tests/test_client.py` & `mpcontribs-client-5.8.3/tests/test_client.py`

 * *Files identical despite different names*

