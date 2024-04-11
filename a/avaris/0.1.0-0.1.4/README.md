# Comparing `tmp/avaris-0.1.0.tar.gz` & `tmp/avaris-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avaris-0.1.0.tar", max compression
+gzip compressed data, was "avaris-0.1.4.tar", max compression
```

## Comparing `avaris-0.1.0.tar` & `avaris-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0    11357 2024-02-29 21:44:09.553077 avaris-0.1.0/LICENSE
--rw-r--r--   0        0        0     4049 2024-03-07 19:27:24.783897 avaris-0.1.0/README.md
--rw-r--r--   0        0        0      137 2024-03-07 22:17:25.880735 avaris-0.1.0/config/conf.yml
--rw-r--r--   0        0        0      929 2024-03-07 21:39:59.810059 avaris-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      299 2024-03-07 20:45:42.376476 avaris-0.1.0/src/avaris/__init__.py
--rw-r--r--   0        0        0      111 2024-03-07 19:27:24.783897 avaris-0.1.0/src/avaris/__main__.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/api/__init__.py
--rw-r--r--   0        0        0     2431 2024-03-07 22:27:49.184178 avaris-0.1.0/src/avaris/api/models.py
--rw-r--r--   0        0        0      540 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/api/output.py
--rw-r--r--   0        0        0     1864 2024-03-07 21:46:29.136706 avaris-0.1.0/src/avaris/cli.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/config/__init__.py
--rw-r--r--   0        0        0     2149 2024-03-07 21:56:31.962357 avaris-0.1.0/src/avaris/config/config_loader.py
--rw-r--r--   0        0        0     2064 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/config/config_manager.py
--rw-r--r--   0        0        0      364 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/config/error.py
--rw-r--r--   0        0        0      961 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/config/exception.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/__init__.py
--rw-r--r--   0        0        0     1142 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/datamanager.py
--rw-r--r--   0        0        0      383 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/models.py
--rw-r--r--   0        0        0      341 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/s3.py
--rw-r--r--   0        0        0      197 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/shipper.py
--rw-r--r--   0        0        0     6773 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/data/sql.py
--rw-r--r--   0        0        0      937 2024-03-07 22:27:59.804170 avaris-0.1.0/src/avaris/defaults.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/engine/__init__.py
--rw-r--r--   0        0        0      114 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/engine/commands.py
--rw-r--r--   0        0        0     4107 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/engine/engine.py
--rw-r--r--   0        0        0      446 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/engine/listener.py
--rw-r--r--   0        0        0     6998 2024-03-07 22:25:53.658350 avaris-0.1.0/src/avaris/engine/start.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/__init__.py
--rw-r--r--   0        0        0      943 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/apicall.py
--rw-r--r--   0        0        0     1700 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/endpoint.py
--rw-r--r--   0        0        0     4023 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/executor.py
--rw-r--r--   0        0        0     2526 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/fetch_file.py
--rw-r--r--   0        0        0     2878 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/github_release.py
--rw-r--r--   0        0        0     1080 2024-03-07 19:27:24.793897 avaris-0.1.0/src/avaris/executor/http_request.py
--rw-r--r--   0        0        0     1121 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/executor/shell.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/handler/__init__.py
--rw-r--r--   0        0        0      688 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/handler/handler.py
--rw-r--r--   0        0        0      762 2024-02-29 21:44:09.553077 avaris-0.1.0/src/avaris/manage.py
--rw-r--r--   0        0        0      132 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/registry.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/service/__init__.py
--rw-r--r--   0        0        0      411 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/service/dataqueue.py
--rw-r--r--   0        0        0     4891 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/service/datasource.py
--rw-r--r--   0        0        0      312 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/service/service.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/task/__init__.py
--rw-r--r--   0        0        0      773 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/task/task_registry.py
--rw-r--r--   0        0        0     7055 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/task/taskmaster.py
--rw-r--r--   0        0        0     4032 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/task/taskmaster_apscheduler.py
--rw-r--r--   0        0        0     1346 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/task/taskmaster_celery.py
--rw-r--r--   0        0        0        0 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/utils/__init__.py
--rw-r--r--   0        0        0     1644 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/utils/logging.py
--rw-r--r--   0        0        0      529 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/utils/management.py
--rw-r--r--   0        0        0     6266 2024-03-07 19:27:24.803897 avaris-0.1.0/src/avaris/utils/parse.py
--rw-r--r--   0        0        0     5322 1970-01-01 00:00:00.000000 avaris-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-10 12:46:19.234737 avaris-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4095 2024-04-10 12:46:19.234737 avaris-0.1.4/README.md
+-rw-r--r--   0        0        0     1107 2024-04-10 12:46:19.238737 avaris-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      656 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/__init__.py
+-rw-r--r--   0        0        0     4112 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/models.py
+-rw-r--r--   0        0        0      540 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/api/output.py
+-rw-r--r--   0        0        0     3427 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/cli.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/__init__.py
+-rw-r--r--   0        0        0     2051 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/config_loader.py
+-rw-r--r--   0        0        0     2746 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/config_manager.py
+-rw-r--r--   0        0        0      371 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/error.py
+-rw-r--r--   0        0        0      961 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/config/exception.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/__init__.py
+-rw-r--r--   0        0        0     1152 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/datamanager.py
+-rw-r--r--   0        0        0      383 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/models.py
+-rw-r--r--   0        0        0      341 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/s3.py
+-rw-r--r--   0        0        0      197 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/shipper.py
+-rw-r--r--   0        0        0     6676 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/data/sql.py
+-rw-r--r--   0        0        0     2444 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/defaults.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/commands.py
+-rw-r--r--   0        0        0     4099 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/engine.py
+-rw-r--r--   0        0        0      446 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/listener.py
+-rw-r--r--   0        0        0     6900 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/engine/start.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/__init__.py
+-rw-r--r--   0        0        0      943 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/apicall.py
+-rw-r--r--   0        0        0     1700 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/endpoint.py
+-rw-r--r--   0        0        0     4023 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/executor.py
+-rw-r--r--   0        0        0     2526 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/fetch_file.py
+-rw-r--r--   0        0        0     2865 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/github_release.py
+-rw-r--r--   0        0        0     1084 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/http_get_request.py
+-rw-r--r--   0        0        0     1121 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/executor/shell.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/handler/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/handler/handler.py
+-rw-r--r--   0        0        0      762 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/manage.py
+-rw-r--r--   0        0        0      132 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/registry.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/dataqueue.py
+-rw-r--r--   0        0        0     6205 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/datasource.py
+-rw-r--r--   0        0        0      312 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/service/service.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/__init__.py
+-rw-r--r--   0        0        0     1073 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/plugins.py
+-rw-r--r--   0        0        0      773 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/task_registry.py
+-rw-r--r--   0        0        0     7105 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster.py
+-rw-r--r--   0        0        0     3782 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster_apscheduler.py
+-rw-r--r--   0        0        0     1346 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/task/taskmaster_celery.py
+-rw-r--r--   0        0        0        0 2024-04-10 12:46:19.238737 avaris-0.1.4/src/avaris/utils/__init__.py
+-rw-r--r--   0        0        0     1455 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/auth.py
+-rw-r--r--   0        0        0     2188 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/logging.py
+-rw-r--r--   0        0        0      529 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/management.py
+-rw-r--r--   0        0        0     7339 2024-04-10 12:46:19.242737 avaris-0.1.4/src/avaris/utils/parse.py
+-rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 avaris-0.1.4/PKG-INFO
```

### Comparing `avaris-0.1.0/LICENSE` & `avaris-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/README.md` & `avaris-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <h1 align="center" style="border-bottom: none">
-    <a href="//github.com/avyrion/avaris" target="_blank"><img alt="Avaris" src="etc/avaris.png"></a><br>Avaris Task Engine
+    <a href="//github.com/avyr-io/avaris" target="_blank"><img alt="Avaris" src="etc/avaris.png"></a><br>Avaris Task Engine
 </h1>
 
 <div align="center">
 
 </div>
 
 Avaris is a modular task execution and data processing engine designed for easy integration and customization for various task executions, with a strong focus on data management tasks.
