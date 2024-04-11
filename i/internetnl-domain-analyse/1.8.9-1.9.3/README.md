# Comparing `tmp/internetnl_domain_analyse-1.8.9.tar.gz` & `tmp/internetnl_domain_analyse-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetnl_domain_analyse-1.8.9.tar", last modified: Wed Apr 10 20:31:39 2024, max compression
+gzip compressed data, was "internetnl_domain_analyse-1.9.3.tar", last modified: Thu Apr 11 18:52:44 2024, max compression
```

## Comparing `internetnl_domain_analyse-1.8.9.tar` & `internetnl_domain_analyse-1.9.3.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.928037 internetnl_domain_analyse-1.8.9/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/.coveragerc
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      461 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/.readthedocs.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/AUTHORS.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      893 2024-04-10 20:30:31.000000 internetnl_domain_analyse-1.8.9/CHANGELOG.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    14049 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/CONTRIBUTING.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/LICENSE.txt
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1609 2024-04-10 20:31:39.928037 internetnl_domain_analyse-1.8.9/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/README.rst
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.916036 internetnl_domain_analyse-1.8.9/docs/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/Makefile
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.916036 internetnl_domain_analyse-1.8.9/docs/_static/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/_static/.gitignore
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/authors.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/changelog.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     9808 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/conf.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/contributing.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2314 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/index.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/license.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/docs/readme.rst
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.8.9/docs/requirements.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.920037 internetnl_domain_analyse-1.8.9/examples/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/examples/domain_analyse_settings.yml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/pyproject.toml
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.8.9/requirements.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1631 2024-04-10 20:31:39.928037 internetnl_domain_analyse-1.8.9/setup.cfg
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/setup.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.912036 internetnl_domain_analyse-1.8.9/src/
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.924037 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/__init__.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    71906 2024-04-10 19:36:35.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domain_analyse_classes.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domain_plots.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domein_analyse.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/latex_output.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/public_suffix_list.dat
--rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/utils.py
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.924037 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/
--rw-r--r--   0 eelco     (1000) eelco     (1000)     1609 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/PKG-INFO
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     1130 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/dependency_links.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/entry_points.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/not-zip-safe
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/requires.txt
--rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-10 20:31:39.000000 internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/top_level.txt
-drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-10 20:31:39.924037 internetnl_domain_analyse-1.8.9/tests/
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/tests/conftest.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.8.9/tests/test_internetnl_scan.py
--rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.8.9/tox.ini
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      598 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/.coveragerc
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      550 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      264 2024-04-11 18:45:46.000000 internetnl_domain_analyse-1.9.3/.pre-commit-config.yaml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1030 2024-04-11 18:45:43.000000 internetnl_domain_analyse-1.9.3/.readthedocs.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       50 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/AUTHORS.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      920 2024-04-11 18:50:41.000000 internetnl_domain_analyse-1.9.3/CHANGELOG.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    12063 2024-04-11 18:39:44.000000 internetnl_domain_analyse-1.9.3/CONTRIBUTING.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1071 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/LICENSE.txt
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      382 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/README.rst
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/docs/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/Makefile
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/docs/_static/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       18 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/_static/.gitignore
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       41 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/authors.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       43 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/changelog.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     9868 2024-04-11 18:47:22.000000 internetnl_domain_analyse-1.9.3/docs/conf.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       33 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/contributing.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1427 2024-04-11 18:40:55.000000 internetnl_domain_analyse-1.9.3/docs/index.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       67 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/license.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       39 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/docs/readme.rst
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      385 2024-04-10 20:29:58.000000 internetnl_domain_analyse-1.9.3/docs/requirements.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.263559 internetnl_domain_analyse-1.9.3/examples/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   107886 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/examples/domain_analyse_settings.yml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      311 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/pyproject.toml
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      153 2024-04-10 19:59:19.000000 internetnl_domain_analyse-1.9.3/requirements.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1689 2024-04-11 18:52:44.275560 internetnl_domain_analyse-1.9.3/setup.cfg
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      722 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/setup.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.259559 internetnl_domain_analyse-1.9.3/src/
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.267559 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      577 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/__init__.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    71935 2024-04-11 18:06:06.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_analyse_classes.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    44531 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_plots.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    17345 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domein_analyse.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     7022 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/latex_output.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)   241248 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/public_suffix_list.dat
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)    15460 2024-04-10 20:02:21.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/utils.py
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.271560 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/
+-rw-r--r--   0 eelco     (1000) eelco     (1000)     1667 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/PKG-INFO
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     1154 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/dependency_links.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       92 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/entry_points.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)        1 2024-04-10 19:31:37.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/not-zip-safe
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      285 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/requires.txt
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)       26 2024-04-11 18:52:44.000000 internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/top_level.txt
+drwxrwxr-x   0 eelco     (1000) eelco     (1000)        0 2024-04-11 18:52:44.271560 internetnl_domain_analyse-1.9.3/tests/
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      293 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/tests/conftest.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)      237 2024-04-10 20:26:08.000000 internetnl_domain_analyse-1.9.3/tests/test_internetnl_scan.py
+-rw-rw-r--   0 eelco     (1000) eelco     (1000)     2009 2024-04-10 12:54:04.000000 internetnl_domain_analyse-1.9.3/tox.ini
```

### Comparing `internetnl_domain_analyse-1.8.9/.coveragerc` & `internetnl_domain_analyse-1.9.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/.gitignore` & `internetnl_domain_analyse-1.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/CHANGELOG.rst` & `internetnl_domain_analyse-1.9.3/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 =========
 Changelog
 =========
 
