# Comparing `tmp/ocxtools-1.4.0.tar.gz` & `tmp/ocxtools-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocxtools-1.4.0.tar", max compression
+gzip compressed data, was "ocxtools-1.5.1.tar", max compression
```

## Comparing `ocxtools-1.4.0.tar` & `ocxtools-1.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1066 2024-03-11 13:43:17.634488 ocxtools-1.4.0/LICENSE
--rw-r--r--   0        0        0     2202 2024-03-11 13:43:17.634488 ocxtools-1.4.0/README.md
--rw-r--r--   0        0        0      158 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/__init__.py
--rw-r--r--   0        0        0     5969 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/cli.py
--rw-r--r--   0        0        0     1432 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/cli_plugin.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/clients/__init__.py
--rw-r--r--   0        0        0    15845 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/clients/clients.py
--rw-r--r--   0        0        0     2068 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/config.py
--rw-r--r--   0        0        0      106 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/console/__init__.py
--rw-r--r--   0        0        0     4907 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/console/console.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/context/__init__.py
--rw-r--r--   0        0        0     2908 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/context/context_manager.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/converter/__init__.py
--rw-r--r--   0        0        0     8781 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/converter/converter.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/dataclass/__init__.py
--rw-r--r--   0        0        0    14494 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/dataclass/dataclasses.py
--rw-r--r--   0        0        0    10871 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/docker/README.md
--rw-r--r--   0        0        0      130 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/docker/__init__.py
--rw-r--r--   0        0        0     4255 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/docker/cli.py
--rw-r--r--   0        0        0      433 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/exceptions.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/interfaces/__init__.py
--rw-r--r--   0        0        0     3691 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/interfaces/interfaces.py
--rw-r--r--   0        0        0       99 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/jupyter/__init__.py
--rw-r--r--   0        0        0     3543 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/jupyter/cli.py
--rw-r--r--   0        0        0     5175 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/jupyter/readme.md
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/loader/__init__.py
--rw-r--r--   0        0        0     4624 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/loader/loader.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/parser/__init__.py
--rw-r--r--   0        0        0    10137 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/parser/parser.py
--rw-r--r--   0        0        0       94 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/rds/__init__.py
--rw-r--r--   0        0        0     7898 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/rds/cli.py
--rw-r--r--   0        0        0      119 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/renderer/__init__.py
--rw-r--r--   0        0        0     2193 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/renderer/cli.py
--rw-r--r--   0        0        0     6924 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/renderer/renderer.py
--rw-r--r--   0        0        0      102 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/reporter/__init__.py
--rw-r--r--   0        0        0    11042 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/reporter/cli.py
--rw-r--r--   0        0        0     3922 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/reporter/report_manager.py
--rw-r--r--   0        0        0    16294 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/reporter/reporter.py
--rw-r--r--   0        0        0      100 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/serializer/__init__.py
--rw-r--r--   0        0        0     2511 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/serializer/cli.py
--rw-r--r--   0        0        0    12060 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/serializer/resource/gitb_trl_stylesheet_v1.0.xsl
--rw-r--r--   0        0        0     4173 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/serializer/serializer.py
--rw-r--r--   0        0        0       73 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/utils/__init__.py
--rw-r--r--   0        0        0     9847 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/utils/utilities.py
--rw-r--r--   0        0        0       99 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/validator/__init__.py
--rw-r--r--   0        0        0    13035 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/validator/cli.py
--rw-r--r--   0        0        0    22004 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/validator/validator_client.py
--rw-r--r--   0        0        0     5427 2024-03-11 13:43:17.702488 ocxtools-1.4.0/ocxtools/validator/validator_report.py
--rw-r--r--   0        0        0     3135 2024-03-11 13:43:17.702488 ocxtools-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 ocxtools-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-11 13:59:32.261931 ocxtools-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2202 2024-04-11 13:59:32.261931 ocxtools-1.5.1/README.md
+-rw-r--r--   0        0        0      158 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/__init__.py
+-rw-r--r--   0        0        0     5970 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/cli.py
+-rw-r--r--   0        0        0     1433 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/cli_plugin.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/clients/__init__.py
+-rw-r--r--   0        0        0    15843 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/clients/clients.py
+-rw-r--r--   0        0        0     2069 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/config.py
+-rw-r--r--   0        0        0      106 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/console/__init__.py
+-rw-r--r--   0        0        0     4909 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/console/console.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/context/__init__.py
+-rw-r--r--   0        0        0     3335 2024-04-11 13:59:32.273931 ocxtools-1.5.1/ocxtools/context/context_manager.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/converter/__init__.py
+-rw-r--r--   0        0        0     8817 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/converter/converter.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/dataclass/__init__.py
+-rw-r--r--   0        0        0    14494 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/dataclass/dataclasses.py
+-rw-r--r--   0        0        0    10871 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/docker/README.md
+-rw-r--r--   0        0        0      130 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/docker/__init__.py
+-rw-r--r--   0        0        0     4255 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/docker/cli.py
+-rw-r--r--   0        0        0      433 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/interfaces/__init__.py
+-rw-r--r--   0        0        0     3692 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/interfaces/interfaces.py
+-rw-r--r--   0        0        0       99 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/jupyter/__init__.py
+-rw-r--r--   0        0        0     3520 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/jupyter/cli.py
+-rw-r--r--   0        0        0     5175 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/jupyter/readme.md
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/loader/__init__.py
+-rw-r--r--   0        0        0     4624 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/loader/loader.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/parser/__init__.py
+-rw-r--r--   0        0        0    10182 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/parser/parser.py
+-rw-r--r--   0        0        0       94 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/rds/__init__.py
+-rw-r--r--   0        0        0     7944 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/rds/cli.py
+-rw-r--r--   0        0        0      119 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/renderer/__init__.py
+-rw-r--r--   0        0        0     2195 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/renderer/cli.py
+-rw-r--r--   0        0        0     6925 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/renderer/renderer.py
+-rw-r--r--   0        0        0      102 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/reporter/__init__.py
+-rw-r--r--   0        0        0    11325 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/reporter/cli.py
+-rw-r--r--   0        0        0     3921 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/reporter/report_manager.py
+-rw-r--r--   0        0        0    16392 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/reporter/reporter.py
+-rw-r--r--   0        0        0      100 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/serializer/__init__.py
+-rw-r--r--   0        0        0     2510 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/serializer/cli.py
+-rw-r--r--   0        0        0    12060 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/serializer/resource/gitb_trl_stylesheet_v1.0.xsl
+-rw-r--r--   0        0        0     4175 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/serializer/serializer.py
+-rw-r--r--   0        0        0       73 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/utils/__init__.py
+-rw-r--r--   0        0        0     9830 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/utils/utilities.py
+-rw-r--r--   0        0        0       99 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/validator/__init__.py
+-rw-r--r--   0        0        0    13169 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/validator/cli.py
+-rw-r--r--   0        0        0    22065 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/validator/validator_client.py
+-rw-r--r--   0        0        0     5520 2024-04-11 13:59:32.277931 ocxtools-1.5.1/ocxtools/validator/validator_report.py
+-rw-r--r--   0        0        0     3135 2024-04-11 13:59:32.277931 ocxtools-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3129 1970-01-01 00:00:00.000000 ocxtools-1.5.1/PKG-INFO
```

### Comparing `ocxtools-1.4.0/LICENSE` & `ocxtools-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ocxtools-1.4.0/README.md` & `ocxtools-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ocxtools-1.4.0/ocxtools/cli.py` & `ocxtools-1.5.1/ocxtools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """generator CLI commands."""
 
 # System imports
 from __future__ import annotations
