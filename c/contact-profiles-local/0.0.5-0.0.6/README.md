# Comparing `tmp/contact-profiles-local-0.0.5.tar.gz` & `tmp/contact-profiles-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact-profiles-local-0.0.5.tar", last modified: Fri Feb 23 10:23:15 2024, max compression
+gzip compressed data, was "contact-profiles-local-0.0.6.tar", last modified: Thu Apr 11 21:29:42 2024, max compression
```

## Comparing `contact-profiles-local-0.0.5.tar` & `contact-profiles-local-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 10:23:15.295860 contact-profiles-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-23 10:23:15.295860 contact-profiles-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 10:23:15.291859 contact-profiles-local-0.0.5/contact_profiles_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 10:23:15.295860 contact-profiles-local-0.0.5/contact_profiles_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/contact_profiles_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/contact_profiles_local/src/contact_profiles_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/contact_profiles_local/src/contact_profiles_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 10:23:15.295860 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-23 10:23:15.000000 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-23 10:23:15.000000 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 10:23:15.000000 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-23 10:23:15.000000 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-23 10:23:15.000000 contact-profiles-local-0.0.5/contact_profiles_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 10:23:15.295860 contact-profiles-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-23 10:22:18.000000 contact-profiles-local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7321 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 21:29:42.000000 contact-profiles-local-0.0.6/contact_profiles_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:29:42.429345 contact-profiles-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-11 21:29:16.000000 contact-profiles-local-0.0.6/setup.py
```

### Comparing `contact-profiles-local-0.0.5/PKG-INFO` & `contact-profiles-local-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profiles-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles contact-profiles-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-profiles-local-0.0.5/contact_profiles_local/src/contact_profiles_local.py` & `contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,57 +54,79 @@
         if person_ids:
             person_id = person_ids[0]
             profile_id_tuple = self.profiles_local.select_one_tuple_by_id(
                 select_clause_value="profile_id",
                 id_column_name="person_id",
                 id_column_value=person_id
             )
-        if not profile_id_tuple:
-            # Create a new  profile and add it to profile_table and profile_ml_table
-            logger.info(log_message="profile_id is None, creating a new profile and adding it to"
-                        " profile_table and profile_ml_table")
-            profile_dict = {
-                "person_id": person_id,
-                "name": contact_dict.get("display_as"),
-                "lang_code": self.lang_code.value,
-                "visibility_id": visibility_id,
-                "is_approved": is_approved,
-                "stars": stars,
-                "last_dialog_workflow_state_id": last_dialog_workflow_state_id
-            }
-            profile_id = self.profiles_local.insert(person_id=person_id, profile_dict=profile_dict)
-            if not profile_id:
-                logger.error(log_message="profile was not created and inserted to the database, profile_id is None")
-                return None
-            logger.info(log_message="profile was created and inserted to the database")
-            logger.info(log_message="Linking contact to profile")
-            contact_profile_id = self.insert_mapping(entity_name1=self.default_entity_name1,
-                                                     entity_name2=self.default_entity_name2,
-                                                     entity_id1=contact_id, entity_id2=profile_id)
-            if not contact_profile_id:
-                logger.error(log_message="contact was not linked to profile, contact_profile_id is None")
-                return None
-            logger.info(log_message="contact was linked to profile")
-        else:
-            # Check if there is link to existing profile
-            logger.info(log_message="Checking if there is link to existing profile")
-            profile_id = profile_id_tuple[0]
-            mapping_tuple_list = self.select_multi_mapping_tuple_by_id(entity_name1=self.default_entity_name1,
-                                                                       entity_name2=self.default_entity_name2,
-                                                                       entity_id1=contact_id,
-                                                                       entity_id2=profile_id)
-            if not mapping_tuple_list:
-                # Link contact to existing profile
-                logger.info(log_message="Linking contact to existing profile")
+            if not profile_id_tuple:
+                # Create a new  profile and add it to profile_table and profile_ml_table
+                logger.info(log_message="profile_id is None, creating a new profile and adding it to"
+                            " profile_table and profile_ml_table")
+                profile_dict = {
+                    "person_id": person_id,
+                    "name": contact_dict.get("display_as"),
+                    "lang_code": self.lang_code.value,
+                    "visibility_id": visibility_id,
+                    "is_approved": is_approved,
+                    "stars": stars,
+                    "last_dialog_workflow_state_id": last_dialog_workflow_state_id
+                }
+                profile_id = self.profiles_local.insert(
+                    person_id=person_id, profile_dict=profile_dict)
+                if not profile_id:
+                    logger.error(
+                        log_message="profile was not created and inserted to the database, profile_id is None")
+                    return None
+                logger.info(log_message="profile was created and inserted to the database")
+                logger.info(log_message="Linking contact to profile")
                 contact_profile_id = self.insert_mapping(entity_name1=self.default_entity_name1,
                                                          entity_name2=self.default_entity_name2,
                                                          entity_id1=contact_id, entity_id2=profile_id)
