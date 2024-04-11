# Comparing `tmp/kodexa_cli-7.0.8552549159.tar.gz` & `tmp/kodexa_cli-7.0.8649253175.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-7.0.8552549159.tar", max compression
+gzip compressed data, was "kodexa_cli-7.0.8649253175.tar", max compression
```

## Comparing `kodexa_cli-7.0.8552549159.tar` & `kodexa_cli-7.0.8649253175.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2024-04-04 09:41:19.805145 kodexa_cli-7.0.8552549159/LICENSE
--rw-r--r--   0        0        0     2157 2024-04-04 09:41:19.805145 kodexa_cli-7.0.8552549159/README.md
--rw-r--r--   0        0        0       64 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      402 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-container/Dockerfile
--rw-r--r--   0        0        0      174 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-container/health-check.conf
--rw-r--r--   0        0        0        0 2024-04-04 09:41:19.809145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-container/index.html
--rw-r--r--   0        0        0      349 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/.helmignore
--rw-r--r--   0        0        0      140 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/Chart.yaml
--rw-r--r--   0        0        0     1528 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0     1791 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/templates/deployment.yaml
--rw-r--r--   0        0        0      410 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/templates/service.yaml
--rw-r--r--   0        0        0      330 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/values.yaml
--rw-r--r--   0        0        0    48746 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      722 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2024-04-04 09:41:19.813145 kodexa_cli-7.0.8552549159/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      808 2024-04-04 09:41:33.389203 kodexa_cli-7.0.8552549159/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8552549159/setup.py
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8552549159/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 15:25:00.726642 kodexa_cli-7.0.8649253175/LICENSE
+-rw-r--r--   0        0        0     2157 2024-04-11 15:25:00.726642 kodexa_cli-7.0.8649253175/README.md
+-rw-r--r--   0        0        0       64 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      402 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      174 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0        0 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-container/index.html
+-rw-r--r--   0        0        0      349 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1528 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1791 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      410 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/service.yaml
+-rw-r--r--   0        0        0      330 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    48988 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2024-04-11 15:25:00.730641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      722 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2024-04-11 15:25:00.734641 kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      808 2024-04-11 15:25:12.006599 kodexa_cli-7.0.8649253175/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8649253175/setup.py
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8649253175/PKG-INFO
```

### Comparing `kodexa_cli-7.0.8552549159/LICENSE` & `kodexa_cli-7.0.8649253175/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/README.md` & `kodexa_cli-7.0.8649253175/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8649253175/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/charts/resource-pack/templates/deployment.yaml` & `kodexa_cli-7.0.8649253175/kodexa_cli/charts/resource-pack/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/cli.py` & `kodexa_cli-7.0.8649253175/kodexa_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,26 +486,28 @@
 )
 @click.option("--token", default=get_current_access_token(), help="Access token")
 @click.option("--query", default="*", help="Limit the results using a query")
 @click.option("--format", default=None, help="The format to output (json, yaml)")
 @click.option("--page", default=1, help="Page number")
 @click.option("--pageSize", default=10, help="Page size")
 @click.option("--sort", default=None, help="Sort by (ie. startDate:desc)")
+@click.option("--truncate/--no-truncate", default=True, help="Truncate the output or not")
 @pass_info
 def get(
         _: Info,
         object_type: str,
         ref: Optional[str],
         url: str,
         token: str,
         query: str,
         format=None,
         page: int = 1,
         pagesize: int = 10,
         sort: str = None,
+        truncate: bool = True,
 ):
     """
     List the instances of the component or entity type
 
     object_type is the type of object to list (component, document, execution, etc.)
     ref is the reference to the object
     """
@@ -530,15 +532,15 @@
                 GLOBAL_IGNORE_COMPLETE = True
             elif format == "yaml":
                 object_dict = object_instance.model_dump(by_alias=True)
                 print(yaml.dump(object_dict, indent=4), "yaml")
                 GLOBAL_IGNORE_COMPLETE = True
         else:
             print_object_table(
-                object_metadata, objects_endpoint, query, page, pagesize, sort
+                object_metadata, objects_endpoint, query, page, pagesize, sort, truncate
             )
     else:
         if ref and not ref.isspace():
             if "/" in ref:
                 object_instance = client.get_object_by_ref(
                     object_metadata["plural"], ref
                 )
@@ -559,22 +561,22 @@
 
                 if organization is None:
                     print(f"Could not find organization with slug {ref}")
                     exit(1)
 
                 objects_endpoint = client.get_object_type(object_type, organization)
                 print_object_table(
-                    object_metadata, objects_endpoint, query, page, pagesize, sort
+                    object_metadata, objects_endpoint, query, page, pagesize, sort, truncate
                 )
         else:
             print(f"You must provide a ref to get a specific object")
             exit(1)
 
 
-def print_object_table(object_metadata, objects_endpoint, query, page, pagesize, sort):
+def print_object_table(object_metadata, objects_endpoint, query, page, pagesize, sort, truncate):
     """
     Print the output of the list in a table form
 
     """
     from rich.table import Table
 
     table = Table(title=f"Listing {object_metadata['plural']}", title_style="bold blue")
@@ -583,15 +585,18 @@
     if object_metadata["plural"] in DEFAULT_COLUMNS:
         column_list = DEFAULT_COLUMNS[object_metadata["plural"]]
     else:
         column_list = DEFAULT_COLUMNS["default"]
 
     # Create column header for the table
     for col in column_list:
-        table.add_column(col)
+        if truncate:
+            table.add_column(col)
+        else:
+            table.add_column(col, overflow="fold")
 
     try:
         page_of_object_endpoints = objects_endpoint.list(
             query=query, page=page, page_size=pagesize, sort=sort
         )
     except Exception as e:
         print("e:", e)
```

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/documentation.py` & `kodexa_cli-7.0.8649253175/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/header.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/model.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/options.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-7.0.8649253175/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8552549159/pyproject.toml` & `kodexa_cli-7.0.8649253175/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "7.0.08552549159"
+version = "7.0.08649253175"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli.cli:safe_entry_point'
```

### Comparing `kodexa_cli-7.0.8552549159/setup.py` & `kodexa_cli-7.0.8649253175/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'wrapt>=1.15.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli.cli:safe_entry_point']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '7.0.8552549159',
+    'version': '7.0.8649253175',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-7.0.8552549159/PKG-INFO` & `kodexa_cli-7.0.8649253175/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 7.0.8552549159
+Version: 7.0.8649253175
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

