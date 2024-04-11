# Comparing `tmp/t_bug_catcher-0.4.1.tar.gz` & `tmp/t_bug_catcher-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-fga7s_nv/t_bug_catcher-0.4.1.tar", last modified: Mon Apr  8 11:24:56 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-956qxe83/t_bug_catcher-0.4.2.tar", last modified: Wed Apr 10 13:16:11 2024, max compression
```

## Comparing `t_bug_catcher-0.4.1.tar` & `t_bug_catcher-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/bug_catcher.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/bug_snag.py
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/config.py
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    44739 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/jira.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/resources/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/resources/whispers_config.yml
--rw-rw-rw-   0 root         (0) root         (0)     5845 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/stack_saver.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/t_bug_catcher/utils/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1108 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/common.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/t_bug_catcher/workitems.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.803412 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-08 11:24:56.000000 t_bug_catcher-0.4.1/t_bug_catcher.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-08 11:24:56.799412 t_bug_catcher-0.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-08 11:24:26.000000 t_bug_catcher-0.4.1/tests/test_t_bug_catcher.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-10 13:16:11.299898 t_bug_catcher-0.4.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.291898 t_bug_catcher-0.4.2/t_bug_catcher/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10746 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/bug_catcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3115 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/bug_snag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    44739 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/jira.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/resources/whispers_config.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/stack_saver.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2051 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/t_bug_catcher/workitems.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2024-04-10 13:16:11.000000 t_bug_catcher-0.4.2/t_bug_catcher.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-10 13:16:11.295898 t_bug_catcher-0.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2934 2024-04-10 13:15:38.000000 t_bug_catcher-0.4.2/tests/test_t_bug_catcher.py
```

### Comparing `t_bug_catcher-0.4.1/PKG-INFO` & `t_bug_catcher-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.1
+Version: 0.4.2
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.1/README.rst` & `t_bug_catcher-0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/setup.py` & `t_bug_catcher-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
     description="Bug catcher",
     long_description=readme,
     keywords="t_bug_catcher",
     name="t_bug_catcher",
     packages=find_packages(include=["t_bug_catcher", "t_bug_catcher.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.4.1",
+    version="0.4.2",
     zip_safe=False,
     install_requires=install_requirements,
     include_package_data=True,
     package_data={"": ["resources/*.yml"]},
 )
```

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/bug_catcher.py` & `t_bug_catcher-0.4.2/t_bug_catcher/bug_catcher.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/bug_snag.py` & `t_bug_catcher-0.4.2/t_bug_catcher/bug_snag.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/config.py` & `t_bug_catcher-0.4.2/t_bug_catcher/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         MAX_ISSUE_ATTACHMENTS: int = 100
         MAX_DESCRIPTION_LENGTH: int = 250
         SUMMARY_LENGTH: int = 120
         STACK_SCOPE: int = 3
 
     SUPPORT_BOARD = "AB"
 
+    KEYS_TO_REMOVE = ["credential", "password"]
+
     RC_RUN_LINK = (
         f"https://cloud.robocorp.com/organizations/{os.environ.get('RC_ORGANIZATION_ID')}"
         f"/workspaces/{os.environ.get('RC_WORKSPACE_ID')}/processes"
         f"/{os.environ.get('RC_PROCESS_ID')}/runs/{os.environ.get('RC_PROCESS_RUN_ID')}/"
         f"stepRuns/{os.environ.get('RC_ACTIVITY_RUN_ID')}/"
     )
```

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/jira.py` & `t_bug_catcher-0.4.2/t_bug_catcher/jira.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/resources/whispers_config.yml` & `t_bug_catcher-0.4.2/t_bug_catcher/resources/whispers_config.yml`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/stack_saver.py` & `t_bug_catcher-0.4.2/t_bug_catcher/stack_saver.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from types import FunctionType, ModuleType
 from typing import Optional
 
 import whispers
 
 from .config import CONFIG
 from .utils import logger
-from .utils.common import Encoder
+from .utils.common import Encoder, convert_keys_to_primitives
 
 
 class StackSaver:
     """A class to save the stack trace."""
 
     def __init__(self):
         """Initializes the StackSaver class."""
@@ -30,41 +30,25 @@
             path (str): The path from which to strip the current working directory path.
 
         Returns:
             str: The stripped path.
         """
         return path.replace(os.getcwd(), "").strip(os.sep)
 
-    @staticmethod
-    def serialize_frame_info(frame_info: dict) -> dict:
+    def serialize_frame_info(self, frame_info: dict) -> dict:
         """A static method to serialize the frame info.
 
         Args:
             frame_info (dict): The frame info to be serialized.
 
         Returns:
             dict: The serialized frame info.
         """
-        run_locals = {}
-        run_args = {}
-        if frame_info["locals"]:
-            for key, value in frame_info["locals"].items():
-                if str(key).lower() == "credentials":
-                    continue
-                if isinstance(value, dict):
-                    run_locals[str(key)] = value
-                else:
-                    run_locals[str(key)] = str(value)
-        for key, value in frame_info["args"].items():
-            if str(key).lower() == "credentials":
-                continue
-            if isinstance(value, dict):
-                run_args[str(key)] = value
-            else:
-                run_args[str(key)] = str(value)
+        run_locals = convert_keys_to_primitives(frame_info["locals"]) if frame_info["locals"] else {}
+        run_args = convert_keys_to_primitives(frame_info["args"]) if frame_info["args"] else {}
         serializable_frame_info = {
             "filename": frame_info["filename"],
             "function_name": frame_info["function_name"],
             "locals": run_locals,
             "args": run_args,
         }
         return serializable_frame_info
@@ -84,15 +68,15 @@
         else:
             local_variables = {}
             for var_name, var in variables.items():
                 if re.match(r"^__\w+__$", var_name):
                     continue
                 if isinstance(var, (ModuleType, FunctionType)):
                     continue
-                local_variables[var_name] = var
+                local_variables[str(var_name)] = var
             return local_variables
 
     def mask_credentials(self, file_path: str) -> None:
         """A method to mask the credentials in the file.
 
         Args:
             file_path (str): The path of the file to be masked.
@@ -107,33 +91,26 @@
             filedata = f.readlines()
 
         config_path = Path(__file__).parent.resolve().as_posix() + "/resources/whispers_config.yml"
 
         args = f"-c {config_path} {file_path}"
 
         secrets = [secret for secret in whispers.secrets(args)]
-        unique_secrets = []
-        seen = set()
-        for secret in secrets:
-            item = (secret.key, secret.value, secret.line)
-            if item not in seen:
-                seen.add(item)
-                unique_secrets.append(secret)
 
         for index, line in enumerate(filedata):
-            if not unique_secrets:
+            if not secrets:
                 break
 
-            for secret in unique_secrets:
+            for secret in secrets:
                 if secret.key in line and secret.value in line:
                     filedata[index] = line.replace(secret.value, secret.value[:1] + "***")
-                    unique_secrets.pop(unique_secrets.index(secret))
+                    secrets.pop(secrets.index(secret))
                     break
 
-        if unique_secrets:
+        if secrets:
             logger.warning("Failed to mask credentials")
             os.remove(file_path)
             raise Exception("Failed to mask credentials")
 
         with open(file_path, "w") as file:
             file.writelines(filedata)
 
@@ -153,15 +130,15 @@
             while tb is not None:
                 frame = tb.tb_frame
                 if "site-packages" in frame.f_code.co_filename:
                     tb = tb.tb_next
                     continue
                 frames.append(frame)
                 tb = tb.tb_next
-            frames = frames[: CONFIG.LIMITS.STACK_SCOPE]
+            frames = frames[-CONFIG.LIMITS.STACK_SCOPE :]
 
             for frame in frames:
                 frame_info = {
                     "filename": self.strip_path(frame.f_code.co_filename),
                     "function_name": frame.f_code.co_name,
                     "locals": self.filter_variables(frame.f_locals),
                     "args": self.filter_variables(inspect.getargvalues(frame)[3]),
```

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher/utils/logger.py` & `t_bug_catcher-0.4.2/t_bug_catcher/utils/logger.py`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher.egg-info/PKG-INFO` & `t_bug_catcher-0.4.2/t_bug_catcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_bug_catcher
-Version: 0.4.1
+Version: 0.4.2
 Summary: Bug catcher
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_bug_catcher
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_bug_catcher-0.4.1/t_bug_catcher.egg-info/SOURCES.txt` & `t_bug_catcher-0.4.2/t_bug_catcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `t_bug_catcher-0.4.1/tests/test_t_bug_catcher.py` & `t_bug_catcher-0.4.2/tests/test_t_bug_catcher.py`

 * *Files identical despite different names*