@@ -17,62 +17,62 @@
 - **Extensible Executors:** Execute tasks based on predefined or custom logic.
 - **Data Management:** Introduces `SQLDataManager` for relational database management, in addition to customizable data managers and handlers for diverse data storage and processing needs.
 
 ## Installation
 
 ```bash
 # Clone the repository
-git clone https://github.com/avyrion/avaris.git
+git clone https://github.com/avyr-io/avaris.git
 cd avaris
 
 # Install requirements
 python -m pip install poetry
 poetry install
-python -m avaris start --config config/conf.yml --scraper-dir ./scrapers
+python -m avaris start --config config/conf.yml --compendium-dir ./compendium
 ```
 
 ## Getting Started
 
-To run Avaris, you'll need to specify your engine configuration and scraper directory. Here's a quick guide to get you started.
+To run Avaris, you'll need to specify your engine configuration and compendium directory. Here's a quick guide to get you started.
 
 ### Configuration Files
 
 Avaris requires two main types of configuration files:
 
 - **Engine Configuration (`config/conf.yml`):** Defines global settings for the Avaris avaris.engine.
-- **Scraper Configurations (`./scrapers`):** Each scraper should have its own configuration file in this directory, detailing tasks, endpoints, and data management settings.
+- **Compendium Configurations (`./compendium`):** Each compendium file should have its own configuration file in this directory, detailing tasks, endpoints, and data management settings.
 
 ### Running Avaris
 
 ```bash
-python -m avaris start --config config/conf.yml --scraper-dir ./scrapers
+python -m avaris start --config config/conf.yml --compendium-dir ./compendium
 ```
 
-Replace `config/conf.yml` and `./scrapers` with the paths to your actual engine configuration file and scraper configuration directory, respectively.
+Replace `config/conf.yml` and `./compendium` with the paths to your actual engine configuration file and compendium configuration directory, respectively.
 
 ## Examples
 
 Here are some examples of how to use Avaris for different tasks.
 
-### Defining a Scraper Configuration
+### Defining a compendium Configuration
 
 ```yaml
-# scraper_config.yml
-scraper:
-  - name: PrometheusVersionScraper
+# compendium_config.yml
+compendium:
+  - name: PrometheusVersioncompendium
     destination: local
     tasks:
       - name: FetchLatestPrometheusVersion
         schedule: "* * * * *"
         executor:
           task: http_get_github_release
           parameters:
             api_url: "https://api.github.com/repos/prometheus/prometheus/releases/latest"
 
-  - name: FluentBitVersionScraper
+  - name: FluentBitVersioncompendium
     destination: local
     tasks:
       - name: FetchLatestFluentBitVersion
         schedule: "* * * * *"
         executor:
           task: http_get_github_release
           parameters:
```

### Comparing `avaris-0.1.0/src/avaris/api/output.py` & `avaris-0.1.4/src/avaris/api/output.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/config/config_loader.py` & `avaris-0.1.4/src/avaris/config/config_loader.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-import yaml
 from pathlib import Path
-from avaris.defaults import Defaults
-from avaris.api.models import ScraperConfig
-from pydantic import ValidationError
 from typing import List, Union
-from avaris.config.error import ConfigError, MissingScraperKeyError
-from avaris.api.models import AppConfig
+
+import yaml
+from pydantic import ValidationError
+
+from avaris.api.models import AppConfig, Compendium, CompendiumWrapper
+from avaris.config.error import ConfigError
+from avaris.defaults import Defaults
 from avaris.utils.logging import get_logger
 
 logger = get_logger()
 
+
 class ConfigLoader:
 
     @staticmethod
-    def load_scraper_config(file_path: Union[str, Path]) -> List[ScraperConfig]:
-        with open(file_path, 'r') as file:
+    def load_compendium_config(file_path: Union[str, Path]) -> List[Compendium]:
+        with open(file_path, "r") as file:
             config_data = yaml.safe_load(file)
             # Handle the case where the YAML file is empty or contains only comments
             if config_data is None:
                 config_data = {}  # Use an empty dictionary if no data is found
 
         try:
-            if ScraperConfig.__NAME__ in config_data:  # Adjust to match your actual root key
-                config_list = config_data[ScraperConfig.__NAME__]
-                return [ScraperConfig(**item) for item in config_list]
-            else:
-                raise MissingScraperKeyError(
-                    f"No '{ScraperConfig.__NAME__}' key found in YAML.")
+            compendium_wrapper = CompendiumWrapper(**config_data)
+            return compendium_wrapper.compendium
         except ValidationError as e:
             raise ConfigError(f"Invalid configuration in {file_path}: {e}")
 
     @staticmethod
     def load_global_config(file_path: str) -> AppConfig:
         if file_path:
             # None goes to else block
             if Path(file_path).exists():
-                with open(file_path, 'r') as file:
+                with open(file_path, "r") as file:
                     config_data = yaml.safe_load(file)
                 try:
                     return AppConfig(**config_data)
                 except ValidationError as e:
-                    raise ConfigError(f"Invalid Avaris configuration in {file_path}: {e}")
+                    logger.error(f"Invalid Avaris configuration in {file_path}: {e}")
+                    raise ConfigError(
+                        f"Invalid Avaris configuration in {file_path}: {e}"
+                    )
             else:
                 logger.warning(f"No configuration file found at {file_path}!")
                 raise ConfigError(f"No configuration found {file_path}: {e}")
         else:
-            logger.warning(f"No configuration file provided {file_path}, using defaults...")
+            logger.warning(
+                f"No configuration file provided{f' {file_path}' if file_path else '.'} Using defaults..."
+            )
             config_data = yaml.safe_load(Defaults.DEFAULT_CONF)
-            return AppConfig(**config_data)
+            return AppConfig(**config_data)
```

### Comparing `avaris-0.1.0/src/avaris/config/exception.py` & `avaris-0.1.4/src/avaris/config/exception.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/data/datamanager.py` & `avaris-0.1.4/src/avaris/data/datamanager.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class DataManager(ABC):
 
     def __init__(self, logger: Optional[Logger] = None):
         self.logger = logger or get_logger()
 
     @abstractmethod
-    async def add_task_result(self, job_id: str, data: dict) -> None:
+    async def add_task_result(self, execution_result: ExecutionResult) -> None:
         raise NotImplementedError()
 
     @abstractmethod
     async def get_task_result(self, job_id: str) -> ExecutionResult:
         raise NotImplementedError()
 
     @abstractmethod
```

### Comparing `avaris-0.1.0/src/avaris/data/sql.py` & `avaris-0.1.4/src/avaris/data/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,32 +12,33 @@
 from avaris.api.models import ExecutionResult
 from avaris.data.datamanager import DataManager
 from avaris.data.models import Base, SQLExecutionResult
 
 
 class SQLDataManager(DataManager):
 
-    def __init__(self,
-                 logger: Optional[Logger] = None,
-                 database_url: str = None):
+    def __init__(self, logger: Optional[Logger] = None, database_url: str = None):
         super().__init__(logger)
         self.database_url = database_url
-        self.engine = create_async_engine(self.database_url, echo=True)
-        self.SessionLocal = sessionmaker(autocommit=False,
-                                         autoflush=False,
-                                         bind=self.engine,
-                                         class_=AsyncSession)
+        self.engine = create_async_engine(self.database_url, echo=False)
+        self.SessionLocal = sessionmaker(
+            autocommit=False,
+            autoflush=False,
+            bind=self.engine,
+            class_=AsyncSession,
+        )
 
     async def init_db(self):
         async with self.engine.begin() as conn:
             await conn.run_sync(Base.metadata.create_all)
             self.logger.info("SQL Database initialized")
 