+
 import logging
 import warnings
+
+import typer
 # Third party
 from click import pass_context
 from click_shell import shell
-import typer
 from loguru import logger
 
-# Project imports
-from ocxtools import __app_name__, __version__
-import ocxtools.serializer.cli
-import ocxtools.validator.cli
 import ocxtools.docker.cli
-import ocxtools.reporter.cli
-import ocxtools.renderer.cli
 import ocxtools.jupyter.cli
+import ocxtools.renderer.cli
+import ocxtools.reporter.cli
+import ocxtools.serializer.cli
+import ocxtools.validator.cli
+# Project imports
+from ocxtools import __app_name__, __version__
+from ocxtools.config import config
 from ocxtools.console.console import CliConsole
 from ocxtools.context.context_manager import ContextManager
-from ocxtools.config import config
-
 
 LOG_FILE = config.get('FileLogger', 'log_file')
 RETENTION = config.get('FileLogger', 'retention')
 ROTATION = config.get('FileLogger', 'rotation')
 SINK_LEVEL = config.get('FileLogger', 'level')
 if DEBUG := config.getboolean('Defaults', 'debug'):
     SINK_LEVEL = 'DEBUG'
```

### Comparing `ocxtools-1.4.0/ocxtools/cli_plugin.py` & `ocxtools-1.5.1/ocxtools/cli_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """CLI plugin method"""
-from typing import Tuple, Any, List
+from typing import Any, List, Tuple
+
 import typer
 from typer import Typer
 
 # Project imports
 from ocxtools.loader.loader import DynamicLoader, ModuleDeclaration
