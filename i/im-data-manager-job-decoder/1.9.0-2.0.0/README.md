# Comparing `tmp/im-data-manager-job-decoder-1.9.0.tar.gz` & `tmp/im-data-manager-job-decoder-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im-data-manager-job-decoder-1.9.0.tar", last modified: Tue May  3 17:57:09 2022, max compression
+gzip compressed data, was "im-data-manager-job-decoder-2.0.0.tar", last modified: Thu Apr 11 16:31:16 2024, max compression
```

## Comparing `im-data-manager-job-decoder-1.9.0.tar` & `im-data-manager-job-decoder-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.916736 im-data-manager-job-decoder-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/decoder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1833 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/decode_jinja2_3_0.py
--rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/decoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/job-definition-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/decoder/manifest-schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 17:57:09.912736 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2439 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 17:57:07.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-05-03 17:57:09.000000 im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-03 17:57:09.916736 im-data-manager-job-decoder-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-05-03 17:56:57.000000 im-data-manager-job-decoder-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:31:16.180104 im-data-manager-job-decoder-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-11 16:31:16.180104 im-data-manager-job-decoder-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:31:16.176104 im-data-manager-job-decoder-2.0.0/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/decoder/decode_jinja2_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/decoder/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/decoder/job-definition-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/decoder/manifest-schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:31:16.180104 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:31:16.000000 im-data-manager-job-decoder-2.0.0/im_data_manager_job_decoder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:31:16.180104 im-data-manager-job-decoder-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:31:16.180104 im-data-manager-job-decoder-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_decode_jinja2_3_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_asset_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_environment_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_file_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_job_doc_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_jobs_replaced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_get_pull_secret_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_validate_job_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-11 16:31:11.000000 im-data-manager-job-decoder-2.0.0/tests/test_validate_manifest.py
```

### Comparing `im-data-manager-job-decoder-1.9.0/LICENSE` & `im-data-manager-job-decoder-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.9.0/PKG-INFO` & `im-data-manager-job-decoder-2.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-Metadata-Version: 2.1
-Name: im-data-manager-job-decoder
-Version: 1.9.0
-Summary: Job decoding logic
-Home-page: https://github.com/informaticsmatters/data-manager-job-decoder
-Author: Alan Christie
-Author-email: achristie@informaticsmatters.com
-License: MIT
-Keywords: jinja2 decoder
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Other Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: POSIX :: Linux
-License-File: LICENSE
-
 Informatics Matters Data Manager Job Decoder
 ============================================
 
 .. image:: https://badge.fury.io/py/im-data-manager-job-decoder.svg
    :target: https://badge.fury.io/py/im-data-manager-job-decoder
    :alt: PyPI package (latest)
 
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/build.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/build.yaml
+   :alt: Build
+
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/publish.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/publish.yaml
+   :alt: Publish
+
 A package that simplifies the decoding of encoded text strings.
 Given an encoded string the ``decode()`` method
 returns the decoded value or an error.
 
 For example, given the following `jinja2`_ encoded string
 ``'{{ foo }}, bar={{ bar }}, baz={{ baz }}'`` and variable map
 ``{'foo': 1, 'bar': 2, 'baz': 3}`` the decoder returns
@@ -49,27 +38,43 @@
 
 The Job decoder is published on `PyPI`_ and can be installed from
 there::
 
     pip install im-data-manager-job-decoder
 
 Once installed you can validate the definition (expected to be a dictionary
-formed from the definition YAML file) with:
-
->>> from decoder import decoder
->>> error = decoder.validate_manifest_schema(manifest)
->>> error = decoder.validate_job_schema(job_definition)
+formed from the definition YAML file) with::
 
-And run the decoder with:
+    >>> from decoder import decoder
+    >>> error: Optional[str] = decoder.validate_manifest_schema(manifest)
+    >>> error: Optional[str] = decoder.validate_job_schema(job_definition)
+
+And you can decode encoded fields within the job definition.
+Here we're decoding the job's 'command' using a map of variables and their
+values::
+
+    >>> decoded, success = decoder.decode(definition['command'],
+                                          variables,
+                                          'command',
+                                          decoder.TextEncoding.JINJA2_3_0)
+
+A method also exists to generate a Data Manger Job documentation URL
+for the supported repository types. For example, to get the
+auto-generated documentation URL for a job definition hosted in a GitHub
+repository you can do this::
+
+    >>> doc_url: str = decoder.get_job_doc_url("github",
+                                               collection
+                                               job_id,
+                                               job_definition,
+                                               manifest_url)
 
->>> decoded, success = decoder.decode(text, variables, 'command', decoder.TextEncoding.JINJA2_3_0)
+We support ``github`` and ``gitlab`` as repository types.
 
 .. _PyPI: https://pypi.org/project/im-data-manager-job-decoder
 
 Get in touch
 ============
 
 - Report bugs, suggest features or view the source code `on GitHub`_.
 
-.. _on GitHub: https://github.com/informaticsmatters/data-manager-job-decoder
-
-
+.. _on GitHub: https://github.com/informaticsmatters/squonk2-data-manager-job-decoder
```

### Comparing `im-data-manager-job-decoder-1.9.0/decoder/decode_jinja2_3_0.py` & `im-data-manager-job-decoder-2.0.0/decoder/decode_jinja2_3_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """A decoder for jinja2 3.0.x formatted strings.
 """
