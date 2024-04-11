# Comparing `tmp/misc_python_utils-0.1.6.tar.gz` & `tmp/misc_python_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_python_utils-0.1.6.tar", max compression
+gzip compressed data, was "misc_python_utils-0.1.7.tar", max compression
```

## Comparing `misc_python_utils-0.1.6.tar` & `misc_python_utils-0.1.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1073 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/LICENSE
--rw-r--r--   0        0        0      973 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/README.md
--rw-r--r--   0        0        0       73 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/__init__.py
--rw-r--r--   0        0        0     1599 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/base64_utils.py
--rw-r--r--   0        0        0     5617 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/beartypes.py
--rw-r--r--   0        0        0       73 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/__init__.py
--rw-r--r--   0        0        0     3586 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable.py
--rw-r--r--   0        0        0     1301 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable_container.py
--rw-r--r--   0        0        0     4737 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable_data.py
--rw-r--r--   0        0        0       33 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/readme.md
--rw-r--r--   0        0        0     1429 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/colored_logs_formatter.py
--rw-r--r--   0        0        0     1008 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/command_line_styling.py
--rw-r--r--   0        0        0     1256 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/dataclass_utils.py
--rw-r--r--   0        0        0     1628 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/dict_utils.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/error_handling/__init__.py
--rw-r--r--   0        0        0     3311 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/error_handling/as_result_logged.py
--rw-r--r--   0        0        0     3924 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/error_handling/exception_as_err.py
--rw-r--r--   0        0        0      217 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/error_handling/readme.md
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/file_utils/__init__.py
--rw-r--r--   0        0        0     2882 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/file_utils/readwrite_csv_files.py
--rw-r--r--   0        0        0     4205 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/file_utils/readwrite_files.py
--rw-r--r--   0        0        0     1371 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/file_utils/tarfile_utils.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/gitrepo_utils/__init__.py
--rw-r--r--   0        0        0     1845 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/gitrepo_utils/git_repo_content.py
--rw-r--r--   0        0        0     4060 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/gitrepo_utils/git_repo_state.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/hashcached_data/__init__.py
--rw-r--r--   0        0        0     6309 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/hashcached_data/hashcached_data.py
--rw-r--r--   0        0        0     2493 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/hashcached_data/hashcached_data_specific.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/__init__.py
--rw-r--r--   0        0        0     5048 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py
--rw-r--r--   0        0        0     7603 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/flowchart_from_code.py
--rw-r--r--   0        0        0     1753 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/markdown_table_utils.py
--rw-r--r--   0        0        0     1114 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_dag.py
--rw-r--r--   0        0        0     3355 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_data_models.py
--rw-r--r--   0        0        0     1545 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py
--rw-r--r--   0        0        0     2146 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/prefix_suffix.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/processing_utils/__init__.py
--rw-r--r--   0        0        0     1969 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/processing_utils/processing_utils.py
--rw-r--r--   0        0        0     2232 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/processing_utils/threadpool_with_backpressure.py
--rw-r--r--   0        0        0        0 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/text_processing/__init__.py
--rw-r--r--   0        0        0     2336 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/text_processing/diffmatchpatch_html.py
--rw-r--r--   0        0        0     3638 2024-03-21 06:34:32.850561 misc_python_utils-0.1.6/misc_python_utils/utils.py
--rw-r--r--   0        0        0      839 2024-03-21 06:34:53.750690 misc_python_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 misc_python_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/LICENSE
+-rw-r--r--   0        0        0      973 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/README.md
+-rw-r--r--   0        0        0       73 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/__init__.py
+-rw-r--r--   0        0        0     1599 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/base64_utils.py
+-rw-r--r--   0        0        0     5617 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/beartypes.py
+-rw-r--r--   0        0        0       73 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable.py
+-rw-r--r--   0        0        0     1301 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable_container.py
+-rw-r--r--   0        0        0     4937 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable_data.py
+-rw-r--r--   0        0        0       33 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/readme.md
+-rw-r--r--   0        0        0     1429 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/colored_logs_formatter.py
+-rw-r--r--   0        0        0     1008 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/command_line_styling.py
+-rw-r--r--   0        0        0     1256 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/dataclass_utils.py
+-rw-r--r--   0        0        0     1628 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/dict_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/error_handling/__init__.py
+-rw-r--r--   0        0        0     3311 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/error_handling/as_result_logged.py
+-rw-r--r--   0        0        0     3924 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/error_handling/exception_as_err.py
+-rw-r--r--   0        0        0      217 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/error_handling/readme.md
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/file_utils/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/file_utils/readwrite_csv_files.py
+-rw-r--r--   0        0        0     4205 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/file_utils/readwrite_files.py
+-rw-r--r--   0        0        0     1335 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/file_utils/tarfile_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/gitrepo_utils/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/gitrepo_utils/git_repo_content.py
+-rw-r--r--   0        0        0     4060 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/gitrepo_utils/git_repo_state.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.084039 misc_python_utils-0.1.7/misc_python_utils/hashcached_data/__init__.py
+-rw-r--r--   0        0        0     6309 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/hashcached_data/hashcached_data.py
+-rw-r--r--   0        0        0     2493 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/hashcached_data/hashcached_data_specific.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/__init__.py
+-rw-r--r--   0        0        0     5048 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py
+-rw-r--r--   0        0        0     7603 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/flowchart_from_code.py
+-rw-r--r--   0        0        0     1753 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/markdown_table_utils.py
+-rw-r--r--   0        0        0     1114 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_dag.py
+-rw-r--r--   0        0        0     3355 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_data_models.py
+-rw-r--r--   0        0        0     1545 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py
+-rw-r--r--   0        0        0     2204 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/prefix_suffix.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/processing_utils/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/processing_utils/processing_utils.py
+-rw-r--r--   0        0        0     2232 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/processing_utils/threadpool_with_backpressure.py
+-rw-r--r--   0        0        0        0 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/text_processing/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/text_processing/diffmatchpatch_html.py
+-rw-r--r--   0        0        0     3638 2024-04-11 06:17:46.088039 misc_python_utils-0.1.7/misc_python_utils/utils.py
+-rw-r--r--   0        0        0      839 2024-04-11 06:18:00.999996 misc_python_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 misc_python_utils-0.1.7/PKG-INFO
```

### Comparing `misc_python_utils-0.1.6/LICENSE` & `misc_python_utils-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/README.md` & `misc_python_utils-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/base64_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/beartypes.py` & `misc_python_utils-0.1.7/misc_python_utils/beartypes.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable.py` & `misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     @property
     def _is_ready(self) -> bool:
         return self.buildable_behavior.it_is_ready(self)
 
     @final  # does not enforce it but at least the IDE warns you!
     def build(
         self: TBuildable,
-    ) -> TBuildable:
+    ) -> TBuildable:  # TODO: Self here?
         """
         should NOT be overwritten!
         """
         if not self._is_ready:
             all_undefined_must_be_filled(self)
             self._build_all_children()
             start = time()