```

### Comparing `ocxtools-1.4.0/ocxtools/clients/clients.py` & `ocxtools-1.5.1/ocxtools/clients/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Module for server clients."""
 
-# System reports
-import httpx
 import json
 from abc import ABC, abstractmethod
 from enum import Enum
 from io import BytesIO
 from typing import Any, Coroutine, Dict, List, Tuple, Union
 
+# System reports
+import httpx
 import pycurl
 import requests
-
 # Third party
 from loguru import logger
 from pycurl import error as pycurl_error
 
-
 # Project imports
 
 
 class RequestClientError(requests.RequestException):
     """Request client errors."""
```

### Comparing `ocxtools-1.4.0/ocxtools/config.py` & `ocxtools-1.5.1/ocxtools/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,14 @@
 }
 
 config["StdoutLogger"] = {
     "level": 'INFO',
 }
 # Plugins to include
 config["Plugins"] = {
-    "serializer": 'no',
+    "serializer": 'yes',
     "validator": 'yes',
-    "reporter": 'yes',
+    "reporter": 'no',
     "docker": 'yes',
     "renderer": 'no',
-    "jupyter": 'no'
+    "jupyter": 'yes'
 }
```

### Comparing `ocxtools-1.4.0/ocxtools/console/console.py` & `ocxtools-1.5.1/ocxtools/console/console.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """CLI console"""
 
 # System imports
 
 
-from enum import Enum
-from typing import List, Union
 import subprocess
+from enum import Enum
 from pathlib import Path
+from typing import List, Union
+
+from loguru import logger
 # Third party imports
 from rich.console import Console
+from rich.markdown import Markdown
+from rich.style import Style
 from rich.table import Table
 from rich.theme import Theme
-from rich.style import Style
-from rich.markdown import Markdown
-from loguru import logger
+
+from ocxtools import config
 # Project imports
 from ocxtools.utils.utilities import get_file_path
-from ocxtools import config
 
 # # Defaults
 README_FOLDER = config.get("Defaults", "readme_folder")
 
 console = Console()
 
 # Styling
```

### Comparing `ocxtools-1.4.0/ocxtools/context/context_manager.py` & `ocxtools-1.5.1/ocxtools/context/context_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Provide context information between sub-commands."""
 
+from configparser import ConfigParser
 # System imports
-from typing import Union, Dict
+from typing import Dict, Union
+
 # Third party imports
 import click
-from configparser import ConfigParser
+
 # Project
 from ocxtools.console.console import CliConsole
-from ocxtools.dataclass.dataclasses import ValidationReport, OcxHeader
+from ocxtools.dataclass.dataclasses import OcxHeader, ValidationReport
+from ocxtools.reporter.report_manager import OcxReportManager
 from ocxtools.validator.validator_client import ValidationDomain
 
 
 class ContextManager:
     """
     Provide context between sub commands.
 
@@ -24,14 +27,15 @@
 
     def __init__(self, console: CliConsole, config: ConfigParser):
         self._ocx_reports: Dict = {}
         self._schematron_reports: Dict = {}
         self._console = console
         self._config = config
         self._headers: Dict = {}
+        self._report_manager = OcxReportManager()
 
     def add_header(self, header: OcxHeader):
         """
             Add the 3Docx header information.
         Args:
             header: The header dataclass
 
@@ -65,14 +69,23 @@
 
         """
         if model in self._ocx_reports:
             return self._ocx_reports.get(model)
         else:
             return self._schematron_reports.get(model)
 
+    def get_report_manager(self) -> OcxReportManager:
+        """
+        Returns the OcxReportManager instance associated with the context manager.
+
+        Returns:
+            OcxReportManager: The OcxReportManager instance associated with the context manager.
+        """
+        return self._report_manager
+
     def get_ocx_reports(self) -> Dict:
         """
             List of OCX validation reports
         Returns:
             List of reports
 
         """
```

### Comparing `ocxtools-1.4.0/ocxtools/converter/converter.py` & `ocxtools-1.5.1/ocxtools/converter/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 client from the conversion rules. """
 # System imports
 from abc import ABC
 from enum import Enum
 from typing import Dict, List
 
 import packaging.version
-
 # Third party imports
 from loguru import logger
 
 from ocxtools.exceptions import ConverterError, ConverterWarning
 from ocxtools.interfaces.interfaces import IObservable, IObserver, IRule
-
 # Project imports
-from ocxtools.loader.loader import DeclarationOfOcxImport, DynamicLoader, DynamicLoaderError
+from ocxtools.loader.loader import (DeclarationOfOcxImport, DynamicLoader,
+                                    DynamicLoaderError)
 from ocxtools.utils.utilities import all_equal
 
 
 class RuleType(Enum):
     """
     Rule type enumeration.
```

### Comparing `ocxtools-1.4.0/ocxtools/dataclass/dataclasses.py` & `ocxtools-1.5.1/ocxtools/dataclass/dataclasses.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #  Copyright (c) 2023-2024. OCX Consortium https://3docx.org. See the LICENSE
 """The validation data dataclasses."""
 
+from abc import ABC
+from collections import defaultdict
 # System imports
 from dataclasses import dataclass, field, fields
 from enum import Enum
 from typing import Dict, List, Union
-from abc import ABC
-import pandas as pd
-from collections import defaultdict
 
+import pandas as pd
 # Third party imports
 from xsdata.utils.text import snake_case
 
 # Project imports
 from ocxtools.exceptions import ReporterError
```

### Comparing `ocxtools-1.4.0/ocxtools/docker/README.md` & `ocxtools-1.5.1/ocxtools/docker/README.md`

 * *Files identical despite different names*

### Comparing `ocxtools-1.4.0/ocxtools/docker/cli.py` & `ocxtools-1.5.1/ocxtools/docker/cli.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Docker CLI."""
 # System imports
-from typing import Any, Tuple
-from typing_extensions import Annotated
-from pathlib import Path
 import re
+from pathlib import Path
+from typing import Any, Tuple
+
 # 3rd party imports
 import typer
+from typing_extensions import Annotated
 
 # Project imports
 from ocxtools import config
 from ocxtools.context.context_manager import get_context_manager
 from ocxtools.docker import __app_name__
 
