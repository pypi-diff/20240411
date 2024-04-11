# Comparing `tmp/screenapi_cli-0.1.5a1.tar.gz` & `tmp/screenapi_cli-0.1.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenapi_cli-0.1.5a1.tar", max compression
+gzip compressed data, was "screenapi_cli-0.1.5a2.tar", max compression
```

## Comparing `screenapi_cli-0.1.5a1.tar` & `screenapi_cli-0.1.5a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a1/LICENSE
--rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a1/README.md
--rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a1/app/__init__.py
--rw-r--r--   0        0        0     9241 2024-04-06 03:08:21.572497 screenapi_cli-0.1.5a1/app/__main__.py
--rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a1/app/common.py
--rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a1/app/export/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-26 08:34:32.751466 screenapi_cli-0.1.5a1/app/export/cli.py
--rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a1/app/setup/__init__.py
--rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a1/app/setup/utils.py
--rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a1/app/txt/__init__.py
--rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a1/app/txt/cli.py
--rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a1/app/txt/deprecated_cli.py
--rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a1/app/xlsx/__init__.py
--rw-r--r--   0        0        0    10280 2024-04-06 05:15:13.050341 screenapi_cli-0.1.5a1/app/xlsx/main.py
--rw-r--r--   0        0        0      768 2024-04-06 02:55:02.617598 screenapi_cli-0.1.5a1/pyproject.toml
--rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-03-23 16:06:49.120124 screenapi_cli-0.1.5a2/LICENSE
+-rw-r--r--   0        0        0     1381 2024-03-25 19:41:34.179648 screenapi_cli-0.1.5a2/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 06:15:38.237432 screenapi_cli-0.1.5a2/app/__init__.py
+-rw-r--r--   0        0        0     9241 2024-04-11 16:34:55.215188 screenapi_cli-0.1.5a2/app/__main__.py
+-rw-r--r--   0        0        0     1360 2024-04-01 07:33:03.304661 screenapi_cli-0.1.5a2/app/common.py
+-rw-r--r--   0        0        0        0 2024-03-24 18:09:29.678307 screenapi_cli-0.1.5a2/app/export/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-26 08:34:32.751466 screenapi_cli-0.1.5a2/app/export/cli.py
+-rw-r--r--   0        0        0        0 2024-03-24 14:33:45.903715 screenapi_cli-0.1.5a2/app/setup/__init__.py
+-rw-r--r--   0        0        0     1083 2024-03-25 19:15:41.722738 screenapi_cli-0.1.5a2/app/setup/utils.py
+-rw-r--r--   0        0        0       97 2024-03-24 17:32:30.550768 screenapi_cli-0.1.5a2/app/txt/__init__.py
+-rw-r--r--   0        0        0     5737 2024-03-29 09:45:40.583647 screenapi_cli-0.1.5a2/app/txt/cli.py
+-rw-r--r--   0        0        0     6056 2024-03-25 18:55:58.756247 screenapi_cli-0.1.5a2/app/txt/deprecated_cli.py
+-rw-r--r--   0        0        0        0 2024-03-27 04:52:19.596215 screenapi_cli-0.1.5a2/app/xlsx/__init__.py
+-rw-r--r--   0        0        0    10708 2024-04-11 16:39:15.866431 screenapi_cli-0.1.5a2/app/xlsx/main.py
+-rw-r--r--   0        0        0      795 2024-04-11 16:46:32.022697 screenapi_cli-0.1.5a2/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 screenapi_cli-0.1.5a2/PKG-INFO
```

### Comparing `screenapi_cli-0.1.5a1/LICENSE` & `screenapi_cli-0.1.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/README.md` & `screenapi_cli-0.1.5a2/README.md`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/__main__.py` & `screenapi_cli-0.1.5a2/app/__main__.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/common.py` & `screenapi_cli-0.1.5a2/app/common.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/export/cli.py` & `screenapi_cli-0.1.5a2/app/export/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/setup/utils.py` & `screenapi_cli-0.1.5a2/app/setup/utils.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/txt/cli.py` & `screenapi_cli-0.1.5a2/app/txt/cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/txt/deprecated_cli.py` & `screenapi_cli-0.1.5a2/app/txt/deprecated_cli.py`

 * *Files identical despite different names*

