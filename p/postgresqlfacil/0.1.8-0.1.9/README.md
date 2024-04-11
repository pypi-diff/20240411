# Comparing `tmp/postgresqlfacil-0.1.8.tar.gz` & `tmp/postgresqlfacil-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresqlfacil-0.1.8.tar", max compression
+gzip compressed data, was "postgresqlfacil-0.1.9.tar", max compression
```

## Comparing `postgresqlfacil-0.1.8.tar` & `postgresqlfacil-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1093 2023-08-25 19:59:40.553808 postgresqlfacil-0.1.8/LICENSE
--rw-r--r--   0        0        0       64 2023-08-28 18:27:49.420723 postgresqlfacil-0.1.8/postgresqlfacil/__init__.py
--rw-r--r--   0        0        0     4948 2023-10-19 20:13:50.855051 postgresqlfacil-0.1.8/postgresqlfacil/postgresqlfacil.py
--rw-r--r--   0        0        0      600 2023-11-10 13:26:11.081585 postgresqlfacil-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2448 2023-08-29 18:46:47.720724 postgresqlfacil-0.1.8/README.md
--rw-r--r--   0        0        0     3225 1970-01-01 00:00:00.000000 postgresqlfacil-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-08-25 19:59:40.553808 postgresqlfacil-0.1.9/LICENSE
+-rw-r--r--   0        0        0       64 2023-08-28 18:27:49.420723 postgresqlfacil-0.1.9/postgresqlfacil/__init__.py
+-rw-r--r--   0        0        0     4952 2024-04-11 17:28:50.217742 postgresqlfacil-0.1.9/postgresqlfacil/postgresqlfacil.py
+-rw-r--r--   0        0        0      600 2024-04-11 17:28:50.224510 postgresqlfacil-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2448 2023-08-29 18:46:47.720724 postgresqlfacil-0.1.9/README.md
+-rw-r--r--   0        0        0     3276 1970-01-01 00:00:00.000000 postgresqlfacil-0.1.9/PKG-INFO
```

### Comparing `postgresqlfacil-0.1.8/LICENSE` & `postgresqlfacil-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresqlfacil-0.1.8/postgresqlfacil/postgresqlfacil.py` & `postgresqlfacil-0.1.9/postgresqlfacil/postgresqlfacil.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
     @staticmethod
     def transforma_df_em_insert_statement(
         df: pd.DataFrame, tabela: str
     ) -> str:
         query = f"""
             INSERT INTO {tabela}
-            ({",".join(x for x in df.columns)})
+            ("{'","'.join(x for x in df.columns)}")
             VALUES
             """
         for linha in df.itertuples():
             values = " ("
             for index, coluna in enumerate(df.columns):
                 value = getattr(linha, coluna)
                 if isinstance(value, str):
```

### Comparing `postgresqlfacil-0.1.8/pyproject.toml` & `postgresqlfacil-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgresqlfacil"
-version = "0.1.8"
+version = "0.1.9"
 description = "O pacote PostgreSQLFacil oferece uma interface simplificada para interagir com o banco de dados PostgreSQL, abstraindo as operações comuns de SELECT, INSERT, UPDATE e DELETE em métodos convenientes e com integrações em DataFrames do pandas."
 authors = ["eduardo.barreto <edugobarreto@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
```

### Comparing `postgresqlfacil-0.1.8/README.md` & `postgresqlfacil-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `postgresqlfacil-0.1.8/PKG-INFO` & `postgresqlfacil-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: postgresqlfacil
-Version: 0.1.8
+Version: 0.1.9
 Summary: O pacote PostgreSQLFacil oferece uma interface simplificada para interagir com o banco de dados PostgreSQL, abstraindo as operações comuns de SELECT, INSERT, UPDATE e DELETE em métodos convenientes e com integrações em DataFrames do pandas.
 License: MIT
 Author: eduardo.barreto
 Author-email: edugobarreto@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2 (>=2.9.7,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PostgreSQLFacil
 O pacote PostgreSQLFacil oferece uma interface simplificada para interagir com o banco de dados PostgreSQL, abstraindo as operações comuns de SELECT, INSERT, UPDATE e DELETE em métodos convenientes e com integrações em DataFrames do pandas.
```

