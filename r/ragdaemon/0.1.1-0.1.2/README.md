# Comparing `tmp/ragdaemon-0.1.1.tar.gz` & `tmp/ragdaemon-0.1.2.tar.gz`

## Comparing `ragdaemon-0.1.1.tar` & `ragdaemon-0.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/app.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/context.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/errors.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/llm.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/test_context.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/test_daemon.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/test_database.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/test_sample.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/LICENSE
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/README.md
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 ragdaemon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/app.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/context.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/errors.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     5432 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_context.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_daemon.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_database.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/test_sample.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/README.md
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 ragdaemon-0.1.2/PKG-INFO
```

### Comparing `ragdaemon-0.1.1/.github/workflows/run-tests.yml` & `ragdaemon-0.1.2/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/app.py` & `ragdaemon-0.1.2/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/context.py` & `ragdaemon-0.1.2/ragdaemon/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 from pathlib import Path
 from typing import Any
 
 import networkx as nx
 
 from ragdaemon.annotators.diff import parse_diff_id
-from ragdaemon.database import get_db
+from ragdaemon.database import Database
 from ragdaemon.utils import parse_path_ref
 
 
 class ContextBuilder:
     """Renders items from a graph into an llm-readable string."""
 
-    def __init__(self, graph: nx.MultiDiGraph, verbose: bool = False):
+    def __init__(self, graph: nx.MultiDiGraph, db: Database, verbose: bool = False):
         self.graph = graph
+        self.db = db
         self.verbose = verbose
         self.context = dict[
             str, dict[str, Any]
         ]()  # {path: {lines, tags, document, diff}}
 
     def _add_path(self, path_str: str):
         """Create a new record in the context for the given path."""
         cwd = self.graph.graph["cwd"]
         if path_str not in self.graph:  # e.g. deleted file
             document = ""
         else:
             checksum = self.graph.nodes[path_str]["checksum"]
-            document = get_db(cwd).get(checksum)["documents"][0]
+            document = self.db.get(checksum)["documents"][0]
         message = {
             "lines": set(),
             "tags": set(),
             "document": document,
             "diffs": set(),
         }
         self.context[path_str] = message
@@ -117,15 +118,15 @@
         git_command = "--git diff"
         if diff_str != "DEFAULT":
             git_command += f" {diff_str}"
         output += f"{git_command}\n"
         cwd = self.graph.graph["cwd"]
         for id in sorted(ids):
             checksum = self.graph.nodes[id]["checksum"]
-            document = get_db(cwd).get(checksum)["documents"][0]
+            document = self.db.get(checksum)["documents"][0]
             # TODO: Add line numbers
             without_git_command = "\n".join(document.splitlines()[1:])
             output += without_git_command + "\n"
         return output
 
     def to_refs(self) -> list[str]:
         """Return a list of path:interval,interval for everything in current context."""
```

### Comparing `ragdaemon-0.1.1/ragdaemon/daemon.py` & `ragdaemon-0.1.2/ragdaemon/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Optional
 
 import networkx as nx
 from spice import Spice
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
-from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, get_db, set_db
+from ragdaemon.database import Database, DEFAULT_EMBEDDING_MODEL, get_db
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL, token_counter
 from ragdaemon.utils import get_non_gitignored_files
 
 
 def default_annotators():
     return {
         "hierarchy": {},
@@ -22,14 +22,15 @@
     }
 
 
 class Daemon:
     """Build and maintain a searchable knowledge graph of codebase."""
 
     graph: nx.MultiDiGraph
