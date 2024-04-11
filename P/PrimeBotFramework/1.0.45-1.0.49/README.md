# Comparing `tmp/PrimeBotFramework-1.0.45.tar.gz` & `tmp/PrimeBotFramework-1.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-_iyq8x4i/PrimeBotFramework-1.0.45.tar", last modified: Fri Oct  6 14:41:54 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-da2vlkbm/PrimeBotFramework-1.0.49.tar", last modified: Thu Apr 11 12:01:40 2024, max compression
```

## Comparing `PrimeBotFramework-1.0.45.tar` & `PrimeBotFramework-1.0.49.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.728845 PrimeBotFramework-1.0.45/
--rw-r--r--   0 root         (0) root         (0)      891 2023-10-06 14:41:54.728845 PrimeBotFramework-1.0.45/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.720846 PrimeBotFramework-1.0.45/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.720846 PrimeBotFramework-1.0.45/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.720846 PrimeBotFramework-1.0.45/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10261 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.720846 PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     5755 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/FeriadosBancarios/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/FeriadosBancarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/FeriadosBancarios/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.724846 PrimeBotFramework-1.0.45/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-10-06 14:41:54.728845 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      891 2023-10-06 14:41:54.000000 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-10-06 14:41:54.000000 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-10-06 14:41:54.000000 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-10-06 14:41:54.000000 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-10-06 14:41:54.000000 PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-10-06 14:41:54.728845 PrimeBotFramework-1.0.45/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-10-06 14:41:44.000000 PrimeBotFramework-1.0.45/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.517194 PrimeBotFramework-1.0.49/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 12:01:40.517194 PrimeBotFramework-1.0.49/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10261 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     5755 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/EmailAlert/
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/EmailAlert/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-11 12:01:40.513194 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-04-11 12:01:40.000000 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-04-11 12:01:40.000000 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-11 12:01:40.000000 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-11 12:01:40.000000 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-11 12:01:40.000000 PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-11 12:01:40.517194 PrimeBotFramework-1.0.49/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-11 12:01:31.000000 PrimeBotFramework-1.0.49/setup.py
```

### Comparing `PrimeBotFramework-1.0.45/PKG-INFO` & `PrimeBotFramework-1.0.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.45
+Version: 1.0.49
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/Cnab750/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/Cnab750/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.49/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/FeriadosBancarios/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/FeriadosBancarios/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.49/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.45
+Version: 1.0.49
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.45/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.49/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 PrimeBot/CpfCnpj/__init__.py
 PrimeBot/CpfCnpj/api_codes.py
 PrimeBot/CpfCnpj/model.py
 PrimeBot/D4Sign/__init__.py
 PrimeBot/DeathByCaptcha/__init__.py
 PrimeBot/Documents/__init__.py
 PrimeBot/Elastic/__init__.py
+PrimeBot/EmailAlert/__init__.py
 PrimeBot/ExchangeGraph/__init__.py
 PrimeBot/FeriadosBancarios/__init__.py
 PrimeBot/FeriadosBancarios/model.py
 PrimeBot/IntegracaoSendGrid/__init__.py
 PrimeBot/ListenerECS/__init__.py
 PrimeBot/Mongo/__init__.py
 PrimeBot/OracleDB/__init__.py
```

### Comparing `PrimeBotFramework-1.0.45/setup.py` & `PrimeBotFramework-1.0.49/setup.py`

 * *Files identical despite different names*

