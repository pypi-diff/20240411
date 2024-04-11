# Comparing `tmp/decision_optimization_client-1.1.0.tar.gz` & `tmp/decision_optimization_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decision_optimization_client-1.1.0.tar", last modified: Thu Jan 19 13:36:44 2023, max compression
+gzip compressed data, was "decision_optimization_client-1.1.1.tar", last modified: Thu Apr 11 07:28:09 2024, max compression
```

## Comparing `decision_optimization_client-1.1.0.tar` & `decision_optimization_client-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tymek      (501) staff       (20)        0 2023-01-19 13:36:44.526433 decision_optimization_client-1.1.0/
--rw-r--r--   0 tymek      (501) staff       (20)    11350 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/LICENSE.txt
--rw-r--r--   0 tymek      (501) staff       (20)       89 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/MANIFEST.in
--rw-r--r--   0 tymek      (501) staff       (20)    13182 2023-01-19 13:36:44.526014 decision_optimization_client-1.1.0/PKG-INFO
--rw-r--r--   0 tymek      (501) staff       (20)     1378 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/README.rst
-drwxr-xr-x   0 tymek      (501) staff       (20)        0 2023-01-19 13:36:44.524830 decision_optimization_client-1.1.0/decision_optimization_client/
--rw-r--r--   0 tymek      (501) staff       (20)      631 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/__init__.py
--rw-r--r--   0 tymek      (501) staff       (20)     1522 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/asset.py
--rw-r--r--   0 tymek      (501) staff       (20)     3576 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/base_resource.py
--rw-r--r--   0 tymek      (501) staff       (20)    59038 2022-12-02 13:41:34.000000 decision_optimization_client-1.1.0/decision_optimization_client/client.py
--rw-r--r--   0 tymek      (501) staff       (20)    15198 2022-12-02 13:41:05.000000 decision_optimization_client-1.1.0/decision_optimization_client/container.py
--rw-r--r--   0 tymek      (501) staff       (20)     6659 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/context.py
--rw-r--r--   0 tymek      (501) staff       (20)     5760 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/experiment.py
--rw-r--r--   0 tymek      (501) staff       (20)     3878 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/proxyUtils.py
--rw-r--r--   0 tymek      (501) staff       (20)     3004 2022-11-04 13:08:12.000000 decision_optimization_client-1.1.0/decision_optimization_client/solve.py
--rw-r--r--   0 tymek      (501) staff       (20)     3270 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/table.py
--rw-r--r--   0 tymek      (501) staff       (20)     4635 2022-10-19 07:44:48.000000 decision_optimization_client-1.1.0/decision_optimization_client/token.py
-drwxr-xr-x   0 tymek      (501) staff       (20)        0 2023-01-19 13:36:44.525770 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/
--rw-r--r--   0 tymek      (501) staff       (20)    13182 2023-01-19 13:36:44.000000 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/PKG-INFO
--rw-r--r--   0 tymek      (501) staff       (20)      748 2023-01-19 13:36:44.000000 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/SOURCES.txt
--rw-r--r--   0 tymek      (501) staff       (20)        1 2023-01-19 13:36:44.000000 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/dependency_links.txt
--rw-r--r--   0 tymek      (501) staff       (20)       13 2023-01-19 13:36:44.000000 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/requires.txt
--rw-r--r--   0 tymek      (501) staff       (20)       29 2023-01-19 13:36:44.000000 decision_optimization_client-1.1.0/decision_optimization_client.egg-info/top_level.txt
--rw-r--r--   0 tymek      (501) staff       (20)       38 2023-01-19 13:36:44.526506 decision_optimization_client-1.1.0/setup.cfg
--rw-r--r--   0 tymek      (501) staff       (20)     1083 2023-01-02 11:37:36.000000 decision_optimization_client-1.1.0/setup.py
+drwxr-xr-x   0 arnaud     (501) staff       (20)        0 2024-04-11 07:28:09.239409 decision_optimization_client-1.1.1/
+-rw-r--r--   0 arnaud     (501) staff       (20)    11350 2022-06-29 14:43:25.000000 decision_optimization_client-1.1.1/LICENSE.txt
+-rw-r--r--   0 arnaud     (501) staff       (20)       89 2022-09-02 12:40:46.000000 decision_optimization_client-1.1.1/MANIFEST.in
+-rw-r--r--   0 arnaud     (501) staff       (20)    13225 2024-04-11 07:28:09.239100 decision_optimization_client-1.1.1/PKG-INFO
+-rw-r--r--   0 arnaud     (501) staff       (20)     1378 2022-09-02 12:40:46.000000 decision_optimization_client-1.1.1/README.rst
+drwxr-xr-x   0 arnaud     (501) staff       (20)        0 2024-04-11 07:28:09.237191 decision_optimization_client-1.1.1/decision_optimization_client/
+-rw-r--r--   0 arnaud     (501) staff       (20)      631 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/__init__.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     1522 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/asset.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     3576 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/base_resource.py
+-rw-r--r--   0 arnaud     (501) staff       (20)    60234 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/client.py
+-rw-r--r--   0 arnaud     (501) staff       (20)    15196 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/container.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     6653 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/context.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     5616 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/experiment.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     4386 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/proxyUtils.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     3004 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/solve.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     3270 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/table.py
+-rw-r--r--   0 arnaud     (501) staff       (20)     4635 2024-03-22 10:26:11.000000 decision_optimization_client-1.1.1/decision_optimization_client/token.py
+drwxr-xr-x   0 arnaud     (501) staff       (20)        0 2024-04-11 07:28:09.238749 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/
+-rw-r--r--   0 arnaud     (501) staff       (20)    13225 2024-04-11 07:28:09.000000 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/PKG-INFO
+-rw-r--r--   0 arnaud     (501) staff       (20)      748 2024-04-11 07:28:09.000000 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/SOURCES.txt
+-rw-r--r--   0 arnaud     (501) staff       (20)        1 2024-04-11 07:28:09.000000 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/dependency_links.txt
+-rw-r--r--   0 arnaud     (501) staff       (20)       13 2024-04-11 07:28:09.000000 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/requires.txt
+-rw-r--r--   0 arnaud     (501) staff       (20)       29 2024-04-11 07:28:09.000000 decision_optimization_client-1.1.1/decision_optimization_client.egg-info/top_level.txt
+-rw-r--r--   0 arnaud     (501) staff       (20)       38 2024-04-11 07:28:09.239459 decision_optimization_client-1.1.1/setup.cfg
+-rw-r--r--   0 arnaud     (501) staff       (20)     1083 2024-03-22 10:34:32.000000 decision_optimization_client-1.1.1/setup.py
```

### Comparing `decision_optimization_client-1.1.0/LICENSE.txt` & `decision_optimization_client-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `decision_optimization_client-1.1.0/PKG-INFO` & `decision_optimization_client-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision_optimization_client
-Version: 1.1.0
+Version: 1.1.1
 Summary: The IBM Decision Optimization Scenario Python client
 Author: The IBM Decision Optimization on team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,7 +203,9 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: six
```

### Comparing `decision_optimization_client-1.1.0/README.rst` & `decision_optimization_client-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/__init__.py` & `decision_optimization_client-1.1.1/decision_optimization_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 #
 # Import modules from the various sub-module so that we can have everything at hand
 #
 from .experiment import Experiment
 from .container import Container
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/asset.py` & `decision_optimization_client-1.1.1/decision_optimization_client/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import json
 from six import string_types
 
 from .base_resource import DDObject
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/base_resource.py` & `decision_optimization_client-1.1.1/decision_optimization_client/base_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import json
 
 try:
    from collections.abc import MutableMapping
 except ImportError:
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/client.py` & `decision_optimization_client-1.1.1/decision_optimization_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 
 import json
-import requests
 import os
-import warnings
 import threading
+import warnings
 
-
-from six import string_types
+import requests
 from setuptools.command.easy_install import get_exe_prefixes
+from six import string_types
 
 try:
     from urllib import urlencode
 except ImportError:
     # py3
     from urllib.parse import urlencode
 
@@ -27,206 +26,227 @@
     pd = None
 
 try:
     from StringIO import StringIO as BytesIO
 except ImportError:
     from io import BytesIO
 
-from six import iteritems
 import time
 
-from .container import Container, get_container_name
 from decision_optimization_client.experiment import Experiment, get_experiment_id
+from six import iteritems
+
 from .asset import Asset, get_asset_name
-from .table import Table, get_table_name, TableType
-from .solve import SolveStatus, SolveConfig
-from .proxyUtils import CallWithToken
-from .token import Token
+from .container import Container, get_container_name
 from .context import Context
-from .token import read_token_file
+from .proxyUtils import CallWithToken
+from .solve import SolveConfig, SolveStatus
+from .table import Table, TableType, get_table_name
+from .token import Token, read_token_file
+
+content_json = {"Content-Type": "application/json"}
+content_octet_stream = {
+    "Content-Type": "application/octet-stream",
+    "Content-Encoding": "identity",
+}
+content_csv = {"Content-Type": "text/csv"}
+accept_csv = {"Content-Type": "application/json", "Accept": "text/csv"}
 
-content_json = {'Content-Type': 'application/json'}
-content_octet_stream = {'Content-Type': 'application/octet-stream',
-                        'Content-Encoding': 'identity'}
-content_csv = {'Content-Type': 'text/csv'}
-accept_csv = {'Content-Type': 'application/json',
-              'Accept': 'text/csv'}
 
 def display_headers(session, headers=None):
     h = {}
     h.update(session.headers)
     h.update(headers)
     print(json.dumps(h, indent=3))
 
 
 class DDException(Exception):