+    db: Database = None
 
     def __init__(
         self,
         cwd: Path,
         annotators: Optional[dict[str, dict]] = None,
         verbose: bool = False,
         graph_path: Optional[Path] = None,
@@ -45,20 +46,14 @@
         if spice_client is None:
             spice_client = Spice(
                 default_text_model=DEFAULT_COMPLETION_MODEL,
                 default_embeddings_model=DEFAULT_EMBEDDING_MODEL,
             )
         self.spice_client = spice_client
 
-        # Establish a dedicated database client for this instance
-        set_db(self.cwd, spice_client=spice_client)
-        count = get_db(Path(self.cwd)).count()
-        if self.verbose:
-            print(f"Initialized database with {count} records.")
-
         # Initialize an empty graph
         self.graph = nx.MultiDiGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
         annotators = annotators if annotators is not None else default_annotators()
@@ -77,19 +72,24 @@
         with open(self.graph_path, "w") as f:
             json.dump(data, f, indent=4)
         if self.verbose:
             print(f"Saved updated graph to {self.graph_path}")
 
     async def update(self, refresh=False):
         """Iteratively build the knowledge graph"""
+
+        # Establish a dedicated database client for this instance
+        if self.db is None:
+            self.db = get_db(self.cwd, spice_client=self.spice_client)
+
         _graph = self.graph.copy()
         self.graph.graph["refreshing"] = True
         for annotator in self.pipeline.values():
-            if refresh or not annotator.is_complete(_graph):
-                _graph = await annotator.annotate(_graph, refresh=refresh)
+            if refresh or not annotator.is_complete(_graph, self.db):
+                _graph = await annotator.annotate(_graph, self.db, refresh=refresh)
         self.graph = _graph
         self.save()
 
     async def watch(self, interval=2, debounce=5):
         """Calls self.update interval debounce seconds after a file is modified."""
         git_paths = get_non_gitignored_files(self.cwd)
         last_updated = 0
@@ -109,25 +109,25 @@
                     except asyncio.CancelledError:
                         pass
                 last_updated = _last_updated
                 _update_task = asyncio.create_task(self.update())
 
     def search(self, query: str, n: Optional[int] = None) -> list[dict[str, Any]]:
         """Return a sorted list of nodes that match the query."""
-        return get_db(self.cwd).query_graph(query, self.graph, n=n)
+        return self.db.query_graph(query, self.graph, n=n)
 
     def get_context(
         self,
         query: str,
         context_builder: Optional[ContextBuilder] = None,
         max_tokens: int = 8000,
         auto_tokens: int = 0,
-    ):
+    ) -> ContextBuilder:
         if context_builder is None:
-            context = ContextBuilder(self.graph, self.verbose)
+            context = ContextBuilder(self.graph, self.db, self.verbose)
         else:
             # TODO: Compare graph hashes, reconcile changes
             context = context_builder
         include_context_message = context.render()
         include_tokens = token_counter(include_context_message)
         if not auto_tokens or include_tokens >= max_tokens:
             return context