-
 # Docker
 DOCKER_DESKTOP = config.get("DockerSettings", "docker_desktop")
 
 docker = typer.Typer(help="Commands for managing the docker OCX validator.")
 
 
 def extract_jupyter_url_with_token(log_content: str, server_location: str) -> str:
```

### Comparing `ocxtools-1.4.0/ocxtools/interfaces/interfaces.py` & `ocxtools-1.5.1/ocxtools/interfaces/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Interfaces module."""
 
 # System imports
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from enum import Enum
 from typing import Dict, Iterator, List
+
 import packaging.version
-from enum import Enum
 
 # Project imports
 from ocxtools.exceptions import ConverterError
 
 
 class ObservableEvent(Enum):
     """Events that can be listened to and broadcast."""
```

### Comparing `ocxtools-1.4.0/ocxtools/jupyter/cli.py` & `ocxtools-1.5.1/ocxtools/jupyter/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Docker CLI."""
 # System imports
-from typing import Any, Tuple
-from typing_extensions import Annotated
-from ocxtools.renderer.renderer import RichTable
 import re
+from typing import Any, Tuple
+
 # 3rd party imports
 import typer
+from typing_extensions import Annotated
 
 # Project imports
 from ocxtools import config
 from ocxtools.context.context_manager import get_context_manager
+from ocxtools.docker.cli import run
 from ocxtools.jupyter import __app_name__
+from ocxtools.renderer.renderer import RichTable
 from ocxtools.utils.utilities import SourceValidator
-from ocxtools.docker.cli import run
 
 # Docker
 DOCKER_DESKTOP = config.get("DockerSettings", "docker_desktop")
 
 jupyter = typer.Typer(help="Commands for managing the docker jupyter lab notebook.")
 
 
@@ -80,15 +81,15 @@
 
 @jupyter.command()
 def settings():
     """Show the jupyter lab container settings."""
     context_manager = get_context_manager()
     console = context_manager.get_console()
     console.section('Jupyter lab settings')
-    data = {key:value for key, value in config.items('JupyterSettings')}
+    data = dict(config.items('JupyterSettings'))
     table = RichTable.render(data=[data], title='Settings')
     console.print_table(table)
 
 
 @jupyter.command()
 def readme(
 ):
```

### Comparing `ocxtools-1.4.0/ocxtools/jupyter/readme.md` & `ocxtools-1.5.1/ocxtools/jupyter/readme.md`

 * *Files identical despite different names*

### Comparing `ocxtools-1.4.0/ocxtools/loader/loader.py` & `ocxtools-1.5.1/ocxtools/loader/loader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Dynamically load a python module."""
 # system imports
 import importlib
-from abc import ABC
 import sys
+from abc import ABC
 from types import ModuleType
 from typing import Any, List
 
 # 3rd party imports
 from loguru import logger
 
 # Project imports
```

### Comparing `ocxtools-1.4.0/ocxtools/parser/parser.py` & `ocxtools-1.5.1/ocxtools/parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Module for parsing a 3Docx model."""
 
 import dataclasses
-
 # system imports
 from abc import ABC
 from dataclasses import dataclass
 from typing import Dict, Iterator
+
 # 3rd party imports
 import lxml.etree
-from lxml.etree import Element
 from loguru import logger
+from lxml.etree import Element
 from xsdata.exceptions import ParserError
 from xsdata.formats.dataclass.context import XmlContext, XmlContextError
+from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.config import ParserConfig
 from xsdata.formats.dataclass.parsers.handlers import LxmlEventHandler
-from xsdata.formats.dataclass.parsers import XmlParser
 
 from ocxtools.exceptions import XmlParserError
-
 # Project imports
-from ocxtools.interfaces.interfaces import IObservable, IParser, ObservableEvent
+from ocxtools.interfaces.interfaces import (IObservable, IParser,
+                                            ObservableEvent)
 from ocxtools.loader.loader import DeclarationOfOcxImport, DynamicLoader
 from ocxtools.utils.utilities import OcxVersion, SourceValidator
 
 
 class MetaData:
     """Dataclass metadata."""
```

### Comparing `ocxtools-1.4.0/ocxtools/rds/cli.py` & `ocxtools-1.5.1/ocxtools/rds/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """This module provides the ocx_attribute_reader app functionality."""
 # System imports
-from typing import Tuple, Any, Annotated
+from typing import Annotated, Any, Tuple
 
 # 3rd party imports
 import typer
 
 # Project imports
 from ocxtools import config
-from ocxtools.renderer.renderer import RichTable
+from ocxtools.context.context_manager import get_context_manager
+from ocxtools.dataclass.dataclasses import ReportType
 from ocxtools.exceptions import ReporterError
+from ocxtools.rds import __app_name__
+from ocxtools.renderer.renderer import RichTable
 from ocxtools.reporter.report_manager import OcxReportManager
 from ocxtools.reporter.reporter import OcxReporter