-    '''The base exception for the Decision Optimization client.
+    """The base exception for the Decision Optimization client.
 
     Attributes:
         errors: A list of errors as [{'code': code, 'message': message}]
         trace: The trace id
         message: a string representation of the errors
-    '''
+    """
+
     def __init__(self, json_def):
-        self.errors = json_def['errors']
-        self.trace = json_def.get('trace')
+        self.errors = json_def["errors"]
+        self.trace = json_def.get("trace")
         super(DDException, self).__init__(self.message)
 
     @property
     def message(self):
-        m = [('%s:%s' % (x['code'], x['message'])) for x in self.errors]
-        return '\n'.join(m)
+        m = [("%s:%s" % (x["code"], x["message"])) for x in self.errors]
+        return "\n".join(m)
+
 
 class DDClientException(Exception):
-    '''Generic client exception
-    '''
+    """Generic client exception"""
+
     pass
 
 
 class IAMAuthHandler(object):
     def __init__(self, apikey):
         self.apikey = apikey
 
     def get_authorization(self):
         from project_lib.utils import environment as pcl_env  # @UnresolvedImport
+
         iam_api = pcl_env.get_iam_service_url()
-        headers = {'Authorization': 'Basic Yng6Yng=',
-                   'Accept': 'application/json',
-                   'Content-Type': 'application/x-www-form-urlencoded',
-                   'cache-control': 'no-cache'
-            }
-        data = 'grant_type=urn%3Aibm%3Aparams%3Aoauth%3Agrant-type%3Aapikey&apikey={apikey}&response_type=cloud_iam'.format(apikey=self.apikey)
+        headers = {
+            "Authorization": "Basic Yng6Yng=",
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "cache-control": "no-cache",
+        }
+        data = "grant_type=urn%3Aibm%3Aparams%3Aoauth%3Agrant-type%3Aapikey&apikey={apikey}&response_type=cloud_iam".format(
+            apikey=self.apikey
+        )
         r = requests.post(iam_api, headers=headers, data=data)
         if r.status_code == 200:
-            os.environ['RUNTIME_OAUTH_CLIENT_ID'] = "bx"
-            os.environ['RUNTIME_OAUTH_CLIENT_SECRET'] = "bx"
-            os.environ['RUNTIME_OAUTH_URL'] = iam_api
-            iam_info = json.loads(r.content.decode(r.encoding if r.encoding else 'utf-8'))
-            if not 'access_token' in iam_info:
-                raise DDClientException('Could not request access_token from IAM server')
-            return [iam_info['access_token'],iam_info['refresh_token']]
+            os.environ["RUNTIME_OAUTH_CLIENT_ID"] = "bx"
+            os.environ["RUNTIME_OAUTH_CLIENT_SECRET"] = "bx"
+            os.environ["RUNTIME_OAUTH_URL"] = iam_api
+            iam_info = json.loads(
+                r.content.decode(r.encoding if r.encoding else "utf-8")
+            )
+            if not "access_token" in iam_info:
+                raise DDClientException(
+                    "Could not request access_token from IAM server"
+                )
+            return [iam_info["access_token"], iam_info["refresh_token"]]
         else:
             r.raise_for_status()
 
 
-
-
 class Client(object):
-    '''The class to access Experiments in Decision Optimization.
+    """The class to access Experiments in Decision Optimization.
 
     To use the client in Cloud Pak For Data::
 
         from decision_optimization_client import Client
         client = Client()
-        
+
     To use the client in Cloud Pak For Data as a Service::
 
         from decision_optimization_client import Client
         client = Client(pc=pc) # with pc being the project context
 
     or if you want to access another project::
 
         from decision_optimization_client import Client
         client = Client(project_id="project id string",
                         authorization="bearer authorization token")
-                        
+
     Then use the following method to retrieve one or more experiments:
 
         * :meth:`~decision_optimization_client.Client.get_experiment`
         * :meth:`~decision_optimization_client.Client.get_experiments`
 
     Example:
         To return the list of experiments::
 
             from decision_optimization_client import Client
 
             client = Client()
             # get list of available experiments
             containers = client.get_experiments()
-    '''
+    """
 
-    def __init__(self,
-                 api_url=None,
-                 authorization=None,
-                 refresh_token=None,
-                 project_id=None,
-                 max_retries=3,
-                 proxies=None,
-                 cognitive_url=None,
-                 pc=None,
-                 apikey=None,
-                 verify=None):
-        '''Creates a new Decision Optimization scenario client.
+    def __init__(
+        self,
+        api_url=None,
+        authorization=None,
+        refresh_token=None,
+        project_id=None,
+        max_retries=3,
+        proxies=None,
+        cognitive_url=None,
+        pc=None,
+        apikey=None,
+        verify=None,
+    ):
+        """Creates a new Decision Optimization scenario client.
 
         Args:
             authorization (:obj:`str`, optional): The authorization key (to set the value of the bearer token (that you get from your api key when using iam).
             max_retries (:obj:`int`, optional): maximum number of retries.
                 Default is 3.
             proxies (:obj:`dict`, optional): Optional dictionary mapping
                 protocol to the URL of the proxy. (more info: https://docs.python-requests.org/en/master/user/advanced/#proxies)
             pc (:obj:`object`, mandatory only in Cloud Pak for Data as a Service): Project context
             apikey (:obj:`str`, optional): IAM api key
             verify (:obj:`boolean`, optional): override http's verify property
-        '''
+        """
         context = Context()
-        self.api_url = api_url if api_url is not None else '%s/v2' % context.get_common_api_url()
+        self.api_url = (
+            api_url if api_url is not None else "%s/v2" % context.get_common_api_url()
+        )
 
         # legacy support for apikey which is not necessary anymore
         if apikey:
             # apikey is an IAM apikey, request for a token
             auth_handler = IAMAuthHandler(apikey)
             authorizations = auth_handler.get_authorization()
             authorization = authorizations[0]
             refresh_token = authorizations[1]
         # at this point, if api_url has not been guessed, use a default
         # value suitable for use with DSX
-        self.cognitive_url = cognitive_url if cognitive_url is not None else \
-            'https://internal-nginx-svc:12443/v1/cognitive'
+        self.cognitive_url = (
+            cognitive_url
+            if cognitive_url is not None
+            else "https://internal-nginx-svc:12443/v1/cognitive"
+        )
         # Create session
         self.session = requests.Session()
         # mount custom adapters for http and https for this session
         hta = requests.adapters.HTTPAdapter
-        self.session.mount('http://', hta(max_retries=max_retries))
-        self.session.mount('https://', hta(max_retries=max_retries))
+        self.session.mount("http://", hta(max_retries=max_retries))
+        self.session.mount("https://", hta(max_retries=max_retries))
+        if verify is not None:
+            self.session.verify = verify
         # Relay authorization token
         token = ""
         token_file = None
         self.token_file = None
         if authorization:
             token = authorization
             refresh_token = refresh_token
         else:
             if pc:
                 token = pc.accessToken
                 refresh_token = None
             else:
-                if 'RUNTIME_ENV_ACCESS_TOKEN_FILE' in  os.environ:
-                    token_file = os.environ['RUNTIME_ENV_ACCESS_TOKEN_FILE']
+                if "RUNTIME_ENV_ACCESS_TOKEN_FILE" in os.environ:
+                    token_file = os.environ["RUNTIME_ENV_ACCESS_TOKEN_FILE"]
                     self.token_file = token_file
                     if os.path.isdir(token_file):
-                        self.token_file = os.path.join(token_file, 'USER_ACCESS_TOKEN')
+                        self.token_file = os.path.join(token_file, "USER_ACCESS_TOKEN")
                     token = read_token_file(self.token_file)
-                    refresh_token = None          
+                    refresh_token = None
                 else:
                     # old fashion to get tokens
-                    token = os.environ.get('USER_ACCESS_TOKEN')
-                    refresh_token = os.environ.get('USER_REFRESH_TOKEN')
-        self._call = CallWithToken(Token(token, refresh_token, context.get_iam_service_url(), self.token_file), lambda r: r.status_code == 401)
-        #bearer = "Bearer"
-        #if bearer != token[:len(bearer)]:
+                    token = os.environ.get("USER_ACCESS_TOKEN")
+                    refresh_token = os.environ.get("USER_REFRESH_TOKEN")
+        self._call = CallWithToken(
+            Token(token, refresh_token, context.get_iam_service_url(), self.token_file),
+            lambda r: r.status_code == 401,
+            session=self.session,
+        )
+        # bearer = "Bearer"
+        # if bearer != token[:len(bearer)]:
         #    token = "%s %s" % (bearer, token)
-        #self.session.headers.update({'Authorization': token})
-        if verify is not None:
-            self.session.verify = verify
+        # self.session.headers.update({'Authorization': token})
         self.project_id = project_id
-        if (self.project_id is None):
+        if self.project_id is None:
             if pc:
                 self.project_id = pc.projectID
             else:
-                self.project_id = os.environ.get('PROJECT_ID')
+                self.project_id = os.environ.get("PROJECT_ID")
         # proxies
         if proxies is not None:
             self.session.proxies.update(proxies)
         self.lock = threading.Lock()
 
     def __enter__(self):
         return self
@@ -242,23 +262,22 @@
         # Checks that the request is performed correctly. '''
         if not (response.status_code in ok_status):
             # if the error already has a corresponding exception in the HTTP
             # lib, just raise it
             raise_this = None
             try:
                 j = response.json()