```

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.2/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.2/ragdaemon/annotators/chunker.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import json
 from pathlib import Path
 
 import networkx as nx
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import get_db
+from ragdaemon.database import Database
 from ragdaemon.utils import get_document, hash_str
 
 
 def is_chunk_valid(chunk: dict) -> bool:
     # Includes the correct fields
     if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
         return False
@@ -39,15 +39,15 @@
         return False
     # TODO: Validate the ref, i.e. a parent chunk exists
 
     return True
 
 
 async def get_file_chunk_data(
-    cwd, node, data, chunk_function: callable, verbose: bool = False
+    cwd, node, data, chunk_function: callable, db: Database, verbose: bool = False
 ) -> list[dict]:
     """Get or add chunk data to database, load into file data"""
     file_lines = (cwd / Path(node)).read_text().splitlines()
     if len(file_lines) == 0:
         chunks = []
     else:
         chunks = await chunk_function(node, file_lines, verbose)
@@ -83,24 +83,25 @@
             {
                 "id": chunk["id"],
                 "ref": f"{node}:{chunk['start_line']}-{chunk['end_line']}",
             }
             for chunk in chunks
         ] + [base_chunk]
     # Save to db and graph
-    metadatas = get_db(cwd).get(data["checksum"])["metadatas"][0]
+    metadatas = db.get(data["checksum"])["metadatas"][0]
     metadatas["chunks"] = json.dumps(chunks)
-    get_db(cwd).update(data["checksum"], metadatas=metadatas)
+    db.update(data["checksum"], metadatas=metadatas)
     data["chunks"] = chunks
 
 
 def add_file_chunks_to_graph(
     file: str,
     data: dict,
     graph: nx.MultiDiGraph,
+    db: Database,
     refresh: bool = False,
     verbose: bool = False,
 ) -> dict[str:list]:
     """Load chunks from file data into db/graph"""
     cwd = Path(graph.graph["cwd"])
     add_to_db = {"ids": [], "documents": [], "metadatas": []}
     if not isinstance(data["chunks"], list):
@@ -114,15 +115,15 @@
     for chunk in chunks:
         try:
             # Get the checksum record from database
             id = chunk["id"]
             ref = chunk["ref"]
             document = get_document(ref, cwd)
             checksum = hash_str(document)
-            records = get_db(cwd).get(checksum)["metadatas"]
+            records = db.get(checksum)["metadatas"]
             if not refresh and len(records) > 0:
                 record = records[0]
             else:
                 record = {
                     "id": id,
                     "type": "chunk",
                     "ref": chunk["ref"],
@@ -183,15 +184,15 @@
                 ".ts",
                 ".jsx",
                 ".tsx",
                 ".scss",
             ]
         self.chunk_extensions = chunk_extensions
 
-    def is_complete(self, graph: nx.MultiDiGraph) -> bool:
+    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
         for _, data in graph.nodes(data=True):
             if data.get("type") != "file":
                 continue
             chunks = data.get("chunks", None)
             if chunks is None:
                 if self.chunk_extensions is None:
                     return False
@@ -219,15 +220,15 @@
             id (str): The complete call path, e.g. `path/to/file:class.method`
             start_line (int): Where the function, class or method begins
             end_line (int): Where it ends - INCLUSIVE
         """
         raise NotImplementedError()
 
     async def annotate(
-        self, graph: nx.MultiDiGraph, refresh: bool = False
+        self, graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
     ) -> nx.MultiDiGraph:
         # Remove any existing chunk nodes from the graph
         for node, data in graph.nodes(data=True):
             if data.get("type") == "chunk":
                 graph.remove_node(node)
 
         cwd = Path(graph.graph["cwd"])
@@ -244,26 +245,26 @@
             ]
         # Generate/add chunk data to file nodes
         tasks = []
         for node, data in file_nodes:
             if refresh or data.get("chunks", None) is None:
                 tasks.append(
                     get_file_chunk_data(
-                        cwd, node, data, self.chunk_file, verbose=self.verbose
+                        cwd, node, data, self.chunk_file, db, verbose=self.verbose
                     )
                 )
         if len(tasks) > 0:
             if self.verbose:
                 await tqdm.gather(*tasks, desc="Chunking files...")
             else:
                 await asyncio.gather(*tasks)
         # Load/Create chunk nodes into database and graph
         add_to_db = {"ids": [], "documents": [], "metadatas": []}
         for file, data in file_nodes:
             _add_to_db = add_file_chunks_to_graph(
-                file, data, graph, verbose=self.verbose
+                file, data, graph, db, verbose=self.verbose
             )
             for field, values in _add_to_db.items():
                 add_to_db[field].extend(values)
         if len(add_to_db["ids"]) > 0:
-            get_db(cwd).upsert(**add_to_db)
+            db.upsert(**add_to_db)
         return graph
```

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.2/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.2/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.2/ragdaemon/annotators/diff.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import json
 import re
 from pathlib import Path
 
 import networkx as nx
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import get_db
+from ragdaemon.database import (
+    DEFAULT_EMBEDDING_MODEL,
+    Database,
+    MAX_TOKENS_PER_EMBEDDING,
+)
 from ragdaemon.errors import RagdaemonError
+from ragdaemon.llm import token_counter
 from ragdaemon.utils import get_document, hash_str, parse_path_ref
 
 
 def get_chunks_from_diff(id: str, diff: str) -> list[dict[str, str]]:
     # Match files and line numbers
     file_regex = re.compile(r"^diff --git a/(.+) b/(.+)$")
     hunk_header_regex = re.compile(r"^@@ -\d+,\d+ \+(\d+),(\d+) @@.*$")
@@ -58,66 +63,80 @@
         path, lines = parse_path_ref(path_ref)
     else:
         diff_ref, path, lines = id, None, None
     return diff_ref, path, lines
 
 
 class Diff(Annotator):
-    name: str = "base_annotator"
+    name: str = "diff"
 
     def __init__(self, *args, diff: str = "", **kwargs):
         if ":" in diff:
             raise RagdaemonError("diff cannot contain ':'")
         super().__init__(*args, **kwargs)
         self.diff_args = diff
 
     @property
     def id(self) -> str:
         return "DEFAULT" if not self.diff_args else self.diff_args
 
-    def is_complete(self, graph: nx.MultiDiGraph) -> bool:
+    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
         cwd = graph.graph["cwd"]
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         return self.id in graph and graph.nodes[self.id]["checksum"] == checksum
 
     async def annotate(
-        self, graph: nx.MultiDiGraph, refresh: bool = False
+        self, graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
     ) -> nx.MultiDiGraph:
         graph_nodes = {
             node for node, data in graph.nodes(data=True) if data.get("type") == "diff"
         }
         graph.remove_nodes_from(graph_nodes)
         cwd = graph.graph["cwd"]
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
-        existing_records = get_db(cwd).get(checksum)
+        existing_records = db.get(checksum)
         if refresh or len(existing_records["ids"]) == 0:
             chunks = get_chunks_from_diff(id=self.id, diff=document)
             data = {
                 "id": self.id,
                 "ref": self.diff_args,
                 "type": "diff",
                 "checksum": checksum,
                 "chunks": json.dumps(chunks),
                 "active": False,
             }