-from ocxtools.dataclass.dataclasses import ReportType
-from ocxtools.context.context_manager import get_context_manager
-from ocxtools.rds import __app_name__
-from ocxtools.utils.utilities import SourceValidator, SourceError
-from ocxtools.serializer.serializer import ReportFormat, Serializer, SerializerError
+from ocxtools.serializer.serializer import (ReportFormat, Serializer,
+                                            SerializerError)
+from ocxtools.utils.utilities import SourceError, SourceValidator
 
 rds = typer.Typer(help="Reference Designation System output.")
 report_manager = OcxReportManager()  # Singleton
 REPORT_FOLDER = SourceValidator.mkdir(config.get('ValidatorSettings', 'report_folder'))
 
 
 @rds.command()
```

### Comparing `ocxtools-1.4.0/ocxtools/renderer/cli.py` & `ocxtools-1.5.1/ocxtools/renderer/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 #
 """Renderer CLI commands."""
 
 from pathlib import Path
-from typing import Tuple, Any
+from typing import Any, Tuple
+
 # 3rd party imports
 import typer
 
+from ocxtools import config
+from ocxtools.context.context_manager import get_context_manager
+from ocxtools.parser.parser import OcxParser
 # Project imports
 from ocxtools.renderer import __app_name__
-from ocxtools.parser.parser import OcxParser
 from ocxtools.renderer.renderer import XsltTransformer
-from ocxtools.context.context_manager import get_context_manager
-from ocxtools import config
 from ocxtools.utils.utilities import SourceValidator
+
 # # Renderer
 RESOURCES = config.get("RendererSettings", "resource_folder")
 OCX_XSLT = config.get("RendererSettings", "ocx_xslt")
 SCHEMATRON_XSLT = config.get("RendererSettings", "schematron_xslt")
 
 render = typer.Typer(help="Rendering of 3Docx models.")
 ocx_parser = OcxParser()
```

### Comparing `ocxtools-1.4.0/ocxtools/renderer/renderer.py` & `ocxtools-1.5.1/ocxtools/renderer/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """ Render classes"""
 
+from enum import Enum
+from pathlib import Path
 # System imports
 from typing import Dict, List, Optional
-from pathlib import Path
-from enum import Enum
+
 import pandas as pd
-# Third party imports
-from tabulate import tabulate
+from loguru import logger
 from lxml import etree
 from rich.table import Table
 from rich.tree import Tree
-from loguru import logger
+# Third party imports
+from tabulate import tabulate
 
+from ocxtools.console.console import style_table_header
+from ocxtools.exceptions import SourceError
 # Project imports
 from ocxtools.utils.utilities import SourceValidator
-from ocxtools.exceptions import SourceError
-from ocxtools.console.console import style_table_header
 
 
 class TreeNode:
     """
     Represents a node in a tree structure.
 
     Args:
```

### Comparing `ocxtools-1.4.0/ocxtools/reporter/cli.py` & `ocxtools-1.5.1/ocxtools/reporter/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """This module provides the ocx_attribute_reader app functionality."""
 # System imports
 from pathlib import Path
-from typing import Tuple, Any, List, Annotated, Union
+from typing import Annotated, Any, List, Tuple, Union
 
 # 3rd party imports
 import typer
-# Project imports
-from ocxtools.reporter import __app_name__
+
 from ocxtools import config
 from ocxtools.console.console import CliConsole
-from ocxtools.renderer.renderer import RichTable
+from ocxtools.context.context_manager import get_context_manager
+from ocxtools.dataclass.dataclasses import Report, ReportDataFrame, ReportType
 from ocxtools.exceptions import ReporterError
-from ocxtools.reporter.report_manager import OcxReportManager
+from ocxtools.renderer.renderer import RichTable
+# Project imports
+from ocxtools.reporter import __app_name__
 from ocxtools.reporter.reporter import OcxReporter
-from ocxtools.dataclass.dataclasses import ReportType, Report, ReportDataFrame
-from ocxtools.context.context_manager import get_context_manager
-
-from ocxtools.utils.utilities import SourceValidator, SourceError
-from ocxtools.serializer.serializer import ReportFormat, Serializer, SerializerError
+from ocxtools.serializer.serializer import (ReportFormat, Serializer,
+                                            SerializerError)
+from ocxtools.utils.utilities import SourceError, SourceValidator
 
 report = typer.Typer(help="Reporting of 3Docx attributes")
-report_manager = OcxReportManager()  # Singleton
 REPORT_FOLDER = SourceValidator.mkdir(config.get('ValidatorSettings', 'report_folder'))
 
 
 def parse_content(console: CliConsole, status, model: str, report_type: ReportType) -> Union[Report, None]:
     """
     Parses the content of a given model and report type.
 
@@ -90,14 +89,15 @@
 def delete(
         model: str,
 
 ):
     """Delete all reports for a given model."""
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     count = report_manager.delete_report(model=model)
     console.info(f'Deleted {count} reports for model: {model!r}')
 
 
 @report.command()
 def content(
         model: str,
@@ -107,14 +107,15 @@
             bool, typer.Option(help="Save a detailed report of the validated models in the report folder.")] = True,
         report_format: Annotated[ReportFormat, typer.Option(help="File format")] = ReportFormat.PARQUET.value,
         report_folder: Annotated[str, typer.Option(help="Path to the report folder")] = REPORT_FOLDER,
 ):
     """Create the 3Docx content reports."""
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     try:
         SourceValidator.validate(model)
         match report_type.value:
             case ReportType.ALL.value:
                 with console.status("Parsing the model content for all elements...") as status:
                     for member_name, member_value in ReportType.__members__.items():
                         if member_value.value not in [ReportType.ALL.value, ReportType.COUNT.value]:
@@ -164,14 +165,15 @@
         model: str,
 ):
     """
     3Docx model count elements report
     """
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     try:
         with console.status("Counting elements in the model..."):
             reporter = OcxReporter()
             reporter.parse_model(model)
             report = reporter.element_count()
             if report is not None:
                 report_manager.add_report(report)
@@ -184,14 +186,15 @@
 @report.command()
 def summary():
     """
     3Docx model summary reports
     """
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     console.section('Report Summary')
     try:
         summary = report_manager.report_summary()
         if len(summary) > 0:
             table = RichTable.render(data=summary, title='Summary')
             console.print_table(table)
         else:
@@ -213,14 +216,15 @@
 
 ):
     """
     3Docx model detailed reports.
     """
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     try:
         to_col = int(max_col)
         console.section('Report Details')
         for item in report_manager.report_detail(report_type=report,
                                                  level=level,
                                                  max_col=to_col,
                                                  member=member,
@@ -246,14 +250,15 @@
             ReportType, typer.Option(help="Specify the 3Docx report.")] = ReportType.VESSEL.value,
 ):
     """
     3Docx content table levels.
     """
     context_manager = get_context_manager()
     console = context_manager.get_console()
+    report_manager = context_manager.get_report_manager()
     try:
         console.section('Table Tree')
         for item in report_manager.report_tree(report_type=report):
             if item is not None:
                 table = RichTable.render(data=[item], title=report.value)
                 console.print_table(table)
             else:
```

### Comparing `ocxtools-1.4.0/ocxtools/reporter/report_manager.py` & `ocxtools-1.5.1/ocxtools/reporter/report_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #  Copyright (c) 2024. OCX Consortium https://3docx.org. See the LICENSE
 """The report manager implementation."""
 # System imports
-from collections import defaultdict
 import os
-
+from collections import defaultdict
 from typing import Dict, List
 
 # Third party
 # project imports
-from ocxtools.dataclass.dataclasses import Report, ReportType, DetailedReport
+from ocxtools.dataclass.dataclasses import DetailedReport, Report, ReportType
 
 
 class OcxReportManager:
     """
     The OCX reporter class.
     """
```

### Comparing `ocxtools-1.4.0/ocxtools/reporter/reporter.py` & `ocxtools-1.5.1/ocxtools/reporter/reporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 #  Copyright (c) 2023-2024. OCX Consortium https://3docx.org. See the LICENSE
 """OCX reporter module"""
 
 # System imports
 from collections import defaultdict
-from typing import Any, Dict, List, Union
-from pathlib import Path
-from itertools import groupby
 from dataclasses import dataclass, is_dataclass
-import pandas as pd
 from enum import Enum
+from itertools import groupby
+from pathlib import Path
+from typing import Any, Dict, List, Union
 
+import arrow
 # Third party
 import lxml
-from lxml.etree import Element, QName
+import pandas as pd
 from loguru import logger
-import arrow
+from lxml.etree import Element, QName
+from ocx_schema_parser.xelement import LxmlElement
+from xsdata.exceptions import ParserError
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.parsers.handlers import LxmlEventHandler
-from xsdata.exceptions import ParserError
-
 
+from ocxtools.dataclass.dataclasses import (ElementCount, OcxHeader,
+                                            ReportDataFrame,
+                                            ReportElementCount, ReportType)
+from ocxtools.exceptions import ReporterError, SourceError
+from ocxtools.interfaces.interfaces import ABC, IObserver, ObservableEvent
+from ocxtools.loader.loader import (DeclarationOfOcxImport, DynamicLoader,
+                                    DynamicLoaderError)
 # project imports
 from ocxtools.parser.parser import OcxNotifyParser
-from ocxtools.dataclass.dataclasses import (OcxHeader, ReportDataFrame, ReportElementCount, ElementCount,
-                                            ReportType)
-from ocxtools.interfaces.interfaces import ABC, IObserver, ObservableEvent
-from ocxtools.utils.utilities import SourceValidator, OcxVersion, is_substring_in_list
-from ocxtools.exceptions import ReporterError, SourceError
-from ocx_schema_parser.xelement import LxmlElement
-from ocxtools.loader.loader import DeclarationOfOcxImport, DynamicLoader, DynamicLoaderError
+from ocxtools.utils.utilities import (OcxVersion, SourceValidator,
+                                      is_substring_in_list)
 
 
 def all_empty_array(column: pd.Series) -> bool:
     """
     Check if all elements in a column are empty arrays.
 
     Args:
         column: A pandas Series representing a column of data.
 
     Returns:
         bool: True if all elements in the column are empty arrays, False otherwise.
 
     """