```

### Comparing `misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable_container.py` & `misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable_container.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/buildable_dataclasses/buildable_data.py` & `misc_python_utils-0.1.7/misc_python_utils/buildable_dataclasses/buildable_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     @classmethod
     def build_it(cls, obj: TBuildableData) -> None:
         Path(obj.data_dir).mkdir(
             parents=True,
             exist_ok=True,
         )
         obj._build_data()  # noqa: SLF001
+        obj._was_built = True  # noqa: SLF001 # tilo: this _was_built refers to "was built in this python-process"
         if not obj._is_data_valid:  # noqa: SLF001
             msg = f"{cls.__class__.__name__}: {obj.name} failed to build data in {obj.data_dir=}"
             raise AssertionError(msg)
 
 
 @dataclass(kw_only=True)
 class BuildableData(ABC, Buildable):
@@ -86,16 +87,18 @@
 
     @property
     @abstractmethod
     def name(self) -> NameSlug:
         ...
 
     @property
+    @abstractmethod
     def _is_data_valid(self) -> bool:
-        return False
+        # if you want to rebuilt all the time check for "_was_built" here
+        ...
 
     @abstractmethod
     def _build_data(self) -> None:
         """
         build/write data
         """
         ...
```

### Comparing `misc_python_utils-0.1.6/misc_python_utils/colored_logs_formatter.py` & `misc_python_utils-0.1.7/misc_python_utils/colored_logs_formatter.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/command_line_styling.py` & `misc_python_utils-0.1.7/misc_python_utils/command_line_styling.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/dataclass_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/dataclass_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/dict_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/error_handling/as_result_logged.py` & `misc_python_utils-0.1.7/misc_python_utils/error_handling/as_result_logged.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/error_handling/exception_as_err.py` & `misc_python_utils-0.1.7/misc_python_utils/error_handling/exception_as_err.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/file_utils/readwrite_csv_files.py` & `misc_python_utils-0.1.7/misc_python_utils/file_utils/readwrite_csv_files.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/file_utils/readwrite_files.py` & `misc_python_utils-0.1.7/misc_python_utils/file_utils/readwrite_files.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/file_utils/tarfile_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/file_utils/tarfile_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 @dataclasses.dataclass(slots=True, frozen=True)
 class TarFileOutput:
     info: tarfile.TarInfo
     exfile_object: tarfile.ExFileObject
 
 
