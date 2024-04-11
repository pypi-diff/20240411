# Comparing `tmp/ezirion_api-0.1.0.tar.gz` & `tmp/ezirion_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezirion_api-0.1.0.tar", last modified: Thu Apr 11 00:04:15 2024, max compression
+gzip compressed data, was "ezirion_api-0.1.2.tar", last modified: Thu Apr 11 01:26:06 2024, max compression
```

## Comparing `ezirion_api-0.1.0.tar` & `ezirion_api-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 00:04:15.321803 ezirion_api-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      963 2024-04-11 00:04:15.318469 ezirion_api-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      742 2024-04-11 00:01:43.000000 ezirion_api-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 00:04:15.318469 ezirion_api-0.1.0/ezirion_api/
--rwxr-xr-x   0 root         (0) root         (0)       44 2024-04-09 19:48:59.000000 ezirion_api-0.1.0/ezirion_api/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      760 2024-04-10 15:27:59.000000 ezirion_api-0.1.0/ezirion_api/courses.py
--rw-r--r--   0 root         (0) root         (0)      188 2024-04-09 19:47:39.000000 ezirion_api-0.1.0/ezirion_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 00:04:15.318469 ezirion_api-0.1.0/ezirion_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      963 2024-04-11 00:04:15.000000 ezirion_api-0.1.0/ezirion_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2024-04-11 00:04:15.000000 ezirion_api-0.1.0/ezirion_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 00:04:15.000000 ezirion_api-0.1.0/ezirion_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-11 00:04:15.000000 ezirion_api-0.1.0/ezirion_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 00:04:15.321803 ezirion_api-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 00:02:41.000000 ezirion_api-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:26:06.433742 ezirion_api-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-11 01:26:06.433742 ezirion_api-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-11 01:25:46.000000 ezirion_api-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:26:06.433742 ezirion_api-0.1.2/ezirion_api/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-04-09 19:48:59.000000 ezirion_api-0.1.2/ezirion_api/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      731 2024-04-11 01:19:20.000000 ezirion_api-0.1.2/ezirion_api/courses.py
+-rw-r--r--   0 root         (0) root         (0)      188 2024-04-09 19:47:39.000000 ezirion_api-0.1.2/ezirion_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 01:26:06.433742 ezirion_api-0.1.2/ezirion_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-11 01:26:06.000000 ezirion_api-0.1.2/ezirion_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      226 2024-04-11 01:26:06.000000 ezirion_api-0.1.2/ezirion_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 01:26:06.000000 ezirion_api-0.1.2/ezirion_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-11 01:26:06.000000 ezirion_api-0.1.2/ezirion_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 01:26:06.433742 ezirion_api-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-11 01:20:10.000000 ezirion_api-0.1.2/setup.py
```

### Comparing `ezirion_api-0.1.0/PKG-INFO` & `ezirion_api-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezirion_api
-Version: 0.1.0
+Version: 0.1.2
 Summary: Biblioteca de mis cursos (Prueba para mi primera api)
 Home-page: https://miurlinventada.com
 Author: Adrián García
 Description-Content-Type: text/markdown
 
 # Mi primera API
 
@@ -20,14 +20,19 @@
 
 Instala el paquete usando `pip3`:
 
 ```python3
 pip3 install ezirion_api
 ```
 
+## Notas de versión 
+
+0.1.2 >>> Parche al llamar a la variable `courses` salía el objeto por pantalla y no sus propiedades.
+
+
 ## Uso básico
 
 ### Listar todos los cursos
 
 ```python
 from ezirion_api import list_courses
```

### Comparing `ezirion_api-0.1.0/README.md` & `ezirion_api-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 Instala el paquete usando `pip3`:
 
 ```python3
 pip3 install ezirion_api
 ```
 
+## Notas de versión 
+
+0.1.2 >>> Parche al llamar a la variable `courses` salía el objeto por pantalla y no sus propiedades.
+
+
 ## Uso básico
 
 ### Listar todos los cursos
 
 ```python
 from ezirion_api import list_courses
```

### Comparing `ezirion_api-0.1.0/ezirion_api/courses.py` & `ezirion_api-0.1.2/ezirion_api/courses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 class Course:
 
-    def __init__(self, name, duration, link):
-        self.name = name
-        self.duration = duration
-        self.link = link
+	def __init__(self, name, duration, link):
+		self.name = name
+		self.duration = duration
+		self.link = link
 
-    def __str__(self):
-        return f"{self.name} [{self.duration} horas] | Link: {self.link}"
+	def __repr__(self):
+		return f"{self.name} [{self.duration} horas] | Link: {self.link}"
 
 courses = [
     Course("Mi primer curso", 12, "https://milink1.com"),
     Course("Mi segundo curso", 15, "https://milink2.com"),
     Course("Mi tercer curso", 16, "https://milink3.com")
 ]
```

### Comparing `ezirion_api-0.1.0/ezirion_api.egg-info/PKG-INFO` & `ezirion_api-0.1.2/ezirion_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezirion_api
-Version: 0.1.0
+Version: 0.1.2
 Summary: Biblioteca de mis cursos (Prueba para mi primera api)
 Home-page: https://miurlinventada.com
 Author: Adrián García
 Description-Content-Type: text/markdown
 
 # Mi primera API
 
@@ -20,14 +20,19 @@
 
 Instala el paquete usando `pip3`:
 
 ```python3
 pip3 install ezirion_api
 ```
 
+## Notas de versión 
+
+0.1.2 >>> Parche al llamar a la variable `courses` salía el objeto por pantalla y no sus propiedades.
+
+
 ## Uso básico
 
 ### Listar todos los cursos
 
 ```python
 from ezirion_api import list_courses
```

