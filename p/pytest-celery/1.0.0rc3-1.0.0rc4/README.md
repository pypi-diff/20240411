# Comparing `tmp/pytest_celery-1.0.0rc3.tar.gz` & `tmp/pytest_celery-1.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_celery-1.0.0rc3.tar", max compression
+gzip compressed data, was "pytest_celery-1.0.0rc4.tar", max compression
```

## Comparing `pytest_celery-1.0.0rc3.tar` & `pytest_celery-1.0.0rc4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1791 2024-04-05 16:14:25.718155 pytest_celery-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0     4531 2024-04-05 16:14:43.834252 pytest_celery-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     7303 2024-04-05 16:14:43.918253 pytest_celery-1.0.0rc3/src/pytest_celery/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/__init__.py
--rw-r--r--   0        0        0     1923 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/backend.py
--rw-r--r--   0        0        0    10591 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/base.py
--rw-r--r--   0        0        0     1880 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/broker.py
--rw-r--r--   0        0        0     5284 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/container.py
--rw-r--r--   0        0        0     9307 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/setup.py
--rw-r--r--   0        0        0     3737 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/api/worker.py
--rw-r--r--   0        0        0     3728 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/defaults.py
--rw-r--r--   0        0        0        0 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/__init__.py
--rw-r--r--   0        0        0     2287 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/backend.py
--rw-r--r--   0        0        0     2312 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/broker.py
--rw-r--r--   0        0        0     2816 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/setup.py
--rw-r--r--   0        0        0     2033 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/worker.py
--rw-r--r--   0        0        0      207 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/plugin.py
--rw-r--r--   0        0        0      452 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/__init__.py
--rw-r--r--   0        0        0      147 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/__init__.py
--rw-r--r--   0        0        0      298 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/api.py
--rw-r--r--   0        0        0     1861 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/container.py
--rw-r--r--   0        0        0      431 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/defaults.py
--rw-r--r--   0        0        0     2775 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/fixtures.py
--rw-r--r--   0        0        0      145 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/__init__.py
--rw-r--r--   0        0        0      291 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/api.py
--rw-r--r--   0        0        0     2056 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/container.py
--rw-r--r--   0        0        0      404 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/defaults.py
--rw-r--r--   0        0        0     2706 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/fixtures.py
--rw-r--r--   0        0        0      135 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/__init__.py
--rw-r--r--   0        0        0      143 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/__init__.py
--rw-r--r--   0        0        0      780 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/api.py
--rw-r--r--   0        0        0      238 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/defaults.py
--rw-r--r--   0        0        0     3049 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/fixtures.py
--rw-r--r--   0        0        0      142 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/__init__.py
--rw-r--r--   0        0        0      285 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/api.py
--rw-r--r--   0        0        0      233 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/defaults.py
--rw-r--r--   0        0        0     3015 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/fixtures.py
--rw-r--r--   0        0        0     2235 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/container.py
--rw-r--r--   0        0        0      274 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/defaults.py
--rw-r--r--   0        0        0     1170 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/Dockerfile
--rw-r--r--   0        0        0      152 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/__init__.py
--rw-r--r--   0        0        0     7317 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/container.py
--rw-r--r--   0        0        0      152 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/__init__.py
--rw-r--r--   0        0        0      498 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/app.py
--rw-r--r--   0        0        0      677 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/utils.py
--rw-r--r--   0        0        0     1192 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/defaults.py
--rw-r--r--   0        0        0     9720 2024-04-05 16:14:25.726155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/fixtures.py
--rw-r--r--   0        0        0     3549 2024-04-05 16:14:25.730155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/tasks.py
--rw-r--r--   0        0        0     9142 2024-04-05 16:14:25.730155 pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/volume.py
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 pytest_celery-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1791 2024-04-11 21:57:32.272879 pytest_celery-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0     6703 2024-04-11 21:57:41.716776 pytest_celery-1.0.0rc4/README.rst
+-rw-r--r--   0        0        0     4585 2024-04-11 21:57:41.632777 pytest_celery-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     7303 2024-04-11 21:57:41.716776 pytest_celery-1.0.0rc4/src/pytest_celery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/__init__.py
+-rw-r--r--   0        0        0     1923 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/backend.py
+-rw-r--r--   0        0        0    10591 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/base.py
+-rw-r--r--   0        0        0     1880 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/broker.py
+-rw-r--r--   0        0        0     5284 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/container.py
+-rw-r--r--   0        0        0     9307 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/setup.py
+-rw-r--r--   0        0        0     3737 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/api/worker.py
+-rw-r--r--   0        0        0     3728 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/__init__.py
+-rw-r--r--   0        0        0     2287 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/backend.py
+-rw-r--r--   0        0        0     2312 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/broker.py
+-rw-r--r--   0        0        0     2816 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/setup.py
+-rw-r--r--   0        0        0     2033 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/worker.py
+-rw-r--r--   0        0        0      207 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/plugin.py
+-rw-r--r--   0        0        0      452 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/__init__.py
+-rw-r--r--   0        0        0      298 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/api.py
+-rw-r--r--   0        0        0     1861 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/container.py
+-rw-r--r--   0        0        0      431 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/defaults.py
+-rw-r--r--   0        0        0     2775 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/fixtures.py
+-rw-r--r--   0        0        0      145 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/__init__.py
+-rw-r--r--   0        0        0      291 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/api.py
+-rw-r--r--   0        0        0     2056 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/container.py
+-rw-r--r--   0        0        0      404 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/defaults.py
+-rw-r--r--   0        0        0     2706 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/fixtures.py
+-rw-r--r--   0        0        0      135 2024-04-11 21:57:32.280879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/__init__.py
+-rw-r--r--   0        0        0      143 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/__init__.py
+-rw-r--r--   0        0        0      780 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/api.py
+-rw-r--r--   0        0        0      238 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/defaults.py
+-rw-r--r--   0        0        0     3049 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/fixtures.py
+-rw-r--r--   0        0        0      142 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/broker/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/broker/api.py
+-rw-r--r--   0        0        0      233 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/broker/defaults.py
+-rw-r--r--   0        0        0     3015 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/broker/fixtures.py
+-rw-r--r--   0        0        0     2235 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/container.py
+-rw-r--r--   0        0        0      274 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/defaults.py
+-rw-r--r--   0        0        0     1177 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/Dockerfile
+-rw-r--r--   0        0        0      152 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/__init__.py
+-rw-r--r--   0        0        0     7317 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/container.py
+-rw-r--r--   0        0        0      152 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/content/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/content/app.py
+-rw-r--r--   0        0        0      677 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/content/utils.py
+-rw-r--r--   0        0        0     1192 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/defaults.py
+-rw-r--r--   0        0        0     9720 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/fixtures.py
+-rw-r--r--   0        0        0     3549 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/tasks.py
+-rw-r--r--   0        0        0     9142 2024-04-11 21:57:32.284879 pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/volume.py
+-rw-r--r--   0        0        0     8204 1970-01-01 00:00:00.000000 pytest_celery-1.0.0rc4/PKG-INFO
```

### Comparing `pytest_celery-1.0.0rc3/LICENSE` & `pytest_celery-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/pyproject.toml` & `pytest_celery-1.0.0rc4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     "Operating System :: OS Independent",
 ]
 
 description = "Pytest plugin for Celery"
 homepage = "https://github.com/celery/pytest-celery"
 license = "BSD"
 name = "pytest-celery"
