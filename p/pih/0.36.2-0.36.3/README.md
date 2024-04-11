# Comparing `tmp/pih-0.36.2.tar.gz` & `tmp/pih-0.36.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.2.tar", last modified: Wed Apr 10 10:22:39 2024, max compression
+gzip compressed data, was "pih-0.36.3.tar", last modified: Wed Apr 10 22:20:22 2024, max compression
```

## Comparing `pih-0.36.2.tar` & `pih-0.36.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.835213 pih-0.36.2/
--rw-rw-rw-   0        0        0      249 2024-04-10 10:22:39.788345 pih-0.36.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:37.013144 pih-0.36.2/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.2/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:37.381862 pih-0.36.2/pih/collections/
--rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.2/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.2/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.2/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.2/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.265255 pih-0.36.2/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-10 10:21:26.000000 pih-0.36.2/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.2/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.2/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.2/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.2/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.2/pih/consts/errors.py
--rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.2/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.2/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.2/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.2/pih/consts/hosts.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.2/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.2/pih/consts/password.py
--rw-rw-rw-   0        0        0    11367 2024-04-10 03:41:38.000000 pih-0.36.2/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11074 2024-03-13 06:46:40.000000 pih-0.36.2/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.2/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.2/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.2/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.2/pih/consts/service.py
--rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.2/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.2/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.2/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.2/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.2/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   547814 2024-04-10 10:20:59.000000 pih-0.36.2/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.531925 pih-0.36.2/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.2/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.2/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.2/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.2/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.678990 pih-0.36.2/pih/tools/
--rw-rw-rw-   0        0        0    51419 2024-04-10 09:08:04.000000 pih-0.36.2/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.2/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.2/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-10 10:22:39.741479 pih-0.36.2/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      938 2024-04-10 10:22:36.000000 pih-0.36.2/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-10 10:22:35.000000 pih-0.36.2/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 10:22:39.835213 pih-0.36.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:22.157972 pih-0.36.3/
+-rw-rw-rw-   0        0        0      249 2024-04-10 22:20:22.126710 pih-0.36.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:19.362056 pih-0.36.3/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.3/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:20.085100 pih-0.36.3/pih/collections/
+-rw-rw-rw-   0        0        0    28187 2024-04-04 06:10:57.000000 pih-0.36.3/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.3/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.3/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.3/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:21.613499 pih-0.36.3/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-10 22:19:25.000000 pih-0.36.3/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.3/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.3/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.3/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.3/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.3/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    29599 2024-04-09 12:52:51.000000 pih-0.36.3/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.3/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.3/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.3/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.3/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.3/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.3/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11096 2024-04-10 11:19:30.000000 pih-0.36.3/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.3/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.3/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.3/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.3/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6537 2024-03-06 10:20:49.000000 pih-0.36.3/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12172 2024-03-13 04:17:39.000000 pih-0.36.3/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.3/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.3/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.3/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   547821 2024-04-10 22:10:26.000000 pih-0.36.3/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:21.816636 pih-0.36.3/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.3/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.3/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.3/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.3/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:21.999646 pih-0.36.3/pih/tools/
+-rw-rw-rw-   0        0        0    51419 2024-04-10 09:08:04.000000 pih-0.36.3/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.3/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.3/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-10 22:20:22.078771 pih-0.36.3/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-10 22:20:18.000000 pih-0.36.3/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      938 2024-04-10 22:20:18.000000 pih-0.36.3/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 22:20:18.000000 pih-0.36.3/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-10 22:20:18.000000 pih-0.36.3/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-10 22:20:18.000000 pih-0.36.3/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-10 22:20:22.173633 pih-0.36.3/setup.cfg
```

### Comparing `pih-0.36.2/pih/collections/__init__.py` & `pih-0.36.3/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/collections/service.py` & `pih-0.36.3/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/console_api.py` & `pih-0.36.3/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/console_api_wrapper.py` & `pih-0.36.3/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/__init__.py` & `pih-0.36.3/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.2"
+VERSION: str = "0.36.3"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36.2/pih/consts/ad.py` & `pih-0.36.3/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/addresses.py` & `pih-0.36.3/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/date_time.py` & `pih-0.36.3/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/errors.py` & `pih-0.36.3/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/events.py` & `pih-0.36.3/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/hosts.py` & `pih-0.36.3/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/names.py` & `pih-0.36.3/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/password.py` & `pih-0.36.3/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/paths.py` & `pih-0.36.3/pih/consts/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     PATH: str = os.path.join(AD.PATH_ROOT, NAME)
 
 
 class PATH_FACADE:
     LINUX_MOUNT_POINT: str = j((PATH_SPLITTER, "mnt"))
     SHARED_POINT_PATH: str = os.path.join("S$", FACADE.NAME)
     LINUX_MOUNT_POINT_PATH: str = j((LINUX_MOUNT_POINT, FACADE.NAME), PATH_SPLITTER)
