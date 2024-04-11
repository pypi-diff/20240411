# Comparing `tmp/ryax-0.0.2.tar.gz` & `tmp/ryax-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryax-0.0.2.tar", max compression
+gzip compressed data, was "ryax-0.0.3.tar", max compression
```

## Comparing `ryax-0.0.2.tar` & `ryax-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0    16725 2023-10-12 15:25:59.624179 ryax-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0       52 2023-10-09 15:41:03.902022 ryax-0.0.2/README.md
--rw-r--r--   0        0        0      609 2023-10-26 14:18:34.853886 ryax-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-09 15:45:09.192708 ryax-0.0.2/ryax/__init__.py
--rw-r--r--   0        0        0       50 2023-10-12 15:46:44.060437 ryax-0.0.2/ryax/command_line.py
--rw-r--r--   0        0        0       42 2023-10-12 15:32:07.321851 ryax-0.0.2/ryax/triggers/__init__.py
--rw-r--r--   0        0        0      708 2023-10-09 15:59:12.581917 ryax-0.0.2/ryax/triggers/protocols.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 ryax-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-10-12 15:25:59.624179 ryax-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0       52 2023-10-09 15:41:03.902022 ryax-0.0.3/README.md
+-rw-r--r--   0        0        0     1002 2024-04-11 14:26:13.621266 ryax-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-11-02 11:25:08.803612 ryax-0.0.3/ryax/__init__.py
+-rw-r--r--   0        0        0     2321 2024-04-11 14:26:41.159619 ryax-0.0.3/ryax/command_line.py
+-rw-r--r--   0        0        0        0 2024-04-09 14:52:13.678649 ryax-0.0.3/ryax/ryax_metadata/__init__.py
+-rw-r--r--   0        0        0    13543 2024-04-11 14:13:03.377970 ryax-0.0.3/ryax/ryax_metadata/entities.py
+-rw-r--r--   0        0        0    15465 2024-04-11 14:26:41.271611 ryax-0.0.3/ryax/ryax_metadata/ryax_metadata.py
+-rw-r--r--   0        0        0        0 2023-11-02 11:25:08.804219 ryax-0.0.3/ryax/triggers/__init__.py
+-rw-r--r--   0        0        0      710 2023-11-02 11:25:08.804802 ryax-0.0.3/ryax/triggers/protocols.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:44:49.495676 ryax-0.0.3/ryax/utils/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-11 12:20:37.518759 ryax-0.0.3/ryax/utils/check.py
+-rw-r--r--   0        0        0     3645 2024-04-11 13:57:08.177820 ryax-0.0.3/ryax/utils/exceptions.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ryax-0.0.3/PKG-INFO
```

### Comparing `ryax-0.0.2/LICENSE.txt` & `ryax-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ryax-0.0.2/ryax/triggers/protocols.py` & `ryax-0.0.3/ryax/triggers/protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Copyright 2022 Ryax Technologies
 # Use of this trigger code is governed by a BSD-style
 # license that can be found in the LICENSE file.
 import abc
 from enum import Enum
 from typing import Any, Dict
 
+
 class RyaxRunStatus(Enum):
     DONE = 1
     ERROR = 2
 
+
 class RyaxTriggerProtocol(metaclass=abc.ABCMeta):
     async def create_run_error(self) -> None:
         await self.create_run({}, status=RyaxRunStatus.ERROR)
 
     @abc.abstractmethod
     async def create_run(
         self,
```

