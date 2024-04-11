# Comparing `tmp/arcor2_mocks-1.0.0.tar.gz` & `tmp/arcor2_mocks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcor2_mocks-1.0.0.tar", last modified: Tue Feb 14 12:55:50 2023, max compression
+gzip compressed data, was "arcor2_mocks-1.1.0.tar", last modified: Thu Apr 11 09:47:31 2024, max compression
```

## Comparing `arcor2_mocks-1.0.0.tar` & `arcor2_mocks-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)       12 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/MANIFEST.in
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3424 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/PKG-INFO
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/arcor2_mocks/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        5 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/VERSION
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      351 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      731 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/exceptions_asset.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      447 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/exceptions_project.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/py.typed
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/arcor2_mocks/scripts/
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/scripts/__init__.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     6597 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/scripts/mock_asset.py
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)    23766 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks/scripts/mock_project.py
-drwxrwxr-x   0 zdenal    (1000) zdenal    (1000)        0 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)     3424 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/PKG-INFO
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      540 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)      136 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/entry_points.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)        1 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       58 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/requires.txt
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       13 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/arcor2_mocks.egg-info/top_level.txt
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)      698 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/backend_shim.py
--rw-rw-r--   0 zdenal    (1000) zdenal    (1000)       38 2023-02-14 12:55:50.371362 arcor2_mocks-1.0.0/setup.cfg
--rw-r--r--   0 zdenal    (1000) zdenal    (1000)     4262 2023-02-14 12:55:50.000000 arcor2_mocks-1.0.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.849252 arcor2_mocks-1.1.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     3512 2024-04-11 09:47:31.845252 arcor2_mocks-1.1.0/PKG-INFO
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.841252 arcor2_mocks-1.1.0/arcor2_mocks/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        5 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/VERSION
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      351 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      731 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/exceptions_asset.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      447 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/exceptions_project.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.845252 arcor2_mocks-1.1.0/arcor2_mocks/scripts/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/scripts/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6597 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/scripts/mock_asset.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    26057 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/arcor2_mocks/scripts/mock_project.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-11 09:47:31.845252 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     3512 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      540 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      136 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/entry_points.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       58 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       13 2024-04-11 09:47:31.000000 arcor2_mocks-1.1.0/arcor2_mocks.egg-info/top_level.txt
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      835 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/backend_shim.py
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-11 09:47:31.849252 arcor2_mocks-1.1.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4350 2024-04-11 09:47:30.000000 arcor2_mocks-1.1.0/setup.py
```

### Comparing `arcor2_mocks-1.0.0/PKG-INFO` & `arcor2_mocks-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: arcor2_mocks
-Version: 1.0.0
+Version: 1.1.0
 Summary: Mocks for services developed by Kinali.
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_mocks
 
 Mocks for services developed by Kinali.
 
 ## Environment variables
 
 - `ARCOR2_PROJECT_SERVICE_MOCK_PORT=5012` - by default, the Project mock listens on port 5012.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - REST API updated to match Project 1.0.0-rc.1.