-                if 'errors' in j:
+                if "errors" in j:
                     raise DDException(j)
             except DDException:
                 raise
-            except ValueError: # no json
+            except ValueError:  # no json
                 pass
             response.raise_for_status()
-            raise RuntimeError("%s: %s" % (response.status_code,
-                                           response.reason))
+            raise RuntimeError("%s: %s" % (response.status_code, response.reason))
 
     def get_containers(self, parent_id, category=None):
         # Returns the list of containers.
         #
         # Container type include:
         #
         #     * ``scenario``
@@ -267,58 +286,65 @@
         #
         # Args:
         #     parent_id: The parent_id
         #     category: The container category.
         # Returns:
         #     a list of :class:`~decision_optimization_client.Container`
         type_sel = "&category=%s" % category if category else ""
-        url = '{api_url}/containers?projectId={pid}&parentId={parent}{type_sel}'.format(
+        url = "{api_url}/containers?projectId={pid}&parentId={parent}{type_sel}".format(
             api_url=self.api_url,
             pid=self.project_id,
             parent=parent_id,
-            type_sel=type_sel)
+            type_sel=type_sel,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         containers_as_json = response.json()
-        return [Container(parent_id=parent_id, json=s, client=self) for s in containers_as_json]
+        return [
+            Container(parent_id=parent_id, json=s, client=self)
+            for s in containers_as_json
+        ]
 
     def create_container(self, parent_id, container):
         # Creates a container.
         #
         # Args:
         #     container (:class:`~decision_optimization_client.Container`): The container metadata
         # Returns:
         #     The container.
-        if getattr(container, 'projectId') == None:
+        if getattr(container, "projectId") == None:
             container.projectId = self.project_id
-        url = '{api_url}/containers/{container_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container.name,
             pid=self.project_id,
-            parent=parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                     data=container._DDObject__to_json())
+            parent=parent_id,
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=container._DDObject__to_json()
+        )
         self._check_status(response, [200, 201])
         container_as_json = response.json()
         return Container(parent_id=parent_id, json=container_as_json, client=self)
 
     def get_container(self, parent_id, id):
         #  Returns the container metadata.
         #
         # Args:
         #     id: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         # Returns:
         #     a list of :class:`~decision_optimization_client.Container`
         sid = get_container_name(id)
-        url = '{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=sid,
             pid=self.project_id,
-            parent=parent_id)
+            parent=parent_id,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         container_as_json = response.json()
         return Container(parent_id=parent_id, json=container_as_json, client=self)
 
     def update_container(self, container, new_data):
         #  Updates container metadata.
@@ -326,135 +352,150 @@
         # Args:
         #     container: A :class:`~decision_optimization_client.Container`. This ``container`` is used to indicate which container
         #        is to be updated. If ``new_data`` is None, the container is
         #        updated with the data from this ``container``.
         #     new_data (:class:`~decision_optimization_client.Container`, optional): A
         #        :class:`~decision_optimization_client.Container` containing metadata to update.
         sid = get_container_name(container)
-        url = '{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=sid,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                    data=new_data._DDObject__to_json(),allow_redirects=False)
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(
+            url,
+            headers=content_json,
+            data=new_data._DDObject__to_json(),
+            allow_redirects=False,
+        )
         self._check_status(response, [200, 301])
 
     def delete_container(self, container):
         # Deletes the container.
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         sid = get_container_name(container)
-        url = '{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=sid,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def delete_containers(self, parent_id):
         #  Deletes all of the parents' containers.
         #
         #  Args:
         #       parent_id: The parent_id
-        url = '{api_url}/containers?projectId={pid}&parentId={parent}'.format(
-            api_url=self.api_url,
-            pid=self.project_id,
-            parent=parent_id)
+        url = "{api_url}/containers?projectId={pid}&parentId={parent}".format(
+            api_url=self.api_url, pid=self.project_id, parent=parent_id
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def copy_container(self, container, metadata=None):
         # Copies a container.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string. This is the source container.
         #     metadata (:class:`~decision_optimization_client.Container`, optional): new metadata
         #         to override, as a ``Container``.
         # Returns:
         #     The created container
         sid = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/copy?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/copy?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=sid,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         container_data = metadata
         if isinstance(container, Container) and metadata is None:
             container_data = container
-        response = self._call.POST(url, headers=content_json,
-                                     data=container_data._DDObject__to_json() if container_data else None)
+        response = self._call.POST(
+            url,
+            headers=content_json,
+            data=container_data._DDObject__to_json() if container_data else None,
+        )
         self._check_status(response, [201])
         container_as_json = response.json()
-        return Container(container.parent_id, json=container_as_json, client=self)
+        return Container(
+            parent_id=container.parent_id, json=container_as_json, client=self
+        )
 
     def get_assets(self, container, name=None):
         # Returns assets for a container.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string.
         # Returns:
         #     A dict where keys are asset name and values are
         #     :class:`~decision_optimization_client.Asset`.
         qparams = {}
         if name is not None:
-            qparams['name'] = name
-        query_str = '&%s' % urlencode(qparams) if qparams else ""
+            qparams["name"] = name
+        query_str = "&%s" % urlencode(qparams) if qparams else ""
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/assets?projectId={pid}&parentId={parent}{qstr}'.format(
+        url = "{api_url}/containers/{container_id}/assets?projectId={pid}&parentId={parent}{qstr}".format(
             api_url=self.api_url,
             container_id=container_id,
             pid=self.project_id,
             parent=container.parent_id,
-            qstr=query_str)
+            qstr=query_str,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         assets_as_json = response.json()
-        return {asset_json["name"]: Asset(asset_json)
-                for asset_json in assets_as_json}
+        return {asset_json["name"]: Asset(asset_json) for asset_json in assets_as_json}
 
     def update_asset(self, container, name, new_data=None):
         #  Updates asset metadata.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string. This ``container`` is used to indicate which container
         #        is to be updated.
         #     name: An asset name.
         #     new_data (:class:`~decision_optimization_client.Asset`): A
         #        :class:`~decision_optimization_client.Asset` containing metadata to update.
         container_id = get_container_name(container)
         if new_data is None:
             raise ValueError("No asset data provided")
-        url = '{api_url}/containers/{container_id}/assets/{asset_id}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/assets/{asset_id}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             asset_id=name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.POST(url, headers=content_json,
-                                    data=json.dumps(new_data),allow_redirects=False)
+            parent=container.parent_id,
+        )
+        response = self._call.POST(
+            url, headers=content_json, data=json.dumps(new_data), allow_redirects=False
+        )
         self._check_status(response, [200, 301])
 
     def create_asset(self, container, asset_meta=None):
         # Creates a new asset with given meta data.
         container_name = get_container_name(container)
         asset_name = get_asset_name(asset_meta)
-        url = '{api_url}/containers/{container_name}/assets/{asset_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_name}/assets/{asset_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container_name,
             asset_name=asset_name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                     data=asset_meta._DDObject__to_json())
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=asset_meta._DDObject__to_json()
+        )
         self._check_status(response, [201])
         asset_as_json = response.json()
         return Asset(json=asset_as_json, container=container)
 
     def get_asset(self, container, name):
         # Gets asset metadata.
         #
@@ -469,22 +510,23 @@
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_name = get_container_name(container)
         if name is None:
             return None
         if not isinstance(name, string_types):
             raise ValueError("name shoudl be a string type")
-        url = '{api_url}/containers/{container_name}/assets/{asset_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_name}/assets/{asset_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container_name,
             asset_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=content_json)
-        self._check_status(response, [200,404])
+        self._check_status(response, [200, 404])
         if response.status_code == 404:
             return None
         asset_as_json = response.json()
         return Asset(json=asset_as_json, client=self)
 
     def get_asset_data(self, container, name):
         # Gets asset data.
@@ -494,20 +536,21 @@
         #        as string.
         #     name: An asset name.
         # Returns:
         #     The asset data as a byte array.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/assets/{asset_id}/data?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/assets/{asset_id}/data?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             asset_id=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=content_octet_stream)
         self._check_status(response, [200, 204])
         if response.status_code == 204:
             return None
         return response.content
 
     def get_asset_name(self, asset=None, name=None):
@@ -524,90 +567,148 @@
         table_name = None
         if name:
             table_name = name
         if not table_name:
             table_name = get_table_name(table)
         return table_name
 
-
-    def import_table(self, container, project_asset_id, imported_table_name, category="input", lineage=None):
-        return self.__import_from_project_asset(container, project_asset_id, imported_table_name, "table", category=category, lineage=lineage)
-  
-    def export_table(self, container, container_table_name, project_asset_name = None, project_asset_id = None, write_mode=None):
-        if (project_asset_name != None and project_asset_id != None):
-            raise ValueError("Either project_asset_name or project_asset_id should be provided, but not both")
-        if (write_mode != None and write_mode not in ['append', 'truncate']):
-            raise ValueError("Only valid values for `write_mode` are `append` and `truncate`.")
+    def import_table(
+        self,
+        container,
+        project_asset_id,
+        imported_table_name,
+        category="input",
+        lineage=None,
+    ):
+        return self.__import_from_project_asset(
+            container,
+            project_asset_id,
+            imported_table_name,
+            "table",
+            category=category,
+            lineage=lineage,
+        )
+
+    def export_table(
+        self,
+        container,
+        container_table_name,
+        project_asset_name=None,
+        project_asset_id=None,
+        write_mode=None,
+    ):
+        if project_asset_name != None and project_asset_id != None:
+            raise ValueError(
+                "Either project_asset_name or project_asset_id should be provided, but not both"
+            )
+        if write_mode != None and write_mode not in ["append", "truncate"]:
+            raise ValueError(
+                "Only valid values for `write_mode` are `append` and `truncate`."
+            )
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/tables/{table_name}/data/asset?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables/{table_name}/data/asset?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             table_name=container_table_name,
             pid=self.project_id,