-            get_db(cwd).upsert(ids=checksum, documents=document, metadatas=data)
+
+            # If the full diff is too long to embed, it is truncated. Anything
+            # removed will be captured in chunks.
+            tokens = token_counter(
+                document, model=DEFAULT_EMBEDDING_MODEL, full_message=False
+            )
+            if tokens > MAX_TOKENS_PER_EMBEDDING:
+                truncate_ratio = (MAX_TOKENS_PER_EMBEDDING / tokens) * 0.99
+                document = document[: int(len(document) * truncate_ratio)]
+                if self.verbose:
+                    print(
+                        f"Truncated full diff by {1 - truncate_ratio:.2%} for embedding."
+                    )
+
+            db.upsert(ids=checksum, documents=document, metadatas=data)
         else:
             data = existing_records["metadatas"][0]
         data["chunks"] = json.loads(data["chunks"])
         graph.add_node(self.id, **data)
 
         # Add chunks
         add_to_db = {"ids": [], "documents": [], "metadatas": []}
         edges_to_add = set()
         for chunk_id, chunk_ref in data["chunks"].items():
             document = get_document(chunk_ref, cwd, type="diff")
             chunk_checksum = hash_str(document)
-            existing_records = get_db(cwd).get(chunk_checksum)
+            existing_records = db.get(chunk_checksum)
             if refresh or len(existing_records["ids"]) == 0:
                 data = {
                     "id": chunk_id,
                     "ref": chunk_ref,
                     "type": "diff",
                     "checksum": chunk_checksum,
                     "active": False,
@@ -154,10 +173,10 @@
                     _link_to_successors(successor, visited)
 
             _link_to_successors(file_str)
 
         for source, origin in edges_to_add:
             graph.add_edge(source, origin, type="diff")
         if len(add_to_db["ids"]) > 0:
-            get_db(cwd).upsert(**add_to_db)
+            db.upsert(**add_to_db)
 
         return graph
```

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.2/ragdaemon/annotators/hierarchy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import fnmatch
 from pathlib import Path
 
 import networkx as nx
 
 from ragdaemon.annotators.base_annotator import Annotator
-from ragdaemon.database import MAX_TOKENS_PER_EMBEDDING, get_db
+from ragdaemon.database import MAX_TOKENS_PER_EMBEDDING, Database
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.llm import token_counter
 from ragdaemon.utils import get_document, get_non_gitignored_files, hash_str
 
 
 def match_path_with_patterns(path: Path, cwd: Path, patterns: list[str] = []) -> bool:
     """Check if the given absolute path matches any of the patterns.
@@ -33,14 +33,15 @@
         if path.is_relative_to(pattern):
             return True
     return False
 
 
 def get_active_checksums(
     cwd: Path,
+    db: Database,
     refresh: bool = False,
     verbose: bool = False,
     ignore_patterns: list[str] = [],
 ) -> dict[Path:str]:
     checksums: dict[Path:str] = {}
     git_paths = get_non_gitignored_files(cwd)
     add_to_db = {
@@ -55,15 +56,15 @@
             path_str = path.as_posix()
             ref = path_str
             document = get_document(ref, cwd)
             tokens = token_counter(document)
             if tokens > MAX_TOKENS_PER_EMBEDDING:  # e.g. package-lock.json
                 continue
             checksum = hash_str(document)
-            existing_record = len(get_db(cwd).get(checksum)["ids"]) > 0
+            existing_record = len(db.get(checksum)["ids"]) > 0
             if refresh or not existing_record:
                 # add new items to db (will generate embeddings)
                 metadatas = {
                     "id": path_str,
                     "type": "file",
                     "ref": ref,
                     "checksum": checksum,
@@ -75,54 +76,65 @@
             checksums[path] = checksum
         except UnicodeDecodeError:  # Ignore non-text files
             pass
         except RagdaemonError as e:
             if verbose:
                 print(f"Error processing path {path}: {e}")
     if len(add_to_db["ids"]) > 0:
-        get_db(cwd).upsert(**add_to_db)
+        db.upsert(**add_to_db)
     return checksums
 
 
+def files_checksum(cwd: Path, ignore_patterns: list[str] = []) -> str:
+    timestamps = ""
+    for path in get_non_gitignored_files(cwd):
+        if match_path_with_patterns(path, cwd, ignore_patterns):
+            continue
+        try:
+            timestamps += str(path.stat().st_mtime)
+        except FileNotFoundError:
+            pass
+    return hash_str(timestamps)
+
+
 class Hierarchy(Annotator):
     name = "hierarchy"
 
     def __init__(self, *args, ignore_patterns: list[str] = [], **kwargs):
         self.ignore_patterns = ignore_patterns
         super().__init__(*args, **kwargs)
 
-    def is_complete(self, graph: nx.MultiDiGraph) -> bool:
+    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
         cwd = Path(graph.graph["cwd"])
-        checksums = get_active_checksums(
-            cwd, verbose=self.verbose, ignore_patterns=self.ignore_patterns
+        return graph.graph.get("files_checksum") == files_checksum(
+            cwd, self.ignore_patterns
         )
-        files_checksum = hash_str("".join(sorted(checksums.values())))
-        return graph.graph.get("files_checksum") == files_checksum
 
     async def annotate(
-        self, old_graph: nx.MultiDiGraph, refresh: bool = False
+        self, old_graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
     ) -> nx.MultiDiGraph:
         """Build a graph of active files and directories with hierarchy edges."""
         cwd = Path(old_graph.graph["cwd"])
         checksums = get_active_checksums(
             cwd,
+            db,
             refresh=refresh,
             verbose=self.verbose,
             ignore_patterns=self.ignore_patterns,
         )
-        files_checksum = hash_str("".join(sorted(checksums.values())))
+        _files_checksum = files_checksum(cwd, self.ignore_patterns)
 
         # Initialize an empty graph. We'll build it from scratch.
         graph = nx.MultiDiGraph()
         graph.graph["cwd"] = str(cwd)
         edges_to_add = set()
         for path, checksum in checksums.items():
             # add db reecord
             id = path.as_posix()
-            results = get_db(cwd).get(checksum)
+            results = db.get(checksum)
             data = results["metadatas"][0]
             graph.add_node(id, **data)
 
             # add hierarchy edges
             def _link_to_cwd(_path: Path):
                 _parent = _path.parent.as_posix() if len(_path.parts) > 1 else "ROOT"
                 edges_to_add.add((_parent, _path.as_posix()))
@@ -136,9 +148,9 @@
             for id in (source, target):
                 if id not in graph:
                     # add directories to graph (to link hierarchy) but not db
                     record = {"id": id, "type": "directory", "ref": id}
                     graph.add_node(id, **record)
             graph.add_edge(source, target, type="hierarchy")
 
-        graph.graph["files_checksum"] = files_checksum
+        graph.graph["files_checksum"] = _files_checksum
         return graph
```

### Comparing `ragdaemon-0.1.1/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.2/ragdaemon/annotators/layout_hierarchy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import networkx as nx
 import numpy as np
 from tqdm import tqdm
 
+from ragdaemon.database import Database
 from ragdaemon.annotators.base_annotator import Annotator
 
 
 def fruchterman_reingold_3d(
     G,
     iterations=40,
     repulsive_force=0.2,
@@ -79,24 +80,25 @@
         for node in G.nodes()
     }
 
 
 class LayoutHierarchy(Annotator):
     name = "layout_hierarchy"
 
-    def is_complete(self, graph: nx.MultiDiGraph) -> bool:
+    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
         # Check that they have data.layout.hierarchy
         for _, data in graph.nodes(data=True):
             if not data.get("layout", {}).get("hierarchy"):
                 return False
         return True
 
     async def annotate(
         self,
         graph: nx.MultiDiGraph,
+        db: Database = None,
         refresh: bool = False,
         iterations: int = 40,
     ) -> nx.MultiDiGraph:
         """
         a. Regenerate x/y/z for all nodes
         b. Update all nodes
         c. Save to chroma
```

### Comparing `ragdaemon-0.1.1/ragdaemon/database/__init__.py` & `ragdaemon-0.1.2/ragdaemon/database/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 import os
-from contextvars import ContextVar
 from pathlib import Path
 
 from spice import Spice, SpiceError
 
 from ragdaemon.database.database import Database
 from ragdaemon.database.chroma_database import ChromaDB
 from ragdaemon.database.lite_database import LiteDB
 from ragdaemon.utils import mentat_dir_path
 
 MAX_TOKENS_PER_EMBEDDING = 8192
 DEFAULT_EMBEDDING_MODEL = "text-embedding-ada-002"
 
 
-_db: ContextVar = ContextVar("_db", default=None)
-
-
-def set_db(cwd: Path, spice_client: Spice):
-    global _db
+def get_db(cwd: Path, spice_client: Spice) -> Database:
     db_path = mentat_dir_path / "chroma"
     db_path.mkdir(parents=True, exist_ok=True)
     if "PYTEST_CURRENT_TEST" not in os.environ:
         try:
-            _db.set(ChromaDB(cwd=cwd, db_path=db_path, spice_client=spice_client))
-            return
+            return ChromaDB(cwd=cwd, db_path=db_path, spice_client=spice_client)
         except SpiceError:
             pass
-    _db.set(LiteDB(cwd=cwd, db_path=db_path))
-
-
-def get_db(cwd: Path) -> Database:
-    global _db
-    db = _db.get()
-    if db is None:
-        set_db(cwd)
-        db = _db.get()
-    return db
+    return LiteDB(cwd=cwd, db_path=db_path)
```

### Comparing `ragdaemon-0.1.1/ragdaemon/database/database.py` & `ragdaemon-0.1.2/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.2/ragdaemon/database/lite_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from pathlib import Path
 from typing import Any
 
 from ragdaemon.database.database import Database
 from ragdaemon.utils import parse_path_ref
 
-MAX_TOKENS_PER_EMBEDDING = 8192
-
 
 class LiteDB(Database):
     def __init__(self, cwd: Path, db_path: Path):
         self.cwd = cwd
         self.db_path = db_path
         self._collection = LiteCollection()
```

### Comparing `ragdaemon-0.1.1/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.2/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.2/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/static/js/main.js` & `ragdaemon-0.1.2/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.2/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.2/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.2/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/ragdaemon/templates/index.html` & `ragdaemon-0.1.2/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/conftest.py` & `ragdaemon-0.1.2/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import subprocess
 import tempfile
 from pathlib import Path
 from unittest.mock import AsyncMock, patch
 
 import pytest
 
-from ragdaemon.database import set_db
+from ragdaemon.database import get_db
 
 
 @pytest.fixture
 def cwd():
     return Path("tests/sample")
 
 
 @pytest.fixture
-def mock_set_db(cwd):
-    set_db(cwd, AsyncMock())
+def mock_db(cwd):
+    return get_db(cwd, spice_client=AsyncMock())
 
 
 @pytest.fixture
 def mock_get_llm_response():
     with patch(
         "ragdaemon.annotators.chunker_llm.ChunkerLLM.get_llm_response",
         return_value={"chunks": []},
```

### Comparing `ragdaemon-0.1.1/tests/test_context.py` & `ragdaemon-0.1.2/tests/test_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import networkx as nx
 
 from ragdaemon.context import ContextBuilder
 from ragdaemon.utils import get_document
 
 
-def test_daemon_render_context(cwd):
+def test_daemon_render_context(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Base Chunk
-    context = ContextBuilder(nx.MultiDiGraph())
+    context = ContextBuilder(nx.MultiDiGraph(), mock_db)
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
         }
@@ -61,20 +61,20 @@
 13:        raise ValueError("Invalid operation")
 14:    return int(match.group(1)), match.group(2), int(match.group(3))
 ...
 """
     )
 
 
