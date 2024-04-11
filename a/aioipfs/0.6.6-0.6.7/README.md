# Comparing `tmp/aioipfs-0.6.6.tar.gz` & `tmp/aioipfs-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipfs-0.6.6.tar", last modified: Wed Jan 31 22:22:59 2024, max compression
+gzip compressed data, was "aioipfs-0.6.7.tar", last modified: Thu Apr 11 09:59:15 2024, max compression
```

## Comparing `aioipfs-0.6.6.tar` & `aioipfs-0.6.7.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 22:22:59.321872 aioipfs-0.6.6/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-01-31 22:22:27.000000 aioipfs-0.6.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-01-31 22:22:27.000000 aioipfs-0.6.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6535 2024-01-31 22:22:59.320872 aioipfs-0.6.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4843 2024-01-31 22:22:27.000000 aioipfs-0.6.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 22:22:59.316872 aioipfs-0.6.6/aioipfs/
--rw-rw-rw-   0 root         (0) root         (0)     9968 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    58824 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 22:22:59.318872 aioipfs-0.6.6/aioipfs/apis/
--rw-rw-rw-   0 root         (0) root         (0)     7611 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6764 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/multibase.py
--rw-rw-rw-   0 root         (0) root         (0)    12594 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/p2p.py
--rw-rw-rw-   0 root         (0) root         (0)     7602 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/pin.py
--rw-rw-rw-   0 root         (0) root         (0)     6103 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/pubsub.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/apis/swarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2326 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     6929 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/gitignore_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5322 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10771 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     2371 2024-01-31 22:22:27.000000 aioipfs-0.6.6/aioipfs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 22:22:59.319872 aioipfs-0.6.6/aioipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6535 2024-01-31 22:22:59.000000 aioipfs-0.6.6/aioipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      545 2024-01-31 22:22:59.000000 aioipfs-0.6.6/aioipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-31 22:22:59.000000 aioipfs-0.6.6/aioipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      252 2024-01-31 22:22:59.000000 aioipfs-0.6.6/aioipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-31 22:22:59.000000 aioipfs-0.6.6/aioipfs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-01-31 22:22:27.000000 aioipfs-0.6.6/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-01-31 22:22:27.000000 aioipfs-0.6.6/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-31 22:22:59.321872 aioipfs-0.6.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2208 2024-01-31 22:22:27.000000 aioipfs-0.6.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-31 22:22:59.319872 aioipfs-0.6.6/tests/
--rwxrwxrwx   0 root         (0) root         (0)    35441 2024-01-31 22:22:27.000000 aioipfs-0.6.6/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:15.002682 aioipfs-0.6.7/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-11 09:58:33.000000 aioipfs-0.6.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-11 09:58:33.000000 aioipfs-0.6.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6714 2024-04-11 09:59:15.002682 aioipfs-0.6.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2024-04-11 09:58:33.000000 aioipfs-0.6.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.997682 aioipfs-0.6.7/aioipfs/
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    58824 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.999682 aioipfs-0.6.7/aioipfs/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     7998 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6764 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/multibase.py
+-rw-rw-rw-   0 root         (0) root         (0)    12594 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/p2p.py
+-rw-rw-rw-   0 root         (0) root         (0)     7602 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/pin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/pubsub.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/apis/swarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6929 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/gitignore_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5322 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10771 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/multi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2024-04-11 09:58:33.000000 aioipfs-0.6.7/aioipfs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:15.000682 aioipfs-0.6.7/aioipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6714 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 09:59:14.000000 aioipfs-0.6.7/aioipfs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1825 2024-04-11 09:58:33.000000 aioipfs-0.6.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 09:59:15.002682 aioipfs-0.6.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:14.999682 aioipfs-0.6.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    39157 2024-04-11 09:58:33.000000 aioipfs-0.6.7/tests/test_client.py
```

### Comparing `aioipfs-0.6.6/LICENSE` & `aioipfs-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/PKG-INFO` & `aioipfs-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.6
+Version: 0.6.7
 Summary: Asynchronous IPFS client library
