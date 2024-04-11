# Comparing `tmp/cortex-python-6.4.0a3.tar.gz` & `tmp/cortex_python-6.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex-python-6.4.0a3.tar", last modified: Thu Mar  7 20:15:01 2024, max compression
+gzip compressed data, was "cortex_python-6.5.0a1.tar", max compression
```

## Comparing `cortex-python-6.4.0a3.tar` & `cortex_python-6.5.0a1.tar`

### file list

```diff
@@ -1,54 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.197058 cortex-python-6.4.0a3/
--rw-r--r--   0 root         (0) root         (0)      977 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    11368 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      132 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4623 2024-03-07 20:15:01.197058 cortex-python-6.4.0a3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3938 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.193058 cortex-python-6.4.0a3/cortex/
--rw-r--r--   0 root         (0) root         (0)      667 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/__version__.py
--rw-r--r--   0 root         (0) root         (0)     1600 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/auth.py
--rw-r--r--   0 root         (0) root         (0)     1989 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/camel.py
--rw-r--r--   0 root         (0) root         (0)    27238 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/client.py
--rw-r--r--   0 root         (0) root         (0)     3428 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/connection.py
--rw-r--r--   0 root         (0) root         (0)      684 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/constant.py
--rw-r--r--   0 root         (0) root         (0)     9669 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/content.py
--rw-r--r--   0 root         (0) root         (0)     2532 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/env.py
--rw-r--r--   0 root         (0) root         (0)     2477 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.193058 cortex-python-6.4.0a3/cortex/experiment/
--rw-r--r--   0 root         (0) root         (0)      675 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7794 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/experiment/local.py
--rw-r--r--   0 root         (0) root         (0)    10770 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/experiment/model.py
--rw-r--r--   0 root         (0) root         (0)    37474 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/experiment/remote.py
--rw-r--r--   0 root         (0) root         (0)     3195 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/message.py
--rw-r--r--   0 root         (0) root         (0)     4387 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/model.py
--rw-r--r--   0 root         (0) root         (0)    10071 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/properties.py
--rw-r--r--   0 root         (0) root         (0)     2517 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/secrets.py
--rw-r--r--   0 root         (0) root         (0)    11705 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/serviceconnector.py
--rw-r--r--   0 root         (0) root         (0)     4460 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/session.py
--rw-r--r--   0 root         (0) root         (0)     8521 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/skill.py
--rw-r--r--   0 root         (0) root         (0)     1347 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/timer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/types.py
--rw-r--r--   0 root         (0) root         (0)     8865 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/utils.py
--rw-r--r--   0 root         (0) root         (0)     4410 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/cortex/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.193058 cortex-python-6.4.0a3/cortex_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4623 2024-03-07 20:15:01.000000 cortex-python-6.4.0a3/cortex_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1040 2024-03-07 20:15:01.000000 cortex-python-6.4.0a3/cortex_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-07 20:15:01.000000 cortex-python-6.4.0a3/cortex_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2024-03-07 20:15:01.000000 cortex-python-6.4.0a3/cortex_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-07 20:15:01.000000 cortex-python-6.4.0a3/cortex_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-07 20:15:01.197058 cortex-python-6.4.0a3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2176 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.193058 cortex-python-6.4.0a3/test/
--rw-r--r--   0 root         (0) root         (0)      590 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-07 20:15:01.197058 cortex-python-6.4.0a3/test/unit/
--rw-r--r--   0 root         (0) root         (0)      590 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/authenticationclient_test.py
--rw-r--r--   0 root         (0) root         (0)     4052 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/connectionclient_test.py
--rw-r--r--   0 root         (0) root         (0)     9029 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/cortex_test.py
--rw-r--r--   0 root         (0) root         (0)     5216 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/environment_config_test.py
--rw-r--r--   0 root         (0) root         (0)     6424 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/experiment_test.py
--rw-r--r--   0 root         (0) root         (0)     2933 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/fixtures.py
--rw-r--r--   0 root         (0) root         (0)     8439 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/run_test.py
--rw-r--r--   0 root         (0) root         (0)     1761 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/serviceconnector_test.py
--rw-r--r--   0 root         (0) root         (0)     3111 2024-03-07 20:12:51.000000 cortex-python-6.4.0a3/test/unit/sessionclient_test.py
+-rw-r--r--   0        0        0    11368 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/LICENSE
+-rw-r--r--   0        0        0     4059 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/README.md
+-rw-r--r--   0        0        0      667 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/cortex/__init__.py
+-rw-r--r--   0        0        0     1600 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/cortex/auth.py
+-rw-r--r--   0        0        0     1989 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/cortex/camel.py
+-rw-r--r--   0        0        0    27332 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/cortex/client.py
+-rw-r--r--   0        0        0     3428 2024-04-10 21:15:32.851398 cortex_python-6.5.0a1/cortex/connection.py
+-rw-r--r--   0        0        0      684 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/constant.py
+-rw-r--r--   0        0        0     9669 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/content.py
+-rw-r--r--   0        0        0     2532 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/env.py
+-rw-r--r--   0        0        0     2477 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/exceptions.py
+-rw-r--r--   0        0        0      675 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/experiment/__init__.py
+-rw-r--r--   0        0        0     7794 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/experiment/local.py
+-rw-r--r--   0        0        0    10717 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/experiment/model.py
+-rw-r--r--   0        0        0    37474 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/experiment/remote.py
+-rw-r--r--   0        0        0     3195 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/message.py
+-rw-r--r--   0        0        0     3014 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/models.py
+-rw-r--r--   0        0        0    10071 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/properties.py
+-rw-r--r--   0        0        0     2517 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/secrets.py
+-rw-r--r--   0        0        0    11766 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/serviceconnector.py
+-rw-r--r--   0        0        0     4460 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/session.py
+-rw-r--r--   0        0        0     8521 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/skill.py
+-rw-r--r--   0        0        0     1347 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/timer.py
+-rw-r--r--   0        0        0     1950 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/types.py
+-rw-r--r--   0        0        0     8997 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/utils.py
+-rw-r--r--   0        0        0     4410 2024-04-10 21:15:32.855398 cortex_python-6.5.0a1/cortex/viz.py
+-rw-r--r--   0        0        0     1712 2024-04-10 21:19:27.818851 cortex_python-6.5.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 cortex_python-6.5.0a1/PKG-INFO
```

### Comparing `cortex-python-6.4.0a3/LICENSE` & `cortex_python-6.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/PKG-INFO` & `cortex_python-6.5.0a1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,68 @@
-Metadata-Version: 2.1
-Name: cortex-python
-Version: 6.4.0a3
-Summary: Python module for the CognitiveScale Cortex Cognitive Platform
-Home-page: https://github.com/CognitiveScale/cortex-python
-Author: CognitiveScale
-Author-email: support@cognitivescale.com
-License: Apache 2.0
-Project-URL: Documentation, https://cognitivescale.github.io/cortex-python/master/
-Project-URL: Source, https://github.com/CognitiveScale/cortex-python
-Platform: any
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
-Provides-Extra: viz
-Provides-Extra: jupyter
-License-File: LICENSE
-
 # Python Module for the Cortex Cognitive Platform
 
 The Cortex Python module provides an API client library to easily integrate with the Cortex Cognitive Platform. 
 Refer to the Cortex documentation for details on how to use the library: 
 
 - Developer guide: https://cognitivescale.github.io/cortex-fabric/
 - Cortex Python references: https://cognitivescale.github.io/cortex-python/master/
 
 ## Installation
 
 To install: 