-def test_to_refs(cwd):
+def test_to_refs(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Setup Context
-    context = ContextBuilder(nx.MultiDiGraph())
+    context = ContextBuilder(nx.MultiDiGraph(), mock_db)
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
         }
```

### Comparing `ragdaemon-0.1.1/tests/test_daemon.py` & `ragdaemon-0.1.2/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/test_sample.py` & `ragdaemon-0.1.2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/annotators/test_chunker.py` & `ragdaemon-0.1.2/tests/annotators/test_chunker.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     with open("tests/data/chunker_graph.json", "r") as f:
         data = json.load(f)
         chunker_graph = nx.readwrite.json_graph.node_link_graph(data)
     assert chunker.is_complete(chunker_graph), "Chunker graph should be complete."
 
 
 @pytest.mark.asyncio
-async def test_chunker_llm_annotate(cwd, mock_get_llm_response):
+async def test_chunker_llm_annotate(cwd, mock_get_llm_response, mock_db):
     daemon = Daemon(
         cwd=cwd,
         annotators={"hierarchy": {}},
         graph_path=(Path.cwd() / "tests/data/hierarchy_graph.json"),
     )
     chunker = ChunkerLLM(spice_client=AsyncMock())
-    actual = await chunker.annotate(daemon.graph)
+    actual = await chunker.annotate(daemon.graph, mock_db)
 
     for node, data in actual.nodes(data=True):
         if data["type"] == "file" and Path(node).suffix in chunker.chunk_extensions:
             assert "chunks" in data, f"File {node} is missing chunks"