-    async def get_slice_sql(self, from_time: datetime,
-                            to_time: datetime) -> List[SQLExecutionResult]:
+    async def get_slice_sql(
+        self, from_time: datetime, to_time: datetime
+    ) -> List[SQLExecutionResult]:
         """
         Fetches task results that were recorded within the specified time range.
 
         Args:
             from_time (datetime): The start of the time range.
             to_time (datetime): The end of the time range.
 
@@ -55,34 +56,38 @@
                 return result
             except SQLAlchemyError as e:
                 self.logger.error(
                     f"Failed to retrieve task results within time range from the SQL database: {e}"
                 )
                 return []
 
-    async def get_slice(self, from_time: datetime,
-                        to_time: datetime) -> List[ExecutionResult]:
+    async def get_slice(
+        self, from_time: datetime, to_time: datetime
+    ) -> List[ExecutionResult]:
         """
         Fetches task results that were recorded within the specified time range
         and converts them to ExecutionResult objects.
 
         Args:
             from_time (datetime): The start of the time range.
             to_time (datetime): The end of the time range.
 
         Returns:
             List[ExecutionResult]: A list of ExecutionResult objects within the time range.
         """
         sql_results = await self.get_slice_sql(from_time, to_time)
         execution_results = [
-            ExecutionResult(name=result.name,
-                            task=result.task,
-                            id=result.id,
-                            timestamp=result.timestamp,
-                            result=result.result) for result in sql_results
+            ExecutionResult(
+                name=result.name,
+                task=result.task,
+                id=result.id,
+                timestamp=result.timestamp,
+                result=result.result,
+            )
+            for result in sql_results
         ]
         return execution_results
 
     async def add_task_result(self, execution_result: ExecutionResult):
         async with self.SessionLocal() as session:
             try:
                 db_task_result = SQLExecutionResult(
@@ -96,38 +101,40 @@
                 await session.commit()
                 self.logger.info(
                     f"Task result for {execution_result.task} added to the SQL database"
                 )
             except IntegrityError:
                 await session.rollback()  # Roll back the failed transaction
                 self.logger.info(
-                    f"Unique constraint failed for {execution_result.id}, updating existing record."
+                    f"Found existing {execution_result.task}[{execution_result.id}], updating record."
                 )
                 # Update the existing record
                 await session.execute(
-                    update(SQLExecutionResult).where(
-                        SQLExecutionResult.id == execution_result.id).values(
-                            name=execution_result.name,
-                            task=execution_result.task,
-                            result=execution_result.result,
-                            timestamp=execution_result.timestamp,
-                        ))
+                    update(SQLExecutionResult)
+                    .where(SQLExecutionResult.id == execution_result.id)
+                    .values(
+                        name=execution_result.name,
+                        task=execution_result.task,
+                        result=execution_result.result,
+                        timestamp=execution_result.timestamp,
+                    )
+                )
                 await session.commit()
             except SQLAlchemyError as e:
-                await session.rollback(
-                )  # Ensure to roll back on other SQL errors
+                await session.rollback()  # Ensure to roll back on other SQL errors
                 self.logger.error(
                     f"Failed to add or update task result for {execution_result.task} in the SQL database: {e}"
                 )
 
     async def get_task_result(self, job_id: str):
         try:
             async with self.SessionLocal() as session:
                 query = select(SQLExecutionResult).filter(
-                    SQLExecutionResult.id == job_id)
+                    SQLExecutionResult.id == job_id
+                )
                 result = await session.execute(query)
                 task_result = result.scalars().first()
                 return task_result.result if task_result else None
         except SQLAlchemyError as e:
             self.logger.error(
                 f"Failed to retrieve task result for {job_id} from the SQL database: {e}"
             )
@@ -135,15 +142,16 @@
     async def get_all_tasks(self):
         try:
             async with self.SessionLocal() as session:
                 result = await session.execute(select(SQLExecutionResult))
                 return result.scalars().all()
         except SQLAlchemyError as e:
             self.logger.error(
-                f"Failed to retrieve all tasks from the SQL database: {e}")
+                f"Failed to retrieve all tasks from the SQL database: {e}"
+            )
             return []
 
     async def get_all_task_names(self) -> List[str]:
         """
         Fetches a list of unique task names from the database.
 
         Returns:
```

### Comparing `avaris-0.1.0/src/avaris/engine/start.py` & `avaris-0.1.4/src/avaris/engine/start.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import asyncio
 import importlib
 import os
 import signal
 import sys
 from pathlib import Path
-from avaris.service.service import Service
+from typing import List
+
+from dotenv import load_dotenv
+
 import avaris.registry as registry
-from avaris.data.datamanager import DataManager
+from avaris.api.models import AppConfig
 from avaris.config.config_loader import ConfigLoader
 from avaris.config.error import ConfigError
-from avaris.api.models import AppConfig
+from avaris.data.datamanager import DataManager
 from avaris.data.s3 import S3DataManager
 from avaris.data.sql import SQLDataManager
+from avaris.defaults import Defaults, Names
+from avaris.engine.commands import AvarisEngineCommands
 from avaris.engine.engine import AvarisEngine
 from avaris.handler.handler import ResultHandler
 from avaris.service.datasource import DataSourceService
+from avaris.service.service import Service
+from avaris.task.plugins import PluginManager
 from avaris.task.taskmaster_apscheduler import APSchedulerTaskMaster
 from avaris.utils.logging import get_logger
-from typing import List
-from avaris.engine.commands import AvarisEngineCommands
-from dotenv import load_dotenv
-from avaris.defaults import Defaults,Names
+
 logger = get_logger()
 
 
-async def command_dispatcher(engine: AvarisEngine,
-                             command_queue: asyncio.Queue):
+async def command_dispatcher(engine: AvarisEngine, command_queue: asyncio.Queue):
     while True:
         command = await command_queue.get()
         if command == AvarisEngineCommands.START:
             await engine.start()
         elif command == AvarisEngineCommands.STOP:
             engine.stop()
         elif command == AvarisEngineCommands.SHUTDOWN:
@@ -37,57 +40,62 @@
             break
         elif command == AvarisEngineCommands.RELOAD:
             engine.stop()
             await engine.start()
         command_queue.task_done()
 
 
-async def shutdown_procedures(engine: AvarisEngine,
-                              services: List[Service] = None):
+async def shutdown_procedures(engine: AvarisEngine, services: List[Service] = None):
     logger.info("Initiating shutdown procedures...")
     await engine.shutdown()
     if services:
         for service in services:
             await service.shutdown()  # Assuming this is now an async method
     # Cancel all remaining asyncio tasks
     tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
     for task in tasks:
         task.cancel()
     await asyncio.gather(*tasks, return_exceptions=True)
     logger.info("Shutdown procedures completed.")
 
 
-def setup_signal_handlers(loop: asyncio.AbstractEventLoop,
-                          command_queue: asyncio.Queue):
+def setup_signal_handlers(
+    loop: asyncio.AbstractEventLoop, command_queue: asyncio.Queue
+):
 
     async def handle_signal():
         await command_queue.put(AvarisEngineCommands.SHUTDOWN)
 
     for sig in (signal.SIGINT, signal.SIGTERM):
-        loop.add_signal_handler(sig,
-                                lambda: asyncio.create_task(handle_signal()))
+        loop.add_signal_handler(sig, lambda: asyncio.create_task(handle_signal()))
 
 
-async def main(avaris_config_path: str, scraper_config_dir: str):
+async def main(
+    avaris_config_path: str, compendium_config_dir: str, compendium_file: str
+):
+    # Config file is -f specified. Add it as extra if specified
+    logger.info(f"Using Avaris config: {avaris_config_path}")
     config = ConfigLoader.load_global_config(avaris_config_path)
     services: List[Service] = []
     loop = asyncio.get_running_loop()
     command_queue = asyncio.Queue()
     asyncio.get_event_loop().set_debug(True)
     # Data Backend Setup
     data_manager = await setup_data_manager(config)
 
