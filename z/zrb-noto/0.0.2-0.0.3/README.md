# Comparing `tmp/zrb_noto-0.0.2.tar.gz` & `tmp/zrb_noto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb_noto-0.0.2.tar", max compression
+gzip compressed data, was "zrb_noto-0.0.3.tar", max compression
```

## Comparing `zrb_noto-0.0.2.tar` & `zrb_noto-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1165 2024-04-10 08:47:58.462827 zrb_noto-0.0.2/README.md
--rw-r--r--   0        0        0      749 2024-04-10 10:17:38.611185 zrb_noto-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      758 2024-04-10 08:47:58.532853 zrb_noto-0.0.2/src/zrb_noto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 08:47:58.542857 zrb_noto-0.0.2/src/zrb_noto/__main__.py
--rw-r--r--   0        0        0     1039 2024-04-10 08:47:58.542857 zrb_noto-0.0.2/src/zrb_noto/_config.py
--rw-r--r--   0        0        0      242 2024-04-10 08:47:58.562864 zrb_noto-0.0.2/src/zrb_noto/_env.py
--rw-r--r--   0        0        0      148 2024-04-10 08:47:58.592875 zrb_noto-0.0.2/src/zrb_noto/_group.py
--rw-r--r--   0        0        0      127 2024-04-10 08:47:58.632890 zrb_noto-0.0.2/src/zrb_noto/_helper.py
--rw-r--r--   0        0        0      419 2024-04-10 09:53:23.092906 zrb_noto-0.0.2/src/zrb_noto/lint.py
--rw-r--r--   0        0        0       45 2024-04-10 08:47:58.712920 zrb_noto-0.0.2/src/zrb_noto/lint.sh
--rw-r--r--   0        0        0      666 2024-04-10 08:47:58.552861 zrb_noto-0.0.2/src/zrb_noto/list.py
--rw-r--r--   0        0        0      141 2024-04-10 08:47:58.602879 zrb_noto-0.0.2/src/zrb_noto/log/__init__.py
--rw-r--r--   0        0        0       86 2024-04-10 08:47:58.612883 zrb_noto-0.0.2/src/zrb_noto/log/_group.py
--rw-r--r--   0        0        0     2207 2024-04-10 08:47:58.622887 zrb_noto-0.0.2/src/zrb_noto/log/_helper.py
--rw-r--r--   0        0        0      955 2024-04-10 08:47:58.622887 zrb_noto-0.0.2/src/zrb_noto/log/add.py
--rw-r--r--   0        0        0      887 2024-04-10 08:47:58.602879 zrb_noto-0.0.2/src/zrb_noto/log/list.py
--rw-r--r--   0        0        0      975 2024-04-10 09:53:23.092906 zrb_noto-0.0.2/src/zrb_noto/sync.py
--rw-r--r--   0        0        0     1472 2024-04-10 08:47:58.712920 zrb_noto-0.0.2/src/zrb_noto/sync.sh
--rw-r--r--   0        0        0      489 2024-04-10 08:47:58.642894 zrb_noto-0.0.2/src/zrb_noto/todo/__init__.py
--rw-r--r--   0        0        0    10420 2024-04-10 09:50:20.597518 zrb_noto-0.0.2/src/zrb_noto/todo/_data.py
--rw-r--r--   0        0        0       81 2024-04-10 08:47:58.692912 zrb_noto-0.0.2/src/zrb_noto/todo/_group.py
--rw-r--r--   0        0        0     6130 2024-04-10 08:47:58.692912 zrb_noto-0.0.2/src/zrb_noto/todo/_helper.py
--rw-r--r--   0        0        0     1204 2024-04-10 08:47:58.642894 zrb_noto-0.0.2/src/zrb_noto/todo/_input.py
--rw-r--r--   0        0        0     2698 2024-04-10 08:47:58.702916 zrb_noto-0.0.2/src/zrb_noto/todo/add.py
--rw-r--r--   0        0        0     1684 2024-04-10 08:47:58.702916 zrb_noto-0.0.2/src/zrb_noto/todo/complete.py
--rw-r--r--   0        0        0     1467 2024-04-10 08:47:58.702916 zrb_noto-0.0.2/src/zrb_noto/todo/delete.py
--rw-r--r--   0        0        0     3205 2024-04-10 08:47:58.692912 zrb_noto-0.0.2/src/zrb_noto/todo/edit.py
--rw-r--r--   0        0        0     1150 2024-04-10 08:47:58.652897 zrb_noto-0.0.2/src/zrb_noto/todo/find.py
--rw-r--r--   0        0        0       52 2024-04-10 08:47:58.662901 zrb_noto-0.0.2/src/zrb_noto/todo/kanban/__init__.py
--rw-r--r--   0        0        0     3759 2024-04-10 08:47:58.672905 zrb_noto-0.0.2/src/zrb_noto/todo/kanban/_helper.py
--rw-r--r--   0        0        0      621 2024-04-10 08:47:58.662901 zrb_noto-0.0.2/src/zrb_noto/todo/kanban/kanban.py
--rw-r--r--   0        0        0      524 2024-04-10 08:47:58.682909 zrb_noto-0.0.2/src/zrb_noto/todo/list.py
--rw-r--r--   0        0        0     1650 2024-04-10 08:47:58.672905 zrb_noto-0.0.2/src/zrb_noto/todo/start.py
--rw-r--r--   0        0        0     1667 2024-04-10 08:47:58.682909 zrb_noto-0.0.2/src/zrb_noto/todo/stop.py
--rw-r--r--   0        0        0      341 2024-04-10 08:47:58.572868 zrb_noto-0.0.2/src/zrb_noto/wiki.py
--rw-r--r--   0        0        0     1937 1970-01-01 00:00:00.000000 zrb_noto-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1165 2024-04-11 12:19:34.722909 zrb_noto-0.0.3/README.md
+-rw-r--r--   0        0        0      755 2024-04-11 12:19:34.742909 zrb_noto-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      758 2024-04-11 12:19:34.762909 zrb_noto-0.0.3/src/zrb_noto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 12:19:34.772909 zrb_noto-0.0.3/src/zrb_noto/__main__.py
+-rw-r--r--   0        0        0     1039 2024-04-11 12:19:34.762909 zrb_noto-0.0.3/src/zrb_noto/_config.py
+-rw-r--r--   0        0        0      242 2024-04-11 12:19:34.782909 zrb_noto-0.0.3/src/zrb_noto/_env.py
+-rw-r--r--   0        0        0      148 2024-04-11 12:19:34.792909 zrb_noto-0.0.3/src/zrb_noto/_group.py
+-rw-r--r--   0        0        0      127 2024-04-11 12:19:34.802909 zrb_noto-0.0.3/src/zrb_noto/_helper.py
+-rw-r--r--   0        0        0      419 2024-04-11 12:19:34.782909 zrb_noto-0.0.3/src/zrb_noto/lint.py
+-rw-r--r--   0        0        0       45 2024-04-11 12:19:34.842909 zrb_noto-0.0.3/src/zrb_noto/lint.sh
+-rw-r--r--   0        0        0      666 2024-04-11 12:19:34.772909 zrb_noto-0.0.3/src/zrb_noto/list.py
+-rw-r--r--   0        0        0      141 2024-04-11 12:19:34.792909 zrb_noto-0.0.3/src/zrb_noto/log/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-11 12:19:34.792909 zrb_noto-0.0.3/src/zrb_noto/log/_group.py
+-rw-r--r--   0        0        0     2207 2024-04-11 12:19:34.802909 zrb_noto-0.0.3/src/zrb_noto/log/_helper.py
+-rw-r--r--   0        0        0      955 2024-04-11 12:19:34.802909 zrb_noto-0.0.3/src/zrb_noto/log/add.py
+-rw-r--r--   0        0        0      887 2024-04-11 12:19:34.792909 zrb_noto-0.0.3/src/zrb_noto/log/list.py
+-rw-r--r--   0        0        0     1509 2024-04-11 12:19:34.782909 zrb_noto-0.0.3/src/zrb_noto/sync.py
+-rw-r--r--   0        0        0     1609 2024-04-11 12:19:34.842909 zrb_noto-0.0.3/src/zrb_noto/sync.sh
+-rw-r--r--   0        0        0      489 2024-04-11 12:19:34.802909 zrb_noto-0.0.3/src/zrb_noto/todo/__init__.py
+-rw-r--r--   0        0        0    10420 2024-04-11 12:19:34.842909 zrb_noto-0.0.3/src/zrb_noto/todo/_data.py
+-rw-r--r--   0        0        0       81 2024-04-11 12:19:34.822909 zrb_noto-0.0.3/src/zrb_noto/todo/_group.py
+-rw-r--r--   0        0        0     6130 2024-04-11 12:19:34.832909 zrb_noto-0.0.3/src/zrb_noto/todo/_helper.py
+-rw-r--r--   0        0        0     1204 2024-04-11 12:19:34.812909 zrb_noto-0.0.3/src/zrb_noto/todo/_input.py
+-rw-r--r--   0        0        0     2698 2024-04-11 12:19:34.832909 zrb_noto-0.0.3/src/zrb_noto/todo/add.py
+-rw-r--r--   0        0        0     1684 2024-04-11 12:19:34.832909 zrb_noto-0.0.3/src/zrb_noto/todo/complete.py
+-rw-r--r--   0        0        0     1467 2024-04-11 12:19:34.832909 zrb_noto-0.0.3/src/zrb_noto/todo/delete.py
+-rw-r--r--   0        0        0     3205 2024-04-11 12:19:34.832909 zrb_noto-0.0.3/src/zrb_noto/todo/edit.py
+-rw-r--r--   0        0        0     1150 2024-04-11 12:19:34.812909 zrb_noto-0.0.3/src/zrb_noto/todo/find.py
+-rw-r--r--   0        0        0       52 2024-04-11 12:19:34.812909 zrb_noto-0.0.3/src/zrb_noto/todo/kanban/__init__.py
+-rw-r--r--   0        0        0     3759 2024-04-11 12:19:34.822909 zrb_noto-0.0.3/src/zrb_noto/todo/kanban/_helper.py
+-rw-r--r--   0        0        0      621 2024-04-11 12:19:34.812909 zrb_noto-0.0.3/src/zrb_noto/todo/kanban/kanban.py
+-rw-r--r--   0        0        0      524 2024-04-11 12:19:34.822909 zrb_noto-0.0.3/src/zrb_noto/todo/list.py
+-rw-r--r--   0        0        0     1650 2024-04-11 12:19:34.822909 zrb_noto-0.0.3/src/zrb_noto/todo/start.py
+-rw-r--r--   0        0        0     1667 2024-04-11 12:19:34.822909 zrb_noto-0.0.3/src/zrb_noto/todo/stop.py
+-rw-r--r--   0        0        0      341 2024-04-11 12:19:34.782909 zrb_noto-0.0.3/src/zrb_noto/wiki.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 zrb_noto-0.0.3/PKG-INFO
```

### Comparing `zrb_noto-0.0.2/README.md` & `zrb_noto-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/pyproject.toml` & `zrb_noto-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "zrb-noto"
-version = "0.0.2"
+version = "0.0.3"
 description = "Personal todo and logging management"
 authors = ["Go Frendi Gunawan <gofrendiasgard@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
-homepage = "https://github.com/goFrendiAsgard/noto"
-repository = "https://github.com/goFrendiAsgard/noto"
-documentation = "https://github.com/goFrendiAsgard/noto"
+homepage = "https://github.com/state-alchemists/noto"
+repository = "https://github.com/state-alchemists/noto"
+documentation = "https://github.com/state-alchemists/noto"
 keywords = []
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<4.0.0"
 zrb = ">=0.12.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `zrb_noto-0.0.2/src/zrb_noto/__init__.py` & `zrb_noto-0.0.3/src/zrb_noto/__init__.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/_config.py` & `zrb_noto-0.0.3/src/zrb_noto/_config.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/list.py` & `zrb_noto-0.0.3/src/zrb_noto/list.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/log/_helper.py` & `zrb_noto-0.0.3/src/zrb_noto/log/_helper.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/log/add.py` & `zrb_noto-0.0.3/src/zrb_noto/log/add.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/log/list.py` & `zrb_noto-0.0.3/src/zrb_noto/log/list.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/sync.py` & `zrb_noto-0.0.3/src/zrb_noto/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,57 @@
 import os
 from typing import List, Optional
 
-from zrb import CmdTask, Env, Group, Task, runner
+from zrb import CmdTask, Env, Group, StrInput, Task, runner
 
 from ._env import LOCAL_REPO_DIR_ENV, REMOTE_GIT_URL_ENV
 from ._group import noto_group
 
 _CURRENT_DIR = os.path.dirname(__file__)
 
 
 def create_sync_noto_task(
     group: Optional[Group] = None,
     retry: int = 0,
     ignore_error: bool = True,
     upstreams: List[Task] = [],
+    custom_commit_message: bool = False,
 ) -> Task:
     sync_noto = CmdTask(
         name="sync",
         group=group,
         description="Sync noto",
         upstreams=upstreams,
         envs=[
             LOCAL_REPO_DIR_ENV,
             REMOTE_GIT_URL_ENV,
-            Env(name="IGNORE_ERROR", os_name="", default="1" if ignore_error else "0"),
+            Env(
+                name="IGNORE_ERROR",
+                os_name="",
+                default="1" if ignore_error else "0"
+            ),
+            Env(
+                name="COMMIT_MESSAGE",
+                os_name="",
+                default="{{input.commit_message}}"
+            ),
         ],
         retry=retry,
         cmd_path=os.path.join(_CURRENT_DIR, "sync.sh"),
         should_show_cmd=False,
         should_print_cmd_result=False,
     )
+    if custom_commit_message:
+        sync_noto.add_input(
+            StrInput(
+                name="commit-message",
+                prompt="Commit message, if any (can be empty)",
+                default="",
+            ),
+        )
     return sync_noto
 
 
-sync_noto = create_sync_noto_task(group=noto_group, ignore_error=False, retry=2)
+sync_noto = create_sync_noto_task(
+    group=noto_group, ignore_error=False, custom_commit_message=True, retry=2
+)
 runner.register(sync_noto)
```

### Comparing `zrb_noto-0.0.2/src/zrb_noto/sync.sh` & `zrb_noto-0.0.3/src/zrb_noto/sync.sh`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 cd "${LOCAL_REPO_DIR}"
 git add . -A
 if git diff --quiet && git diff --cached --quiet
 then
     echo "Nothing to commit"
 else
     echo "Commiting changes"
-    git commit -m "Save changes on $(date)"
+    if [ -z "${COMMIT_MESSAGE}" ]
+    then
+        COMMIT_MESSAGE="Modified on $(date)"
+    fi
+    echo "Commiting changes: ${COMMIT_MESSAGE}"
+    git commit -m "${COMMIT_MESSAGE}"
 fi
 GIT_BRANCH="$(git symbolic-ref --short HEAD)"
 echo "Current branch: ${GIT_BRANCH}"
 
 echo "Fetching origin ${GIT_BRANCH}"
 git fetch origin
```

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/_data.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/_data.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/_helper.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/_helper.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/_input.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/_input.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/add.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/add.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/complete.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/complete.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/delete.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/delete.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/edit.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/edit.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/find.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/find.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/kanban/_helper.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/kanban/_helper.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/kanban/kanban.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/kanban/kanban.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/list.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/list.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/start.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/start.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/src/zrb_noto/todo/stop.py` & `zrb_noto-0.0.3/src/zrb_noto/todo/stop.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.2/PKG-INFO` & `zrb_noto-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: zrb-noto
-Version: 0.0.2
+Version: 0.0.3
 Summary: Personal todo and logging management
-Home-page: https://github.com/goFrendiAsgard/noto
+Home-page: https://github.com/state-alchemists/noto
 License: AGPL-3.0-or-later
 Author: Go Frendi Gunawan
 Author-email: gofrendiasgard@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: zrb (>=0.12.0)
-Project-URL: Documentation, https://github.com/goFrendiAsgard/noto
-Project-URL: Repository, https://github.com/goFrendiAsgard/noto
+Project-URL: Documentation, https://github.com/state-alchemists/noto
+Project-URL: Repository, https://github.com/state-alchemists/noto
 Description-Content-Type: text/markdown
 
 # Noto
 
 Noto is a personal management tool based on [Zrb](https://pypi.org/project/zrb) and [todo.txt](https://github.com/todotxt/todo.txt).
 
 # Installing Noto
```

