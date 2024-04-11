# Comparing `tmp/qiskit_scaleway-0.1.3.tar.gz` & `tmp/qiskit_scaleway-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_scaleway-0.1.3.tar", last modified: Thu Mar 28 15:59:01 2024, max compression
+gzip compressed data, was "qiskit_scaleway-0.1.4.tar", last modified: Thu Apr 11 09:28:53 2024, max compression
```

## Comparing `qiskit_scaleway-0.1.3.tar` & `qiskit_scaleway-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-03-28 15:59:01.763616 qiskit_scaleway-0.1.3/
--rw-r--r--   0 bonnie     (501) staff       (20)    11357 2024-03-25 15:53:04.000000 qiskit_scaleway-0.1.3/LICENSE
--rw-r--r--   0 bonnie     (501) staff       (20)      302 2024-03-28 15:59:01.763150 qiskit_scaleway-0.1.3/PKG-INFO
--rw-r--r--   0 bonnie     (501) staff       (20)       18 2024-03-26 09:12:10.000000 qiskit_scaleway-0.1.3/README.md
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-03-28 15:59:01.759327 qiskit_scaleway-0.1.3/qiskit_scaleway/
--rw-r--r--   0 bonnie     (501) staff       (20)       39 2024-03-26 08:50:23.000000 qiskit_scaleway-0.1.3/qiskit_scaleway/__init__.py
--rw-r--r--   0 bonnie     (501) staff       (20)     3724 2024-03-28 15:07:24.000000 qiskit_scaleway-0.1.3/qiskit_scaleway/backend.py
--rw-r--r--   0 bonnie     (501) staff       (20)     2964 2024-03-28 15:44:12.000000 qiskit_scaleway-0.1.3/qiskit_scaleway/client.py
--rw-r--r--   0 bonnie     (501) staff       (20)     4947 2024-03-28 15:56:45.000000 qiskit_scaleway-0.1.3/qiskit_scaleway/job.py
--rw-r--r--   0 bonnie     (501) staff       (20)     2064 2024-03-28 15:53:12.000000 qiskit_scaleway-0.1.3/qiskit_scaleway/provider.py
-drwxr-xr-x   0 bonnie     (501) staff       (20)        0 2024-03-28 15:59:01.762257 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/
--rw-r--r--   0 bonnie     (501) staff       (20)      302 2024-03-28 15:59:01.000000 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/PKG-INFO
--rw-r--r--   0 bonnie     (501) staff       (20)      352 2024-03-28 15:59:01.000000 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/SOURCES.txt
--rw-r--r--   0 bonnie     (501) staff       (20)        1 2024-03-28 15:59:01.000000 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/dependency_links.txt
--rw-r--r--   0 bonnie     (501) staff       (20)       87 2024-03-28 15:59:01.000000 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/requires.txt
--rw-r--r--   0 bonnie     (501) staff       (20)       16 2024-03-28 15:59:01.000000 qiskit_scaleway-0.1.3/qiskit_scaleway.egg-info/top_level.txt
--rw-r--r--   0 bonnie     (501) staff       (20)       38 2024-03-28 15:59:01.763714 qiskit_scaleway-0.1.3/setup.cfg
--rw-r--r--   0 bonnie     (501) staff       (20)      414 2024-03-28 15:58:49.000000 qiskit_scaleway-0.1.3/setup.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.4/LICENSE
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1525 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1330 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/README.md
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/__init__.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     4951 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2877 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1892 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_job.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       70 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      740 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_estimator.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      568 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_sampler.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2532 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/provider.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     4057 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/client.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1525 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      744 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      127 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/requires.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/top_level.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/setup.cfg
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      514 2024-04-10 09:25:44.000000 qiskit_scaleway-0.1.4/setup.py
```

### Comparing `qiskit_scaleway-0.1.3/LICENSE` & `qiskit_scaleway-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.3/qiskit_scaleway/provider.py` & `qiskit_scaleway-0.1.4/qiskit_scaleway/provider.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import httpx
+import warnings
 
 from qiskit.providers import ProviderV1 as Provider
 from qiskit.providers.providerutils import filter_backends
 
-from .backend import ScalewayBackend
-from .client import ScalewayClient
+from .backends import ScalewayBackend, AerBackend, QsimBackend
+from .utils import QaaSClient
 
 
 _ENDPOINT_URL = "https://api.scaleway.com/qaas/v1alpha1"
 
 
 class ScalewayProvider(Provider):
     """
@@ -18,57 +18,60 @@
 
     :param url: optional value, endpoint URL of the API
     """
 
     def __init__(
         self, project_id: str, secret_key: str, url: str = _ENDPOINT_URL
     ) -> None:
-        self._session = None
-        self._project_id = project_id
-        self._url = url
-        self._secret_key = secret_key
-
-        self._client = ScalewayClient(url=url, token=secret_key, project_id=project_id)
-
-    @property
-    def url(self) -> str:
-        return self._url
-
-    @property
-    def project_id(self) -> str:
-        return self._project_id
-
-    @property
-    def session(self) -> str | None:
-        return self._session
-
-    @property
-    def secret_key(self) -> str:
-        return self._secret_key
+        self.__client = QaaSClient(url=url, token=secret_key, project_id=project_id)
 
-    def backends(self, name=None, session=None, **kwargs) -> list[ScalewayBackend]:
+    def backends(self, name: str = None, **kwargs) -> list[ScalewayBackend]:
         """Return a list of backends matching the specified filtering.
 
         Args:
             name (str): name of the backend.
 
         Returns:
             list[ScalewayBackend]: a list of Backends that match the filtering
                 criteria.
         """
-        self._session = session
 
         scaleway_backends = []
-        json_resp = self._client.list_platforms(name)
+        json_resp = self.__client.list_platforms(name)
 
-        for platform in json_resp["platforms"]:
-            scaleway_backends.append(
-                ScalewayBackend(
+        for platform_dict in json_resp["platforms"]:
+            name = platform_dict.get("name")
+            backend = None
+
+            if name.startswith("aer"):
+                backend = AerBackend(
+                    provider=self,
+                    client=self.__client,
+                    backend_id=platform_dict.get("id"),
+                    name=name,
+                    version=platform_dict.get("version"),
+                    num_qubits=platform_dict.get("max_qubit_count"),
+                    metadata=platform_dict.get("metadata", None),
+                )
+            elif name.startswith("qsim"):
+                backend = QsimBackend(
                     provider=self,
-                    platform_id=platform.get("id"),
-                    name=platform.get("name"),
-                    version=platform.get("version"),
-                    num_qubits=platform.get("max_qubit_count"),
+                    client=self.__client,
+                    backend_id=platform_dict.get("id"),
+                    name=name,
+                    version=platform_dict.get("version"),
+                    num_qubits=platform_dict.get("max_qubit_count"),
+                    metadata=platform_dict.get("metadata", None),
                 )
-            )
+
+            if backend is None:
+                warnings.warn(
+                    f"Backend {name} was not created successfully",
+                    UserWarning,
+                    stacklevel=2,
+                )
+
+                continue
+
+            scaleway_backends.append(backend)
 
         return filter_backends(scaleway_backends, **kwargs)
```