-    #Services Setup
-    if config.services["datasource"].enabled:
-        datasource_service = setup_datasource_service(config, data_manager)
-        services.append(datasource_service)
+    # Services Setup
+    if config.services:
+        if config.services.datasource.enabled:
+            datasource_service = setup_datasource_service(config, data_manager)
+            services.append(datasource_service)
 
     # Avaris Engine Setup
-    engine, dispatcher_task = setup_avaris_engine(scraper_config_dir,
-                                                  data_manager, command_queue)
+    engine, dispatcher_task = setup_avaris_engine(
+        compendium_config_dir, compendium_file, data_manager, command_queue
+    )
 
     # Register signal handlers for graceful shutdown
     setup_signal_handlers(loop, command_queue)
     await engine.start()
     await dispatcher_task  # Ensures that the dispatcher task runs and can be cleanly shut down
 
 
@@ -99,84 +107,85 @@
         data_manager = S3DataManager(logger=logger)
     else:
         raise ConfigError(f"Unknown data backend: {config.data_backend}")
     await data_manager.init_db()
     return data_manager
 
 
-def setup_datasource_service(config:AppConfig, data_manager: DataManager):
-    datasource_port = config.services["datasource"].port
+def setup_datasource_service(config: AppConfig, data_manager: DataManager):
+    datasource_port = config.services.datasource.port or 5000
     datasource_service = DataSourceService(data_manager=data_manager,
-                                     port=datasource_port,logger=logger)
+                                           port=datasource_port,
+                                           logger=logger,
+                                           listen=config.services.datasource.listen)
     asyncio.create_task(datasource_service.start())
     return datasource_service
 
 
-def setup_avaris_engine(scraper_config_dir, data_manager, command_queue):
+def setup_avaris_engine(
+    compendium_config_dir, compendium_file, data_manager, command_queue
+):
     result_handler = ResultHandler(data_manager=data_manager, logger=logger)
-    task_master = APSchedulerTaskMaster(logger=logger,
-                                        task_registry=registry.task_registry,
-                                        result_handler=result_handler,
-                                        use_daemon=True)
-    engine = AvarisEngine(data_manager=data_manager,
-                          task_master=task_master,
-                          scraper_config_dir=Path(scraper_config_dir),
-                          logger=logger)
-    dispatcher_task = asyncio.create_task(
-        command_dispatcher(engine, command_queue))
+    task_master = APSchedulerTaskMaster(
+        logger=logger,
+        task_registry=registry.task_registry,
+        result_handler=result_handler,
+        use_daemon=True,
+    )
+    engine = AvarisEngine(
+        data_manager=data_manager,
+        task_master=task_master,
+        compendium_config_dir=[Path(compendium_config_dir), compendium_file],
+        logger=logger,
+    )
+    dispatcher_task = asyncio.create_task(command_dispatcher(engine, command_queue))
     return engine, dispatcher_task
 
 
 def import_package_modules():
     import pkgutil
+
     import avaris.executor as executor_package
 
     for _, modname, ispkg in pkgutil.iter_modules(executor_package.__path__):
         full_module_name = f"{executor_package.__name__}.{modname}"
         if not ispkg:
             __import__(full_module_name)
 
 
-def import_plugin_modules(plugins_dir: Path):
-    if  plugins_dir not in sys.path:
-        sys.path.append(str(plugins_dir))
-    for path in plugins_dir.glob("**/*.py"):
-        if path.name == "__init__.py":
-            continue
-        module_path = f"plugins.executor.{path.stem}"
-        try:
-         
-            importlib.import_module(module_path)
-            logger.info(f"Successfully imported {module_path}")
-        except ModuleNotFoundError as e:
-            logger.error(f"Failed to import {module_path}: {e}")
-
-
-
-
-def start_engine(avaris_config_file:str, scraper_config_directory:str, plugins_directory:str=None):
+def start_engine(
+    avaris_config_file: str,
+    compendium_directory: str = None,
+    compendium_file: str = None,
+    plugins_directory: str = None,
+):
     import_package_modules()
-    avaris_config_file = Path(avaris_config_file) if Path(avaris_config_file).exists() else None
-    plugins_dir = Path(plugins_directory if plugins_directory else Path.cwd() / ".avaris"/"src")
-    if plugins_dir: 
+    avaris_config_path = (
+        Path(avaris_config_file) if Path(avaris_config_file).exists() else None
+    )
+    if not avaris_config_path:
+        logger.warning(f"Avaris config not found in {avaris_config_file}")
+    plugins_dir = (
+        Path(plugins_directory) or Defaults.DEFAULT_PLUGINS_DIR
+    )  # Might have to rework to use lists
+    if plugins_dir:
         logger.info(f"Using plugins directory: {plugins_dir}")
     if plugins_dir.exists():
-        import_plugin_modules(plugins_dir)
-    asyncio.run(main(avaris_config_file, scraper_config_directory))
+        PluginManager.import_plugin_modules(plugins_dir)
+    asyncio.run(main(avaris_config_path, compendium_directory, compendium_file))
 
 
 if __name__ == "__main__":
     if len(sys.argv) < 5:
         print(
-            "Usage: python -m engine.start --config <config_file> --scraper-dir <scraper_directory>"
+            "Usage: python -m engine.start --config <config_file> --compendium-dir <compendium_directory>"
         )
         sys.exit(1)
 
     if sys.argv[1] == "start":
         base_dir = Path(__file__).resolve().parent.parent.parent
         config_file_index = sys.argv.index("--config") + 1
-        scraper_dir_index = sys.argv.index("--scraper-dir") + 1
+        compendium_dir_index = sys.argv.index("--compendium-dir") + 1
         avaris_config_path = sys.argv[config_file_index]
-        scraper_config_dir = sys.argv[scraper_dir_index]
-
+        compendium_config_dir = sys.argv[compendium_dir_index]
 
-        start_engine(avaris_config_path, scraper_config_dir)
+        start_engine(avaris_config_path, compendium_config_dir)
```

### Comparing `avaris-0.1.0/src/avaris/executor/apicall.py` & `avaris-0.1.4/src/avaris/executor/apicall.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/executor/endpoint.py` & `avaris-0.1.4/src/avaris/executor/endpoint.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/executor/executor.py` & `avaris-0.1.4/src/avaris/executor/executor.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/executor/fetch_file.py` & `avaris-0.1.4/src/avaris/executor/fetch_file.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/executor/github_release.py` & `avaris-0.1.4/src/avaris/executor/github_release.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,62 @@
 import re
 import httpx
-from pydantic import BaseModel, HttpUrl,SecretStr
-from typing import  Optional
+from pydantic import BaseModel, HttpUrl, SecretStr
+from typing import Optional
 from avaris.executor.executor import TaskExecutor
 from avaris.task.task_registry import register_task_executor
 
 
 class GitHubReleaseRequestParameters(BaseModel):
     __NAME__ = "http_get_github_release"
     api_url: HttpUrl
     username: Optional[str] = None
     password: Optional[SecretStr] = None
 
 
 @register_task_executor(GitHubReleaseRequestParameters.__NAME__)
 class GitHubReleaseExecutor(TaskExecutor[GitHubReleaseRequestParameters]):
     PARAMETER_TYPE = GitHubReleaseRequestParameters
+
     async def execute(self) -> dict:
         try:
             secrets = await self.load_secrets()
             github_token = secrets.get("GITHUB_TOKEN", None)
             headers = {"Accept": "application/vnd.github.v3+json"}
 
             url = self.parameters.api_url.unicode_string()
             async with httpx.AsyncClient() as client:
                 if github_token:
                     headers[
                         "Authorization"] = f"token {github_token.get_secret_value()}"