### Comparing `screenapi_cli-0.1.5a1/app/xlsx/main.py` & `screenapi_cli-0.1.5a2/app/xlsx/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import concurrent.futures
 from click import echo
 from rich.progress import TaskID, Progress
 import pandas
 import configparser
 from rich import print
 from httpx import Client
+from difflib import SequenceMatcher
 from app.common import providers_pattern, sheetType
 from app.txt.cli import getId
 from app.setup.utils import config_file
 
 # global output_dir
 config = configparser.ConfigParser()
 config.read(config_file())
@@ -60,14 +61,24 @@
 
 
 def convert_to_json(input_path: Path, site: sheetType, save: Optional[bool] = True):
     # setup input_path and output_file (excel to json)
 
     # read excel, rename column, fix date
     df = pandas.read_excel(input_path)
+    # serialNumberCell = df.columns[0]
+    firstColumnMatchRatio = SequenceMatcher(
+        a="S.No.", b=df.columns[0]
+    ).real_quick_ratio()
+
+    # print({ "firstColumnMatchRatio": firstColumnMatchRatio })
+    if firstColumnMatchRatio > 0.7 and firstColumnMatchRatio != 1.0:
+        print("[dim]`S.No.` column is probably in wrong format, fixing..[/]")
+        df.rename(columns={df.columns[0]: "S.No."}, inplace=True)
+
     df.rename(columns=read_mapping(site.value), inplace=True)
 
     if not df["Date Added"].isna().all():
         try:
             df["Date Added"] = df["Date Added"].dt.strftime("%d/%m/%Y")
         except AttributeError:
             try:
@@ -313,29 +324,28 @@
         #             Path(input_path).parent, Path(input_path).stem, "images"
         #         ),
         #     }
         # )
         shutil.copytree(
             os.path.join(output_dir, "images"),
             os.path.join(Path(input_path).parent, Path(input_path).stem, "images"),
-            dirs_exist_ok=True
+            dirs_exist_ok=True,
         )
 
     shutil.move(
         os.path.join(output_dir, Path(input_path).stem + ".xlsx"),
         os.path.join(
             Path(input_path).parent,
             Path(input_path).stem,
             Path(input_path).stem + ".xlsx",
         ),
     )
 
     print("Done!")
 
 
-# if __name__ == "__main__":
-#     main(
-#         input_path=Path("./dumps/Lakme Eyeconic 18-03-2024.xlsx"),
-#         site=[sheetType.meesho, sheetType.flipkart],
-#         max_workers=3,
-#         save=True,
-#     )
+if __name__ == "__main__":
+    convert_to_json(
+        input_path=Path("/home/rony/Downloads/Elle 18 09-04-2024_Shreya Jain.xlsx"),
+        site=sheetType.ecom,
+        save=True,
+    )
```

### Comparing `screenapi_cli-0.1.5a1/pyproject.toml` & `screenapi_cli-0.1.5a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "screenapi-cli"
-version = "0.1.5a1"
+version = "0.1.5a2"
 description = "A cli interface to interact with screenapi"
 authors = ["RONY <iamrony777@pm.me>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "app" },
 ]
@@ -19,14 +19,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.2.1"
 httpx = {extras = ["http2"], version = "^0.27.0"}
 typer = {extras = ["all"], version = "^0.10.0"}
 openpyxl = "^3.1.2"
+python-calamine = "^0.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 
 
 [build-system]
```

### Comparing `screenapi_cli-0.1.5a1/PKG-INFO` & `screenapi_cli-0.1.5a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: screenapi-cli
-Version: 0.1.5a1
+Version: 0.1.5a2
 Summary: A cli interface to interact with screenapi
 License: MIT
 Author: RONY
 Author-email: iamrony777@pm.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: python-calamine (>=0.2.0,<0.3.0)
 Requires-Dist: typer[all] (>=0.10.0,<0.11.0)
 Description-Content-Type: text/markdown
 
 # screenapi-cli
 
 ## Installation
```