-    if column.dtype == object:
-        if not column.isna().any():
-            lengths = column.apply(len)
-            if lengths.max() == 0:
-                return True
+    if column.dtype == object and not column.isna().any():
+        lengths = column.apply(len)
+        if lengths.max() == 0:
+            return True
     return False
 
 
 def flatten_data(data: Any, parent_key: str = '', sep: str = '.') -> Dict[str, Any]:
     """
     Flattens nested data structures into a dictionary.
 
@@ -245,16 +246,16 @@
                 logger.error(f'There are {duplicates} duplicate GUIDRef for element {report_type}')
             return ReportDataFrame(
                 source=model,
                 type=report_type,
                 count=data_frame.shape[0],
                 unique=data_frame.shape[0] - duplicates,
                 columns=data_frame.shape[1],
-                levels=max([col.count('.') for col in data_frame.columns]),
-                elements=data_frame
+                levels=max(col.count('.') for col in data_frame.columns),
+                elements=data_frame,
             )
         except (IndexError, ValueError) as e:
             logger.error(e)
             raise ReporterError(e) from e
 
     @staticmethod
     def datframe_types(model: str, report_type: ReportType, data: List[dataclass]) -> ReportDataFrame:
@@ -315,40 +316,43 @@
     Return the ocx:GUIDRef.
     Args:
         element: The element instance
 
     Returns:
         The GUIDRef value if present, else None
     """
-    guid = None
     attributes = element.attrib
     prefix = element.prefix
     ns = LxmlElement.namespaces_decorate(element.nsmap.get(prefix))
-    if is_substring_in_list('GUIDRef', attributes.keys()) and not is_substring_in_list('refType', attributes.keys()):
-        guid = attributes.get(f'{ns}GUIDRef')
-    return guid
+    return (
+        attributes.get(f'{ns}GUIDRef')
+        if is_substring_in_list('GUIDRef', attributes.keys())
+        and not is_substring_in_list('refType', attributes.keys())
+        else None
+    )
 
 
 def get_guid_ref(element: Element) -> Union[None, str]:
     """
     Return the guid or localref refernce of an element.
     Args:
         element: The element instance
 
     Returns:
         The GUIDRef value if present, else None
     """
-    guid_ref = None
     attributes = element.attrib
     prefix = element.prefix
     ns = element.nsmap[prefix]
     ns = LxmlElement.namespaces_decorate(ns)
-    if is_substring_in_list('refType', attributes.keys()):
-        guid_ref = attributes.get(f'{ns}GUIDRef')
-    return guid_ref
+    return (
+        attributes.get(f'{ns}GUIDRef')
+        if is_substring_in_list('refType', attributes.keys())
+        else None
+    )
 
 
 class OcxReporter:
     """3Docx attribute reporter"""
 
     def __init__(self):
         self._root = None
```

### Comparing `ocxtools-1.4.0/ocxtools/serializer/cli.py` & `ocxtools-1.5.1/ocxtools/serializer/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 from pathlib import Path
 from typing import Any, Tuple
 
 # 3rd party imports
 import typer
 from typing_extensions import Annotated
 
+from ocxtools import config
+from ocxtools.context.context_manager import get_context_manager
 from ocxtools.exceptions import XmlParserError
 from ocxtools.parser.parser import OcxParser
-
+from ocxtools.serializer import __app_name__
 # Project imports
 from ocxtools.serializer.serializer import OcxSerializer
-from ocxtools.serializer import __app_name__
-from ocxtools import config
-from ocxtools.context.context_manager import get_context_manager
 
 JSON_INDENT = int(config.get("SerializerSettings", "json_indent"))
 SERIALIZER_SUFFIX = config.get("SerializerSettings", "suffix")
 
 
 serialize = typer.Typer(help="Serialisation of 3Docx models.")
 ocx_parser = OcxParser()
```

### Comparing `ocxtools-1.4.0/ocxtools/serializer/resource/gitb_trl_stylesheet_v1.0.xsl` & `ocxtools-1.5.1/ocxtools/serializer/resource/gitb_trl_stylesheet_v1.0.xsl`

 * *Files identical despite different names*

### Comparing `ocxtools-1.4.0/ocxtools/serializer/serializer.py` & `ocxtools-1.5.1/ocxtools/serializer/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """OcxSerializer module."""
 
+import csv
 # system imports
 from dataclasses import dataclass
-import pyarrow
-import csv
-from typing import List
 from enum import Enum
 from pathlib import Path
+from typing import List
+
+import pyarrow
+from loguru import logger
 # 3rd party imports
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.serializers import JsonSerializer, XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
-from loguru import logger
+
+from ocxtools.dataclass.dataclasses import ReportDataFrame
 # Project imports
 from ocxtools.parser.parser import MetaData
-from ocxtools.dataclass.dataclasses import ReportDataFrame
 
 
 class ReportFormat(Enum):
     """Serialisation formats"""
     CSV = 'csv'
     PARQUET = 'parquet'
```

### Comparing `ocxtools-1.4.0/ocxtools/utils/utilities.py` & `ocxtools-1.5.1/ocxtools/utils/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Shared utility classes and functions"""
 # System imports
-import sys
 import errno
 import logging
 import os
 import re
+import sys
 from collections import defaultdict
-from typing import Dict, List
-import yaml
 from itertools import groupby
 from pathlib import Path
+from typing import Dict, Generator, List
 from urllib.parse import urlparse
-from typing import Generator
+
+import yaml
 
 # Project imports
 from ocxtools.exceptions import SourceError
 
 
 def is_substring_in_list(substring, string_list):
     """