-version = "v1.0.0rc3"
+version = "v1.0.0rc4"
+readme = "README.rst"
+keywords = ["pytest", "celery"]
 
 [tool.poetry_bumpversion.file."src/pytest_celery/__init__.py"]
 search = '__version__ = "{current_version}"'
 replace = '__version__ = "{new_version}"'
 
 [tool.poetry_bumpversion.file."README.rst"]
 search = ':Version: {current_version}'
```

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/__init__.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Official pytest plugin for Celery."""
 
 # flake8: noqa
 
 
-__version__ = "v1.0.0rc3"
+__version__ = "v1.0.0rc4"
 __author__ = "Tomer Nosrati"
 __contact__ = "tomer.nosrati@gmail.com"
 __homepage__ = "https://pytest-celery.readthedocs.io/"
 __docformat__ = "restructuredtext"
 
 
 import re
```

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/backend.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/backend.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/base.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/base.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/broker.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/broker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/container.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/setup.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/api/worker.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/api/worker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/defaults.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/defaults.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/backend.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/backend.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/broker.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/broker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/setup.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/setup.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/fixtures/worker.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/fixtures/worker.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/container.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/memcached/fixtures.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/memcached/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/container.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/rabbitmq/fixtures.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/rabbitmq/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/api.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/api.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/backend/fixtures.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/backend/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/broker/fixtures.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/broker/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/redis/container.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/redis/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/Dockerfile` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 ENV PYTHONDONTWRITEBYTECODE=1
 
 EXPOSE 5678
 
 # Install Python dependencies
 RUN pip install --no-cache-dir --upgrade \
     pip \
-    celery[redis,pymemcache]${WORKER_VERSION:+==$WORKER_VERSION} \
+    celery[redis,pymemcache,gevent]${WORKER_VERSION:+==$WORKER_VERSION} \
     pytest-celery@git+https://github.com/celery/pytest-celery.git
 
 # The workdir must be /app
 WORKDIR /app
 
 COPY content/ .
```

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/container.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/container.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/content/utils.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/content/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/defaults.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/defaults.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/fixtures.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/tasks.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/tasks.py`

 * *Files identical despite different names*

### Comparing `pytest_celery-1.0.0rc3/src/pytest_celery/vendors/worker/volume.py` & `pytest_celery-1.0.0rc4/src/pytest_celery/vendors/worker/volume.py`

 * *Files identical despite different names*

