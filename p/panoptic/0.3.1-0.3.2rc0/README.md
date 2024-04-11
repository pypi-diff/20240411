# Comparing `tmp/panoptic-0.3.1.tar.gz` & `tmp/panoptic-0.3.2rc0.tar.gz`

## Comparing `panoptic-0.3.1.tar` & `panoptic-0.3.2rc0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/__init__.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/main.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/test.py
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/utils.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/assets/arrow.png
--rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/__init__.py
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/exporter.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/importer.py
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/panoptic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/db/__init__.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/db/create.py
--rw-r--r--   0        0        0    20754 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/db/db.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/db/db_connection.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/db/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/__init__.py
--rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/project.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/project_actions.py
--rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/project_db.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/project_events.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/project/project_ui.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/task/__init__.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/task/import_image_task.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/task/load_plugin_task.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/task/task.py
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/core/task/task_queue.py
--rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/favicon.ico
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/index.html
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/HomeView-94ae33d3.css
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/HomeView-9dc56545.js
--rw-r--r--   0        0        0    49063 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/PanopticView-294e9cef.js
--rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/PanopticView-909fe1da.css
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/Tutorial-37229e07.css
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/Tutorial-3f379c82.js
--rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/bootstrap-icons-476adf42.woff2
--rw-r--r--   0        0        0   176032 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/bootstrap-icons-bb1de989.woff
--rw-r--r--   0        0        0   474970 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/index-03b204ca.css
--rw-r--r--   0        0        0   744587 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/html/assets/index-04947361.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/models/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/models/computed_properties.py
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/models/models.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/models/payloads.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/models/results.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/__init__.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute_vector_task.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/create_faiss_index.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/faiss_plugin.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/__init__.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/ocr.py
--rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/similarity.py
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/transform.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/utils.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/transformers/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/PluginBase/__init__.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/plugins/PluginBase/plugin_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/routes/__init__.py
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/routes/project_routes.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/routes/project_selection_routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/clean_db.sql
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/convert_old_db.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/convert_path.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/create_db.sql
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/create_prop_file.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/populate_db.sql
--rw-r--r--   0        0        0   321258 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/tmp.jpg
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 panoptic-0.3.1/panoptic/scripts/to_pca.py
--rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 panoptic-0.3.1/.gitignore
--rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 panoptic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 panoptic-0.3.1/../README.md
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 panoptic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/__init__.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/main.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/test.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/utils.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/assets/arrow.png
+-rw-r--r--   0        0        0    15332 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/exporter.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/importer.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/panoptic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/db/__init__.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/db/create.py
+-rw-r--r--   0        0        0    20754 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/db/db.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/db/db_connection.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/db/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/__init__.py
+-rw-r--r--   0        0        0     5592 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/project.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/project_actions.py
+-rw-r--r--   0        0        0    14721 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/project_db.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/project_events.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/project/project_ui.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/task/__init__.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/task/import_image_task.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/task/load_plugin_task.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/task/task.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/core/task/task_queue.py
+-rw-r--r--   0        0        0    67646 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/favicon.ico
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/index.html
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/HomeView-94ae33d3.css
+-rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/HomeView-9dc56545.js
+-rw-r--r--   0        0        0    49063 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/PanopticView-294e9cef.js
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/PanopticView-909fe1da.css
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/Tutorial-37229e07.css
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/Tutorial-3f379c82.js
+-rw-r--r--   0        0        0   130396 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/bootstrap-icons-476adf42.woff2
+-rw-r--r--   0        0        0   176032 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/bootstrap-icons-bb1de989.woff
+-rw-r--r--   0        0        0   474970 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/index-03b204ca.css
+-rw-r--r--   0        0        0   744587 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/html/assets/index-04947361.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/models/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/models/computed_properties.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/models/models.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/models/payloads.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/models/results.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/__init__.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute_vector_task.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/create_faiss_index.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/faiss_plugin.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/__init__.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/ocr.py
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/similarity.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/transform.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/utils.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/transformers/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/PluginBase/__init__.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/plugins/PluginBase/plugin_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/routes/__init__.py
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/routes/project_routes.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/routes/project_selection_routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/clean_db.sql
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/convert_old_db.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/convert_path.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/create_db.sql
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/create_prop_file.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/populate_db.sql
+-rw-r--r--   0        0        0   321258 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/tmp.jpg
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/panoptic/scripts/to_pca.py
+-rw-r--r--   0        0        0     3558 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/.gitignore
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/pyproject.toml
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/../README.md
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 panoptic-0.3.2rc0/PKG-INFO
```

### Comparing `panoptic-0.3.1/panoptic/main.py` & `panoptic-0.3.2rc0/panoptic/main.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugin.py` & `panoptic-0.3.2rc0/panoptic/plugin.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/utils.py` & `panoptic-0.3.2rc0/panoptic/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/__init__.py` & `panoptic-0.3.2rc0/panoptic/core/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/exporter.py` & `panoptic-0.3.2rc0/panoptic/core/exporter.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/importer.py` & `panoptic-0.3.2rc0/panoptic/core/importer.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/panoptic.py` & `panoptic-0.3.2rc0/panoptic/core/panoptic.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/db/create.py` & `panoptic-0.3.2rc0/panoptic/core/db/create.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/db/db.py` & `panoptic-0.3.2rc0/panoptic/core/db/db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/db/db_connection.py` & `panoptic-0.3.2rc0/panoptic/core/db/db_connection.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/project/project.py` & `panoptic-0.3.2rc0/panoptic/core/project/project.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/project/project_actions.py` & `panoptic-0.3.2rc0/panoptic/core/project/project_actions.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/project/project_db.py` & `panoptic-0.3.2rc0/panoptic/core/project/project_db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/project/project_ui.py` & `panoptic-0.3.2rc0/panoptic/core/project/project_ui.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/task/import_image_task.py` & `panoptic-0.3.2rc0/panoptic/core/task/import_image_task.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/task/load_plugin_task.py` & `panoptic-0.3.2rc0/panoptic/core/task/load_plugin_task.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/task/task.py` & `panoptic-0.3.2rc0/panoptic/core/task/task.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/core/task/task_queue.py` & `panoptic-0.3.2rc0/panoptic/core/task/task_queue.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/favicon.ico` & `panoptic-0.3.2rc0/panoptic/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/HomeView-94ae33d3.css` & `panoptic-0.3.2rc0/panoptic/html/assets/HomeView-94ae33d3.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/HomeView-9dc56545.js` & `panoptic-0.3.2rc0/panoptic/html/assets/HomeView-9dc56545.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/PanopticView-294e9cef.js` & `panoptic-0.3.2rc0/panoptic/html/assets/PanopticView-294e9cef.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/PanopticView-909fe1da.css` & `panoptic-0.3.2rc0/panoptic/html/assets/PanopticView-909fe1da.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/Tutorial-37229e07.css` & `panoptic-0.3.2rc0/panoptic/html/assets/Tutorial-37229e07.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/Tutorial-3f379c82.js` & `panoptic-0.3.2rc0/panoptic/html/assets/Tutorial-3f379c82.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/bootstrap-icons-476adf42.woff2` & `panoptic-0.3.2rc0/panoptic/html/assets/bootstrap-icons-476adf42.woff2`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/bootstrap-icons-bb1de989.woff` & `panoptic-0.3.2rc0/panoptic/html/assets/bootstrap-icons-bb1de989.woff`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/index-03b204ca.css` & `panoptic-0.3.2rc0/panoptic/html/assets/index-03b204ca.css`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/html/assets/index-04947361.js` & `panoptic-0.3.2rc0/panoptic/html/assets/index-04947361.js`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/models/computed_properties.py` & `panoptic-0.3.2rc0/panoptic/models/computed_properties.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/models/models.py` & `panoptic-0.3.2rc0/panoptic/models/models.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/models/payloads.py` & `panoptic-0.3.2rc0/panoptic/models/payloads.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/models/results.py` & `panoptic-0.3.2rc0/panoptic/models/results.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute_vector_task.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute_vector_task.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/faiss_plugin.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/faiss_plugin.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/ocr.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/ocr.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/similarity.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/similarity.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/transform.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/transform.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/utils.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/utils.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/FaissPlugin/compute/transformers/__init__.py` & `panoptic-0.3.2rc0/panoptic/plugins/FaissPlugin/compute/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/plugins/PluginBase/plugin_base.py` & `panoptic-0.3.2rc0/panoptic/plugins/PluginBase/plugin_base.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/routes/project_routes.py` & `panoptic-0.3.2rc0/panoptic/routes/project_routes.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/routes/project_selection_routes.py` & `panoptic-0.3.2rc0/panoptic/routes/project_selection_routes.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/convert_old_db.py` & `panoptic-0.3.2rc0/panoptic/scripts/convert_old_db.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/convert_path.py` & `panoptic-0.3.2rc0/panoptic/scripts/convert_path.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/create_db.sql` & `panoptic-0.3.2rc0/panoptic/scripts/create_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/create_prop_file.py` & `panoptic-0.3.2rc0/panoptic/scripts/create_prop_file.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/populate_db.sql` & `panoptic-0.3.2rc0/panoptic/scripts/populate_db.sql`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/tmp.jpg` & `panoptic-0.3.2rc0/panoptic/scripts/tmp.jpg`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/panoptic/scripts/to_pca.py` & `panoptic-0.3.2rc0/panoptic/scripts/to_pca.py`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/.gitignore` & `panoptic-0.3.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/pyproject.toml` & `panoptic-0.3.2rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
     "aiofiles",
     "aiosqlite",
     "faiss-cpu",
-    "fastapi",
-    "fastapi-camelcase",
+    "fastapi==0.99.1",
+    "fastapi-camelcase==1.0.5",
     "imagehash",
     "numpy",
     "orjson",
     "pandas",
     "psutil",
     "pydantic",
     "pypika",
```

### Comparing `panoptic-0.3.1/../README.md` & `panoptic-0.3.2rc0/../README.md`

 * *Files identical despite different names*

### Comparing `panoptic-0.3.1/PKG-INFO` & `panoptic-0.3.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panoptic
-Version: 0.3.1
+Version: 0.3.2rc0
 Summary: Explore and analyze large datasets of images
 Project-URL: Repository, https://github.com/CERES-Sorbonne/panoptic
 Project-URL: Documentation, https://github.com/CERES-Sorbonne/panoptic#readme
 Project-URL: Issues, https://github.com/CERES-Sorbonne/panoptic/issues
 Project-URL: Lab's website, https://ceres.sorbonne-universite.fr/
 License-Expression: MPL-2.0
 Keywords: Data visualization,Image analysis,Image clustering,Image corpora,Machine learning,Web application
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: aiofiles
 Requires-Dist: aiosqlite
 Requires-Dist: faiss-cpu
-Requires-Dist: fastapi
-Requires-Dist: fastapi-camelcase
+Requires-Dist: fastapi-camelcase==1.0.5
+Requires-Dist: fastapi==0.99.1
 Requires-Dist: imagehash
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: pydantic
 Requires-Dist: pypika
```

