# Comparing `tmp/salure_helpers_brynq-1.0.0.tar.gz` & `tmp/salure_helpers_brynq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_brynq-1.0.0.tar", last modified: Fri Mar  1 16:19:44 2024, max compression
+gzip compressed data, was "dist/salure_helpers_brynq-1.0.1.tar", last modified: Thu Apr 11 14:40:37 2024, max compression
```

## Comparing `salure_helpers_brynq-1.0.0.tar` & `salure_helpers_brynq-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      231 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers/brynq/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-03-01 16:19:25.000000 salure_helpers_brynq-1.0.0/salure_helpers/brynq/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10872 2024-03-01 16:19:25.000000 salure_helpers_brynq-1.0.0/salure_helpers/brynq/brynq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/
--rw-r--r--   0 root         (0) root         (0)      231 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      333 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/salure_helpers_brynq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 16:19:44.000000 salure_helpers_brynq-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-03-01 16:19:25.000000 salure_helpers_brynq-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers/brynq/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-04-11 14:40:20.000000 salure_helpers_brynq-1.0.1/salure_helpers/brynq/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11194 2024-04-11 14:40:20.000000 salure_helpers_brynq-1.0.1/salure_helpers/brynq/brynq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      333 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/salure_helpers_brynq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 14:40:37.000000 salure_helpers_brynq-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-11 14:40:20.000000 salure_helpers_brynq-1.0.1/setup.py
```

### Comparing `salure_helpers_brynq-1.0.0/salure_helpers/brynq/brynq.py` & `salure_helpers_brynq-1.0.1/salure_helpers/brynq/brynq.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,21 @@
     def get_user_data(self):
         """
         Get all users from BrynQ
         :return: A list of users
         """
         return requests.get(url=f'{self.url}users', headers=self._get_headers())
 
+    def get_user_authorization_qlik_app(self,dashboard_id):
+        """
+        Get all users from BrynQ who have access to a qlik dashboard with their entities
+        :return: A list of users and entities
+        """
+        return requests.get(url=f'{self.url}/qlik/{dashboard_id}/users', headers=self._get_headers())
+
     def get_role_data(self):
         """
         Get all roles from BrynQ
         :return: A list of roles
         """
         return requests.get(url=f'{self.url}roles', headers=self._get_headers())
```

