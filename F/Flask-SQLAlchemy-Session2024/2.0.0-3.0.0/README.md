# Comparing `tmp/Flask-SQLAlchemy-Session2024-2.0.0.tar.gz` & `tmp/Flask-SQLAlchemy-Session2024-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SQLAlchemy-Session2024-2.0.0.tar", last modified: Thu Apr 11 07:41:11 2024, max compression
+gzip compressed data, was "Flask-SQLAlchemy-Session2024-3.0.0.tar", last modified: Thu Apr 11 07:59:41 2024, max compression
```

## Comparing `Flask-SQLAlchemy-Session2024-2.0.0.tar` & `Flask-SQLAlchemy-Session2024-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/
--rw-r--r--   0 user      (1000) user      (1000)       49 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/AUTHORS
--rw-r--r--   0 user      (1000) user      (1000)      955 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/CHANGELOG.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2566 2024-04-11 07:41:11.000000 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      423 2024-04-11 07:41:11.000000 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-11 07:41:11.000000 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       51 2024-04-11 07:41:11.000000 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       29 2024-04-11 07:41:11.000000 Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1068 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       53 2024-04-11 07:38:55.000000 Flask-SQLAlchemy-Session2024-2.0.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     2566 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1751 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/flask_sqlalchemy_session2024/
--rw-r--r--   0 user      (1000) user      (1000)     2485 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/flask_sqlalchemy_session2024/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       31 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/pyproject.toml
--rw-r--r--   0 user      (1000) user      (1000)      131 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1979 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:41:11.739837 Flask-SQLAlchemy-Session2024-2.0.0/tests/
--rw-r--r--   0 user      (1000) user      (1000)     3071 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-2.0.0/tests/test_flask_sqlalchemy_session.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:59:41.027538 Flask-SQLAlchemy-Session2024-3.0.0/
+-rw-r--r--   0 user      (1000) user      (1000)       49 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-3.0.0/AUTHORS
+-rw-r--r--   0 user      (1000) user      (1000)     1215 2024-04-11 07:56:01.000000 Flask-SQLAlchemy-Session2024-3.0.0/CHANGELOG.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:59:41.017538 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2558 2024-04-11 07:59:40.000000 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      419 2024-04-11 07:59:40.000000 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-11 07:59:40.000000 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       51 2024-04-11 07:59:40.000000 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       25 2024-04-11 07:59:40.000000 Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1068 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-3.0.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       53 2024-04-11 07:38:55.000000 Flask-SQLAlchemy-Session2024-3.0.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     2558 2024-04-11 07:59:41.027538 Flask-SQLAlchemy-Session2024-3.0.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1743 2024-04-11 07:53:29.000000 Flask-SQLAlchemy-Session2024-3.0.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:59:41.017538 Flask-SQLAlchemy-Session2024-3.0.0/flask_sqlalchemy_session/
+-rw-r--r--   0 user      (1000) user      (1000)     2485 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-3.0.0/flask_sqlalchemy_session/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       31 2024-04-11 07:36:45.000000 Flask-SQLAlchemy-Session2024-3.0.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)      131 2024-04-11 07:59:41.027538 Flask-SQLAlchemy-Session2024-3.0.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1975 2024-04-11 07:56:13.000000 Flask-SQLAlchemy-Session2024-3.0.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-11 07:59:41.017538 Flask-SQLAlchemy-Session2024-3.0.0/tests/
+-rw-r--r--   0 user      (1000) user      (1000)     3067 2024-04-11 07:53:15.000000 Flask-SQLAlchemy-Session2024-3.0.0/tests/test_flask_sqlalchemy_session.py
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/CHANGELOG.md` & `Flask-SQLAlchemy-Session2024-3.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
 
 ## [Unreleased]
 
