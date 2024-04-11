# Comparing `tmp/mdapi-3.1.5.tar.gz` & `tmp/mdapi-3.1.6a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdapi-3.1.5.tar", max compression
+gzip compressed data, was "mdapi-3.1.6a1.tar", max compression
```

## Comparing `mdapi-3.1.5.tar` & `mdapi-3.1.6a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-04-02 06:10:16.763448 mdapi-3.1.5/LICENSE
--rw-r--r--   0        0        0     6010 2024-04-02 06:10:16.764448 mdapi-3.1.5/README.md
--rw-r--r--   0        0        0     2452 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/__init__.py
--rw-r--r--   0        0        0      878 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/confdata/__init__.py
--rw-r--r--   0        0        0     1357 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/confdata/servlogr.py
--rw-r--r--   0        0        0     2447 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/confdata/standard.py
--rw-r--r--   0        0        0      878 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/database/__init__.py
--rw-r--r--   0        0        0     5746 2024-04-08 07:42:05.217644 mdapi-3.1.5/mdapi/database/base.py
--rw-r--r--   0        0        0    11603 2024-04-08 07:42:05.218644 mdapi-3.1.5/mdapi/database/main.py
--rw-r--r--   0        0        0     4421 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/database/sqlq.py
--rw-r--r--   0        0        0     2439 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/main.py
--rw-r--r--   0        0        0     7359 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/services/__init__.py
--rw-r--r--   0        0        0     2535 2024-04-02 06:10:16.764448 mdapi-3.1.5/mdapi/services/apimodel.py
--rw-r--r--   0        0        0     4264 2024-04-08 07:42:05.219644 mdapi-3.1.5/mdapi/services/appviews.py
--rw-r--r--   0        0        0     5581 2024-04-08 07:50:54.158037 mdapi-3.1.5/mdapi/services/homepage.html
--rw-r--r--   0        0        0     2811 2024-04-02 06:10:16.765448 mdapi-3.1.5/mdapi/services/main.py
--rw-r--r--   0        0        0     2219 2024-04-08 07:50:54.158037 mdapi-3.1.5/pyproject.toml
--rw-r--r--   0        0        0     7941 1970-01-01 00:00:00.000000 mdapi-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 06:10:16.763448 mdapi-3.1.6a1/LICENSE
+-rw-r--r--   0        0        0     6010 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/README.md
+-rw-r--r--   0        0        0     2452 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/mdapi/__init__.py
+-rw-r--r--   0        0        0      878 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/mdapi/confdata/__init__.py
+-rw-r--r--   0        0        0     1357 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/mdapi/confdata/servlogr.py
+-rw-r--r--   0        0        0     2447 2024-04-08 07:42:05.217644 mdapi-3.1.6a1/mdapi/confdata/standard.py
+-rw-r--r--   0        0        0      878 2024-04-08 07:42:05.217644 mdapi-3.1.6a1/mdapi/database/__init__.py
+-rw-r--r--   0        0        0     5746 2024-04-08 07:42:05.217644 mdapi-3.1.6a1/mdapi/database/base.py
+-rw-r--r--   0        0        0    11603 2024-04-11 03:48:46.488190 mdapi-3.1.6a1/mdapi/database/main.py
+-rw-r--r--   0        0        0     4421 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/mdapi/database/sqlq.py
+-rw-r--r--   0        0        0     2439 2024-04-08 07:42:05.219644 mdapi-3.1.6a1/mdapi/main.py
+-rw-r--r--   0        0        0     7359 2024-04-08 07:42:05.219644 mdapi-3.1.6a1/mdapi/services/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-02 06:10:16.764448 mdapi-3.1.6a1/mdapi/services/apimodel.py
+-rw-r--r--   0        0        0     4264 2024-04-08 07:42:05.219644 mdapi-3.1.6a1/mdapi/services/appviews.py
+-rw-r--r--   0        0        0     5583 2024-04-11 03:59:13.640038 mdapi-3.1.6a1/mdapi/services/homepage.html
+-rw-r--r--   0        0        0     2811 2024-04-02 06:10:16.765448 mdapi-3.1.6a1/mdapi/services/main.py
+-rw-r--r--   0        0        0     2221 2024-04-11 03:58:08.474434 mdapi-3.1.6a1/pyproject.toml
+-rw-r--r--   0        0        0     7943 1970-01-01 00:00:00.000000 mdapi-3.1.6a1/PKG-INFO
```

### Comparing `mdapi-3.1.5/LICENSE` & `mdapi-3.1.6a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/README.md` & `mdapi-3.1.6a1/README.md`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/__init__.py` & `mdapi-3.1.6a1/mdapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/confdata/__init__.py` & `mdapi-3.1.6a1/mdapi/confdata/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/confdata/servlogr.py` & `mdapi-3.1.6a1/mdapi/confdata/servlogr.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/confdata/standard.py` & `mdapi-3.1.6a1/mdapi/confdata/standard.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/database/__init__.py` & `mdapi-3.1.6a1/mdapi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/database/base.py` & `mdapi-3.1.6a1/mdapi/database/base.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/database/main.py` & `mdapi-3.1.6a1/mdapi/database/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     stable_releases = list_branches(status="Active")
     for rels in stable_releases:
         if rels["status"] != "Active":
             continue
         versdata = rels["version"]
         for jndx, urli in enumerate(urls[rels["name"]]):
             if rels["name"] in ("Fedora Linux", "Fedora"):
-                name = repodict["fedora"][jndx].format(ridx = rels["koji_name"])
+                name = repodict["fedora"][jndx].format(rlid = rels["koji_name"])
             elif rels["name"] == "Fedora EPEL" and versdata == "8":
                 name = repodict["epel"][jndx].format(rlid = rels["koji_name"])
                 urli = urli.replace("/x86_64/", "/Everything/x86_64/")
             elif rels["name"] == "Fedora EPEL" and versdata == "9":
                 name = repodict["epel"][jndx].format(rlid = rels["koji_name"])
                 urli = urli.replace("/x86_64/", "/Everything/x86_64/")
             else:
```