```

### Comparing `ocxtools-1.4.0/ocxtools/validator/cli.py` & `ocxtools-1.5.1/ocxtools/validator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """Validator CLI."""
 # System imports
-import json
 import base64
-from typing import Any, Tuple, List
+import json
 from pathlib import Path
+from typing import Any, List, Tuple
 
+import click
+import typer
 # 3rd party imports
 from loguru import logger
-import typer
 from typing_extensions import Annotated
-import click
 
 # Project imports
 from ocxtools import config
-from ocxtools.validator import __app_name__
-from ocxtools.validator.validator_report import ValidatorReportFactory
-from ocxtools.validator.validator_client import (
-    EmbeddingMethod,
-    ValidationDomain, OcxValidatorClient,
-    ValidatorError)
-from ocxtools.renderer.renderer import RichTable
-from ocxtools.utils.utilities import SourceValidator
 from ocxtools.context.context_manager import get_context_manager
+from ocxtools.renderer.renderer import RichTable
 from ocxtools.serializer.serializer import ReportFormat, Serializer
+from ocxtools.utils.utilities import SourceValidator
+from ocxtools.validator import __app_name__
+from ocxtools.validator.validator_client import (EmbeddingMethod,
+                                                 OcxValidatorClient,
+                                                 ValidationDomain,
+                                                 ValidatorError)
+from ocxtools.validator.validator_report import ValidatorReportFactory
 
 REPORT_FOLDER = SourceValidator.mkdir(config.get('ValidatorSettings', 'report_folder'))
 SUFFIX = config.get('ValidatorSettings', 'report_suffix')
 VALIDATOR = config.get('ValidatorSettings', 'validator_url')
 validate = typer.Typer(help="Validation of 3Docx models.")
```

### Comparing `ocxtools-1.4.0/ocxtools/validator/validator_client.py` & `ocxtools-1.5.1/ocxtools/validator/validator_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """OCX validator client module."""
 # System imports
-from abc import ABC
-from pathlib import Path
 import base64
+import itertools
 import json
-from enum import Enum
+from abc import ABC
 from collections import defaultdict
-from typing import List, Tuple, Any
-import itertools
+from enum import Enum
+from pathlib import Path
+from typing import Any, Dict, List, Tuple
 
-from typing import Dict
 # 3rd party imports
 import lxml.etree
 from loguru import logger
+
 # Project
-from ocxtools.clients.clients import CurlClientError, CurlRestClient, AsyncRestClient, RequestClientError, RequestType
+from ocxtools.clients.clients import (AsyncRestClient, CurlClientError,
+                                      CurlRestClient, RequestClientError,
+                                      RequestType)
+from ocxtools.dataclass.dataclasses import OcxHeader
 from ocxtools.exceptions import SourceError
+from ocxtools.reporter.reporter import OcxReportFactory
 from ocxtools.utils.utilities import OcxVersion, SourceValidator
 from ocxtools.validator.validator_report import ValidatorReportFactory
-from ocxtools.dataclass.dataclasses import OcxHeader
-from ocxtools.reporter.reporter import OcxReportFactory
 
 
 class ValidatorError(ValueError):
     """Validator errors."""
 
 
 class EmbeddingMethod(Enum):
```

### Comparing `ocxtools-1.4.0/ocxtools/validator/validator_report.py` & `ocxtools-1.5.1/ocxtools/validator/validator_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 """The validator report class."""
 
+import json
 # System imports
 import re
+from typing import List
+
 # Third party imports
 import arrow
 import lxml.etree
 from loguru import logger
-from typing import List
-import json
-# Project imports
-
-from ocxtools.dataclass.dataclasses import ValidationReport, ValidationInformation, ValidationDetails, OcxHeader
 from ocx_schema_parser.xelement import LxmlElement
+
+from ocxtools.dataclass.dataclasses import (OcxHeader, ValidationDetails,
+                                            ValidationInformation,
+                                            ValidationReport)
 from ocxtools.exceptions import ReporterError
 
+# Project imports
+
+
 
 class ValidatorReportFactory:
     """Validator report."""
 
     @staticmethod
     def create_report(source: str, report_data: str, header: OcxHeader) -> ValidationReport:
         """
```

### Comparing `ocxtools-1.4.0/pyproject.toml` & `ocxtools-1.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ocxtools"
-version = "1.4.0"
+version = "1.5.1"
 description = "Python utility CLI for working with 3Docx models."
 authors = ["ocastrup <ole.christian.astrup@dnv.com>"]
 readme = "README.md"
 packages = [{include = "ocxtools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -56,15 +56,15 @@
 ocxtools = "ocxtools.cli:main"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 github_url = "https://github.com/OCXStandard/ocxtools"
 
 [tool.tbump.version]
-current = "1.4.0"
+current = "1.5.1"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `ocxtools-1.4.0/PKG-INFO` & `ocxtools-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocxtools
-Version: 1.4.0
+Version: 1.5.1
 Summary: Python utility CLI for working with 3Docx models.
 Author: ocastrup
 Author-email: ole.christian.astrup@dnv.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