-            parent=container.parent_id)
-        payload = {
-            "description": "Exported from Decision Optimization experiment"
-        }
-        if (project_asset_id):
-            payload['id'] = project_asset_id
+            parent=container.parent_id,
+        )
+        payload = {"description": "Exported from Decision Optimization experiment"}
+        if project_asset_id:
+            payload["id"] = project_asset_id
         else:
-            payload['name'] = project_asset_name or container_table_name
-        if (write_mode):
-            payload['write_mode'] = write_mode
-        response = self._call.POST(url, headers=content_json,
-                                     data=json.dumps(payload))
+            payload["name"] = project_asset_name or container_table_name
+        if write_mode:
+            payload["write_mode"] = write_mode
+        response = self._call.POST(url, headers=content_json, data=json.dumps(payload))
         self._check_status(response, [200])
-        return response.json()['id']
+        return response.json()["id"]
 
-    def __import_from_project_asset(self, container, project_asset_id, imported_name, type="table", category="input", lineage=None):
-        container_id = get_container_name(container)
-        if (not type in ['table', 'asset']):
-            raise ValueError("Incorrect value for 'type' parameter. Supported types 'table', 'asset', but received: '{}'".format(type))
-        url = '{api_url}/containers/{container_id}/bulk_update?projectId={pid}&parentId={parent}'.format(
+    def __import_from_project_asset(
+        self,
+        container,
+        project_asset_id,
+        imported_name,
+        type="table",
+        category="input",
+        lineage=None,
+    ):
+        container_id = get_container_name(container)
+        if not type in ["table", "asset"]:
+            raise ValueError(
+                "Incorrect value for 'type' parameter. Supported types 'table', 'asset', but received: '{}'".format(
+                    type
+                )
+            )
+        url = "{api_url}/containers/{container_id}/bulk_update?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             pid=self.project_id,
-            parent=container.parent_id
+            parent=container.parent_id,
+        )
+        if lineage == None:
+            lineage = "Imported from project asset (asset_id: {})".format(
+                project_asset_id
             )
-        if (lineage == None):
-            lineage = "Imported from project asset (asset_id: {})".format(project_asset_id)
-        payload = [{
-            "id": project_asset_id,
-            "name": imported_name,
-            "type": type,
-            "category": category,
-            "lineage": lineage
-        }]
+        payload = [
+            {
+                "id": project_asset_id,
+                "name": imported_name,
+                "type": type,
+                "category": category,
+                "lineage": lineage,
+            }
+        ]
         response = self._call.POST(url, headers=content_json, data=json.dumps(payload))
         self._check_status(response, [200])
 
-    def import_asset(self, container, project_asset_id, imported_asset_name, category="input", lineage=None):
-        return self.__import_from_project_asset(container, project_asset_id, imported_asset_name, "asset", category=category, lineage=lineage)
-        
-    def export_asset(self, container, container_asset_name, project_asset_name = None, project_asset_id = None):
-        if (project_asset_name != None and project_asset_id != None):
-            raise ValueError("Either project_asset_name or project_asset_id should be provided, but not both")
+    def import_asset(
+        self,
+        container,
+        project_asset_id,
+        imported_asset_name,
+        category="input",
+        lineage=None,
+    ):
+        return self.__import_from_project_asset(
+            container,
+            project_asset_id,
+            imported_asset_name,
+            "asset",
+            category=category,
+            lineage=lineage,
+        )
+
+    def export_asset(
+        self,
+        container,
+        container_asset_name,
+        project_asset_name=None,
+        project_asset_id=None,
+    ):
+        if project_asset_name != None and project_asset_id != None:
+            raise ValueError(
+                "Either project_asset_name or project_asset_id should be provided, but not both"
+            )
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/assets/{asset_name}/data/asset?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/assets/{asset_name}/data/asset?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             asset_name=container_asset_name,
             pid=self.project_id,
-            parent=container.parent_id)
-        payload = {
-            "description": "Exported from Decision Optimization experiment"
-        }
-        if (project_asset_id):
-            payload['id'] = project_asset_id
+            parent=container.parent_id,
+        )
+        payload = {"description": "Exported from Decision Optimization experiment"}
+        if project_asset_id:
+            payload["id"] = project_asset_id
         else:
-            payload['name'] = project_asset_name or container_asset_name
-        response = self._call.POST(url, headers=content_json,
-                                     data=json.dumps(payload))
+            payload["name"] = project_asset_name or container_asset_name
+        response = self._call.POST(url, headers=content_json, data=json.dumps(payload))
         self._check_status(response, [200])
-        return response.json()['id']
+        return response.json()["id"]
 
     def add_asset_data(self, container, name, data=None):
         # Adds or updates asset data.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string. This ``container`` is used to indicate which container
@@ -617,22 +718,22 @@
         # Returns:
         #     the asset metadata as :class:`~decision_optimization_client.Asset`
         container_id = get_container_name(container)
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         if data is None:
             raise ValueError("No data provided")
-        url = '{api_url}/containers/{sid}/assets/{asset_id}/data?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{sid}/assets/{asset_id}/data?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             sid=container_id,
             asset_id=name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_octet_stream,
-                                    data=data)
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(url, headers=content_octet_stream, data=data)
         self._check_status(response, [200])
 
         return Asset(json=response.json(), client=self)
 
     def delete_asset(self, container, name):
         #  Deletes the asset.
         #
@@ -642,42 +743,44 @@
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         #     name: An asset name.
         container_name = get_container_name(container)
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
-        url = '{api_url}/containers/{container_name}/assets/{asset_id}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_name}/assets/{asset_id}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container_name,
             asset_id=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def delete_assets(self, container, category=None):
         #  Deletes all the assets of a container
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         #     category: The category of assets. Can be 'input', 'output' or None
         #         if both input and output assets are to be deleted.
         container_name = get_container_name(container)
         qparams = {}
         if category is not None:
-            qparams['category'] = category
-        query_str = '&%s' % urlencode(qparams) if qparams else ""
-        url = '{api_url}/containers/{container_name}/assets?projectId={pid}&parentId={parent}'.format(
+            qparams["category"] = category
+        query_str = "&%s" % urlencode(qparams) if qparams else ""
+        url = "{api_url}/containers/{container_name}/assets?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container_name,
             pid=self.project_id,
             parent=container.parent_id,
-            qstr=query_str)
+            qstr=query_str,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def get_tables(self, container, category=None, name=None):
         # Returns all container table metadata.
         #
         # Args:
@@ -687,43 +790,48 @@
         #     category: The category of tables. Can be 'input', 'output' or None
         #         if both input and output tables are to be returned.
         # Returns:
         #     A dict where keys are table name and values are
         #     :class:`~decision_optimization_client.Table`.
         qparams = {}
         if category is not None:
-            qparams['category'] = category
+            qparams["category"] = category
         if name is not None:
-            qparams['name'] = name
-        query_str = '&%s' % urlencode(qparams) if qparams else ""
+            qparams["name"] = name
+        query_str = "&%s" % urlencode(qparams) if qparams else ""
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/tables?projectId={pid}&parentId={parent}{qstr}'.format(
+        url = "{api_url}/containers/{container_id}/tables?projectId={pid}&parentId={parent}{qstr}".format(
             api_url=self.api_url,
             container_id=container_id,
             pid=self.project_id,
             parent=container.parent_id,
-            qstr=query_str)
+            qstr=query_str,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         tables_as_json = response.json()
-        return {table_json["name"]: Table(json=table_json, container=container)
-                for table_json in tables_as_json}
+        return {
+            table_json["name"]: Table(json=table_json, container=container)
+            for table_json in tables_as_json
+        }
 
     def create_table(self, container, table_meta=None):
         # Creates a new table with given meta data.
         container_id = get_container_name(container)
         table_name = get_table_name(table_meta)
-        url = '{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             table_name=table_name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                     data=table_meta._DDObject__to_json())
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=table_meta._DDObject__to_json()
+        )
         self._check_status(response, [200, 201])
         table_as_json = response.json()
         return Table(json=table_as_json, container=container)
 
     def add_table(self, container, name, new_data=None, category=None):
         # Adds table metadata.
         #
@@ -740,44 +848,47 @@
         table_data = new_data
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         if table_data is None:
             raise ValueError("No table data provided")
         if category is not None:
             table_data.category = category
-        url = '{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                    data=table_data._DDObject__to_json())
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=table_data._DDObject__to_json()
+        )
         self._check_status(response, [200])
 
     def get_table(self, container, name):
         #  Gets table metadata.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string.
         #     name: A table name.
         # Returns:
         #     A :class:`~decision_optimization_client.Table` instance.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_name = get_container_name(container)
-        url = '{api_url}/containers/{container_name}/tables/{table_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_name}/tables/{table_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_name=container_name,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=content_json)
-        self._check_status(response, [200,404])
+        self._check_status(response, [200, 404])
         if response.status_code == 404:
             return None
         table_as_json = response.json()
         return Table(json=table_as_json, container=container)
 
     def delete_table(self, container, name):
         #  Deletes the table.