### Comparing `mdapi-3.1.5/mdapi/database/sqlq.py` & `mdapi-3.1.6a1/mdapi/database/sqlq.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/main.py` & `mdapi-3.1.6a1/mdapi/main.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/services/__init__.py` & `mdapi-3.1.6a1/mdapi/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/services/apimodel.py` & `mdapi-3.1.6a1/mdapi/services/apimodel.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/services/appviews.py` & `mdapi-3.1.6a1/mdapi/services/appviews.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/mdapi/services/homepage.html` & `mdapi-3.1.6a1/mdapi/services/homepage.html`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 | '_ ` _ \ / _` |/ _` | '_ \| |
 | | | | | | (_| | (_| | |_) | |
 |_| |_| |_|\__,_|\__,_| .__/|_|
                       | |
                       |_|
 
 
-<a href="https://pypi.org/project/mdapi/3.1.5/">mdapi</a> is a small API exposing the metadata contained in different RPM
+<a href="https://pypi.org/project/mdapi/3.1.6a1/">mdapi</a> is a small API exposing the metadata contained in different RPM
 repositories.
 
 mdapi has access to the metadata of the different Fedora repositories and will
 serve you the most recent information available, from updates-testing, if
 there is nothing in updates-testing, it will look for information from the
 updates repository and if there is still nothing, it will look for information
 in the releases repository.
```

### Comparing `mdapi-3.1.5/mdapi/services/main.py` & `mdapi-3.1.6a1/mdapi/services/main.py`

 * *Files identical despite different names*

### Comparing `mdapi-3.1.5/pyproject.toml` & `mdapi-3.1.6a1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdapi"
-version = "3.1.5"
+version = "3.1.6a1"
 description = "A simple API for serving the metadata from the RPM repositories"
 authors = ["Pierre-Yves Chibon <pingou@pingoured.fr>", "Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 license = "GPL-3.0-or-later"
 maintainers = ["Pierre-Yves Chibon <pingou@pingoured.fr>", "Akashdeep Dhar <akashdeep.dhar@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fedora-infra/mdapi"
 repository = "https://github.com/fedora-infra/mdapi"
```

### Comparing `mdapi-3.1.5/PKG-INFO` & `mdapi-3.1.6a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdapi
-Version: 3.1.5
+Version: 3.1.6a1
 Summary: A simple API for serving the metadata from the RPM repositories
 Home-page: https://github.com/fedora-infra/mdapi
 License: GPL-3.0-or-later
 Keywords: rpm,centos,fedora,metadata,repositories
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 Maintainer: Pierre-Yves Chibon
```