-```
-  > pip install cortex-python
+
+```bash
+pip install cortex-python
 ```
 
 or from source code:
-```
-  > git clone git@github.com:CognitiveScale/cortex-python.git
-  > cd cortex-python
-  > pip install -e .
+
+```bash
+git clone git@github.com:CognitiveScale/cortex-python.git
+cd cortex-python
+pip install -e .
 ```
 
 To install the optional components: 
+
+When developing models using jupyter within notebooks
+
+```bash
+poetry install cortex-python[models_dev]
 ```
-  > pip install cortex-python[viz]
-  > pip install cortex-python[jupyter]
+
+When using model SDK using jupyter within notebooks
+
+```bash
+poetry install cortex-python[models_dev]
+```
+
+When 
+
+```bash
+poetry install cortex-python[models_dev]
 ```
 
 ## Development 
 
 ### Setup
 
 When developing, it's a best practice to work in a virtual environment. Create and activate a virtual environment:
-```
-  > virtualenv --python=python3.10 _venv
-  > source _venv/bin/activate
+
+```bash
+poetry install
+poetry shell
 ```
 
 Install developer dependencies:
 
-```
-  > git clone git@github.com:CognitiveScale/cortex-python.git
-  > cd cortex-python
-  > make dev.install
+```bash
+git clone git@github.com:CognitiveScale/cortex-python.git
+cd cortex-python
+make dev.install
 ```
 
 Run Developer test and linting tasks:
 Three types of checks are configured for this:
 1. [symilar](https://pylint.readthedocs.io/en/v2.16.2/symilar.html) - to test code duplication
 2. [pylint](https://pylint.readthedocs.io/en/v2.16.2/) - for linting
 3. [pytest](https://docs.pytest.org/en/7.2.x/) - for running the unit tests. These are orchestrated through [tox](https://tox.wiki/en/3.27.1/). The tox configuration is available at [`tox.ini`](/tox.ini)
@@ -99,44 +97,49 @@
 1. Run unit tests via `make test`
 2. Manually verification (i.e. try the new changes out in Cortex) to make sure everything is going well. Not required, but highly encouraged.
 3. Bump up `setup.py` version and update the `CHANGELOG.md` 
 
 ### Documentation
 
 Activate your virtual environment:
-```
-> source _venv/bin/activate
+
+```bash
+poetry shell
 ```
 
 Set up your environment, if you have not done so:
-```
-> make dev.install 
+
+```bash
+make dev.install 
 ```
 
 The package documentation is built with Sphinx and generates versioned documentation for all tag matching the `release/X.Y.Z` pattern and for the `master` branch. To build the documentation:
 
-```
-> make docs.multi
+```bash
+make docs.multi
 ```
 The documentation will be rendered in HTML format under the `docs/_build/${VERSION}` directory.
 
 ### Pre-release to staging
 
 1. Create and push an alpha release:
-    ```
-    > make dev.push
-    ```
+
+```bash
+make dev.push
+```
     This will build an alpha-tagged package.
 2. Merge `develop` to `staging` branch:
-    ```
-    > make stage
-    ```
+
+```bash
+make stage
+```
+
 3. In GitHub, create a pull request from `staging` to `master`.
 
 
 ## TODO
 - [x] extending the client with helpers for cortex resources 
 - [x] camelcase in pylinyrc
 - [ ] Update all documentation with proper Sphinx formatting
   - [x] Most of the major modules have been fixed except skill.py, model.py
 - [x] use exceptions defined in `cortex/exceptions.py`
-- [ ] integrate the cortex-python-profiles package back into the python SDK
+- [ ] integrate the cortex-python-profiles package back into the python SDK
```

### Comparing `cortex-python-6.4.0a3/cortex/__init__.py` & `cortex_python-6.5.0a1/cortex/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/auth.py` & `cortex_python-6.5.0a1/cortex/auth.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/camel.py` & `cortex_python-6.5.0a1/cortex/camel.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/client.py` & `cortex_python-6.5.0a1/cortex/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import os
 import time
 from .constant import VERSION
 from .experiment.local import LocalExperiment
 from .connection import ConnectionClient
 from .content import ManagedContentClient
-from .model import ModelClient
+from .models import ModelClient
 from .secrets import SecretsClient
 from .session import SessionClient
 from .skill import SkillClient
 from .types import TypeClient
 from .experiment import ExperimentClient
 from .serviceconnector import ServiceConnector
 from .env import CortexEnv
@@ -121,14 +121,15 @@
         url: str,
         token: _Token = None,
         config: dict = None,
         project: str = None,
         version: int = VERSION,
         verify_ssl_cert: bool = False,
     ):
+        self._serviceconnector = None
         self._token = token
         self._config = config
         self._project = project
         self._url = url
         self._version = version
         self._verify_ssl_cert = verify_ssl_cert
 
@@ -147,15 +148,16 @@
         """Constructs a Message from payload and properties if given. This is useful for
         testing skills, as this the message passed when skills are invoked
         :param payload: The payload to include in the Message.
         :param properties: The properties to include in the Message.
         :return: A Message object.
         """
         if not self._token.token:
-            self._token = _Token(generate_token(self._config))
+            self._token = _Token(generate_token(self._serviceconnector._config))  # pylint: disable=protected-access
+
         params = {"payload": payload}
         if properties:
             params["properties"] = properties
         params["apiEndpoint"] = self._url
         params["token"] = self._token.token
         return Message(params)
```

### Comparing `cortex-python-6.4.0a3/cortex/connection.py` & `cortex_python-6.5.0a1/cortex/connection.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/constant.py` & `cortex_python-6.5.0a1/cortex/constant.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/content.py` & `cortex_python-6.5.0a1/cortex/content.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/env.py` & `cortex_python-6.5.0a1/cortex/env.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/exceptions.py` & `cortex_python-6.5.0a1/cortex/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/experiment/__init__.py` & `cortex_python-6.5.0a1/cortex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/experiment/local.py` & `cortex_python-6.5.0a1/cortex/experiment/local.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/experiment/model.py` & `cortex_python-6.5.0a1/cortex/experiment/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-
 import cuid
 from ..timer import Timer
 from ..exceptions import ConfigurationException
 
 
 class Run:
     # pylint: disable=too-many-instance-attributes,too-many-public-methods
@@ -267,15 +266,14 @@
             return np.asscalar(arr)
         return arr
 
 
 def _to_html(exp):
     # pylint: disable=import-outside-toplevel
     try:
-        import maya
         from jinja2 import Template
     except (ImportError, NameError) as exc:
         raise ConfigurationException(
             "The jupyter extras are required to use this,"
             'please install using "pip install cortex-python[viz]"'
         ) from exc
 
@@ -330,15 +328,15 @@
                             {% endfor %}
                         </tr>
                         </thead>
                         <tbody>
                             {% for run in runs %}
                             <tr>
                             <td>{{run.id}}</td>
-                            <td>{{maya(run.start_time)}}</td>
+                            <td>{{run.start_time}}</td>
                             <td>{{'%.2f' % run.took}} s</td>
                             {% for param in param_names %}
                             <td>{{run.params.get(param, "&#x2011;")}}</td>
                             {% endfor %}
                             {% for metric in metric_names %}
                             <td>{{'%.6f' % run.metrics.get(metric, 0.0)}}</td>
                             {% endfor %}
@@ -358,13 +356,12 @@
             metric_names.update(one_run.metrics.keys())
             num_metrics = len(metric_names)
 
     tmpl = Template(template)
     return tmpl.render(
         name=exp.name,
         runs=runs,
-        maya=maya.MayaDT,
         num_params=num_params,
         param_names=sorted(list(param_names)),
         num_metrics=num_metrics,
         metric_names=sorted(list(metric_names)),
     )
```

### Comparing `cortex-python-6.4.0a3/cortex/experiment/remote.py` & `cortex_python-6.5.0a1/cortex/experiment/remote.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/message.py` & `cortex_python-6.5.0a1/cortex/message.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/properties.py` & `cortex_python-6.5.0a1/cortex/properties.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/secrets.py` & `cortex_python-6.5.0a1/cortex/secrets.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/serviceconnector.py` & `cortex_python-6.5.0a1/cortex/serviceconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,26 @@
 import json
 import platform
 import sys
 from typing import Dict, Any, List, Union, Optional, Type, TypeVar
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
-
+from importlib_metadata import metadata
 from .constant import VERSION
-from .__version__ import __version__, __title__
-
 from .utils import get_logger, get_cortex_profile, verify_JWT, generate_token
 from .utils import raise_for_status_with_detail
 
 log = get_logger(__name__)
 
 JSONType = Union[str, int, float, bool, None, Dict[str, Any], List[Any]]
 T = TypeVar("T", bound="_Client")
-
+package_meta = metadata('cortex-python')
 userAgent = (
-    f"{__title__}/{__version__} ({sys.platform};"
+    f"{package_meta.get('Name')}/{package_meta.get('Version')} ({sys.platform};"
     f"{platform.architecture()[0]}; {platform.release()})"
 )
 
 
 class ServiceConnector:
     """
     Defines the settings and security credentials required to access a service.
```

### Comparing `cortex-python-6.4.0a3/cortex/session.py` & `cortex_python-6.5.0a1/cortex/session.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/skill.py` & `cortex_python-6.5.0a1/cortex/skill.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/timer.py` & `cortex_python-6.5.0a1/cortex/timer.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/types.py` & `cortex_python-6.5.0a1/cortex/types.py`

 * *Files identical despite different names*

### Comparing `cortex-python-6.4.0a3/cortex/utils.py` & `cortex_python-6.5.0a1/cortex/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
 import json
 import base64
 import hashlib
 import logging
 import urllib.parse
 from collections import namedtuple
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import Union
 
 import python_jwt as py_jwt
 import jwcrypto.jwk as jwkLib
+from pytimeparse2 import parse
 from requests.exceptions import HTTPError
 from requests import request
 from .exceptions import BadTokenException, AuthenticationHeaderError
 
 
 def md5sum(file_name, blocksize=65536):
     """
@@ -148,38 +149,38 @@
     return request("GET", uri, headers=headers, verify=verify_ssl_cert,).json()
 
 
 def _get_fabric_server_ts(config: dict, verify_ssl_cert: Union[bool, str]=True):
     return _get_fabric_info(config, verify_ssl_cert).get("serverTs")
 
 
-def generate_token(config, verify_ssl_cert: Union[bool, str]=True, validity=2):
+def generate_token(config, verify_ssl_cert: Union[bool, str, None]=True, validity: Union[int, str, None]='2m'):
     """
     Use the Personal Access Token (JWK) obtained from Cortex's console
     to generate JWTs to access cortex services..
     
     :param verify_ssl_cert: (optional) Either a boolean, in which case it controls whether we verify
             the server's TLS certificate, or a string, in which case it must be a path
             to a CA bundle to use. Defaults to ``True``.
+    :param validity: (optional) Token validity duration. Defaults to `2m`
     """
     try:
         server_ts = int(
             _get_fabric_server_ts(config, verify_ssl_cert) / 1000
         )  # fabric info returns serverTs in milliseconds
         key = jwkLib.JWK.from_json(json.dumps(config.get("jwk")))
         token_payload = {
             "iss": config.get("issuer"),
             "aud": config.get("audience"),
             "sub": config.get("username"),
             "iat": server_ts / 1000,
         }
 
         server_ts_dt = datetime.fromtimestamp(server_ts, tz=timezone.utc)
-
-        expiry = server_ts_dt + timedelta(minutes=validity)
+        expiry = server_ts_dt + parse(validity, as_timedelta=True)
 
         token = py_jwt.generate_jwt(
             claims=token_payload,
             priv_key=key,
             algorithm="EdDSA",
             expires=expiry,
             other_headers={
```

### Comparing `cortex-python-6.4.0a3/cortex/viz.py` & `cortex_python-6.5.0a1/cortex/viz.py`

 * *Files identical despite different names*