-Home-page: https://gitlab.com/cipres/aioipfs
-Author: cipres
-Author-email: alkaline@gmx.co.uk
+Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
+Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,27 +37,31 @@
 Requires-Dist: ipfs-car-decoder==0.1.1; extra == "car"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
+Requires-Dist: guzzle_sphinx_theme; extra == "docs"
 
 =======
 aioipfs
 =======
 
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.26.0*. Unit tests are run against
+for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs
@@ -198,30 +201,30 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.26.0
+- kubo >=0.14.0,<=0.27.0
 
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
 the IPFS daemon when using the */api/v0/get* API call, to avoid blocking the
 event loop. TAR extraction is done in asyncio's threadpool.
 
 Requirements
 ============
 
-- Python >= 3.6, <= 3.11
+- Python >= 3.6, <= 3.12
 - aiohttp_
 - aiofiles_
 - py-multibase_
 - yarl_
 
 .. _aiohttp: https://pypi.python.org/pypi/aiohttp
 .. _aiofiles: https://pypi.python.org/pypi/aiofiles
```

### Comparing `aioipfs-0.6.6/README.rst` & `aioipfs-0.6.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.26.0*. Unit tests are run against
+for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs
@@ -153,30 +153,30 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.26.0
+- kubo >=0.14.0,<=0.27.0
 
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
 the IPFS daemon when using the */api/v0/get* API call, to avoid blocking the
 event loop. TAR extraction is done in asyncio's threadpool.
 
 Requirements
 ============
 
-- Python >= 3.6, <= 3.11
+- Python >= 3.6, <= 3.12
 - aiohttp_
 - aiofiles_
 - py-multibase_
 - yarl_
 
 .. _aiohttp: https://pypi.python.org/pypi/aiohttp
 .. _aiofiles: https://pypi.python.org/pypi/aiofiles
```

### Comparing `aioipfs-0.6.6/aioipfs/__init__.py` & `aioipfs-0.6.7/aioipfs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-__version__ = '0.6.6'
+__version__ = '0.6.7'
 
 from yarl import URL
 from distutils.version import StrictVersion
 from typing import Union
 
 import asyncio
 import aiohttp
 import ipaddress
 import re
 import socket
 
+from aiohttp import BasicAuth
+
 from multiaddr import Multiaddr
 from multiaddr.exceptions import ParseError
 from multiaddr.exceptions import StringParseError
 
 from aioipfs import api
 from aioipfs.exceptions import *  # noqa
 from aioipfs.apis import dag as dag_api
@@ -28,14 +30,26 @@
 RPC_API_DEFAULT_PORT = 5001
 
 
 class IpfsDaemonVersion(StrictVersion):
     pass
 
 
+class BearerAuth(BasicAuth):
+    """
+    Cheap subclass of BasicAuth to authenticate with a token
+    """
+
+    def __init__(self, token: str):
+        self.token = token
+
+    def encode(self) -> str:
+        return f'Bearer {self.token}'
+
+
 class AsyncIPFS(object):
     """
     Asynchronous IPFS API client
 
     :param str maddr: The multiaddr for the IPFS daemon's RPC API
         (this is the preferred method of specifying the node's address)
     :param str host: Hostname/IP of the IPFS daemon to connect to
@@ -52,14 +66,15 @@
     """
 
     def __init__(self,
                  host: str = 'localhost',
                  port: int = RPC_API_DEFAULT_PORT,
                  scheme: str = 'http',
                  maddr: Union[Multiaddr, str] = None,
+                 auth: Union[BasicAuth, BearerAuth] = None,
                  loop=None,
                  conns_max: int = 0,
                  conns_max_per_host: int = 0,
                  read_timeout: int = 0,
                  api_version: str = 'v0',
                  debug: bool = False):
 
