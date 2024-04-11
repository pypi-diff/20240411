# Comparing `tmp/privateai_client-3.7.2.tar.gz` & `tmp/privateai_client-3.8.0.tar.gz`

## Comparing `privateai_client-3.7.2.tar` & `privateai_client-3.8.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 privateai_client-3.7.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 privateai_client-3.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 privateai_client-3.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.7.2/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateai_client-3.7.2/requirements.dev.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 privateai_client-3.7.2/requirements.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-3.7.2/.github/pull-request-template.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/objects.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    29102 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/.env
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/.env.example
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/test_client.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/test_integration.py
--rw-r--r--   0        0        0    45025 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/test_request_objects.py
--rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/test_files/simpsons_wiki.txt
--rw-r--r--   0        0        0    98054 2020-02-02 00:00:00.000000 privateai_client-3.7.2/src/privateai_client/tests/test_files/test_audio.mp3
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 privateai_client-3.7.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-3.7.2/LICENSE
--rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-3.7.2/README.md
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 privateai_client-3.7.2/pyproject.toml
--rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 privateai_client-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 privateai_client-3.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 privateai_client-3.8.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.0/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateai_client-3.8.0/requirements.dev.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 privateai_client-3.8.0/requirements.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.github/pull-request-template.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    29790 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.env
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.env.example
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_client.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_integration.py
+-rw-r--r--   0        0        0    45748 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_request_objects.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_files/simpsons_wiki.txt
+-rw-r--r--   0        0        0    98054 2020-02-02 00:00:00.000000 privateai_client-3.8.0/src/privateai_client/tests/test_files/test_audio.mp3
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 privateai_client-3.8.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-3.8.0/LICENSE
+-rw-r--r--   0        0        0    12634 2020-02-02 00:00:00.000000 privateai_client-3.8.0/README.md
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 privateai_client-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0    13487 2020-02-02 00:00:00.000000 privateai_client-3.8.0/PKG-INFO
```

### Comparing `privateai_client-3.7.2/CHANGELOG.md` & `privateai_client-3.8.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,23 @@
 
 ### Added
 
 ### Changed
 
 ### Fixed
 
+## [3.8.0] - 2024-03-27
+
+### Added
+- Added support for the "enable_pdf_text_layer" PDFOption
+
+### Changed
+
+### Fixed
+
 ## [3.7.2] - 2024-03-04
 
 ### Added
 
 ### Changed
 - Minor formatting
```

### Comparing `privateai_client-3.7.2/CONTRIBUTING.md` & `privateai_client-3.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/objects.py` & `privateai_client-3.8.0/src/privateai_client/objects.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/pai_client.py` & `privateai_client-3.8.0/src/privateai_client/pai_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/components/pai_requests.py` & `privateai_client-3.8.0/src/privateai_client/components/pai_requests.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/components/pai_responses.py` & `privateai_client-3.8.0/src/privateai_client/components/pai_responses.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/components/pai_uris.py` & `privateai_client-3.8.0/src/privateai_client/components/pai_uris.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/components/request_objects.py` & `privateai_client-3.8.0/src/privateai_client/components/request_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,57 +384,74 @@
                 "FilterSelector can only accept the values 'type' and 'pattern'"
             )
 
 
 class PDFOptions(BaseRequestObject):
     default_density = 200
     default_max_resolution = 3000
+    default_enable_pdf_text_layer: bool = True
 
     def __init__(
         self,
         density: int = default_density,
         max_resolution: int = default_max_resolution,
+        enable_pdf_text_layer: bool = default_enable_pdf_text_layer
     ):
         self._density = density
         self._max_resolution = max_resolution
+        self._enable_pdf_text_layer = enable_pdf_text_layer
 
     @property
     def density(self):
         return self._density
 
     @property
     def max_resolution(self):
         return self._max_resolution
 
+    @property
+    def enable_pdf_text_layer(self):
+        return self._enable_pdf_text_layer
+
     @density.setter
     def density(self, var):
         if self._density_validator(var):
             self._density = var
 
     @max_resolution.setter
     def max_resolution(self, var):
         if self._max_resolution_validator(var):
             self._max_resolution = var
 
+    @enable_pdf_text_layer.setter
+    def enable_pdf_text_layer(self, var):
+        if self._enable_pdf_text_layer_validator(var):
+            self._enable_pdf_text_layer = var
+
     def _density_validator(self, var):
         if type(var) is not int:
             raise ValueError("PDFOptions.density must be of type int and >0")
         return True
 
     def _max_resolution_validator(self, var):
         if type(var) is not int:
             raise ValueError("PDFOptions.max_resolution must be of type int and >0")
         return True
 
+    def _enable_pdf_text_layer_validator(self, var):
+        if type(var) is not bool:
+            raise ValueError("PDFOptions.enable_pdf_text_layer must be of type bool")
+        return True
+
     @classmethod
     def fromdict(cls, values: dict):
         try:
             return cls._fromdict(values)
         except TypeError:
-            raise TypeError("PDFOptions can only accept 'density'")
+            raise TypeError("PDFOptions can only accept 'density', 'max_resolution' and 'enable_pdf_text_layer'")
 
 
 class ProcessedMarkerText(BaseRequestObject):
     attributes = ["_pattern"]
     default_pattern = "[UNIQUE_NUMBERED_ENTITY_TYPE]"
     valid_patterns = [
         "BEST_ENTITY_TYPE",
```

### Comparing `privateai_client-3.7.2/src/privateai_client/tests/test_client.py` & `privateai_client-3.8.0/src/privateai_client/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/tests/test_integration.py` & `privateai_client-3.8.0/src/privateai_client/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/tests/test_request_objects.py` & `privateai_client-3.8.0/src/privateai_client/tests/test_request_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,41 +438,45 @@
 
 
 # PDF Options Tests
 def test_pdf_options_default_initializer():
     pdf_options = PDFOptions()
     assert pdf_options.density == 200
     assert pdf_options.max_resolution == 3000
+    assert pdf_options.enable_pdf_text_layer is True
 
 
 def test_pdf_options_initializer():
-    pdf_options = PDFOptions(density=300, max_resolution=500)
+    pdf_options = PDFOptions(density=300, max_resolution=500, enable_pdf_text_layer=False)
     assert pdf_options.density == 300
     assert pdf_options.max_resolution == 500
+    assert pdf_options.enable_pdf_text_layer is False
 
 
 def test_pdf_options_initialize_fromdict():
-    pdf_options = PDFOptions.fromdict({"density": 300, "max_resolution": 500})
+    pdf_options = PDFOptions.fromdict({"density": 300, "max_resolution": 500, 'enable_pdf_text_layer': True})
     assert pdf_options.density == 300
     assert pdf_options.max_resolution == 500
-
+    assert pdf_options.enable_pdf_text_layer is True
 
 def test_pdf_options_invalid_initialize_fromdict():
-    error_msg = "PDFOptions can only accept 'density'"
+    error_msg = "PDFOptions can only accept 'density', 'max_resolution' and 'enable_pdf_text_layer'"
     with pytest.raises(TypeError) as excinfo:
         PDFOptions.fromdict({"density": 300, "max_resolution": 500, "junk": "value"})
     assert error_msg in str(excinfo.value)
 
 
 def test_pdf_options_setters():
     pdf_options = PDFOptions(density=300)
     pdf_options.density = 10
     assert pdf_options.density == 10
     pdf_options.max_resolution = 10
     assert pdf_options.max_resolution == 10
+    pdf_options.enable_pdf_text_layer = False
+    assert pdf_options.enable_pdf_text_layer is False
 
 
 def test_pdf_options_density_validator():
     error_msg = "PDFOptions.density must be of type int and >0"
     pdf_options = PDFOptions()
     with pytest.raises(ValueError) as excinfo:
         pdf_options.density = "junk"
@@ -483,18 +487,27 @@
     error_msg = "PDFOptions.max_resolution must be of type int and >0"
     pdf_options = PDFOptions()
     with pytest.raises(ValueError) as excinfo:
         pdf_options.max_resolution = "junk"
     assert error_msg in str(excinfo.value)
 
 
+def test_pdf_options_enable_pdf_text_layer_validator():
+    error_msg = "PDFOptions.enable_pdf_text_layer must be of type bool"
+    pdf_options = PDFOptions()
+    with pytest.raises(ValueError) as excinfo:
+        pdf_options.enable_pdf_text_layer = "junk"
+    assert error_msg in str(excinfo.value)
+
+
 def test_pdf_options_to_dict():
     pdf_options = PDFOptions().to_dict()
     assert pdf_options["density"] == 200
     assert pdf_options["max_resolution"] == 3000
+    assert pdf_options["enable_pdf_text_layer"] is True
 
 
 # Audio Options Tests
 def test_audio_options_default_initializer():
     audio_options = AudioOptions()
     assert audio_options.bleep_end_padding == 0.5
     assert audio_options.bleep_start_padding == 0.5
```

### Comparing `privateai_client-3.7.2/src/privateai_client/tests/test_files/simpsons_wiki.txt` & `privateai_client-3.8.0/src/privateai_client/tests/test_files/simpsons_wiki.txt`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/src/privateai_client/tests/test_files/test_audio.mp3` & `privateai_client-3.8.0/src/privateai_client/tests/test_files/test_audio.mp3`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/LICENSE` & `privateai_client-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/README.md` & `privateai_client-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/pyproject.toml` & `privateai_client-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `privateai_client-3.7.2/PKG-INFO` & `privateai_client-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: privateai_client
-Version: 3.7.2
+Version: 3.8.0
 Summary: A thin client for communicating with the Private AI de-identication API.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Project-URL: Changelog, https://github.com/privateai/pai-thin-client/blob/main/CHANGELOG.md
 Project-URL: Contributing, https://github.com/privateai/pai-thin-client/blob/main/CONTRIBUTING.md
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
 License-File: LICENSE
```