-                    response = await client.get(url,
-                                                headers=headers)
+                    response = await client.get(url, headers=headers)
                 elif self.parameters.username and self.parameters.password:
                     auth = (self.parameters.username,
                             self.parameters.password.get_secret_value())
                     response = await client.get(url,
                                                 headers=headers,
                                                 auth=auth)
                 else:
-                    response = await client.get(url,
-                                                headers=headers)
+                    response = await client.get(url, headers=headers)
 
             if response.status_code == 200:
                 data = response.json()
                 version_tag = data.get("tag_name", "").strip(
                     "v")  # Remove leading 'v' if present
                 release_date = data.get("published_at",
                                         "").split("T")[0]  # YYYY-MM-DD format
-
+                release_notes_url = data.get("html_url", "")
                 # Extract repository name
-                match = re.search(r"/repos/([^/]+/[^/]+)/releases/latest",
-                                  url)
+                match = re.search(r"/repos/([^/]+/[^/]+)/releases/latest", url)
                 repository_name = match.group(1) if match else "Unknown"
 
                 return {
                     "name": repository_name,
                     "latest_version": version_tag,
+                    "release_notes": release_notes_url,
                     "release_date": release_date
                 }
 
             else:
                 self.logger.error(
                     f"Failed to fetch {self.parameters.api_url}: Status {response.status_code}"
                 )
```

### Comparing `avaris-0.1.0/src/avaris/executor/http_request.py` & `avaris-0.1.4/src/avaris/executor/http_get_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 from pydantic import BaseModel
 
 from avaris.executor.executor import TaskExecutor
 from avaris.task.task_registry import register_task_executor
 
 
 class HttpRequestParameters(BaseModel):
-    __NAME__ = "http_request"
+    __NAME__ = "http_get_request"
     url: str
-    method: str
 
 @register_task_executor(HttpRequestParameters.__NAME__)
 class HttpExecutor(TaskExecutor[HttpRequestParameters]):
     PARAMETER_TYPE = HttpRequestParameters
 
     async def execute(self) -> dict:
         try:
             response = requests.get(self.parameters.url)
             if response.status_code == 200:
                 return {
-                    response: f"Failed to fetch data from {url}. Status code: {response.text}"
+                    response: f"Failed to fetch data from {self.parameters.url}. Status code: {response.text}"
                 }
             else:
                 self.logger.error(
                     f"Failed to fetch {self.parameters.url}: Status {response.status_code}"
                 )
                 return {}
         except Exception as e:
```

### Comparing `avaris-0.1.0/src/avaris/executor/shell.py` & `avaris-0.1.4/src/avaris/executor/shell.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/handler/handler.py` & `avaris-0.1.4/src/avaris/handler/handler.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/manage.py` & `avaris-0.1.4/src/avaris/manage.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/service/datasource.py` & `avaris-0.1.4/src/avaris/service/datasource.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from datetime import datetime
 from logging import Logger
 from avaris.service.service import Service
-from fastapi import FastAPI, Request
+from fastapi import FastAPI, Request, HTTPException, Depends
 from uvicorn import Config, Server
 from avaris.data.datamanager import DataManager
 from avaris.utils.logging import get_logger
 import multiprocessing
 from typing import List
-from avaris.api.models import ExecutionResult
-
-
+from avaris.api.models import ExecutionResult, ListenerData
+from avaris.utils.parse import generate_task_id
+from avaris.utils.auth import validate_signature
+from avaris.defaults import Names
+import traceback
 class UvicornServer(multiprocessing.Process):
 
     def __init__(self, config: Config):
         super().__init__()
 
         self.config = config
 
@@ -26,27 +28,32 @@
 
 
 class DataSourceService(Service):
 
     def __init__(self,
                  data_manager: DataManager,
                  port: int = 5000,
-                 logger: Logger = None):
+                 logger: Logger = None,
+                 listen: bool = False):
+        self.listen = listen
+
         self.data_manager = data_manager
         self.port = port
         self.logger = logger or get_logger()
         self.app = FastAPI(title="datasource Data Source Service")
         self.setup_routes()
 
         self.config = Config(app=self.app,
                              host="0.0.0.0",
                              port=self.port,
                              log_level="info",
                              loop="asyncio")
         self.server = UvicornServer(config=self.config)
+        if self.listen:
+            self.logger.info("Listening enabled. Payloads to /push will be pushed to database.")
 
     def setup_routes(self):
 
         @self.app.post("/metrics")
         async def post_metrics():
             metrics = await self.data_manager.get_all_task_names()
             return metrics
@@ -93,19 +100,40 @@
                         series["datapoints"].append([metric_value, task_time])
 
                 return datasource_response
             except Exception as e:
                 self.logger.error(f"Error querying Data Source: {e}")
                 return {"error": f"Error querying Data Source: {e}"}
 
-        @self.app.post("/annotations")
-        async def annotations():
-            # Implement if you need annotations feature
-            # This should return a list of annotations.
-            return []
+        @self.app.post("/push")
+        async def push(request: Request,
+                       valid: bool = Depends(validate_signature)):
+            if not self.listen:
+                return {"status": "listening is disabled"}
+            try:
+                req_body = await request.json()
+                header = dict(request.headers)
+                result = ListenerData(body=req_body,
+                    header=header,
+                )
+                task_name = "_".join(header.keys())
+                await self.data_manager.add_task_result(ExecutionResult(
+                    name=f"push_{task_name}",
+                    task=Names.LISTENER_TASK,
+                    id=generate_task_id(compendium_name="",task_name=task_name,parameters=result),
+                    timestamp=datetime.now(),
+                    result=req_body
+                ))
+            except Exception as e:
+                self.logger.error(f"Error parsing request body: {e}")
+                self.logger.error(f"{traceback.format_exc()}")
+                return {"error": f"Error parsing request body: {e}"}, 400
+            return {"status": "ok"}
+
+
 
         @self.app.get("/health")
         async def health_check():
             return {"status": "ok"}
 
         @self.app.get("/tasks")
         async def get_all_tasks():
```

### Comparing `avaris-0.1.0/src/avaris/task/task_registry.py` & `avaris-0.1.4/src/avaris/task/task_registry.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/task/taskmaster.py` & `avaris-0.1.4/src/avaris/task/taskmaster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-from typing import List, Dict, Type, Callable, Optional
 from abc import ABC, abstractmethod
-from avaris.api.models import ScraperConfig, TaskConfig
-from avaris.executor.executor import TaskExecutor
-from avaris.utils.logging import get_logger
-from avaris.utils.parse import parse_cron_schedule, generate_task_id
-from typing import Set, Tuple
 from logging import Logger
+from typing import Callable, Dict, List, Optional, Set, Tuple, Type
+
+from avaris.api.models import Compendium, TaskConfig
 from avaris.config.error import ConfigError
+from avaris.executor.executor import TaskExecutor
 from avaris.handler.handler import ResultHandler
+from avaris.utils.logging import get_logger
+from avaris.utils.parse import generate_task_id, parse_cron_schedule
 
 
 class TaskMaster(ABC):
 
-    def __init__(self,
-                 task_registry: Dict[str, Type[TaskExecutor]],
-                 logger: Logger = None,
-                 result_handler: ResultHandler = None):
+    def __init__(
+        self,
+        task_registry: Dict[str, Type[TaskExecutor]],
+        logger: Logger = None,
+        result_handler: ResultHandler = None,
+    ):
         self.__running__ = False
         self.result_handler: ResultHandler = result_handler
         self.logger: Logger = logger or get_logger()
         self.task_registry: Dict[str, Type[TaskExecutor]] = task_registry
 
-        self.active_jobs: List[ScraperConfig] = []
+        self.active_jobs: List[Compendium] = []
         self.scheduled_job_ids: Set[str] = set()
         self.scheduler = self.create_scheduler()
         self.logger.info(f"Using {type(self.scheduler).__name__}")
 
