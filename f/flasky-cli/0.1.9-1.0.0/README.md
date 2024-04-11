# Comparing `tmp/flasky_cli-0.1.9.tar.gz` & `tmp/flasky_cli-1.0.0.tar.gz`

## Comparing `flasky_cli-0.1.9.tar` & `flasky_cli-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.python-version
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/requirements-dev.lock
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/requirements.lock
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/__version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/cli/__init__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/cli/main.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/__init__.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/cookiemod.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/common/prompts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/create/__init__.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/create/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/cli.py
--rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/domain.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/data/__init__.py
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/src/flask_cli/templates/data/default.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/.gitignore
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/README.md
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 flasky_cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/.python-version
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/requirements.lock
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/__version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/cli/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/cli/main.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/common/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/create/__init__.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/create/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/templates/__init__.py
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/templates/cli.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/templates/exception.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/src/flask_cli/templates/templates.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 flasky_cli-1.0.0/PKG-INFO
```

### Comparing `flasky_cli-0.1.9/requirements-dev.lock` & `flasky_cli-1.0.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.9/requirements.lock` & `flasky_cli-1.0.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.9/.github/workflows/python-publish.yml` & `flasky_cli-1.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `flasky_cli-0.1.9/src/flask_cli/create/cli.py` & `flasky_cli-1.0.0/src/flask_cli/create/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 
     console.rule()
     console.print(f"[bold green]🏗️  Project created in {destination}")
     console.rule()
     console.print("-- Let's get flasky! --")
 
 
+@click.group()
+def create():
+    """
+    Commands to create templates.
+    """
+
+
 @click.command(name="create")
 @click.option(
     "--template",
     "-t",
     help="Project template name.",
     required=False,
 )
@@ -38,10 +45,13 @@
     """
 
     if template:
         template_obj = get_template_by_name(template)
     else:
         template_obj = prompt_template()
 
-    destination = cookiecutter(template_obj.source)
+    destination = cookiecutter(template_obj['source'])
 
     print_instructions(destination)
+
+
+create.add_command(create_project)
```

### Comparing `flasky_cli-0.1.9/README.md` & `flasky_cli-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 ## Creating a new project
 
 ```bash
 flask-cli create
 ```
 
+## Createing a new project with template name
+```bash
+flask-cli create --template <template>
+```
+
 ## Listing the project templates
 
 ```bash
 flask-cli templates list
 ```
 
 With details:
```

### Comparing `flasky_cli-0.1.9/pyproject.toml` & `flasky_cli-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flasky-cli"
-version = "0.1.9"
+version = "1.0.0"
 description = " CLI to start Flask projects"
 authors = [
     { name = "jennier0107", email = "mt3085570450@outlook.com" }
 ]
 dependencies = [
     "click>=8.1.7",
     "rich-click>=1.7.4",
@@ -32,12 +32,13 @@
 Homepage = "https://github.com/jennier0107/flasky-cli"
 Repository = "https://github.com/jennier0107/flasky-cli"
 "Bug Tracker" = "https://github.com/jennier0107/flasky-cli/issues"
 
 [project.scripts]
 flask-cli = "flask_cli.cli.main:main"
 
+
 [tool.hatch.build.targets.wheel]
 packages = ["src/flask_cli"]
 
 [tool.hatch.build.targets.sdist]
 exclude = ["tests", "static"]
```

### Comparing `flasky_cli-0.1.9/PKG-INFO` & `flasky_cli-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: flasky-cli
-Version: 0.1.9
+Version: 1.0.0
 Summary:  CLI to start Flask projects
 Project-URL: Homepage, https://github.com/jennier0107/flasky-cli
 Project-URL: Repository, https://github.com/jennier0107/flasky-cli
 Project-URL: Bug Tracker, https://github.com/jennier0107/flasky-cli/issues
 Author-email: jennier0107 <mt3085570450@outlook.com>
 Requires-Python: >=3.8
 Requires-Dist: click>=8.1.7
@@ -37,14 +37,19 @@
 
 ## Creating a new project
 
 ```bash
 flask-cli create
 ```
 
+## Createing a new project with template name
+```bash
+flask-cli create --template <template>
+```
+
 ## Listing the project templates
 
 ```bash
 flask-cli templates list
 ```
 
 With details:
```