@@ -785,42 +896,44 @@
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         #     name: A table name.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables/{table_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def delete_tables(self, container, category=None):
         #  Deletes all the tables of a container.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         #     category: The category of tables. Can be 'input', 'output' or None
         #         if both input and output tables are to be deleted.
         qparams = {}
         if category is not None:
-            qparams['category'] = category
-        query_str = '&%s' % urlencode(qparams) if qparams else ""
+            qparams["category"] = category
+        query_str = "&%s" % urlencode(qparams) if qparams else ""
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/tables?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             pid=self.project_id,
             parent=container.parent_id,
-            qstr=query_str)
+            qstr=query_str,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
     def get_table_type(self, container, name):
         # Gets table type.
         #
         # Args:
@@ -828,20 +941,21 @@
         #        as string.
         #     name: the name of the table
         # Returns:
         #     A :class:`~decision_optimization_client.TableType` instance.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{sid}/tables/{table_name}/type?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{sid}/tables/{table_name}/type?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             sid=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         type_as_json = response.json()
         return TableType(json=type_as_json, id=name)
 
     def update_table_type(self, container, name, new_value=None):
         #  Updates table type.
@@ -852,44 +966,49 @@
         #        is to be updated.
         #     name: the name of the table.
         #     new_value (:class:`~dd_container.TableType`): A
         #        :class:`~dd_container.TableType` containing metadata to update.
         container_id = get_container_name(container)
         if new_value is None:
             raise ValueError("No container table type provided")
-        url = '{api_url}/containers/{sid}/tables/{table_name}/type?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{sid}/tables/{table_name}/type?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             sid=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.PUT(url, headers=content_json,
-                                    data=json.dumps(new_value._DDObject__to_json()))
+            parent=container.parent_id,
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=json.dumps(new_value._DDObject__to_json())
+        )
         self._check_status(response, [200])
 
     def get_tables_type(self, container):
         # Returns a dictionary of table types for each table.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #     as string.
         # Returns:
         #     A dict which keys are table names and values are
         #     :class:`~decision_optimization_client.TableType`'s.
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/tables/types?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/tables/types?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         types_as_json = response.json()
-        return {name: TableType(json=type_json, name=name)
-                for name, type_json in iteritems(types_as_json)}
+        return {
+            name: TableType(json=type_json, name=name)
+            for name, type_json in iteritems(types_as_json)
+        }
 
     def get_table_data(self, container, name, raw=False):
         # Gets table data.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string.
@@ -897,20 +1016,21 @@
         #     raw: If set, data is returned as is from the server, without
         #        conversion into a `pandas.DataFrame`
         # Returns:
         #     A :py:obj:`pandas.DataFrame` containing the data or the raw data.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{sid}/tables/{table_name}/data?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{sid}/tables/{table_name}/data?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             sid=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.GET(url, headers=accept_csv)
         self._check_status(response, [200, 204])
         if response.status_code == 200:
             if pd and not raw:
                 data = BytesIO(response.content)
                 return pd.read_csv(data, index_col=None)
             else:
@@ -937,354 +1057,373 @@
         if pd and isinstance(data, pd.DataFrame):
             if type(data.index) != pd.RangeIndex:
                 data = data.reset_index()
             data = data.to_csv(index=False)
         qparams = []
         if category is not None:
             qparams.append("category=%s" % category)
-        query_str = '&%s' % '&'.join(qparams) if qparams else ""
-        url = '{api_url}/containers/{sid}/tables/{table_name}/data?projectId={pid}&parentId={parent}{query_str}'.format(
+        query_str = "&%s" % "&".join(qparams) if qparams else ""
+        url = "{api_url}/containers/{sid}/tables/{table_name}/data?projectId={pid}&parentId={parent}{query_str}".format(
             api_url=self.api_url,
             sid=container_id,
             table_name=name,
             pid=self.project_id,
             parent=container.parent_id,
-            query_str=query_str)
-        response = self._call.PUT(url, headers=content_csv,
-                                    data=data)
+            query_str=query_str,
+        )
+        response = self._call.PUT(url, headers=content_csv, data=data)
         self._check_status(response, [200])
 
     def delete_table_data(self, container, name):
         #  Deletes table data.
         #
         # Args:
         #     container: A :class:`~decision_optimization_client.Container` or a container name
         #        as string
         #     name: the name of the table.
         if not isinstance(name, string_types):
             raise ValueError("name should be a string type")
         container_id = get_container_name(container)
