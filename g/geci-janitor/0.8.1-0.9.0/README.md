# Comparing `tmp/geci_janitor-0.8.1.tar.gz` & `tmp/geci_janitor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geci_janitor-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geci_janitor-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geci_janitor-0.8.1.tar` & `geci_janitor-0.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      449 2024-03-04 21:36:13.224394 geci_janitor-0.8.1/README.md
--rw-r--r--   0        0        0       81 2024-03-04 21:36:13.224394 geci_janitor-0.8.1/geci_janitor/__init__.py
--rw-r--r--   0        0        0     4223 2024-03-04 21:36:13.224394 geci_janitor-0.8.1/geci_janitor/cli.py
--rw-r--r--   0        0        0      504 2024-03-04 21:36:13.224394 geci_janitor-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 geci_janitor-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      449 2024-04-11 17:59:20.736105 geci_janitor-0.9.0/README.md
+-rw-r--r--   0        0        0       81 2024-04-11 17:59:20.736105 geci_janitor-0.9.0/geci_janitor/__init__.py
+-rw-r--r--   0        0        0     4655 2024-04-11 17:59:20.736105 geci_janitor-0.9.0/geci_janitor/cli.py
+-rw-r--r--   0        0        0      504 2024-04-11 17:59:20.736105 geci_janitor-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      840 1970-01-01 00:00:00.000000 geci_janitor-0.9.0/PKG-INFO
```

### Comparing `geci_janitor-0.8.1/geci_janitor/cli.py` & `geci_janitor-0.9.0/geci_janitor/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,26 @@
     command = f'docker run --volume $PWD:/workdir islasgeci/clean_camera_data R -e \'cameraData::add_data_check_column_to_campo("{file}", "{salida_campo}", "with_date_{salida_campo}")\''
     os.system(command)
     command = f'docker run --volume $PWD:/workdir islasgeci/clean_camera_data R -e \'cameraData::add_data_check_column_to_memoria("{file}", "{salida_memoria}", "with_date_{salida_memoria}")\''
     os.system(command)
 
 
 @janitor.command()
+def check_cameras_ids(
+    mapsource_path: str = typer.Option(),
+    revision_campo_path: str = "with_date_camaras_extra_revision_campo.csv",
+):
+    """
+    Check if all cameras are listed in Mapsource and revision_campo.
+    """
+    command = f'docker run --volume $PWD:/workdir islasgeci/read_mapsource Rscript -e \'readMS::check_cameras("{revision_campo_path}", "{mapsource_path}")\''
+    os.system(command)
+
+
+@janitor.command()
 def cameras_info(file: str = "camaras_extra_revision_campo.csv"):
     """
     Get cameras info. Run after `clean-cameras` command.
     """
     command = f'docker run --volume $PWD:/workdir islasgeci/clean_camera_data R -e \'cameraData::write_camera_info("{file}", "cameras_info.csv")\''
     os.system(command)
     command = f'docker run --volume $PWD:/workdir islasgeci/clean_camera_data R -e \'cameraData::write_cameras_last_check("{file}", "cameras_last_check.csv")\''
```

### Comparing `geci_janitor-0.8.1/PKG-INFO` & `geci_janitor-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geci_janitor
-Version: 0.8.1
+Version: 0.9.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/janitor
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: geci_janitor Version: 0.8.1 Summary: A template
+Metadata-Version: 2.1 Name: geci_janitor Version: 0.9.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/janitor Author: Ciencia
 de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-Python:
 >=3.9 Description-Content-Type: text/markdown Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 typer[all] # Janitor _[_h_t_t_p_s_:_/_/_w_w_w_._i_s_l_a_s_._o_r_g_._m_x_/_i_m_g_/_l_o_g_o_._s_v_g_][![codecov](https:/
 /codecov.io/gh/IslasGECI/janitor/branch/develop/graph/
 badge.svg?token=zXmBXOWRbG)](https://codecov.io/gh/IslasGECI/janitor) ![PyPI -
```