-Version 1.8.9
+Version 1.9.3
 =============
 - Nu statistieken op basis van weighted_sample_statistics
+- Force calculate included
 
 Version 1.8.7
 =============
 - Nu kan je breakdowns ook als combinaties geven. Nodig voor publicatie 2023
 - legend default aan plaatjes toegevoegd nu we meerdere jaren hebben
 - eval statement kan gebruikt worden om afgeleide kolommen te maken
 - dump cache as sqlite optie. Duplicated kolommen worden verwijderd
```

### Comparing `internetnl_domain_analyse-1.8.9/CONTRIBUTING.rst` & `internetnl_domain_analyse-1.9.3/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-.. todo:: THIS IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
-
-   The document assumes you are using a source repository service that promotes a
-   contribution model similar to `GitHub's fork and pull request workflow`_.
-   While this is true for the majority of services (like GitHub, GitLab,
-   BitBucket), it might not be the case for private repositories (e.g., when
-   using Gerrit).
-
-   Also notice that the code examples might refer to GitHub URLs or the text
-   might use GitHub specific terminology (e.g., *Pull Request* instead of *Merge
-   Request*).
-
-   Please make sure to check the document having these assumptions in mind
-   and update things accordingly.
-
-.. todo:: Provide the correct links/replacements at the bottom of the document.
-
-.. todo:: You might want to have a look on `PyScaffold's contributor's guide`_,
-
-   especially if your project is open source. The text should be very similar to
-   this template, but there are a few extra contents that you might decide to
-   also include, like mentioning labels of your issue tracker or automated
-   releases.
-
-
 ============
 Contributing
 ============
 
 Welcome to ``internetnl_domain_analyse`` contributor's guide.
 
 This document focuses on getting any potential contributor familiarized
@@ -68,20 +43,14 @@
 You can help improve ``internetnl_domain_analyse`` docs by making them more readable and coherent, or
 by adding missing information and correcting mistakes.
 
 ``internetnl_domain_analyse`` documentation uses Sphinx_ as its main documentation compiler.
 This means that the docs are kept in the same repository as the project code, and
 that any documentation update is done in the same way was a code contribution.
 
-.. todo:: Don't forget to mention which markup language you are using.
-
-    e.g.,  reStructuredText_ or CommonMark_ with MyST_ extensions.
-
-.. todo:: If your project is hosted on GitHub, you can also mention the following tip:
-
    .. tip::
       Please notice that the `GitHub web interface`_ provides a quick way of
       propose changes in ``internetnl_domain_analyse``'s files. While this mechanism can
       be tricky for normal code contributions, it works perfectly fine for
       contributing to the docs, and can be quite handy.
 
       If you are interested in trying this method out, please navigate to
