# Comparing `tmp/mustopt-0.1.3.tar.gz` & `tmp/mustopt-0.1.4.tar.gz`

## Comparing `mustopt-0.1.3.tar` & `mustopt-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mustopt-0.1.3/src/mustopt/__about__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 mustopt-0.1.3/src/mustopt/__init__.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 mustopt-0.1.3/src/mustopt/model.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 mustopt-0.1.3/tests/test_mustopt.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 mustopt-0.1.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mustopt-0.1.3/LICENSE
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mustopt-0.1.3/README.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 mustopt-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 mustopt-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 mustopt-0.1.4/coverage.toml
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 mustopt-0.1.4/ruff.toml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/__about__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/__init__.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 mustopt-0.1.4/src/mustopt/model.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mustopt-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mustopt-0.1.4/tests/test_model.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 mustopt-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 mustopt-0.1.4/LICENSE
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mustopt-0.1.4/README.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 mustopt-0.1.4/hatch.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 mustopt-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 mustopt-0.1.4/PKG-INFO
```

### Comparing `mustopt-0.1.3/tests/test_mustopt.py` & `mustopt-0.1.4/tests/test_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,52 @@
+"""Tests for mustopt.model."""
+
 import unittest
 
-from hamcrest import assert_that, equal_to
+from hamcrest import assert_that, calling, equal_to, raises
 
-from mustopt import MustOpt
+from mustopt import InvalidContainerError, MustOpt
 
 
 class TestMustOpt(unittest.TestCase):
-    def test_empty_new_is_invalid(self):
-        assert_that(MustOpt.new().valid(), equal_to(False))
-
-    def test_new_from_value_is_valid(self):
-        assert_that(MustOpt.new(1).valid(), equal_to(True))
+    """Tests for MustOpt."""
 
-    def test_unset_makes_container_invalid(self):
+    @staticmethod
+    def test_empty_new_is_invalid():
+        """Test empty new() returns invalid container."""
+        assert_that(not MustOpt.new().valid())
+
+    @staticmethod
+    def test_new_from_value_is_valid():
+        """Test new() with value returns valid container."""
+        assert_that(MustOpt.new(1).valid())
+
+    @staticmethod
+    def test_unset_makes_container_invalid():
+        """Test unset() invalidates container."""
         val = MustOpt.new(1)
         val.unset()
-        assert_that(val.valid(), equal_to(False))
+        assert_that(not val.valid())
 
-    def test_set_value_makes_container_valid(self):
-        val = MustOpt.new()
+    @staticmethod
+    def test_set_value_makes_container_valid():
+        """Test set() with non-None value makes container valid."""
+        val: MustOpt[int] = MustOpt.new()
         val.set(1)
-        assert_that(val.valid(), equal_to(True))
+        assert_that(val.valid())
 
-    def test_set_none_makes_container_invalid(self):
-        val = MustOpt.new()
+    @staticmethod
+    def test_set_none_makes_container_invalid():
+        """Test set() with None value makes container invalid."""
+        val: MustOpt[None] = MustOpt.new()
         val.set(None)
-        assert_that(val.valid(), equal_to(False))
+        assert_that(not val.valid())
 
-    def test_must_from_valid_container_works(self):
+    @staticmethod
+    def test_must_from_valid_container_works():
+        """Test must() for valid container works."""
         assert_that(MustOpt.new(1).must(), equal_to(1))
 
-    def test_must_from_invalid_container_raises_exception(self):
-        try:
-            MustOpt.new().must()
-        except RuntimeError as e:
-            assert_that(str(e), equal_to('Underlying value is not valid'))
+    @staticmethod
+    def test_must_from_invalid_container_raises_exception():
+        """Test must() for invalid container fails."""
+        assert_that(calling(MustOpt.must).with_args(MustOpt.new()), raises(InvalidContainerError))
```

### Comparing `mustopt-0.1.3/.gitignore` & `mustopt-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mustopt-0.1.3/LICENSE` & `mustopt-0.1.4/LICENSE`

 * *Files identical despite different names*