+                if not contact_profile_id:
+                    logger.error(
+                        log_message="contact was not linked to profile, contact_profile_id is None")
+                    return None
+                logger.info(log_message="contact was linked to profile")
+                self.__insert_person_profile(person_id=person_id, profile_id=profile_id)
             else:
-                logger.info(log_message="contact is already linked to profile")
-                contact_profile_id = mapping_tuple_list[0][0]
-        logger.end(object={"contact_profile_id": contact_profile_id})
-        insert_information = {
-            "contact_profile_id": contact_profile_id,
-            "contact_id": contact_id,
-            "profile_id": profile_id
-        }
-        return insert_information
+                # Check if there is link to existing profile
+                logger.info(log_message="Checking if there is link to existing profile")
+                profile_id = profile_id_tuple[0]
+                mapping_tuple_list = self.select_multi_mapping_tuple_by_id(entity_name1=self.default_entity_name1,
+                                                                           entity_name2=self.default_entity_name2,
+                                                                           entity_id1=contact_id,
+                                                                           entity_id2=profile_id)
+                if not mapping_tuple_list:
+                    # Link contact to existing profile
+                    logger.info(log_message="Linking contact to existing profile")
+                    contact_profile_id = self.insert_mapping(entity_name1=self.default_entity_name1,
+                                                             entity_name2=self.default_entity_name2,
+                                                             entity_id1=contact_id, entity_id2=profile_id)
+                else:
+                    logger.info(log_message="contact is already linked to profile")
+                    contact_profile_id = mapping_tuple_list[0][0]
+            logger.end(object={"contact_profile_id": contact_profile_id})
+            insert_information = {
+                "contact_profile_id": contact_profile_id,
+                "contact_id": contact_id,
+                "profile_id": profile_id
+            }
+            return insert_information
+        else:
+            logger.end(log_message="person_id is None")
+            return None
+
+    def __insert_person_profile(self, person_id: int, profile_id: int) -> int:
+        """
+        Insert person_profile
+        :param person_id: person_id
+        :param profile_id: profile_id
+        :return: person_profile_id
+        """
+        logger.start(object={"person_id": person_id, "profile_id": profile_id})
+        person_profile_id = self.insert_mapping(
+            schema_name="person_profile",
+            entity_name1="person", entity_name2="profile",
+            entity_id1=person_id, entity_id2=profile_id)
+        logger.end(object={"person_profile_id": person_profile_id})
+        return person_profile_id
```

### Comparing `contact-profiles-local-0.0.5/contact_profiles_local/src/contact_profiles_local_constants.py` & `contact-profiles-local-0.0.6/contact_profiles_local/src/contact_profiles_local_constants.py`

 * *Files identical despite different names*

### Comparing `contact-profiles-local-0.0.5/contact_profiles_local.egg-info/PKG-INFO` & `contact-profiles-local-0.0.6/contact_profiles_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-profiles-local
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyPI Package for Circles contact-profiles-local Python
 Home-page: https://github.com/circles-zone/contact-profile-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact-profiles-local-0.0.5/setup.py` & `contact-profiles-local-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-profiles-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.5',  # update only the minor version each time # https://pypi.org/project/contact-profiles-local/
+    version='0.0.6',  # update only the minor version each time # https://pypi.org/project/contact-profiles-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-profiles-local Python",
     long_description="PyPI Package for Circles contact-profiles-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/contact-profile-local-python-package",
     packages=[package_dir],
```