-## [2.0] - 2024-04-11
+## [3.0.0] - 2024-04-11
+
+### Changed
+
+- Rename the Python module itself back to its original name. It is unlikely that
+  anyone will install both the original and the fork at the same time, and it is
+  better to avoid breaking people's imports if possible.
+
+## [2.0.0] - 2024-04-11
 
 ### Changed
 
 - Fork package and rename due to inactive upstream.
 - Rewrite class to stop using deprecated Flask API (`_app_ctx_stack`). Thanks to
   https://github.com/vincent-olivert-riera and https://github.com/schettino72
   for contributing PRs (in the original project) which inspired this rewrite.
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/Flask_SQLAlchemy_Session2024.egg-info/PKG-INFO` & `Flask-SQLAlchemy-Session2024-3.0.0/Flask_SQLAlchemy_Session2024.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQLAlchemy-Session2024
-Version: 2.0.0
+Version: 3.0.0
 Summary: SQL Alchemy session scoped on Flask requests.
 Home-page: https://github.com/e-c-d/flask-sqlalchemy-session2024
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 Initialize a `flask_scoped_session` as you would a
 `scoped_session`, with the addition of a Flask
 app. Then use the resulting session to query models:
 
 ```python
 from flask import Flask, abort, jsonify
-from flask_sqlalchemy_session2024 import flask_scoped_session
+from flask_sqlalchemy_session import flask_scoped_session
 
 app = Flask(__name__)
 session = flask_scoped_session(session_factory, app)
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = session.query(User).get(user_id)
@@ -59,15 +59,15 @@
 ```
 
 The `current_session` is also provided as a convenient accessor to the session
 of the current request, in the same spirit of `flask.request` and
 `flask.current_app`.
 
 ```python
-from flask_sqlalchemy_session2024 import current_session
+from flask_sqlalchemy_session import current_session
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = current_session.query(User).get(user_id)
     if user is None:
         abort(404)
     return flask.jsonify(**user.to_dict())
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/LICENSE` & `Flask-SQLAlchemy-Session2024-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/PKG-INFO` & `Flask-SQLAlchemy-Session2024-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SQLAlchemy-Session2024
-Version: 2.0.0
+Version: 3.0.0
 Summary: SQL Alchemy session scoped on Flask requests.
 Home-page: https://github.com/e-c-d/flask-sqlalchemy-session2024
 Author: Eduard Christian Dumitrescu
 Author-email: eduard.c.dumitrescu@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -41,15 +41,15 @@
 
 Initialize a `flask_scoped_session` as you would a
 `scoped_session`, with the addition of a Flask
 app. Then use the resulting session to query models:
 
 ```python
 from flask import Flask, abort, jsonify
-from flask_sqlalchemy_session2024 import flask_scoped_session
+from flask_sqlalchemy_session import flask_scoped_session
 
 app = Flask(__name__)
 session = flask_scoped_session(session_factory, app)
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = session.query(User).get(user_id)
@@ -59,15 +59,15 @@
 ```
 
 The `current_session` is also provided as a convenient accessor to the session
 of the current request, in the same spirit of `flask.request` and
 `flask.current_app`.
 
 ```python
-from flask_sqlalchemy_session2024 import current_session
+from flask_sqlalchemy_session import current_session
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = current_session.query(User).get(user_id)
     if user is None:
         abort(404)
     return flask.jsonify(**user.to_dict())
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/README.md` & `Flask-SQLAlchemy-Session2024-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Initialize a `flask_scoped_session` as you would a
 `scoped_session`, with the addition of a Flask
 app. Then use the resulting session to query models:
 
 ```python
 from flask import Flask, abort, jsonify
-from flask_sqlalchemy_session2024 import flask_scoped_session
+from flask_sqlalchemy_session import flask_scoped_session
 
 app = Flask(__name__)
 session = flask_scoped_session(session_factory, app)
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = session.query(User).get(user_id)
@@ -38,15 +38,15 @@
 ```
 
 The `current_session` is also provided as a convenient accessor to the session
 of the current request, in the same spirit of `flask.request` and
 `flask.current_app`.
 
 ```python
-from flask_sqlalchemy_session2024 import current_session
+from flask_sqlalchemy_session import current_session
 
 @app.route("/users/<int:user_id>")
 def user(user_id):
     user = current_session.query(User).get(user_id)
     if user is None:
         abort(404)
     return flask.jsonify(**user.to_dict())
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/flask_sqlalchemy_session2024/__init__.py` & `Flask-SQLAlchemy-Session2024-3.0.0/flask_sqlalchemy_session/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/setup.py` & `Flask-SQLAlchemy-Session2024-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     del os.link
 
 with open("README.md", "rt", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="Flask-SQLAlchemy-Session2024",
-    version="2.0.0",
-    packages=["flask_sqlalchemy_session2024"],
+    version="3.0.0",
+    packages=["flask_sqlalchemy_session"],
     author="Eduard Christian Dumitrescu",
     author_email="eduard.c.dumitrescu@gmail.com",
     url="https://github.com/e-c-d/flask-sqlalchemy-session2024",
     license="MIT",
     description="SQL Alchemy session scoped on Flask requests.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `Flask-SQLAlchemy-Session2024-2.0.0/tests/test_flask_sqlalchemy_session.py` & `Flask-SQLAlchemy-Session2024-3.0.0/tests/test_flask_sqlalchemy_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import mock
 
 import pytest
 from flask import Flask
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session, sessionmaker
 
-from flask_sqlalchemy_session2024 import flask_scoped_session, current_session
+from flask_sqlalchemy_session import flask_scoped_session, current_session
 
 
 @pytest.fixture
 def sqlite_engine():
     """Return an sqlite engine"""
     return create_engine("sqlite://")
```