+    FILES_NAME: str = ".files"
+    TOOLS_NAME: str = ".tools"
 
     VALUE: str = j(
         (
             PATH_DOUBLE_SPLITTER,
             AD.DOMAIN_MAIN,
             PATH_SPLITTER,
             FACADE.NAME,
@@ -42,29 +44,45 @@
     def SERVICE(service_name: str) -> str:
         return os.path.join(
             PATH_FACADE.VALUE,
             FACADE.SERVICE_NAME(service_name),
         )
 
     @staticmethod
+    def SERVICE_FILES(standalone_name: str) -> str:
+        return os.path.join(PATH_FACADE.FILES(), standalone_name)
+
+    @staticmethod
+    def SERVICE_TOOLS(standalone_name: str) -> str:
+        return os.path.join(PATH_FACADE.TOOLS(), standalone_name)
+
+    @staticmethod
+    def FILES() -> str:
+        return os.path.join(PATH_FACADE.VALUE, PATH_FACADE.FILES_NAME)
+
+    @staticmethod
+    def TOOLS() -> str:
+        return os.path.join(PATH_FACADE.VALUE, PATH_FACADE.TOOLS_NAME)
+
+    @staticmethod
     def STORAGE() -> str:
         return os.path.join(r"\\", Hosts.DC1.NAME, PATH_FACADE.SHARED_POINT_PATH)
 
     class DITRIBUTIVE:
 
-        DELIMITER: str = "-"
+        SPLITTER: str = "-"
         FOLDER_NAME: str = ".distr"
         PACKAGE_FOLDER_NAME: str = "all"
         DEFAULT_PACKAGE_TAG: str = "py3-none-any"
 
         @staticmethod
         def NAME(value: str, version: str | None = None) -> str:
             return j(
                 (ROOT_MODULE_NAME, value, None if n(version) else j(("==", version))),
-                PATH_FACADE.DITRIBUTIVE.DELIMITER,
+                PATH_FACADE.DITRIBUTIVE.SPLITTER,
             )
 
         @staticmethod
         def VALUE() -> str:
             return os.path.join(PATH_FACADE.VALUE, PATH_FACADE.DITRIBUTIVE.FOLDER_NAME)
 
         @staticmethod
@@ -82,22 +100,22 @@
                 try:
                     dist: Distribution = Distribution(
                         attrs={"name": name, "version": version}
                     )
                     bdist_wheel_cmd = dist.get_command_obj("bdist_wheel")
                     bdist_wheel_cmd.ensure_finalized()
                     dist_name = bdist_wheel_cmd.wheel_dist_name
-                    tag = PATH_FACADE.DITRIBUTIVE.DELIMITER.join(
+                    tag = PATH_FACADE.DITRIBUTIVE.SPLITTER.join(
                         bdist_wheel_cmd.get_tag()
                     )
                 except BaseException as _:
-                    dist_name = PATH_FACADE.DITRIBUTIVE.DELIMITER.join((name, version))
+                    dist_name = PATH_FACADE.DITRIBUTIVE.SPLITTER.join((name, version))
                     tag = PATH_FACADE.DITRIBUTIVE.DEFAULT_PACKAGE_TAG
                 return PathTool.add_extension(
-                    j((dist_name, PATH_FACADE.DITRIBUTIVE.DELIMITER, tag)),
+                    j((dist_name, PATH_FACADE.DITRIBUTIVE.SPLITTER, tag)),
                     PYTHON.PACKAGE_EXTENSION,
                 )
 
             return os.path.join(
                 *[
                     PATH_FACADE.DITRIBUTIVE.PACKAGE_FOLDER(name, version),
                     wheel_name(
```

### Comparing `pih-0.36.2/pih/consts/polibase.py` & `pih-0.36.3/pih/consts/polibase.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         "согласен",
         "согласна",
         "ok",
         "ок",
         "yes",
         "хорошо",
         "ага",
+        "можно"
     )
 
     NO_ANSWER: tuple[str, ...] = ("нет", "не согласен", "не согласна", "no", "занят")
 
     TAKE_TELEGRAM_BOT_URL_TEXT: str = "*{name}*, отправляем Вам ссылку:\n"
     TAKE_TELEGRAM_BOT_URL_PERSONLESS_TEXT: str = "Отправляем Вам ссылку:\n"
```

### Comparing `pih-0.36.2/pih/consts/service.py` & `pih-0.36.3/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/service_commands.py` & `pih-0.36.3/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/service_roles.py` & `pih-0.36.3/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/consts/settings.py` & `pih-0.36.3/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/pih.py` & `pih-0.36.3/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -3450,15 +3450,15 @@
             return PIH.DATA.CHECK.returncode(result) and (
                 output.count("(TTL)") < count or output.count("TTL=") < count
             )
 
         @staticmethod
         def get_executor_path(executor_name: str) -> str:
             return PIH.PATH.for_windows(
-                PIH.PATH.join(PATHS.WS.PATH, CONST.PSTOOLS.NAME, executor_name)
+                PIH.PATH.join(PATHS.FACADE.TOOLS(), CONST.PSTOOLS.NAME, executor_name)
             )
 
         @staticmethod
         def create_command_for_executor(
             executor_name: str,
             command: tuple[str, ...] | str,
             login: str | None = None,
```

### Comparing `pih-0.36.2/pih/rpc/__init__.py` & `pih-0.36.3/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.3/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.3/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/tools/__init__.py` & `pih-0.36.3/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/tools/service.py` & `pih-0.36.3/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih/widgets.py` & `pih-0.36.3/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.2/pih.egg-info/SOURCES.txt` & `pih-0.36.3/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