@@ -71,14 +86,16 @@
         self.loop = loop if loop else asyncio.get_event_loop()
 
         self._api_url = self.__compute_base_api_url(host=host,
                                                     port=port,
                                                     scheme=scheme,
                                                     maddr=maddr,
                                                     api_version=api_version)
+        self.__auth = auth if isinstance(auth,
+                                         (BasicAuth, BearerAuth)) else None
 
         self.session = self.get_session()
 
         # Install the API handlers
         self.core = api.CoreAPI(self)
         self.p2p = p2p_api.P2PAPI(self)
         self.block = api.BlockAPI(self)
@@ -192,14 +209,25 @@
     def version(self):
         return self.core.version
 
     @property
     def commands(self):
         return self.core.commands
 
+    @property
+    def auth(self):
+        return self.__auth
+
+    @auth.setter
+    def auth(self, authh: Union[BasicAuth, BearerAuth, None]):
+        if authh and not isinstance(authh, (BasicAuth, BearerAuth)):
+            raise ValueError('Invalid authentication helper')
+
+        self.__auth = authh
+
     def __compute_base_api_url(self, host=None, port=None, scheme='http',
                                maddr=None, api_version='v0'):
         """
         Compute and return the base kubo API url from the settings
         passed to the constructor. If a multiaddr is passed, use that
         to build the API URL, otherwise use host/port.
```

### Comparing `aioipfs-0.6.6/aioipfs/api.py` & `aioipfs-0.6.7/aioipfs/api.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/__init__.py` & `aioipfs-0.6.7/aioipfs/apis/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,18 @@
             # 404
             raise EndpointNotFoundError(
                 f'Endpoint for URL: {response.url} NOT FOUND'
             )
 
         msg, code = self.decode_error(data)
 
+        if response.status == HTTPForbidden.status_code:
+            # 403
+            raise RPCAccessDenied(str(msg))
+
         if isinstance(msg, str) and code is not None:
             # Check for specific errors
 
             for errclass in [NotPinnedError,
                              InvalidCIDError,
                              NoSuchLinkError,
                              IpnsKeyError,
@@ -84,50 +88,54 @@
             raise APIError(code=code,
                            message=msg,
                            http_status=response.status)
         else:
             raise UnknownAPIError()
 
     async def fetch_text(self, url, params={}, timeout=DEFAULT_TIMEOUT):
-        async with self.driver.session.post(url, params=params) as response:
+        async with self.driver.session.post(url, params=params,
+                                            auth=self.driver.auth) as response:
             status, textdata = response.status, await response.text()
             if status in HTTP_ERROR_CODES:
                 self.handle_error(response, textdata)
 
             return textdata
 
     async def fetch_raw(self, url, params={}, timeout=DEFAULT_TIMEOUT):
-        async with self.driver.session.post(url, params=params) as response:
+        async with self.driver.session.post(url, params=params,
+                                            auth=self.driver.auth) as response:
             status, data = response.status, await response.read()
             if status in HTTP_ERROR_CODES:
                 self.handle_error(response, data)
 
             return data
 
     async def car_stream(self, url, params={}):
         if not have_car_decoder:
             raise Exception('The CAR decoding library is not available')
 
         stream = car_decoder.ChunkedMemoryByteStream()
 
-        async with self.driver.session.post(url, params=params) as resp:
+        async with self.driver.session.post(url, params=params,
+                                            auth=self.driver.auth) as resp:
             async for chunk, _ in resp.content.iter_chunks():
                 await stream.append_bytes(chunk)
 
         await stream.mark_complete()
 
         return stream
 
     async def fetch_json(self, url, params={}, timeout=DEFAULT_TIMEOUT):
         return await self.post(url, params=params, outformat='json')
 
     async def post(self, url, data=None, headers={}, params={},
                    outformat='text'):
         try:
             async with self.driver.session.post(url, data=data,
+                                                auth=self.driver.auth,
                                                 headers=headers,
                                                 params=params) as response:
                 if response.status in HTTP_ERROR_CODES:
                     return self.handle_error(
                         response, await response.read()
                     )
 
@@ -144,16 +152,15 @@
             if self.driver.debug:
                 print(f'{url}: Post API error: {apierr}',
                       file=sys.stderr)
 
             raise apierr
         except (ClientPayloadError,
                 ClientConnectorError,
-                ServerDisconnectedError,
-                BaseException) as err:
+                ServerDisconnectedError) as err:
             if self.driver.debug:
                 print(f'{url}: aiohttp error: {err}',
                       file=sys.stderr)
 
             return None
 
     async def mjson_decode(self, url, method='post', data=None,
@@ -166,15 +173,15 @@
         the API endpoints which return multiple JSON messages
 
         :param str method: http method, get or post
         :param data: data, for POST only
         :param params: http params
         """
 