-# TODO: why was this commented out?
 def filter_gen_targz_members(
     targz_file: str,
     is_of_interest_fun: Callable[[tarfile.TarInfo], bool],
     start: int | None = None,
     stop: int | None = None,
 ) -> Iterator[TarFileOutput]:
     with tarfile.open(targz_file, "r:gz") as tar:
```

### Comparing `misc_python_utils-0.1.6/misc_python_utils/gitrepo_utils/git_repo_content.py` & `misc_python_utils-0.1.7/misc_python_utils/gitrepo_utils/git_repo_content.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/gitrepo_utils/git_repo_state.py` & `misc_python_utils-0.1.7/misc_python_utils/gitrepo_utils/git_repo_state.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/hashcached_data/hashcached_data.py` & `misc_python_utils-0.1.7/misc_python_utils/hashcached_data/hashcached_data.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/hashcached_data/hashcached_data_specific.py` & `misc_python_utils-0.1.7/misc_python_utils/hashcached_data/hashcached_data_specific.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/flowchart_from_code.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/flowchart_from_code.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/markdown_table_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/markdown_table_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_dag.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_dag.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_data_models.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_data_models.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py` & `misc_python_utils-0.1.7/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/prefix_suffix.py` & `misc_python_utils-0.1.7/misc_python_utils/prefix_suffix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import dataclasses
 from dataclasses import dataclass
-from typing import Any, ClassVar, Union
+from typing import Any, ClassVar, TypeVar
 
 from misc_python_utils.buildable_dataclasses.buildable import Buildable
 from misc_python_utils.dataclass_utils import UNDEFINED, Undefined
 
-BASE_PATHES: dict[str, Union[str, "PrefixSuffix"]] = {}
+TPrefixSuffix = TypeVar("TPrefixSuffix", bound="PrefixSuffix")
+BASE_PATHES: dict[str, str | TPrefixSuffix] = {}
 BASE_PATHES[
     "pwd"
 ] = "."  # noqa: S105 -> this is a false-positive! pwd does not stand for "password" but the "current path"
 
 
 @dataclass
 class PrefixSuffix(Buildable):
```

### Comparing `misc_python_utils-0.1.6/misc_python_utils/processing_utils/processing_utils.py` & `misc_python_utils-0.1.7/misc_python_utils/processing_utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/processing_utils/threadpool_with_backpressure.py` & `misc_python_utils-0.1.7/misc_python_utils/processing_utils/threadpool_with_backpressure.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/text_processing/diffmatchpatch_html.py` & `misc_python_utils-0.1.7/misc_python_utils/text_processing/diffmatchpatch_html.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/misc_python_utils/utils.py` & `misc_python_utils-0.1.7/misc_python_utils/utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.6/pyproject.toml` & `misc_python_utils-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "misc-python-utils"
-version = "0.1.6" # see: https://pypi.org/project/poetry-dynamic-versioning/
+version = "0.1.7" # see: https://pypi.org/project/poetry-dynamic-versioning/
 description = ""
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 repository = "https://github.com/dertilo/misc-python-utils"
 
 readme = "README.md"
 packages = [{ include = "misc_python_utils" }]
```

### Comparing `misc_python_utils-0.1.6/PKG-INFO` & `misc_python_utils-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-python-utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/dertilo/misc-python-utils
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