@@ -102,20 +71,14 @@
 
     python3 -m http.server --directory 'docs/_build/html'
 
 
 Code Contributions
 ==================
 
-.. todo:: Please include a reference or explanation about the internals of the project.
-
-   An architecture description, design principles or at least a summary of the
-   main concepts will make it easy for potential contributors to get started
-   quickly.
-
 Submit an issue
 ---------------
 
 Before you work on any non-trivial code contribution it's best to first create
 a report in the `issue tracker`_ to start a discussion on the subject.
 This often provides additional considerations and avoids unnecessary work.
 
@@ -147,16 +110,14 @@
 
 #. You should run::
 
     pip install -U pip setuptools -e .
 
    to be able to import the package under development in the Python REPL.
 
-   .. todo:: if you are not using pre-commit, please remove the following item:
-
 #. Install |pre-commit|_::
 
     pip install pre-commit
     pre-commit install
 
    ``internetnl_domain_analyse`` comes with a lot of hooks configured to automatically help the
    developer to check the code being written.
@@ -178,16 +139,14 @@
 #. When you’re done editing, do::
 
     git add <MODIFIED FILES>
     git commit
 
    to record your changes in git_.
 
-   .. todo:: if you are not using pre-commit, please remove the following item:
-
    Please make sure to see the validation messages from |pre-commit|_ and fix
    any eventual issues.
    This should automatically use flake8_/black_ to check/fix the code style
    in a way that is compatible with the project.
 
    .. important:: Don't forget to add unit tests and documentation in case your
       contribution adds an additional feature and is not just a bugfix.
@@ -214,16 +173,14 @@
 #. If everything works fine, push your local branch to |the repository service| with::
 
     git push -u origin my-feature
 
 #. Go to the web page of your fork and click |contribute button|
    to send your changes for review.
 
-   .. todo:: if you are using GitHub, you can uncomment the following paragraph
-
       Find more detailed information in `creating a PR`_. You might also want to open
       the PR as a draft first and mark it as ready for review after the feedbacks
       from the continuous integration (CI) system or any required fixes.
 
 
 Troubleshooting
 ---------------
@@ -274,16 +231,14 @@
 
 Maintainer tasks
 ================
 
 Releases
 --------
 
-.. todo:: This section assumes you are using PyPI to publicly release your package.
-
    If instead you are using a different/private package index, please update
    the instructions accordingly.
 
 If you are part of the group of maintainers and have correct user permissions
 on PyPI_, the following steps can be used to release a new version for
 ``internetnl_domain_analyse``:
 