```

### Comparing `ragdaemon-0.1.1/tests/annotators/test_diff.py` & `ragdaemon-0.1.2/tests/annotators/test_diff.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,38 +30,38 @@
         actual_ref, actual_path, actual_lines = parse_diff_id(id)
         assert actual_ref == expected_ref
         assert str(actual_path) == expected_path
         assert actual_lines == expected_lines
 
 
 @pytest.mark.asyncio
-async def test_diff_annotate(git_history, mock_set_db):
+async def test_diff_annotate(git_history, mock_db):
     with open("tests/data/chunker_graph.json", "r") as f:
         data = json.load(f)
         graph = nx.readwrite.json_graph.node_link_graph(data)
     graph.graph["cwd"] = git_history.as_posix()
     annotator = Diff()
-    actual = await annotator.annotate(graph)
+    actual = await annotator.annotate(graph, mock_db)
     actual_nodes = {n for n, d in actual.nodes(data=True) if d["type"] == "diff"}
 
     with open("tests/data/diff_graph.json", "r") as f:
         data = json.load(f)
         expected = nx.readwrite.json_graph.node_link_graph(data)
     expected_nodes = {n for n, d in expected.nodes(data=True) if d["type"] == "diff"}
 
     assert actual_nodes == expected_nodes
 
 
 @pytest.mark.asyncio