-        kwargs = {'params': params if params else {}}
+        kwargs = {'params': params if params else {}, 'auth': self.driver.auth}
 
         if new_session is True:
             session = self.driver.get_session(
                 conn_timeout=timeout,
                 read_timeout=read_timeout
             )
         else:
```

### Comparing `aioipfs-0.6.6/aioipfs/apis/dag.py` & `aioipfs-0.6.7/aioipfs/apis/dag.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/multibase.py` & `aioipfs-0.6.7/aioipfs/apis/multibase.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/p2p.py` & `aioipfs-0.6.7/aioipfs/apis/p2p.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/pin.py` & `aioipfs-0.6.7/aioipfs/apis/pin.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/pubsub.py` & `aioipfs-0.6.7/aioipfs/apis/pubsub.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/apis/swarm.py` & `aioipfs-0.6.7/aioipfs/apis/swarm.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/exceptions.py` & `aioipfs-0.6.7/aioipfs/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,20 @@
     pass
 
 
 class IPFSConnectionError(Exception):
     pass
 
 
+class RPCAccessDenied(Exception):
+    """
+    RPC request denied due to invalid authentication credentials
+    """
+
+
 class APIError(Exception):
     """
     IPFS API error
 
     :param int code: IPFS error code
     :param str message: Error message
     :param int http_status: HTTP status code
```

### Comparing `aioipfs-0.6.6/aioipfs/gitignore_parser.py` & `aioipfs-0.6.7/aioipfs/gitignore_parser.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/helpers.py` & `aioipfs-0.6.7/aioipfs/helpers.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/multi.py` & `aioipfs-0.6.7/aioipfs/multi.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs/util.py` & `aioipfs-0.6.7/aioipfs/util.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.6/aioipfs.egg-info/PKG-INFO` & `aioipfs-0.6.7/aioipfs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.6
+Version: 0.6.7
 Summary: Asynchronous IPFS client library
-Home-page: https://gitlab.com/cipres/aioipfs
-Author: cipres
-Author-email: alkaline@gmx.co.uk
+Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
+Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,27 +37,31 @@
 Requires-Dist: ipfs-car-decoder==0.1.1; extra == "car"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: wheel; extra == "test"
+Provides-Extra: docs
+Requires-Dist: sphinx==5.3.0; extra == "docs"
+Requires-Dist: sphinxcontrib-asyncio; extra == "docs"
+Requires-Dist: guzzle_sphinx_theme; extra == "docs"
 
 =======
 aioipfs
 =======
 
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.26.0*. Unit tests are run against
+for kubo_ version *0.27.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See `the documentation here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs
@@ -198,30 +201,30 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.26.0
+- kubo >=0.14.0,<=0.27.0
 
 Features
 ========
 
 Async file writing on get operations
 ------------------------------------
 
 The **aiofiles** library is used to asynchronously write data retrieved from
 the IPFS daemon when using the */api/v0/get* API call, to avoid blocking the
 event loop. TAR extraction is done in asyncio's threadpool.
 
 Requirements
 ============
 
-- Python >= 3.6, <= 3.11
+- Python >= 3.6, <= 3.12
 - aiohttp_
 - aiofiles_
 - py-multibase_
 - yarl_
 
 .. _aiohttp: https://pypi.python.org/pypi/aiohttp
 .. _aiofiles: https://pypi.python.org/pypi/aiofiles
```

### Comparing `aioipfs-0.6.6/tests/test_client.py` & `aioipfs-0.6.7/tests/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,24 @@
 import os
 import os.path
 import platform
 import json
 import tarfile
 import sys
 
+from distutils.version import StrictVersion
 from pathlib import Path
 from multiaddr import Multiaddr
 
 import asyncio
 import aioipfs
 
 from aioipfs import util
 from aioipfs.multi import DirectoryListing
+from aioipfs.exceptions import RPCAccessDenied
 
 
 def ipfs_config_get():
     p = subprocess.Popen(['ipfs', 'config', 'show'],
                          stdout=subprocess.PIPE)
     out, err = p.communicate()
 
@@ -46,14 +48,22 @@
     sp_getconfig = subprocess.Popen(['ipfs', 'config',
                                      var], stdout=subprocess.PIPE)
     stdout, stderr = sp_getconfig.communicate()
     return stdout.decode()
 
 
 @pytest.fixture
+def ipfs_version():
+    p = subprocess.Popen(['ipfs', 'version'],
+                         stdout=subprocess.PIPE)
+    stdout, _ = p.communicate()
+    return StrictVersion(stdout.decode().replace('ipfs version ', ''))
+
+
+@pytest.fixture
 def datafiles():
     return Path(os.path.dirname(__file__)).joinpath('datafiles')
 
 
 @pytest.fixture
 def smalltar():
     fd, tpath = tempfile.mkstemp()
@@ -174,26 +184,90 @@
     yield tmpdir, sp
 
     time.sleep(0.5)
     # Cleanup
     sp.terminate()
 
 
+apiport_a = 9011
+gwport_a = 9090
+swarmport_a = 9012
+
+
+@pytest.fixture(scope='module')
+def ipfsdaemon_with_auth():
+    tmpdir = tempfile.mkdtemp()
+
+    os.putenv('IPFS_PATH', tmpdir)
+    os.system('ipfs init -e')
+
+    cfg = ipfs_config_get()
+
+    with tempfile.NamedTemporaryFile(mode='wt', delete=False) as ncfgf:
+        cfg.Addresses.API = [
+            f'/ip4/127.0.0.1/tcp/{apiport_a}',
+            f'/ip6/::1/tcp/{apiport_a}',
+        ]
+
+        cfg.Addresses.Gateway = f'/ip4/127.0.0.1/tcp/{gwport_a}'
+        cfg.Addresses.Swarm = [f"/ip4/127.0.0.1/tcp/{swarmport_a}"]
+
+        # Empty bootstrap so we're not bothered
+        cfg.Bootstrap = []
+
+        cfg.Experimental.Libp2pStreamMounting = True
+        cfg.Experimental.FilestoreEnabled = True
+
+        cfg.API.Authorizations = {
+            'Alice': {
+                "AuthSecret": "basic:alice:password123",
+                "AllowedPaths": ["/api/v0/files"]
+            },
+            'John': {
+                "AuthSecret": "basic:john:12345",
+                "AllowedPaths": ["/api/v0/add"]
+            },
+            'Bear': {
+                "AuthSecret": "bearer:token123",
+                "AllowedPaths": ["/api/v0"]
+            }
+        }
+
+        cfg.write(ncfgf)
+
+    ipfs_config_replace(ncfgf.name)
+
+    sp = subprocess.Popen(['ipfs', 'daemon'], stdout=subprocess.PIPE)
+    time.sleep(1)
+
+    yield tmpdir, sp
+
+    time.sleep(0.5)
+    sp.terminate()
+
+
 @pytest.fixture
 def ipfs_peerid(ipfsdaemon):
     return ipfs_getconfig_var('Identity.PeerID').strip()
 
 
 @pytest.fixture(autouse=True)
 async def iclient(event_loop):
     client = aioipfs.AsyncIPFS(port=apiport, loop=event_loop)
     yield client
     await client.close()
 
 
+@pytest.fixture(autouse=True)
+async def iclient_with_auth(event_loop):
+    client = aioipfs.AsyncIPFS(port=apiport_a, loop=event_loop)
+    yield client
+    await client.close()
+
+
 class TestClientConstructor:
     @pytest.mark.asyncio
     async def test_invalid_constructor(self, event_loop):
         # Invalid host
         with pytest.raises(aioipfs.InvalidNodeAddressError):
             aioipfs.AsyncIPFS(host=None, loop=event_loop)
 
@@ -280,14 +354,30 @@
 
         assert str(client.api_url) == f'http://127.0.0.1:{apiport}/api/v0/'
 
         # The default constructor should always use localhost:5001
         client = aioipfs.AsyncIPFS()
         assert str(client.api_url) == 'http://localhost:5001/api/v0/'
 
+    @pytest.mark.asyncio
+    async def test_constructor_auth(self, event_loop):
+        client = aioipfs.AsyncIPFS(auth=aioipfs.BasicAuth('bob', 'pwd'))
+        assert client.auth.login == 'bob'
+        assert client.auth.password == 'pwd'
+
+        clif = aioipfs.AsyncIPFS()
+        with pytest.raises(ValueError):
+            clif.auth = 'basic:test:test'
+
+        clif.auth = aioipfs.BearerAuth('secret-token')
+        assert clif.auth.token == 'secret-token'
+
+        clif.auth = None
+        assert clif.auth is None
+
 
 class TestAsyncIPFS:
     @pytest.mark.asyncio
     async def test_basic(self, event_loop, ipfsdaemon, iclient):
         tmpdir, sp = ipfsdaemon
         await iclient.id()
         await iclient.core.version()
@@ -385,14 +475,46 @@
                 await iclient.files.read('/noslash')
 
             # Valid MFS path
             await iclient.add_str('test', to_files='/wslash')
             assert (await iclient.files.read('/wslash')).decode() == 'test'
 
     @pytest.mark.asyncio
+    async def test_auth(self, event_loop, ipfsdaemon_with_auth,
+                        ipfs_version,
+                        iclient_with_auth, testfile1):
+        if ipfs_version < aioipfs.IpfsDaemonVersion('0.25.0'):
+            # RPC Authorization was introduced in kubo v0.25.0
+            pytest.skip('RPC Authorization not supported ')
+
+        iclient_with_auth.auth = aioipfs.BasicAuth('alice', 'password123')
+
+        with pytest.raises(RPCAccessDenied):
+            await iclient_with_auth.core.id()
+
+        # alice can use the 'files' API
+        assert await iclient_with_auth.files.ls('/')
+
+        # alice doesn't have access to the 'add' API
+        cids = [added['Hash'] async for added in iclient_with_auth.add(
+            str(testfile1))]
+        assert len(cids) == 0
+
+        # john, however, does
+        iclient_with_auth.auth = aioipfs.BasicAuth('john', '12345')
+        cids = [added['Hash'] async for added in iclient_with_auth.add(
+            str(testfile1))]
+        assert len(cids) == 1
+
+        # The token has access to the whole APi
+        iclient_with_auth.auth = aioipfs.BearerAuth('token123')
+        assert await iclient_with_auth.files.ls('/')
+        assert await iclient_with_auth.core.id()
+
+    @pytest.mark.asyncio
     async def test_hidden(self, event_loop, ipfsdaemon, iclient,
                           dir_hierarchy1):
         async for added in iclient.add(dir_hierarchy1, hidden=False):
             parts = added['Name'].split('/')
             for part in parts:
                 assert not part.startswith('.')
```