```

### Comparing `arcor2_mocks-1.0.0/arcor2_mocks/exceptions_asset.py` & `arcor2_mocks-1.1.0/arcor2_mocks/exceptions_asset.py`

 * *Files identical despite different names*

### Comparing `arcor2_mocks-1.0.0/arcor2_mocks/scripts/mock_asset.py` & `arcor2_mocks-1.1.0/arcor2_mocks/scripts/mock_asset.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 app = create_app(__name__)
 
 ASSETS: dict[str, Asset] = {}
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 
+
 # TODO dependencies and tags parameters omitted as not really needed at the moment
 @app.route("/assets", methods=["POST"])
 def post_asset() -> RespT:
     """Creates the asset.
     ---
     post:
         tags:
@@ -217,15 +218,14 @@
     return Response(status=200)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 def main() -> None:
-
     parser = argparse.ArgumentParser(description=ASSET_SERVICE_NAME)
     parser.add_argument("-s", "--swagger", action="store_true", default=False)
     args = parser.parse_args()
 
     run_app(
         app,
         ASSET_SERVICE_NAME,
```

### Comparing `arcor2_mocks-1.0.0/arcor2_mocks/scripts/mock_project.py` & `arcor2_mocks-1.1.0/arcor2_mocks/scripts/mock_project.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from arcor2_mocks import PROJECT_PORT, PROJECT_SERVICE_NAME, version
 from arcor2_mocks.exceptions_project import NotFound, ProjectGeneral, WebApiError
 
 app = create_app(__name__)
 
 SCENES: dict[str, common.Scene] = {}
 PROJECTS: dict[str, common.Project] = {}
+PROJECT_SOURCES: dict[str, common.ProjectSources] = {}
 OBJECT_TYPES: dict[str, object_type.ObjectType] = {}
 
 BOXES: dict[str, object_type.Box] = {}
 CYLINDERS: dict[str, object_type.Cylinder] = {}
 SPHERES: dict[str, object_type.Sphere] = {}
 MESHES: dict[str, object_type.Mesh] = {}
 
@@ -70,14 +71,88 @@
     else:
         project.created = PROJECTS[project.id].created
 
     PROJECTS[project.id] = project
     return jsonify(project.modified.isoformat())
 
 
+@app.route("/projects/sources", methods=["PUT"])
+def put_project_sources() -> RespT:
+    """Add or update project sources.
+    ---
+    put:
+        tags:
+            - Project
+        description: Add or update project sources.
+        requestBody:
+              content:
+                application/json:
+                  schema:
+                    $ref: ProjectSources
+        responses:
+            200:
+              description: Timestamp of last project modification.
+            500:
+              description: "Error types: **General**, **ProjectGeneral**, **NotFound**."
+              content:
+                application/json:
+                  schema:
+                    $ref: WebApiError
+    """
+
+    if not isinstance(request.json, dict):
+        raise ProjectGeneral("Body should be a JSON dict containing ProjectSources.")
+
+    project_sources = common.ProjectSources.from_dict(humps.decamelize(request.json))
+
+    if project_sources.id not in PROJECTS:
+        raise NotFound(f"Project {project_sources.id} does not exist.")
+
+    PROJECT_SOURCES[project_sources.id] = project_sources
+    return Response(status=200)
+
+
+@app.route("/projects/<string:id>/sources", methods=["GET"])
+def get_project_sources(id: str) -> RespT:
+    """Get project sources.
+    ---
+    get:
+        tags:
+            - Project
+        summary: Gets project by project id.
+        parameters:
+            - name: id
+              in: path
+              description: unique ID
+              required: true
+              schema:
+                type: string
+        responses:
+            200:
+              description: Ok
+              content:
+                application/json:
+                  schema:
+                    $ref: ProjectSources
+            500:
+              description: "Error types: **General**, **NotFound**."
+              content:
+                application/json:
+                  schema:
+                    $ref: WebApiError
+    """
+
+    try:
+        project_sources = PROJECT_SOURCES[id]
+    except KeyError:
+        raise NotFound(f"Sources for project {id} not found.")
+
+    return jsonify(humps.camelize(project_sources.to_dict()))
+
+
 @app.route("/projects/<string:id>", methods=["GET"])
 def get_project(id: str) -> RespT:
     """Add or update project.
     ---
     get:
         tags:
             - Project
@@ -101,18 +176,20 @@
               content:
                 application/json:
                   schema:
                     $ref: WebApiError
     """
 
     try:
-        return jsonify(humps.camelize(PROJECTS[id].to_dict()))
+        project = PROJECTS[id]
     except KeyError:
         raise NotFound(f"Project {id} was not found.")
 
+    return jsonify(humps.camelize(project.to_dict()))
+
 
 @app.route("/projects/<string:id>", methods=["DELETE"])
 def delete_project(id: str) -> RespT:
     """Deletes project.
     ---
     delete:
         tags:
@@ -261,18 +338,20 @@
               content:
                 application/json:
                   schema:
                     $ref: WebApiError
     """
 
     try:
-        return jsonify(humps.camelize(SCENES[id].to_dict()))
+        scene = SCENES[id]
     except KeyError:
         raise NotFound(f"Scene {id} was not found.")
 
+    return jsonify(humps.camelize(scene.to_dict()))
+
 
 @app.route("/scenes/<string:id>", methods=["DELETE"])
 def delete_scene(id: str) -> RespT:
     """Deletes scene.
     ---
     delete:
         tags:
@@ -853,26 +932,26 @@
     return Response(status=200)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 def main() -> None:
-
     parser = argparse.ArgumentParser(description=PROJECT_SERVICE_NAME)
     parser.add_argument("-s", "--swagger", action="store_true", default=False)
     args = parser.parse_args()
 
     run_app(
         app,
         PROJECT_SERVICE_NAME,
         version(),
         PROJECT_PORT,
         [
             common.Project,
+            common.ProjectSources,
             common.Scene,
             common.IdDesc,
             object_type.ObjectType,
             object_type.Box,
             object_type.Cylinder,
             object_type.Sphere,
             object_type.Mesh,
```

### Comparing `arcor2_mocks-1.0.0/arcor2_mocks.egg-info/PKG-INFO` & `arcor2_mocks-1.1.0/arcor2_mocks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 Metadata-Version: 2.1
 Name: arcor2-mocks
-Version: 1.0.0
+Version: 1.1.0
 Summary: Mocks for services developed by Kinali.
 Author: Robo@FIT
 Author-email: imaterna@fit.vut.cz
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.10.*
+Requires-Python: ==3.11.*
 Description-Content-Type: text/markdown
 
 # arcor2_mocks
 
 Mocks for services developed by Kinali.
 
 ## Environment variables
 
 - `ARCOR2_PROJECT_SERVICE_MOCK_PORT=5012` - by default, the Project mock listens on port 5012.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - REST API updated to match Project 1.0.0-rc.1.
```

### Comparing `arcor2_mocks-1.0.0/arcor2_mocks.egg-info/SOURCES.txt` & `arcor2_mocks-1.1.0/arcor2_mocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcor2_mocks-1.0.0/setup.py` & `arcor2_mocks-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     'author': 'Robo@FIT',
     'author_email': 'imaterna@fit.vut.cz',
     'classifiers': [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
-        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Natural Language :: English',
         'Topic :: Scientific/Engineering',
     ],
     'description': 'Mocks for services developed by Kinali.',
     'entry_points': {
         'console_scripts': [
             'arcor2_mock_project = arcor2_mocks.scripts.mock_project:main',
             'arcor2_mock_asset = arcor2_mocks.scripts.mock_asset:main',
         ],
     },
     'install_requires': (
-        'Flask~=2.2.2',
-        'arcor2~=1.0.0',
+        'Flask~=3.0.2',
+        'arcor2~=1.3.0',
         'fastuuid~=0.8.0',
         'pyhumps==3.8.0',
     ),
     'license': 'LGPL',
     'long_description': """# arcor2_mocks
 
 Mocks for services developed by Kinali.
@@ -38,14 +38,20 @@
 
 - `ARCOR2_PROJECT_SERVICE_MOCK_PORT=5012` - by default, the Project mock listens on port 5012.
 - `ARCOR2_REST_API_DEBUG=1` - turns on Flask debugging (logs each endpoint call).
 # Changelog
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 
+## [1.1.0] - 2024-04-11
+
+### Changed
+
+- Updated dependencies, switched to Python 3.11.
+
 ## [1.0.0] - 2023-02-14
 
 ### Changed
 
 - Marked as a stable version.
 - REST API updated to match Project 1.0.0-rc.1.
 
@@ -162,10 +168,10 @@
             'py.typed',
         ),
     },
     'packages': (
         'arcor2_mocks',
         'arcor2_mocks.scripts',
     ),
-    'python_requires': '==3.10.*',
-    'version': '1.0.0',
+    'python_requires': '==3.11.*',
+    'version': '1.1.0',
 })
```