-    def validate(self, task_list: List[ScraperConfig]) -> bool:
+    def validate(self, task_list: List[Compendium]) -> bool:
         active_tasks = [
-            task for scraper_config in task_list
-            for task in scraper_config.tasks
+            task for compendium_config in task_list for task in compendium_config.tasks
         ]
         # TODO: Implement actual validation logic
         return True
 
-    def reconfigure_active_jobs(
-            self, task_list: List[ScraperConfig]) -> Tuple[bool, str]:
+    def reconfigure_active_jobs(self, task_list: List[Compendium]) -> Tuple[bool, str]:
         if not task_list:  # If the task list is empty
             return False, "No valid configurations found."
 
         if self.validate(task_list):
             active_tasks = [
-                task.name for scraper_config in task_list
-                for task in scraper_config.tasks
+                task.name
+                for compendium_config in task_list
+                for task in compendium_config.tasks
             ]
             self.logger.info(f"Reconfiguring active jobs: {active_tasks}")
             self.active_jobs = task_list
             return True, ""  # Indicates success with no error message
         else:
             return False, "Validation failed for configurations."
 
@@ -54,77 +55,86 @@
         if not task_config.executor:
             raise ValueError("TaskConfig missing executor info.")
         executor_class = self.task_registry.get(task_config.executor.task)
         if not executor_class:
             raise ValueError(
                 f"No executor registered for type '{task_config.executor.task}'"
             )
-        return executor_class(task_config=task_config,
-                              result_handler=self.result_handler)
+        return executor_class(
+            task_config=task_config, result_handler=self.result_handler
+        )
 
     def configure_task_for_scheduling(
-            self, executor: TaskExecutor,
-            task_config: TaskConfig) -> Optional[Callable]:
+        self, executor: TaskExecutor, task_config: TaskConfig
+    ) -> Optional[Callable]:
         self.logger.debug(
             f"Fetching executor for task {task_config.name}:{task_config.executor.task}"
         )
 
-        task_with_handler = executor.get_task(
-            result_handler=self.result_handler)
+        task_with_handler = executor.get_task(result_handler=self.result_handler)
 
         return task_with_handler
 
     def reconcile(self) -> None:
         try:
             self.clear_invalid_jobs()
             self.schedule_active()
             self.logger.info(f"Reconciliation success")
         except Exception as e:
             self.logger.error(f"Error reconciling : {e}")
             raise RuntimeError(f"Error reconciling : {e}")
 
     def schedule_active(self):
         # Schedule new and updated jobs from the active_jobs list.
-        for scraper_config in self.active_jobs:
+        for compendium_config in self.active_jobs:
             try:
-                self.scraper_commit(scraper_config)
+                self.compendium_commit(compendium_config)
             except ValueError as e:
                 self.logger.error(f"Error scheduling task: {e}")
                 raise ConfigError(f"Error scheduling task: {e}")
 
-    def scraper_commit(self, scraper_config: ScraperConfig) -> None:
-        self.logger.info(f"Starting scraper_commit for: {scraper_config.name}")
-        for task_config in scraper_config.tasks:
+    def compendium_commit(self, compendium_config: Compendium) -> None:
+        self.logger.info(f"Compendium Commit for: {compendium_config.name}")
+        for task_config in compendium_config.tasks:
             executor = self.get_executor(task_config)
             if not executor:
-                self.logger.error(
-                    f"No executor found for task: {task_config.name}")
+                self.logger.error(f"No executor found for task: {task_config.name}")
                 continue
-            job_id = generate_task_id(scraper_config.name, task_config.name,
-                                      task_config.executor.parameters)
+            job_id = generate_task_id(
+                compendium_config.name,
+                task_config.name,
+                task_config.executor.parameters,
+            )
             func = executor.get_task(job_id)
             if not func:
                 self.logger.warning(
-                    f"No function configured for task: {task_config.name}")
+                    f"No function configured for task: {task_config.name}"
+                )
                 continue
             self.logger.info(
                 f"Scheduling task: {task_config.name}:{task_config.executor.task}"
             )
 
