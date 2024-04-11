# Comparing `tmp/contact-local-0.0.8.tar.gz` & `tmp/contact-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-local-0.0.8.tar", last modified: Wed Aug 23 11:07:18 2023, max compression
+gzip compressed data, was "contact-local-0.0.9.tar", last modified: Wed Aug 23 11:17:48 2023, max compression
```

## Comparing `contact-local-0.0.8.tar` & `contact-local-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.838225 contact-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-23 11:07:18.834225 contact-local-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.830225 contact-local-0.0.8/contact-local-python-package/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.834225 contact-local-0.0.8/contact-local-python-package/contact_api/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/contact_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6374 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/contact_api/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.834225 contact-local-0.0.8/contact-local-python-package/db/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5122 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/db/contactView.py
--rw-r--r--   0 runner    (1001) docker     (999)      285 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/db/database.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.834225 contact-local-0.0.8/contact-local-python-package/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2675 2023-08-23 11:06:59.000000 contact-local-0.0.8/contact-local-python-package/tests/contact_test.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 11:07:18.834225 contact-local-0.0.8/contact_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-23 11:07:18.000000 contact-local-0.0.8/contact_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-23 11:07:18.000000 contact-local-0.0.8/contact_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-23 11:07:18.000000 contact-local-0.0.8/contact_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-08-23 11:07:18.000000 contact-local-0.0.8/contact_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      445 2023-08-23 11:06:59.000000 contact-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-23 11:07:18.838225 contact-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      706 2023-08-23 11:06:59.000000 contact-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.950750 contact-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-23 11:17:48.946750 contact-local-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.946750 contact-local-0.0.9/contact-local-python-package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.946750 contact-local-0.0.9/contact-local-python-package/contact_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/contact_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/contact_api/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.946750 contact-local-0.0.9/contact-local-python-package/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/db/contactView.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/db/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.946750 contact-local-0.0.9/contact-local-python-package/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-23 11:17:26.000000 contact-local-0.0.9/contact-local-python-package/tests/contact_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 11:17:48.946750 contact-local-0.0.9/contact_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-23 11:17:48.000000 contact-local-0.0.9/contact_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-08-23 11:17:48.000000 contact-local-0.0.9/contact_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 11:17:48.000000 contact-local-0.0.9/contact_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-23 11:17:48.000000 contact-local-0.0.9/contact_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-23 11:17:26.000000 contact-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-23 11:17:48.950750 contact-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-23 11:17:26.000000 contact-local-0.0.9/setup.py
```

### Comparing `contact-local-0.0.8/contact-local-python-package/contact_api/contact.py` & `contact-local-0.0.9/contact-local-python-package/contact_api/contact.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 class contact(generic_crud.GenericCRUD):
 
     def __init__(self) -> None:
         pass
 
     @staticmethod
-    def insert(first_name, last_name, phone,
-               birthday, email, location, job_title, organization):
+    def insert(first_name:str, last_name:str, phone:str,
+               birthday:str, email:str, location:str, job_title:str, organization:str)->int:
         try:
             connection = Connector.get_connection("contact")
             object1 = {
                 'first_name': first_name,
                 'last_name': last_name,
                 'phone': phone,
                 'birthday': birthday,
@@ -80,15 +80,16 @@
         finally:
             cursor.close()
 
             logger.end("contact added", object={'contact_id': contact_id})
             return contact_id
 
     @staticmethod
-    def update(person_id, name_prefix, first_name, additional_name, job_title, contact_id):
+    def update(person_id:int, name_prefix:str, first_name:str, additional_name:str, job_title:str,
+                contact_id:int)->None:
         try:
             connection = Connector.get_connection("contact")
 
             object1 = {
                 'person_id': person_id,
                 'name_prefix': name_prefix,
                 'first_name': first_name,
@@ -124,15 +125,15 @@
         except Exception as err:
             logger.exception(f"Contact.update Error: {err}", object=err)
         finally:
             logger.end("contact updated", object={'contact_id': contact_id})
             cursor.close()
 
     @staticmethod
-    def delete(contact_id):
+    def delete(contact_id:int)->None:
         try:
             object1 = {
                 'contact_id': contact_id,
             }
             logger.start(object=object1)
             connection = Connector.get_connection("contact")
             cursor = connection.cursor(buffered=True)
@@ -157,15 +158,15 @@
             logger.exception(f"Contact.delete Error: {err}", object=err)
         finally:
             cursor.close()
 
             logger.end("contact deleted", object={'contact_id': contact_id})
 
     @staticmethod
-    def insert_batch(contact_list):
+    def insert_batch(contact_list:list)->list:
         try:
 
             object1 = {
                 'listToInsert': contact_list
             }
             logger.start(object=object1)
             connection = Connector.get_connection("contact")
```

### Comparing `contact-local-0.0.8/contact-local-python-package/db/contactView.py` & `contact-local-0.0.9/contact-local-python-package/db/contactView.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                             )
                         """)
     # commit change and Close the database connection
     connection.commit()
     mycursor.close()
 
 
-def get_contact_by_id(contact_id):
+def get_contact_by_id(contact_id:int)->tuple:
     try:
         connection = Connector.get_connection("contact")
         cursor = connection.cursor(buffered=True)
         select_query = """
         SELECT * FROM contact.contact_table
         WHERE
             contact_id = %s
@@ -96,15 +96,15 @@
         cursor.execute(select_query, (contact_id,))
         result = cursor.fetchone()
         return result
     except mysql.connector.Error as err:
         logger.exception(f"Contact.get_contact_by_id Error: {err}", object=err)
 
 
-def get_contact_by_first_name(first_name):
+def get_contact_by_first_name(first_name:str)->tuple:
     try:
 
         connection = Connector.get_connection("contact")
         cursor = connection.cursor(buffered=True)
         select_query = """
         SELECT * FROM contact.contact_table
         WHERE
```

### Comparing `contact-local-0.0.8/contact-local-python-package/tests/contact_test.py` & `contact-local-0.0.9/contact-local-python-package/tests/contact_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,7 +99,8 @@
         'organization': 'Web Solutions'
     }
 ]
 
     inserted_ids = contact.insert_batch(contacts_to_insert)
     inserted_ids is not None
     logger.end("success")
+test_update()
```

### Comparing `contact-local-0.0.8/contact_local.egg-info/SOURCES.txt` & `contact-local-0.0.9/contact_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contact-local-0.0.8/setup.py` & `contact-local-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name='contact-local',
-    version='0.0.8',
+    version='0.0.9',
     author="Circlez",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-local Local/Remote Python",
     long_description="This is a package for sharing common contact function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles",
     packages=setuptools.find_packages(),
```