+
 from typing import Dict, Optional, Set, Tuple
 
 import jinja2
 from jinja2.exceptions import TemplateSyntaxError
 from jinja2.meta import find_undeclared_variables
```

### Comparing `im-data-manager-job-decoder-1.9.0/decoder/manifest-schema.yaml` & `im-data-manager-job-decoder-2.0.0/decoder/manifest-schema.yaml`

 * *Files identical despite different names*

### Comparing `im-data-manager-job-decoder-1.9.0/im_data_manager_job_decoder.egg-info/PKG-INFO` & `im-data-manager-job-decoder-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 Metadata-Version: 2.1
 Name: im-data-manager-job-decoder
-Version: 1.9.0
+Version: 2.0.0
 Summary: Job decoding logic
-Home-page: https://github.com/informaticsmatters/data-manager-job-decoder
+Home-page: https://github.com/informaticsmatters/squonk2-data-manager-job-decoder
 Author: Alan Christie
 Author-email: achristie@informaticsmatters.com
 License: MIT
 Keywords: jinja2 decoder
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.10
 License-File: LICENSE
+Requires-Dist: jinja2==3.1.3
+Requires-Dist: jsonschema<5.0,>=4.21.1
+Requires-Dist: pyyaml<7.0,>=5.3.1
 
 Informatics Matters Data Manager Job Decoder
 ============================================
 
 .. image:: https://badge.fury.io/py/im-data-manager-job-decoder.svg
    :target: https://badge.fury.io/py/im-data-manager-job-decoder
    :alt: PyPI package (latest)
 
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/build.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/build.yaml
+   :alt: Build
+
+.. image:: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/publish.yaml/badge.svg
+   :target: https://github.com/InformaticsMatters/squonk2-data-manager-job-decoder/actions/workflows/publish.yaml
+   :alt: Publish
+
 A package that simplifies the decoding of encoded text strings.
 Given an encoded string the ``decode()`` method
 returns the decoded value or an error.
 
 For example, given the following `jinja2`_ encoded string
 ``'{{ foo }}, bar={{ bar }}, baz={{ baz }}'`` and variable map
 ``{'foo': 1, 'bar': 2, 'baz': 3}`` the decoder returns
@@ -49,27 +63,43 @@
 
 The Job decoder is published on `PyPI`_ and can be installed from
 there::
 
     pip install im-data-manager-job-decoder
 
 Once installed you can validate the definition (expected to be a dictionary
-formed from the definition YAML file) with:
-
->>> from decoder import decoder
->>> error = decoder.validate_manifest_schema(manifest)
->>> error = decoder.validate_job_schema(job_definition)
+formed from the definition YAML file) with::
 
-And run the decoder with:
+    >>> from decoder import decoder
+    >>> error: Optional[str] = decoder.validate_manifest_schema(manifest)
+    >>> error: Optional[str] = decoder.validate_job_schema(job_definition)
+
+And you can decode encoded fields within the job definition.
+Here we're decoding the job's 'command' using a map of variables and their
+values::
+
+    >>> decoded, success = decoder.decode(definition['command'],
+                                          variables,
+                                          'command',
+                                          decoder.TextEncoding.JINJA2_3_0)
+
+A method also exists to generate a Data Manger Job documentation URL
+for the supported repository types. For example, to get the
+auto-generated documentation URL for a job definition hosted in a GitHub
+repository you can do this::
+
+    >>> doc_url: str = decoder.get_job_doc_url("github",
+                                               collection
+                                               job_id,
+                                               job_definition,
+                                               manifest_url)
 
->>> decoded, success = decoder.decode(text, variables, 'command', decoder.TextEncoding.JINJA2_3_0)
+We support ``github`` and ``gitlab`` as repository types.
 
 .. _PyPI: https://pypi.org/project/im-data-manager-job-decoder
 
 Get in touch
 ============
 
 - Report bugs, suggest features or view the source code `on GitHub`_.
 
-.. _on GitHub: https://github.com/informaticsmatters/data-manager-job-decoder
-
-
+.. _on GitHub: https://github.com/informaticsmatters/squonk2-data-manager-job-decoder
```

### Comparing `im-data-manager-job-decoder-1.9.0/setup.py` & `im-data-manager-job-decoder-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,30 +17,33 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="im-data-manager-job-decoder",
     version=os.environ.get("GITHUB_REF_SLUG", "1.0.0"),
     author="Alan Christie",
     author_email="achristie@informaticsmatters.com",
-    url="https://github.com/informaticsmatters/data-manager-job-decoder",
+    url="https://github.com/informaticsmatters/squonk2-data-manager-job-decoder",
     license="MIT",
     description="Job decoding logic",
     long_description=long_description,
     keywords="jinja2 decoder",
     platforms=["any"],
+    python_requires=">=3.10",
     # Our modules to package
     packages=["decoder"],
     include_package_data=True,
     # Project classification:
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Operating System :: POSIX :: Linux",
     ],
     install_requires=requirements,
     zip_safe=False,
 )
```

