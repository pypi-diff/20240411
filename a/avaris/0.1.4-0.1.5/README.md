# Comparing `tmp/avaris-0.1.4.tar.gz` & `tmp/avaris-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avaris-0.1.4.tar", max compression
+gzip compressed data, was "avaris-0.1.5.tar", max compression
```

## Comparing `avaris-0.1.4.tar` & `avaris-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2024-04-10 12:46:19.234737 avaris-0.1.4/LICENSE
--rw-r--r--   0        0        0     4095 2024-04-10 12:46:19.234737 avaris-0.1.4/README.md
--rw-r--r--   0        0        0     1107 2024-04-10 12:46:19.238737 avaris-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      656 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/__init__.py
--rw-r--r--   0        0        0      187 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/__main__.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/__init__.py
--rw-r--r--   0        0        0     4112 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/models.py
--rw-r--r--   0        0        0      540 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/output.py
--rw-r--r--   0        0        0     3427 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/cli.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/__init__.py
--rw-r--r--   0        0        0     2051 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/config_loader.py
--rw-r--r--   0        0        0     2746 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/config_manager.py
--rw-r--r--   0        0        0      371 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/error.py
--rw-r--r--   0        0        0      961 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/exception.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/__init__.py
--rw-r--r--   0        0        0     1152 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/datamanager.py
--rw-r--r--   0        0        0      383 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/models.py
--rw-r--r--   0        0        0      341 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/s3.py
--rw-r--r--   0        0        0      197 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/shipper.py
--rw-r--r--   0        0        0     6676 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/sql.py
--rw-r--r--   0        0        0     2444 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/defaults.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/__init__.py
--rw-r--r--   0        0        0      114 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/commands.py
--rw-r--r--   0        0        0     4099 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/engine.py
--rw-r--r--   0        0        0      446 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/listener.py
--rw-r--r--   0        0        0     6900 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/start.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/__init__.py
--rw-r--r--   0        0        0      943 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/apicall.py
--rw-r--r--   0        0        0     1700 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/endpoint.py
--rw-r--r--   0        0        0     4023 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/executor.py
--rw-r--r--   0        0        0     2526 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/fetch_file.py
--rw-r--r--   0        0        0     2865 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/github_release.py
--rw-r--r--   0        0        0     1084 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/http_get_request.py
--rw-r--r--   0        0        0     1121 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/shell.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/handler/__init__.py
--rw-r--r--   0        0        0      688 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/handler/handler.py
--rw-r--r--   0        0        0      762 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/manage.py
--rw-r--r--   0        0        0      132 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/registry.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/__init__.py
--rw-r--r--   0        0        0      411 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/dataqueue.py
--rw-r--r--   0        0        0     6205 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/datasource.py
--rw-r--r--   0        0        0      312 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/service.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/__init__.py
--rw-r--r--   0        0        0     1073 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/plugins.py
--rw-r--r--   0        0        0      773 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/task_registry.py
--rw-r--r--   0        0        0     7105 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster.py
--rw-r--r--   0        0        0     3782 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster_apscheduler.py
--rw-r--r--   0        0        0     1346 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster_celery.py
--rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/utils/__init__.py
--rw-r--r--   0        0        0     1455 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/auth.py
--rw-r--r--   0        0        0     2188 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/logging.py
--rw-r--r--   0        0        0      529 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/management.py
--rw-r--r--   0        0        0     7339 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/parse.py
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 avaris-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 10:00:42.966962 avaris-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4095 2024-04-11 10:00:42.966962 avaris-0.1.5/README.md
+-rw-r--r--   0        0        0     1107 2024-04-11 10:00:42.970962 avaris-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/api/__init__.py
+-rw-r--r--   0        0        0     4112 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/api/models.py
+-rw-r--r--   0        0        0      540 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/api/output.py
+-rw-r--r--   0        0        0     3427 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/cli.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/config/__init__.py
+-rw-r--r--   0        0        0     2051 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/config/config_loader.py
+-rw-r--r--   0        0        0     2746 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/config/config_manager.py
+-rw-r--r--   0        0        0      371 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/config/error.py
+-rw-r--r--   0        0        0      961 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/config/exception.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/datamanager.py
+-rw-r--r--   0        0        0      383 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/models.py
+-rw-r--r--   0        0        0      341 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/s3.py
+-rw-r--r--   0        0        0      197 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/shipper.py
+-rw-r--r--   0        0        0     7665 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/data/sql.py
+-rw-r--r--   0        0        0     2444 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/engine/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/engine/commands.py
+-rw-r--r--   0        0        0     4099 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/engine/engine.py
+-rw-r--r--   0        0        0      446 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/engine/listener.py
+-rw-r--r--   0        0        0     6900 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/engine/start.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/apicall.py
+-rw-r--r--   0        0        0     1700 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/endpoint.py
+-rw-r--r--   0        0        0     4023 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/executor.py
+-rw-r--r--   0        0        0     2526 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/fetch_file.py
+-rw-r--r--   0        0        0     2865 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/github_release.py
+-rw-r--r--   0        0        0     1084 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/http_get_request.py
+-rw-r--r--   0        0        0     1121 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/executor/shell.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/handler/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/handler/handler.py
+-rw-r--r--   0        0        0      762 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/manage.py
+-rw-r--r--   0        0        0      132 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/registry.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/service/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/service/dataqueue.py
+-rw-r--r--   0        0        0     7031 2024-04-11 10:00:42.970962 avaris-0.1.5/src/avaris/service/datasource.py
+-rw-r--r--   0        0        0      312 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/plugins.py
+-rw-r--r--   0        0        0      773 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/task_registry.py
+-rw-r--r--   0        0        0     7105 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/taskmaster.py
+-rw-r--r--   0        0        0     3782 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/taskmaster_apscheduler.py
+-rw-r--r--   0        0        0     1346 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/task/taskmaster_celery.py
+-rw-r--r--   0        0        0        0 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/utils/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/utils/auth.py
+-rw-r--r--   0        0        0     2188 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/utils/logging.py
+-rw-r--r--   0        0        0      529 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/utils/management.py
+-rw-r--r--   0        0        0     7339 2024-04-11 10:00:42.974962 avaris-0.1.5/src/avaris/utils/parse.py
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 avaris-0.1.5/PKG-INFO
```

### Comparing `avaris-0.1.4/LICENSE` & `avaris-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/README.md` & `avaris-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/pyproject.toml` & `avaris-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "avaris"
-version = "0.1.4"
+version = "0.1.5"
 description = "Task execution engine for data management and monitoring"
 authors = ["dennis <denngohis@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{ include = "avaris", from = "src" }]
 
 [tool.poetry.scripts]
```

### Comparing `avaris-0.1.4/src/avaris/__init__.py` & `avaris-0.1.5/src/avaris/__init__.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/api/models.py` & `avaris-0.1.5/src/avaris/api/models.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/api/output.py` & `avaris-0.1.5/src/avaris/api/output.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/cli.py` & `avaris-0.1.5/src/avaris/cli.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/config/config_loader.py` & `avaris-0.1.5/src/avaris/config/config_loader.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/config/config_manager.py` & `avaris-0.1.5/src/avaris/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/config/exception.py` & `avaris-0.1.5/src/avaris/config/exception.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/data/datamanager.py` & `avaris-0.1.5/src/avaris/data/datamanager.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,19 @@
         self.logger = logger or get_logger()
 
     @abstractmethod
     async def add_task_result(self, execution_result: ExecutionResult) -> None:
         raise NotImplementedError()
 
     @abstractmethod
+    async def get_filtered_tasks(self, **kwargs):
+        raise NotImplementedError()
+
+
+    @abstractmethod
     async def get_task_result(self, job_id: str) -> ExecutionResult:
         raise NotImplementedError()
 
     @abstractmethod
     async def get_all_tasks(self) -> List[ExecutionResult]:
         raise NotImplementedError()
```

### Comparing `avaris-0.1.4/src/avaris/data/sql.py` & `avaris-0.1.5/src/avaris/data/sql.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from datetime import datetime
 from logging import Logger
 from typing import List, Optional
+from sqlalchemy import and_
 
 from sqlalchemy import update  # Ensure this is imported
 from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 from sqlalchemy.ext.asyncio import AsyncSession, create_async_engine
 from sqlalchemy.future import select
 from sqlalchemy.orm import sessionmaker
 
@@ -121,14 +122,38 @@
                 await session.commit()
             except SQLAlchemyError as e:
                 await session.rollback()  # Ensure to roll back on other SQL errors
                 self.logger.error(
                     f"Failed to add or update task result for {execution_result.task} in the SQL database: {e}"
                 )
 
+    async def get_filtered_tasks(self, **kwargs):
+        async with self.SessionLocal() as session:
+            query = select(SQLExecutionResult)
+
+            conditions = []
+            for key, value in kwargs.items():
+                if hasattr(SQLExecutionResult, key) and value is not None:
+                    # Use the '==' operator for most fields
+                    condition = getattr(SQLExecutionResult, key) == value
+
+                    # Special handling for date range queries
+                    if key == "start_date":
+                        condition = SQLExecutionResult.timestamp >= value
+                    elif key == "end_date":
+                        condition = SQLExecutionResult.timestamp <= value
+
+                    conditions.append(condition)
+
+            if conditions:
+                query = query.filter(and_(*conditions))
+
+            results = await session.execute(query)
+            return results.scalars().all()
+
     async def get_task_result(self, job_id: str):
         try:
             async with self.SessionLocal() as session:
                 query = select(SQLExecutionResult).filter(
                     SQLExecutionResult.id == job_id
                 )
                 result = await session.execute(query)
```

### Comparing `avaris-0.1.4/src/avaris/defaults.py` & `avaris-0.1.5/src/avaris/defaults.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/engine/engine.py` & `avaris-0.1.5/src/avaris/engine/engine.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/engine/start.py` & `avaris-0.1.5/src/avaris/engine/start.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/apicall.py` & `avaris-0.1.5/src/avaris/executor/apicall.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/endpoint.py` & `avaris-0.1.5/src/avaris/executor/endpoint.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/executor.py` & `avaris-0.1.5/src/avaris/executor/executor.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/fetch_file.py` & `avaris-0.1.5/src/avaris/executor/fetch_file.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/github_release.py` & `avaris-0.1.5/src/avaris/executor/github_release.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/http_get_request.py` & `avaris-0.1.5/src/avaris/executor/http_get_request.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/executor/shell.py` & `avaris-0.1.5/src/avaris/executor/shell.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/handler/handler.py` & `avaris-0.1.5/src/avaris/handler/handler.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/manage.py` & `avaris-0.1.5/src/avaris/manage.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/service/datasource.py` & `avaris-0.1.5/src/avaris/service/datasource.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from avaris.service.service import Service
 from fastapi import FastAPI, Request, HTTPException, Depends
 from uvicorn import Config, Server
 from avaris.data.datamanager import DataManager
 from avaris.utils.logging import get_logger
 import multiprocessing
 from typing import List
+from fastapi import Query
 from avaris.api.models import ExecutionResult, ListenerData
 from avaris.utils.parse import generate_task_id
 from avaris.utils.auth import validate_signature
 from avaris.defaults import Names
 import traceback
 class UvicornServer(multiprocessing.Process):
 
@@ -132,18 +133,34 @@
 
 
         @self.app.get("/health")
         async def health_check():
             return {"status": "ok"}
 
         @self.app.get("/tasks")
-        async def get_all_tasks():
-            tasks = await self.data_manager.get_all_tasks()
+        async def get_filtered_tasks(
+            id: str = Query(None, description="Filter tasks by ID"),
+            name: str = Query(None, description="Filter tasks by name"),
+            task: str = Query(None, description="Filter tasks by task type"),
+            start_date: datetime = Query(None, description="Start date for task filter (ISO 8601 format)"),
+            end_date: datetime = Query(None, description="End date for task filter (ISO 8601 format)"),
+        ):
+            # Prepare the filtering criteria as a dictionary
+            filter_criteria = {
+                "id": id,
+                "name": name,
+                "task": task,
+                "start_date": start_date,
+                "end_date": end_date
+            }
+            # Pass filtering criteria as keyword arguments
+            tasks = await self.data_manager.get_filtered_tasks(**filter_criteria)
             return tasks
 
+
     async def start(self) -> bool:
         # Runs Uvicorn server in the same asyncio event loop
         try:
             self.server.start()
             return True
         except Exception as e:
             self.logger.error(f"Error starting datasource Service: {e}")
```

### Comparing `avaris-0.1.4/src/avaris/task/plugins.py` & `avaris-0.1.5/src/avaris/task/plugins.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/task/task_registry.py` & `avaris-0.1.5/src/avaris/task/task_registry.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/task/taskmaster.py` & `avaris-0.1.5/src/avaris/task/taskmaster.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/task/taskmaster_apscheduler.py` & `avaris-0.1.5/src/avaris/task/taskmaster_apscheduler.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/task/taskmaster_celery.py` & `avaris-0.1.5/src/avaris/task/taskmaster_celery.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/utils/auth.py` & `avaris-0.1.5/src/avaris/utils/auth.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/utils/logging.py` & `avaris-0.1.5/src/avaris/utils/logging.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/utils/management.py` & `avaris-0.1.5/src/avaris/utils/management.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/src/avaris/utils/parse.py` & `avaris-0.1.5/src/avaris/utils/parse.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.4/PKG-INFO` & `avaris-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avaris
-Version: 0.1.4
+Version: 0.1.5
 Summary: Task execution engine for data management and monitoring
 License: Apache-2.0
 Author: dennis
 Author-email: denngohis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