-        url = '{api_url}/containers/{container_id}/table/{table_name}?projectId={pid}&parentId={parent}'.format(
+        url = "{api_url}/containers/{container_id}/table/{table_name}?projectId={pid}&parentId={parent}".format(
             api_url=self.api_url,
             container_id=container_id,
             table_name=name,
             pid=self.project_id,
-            parent=container.parent_id)
+            parent=container.parent_id,
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
 
-    def get_experiments(self, name=None):
-        '''Returns the list of decision Experiments.
+    def get_experiments(self, name=None, folder_id=None, folder_path=None):
+        """Returns the list of decision Experiments.
 
         Args:
             name: An optional parameter. If given, only the Experiments for which
                 names match ``name`` are returned.
         Returns:
             a list of :class:`~decision_optimization_client.Experiment`
-        '''
-        url = '{api_url}/decisions?projectId={pid}'.format(
-            api_url=self.api_url,
-            pid=self.project_id)
+        """
+        query_params = "projectId={pid}".format(pid=self.project_id)
+        if name is not None:
+            query_params += "&name={param}".format(param=name)
+        if folder_id is not None:
+            query_params += "&folder_id={param}".format(param=folder_id)
+        if folder_path is not None:
+            query_params += "&folder_path={param}".format(param=folder_path)
+        url = "{api_url}/decisions?{params}".format(
+            api_url=self.api_url, params=query_params
+        )
         response = self._call.GET(url, headers=content_json)
         self._check_status(response, [200])
         experiments_as_json = response.json()
-        experiments = [Experiment(json=s, client=self) for s in experiments_as_json]
-        if name:
-            return [x for x in experiments if x.name == name]
-        else:
-            return experiments
+        return [Experiment(json=s, client=self) for s in experiments_as_json]
+
+    def create_experiment(self, experiment=None, folder_id=None, **kwargs):
+        """
+            Creates a decision experiment.
+
+
+        If this method is given an ``experiment`` argument, that experiment is
+        used to initialize the values for the new experiment. Otherwise, the
+        ``**kwargs`` are used to initialize a
+        :class:`~decision_optimization_client.Experiment`.
+
+        Example:
+
+            Creates a Experiment using the Experiment name passed as ``kwargs``::
 
-    def create_experiment(self, experiment=None, **kwargs):
-        '''
-             Creates a decision experiment.
-        
-        
-         If this method is given an ``experiment`` argument, that experiment is
-         used to initialize the values for the new experiment. Otherwise, the
-         ``**kwargs`` are used to initialize a
-         :class:`~decision_optimization_client.Experiment`.
-        
-         Example:
-        
-             Creates a Experiment using the Experiment name passed as ``kwargs``::
-        
-                 experiment = client.create_experiment(name='test experiment')
-        
-             Creates a Experiment using the experiment passed as a Experiment:
-        
-                 meta = Experiment(name='test experiment')
-                 experiment = client.create_experiment(experiment=meta)
-        
-         Args:
-             experiment (:class:`~decision_optimization_client.Experiment`): The
-                 Experiment metadata used as initial data.
-             **kwargs: kwargs used to initialize the Experiment
-         Returns:
-             The decision Experiment as a :class:`~decision_optimization_client.Experiment`
-        '''
+                experiment = client.create_experiment(name='test experiment')
+
+            Creates a Experiment using the experiment passed as a Experiment:
+
+                meta = Experiment(name='test experiment')
+                experiment = client.create_experiment(experiment=meta)
+
+        Args:
+            experiment (:class:`~decision_optimization_client.Experiment`): The
+                Experiment metadata used as initial data.
+            **kwargs: kwargs used to initialize the Experiment
+        Returns:
+            The decision Experiment as a :class:`~decision_optimization_client.Experiment`
+        """
         experiment_value = Experiment()
         if experiment:
             experiment_value.json.update(experiment.json)
         if kwargs:
             experiment_value.json.update(kwargs)
-        url = '{api_url}/decisions/{decision_name}?projectId={pid}'.format(
-            api_url=self.api_url,
-            decision_name=get_experiment_id(experiment_value),
-            pid=self.project_id)
-        response = self._call.PUT(url, headers=content_json,
-                                     data=experiment_value.to_json())
+        query_params = "projectId={pid}".format(pid=self.project_id)
+        if folder_id is not None:
+            query_params += "&folder_id={param}".format(param=folder_id)
+        url = "{api_url}/decisions?{params}".format(
+            api_url=self.api_url, params=query_params
+        )
+        response = self._call.POST(
+            url, headers=content_json, data=experiment_value.to_json()
+        )
         self._check_status(response, [201])
         json_resp = response.json()
         return Experiment(json=json_resp, client=self)
 
-    def get_experiment(self, name=None, id=None):
-        ''' Returns the decision Experiment metadata.
+    def get_experiment(self, name=None, id=None, folder_id=None):
+        """Returns the decision Experiment metadata.
 
         Args:
             name: The name of the Experiment to look for
 
         Returns:
             an :class:`~decision_optimization_client.Experiment`
             If the decision doesn't exist, you'll get an error telling you so.
-        '''
+        """
         # search by Experiment name
         if id is not None:
             guid = get_experiment_id(id)
-            url = '{api_url}/decisions/{guid}?projectId={pid}'.format(
-                api_url=self.api_url,
-                guid=guid,
-                pid=self.project_id)
+            url = "{api_url}/decisions/{guid}?projectId={pid}".format(
+                api_url=self.api_url, guid=guid, pid=self.project_id
+            )
             response = self._call.GET(url, headers=content_json)
             self._check_status(response, [200])
             framework_as_json = response.json()
             return Experiment(json=framework_as_json, client=self)
         elif name is not None:
-            possible = self.get_experiments(name=name)
+            possible = self.get_experiments(name=name, folder_id=folder_id)
             return possible[0] if possible else None
         else:
-            raise ValueError("get_experiment expects an id or name to filter decision models.")
+            raise ValueError(
+                "get_experiment expects an id or name to filter decision models."
+            )
+
+    def update_experiment(self, experiment, new_data=None, folder_id=None):
+        """Updates decision model metadata.
+
+        Examples:
+
+          Updates a Experiment with new data using name::
+
+            >>> new = Experiment()
+            >>> new.description = "new description"
+            >>> client.update_experiment(decision_model_name, new)
+
+          Gets a Experiment, then replaces description::
+
+            >>> experiment = client.get_experiment(id=guid)
+            >>> experiment.description = "new description"
+            >>> client.update_experiment(experiment)
 
-    def update_experiment(self, experiment, new_data=None):
-        '''  Updates decision model metadata.
-        
-         Examples:
-        
-           Updates a Experiment with new data using name::
-        
-             >>> new = Experiment()
-             >>> new.description = "new description"
-             >>> client.update_experiment(decision_model_name, new)
-        
-           Gets a Experiment, then replaces description::
-        
-             >>> experiment = client.get_experiment(id=guid)
-             >>> experiment.description = "new description"
-             >>> client.update_experiment(experiment)
-        
-           Gets a Experiment by name, then replaces description::
-        
-             >>> experiment = client.get_experiment(name='decision model name')
-             >>> experiment.description = "new description"
-             >>> client.update_experiment(experiment)
-        
-         Args:
-            experiment: A :class:`~decision_optimization_client.Experiment` or a name
-               as string. This ``experiment`` is used to indicate which
-               Experiment is to be updated. If ``new_data`` is None, the
-               Experiment is updated with the data from this ``experiment``.
-            new_data (:class:`~decision_optimization_client.Experiment`, optional): A
-                :class:`~decision_optimization_client.Experiment` containing metadata to
-                update.
-        '''
+          Gets a Experiment by name, then replaces description::
+
+            >>> experiment = client.get_experiment(name='decision model name')
+            >>> experiment.description = "new description"
+            >>> client.update_experiment(experiment)
+
+        Args:
+           experiment: A :class:`~decision_optimization_client.Experiment` or a name
+              as string. This ``experiment`` is used to indicate which
+              Experiment is to be updated. If ``new_data`` is None, the
+              Experiment is updated with the data from this ``experiment``.
+           new_data (:class:`~decision_optimization_client.Experiment`, optional): A
+               :class:`~decision_optimization_client.Experiment` containing metadata to
+               update.
+        """
         guid = get_experiment_id(experiment)
         experiment_data = new_data
         if isinstance(experiment, Experiment) and new_data is None:
             experiment_data = json.loads(experiment.to_json())
         if experiment_data is None:
             raise ValueError("No experiment data provided")
-        url = '{api_url}/decisions/{guid}?projectId={pid}'.format(
-            api_url=self.api_url,
-            guid=guid,
-            pid=self.project_id)
-        response = self._call.PUT(url, headers=content_json,
-                                    data=json.dumps(experiment_data))
+        query_params = "projectId={pid}".format(pid=self.project_id)
+        if folder_id is not None:
+            query_params += "&folder_id={param}".format(param=folder_id)
+        url = "{api_url}/decisions/{guid}?{params}".format(
+            api_url=self.api_url, guid=guid, params=query_params
+        )
+        response = self._call.PUT(
+            url, headers=content_json, data=json.dumps(experiment_data)
+        )
         self._check_status(response, [200])
 
     def delete_experiment(self, experiment):
         # Deletes the decision model.
         #
         # Args:
         #     experiment: A :class:`~decision_optimization_client.Experiment` or a name
         #        as string
         guid = get_experiment_id(experiment)
-        url = '{api_url}/decisions/{guid}?projectId={pid}'.format(
-            api_url=self.api_url,
-            guid=guid,
-            pid=self.project_id)
+        url = "{api_url}/decisions/{guid}?projectId={pid}".format(
+            api_url=self.api_url, guid=guid, pid=self.project_id
+        )
         response = self._call.DELETE(url, headers=content_json)
         self._check_status(response, [204])
-    
-    def get_experiment_environments(self, container,model_type):
-        experiment = self.get_experiment(name=container.parent_id)
+
+    def get_experiment_environments(self, container, model_type):
+        experiment = self.get_experiment(id=container.parent_id)
         guid = get_experiment_id(experiment)
-        url = '{api_url}/decisions/{guid}/environments?projectId={pid}&model_type={model_type}'.format(
-            api_url=self.api_url,
-            guid=guid,
-            pid=self.project_id,
-            model_type=model_type)
+        url = "{api_url}/decisions/{guid}/environments?projectId={pid}&model_type={model_type}".format(
+            api_url=self.api_url, guid=guid, pid=self.project_id, model_type=model_type
+        )
         response = self._call.GET(url, headers=content_json)
         if response.status_code == 404:
             return None
         self._check_status(response, [200])
         return response.json()
-    
+
     def add_environment_to_experiment(self, container, environment):
-        experiment = self.get_experiment(name=container.parent_id)
+        experiment = self.get_experiment(id=container.parent_id)
         guid = get_experiment_id(experiment)
-        url = '{api_url}/decisions/{guid}/environments?projectId={pid}'.format(
-            api_url=self.api_url,
-            guid=guid,
-            pid=self.project_id)
+        url = "{api_url}/decisions/{guid}/environments?projectId={pid}".format(
+            api_url=self.api_url, guid=guid, pid=self.project_id
+        )
         response = self._call.POST(url, headers=content_json, data=environment)
         self._check_status(response, [202])
-        
+
         json_env = json.loads(environment)
         timeout = 0
         while True:
             time.sleep(1)
             timeout += 1
-            envs = self.get_experiment_environments(container, json_env[0]["model"]["model_type"])
-            state =  envs["environments"][0]['status']['state']
-            if state != "preparing" :
-                env_id = envs["environments"][0]['id']
+            envs = self.get_experiment_environments(
+                container, json_env[0]["model"]["model_type"]
+            )
+            state = envs["environments"][0]["status"]["state"]
+            if state != "preparing":
+                env_id = envs["environments"][0]["id"]
                 break
             if timeout > 120:
                 break
-        
+
     def add_default_environment_to_experiment(self, container, warn=False):
         with self.lock:
             model_type = self.get_model_type(container)
-            environments = self.get_experiment_environments(container,model_type)
-            if(environments is not None and len(environments.get("environments")) == 0):
+            environments = self.get_experiment_environments(container, model_type)
+            if environments is not None and len(environments.get("environments")) == 0:
                 environment = [
                     {
                         "name": "{model_type}-default-2".format(model_type=model_type),
-                        "model": {
-                            "model_type": model_type
-                        },
-                        "default_environment": True
+                        "model": {"model_type": model_type},
+                        "default_environment": True,
                     }
                 ]
                 self.add_environment_to_experiment(container, json.dumps(environment))
                 if warn:
-                    warnings.warn('Default environment for "{model_type}" has been added.'.format(
-                        model_type=model_type))
+                    warnings.warn(
+                        'Default environment for "{model_type}" has been added.'.format(
+                            model_type=model_type
+                        )
+                    )
 
     def is_cognitive_scenario(self, container):
         # get container info
         container_id = get_container_name(container)
         qualifiers = None
         try:
             qualifiers = container.qualifiers
         except AttributeError:
             cc = self.get_container(container.parent_id, container_id)
             qualifiers = cc.qualifiers
         # check if this is a cognitive model
         if qualifiers is None:
             return False
-        qual_dict = {q['name']: q['value'] for q in qualifiers}
-        return ('modelType' in qual_dict and qual_dict.get('modelType') == 'cognitive')
+        qual_dict = {q["name"]: q["value"] for q in qualifiers}
+        return "modelType" in qual_dict and qual_dict.get("modelType") == "cognitive"
 
-    def solve(self,
-              container,
-              **kwargs):
+    def solve(self, container, **kwargs):
         # Solves the scenario model of the container which id is specified.
         #
         # This method returns as soon as the request is sent. Use
         # Client.wait_for_completion() to wait for solve completion.
         #
         # Args:
         #    container: The Container or container id to solve()
         #    **kwargs: extra arguments passed to the solve using a SolveConfig
         self.add_default_environment_to_experiment(container, True)
         container_id = get_container_name(container)
         endpoint = None
         if self.is_cognitive_scenario(container):
-            endpoint = '{api_url}/solve?projectId={pid}&parentId={parent}'.format(
+            endpoint = "{api_url}/solve?projectId={pid}&parentId={parent}".format(
                 api_url=self.cognitive_url,
                 pid=self.project_id,
-                parent=container.parent_id)
+                parent=container.parent_id,
+            )
         else:
-            endpoint = '{api_url}/decisions/solve?projectId={pid}&parentId={parent}'.format(
-                api_url=self.api_url,
-                pid=self.project_id,
-                parent=container.parent_id)
+            endpoint = (
+                "{api_url}/decisions/solve?projectId={pid}&parentId={parent}".format(
+                    api_url=self.api_url,
+                    pid=self.project_id,
+                    parent=container.parent_id,
+                )
+            )
         # create SolveConfig
         sc = SolveConfig(containerId=container_id, **kwargs)
         # run the solve
-        response = self._call.POST(endpoint, headers=content_json,
-                                     data=sc._DDObject__to_json())
+        response = self._call.POST(
+            endpoint, headers=content_json, data=sc._DDObject__to_json()
+        )
         self._check_status(response, [202])
 
     def stop_solve(self, container):
-        '''
-            Stops the solve for a scenario.
-        '''
+        """
+        Stops the solve for a scenario.
+        """
         container_id = get_container_name(container)
         endpoint = None
         if self.is_cognitive_scenario(container):
-            endpoint = '{api_url}/solve/status/{guid}?projectId={pid}&parentId={parent}'.format(
+            endpoint = "{api_url}/solve/status/{guid}?projectId={pid}&parentId={parent}".format(
                 api_url=self.cognitive_url,
                 guid=container_id,
                 pid=self.project_id,
-                parent=container.parent_id)
+                parent=container.parent_id,
+            )
         else:
-            endpoint = '{api_url}/decisions/solve/status/{guid}?projectId={pid}&parentId={parent}'.format(
+            endpoint = "{api_url}/decisions/solve/status/{guid}?projectId={pid}&parentId={parent}".format(
                 api_url=self.api_url,
                 guid=container_id,
                 pid=self.project_id,
-                parent=container.parent_id)
+                parent=container.parent_id,
+            )
         response = self._call.DELETE(endpoint, headers=content_json)
         self._check_status(response, [202])
 
     def wait_for_completion(self, container, timeout=None):
         # Waits for the solve operation specified container to complete.
         #
         # Returns:
         #     The last :class:`~decision_optimization_client.SolveStatus`
         s = self.get_solve_status(container)
         start_time = int(round(time.time() * 1000))
-        while s.state not in {'FAILED', 'TERMINATED'}:
+        while s.state not in {"FAILED", "TERMINATED"}:
             time.sleep(1)
             s = self.get_solve_status(container)
             if timeout != None:
-                if ( int(round(time.time() * 1000)) - start_time > timeout):
-                    print("Timeout reached... Returning whatever we have as a status now")
+                if int(round(time.time() * 1000)) - start_time > timeout:
+                    print(
+                        "Timeout reached... Returning whatever we have as a status now"
+                    )
                     return s
         return s
 
     def get_solve_status(self, container):
         # Queries and returns the solve status for the specified container.
         #
         # Returns:
         #     A :class:`~decision_optimization_client.SolveStatus`
         container_id = get_container_name(container)
         endpoint = None
         if self.is_cognitive_scenario(container):
-            endpoint = '{api_url}/solve/status/{guid}?projectId={pid}&parentId={parent}'.format(
+            endpoint = "{api_url}/solve/status/{guid}?projectId={pid}&parentId={parent}".format(
                 api_url=self.cognitive_url,
                 guid=container_id,
                 pid=self.project_id,
-                parent=container.parent_id)
+                parent=container.parent_id,
+            )
         else:
-            endpoint = '{api_url}/decisions/solve/status/{guid}?projectId={pid}&parentId={parent}'.format(
+            endpoint = "{api_url}/decisions/solve/status/{guid}?projectId={pid}&parentId={parent}".format(
                 api_url=self.api_url,
                 guid=container_id,
                 pid=self.project_id,
-                parent=container.parent_id)
+                parent=container.parent_id,
+            )
         response = self._call.GET(endpoint, headers=content_json)
         return SolveStatus(json=response.json())
 
     def export_notebook(self, container, name, description=None):
         # Creates a notebook from a container's model.
         #
         # Args:
@@ -1295,60 +1434,75 @@
         #     A dict with the notebook creation info::
         #
         #     {
         #        'projectNotebookId': 'aeiou',
         #        'notebookId': 'aeiou',
         #        'notebookUrl': 'aeiou'
         #     }
-        payload = {'containerId': get_container_name(container),
-                   'notebookName': name}
+        payload = {"containerId": get_container_name(container), "notebookName": name}
         if description:
-            payload['notebookDescription'] = description
-        url = '{api_url}/decisions/export/notebook?projectId={pid}&parentId={parent}'.format(
-            api_url=self.api_url,
-            pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.POST(url, headers=content_json,
-                                     data=json.dumps(payload))
+            payload["notebookDescription"] = description
+        url = "{api_url}/decisions/export/notebook?projectId={pid}&parentId={parent}".format(
+            api_url=self.api_url, pid=self.project_id, parent=container.parent_id
+        )
+        response = self._call.POST(url, headers=content_json, data=json.dumps(payload))
         self._check_status(response, [200])
         return response.json()
 
     def import_notebook(self, container, notebook_id):
         # Updates container model from notebook.
         #
         # Args:
         #     container: The container or container_id
         #     name: the name of the notebook
         #     descrition (Optional): The notebook description
-        payload = {'containerId': get_container_name(container),
-                   'notebookId': notebook_id}
-        url = '{api_url}/decisions/import/notebook?projectId={pid}&parentId={parent}'.format(
-            api_url=self.api_url,
-            pid=self.project_id,
-            parent=container.parent_id)
-        response = self._call.POST(url, headers=content_json,
-                                     data=json.dumps(payload))
+        payload = {
+            "containerId": get_container_name(container),
+            "notebookId": notebook_id,
+        }
+        url = "{api_url}/decisions/import/notebook?projectId={pid}&parentId={parent}".format(
+            api_url=self.api_url, pid=self.project_id, parent=container.parent_id
+        )
+        response = self._call.POST(url, headers=content_json, data=json.dumps(payload))
         self._check_status(response, [200])
         print(response.content)
 
     def get_model_type(self, container):
         # Returns
         #     docplex, cplex, cpo, opl
         assets = self.get_assets(container)
-        if next(("docplex" for a in assets.keys() if str(a).endswith(".py")), None) is not None :
-            return 'docplex'
-        if next(("opl" for a in assets.keys() if str(a).endswith(".mod")), None) is not None :
-            return 'opl'
-        if next(("cpo" for a in assets.keys() if str(a).endswith(".cpo")), None) is not None :
-            return 'cpo'
-        if next(("cplex" for a in assets.keys() if str(a).endswith(".lp") 
-                                        or str(a).endswith(".lp.gz")
-                                        or str(a).endswith(".lp.bz2")
-                                        or str(a).endswith(".mps")
-                                        or str(a).endswith(".mps.gz")
-                                        or str(a).endswith(".mps.bz2")
-                                        or str(a).endswith(".sav")
-                                        or str(a).endswith(".sav.gz")
-                                        or str(a).endswith(".sav.bz2")
-                                        ), None) is not None :
-            return 'cplex'
-        return 'docplex'
+        if (
+            next(("docplex" for a in assets.keys() if str(a).endswith(".py")), None)
+            is not None
+        ):
+            return "docplex"
+        if (
+            next(("opl" for a in assets.keys() if str(a).endswith(".mod")), None)
+            is not None
+        ):
+            return "opl"
+        if (
+            next(("cpo" for a in assets.keys() if str(a).endswith(".cpo")), None)
+            is not None
+        ):
+            return "cpo"
+        if (
+            next(
+                (
+                    "cplex"
+                    for a in assets.keys()
+                    if str(a).endswith(".lp")
+                    or str(a).endswith(".lp.gz")
+                    or str(a).endswith(".lp.bz2")
+                    or str(a).endswith(".mps")
+                    or str(a).endswith(".mps.gz")
+                    or str(a).endswith(".mps.bz2")
+                    or str(a).endswith(".sav")
+                    or str(a).endswith(".sav.gz")
+                    or str(a).endswith(".sav.bz2")
+                ),
+                None,
+            )
+            is not None
+        ):
+            return "cplex"
+        return "docplex"
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/container.py` & `decision_optimization_client-1.1.1/decision_optimization_client/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import json
 try:
     from StringIO import StringIO as BytesIO
 except ImportError:  # py3
     from io import BytesIO
@@ -189,15 +189,15 @@
 
         Args:
             table_name: The name of the table in the scenario
             project_asset_name: The name of a new data asset to be created in the project
             project_asset_id: The ID of an existing data asset in the project to be overwritten
             write_mode: The write mode: ``append`` or ``truncate``. Useful for connected data. Ignored for project assets that do not support it
 
-        Only one of ``project_asset_name`` and ``project_asset_id`` parameters can be used. If none is provided a new asset is created using the source table name with .csv extension.
+        Only one of ``project_asset_name`` or ``project_asset_id`` parameters can be used. If none is provided a new asset is created using the source table name with .csv extension.
 
         Returns:
             An ID of the resulting project asset 
         '''
         return self.client.export_table(self, container_table_name=table_name, project_asset_name=project_asset_name, project_asset_id=project_asset_id, write_mode=write_mode)
 
     def import_asset(self, project_asset_id, imported_asset_name, category="input", lineage=None):
@@ -215,15 +215,15 @@
         '''Exports scenario asset into a project data asset.
 
         Args:
             asset_name: The name of the asset in the scenario.
             project_asset_name: The name of a new data asset to be created in the project
             project_asset_id: The ID of an existing data asset in the project to be overwritten
             
-        Only one of ``project_asset_name`` and ``project_asset_id`` parameters can be used. If none is provided a new asset is created using the source asset name.
+        Only one of ``project_asset_name`` or ``project_asset_id`` parameters can be used. If none is provided a new asset is created using the source asset name.
         
         Returns:
             An ID of the resulting project asset 
         '''
         return self.client.export_asset(self, container_asset_name=asset_name, project_asset_name=project_asset_name, project_asset_id=project_asset_id)
 
     def add_asset_data(self, name, data=None, category='model'):
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/context.py` & `decision_optimization_client-1.1.1/decision_optimization_client/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import os
 
 COMMON_API_PREFIX = "COMMON_API_"
 IAM_SERVICE_URL_PREFIX = "IAM_SERVICE_URL_"
 BCOS_URL_PREFIX = "BCOS_URL_"
@@ -33,15 +33,15 @@
     "COMMON_API_QA": "https://api.dataplatform.test.cloud.ibm.com",
     "COMMON_API_YS1_PROD": "https://apsx-api.stage1.ng.bluemix.net",
     "COMMON_API_QA_LONDON": "https://apsx-api-qa.eu-gb.bluemix.net",
     "COMMON_API_PROD_FRA": "https://api.eu-de.dataplatform.cloud.ibm.com",
 
     "IAM_SERVICE_URL_PROD": "https://iam.ng.bluemix.net/oidc/token",
     "IAM_SERVICE_URL_QA": "https://iam.ng.bluemix.net/oidc/token",
-    "IAM_SERVICE_URL_YS1_PROD": "https://iam.stage1.ng.bluemix.net/oidc/token",
+    "IAM_SERVICE_URL_YS1_PROD": "https://iam.test.cloud.ibm.com/oidc/token",
     "IAM_SERVICE_URL_QA_LONDON": "https://iam.eu-gb.bluemix.net/oidc/token",
     "IAM_SERVICE_URL_PROD_FRA": "https://iam.eu-de.bluemix.net/oidc/token",
 
     "BCOS_URL_PROD": "https://s3-api.us-geo.objectstorage.softlayer.net",
     "BCOS_URL_QA": "https://s3-api.us-geo.objectstorage.softlayer.net",
     "BCOS_URL_YS1_PROD": "https://s3.us-west.objectstorage.uat.softlayer.net",
     "BCOS_URL_QA_LONDON": "https://s3.eu-geo.objectstorage.softlayer.net",
@@ -58,15 +58,15 @@
 
 # introducing a new style of looking up endpoints
 STAGE_ENDPOINTS_MAP = {
     ENV_ID_dev : {
         COMMON_API_PREFIX:
         "https://api.dataplatform.dev.cloud.ibm.com",
         IAM_SERVICE_URL_PREFIX:
-        "https://iam.stage1.ng.bluemix.net/oidc/token",
+        "https://iam.test.cloud.ibm.com/oidc/token",
         BCOS_URL_PREFIX:
         "https://s3.us-west.objectstorage.uat.softlayer.net",
         COS_URL_PREFIX:
         "https://s3-api.dal-us-geo.objectstorage.softlayer.net"
     },
 
     ENV_ID_prod_london : {
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/proxyUtils.py` & `decision_optimization_client-1.1.1/decision_optimization_client/proxyUtils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,100 +1,131 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import requests
 
 from .token import attempt_refresh
 
 # =============================================================================
 # There are two sets of functions here. The old ones called send_*_request
 # expect an authentication token. If the token is invalid, the request fails.
 # The new ones in CallWithToken take the token from a project handle.
 # If the token is invalid, they may try to refresh it, if the required
 # information is available in the environment.
 
+
 # The decision whether a token is expired and should be refreshed is left
 # to a callback function. By default, refresh is never attempted.
 def never_refresh(r):
-    '''Decide whether the token needs refresh.
+    """Decide whether the token needs refresh.
     Argument: r - response from an HTTP call with the requests module
     Returns:  True if the token is expired and should be refreshed,
               False otherwise.
     This default implementation always returns False.
-    '''
+    """
     return False
 
 
 class CallWithToken(object):
-
-    def __init__(self, handle, is_token_expired_callback=never_refresh):
+    def __init__(
+        self,
+        handle,
+        is_token_expired_callback=never_refresh,
+        session=requests.Session(),
+    ):
         self._project_handle = handle
         self._is_token_expired = is_token_expired_callback
+        self._session = session
         return
 
     def GET(self, url, headers):
-        r = send_get_request(url, self._project_handle.token, headers)
+        r = send_get_request(self._session, url, self._project_handle.token, headers)
         if self._is_token_expired(r) and attempt_refresh(self._project_handle):
-            r = send_get_request(url, self._project_handle.token, headers)
+            r = send_get_request(
+                self._session, url, self._project_handle.token, headers
+            )
         return r
 
     def POST(self, url, headers, data):
-        r = send_post_request(url, self._project_handle.token, headers, data)
+        r = send_post_request(
+            self._session, url, self._project_handle.token, headers, data
+        )
         if self._is_token_expired(r) and attempt_refresh(self._project_handle):
-            r = send_post_request(url, self._project_handle.token, headers, data)
+            r = send_post_request(
+                self._session, url, self._project_handle.token, headers, data
+            )
         return r
 
     def PUT(self, url, headers, data, allow_redirects=True):
-        r = send_put_multipart_request(url, self._project_handle.token, headers, data, allow_redirects)
+        r = send_put_multipart_request(
+            self._session,
+            url,
+            self._project_handle.token,
+            headers,
+            data,
+            allow_redirects,
+        )
         if self._is_token_expired(r) and attempt_refresh(self._project_handle):
-            #@@@ if files contained streaming data, can't read that on retry
-            r = send_put_multipart_request(url, self._project_handle.token,
-                                           headers, data, allow_redirects)
+            # @@@ if files contained streaming data, can't read that on retry
+            r = send_put_multipart_request(
+                self._session,
+                url,
+                self._project_handle.token,
+                headers,
+                data,
+                allow_redirects,
+            )
         return r
 
     def DELETE(self, url, headers):
-        r = send_delete_request(url, self._project_handle.token, headers)
+        r = send_delete_request(self._session, url, self._project_handle.token, headers)
         if self._is_token_expired(r) and attempt_refresh(self._project_handle):
-            r = send_delete_request(url, self._project_handle.token, headers)
+            r = send_delete_request(
+                self._session, url, self._project_handle.token, headers
+            )
         return r
 
 
-
 # -----------------------------------------------------------------------------
 
-def send_get_request(url, token, headers):
+
+def send_get_request(session, url, token, headers):
     headers["Authorization"] = _append_bearer(token)
-    
-    rsp = requests.get(url, headers=headers)
+
+    rsp = session.get(url, headers=headers)
     return rsp
 
 
-def send_post_request(url, token, headers, payload): 
+def send_post_request(session, url, token, headers, payload):
     headers["Authorization"] = _append_bearer(token)
-       
-    rsp = requests.post(url, headers=headers, data=payload)
+
+    rsp = session.post(url, headers=headers, data=payload)
     return rsp
 
 
-def send_put_multipart_request(url, token, headers, data, allow_redirects=True):
+def send_put_multipart_request(
+    session, url, token, headers, data, allow_redirects=True
+):
     headers["Authorization"] = _append_bearer(token)
-    
-    rsp = requests.put(url, headers=headers, data=data, allow_redirects=allow_redirects)
+
+    rsp = session.put(url, headers=headers, data=data, allow_redirects=allow_redirects)
     return rsp
 
 
-def send_delete_request(url, token, headers):
+def send_delete_request(session, url, token, headers):
     headers["Authorization"] = _append_bearer(token)
 
-    rsp = requests.delete(url, headers=headers)
+    rsp = session.delete(url, headers=headers)
     return rsp
 
+
 # =============================================================================
 # private functions
 
+
 def _append_bearer(access_token):
     if "Bearer" in access_token:
         return access_token
-    return "Bearer " + access_token
+    return "Bearer " + access_token
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/solve.py` & `decision_optimization_client-1.1.1/decision_optimization_client/solve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import json
 
 from six import string_types
 
 from .base_resource import DDObject
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/table.py` & `decision_optimization_client-1.1.1/decision_optimization_client/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 import json
 
 from six import string_types
 
 from .base_resource import DDObject
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client/token.py` & `decision_optimization_client-1.1.1/decision_optimization_client/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2017, 2022
+# (c) Copyright IBM Corp. 2017, 2024
 # --------------------------------------------------------------------------
 
 from os import environ
 import requests
 
 class Token(object):
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client.egg-info/PKG-INFO` & `decision_optimization_client-1.1.1/decision_optimization_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decision-optimization-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: The IBM Decision Optimization Scenario Python client
 Author: The IBM Decision Optimization on team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -203,7 +203,9 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 License-File: LICENSE.txt
+Requires-Dist: requests
+Requires-Dist: six
```

### Comparing `decision_optimization_client-1.1.0/decision_optimization_client.egg-info/SOURCES.txt` & `decision_optimization_client-1.1.1/decision_optimization_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decision_optimization_client-1.1.0/setup.py` & `decision_optimization_client-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     try:
         with open(os.path.join(HERE, *parts)) as f:
             return f.read()
     except:
         return None
 
 setup(name='decision_optimization_client',
-      version='1.1.0', # Check version number on either test pypi or official pypi (depending on where you want to push this)
+      version='1.1.1', # Check version number on either test pypi or official pypi (depending on where you want to push this)
       description='The IBM Decision Optimization Scenario Python client',
       author='The IBM Decision Optimization on team',
       packages=['decision_optimization_client'],
       include_package_data=True,
       install_requires=required,
       license=read('LICENSE.txt')
       )
```