@@ -304,22 +259,21 @@
 
 .. [#contrib1] Even though, these resources focus on open source projects and
    communities, the general ideas behind collaborating with other developers
    to collectively create software are general and can be applied to all sorts
    of environments, including private companies and proprietary code bases.
 
 
-.. <-- strart -->
-.. todo:: Please review and change the following definitions:
+.. <-- start -->
 
 .. |the repository service| replace:: GitHub
 .. |contribute button| replace:: "Create pull request"
 
-.. _repository: https://github.com/<USERNAME>/internetnl_domain_analyse
-.. _issue tracker: https://github.com/<USERNAME>/internetnl_domain_analyse/issues
+.. _repository: https://github.com/eelcovv/internetnl_domain_analyse
+.. _issue tracker: https://github.com/eelcovv/internetnl_domain_analyse/issues
 .. <-- end -->
 
 
 .. |virtualenv| replace:: ``virtualenv``
 .. |pre-commit| replace:: ``pre-commit``
 .. |tox| replace:: ``tox``
```

### Comparing `internetnl_domain_analyse-1.8.9/LICENSE.txt` & `internetnl_domain_analyse-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/PKG-INFO` & `internetnl_domain_analyse-1.9.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.8.9
+Version: 1.9.3
 Summary: A tool to create image belong to internetnl time series
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: EVLT
+Home-page: https://github.com/eelcovv/internetnl_domain_analyse
+Author: Eelco van Vliet
 Author-email: 
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: importlib-metadata; python_version < "3.8"
```

### Comparing `internetnl_domain_analyse-1.8.9/docs/Makefile` & `internetnl_domain_analyse-1.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/docs/conf.py` & `internetnl_domain_analyse-1.9.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,23 @@
 todo_emit_warnings = True
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+# html_theme_options = {
+#    "sidebar_width": "300px",
+#    "page_width": "1200px"
+# }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -242,15 +242,21 @@
     # Additional stuff for the LaTeX preamble.
     # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "user_guide.tex", "internetnl_domain_analyse Documentation", "EVLT", "manual")
+    (
+        "index",
+        "user_guide.tex",
+        "internetnl_domain_analyse Documentation",
+        "EVLT",
+        "manual",
+    )
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `internetnl_domain_analyse-1.8.9/examples/domain_analyse_settings.yml` & `internetnl_domain_analyse-1.9.3/examples/domain_analyse_settings.yml`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/setup.cfg` & `internetnl_domain_analyse-1.9.3/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = internetnl_domain_analyse
 description = A tool to create image belong to internetnl time series
-author = EVLT
+author = Eelco van Vliet
 author_email = 
 license = MIT
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/pyscaffold/pyscaffold/
+url = https://github.com/eelcovv/internetnl_domain_analyse
 project_urls = 
-	Documentation = https://pyscaffold.org/
+	Documentation = https://internetnl-domain-analyse.readthedocs.io/en/latest/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `internetnl_domain_analyse-1.8.9/setup.py` & `internetnl_domain_analyse-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/__init__.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/__init__.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domain_analyse_classes.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_analyse_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,16 @@
                 var_type=var_type,
                 var_weight_key=var_weight_key,
                 scaling_factor_key=schaal_factor_key,
                 units_scaling_factor_key=units_schaal_factor_key,
                 report_numbers=var_prop_klass.report_number,
             )
 
+            stats.calculate()
+
             if (
                     not np.isnan(var_prop_klass.report_number)
                     and var_prop_klass.report_number
             ):
                 all_stats[column] = stats.records_sum
             else:
                 all_stats[column] = stats.records_weighted_mean_agg
@@ -1698,13 +1700,13 @@
                 dd,
                 weights=ww,
                 density=False,
                 bins=n_bins,
                 range=(0, 100),
             )
         except ValueError as err:
-            _logger.warning("Fails for dicts. Skip for now")
+            _logger.debug("Fails for dicts. Skip for now")
         else:
             _logger.debug(f"Success with {var_key}")
             histogram_per_breakdown[grp_key] = histogram
 
     return histogram_per_breakdown
```

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domain_plots.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domain_plots.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/domein_analyse.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/domein_analyse.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/latex_output.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/latex_output.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/public_suffix_list.dat` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse/utils.py` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse/utils.py`

 * *Files identical despite different names*

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/PKG-INFO` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: internetnl_domain_analyse
-Version: 1.8.9
+Version: 1.9.3
 Summary: A tool to create image belong to internetnl time series
-Home-page: https://github.com/pyscaffold/pyscaffold/
-Author: EVLT
+Home-page: https://github.com/eelcovv/internetnl_domain_analyse
+Author: Eelco van Vliet
 Author-email: 
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://internetnl-domain-analyse.readthedocs.io/en/latest/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: importlib-metadata; python_version < "3.8"
```

### Comparing `internetnl_domain_analyse-1.8.9/src/internetnl_domain_analyse.egg-info/SOURCES.txt` & `internetnl_domain_analyse-1.9.3/src/internetnl_domain_analyse.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 pyproject.toml
```

### Comparing `internetnl_domain_analyse-1.8.9/tox.ini` & `internetnl_domain_analyse-1.9.3/tox.ini`

 * *Files identical despite different names*