-            schedule = task_config.schedule  # Assuming schedule is directly compatible with APScheduler's format
+            schedule = (
+                task_config.schedule
+            )  # Assuming schedule is directly compatible with APScheduler's format
 
             self.schedule_job(func, job_id, schedule)
 
     def get_job_ids(self):
         """Generate the set of current job IDs based on the active jobs"""
         return set(
-            generate_task_id(scraper_config.name, task_config.name,
-                             task_config.executor.parameters)
-            for scraper_config in self.active_jobs
-            for task_config in scraper_config.tasks)
+            generate_task_id(
+                compendium_config.name,
+                task_config.name,
+                task_config.executor.parameters,
+            )
+            for compendium_config in self.active_jobs
+            for task_config in compendium_config.tasks
+        )
 
     @abstractmethod
     def get_jobs(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def remove_job(self, job_id: str) -> None:
```

### Comparing `avaris-0.1.0/src/avaris/task/taskmaster_apscheduler.py` & `avaris-0.1.4/src/avaris/task/taskmaster_apscheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,52 @@
-from apscheduler.schedulers.background import BackgroundScheduler
-from apscheduler.triggers.cron import CronTrigger
-import pytz
-from typing import Callable
-from avaris.task.taskmaster import TaskMaster
 import asyncio
-from typing import Dict, Type
-from avaris.executor.executor import TaskExecutor
 from logging import Logger
-from avaris.utils.logging import get_logger
+from typing import Callable, Dict, Type
 
-from apscheduler.schedulers.asyncio import AsyncIOScheduler
+import pytz
 from apscheduler.executors.asyncio import AsyncIOExecutor
 from apscheduler.executors.pool import ThreadPoolExecutor
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
+from apscheduler.schedulers.background import BackgroundScheduler
+from apscheduler.triggers.cron import CronTrigger
+
+from avaris.executor.executor import TaskExecutor
+from avaris.task.taskmaster import TaskMaster
+from avaris.utils.logging import get_logger
 
 
 class APSchedulerTaskMaster(TaskMaster):
     scheduler: BackgroundScheduler
 
-    def __init__(self,
-                 task_registry: Dict[str, Type[TaskExecutor]],
-                 logger: Logger = None,
-                 use_daemon=False,
-                 result_handler: Callable = None):
+    def __init__(
+        self,
+        task_registry: Dict[str, Type[TaskExecutor]],
+        logger: Logger = None,
+        use_daemon=False,
+        result_handler: Callable = None,
+    ):
         self.use_daemon = use_daemon
-        super().__init__(logger=logger,
-                         task_registry=task_registry,
-                         result_handler=result_handler)
+        super().__init__(
+            logger=logger, task_registry=task_registry, result_handler=result_handler
+        )
         """Create and return a BackgroundScheduler instance."""
 
     def create_scheduler(self) -> AsyncIOScheduler:
         """Create and return an AsyncIOScheduler instance."""
         executors = {
-            'default': ThreadPoolExecutor(10),  # For synchronous tasks
-            'asyncio': AsyncIOExecutor(),  # For asynchronous tasks
+            "default": ThreadPoolExecutor(10),  # For synchronous tasks
+            "asyncio": AsyncIOExecutor(),  # For asynchronous tasks
         }
         job_defaults = {
-            'coalesce': False,
-            'max_instances': 3,
+            "coalesce": False,
+            "max_instances": 3,
         }
-        scheduler = AsyncIOScheduler(executors=executors,
-                                     job_defaults=job_defaults,
-                                     timezone="UTC")
+        scheduler = AsyncIOScheduler(
+            executors=executors, job_defaults=job_defaults, timezone="UTC"
+        )
         return scheduler
 
     def start_scheduler(self):
         """Start the APScheduler."""
         self.scheduler.start()
 
     def stop_scheduler(self):
@@ -66,15 +68,17 @@
 
                 # Determine which jobs are outdated (i.e., scheduled but not in current_job_ids)
                 outdated_job_ids = scheduled_job_ids - current_job_ids
 
                 # Remove each outdated job from the scheduler
                 for job_id in outdated_job_ids:
                     self.remove_job(job_id)
-            self.logger.info("Jobs are empty.")
+                    self.logger.info(f"Removed {job_id}.")
+            else:
+                self.logger.info("No jobs to empty.")
             return True
         except Exception as e:
             self.logger.error(f"Error clearing jobs! {e}")
 
     def remove_job(self, job_id: str):
         super().remove_job(job_id)  # Call to super if you need common logic
         if job_id in self.scheduled_job_ids:
@@ -82,19 +86,14 @@
             self.scheduled_job_ids.remove(job_id)  # Remove from tracking set
 
     def schedule_job(self, func: Callable, job_id: str, schedule: str):
         trigger = CronTrigger.from_crontab(schedule, timezone=pytz.UTC)
 
         if asyncio.iscoroutinefunction(func):
             # This is an async function, schedule it with asyncio executor
-            self.scheduler.add_job(func,
-                                   trigger,
-                                   id=job_id,
-                                   executor='asyncio',
-                                   replace_existing=True)
+            self.scheduler.add_job(
+                func, trigger, id=job_id, executor="asyncio", replace_existing=True
+            )
         else:
             # This is a sync function, schedule as usual
-            self.scheduler.add_job(func,
-                                   trigger,
-                                   id=job_id,
-                                   replace_existing=True)
+            self.scheduler.add_job(func, trigger, id=job_id, replace_existing=True)
         self.scheduled_job_ids.add(job_id)
```

### Comparing `avaris-0.1.0/src/avaris/task/taskmaster_celery.py` & `avaris-0.1.4/src/avaris/task/taskmaster_celery.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/utils/management.py` & `avaris-0.1.4/src/avaris/utils/management.py`

 * *Files identical despite different names*

### Comparing `avaris-0.1.0/src/avaris/utils/parse.py` & `avaris-0.1.4/src/avaris/utils/parse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,177 +1,244 @@
 import csv
-import os
+import hashlib
 import json
+import os
+import re
+
 from datetime import datetime
+from pathlib import Path
+from typing import Dict, List, Optional, Union
 import pytz
 from flask import render_template_string
 from pydantic import BaseModel
-import re
-import hashlib
-from typing import Dict, List, Optional, Union
+
+
 
 def parse_cron_schedule(schedule_str: str) -> Dict[str, str]:
     """
     Parses a cron schedule string or shortcut into a dictionary suitable for APScheduler.
 
     Args:
         schedule_str: A cron schedule string, e.g., "*/5 * * * *", or a shortcut like "@hourly".
 
     Returns:
         A dictionary with keys for second, minute, hour, day, month, day_of_week.
     """
     shortcuts = {
-        '@yearly': '0 0 0 1 1 *',
-        '@annually': '0 0 0 1 1 *',
-        '@monthly': '0 0 0 1 * *',
-        '@weekly': '0 0 0 * * 0',
-        '@daily': '0 0 0 * * *',
-        '@hourly': '0 0 * * * *'
+        "@yearly": "0 0 0 1 1 *",
+        "@annually": "0 0 0 1 1 *",
+        "@monthly": "0 0 0 1 * *",
+        "@weekly": "0 0 0 * * 0",
+        "@daily": "0 0 0 * * *",
+        "@hourly": "0 0 * * * *",
     }
 
     schedule_str = shortcuts.get(schedule_str, schedule_str)
     parts = schedule_str.split()
     if len(parts) == 6:
-        return {'second': parts[0], 'minute': parts[1], 'hour': parts[2], 'day': parts[3], 'month': parts[4], 'day_of_week': parts[5]}
+        return {
+            "second": parts[0],
+            "minute": parts[1],
+            "hour": parts[2],
+            "day": parts[3],
+            "month": parts[4],
+            "day_of_week": parts[5],
+        }
     elif len(parts) == 5:
-        return {'second': '0', 'minute': parts[0], 'hour': parts[1], 'day': parts[2], 'month': parts[3], 'day_of_week': parts[4]}
+        return {
+            "second": "0",
+            "minute": parts[0],
+            "hour": parts[1],
+            "day": parts[2],
+            "month": parts[3],
+            "day_of_week": parts[4],
+        }
     else:
-        raise ValueError("Invalid cron schedule format. Expected 5 or 6 parts, or a recognized shortcut.")
+        raise ValueError(
+            "Invalid cron schedule format. Expected 5 or 6 parts, or a recognized shortcut."
+        )
+
 
 def is_valid_cron_expression(expression: str) -> bool:
     """
     Validates a cron expression format.
 
     Args:
         expression: A string representing a cron expression.
 
     Returns:
         True if the expression is valid, False otherwise.
     """
-    return bool(re.match(r'^(\d+|\*)( \d+|\*)( \d+|\*)( \d+|\*)( \d+|\*)$', expression))
+    return bool(re.match(r"^(\d+|\*)( \d+|\*)( \d+|\*)( \d+|\*)( \d+|\*)$", expression))
 
-def generate_task_id(scraper_name: str, task_name: str,
-                     parameters: BaseModel) -> str:
+# Your secret token
+
+def generate_task_id(
+    compendium_name: str, task_name: str, parameters: BaseModel
+) -> str:
     """
-    Generate a unique ID for a task based on its scraper name, task name, and parameters.
+    Generate a unique ID for a task based on its compendium name, task name, and parameters.
 
-    :param scraper_name: The name of the scraper config.
+    :param compendium_name: The name of the compendium config.
     :param task_name: The name of the task config.
     :param parameters: A dictionary of task parameters.
     :return: A unique task ID.
     """
-    params_string = str(sorted(
-        parameters.model_dump().items())) if parameters else ""
+    params_string = str([compendium_name,task_name]+sorted(parameters.model_dump().items())) if parameters else ""
 
     # Create a hash of the parameters string
-    params_hash = hashlib.sha256(params_string.encode()).hexdigest(
-    )[:16]  # Take first 8 chars for brevity
+    params_hash = hashlib.sha256(params_string.encode()).hexdigest()[
+        :16
+    ]  # Take first 8 chars for brevity
 
     # Concatenate elements to form the ID
-    task_id = f"{scraper_name}_{task_name}_{params_hash}"
+    task_id = f"{params_hash}"
 
     return task_id
 
-def extract_data(log: Dict, keys: List[str], default_values: Dict[str, str]) -> List[str]:
+
+def extract_data(
+    log: Dict, keys: List[str], default_values: Dict[str, str]
+) -> List[str]:
     """
     Extracts specified keys from a log dict, substituting defaults where necessary.
 
     Args:
         log: The log data as a dictionary.
         keys: The keys to extract from the log.
         default_values: Default values for keys that are not present in the log.
 
     Returns:
         A list of extracted values.
     """
     return [log.get(key, default_values.get(key, "")) for key in keys]
 
+
 def read_from_json(json_file_name: str) -> Dict:
     """
     Reads data from a JSON file.
 
     Args:
         json_file_name: The name of the JSON file.
 
     Returns:
         The JSON data as a dictionary.
     """
     json_file_path = os.path.join(os.getcwd(), json_file_name)
-    with open(json_file_path, 'r') as json_file:
+    with open(json_file_path, "r") as json_file:
         return json.load(json_file)
 
+
 def convert_from_unix_time(timestamp_unix: Optional[int]) -> Union[str, None]:
     """
     Converts a Unix timestamp to a human-readable string.
 
     Args:
         timestamp_unix: The Unix timestamp in milliseconds.
 
     Returns:
         A string representing the formatted date and time, or None if input is None.
     """
     if timestamp_unix is None:
         return None
     timestamp_seconds = timestamp_unix / 1000
     dt_object = datetime.fromtimestamp(timestamp_seconds)
-    return dt_object.strftime('%Y-%m-%d %H:%M:%S')
+    return dt_object.strftime("%Y-%m-%d %H:%M:%S")
+
+
+def ensure_directory(path):
+    """Ensure the directory exists, create it if it doesn't, then return the path."""
+    p = Path(path)
+    p.mkdir(parents=True, exist_ok=True)
+    return p
+
+
+def find_first_existing_directory(*paths):
+    """Return the first existing directory from a list of paths, or None if none exist."""
+    for path in paths:
+        if path:
+            p = Path(path)
+            if p.is_dir():
+                return p
+    return None
+
 
 def utc_to_local_time(timestamp_str: Optional[str]) -> str:
     """
     Converts a UTC timestamp string to local time string based on the TIMEZONE environment variable.
 
     Args:
         timestamp_str: The UTC timestamp string.
 
     Returns:
         The local time as a string.
     """
-    if timestamp_str is None or timestamp_str == 'No activity':
+    if timestamp_str is None or timestamp_str == "No activity":
         return timestamp_str
     try:
         timestamp_utc = datetime.strptime(timestamp_str.strip(), "%Y-%m-%dT%H:%M:%SZ")
     except ValueError:
         try:
-            timestamp_utc = datetime.strptime(timestamp_str.strip(), "%Y-%m-%dT%H:%M:%S.%f%z")
+            timestamp_utc = datetime.strptime(
+                timestamp_str.strip(), "%Y-%m-%dT%H:%M:%S.%f%z"
+            )
         except ValueError:
             try:
-                timestamp_utc = datetime.strptime(timestamp_str.strip(), "%Y-%m-%d %H:%M:%S %Z")
+                timestamp_utc = datetime.strptime(
+                    timestamp_str.strip(), "%Y-%m-%d %H:%M:%S %Z"
+                )
             except ValueError:
                 return timestamp_str
     local_tz = pytz.timezone(os.getenv("TIMEZONE", "UTC"))
     timestamp_local = timestamp_utc.replace(tzinfo=pytz.utc).astimezone(local_tz)
     return timestamp_local.strftime("%Y-%m-%d %H:%M:%S")
 
+
+def find_first_existing_file(*paths):
+    """Return the first existing file path from a list of paths."""
+    for path in paths:
+        if path:
+            p = Path(path)
+            if p.exists() and p.is_file():
+                return p
+    return None
+
+
 def csv_to_json(csv_file: str, json_file: str) -> None:
     """
     Converts data from a CSV file to a JSON file format.
 
     Args:
         csv_file: The file path of the CSV file.
         json_file: The file path for the output JSON file.
     """
-    with open(csv_file, newline='') as csvfile:
+    with open(csv_file, newline="") as csvfile:
         reader = csv.DictReader(csvfile)
         csv_data = list(reader)
 
-    with open(json_file, 'w') as jsonfile:
+    with open(json_file, "w") as jsonfile:
         json.dump(csv_data, jsonfile, indent=4)
 
+
 def get_current_time_in_timezone() -> datetime:
     """
     Returns the current time adjusted to the timezone specified by the 'TIMEZONE' environment variable.
     Defaults to UTC if 'TIMEZONE' is not set or if an unknown/problematic timezone is specified.
 
     Returns:
         A datetime object representing the current time in the specified (or default) timezone.
     """
     timezone_str: str = os.getenv("TIMEZONE", "UTC")
     try:
         timezone = pytz.timezone(timezone_str)
     except pytz.UnknownTimeZoneError:
-        print(f"Warning: Unknown timezone specified: '{timezone_str}'. Defaulting to UTC.")
+        print(
+            f"Warning: Unknown timezone specified: '{timezone_str}'. Defaulting to UTC."
+        )
         timezone = pytz.timezone("UTC")
 
     current_time_utc: datetime = datetime.utcnow()
-    current_time_utc = current_time_utc.replace(tzinfo=pytz.utc)  # Attach UTC timezone information
+    current_time_utc = current_time_utc.replace(
+        tzinfo=pytz.utc
+    )  # Attach UTC timezone information
     current_time_in_timezone: datetime = current_time_utc.astimezone(timezone)
-    return current_time_in_timezone
+    return current_time_in_timezone
```

### Comparing `avaris-0.1.0/PKG-INFO` & `avaris-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: avaris
-Version: 0.1.0
+Version: 0.1.4
 Summary: Task execution engine for data management and monitoring
 License: Apache-2.0
 Author: dennis
 Author-email: denngohis@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: apscheduler (>=3.10.4,<4.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: celery (>=5.3.6,<6.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: croniter (>=2.0.2,<3.0.0)
 Requires-Dist: databases (>=0.9.0,<0.10.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: python-dotenv[cli] (>=1.0.1,<2.0.0)
@@ -28,15 +30,15 @@
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.28,<3.0.0)
 Requires-Dist: uvicorn (>=0.27.1,<0.28.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: none">
-    <a href="//github.com/avyrion/avaris" target="_blank"><img alt="Avaris" src="etc/avaris.png"></a><br>Avaris Task Engine
+    <a href="//github.com/avyr-io/avaris" target="_blank"><img alt="Avaris" src="etc/avaris.png"></a><br>Avaris Task Engine
 </h1>
 
 <div align="center">
 
 </div>
 
 Avaris is a modular task execution and data processing engine designed for easy integration and customization for various task executions, with a strong focus on data management tasks.
@@ -50,62 +52,62 @@
 - **Extensible Executors:** Execute tasks based on predefined or custom logic.
 - **Data Management:** Introduces `SQLDataManager` for relational database management, in addition to customizable data managers and handlers for diverse data storage and processing needs.
 
 ## Installation
 
 ```bash
 # Clone the repository
-git clone https://github.com/avyrion/avaris.git
+git clone https://github.com/avyr-io/avaris.git
 cd avaris
 
 # Install requirements
 python -m pip install poetry
 poetry install
-python -m avaris start --config config/conf.yml --scraper-dir ./scrapers
+python -m avaris start --config config/conf.yml --compendium-dir ./compendium
 ```
 
 ## Getting Started
 
-To run Avaris, you'll need to specify your engine configuration and scraper directory. Here's a quick guide to get you started.
+To run Avaris, you'll need to specify your engine configuration and compendium directory. Here's a quick guide to get you started.
 
 ### Configuration Files
 
 Avaris requires two main types of configuration files:
 
 - **Engine Configuration (`config/conf.yml`):** Defines global settings for the Avaris avaris.engine.
-- **Scraper Configurations (`./scrapers`):** Each scraper should have its own configuration file in this directory, detailing tasks, endpoints, and data management settings.
+- **Compendium Configurations (`./compendium`):** Each compendium file should have its own configuration file in this directory, detailing tasks, endpoints, and data management settings.
 
 ### Running Avaris
 
 ```bash
-python -m avaris start --config config/conf.yml --scraper-dir ./scrapers
+python -m avaris start --config config/conf.yml --compendium-dir ./compendium
 ```
 
-Replace `config/conf.yml` and `./scrapers` with the paths to your actual engine configuration file and scraper configuration directory, respectively.
+Replace `config/conf.yml` and `./compendium` with the paths to your actual engine configuration file and compendium configuration directory, respectively.
 
 ## Examples
 
 Here are some examples of how to use Avaris for different tasks.
 
-### Defining a Scraper Configuration
+### Defining a compendium Configuration
 
 ```yaml
-# scraper_config.yml
-scraper:
-  - name: PrometheusVersionScraper
+# compendium_config.yml
+compendium:
+  - name: PrometheusVersioncompendium
     destination: local
     tasks:
       - name: FetchLatestPrometheusVersion
         schedule: "* * * * *"
         executor:
           task: http_get_github_release
           parameters:
             api_url: "https://api.github.com/repos/prometheus/prometheus/releases/latest"
 
-  - name: FluentBitVersionScraper
+  - name: FluentBitVersioncompendium
     destination: local
     tasks:
       - name: FetchLatestFluentBitVersion
         schedule: "* * * * *"
         executor:
           task: http_get_github_release
           parameters:
```