-async def test_diff_render(git_history):
+async def test_diff_render(git_history, mock_db):
     daemon = Daemon(cwd=git_history)
     await daemon.update(refresh=True)
 
     # Only diffs
-    context = ContextBuilder(graph=daemon.graph)
+    context = ContextBuilder(daemon.graph, daemon.db)
     context.add_diff("DEFAULT:main.py")
     context.add_diff("DEFAULT:src/operations.py:1-5")
     context.add_diff("DEFAULT:src/operations.py:8-10")
     actual = context.render()
     assert (
         actual
         == """\
```

### Comparing `ragdaemon-0.1.1/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.2/tests/annotators/test_hierarchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import networkx as nx
 import pytest
 
 from ragdaemon.annotators.hierarchy import Hierarchy, get_active_checksums
 
 
-def test_get_active_checksums(cwd):
-    checksums = get_active_checksums(cwd)
+def test_get_active_checksums(cwd, mock_db):
+    checksums = get_active_checksums(cwd, mock_db)
     assert isinstance(checksums, dict), "Checksums is not a dict"
     assert all(isinstance(k, Path) for k in checksums), "Keys are not all Paths"
     assert all(
         isinstance(v, str) for v in checksums.values()
     ), "Values are not all strings"
 
     with open("tests/data/hierarchy_graph.json", "r") as f:
@@ -36,28 +36,26 @@
     incomplete_graph = empty_graph.copy()
     path_str = cwd.as_posix()
     incomplete_graph.add_node(path_str, path=path_str, type="directory", id=path_str)
     assert not hierarchy.is_complete(
         incomplete_graph
     ), "Incomplete graph should not be complete"
 
-    with open("tests/data/hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
-    assert hierarchy.is_complete(hierarchy_graph), "Hierarchy graph should be complete."
-
 
 @pytest.mark.asyncio
-async def test_hierarchy_annotate(cwd):
+async def test_hierarchy_annotate(cwd, mock_db):
     graph = nx.MultiDiGraph()
     graph.graph["cwd"] = cwd.as_posix()
-    actual = await Hierarchy().annotate(graph)
+    hierarchy = Hierarchy()
+    actual = await hierarchy.annotate(graph, mock_db)
 
     # Load the template graph
     with open("tests/data/hierarchy_graph.json", "r") as f:
         data = json.load(f)
         expected = nx.readwrite.json_graph.node_link_graph(data)
     for node in expected:  # Add the ID field back in
         expected.nodes[node]["id"] = node
 
     assert set(actual.nodes) == set(expected.nodes), "Nodes are not equal"
     assert set(actual.edges) == set(expected.edges), "Edges are not equal"
+
+    assert hierarchy.is_complete(actual, mock_db), "Graph should be complete"
```

### Comparing `ragdaemon-0.1.1/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.2/tests/annotators/test_layout_hierarchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         layout_hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
     assert layout_hierarchy.is_complete(
         layout_hierarchy_graph
     ), "Layout hierarchy graph should be complete."
 
 
 @pytest.mark.asyncio
-async def test_layout_hierarchy_annotate(cwd):
+async def test_layout_hierarchy_annotate(cwd, mock_db):
     with open("tests/data/hierarchy_graph.json", "r") as f:
         data = json.load(f)
         hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
-    actual = await LayoutHierarchy().annotate(hierarchy_graph)
+    actual = await LayoutHierarchy().annotate(hierarchy_graph, mock_db)
 
     all_coordinates = set()
     for node, data in actual.nodes(data=True):
         coordinates = data.get("layout", {}).get("hierarchy", {})
         assert coordinates, f"Node {node} is missing hierarchy layout"
         all_coordinates.add((coordinates["x"], coordinates["y"], coordinates["z"]))
     assert (
```

### Comparing `ragdaemon-0.1.1/tests/data/chunker_graph.json` & `ragdaemon-0.1.2/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/data/context_message.txt` & `ragdaemon-0.1.2/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/data/diff_graph.json` & `ragdaemon-0.1.2/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.2/tests/data/hierarchy_graph.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'graph'": "{'files_checksum': '1ea8cdd83015d2a76755b20f648206e7'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "directed": true,
     "graph": {
         "cwd": "tests/sample",
-        "files_checksum": "e0a48ae81e4125ce0bb75ad3450ae998"
+        "files_checksum": "1ea8cdd83015d2a76755b20f648206e7"
     },
     "links": [
         {
             "key": 0,
             "source": "ROOT",
             "target": "src",
             "type": "hierarchy"
```

### Comparing `ragdaemon-0.1.1/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.2/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/tests/sample/src/interface.py` & `ragdaemon-0.1.2/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/LICENSE` & `ragdaemon-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.1/README.md` & `ragdaemon-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -21,27 +21,30 @@
 Ragdaemon is released open-source as a standalone RAG system. It includes a library of python classes to generate and query the knowledge graph. The graph itself is a NetworkX MultiDiGraph which saves/loads to a `.json` file.
 
 ```python
 import asyncio
 from pathlib import Path
 from ragdaemon.daemon import Daemon
 
-cwd = Path.cwd()
-daemon = Daemon(cwd)
-asyncio.run(daemon.update())
+async def main():
+    cwd = Path.cwd()
+    daemon = Daemon(cwd)
+    await daemon.update()
 
-# Search
-results = daemon.search("javascript")
-for result in results:
-    print(f"{result['distance']} | {result['id']}")
+    results = daemon.search("javascript")
+    for result in results:
+        print(f"{result['distance']} | {result['id']}")
 
-# RAG Context Selection
-query = "How do I run the tests?"
-context_builder = daemon.get_context(
-    query, 
-    include=["package.json"], 
-    auto_tokens=5000
-)
-context = context_builder.render()
-query += f"\nCODE CONTEXT\n{context}"
-...
+    query = "How do I run the tests?"
+    context_builder = daemon.get_context(
+        query, 
+        auto_tokens=5000
+    )
+    context = context_builder.render()
+    messages = [
+        {"role": "user", "content": query},
+        {"role": "user", "content": f"CODE CONTEXT\n{context}"}
+    ]
+    print(messages)
+
+asyncio.run(main())
 ```
```

### Comparing `ragdaemon-0.1.1/PKG-INFO` & `ragdaemon-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
@@ -41,27 +41,30 @@
 Ragdaemon is released open-source as a standalone RAG system. It includes a library of python classes to generate and query the knowledge graph. The graph itself is a NetworkX MultiDiGraph which saves/loads to a `.json` file.
 
 ```python
 import asyncio
 from pathlib import Path
 from ragdaemon.daemon import Daemon
 
-cwd = Path.cwd()
-daemon = Daemon(cwd)
-asyncio.run(daemon.update())
-
-# Search
-results = daemon.search("javascript")
-for result in results:
-    print(f"{result['distance']} | {result['id']}")
-
-# RAG Context Selection
-query = "How do I run the tests?"
-context_builder = daemon.get_context(
-    query, 
-    include=["package.json"], 
-    auto_tokens=5000
-)
-context = context_builder.render()
-query += f"\nCODE CONTEXT\n{context}"
-...
+async def main():
+    cwd = Path.cwd()
+    daemon = Daemon(cwd)
+    await daemon.update()
+
+    results = daemon.search("javascript")
+    for result in results:
+        print(f"{result['distance']} | {result['id']}")
+
+    query = "How do I run the tests?"
+    context_builder = daemon.get_context(
+        query, 
+        auto_tokens=5000
+    )
+    context = context_builder.render()
+    messages = [
+        {"role": "user", "content": query},
+        {"role": "user", "content": f"CODE CONTEXT\n{context}"}
+    ]
+    print(messages)
+
+asyncio.run(main())
 ```
```

