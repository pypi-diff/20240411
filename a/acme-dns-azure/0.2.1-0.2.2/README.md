# Comparing `tmp/acme_dns_azure-0.2.1.tar.gz` & `tmp/acme_dns_azure-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acme_dns_azure-0.2.1.tar", max compression
+gzip compressed data, was "acme_dns_azure-0.2.2.tar", max compression
```

## Comparing `acme_dns_azure-0.2.1.tar` & `acme_dns_azure-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1094 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/LICENSE
--rw-r--r--   0        0        0     7438 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/README.md
--rw-r--r--   0        0        0      458 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/___init___.py
--rw-r--r--   0        0        0    17596 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/certbot_manager.py
--rw-r--r--   0        0        0     3283 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/client.py
--rw-r--r--   0        0        0     2282 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/config/__init__.py
--rw-r--r--   0        0        0     2524 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/config/schema.py
--rw-r--r--   0        0        0      282 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/context/__init__.py
--rw-r--r--   0        0        0     1774 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/data.py
--rw-r--r--   0        0        0     4164 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/dns_delegation.py
--rw-r--r--   0        0        0      392 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/exceptions.py
--rw-r--r--   0        0        0     5873 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/key_vault_manager.py
--rw-r--r--   0        0        0     1126 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/log/__init__.py
--rw-r--r--   0        0        0     1548 2024-03-08 15:43:18.779606 acme_dns_azure-0.2.1/acme_dns_azure/os_manager.py
--rw-r--r--   0        0        0     2556 2024-03-08 15:43:18.783606 acme_dns_azure-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9192 1970-01-01 00:00:00.000000 acme_dns_azure-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7438 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/README.md
+-rw-r--r--   0        0        0      458 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/___init___.py
+-rw-r--r--   0        0        0    17596 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/certbot_manager.py
+-rw-r--r--   0        0        0     3283 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/client.py
+-rw-r--r--   0        0        0     2282 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/config/__init__.py
+-rw-r--r--   0        0        0     2524 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/config/schema.py
+-rw-r--r--   0        0        0      282 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/context/__init__.py
+-rw-r--r--   0        0        0     1774 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/data.py
+-rw-r--r--   0        0        0     4164 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/dns_delegation.py
+-rw-r--r--   0        0        0      392 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/exceptions.py
+-rw-r--r--   0        0        0     5873 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/key_vault_manager.py
+-rw-r--r--   0        0        0     1126 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/log/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-11 16:36:42.068721 acme_dns_azure-0.2.2/acme_dns_azure/os_manager.py
+-rw-r--r--   0        0        0     2560 2024-04-11 16:36:42.072721 acme_dns_azure-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9196 1970-01-01 00:00:00.000000 acme_dns_azure-0.2.2/PKG-INFO
```

### Comparing `acme_dns_azure-0.2.1/LICENSE` & `acme_dns_azure-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/README.md` & `acme_dns_azure-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/certbot_manager.py` & `acme_dns_azure-0.2.2/acme_dns_azure/certbot_manager.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/client.py` & `acme_dns_azure-0.2.2/acme_dns_azure/client.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/config/__init__.py` & `acme_dns_azure-0.2.2/acme_dns_azure/config/__init__.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/config/schema.py` & `acme_dns_azure-0.2.2/acme_dns_azure/config/schema.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/data.py` & `acme_dns_azure-0.2.2/acme_dns_azure/data.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/dns_delegation.py` & `acme_dns_azure-0.2.2/acme_dns_azure/dns_delegation.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/key_vault_manager.py` & `acme_dns_azure-0.2.2/acme_dns_azure/key_vault_manager.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/log/__init__.py` & `acme_dns_azure-0.2.2/acme_dns_azure/log/__init__.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/acme_dns_azure/os_manager.py` & `acme_dns_azure-0.2.2/acme_dns_azure/os_manager.py`

 * *Files identical despite different names*

### Comparing `acme_dns_azure-0.2.1/pyproject.toml` & `acme_dns_azure-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 license = "MIT"
 name = "acme-dns-azure"
 packages = [
   {include = "acme_dns_azure"},
 ]
 readme = "README.md"
 repository = "https://github.com/ZEISS/acme-dns-azure"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry_bumpversion.file."acme_dns_azure/___init___.py"]
 
 [tool.poetry.dependencies]
 azure-identity = ">=1.14.0"
 azure-keyvault-certificates = ">=4.7.0"
 azure-keyvault-secrets = ">=4.7.0"
 certbot = ">=2"
-certbot-dns-azure = ">=2"
+certbot-dns-azure = ">=2.5.0"
 cryptography = ">=42.0.0"
 dnspython = ">=2"
 python = "^3.8"
 pyyaml = ">=3"
 requests = ">=2"
 strictyaml = ">=1.7.3"
```

### Comparing `acme_dns_azure-0.2.1/PKG-INFO` & `acme_dns_azure-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acme-dns-azure
-Version: 0.2.1
+Version: 0.2.2
 Summary: ACME client setup based on Certbot for dns-01 challenges via Azure Cloud services
 Home-page: https://github.com/ZEISS/acme-dns-azure
 License: MIT
 Keywords: acme,dns,azure,certbot,letsencrypt
 Author: ZEISS Digital Innovation Partners
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,15 +23,15 @@
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Dist: azure-identity (>=1.14.0)
 Requires-Dist: azure-keyvault-certificates (>=4.7.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0)
 Requires-Dist: certbot (>=2)
-Requires-Dist: certbot-dns-azure (>=2)
+Requires-Dist: certbot-dns-azure (>=2.5.0)
 Requires-Dist: cryptography (>=42.0.0)
 Requires-Dist: dnspython (>=2)
 Requires-Dist: pyyaml (>=3)
 Requires-Dist: requests (>=2)
 Requires-Dist: strictyaml (>=1.7.3)
 Project-URL: Documentation, https://zeiss.github.io/acme-dns-azure/
 Project-URL: PyPI, https://pypi.org/project/acme-dns-azure/
```

