# Comparing `tmp/ludic-0.3.0.tar.gz` & `tmp/ludic-0.3.1.tar.gz`

## Comparing `ludic-0.3.0.tar` & `ludic-0.3.1.tar`

### file list

```diff
@@ -1,74 +1,79 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.3.0/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.3.0/mkdocs.yaml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.3.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.3.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/htmx.md
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.3.0/docs/web-framework.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/README.md
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/bulk_update.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/click_to_edit.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/click_to_load.py
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/delete_row.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/edit_row.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/infinite_scroll.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 ludic-0.3.0/examples/lazy_loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/__init__.py
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/attrs.py
--rw-r--r--   0        0        0     9977 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/components.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/format.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/utils.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/forms.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/items.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/loaders.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7157 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/tables.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/typography.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/collect.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/themes.py
--rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/types.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/__init__.py
--rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/app.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/parsers.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/requests.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/responses.py
--rw-r--r--   0        0        0     4041 2020-02-02 00:00:00.000000 ludic-0.3.0/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_components.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_elements.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_exceptions.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_formatting.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_styles.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_themes.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/web/__init__.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 ludic-0.3.0/tests/web/test_datastructures.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.3.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.3.0/LICENCE
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 ludic-0.3.0/README.md
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 ludic-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 ludic-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.3.1/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.3.1/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/catalog.md
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/getting-started.md
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/README.md
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/__init__.py
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/bulk_update.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/click_to_load.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/delete_row.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/edit_row.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/infinite_scroll.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/lazy_loading.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/__init__.py
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/attrs.py
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/components.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/format.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/utils.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/items.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/collect.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/themes.py
+-rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/types.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/__init__.py
+-rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/responses.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_components.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_formatting.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_styles.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_themes.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.3.1/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.3.1/README.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ludic-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 ludic-0.3.1/PKG-INFO
```

### Comparing `ludic-0.3.0/.pre-commit-config.yaml` & `ludic-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/CONTRIBUTING.md` & `ludic-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/mkdocs.yaml` & `ludic-0.3.1/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/.github/workflows/publish.yaml` & `ludic-0.3.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/.github/workflows/test.yaml` & `ludic-0.3.1/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
         python -m pip install .[full,test]
 
     - name: Test with pytest
       run: |
         pytest --cov --cov-report xml:coverage.xml
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v4.1.0
+      uses: codecov/codecov-action@v4.2.0
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `ludic-0.3.0/docs/catalog.md` & `ludic-0.3.1/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/docs/components.md` & `ludic-0.3.1/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/docs/getting-started.md` & `ludic-0.3.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/docs/htmx.md` & `ludic-0.3.1/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/docs/index.md` & `ludic-0.3.1/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Introduction
+<p align="center">
+    <img width="600px" src="./assets/ludic.png" alt="ludic">
+</p>
 
 [![test](https://github.com/paveldedik/ludic/actions/workflows/test.yaml/badge.svg)](https://github.com/paveldedik/ludic/actions) [![codecov](https://codecov.io/gh/paveldedik/ludic/graph/badge.svg?token=BBDNJWHMGX)](https://codecov.io/gh/paveldedik/ludic) [![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-312/) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Documentation Status](https://readthedocs.org/projects/ludic/badge/?version=latest)](https://ludic.readthedocs.io/en/latest/?badge=latest)
 
 Ludic is a lightweight framework for building HTML pages with a component approach similar to [React](https://react.dev/). It is built to be used together with [htmx.org](https://htmx.org/) so that developers don't need to write almost any JavaScript to create dynamic web services. Its potential can be leveraged together with its web framework which is a wrapper around the powerful [Starlette](https://www.starlette.io/) framework. It is built with the latest Python 3.12 features heavily incorporating typing.
 
 !!! warning "Experimental"
```

### Comparing `ludic-0.3.0/docs/styles.md` & `ludic-0.3.1/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/docs/web-framework.md` & `ludic-0.3.1/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/examples/README.md` & `ludic-0.3.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/examples/bulk_update.py` & `ludic-0.3.1/examples/bulk_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Annotated, Self, override
 
-from examples import Body, Header, Page, app, init_db
+from examples import Body, Header, Page, init_db
+
 from ludic.catalog.buttons import ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import ColumnMeta, Table, create_rows
 from ludic.html import span, style
 from ludic.types import Attrs
-from ludic.web.endpoints import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.parsers import ListParser
 
 db = init_db()
+app = LudicApp(debug=True)
 
 
 class PersonAttrs(Attrs, total=False):
     id: Annotated[str, ColumnMeta(identifier=True)]
     name: Annotated[str, ColumnMeta()]
     email: Annotated[str, ColumnMeta()]
     active: Annotated[
@@ -31,14 +33,16 @@
     id: str = "toast"
     target: str = f"#{id}"
     styles = style.use(
         lambda theme: {
             Toast.target: {
                 "background": theme.colors.success,
                 "margin": "10px 20px",
+                "padding": "5px 8px",
+                "border-radius": "3px",
                 "opacity": "0",
                 "transition": "opacity 3s ease-out",
             },
             f"{Toast.target}.htmx-settling": {
                 "opacity": "100",
             },
         }
```

### Comparing `ludic-0.3.0/examples/click_to_edit.py` & `ludic-0.3.1/examples/click_to_edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from typing import Annotated, NotRequired, Self, override
 
-from examples import Body, Header, Page, app, init_db
-from ludic.catalog.buttons import ButtonDanger, ButtonPrimary
+from examples import Body, Header, Page, init_db
+
+from ludic.catalog.buttons import Button, ButtonDanger, ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form, create_fields
 from ludic.catalog.items import Pairs
 from ludic.catalog.quotes import Quote
 from ludic.html import div
 from ludic.types import Attrs
-from ludic.web.endpoints import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser, ValidationError
 
 db = init_db()
+app = LudicApp(debug=True)
 
 
 def email_validator(email: str) -> str:
     if len(email.split("@")) != 2:
         raise ValidationError("Invalid email")
     return email
 
@@ -67,15 +69,15 @@
 
         return cls(**contact.dict())
 
     @override
     def render(self) -> div:
         return div(
             Pairs(items=self.attrs.items()),
-            ButtonPrimary(
+            Button(
                 "Click To Edit",
                 hx_get=self.url_for(ContactForm),
             ),
             hx_target="this",
             hx_swap="outerHTML",
         )
 
@@ -95,8 +97,9 @@
     def render(self) -> Form:
         return Form(
             *create_fields(self.attrs, spec=ContactAttrs),
             ButtonPrimary("Submit"),
             ButtonDanger("Cancel", hx_get=self.url_for(Contact)),
             hx_put=self.url_for(Contact),
             hx_target="this",
+            hx_swap="outerHTML",
         )
```

### Comparing `ludic-0.3.0/examples/click_to_load.py` & `ludic-0.3.1/examples/click_to_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import Self, override
 
-from examples import Body, Header, Page, app
+from examples import Body, Header, Page
+
 from ludic.attrs import ButtonAttrs
 from ludic.catalog.buttons import ButtonPrimary
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.html import td
 from ludic.types import Attrs, Blank, Component, ComponentStrict
-from ludic.web import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.datastructures import QueryParams
 
+app = LudicApp(debug=True)
+
 
 class ContactAttrs(Attrs):
     id: str
     name: str
     email: str
 
 
@@ -46,36 +49,25 @@
             "Load More Agents...",
             hx_get=self.attrs["url"],
             hx_target=f"#{self.target}",
             hx_swap="outerHTML",
         )
 
 
-class ContactsTable(Component[TableRow, Attrs]):
-    @override
-    def render(self) -> Table:
-        return Table(
-            TableHead("ID", "Name", "Email"),
-            *self.children,
-            style={"text-align": "center"},
-        )
-
-
 @app.get("/")
 async def index() -> Page:
-    slice = await ContactsSlice.get(QueryParams(page=1))
     return Page(
         Header("Click To Edit"),
         Body(
             Quote(
                 "This example shows how to implement click-to-load the next page in "
                 "a table of data.",
                 source_url="https://htmx.org/examples/click-to-load/",
             ),
-            ContactsTable(*slice.render().children),
+            ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
         ),
     )
 
 
 @app.endpoint("/contacts/")
 class ContactsSlice(Endpoint[ContactsSliceAttrs]):
     @classmethod
@@ -90,14 +82,26 @@
             *(
                 TableRow(contact["id"], contact["name"], contact["email"])
                 for contact in self.attrs["contacts"]
             ),
             TableRow(
                 td(
                     LoadMoreButton(
-                        url=self.url_for(ContactsSlice).query(page=next_page)
+                        url=self.url_for(ContactsSlice).include_query_params(
+                            page=next_page
+                        )
                     ),
                     colspan=3,
                 ),
                 id=LoadMoreButton.target,
             ),
         )
+
+
+class ContactsTable(Component[ContactsSlice, Attrs]):
+    @override
+    def render(self) -> Table[TableHead, ContactsSlice]:
+        return Table(
+            TableHead("ID", "Name", "Email"),
+            *self.children,
+            style={"text-align": "center"},
+        )
```

### Comparing `ludic-0.3.0/examples/delete_row.py` & `ludic-0.3.1/examples/delete_row.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Self, override
 
-from examples import Body, Header, Page, app, init_db
+from examples import Body, Header, Page, init_db
+
 from ludic.attrs import Attrs, HtmxAttrs
 from ludic.catalog.buttons import ButtonDanger
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
-from ludic.web.endpoints import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 
 db = init_db()
+app = LudicApp(debug=True)
 
 
 class PersonAttrs(Attrs):
     id: str
     name: str
     email: str
     active: bool
```

### Comparing `ludic-0.3.0/examples/edit_row.py` & `ludic-0.3.1/examples/edit_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from typing import Annotated, NotRequired, Self, override
 
-from examples import Body, Header, Page, app, init_db
+from examples import Body, Header, Page, init_db
+
 from ludic.attrs import Attrs, HtmxAttrs
-from ludic.catalog.buttons import ButtonPrimary, ButtonSecondary
+from ludic.catalog.buttons import (
+    ButtonPrimary,
+    ButtonSecondary,
+    ButtonSuccess,
+)
 from ludic.catalog.forms import InputField
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import ColumnMeta, Table, TableHead, TableRow
 from ludic.html import div
 from ludic.types import JavaScript
-from ludic.web.endpoints import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser
 
 db = init_db()
+app = LudicApp(debug=True)
 
 
 class PersonAttrs(Attrs):
     id: NotRequired[str]
     name: Annotated[str, ColumnMeta()]
     email: Annotated[str, ColumnMeta()]
 
@@ -102,15 +108,15 @@
     @override
     def render(self) -> TableRow:
         return TableRow(
             InputField(name="name", value=self.attrs["name"]),
             InputField(name="email", value=self.attrs["email"]),
             div(
                 ButtonSecondary("Cancel", hx_get=self.url_for(PersonRow)),
-                ButtonPrimary(
+                ButtonSuccess(
                     "Save",
                     hx_put=self.url_for(PersonRow),
                     hx_include="closest tr",
                 ),
             ),
             class_="editing",
         )
```

### Comparing `ludic-0.3.0/examples/infinite_scroll.py` & `ludic-0.3.1/examples/infinite_scroll.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Self, override
 
-from examples import Body, Header, Page, app
+from examples import Body, Header, Page
+
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.types import Attrs, Blank, Component
-from ludic.web import Endpoint
+from ludic.web import Endpoint, LudicApp
 from ludic.web.datastructures import QueryParams
 
+app = LudicApp(debug=True)
+
 
 class ContactAttrs(Attrs):
     id: str
     name: str
     email: str
 
 
@@ -26,36 +29,25 @@
             email=f"void{page * 10 + idx}@null.org",
             name="Agent Smith",
         )
         for idx in range(10)
     ]
 
 
-class ContactsTable(Component[TableRow, Attrs]):
-    @override
-    def render(self) -> Table:
-        return Table(
-            TableHead("ID", "Name", "Email"),
-            *self.children,
-            style={"text-align": "center"},
-        )
-
-
 @app.get("/")
 async def index() -> Page:
-    slice = await ContactsSlice.get(QueryParams(page=1))
     return Page(
         Header("Infinite Scroll"),
         Body(
             Quote(
                 "The infinite scroll pattern provides a way to load content dynamically"
                 "on user scrolling action.",
                 source_url="https://htmx.org/examples/infinite-scroll/",
             ),
-            ContactsTable(*slice.render().children),
+            ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
         ),
     )
 
 
 @app.endpoint("/contacts/")
 class ContactsSlice(Endpoint[ContactsSliceAttrs]):
     @classmethod
@@ -69,12 +61,24 @@
             (contact["id"], contact["name"], contact["email"])
             for contact in self.attrs["contacts"]
         )
         return Blank(
             *(TableRow(*rows) for rows in init),
             TableRow(
                 *last,
-                hx_get=self.url_for(ContactsSlice).query(page=self.attrs["page"] + 1),
+                hx_get=self.url_for(ContactsSlice).include_query_params(
+                    page=self.attrs["page"] + 1
+                ),
                 hx_trigger="revealed",
                 hx_swap="afterend",
             ),
         )
+
+
+class ContactsTable(Component[ContactsSlice, Attrs]):
+    @override
+    def render(self) -> Table[TableHead, ContactsSlice]:
+        return Table(
+            TableHead("ID", "Name", "Email"),
+            *self.children,
+            style={"text-align": "center"},
+        )
```

### Comparing `ludic-0.3.0/examples/lazy_loading.py` & `ludic-0.3.1/examples/lazy_loading.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import asyncio
 
-from examples import Body, Header, Page, app
+from examples import Body, Header, Page
+
 from ludic.catalog.loaders import LazyLoader
 from ludic.catalog.quotes import Quote
 from ludic.html import div, svg
 from ludic.types import Safe
-from ludic.web import Request
+from ludic.web import LudicApp, Request
+
+app = LudicApp(debug=True)
 
 
 @app.get("/")
-async def homepage(request: Request) -> Page:
+async def index(request: Request) -> Page:
     return Page(
         Header("Lazy Loading"),
         Body(
             Quote(
                 "This example shows how to lazily load an element on a page.",
                 source_url="https://htmx.org/examples/lazy-load/",
             ),
```

### Comparing `ludic-0.3.0/ludic/attrs.py` & `ludic-0.3.1/ludic/attrs.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/base.py` & `ludic-0.3.1/ludic/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,20 +79,25 @@
 
     classes: ClassVar[Sequence[str]] = []
     styles: ClassVar["GlobalStyles"] = {}
 
     children: Sequence[Any]
     attrs: Mapping[str, Any]
 
-    _theme: Theme | None = None
+    context: dict[str, Any]
 
     def __init_subclass__(cls) -> None:
         ELEMENT_REGISTRY.setdefault(cls.__name__, [])
         ELEMENT_REGISTRY[cls.__name__].append(cls)
 
+    def __init__(self, *children: Any, **attrs: Any) -> None:
+        self.context = {}
+        self.children = children
+        self.attrs = attrs
+
     def __str__(self) -> str:
         return self.to_string()
 
     def __format__(self, _: str) -> str:
         return self.formatter.append(self)
 
     def __len__(self) -> int:
@@ -130,20 +135,16 @@
 
     def _format_children(
         self,
         format_fun: Callable[[Any], str] = format_element,
     ) -> str:
         formatted = []
         for child in self.children:
-            if (
-                isinstance(child, BaseElement)
-                and child._theme is None
-                and self._theme is not None
-            ):
-                child.theme = self.theme
+            if isinstance(child, BaseElement):
+                child.context.update(self.context)
             formatted.append(format_fun(child))
         return "".join(formatted)
 
     @property
     def aliased_attrs(self) -> dict[str, Any]:
         """Attributes as a dict with keys renamed to their aliases."""
         return format_attrs(type(self), dict(self.attrs))
@@ -155,20 +156,18 @@
             child.text if isinstance(child, BaseElement) else str(child)
             for child in self.children
         )
 
     @property
     def theme(self) -> Theme:
         """Get the theme of the element."""
-        return self._theme or get_default_theme()
-
-    @theme.setter
-    def theme(self, value: Theme) -> None:
-        """Set the theme of the element."""
-        self._theme = value
+        if context_theme := self.context.get("theme"):
+            if isinstance(context_theme, Theme):
+                return context_theme
+        return get_default_theme()
 
     def is_simple(self) -> bool:
         """Check if the element is simple (i.e. contains only one primitive type)."""
         return len(self) == 1 and isinstance(self.children[0], str | int | float | bool)
 
     def has_attributes(self) -> bool:
         """Check if the element has any attributes."""
@@ -210,15 +209,15 @@
 
     def to_html(self) -> str:
         """Convert an element tree to an HTML string."""
         dom = self
         classes = list(dom.classes)
 
         while dom != (rendered_dom := dom.render()):
-            rendered_dom._theme = dom._theme
+            rendered_dom.context.update(dom.context)
             dom = rendered_dom
             classes += dom.classes
 
         element_tag = f"{dom.html_header}\n" if dom.html_header else ""
 
         hidden = dom.html_name == "__hidden__"
         element_tag = "" if hidden else f"<{dom.html_name}"
@@ -301,14 +300,15 @@
 
     def __init__(
         self,
         *children: TChildren,
         # FIXME: https://github.com/python/typing/issues/1399
         **attributes: Unpack[TAttrs],  # type: ignore
     ) -> None:
+        super().__init__()
         self.attrs = cast(TAttrs, attributes)
         self.children = tuple(self.formatter.extract(*children))
 
 
 class ElementStrict(Generic[*TChildrenArgs, TAttrs], BaseElement):
     """Base class for strict elements (elements with concrete types of children).
 
@@ -322,9 +322,10 @@
 
     def __init__(
         self,
         *children: *TChildrenArgs,
         # FIXME: https://github.com/python/typing/issues/1399
         **attrs: Unpack[TAttrs],  # type: ignore
     ) -> None:
+        super().__init__()
         self.attrs = cast(TAttrs, attrs)
         self.children = tuple(self.formatter.extract(*children))
```

### Comparing `ludic-0.3.0/ludic/components.py` & `ludic-0.3.1/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/format.py` & `ludic-0.3.1/ludic/format.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/html.py` & `ludic-0.3.1/ludic/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     VideoAttrs,
 )
 from .styles import (
     Theme,
     format_styles,
     from_components,
     from_loaded,
-    get_default_theme,
 )
 from .types import (
     AnyChildren,
     BaseElement,
     ComplexChildren,
     CSSProperties,
     Element,
@@ -311,17 +310,18 @@
 
     def __init__(
         self,
         styles: GlobalStyles | Callable[[Theme], GlobalStyles] | str,
         theme: Theme | None = None,
         **attrs: Unpack[StyleAttrs],
     ) -> None:
-        self.children = (styles,)
-        self.attrs = attrs
-        self.theme = theme or get_default_theme()
+        super().__init__(styles, **attrs)
+
+        if theme:
+            self.context["theme"] = theme
 
     @classmethod
     def use(cls, styles: GlobalStyles | Callable[[Theme], GlobalStyles]) -> Self:
         return cls(styles)
 
     @classmethod
     def from_components(
```

### Comparing `ludic-0.3.0/ludic/types.py` & `ludic-0.3.1/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/utils.py` & `ludic-0.3.1/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/catalog/buttons.py` & `ludic-0.3.1/ludic/catalog/buttons.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     """
 
     classes = ["btn"]
     styles = style.use(
         lambda theme: {
             "button.btn": {
                 "background-color": theme.colors.light,
-                "color": theme.colors.dark,
+                "color": theme.colors.black,
                 "margin": "8px 10px 8px 0px",
-                "padding": "10px 20px",
-                "border": f"1px solid {theme.colors.light.darken(0.2)}",
+                "padding": "10px 17px",
+                "border": f"1px solid {theme.colors.light.darken(0.1)}",
                 "border-radius": "4px",
                 "cursor": "pointer",
                 "font-size": theme.fonts.sizes.medium,
                 "transition": "0.1s filter linear, 0.1s -webkit-filter linear",
             },
             "button.btn:hover": {
                 "filter": "brightness(85%)",
@@ -45,16 +45,17 @@
     The component creates a button with the ``btn btn-primary`` class.
     """
 
     classes = ["btn", "btn-primary"]
     styles = style.use(
         lambda theme: {
             "button.btn-primary": {
+                "color": theme.colors.primary.readable(),
                 "background-color": theme.colors.primary,
-                "border-color": theme.colors.primary.darken(0.2),
+                "border-color": theme.colors.primary.darken(0.05),
             }
         }
     )
 
 
 class ButtonSecondary(Button):
     """Simple component creating an HTML button.
@@ -62,16 +63,17 @@
     The component creates a button with the ``btn btn-secondary`` class.
     """
 
     classes = ["btn", "btn-secondary"]
     styles = style.use(
         lambda theme: {
             "button.btn-secondary": {
+                "color": theme.colors.secondary.readable(),
                 "background-color": theme.colors.secondary,
-                "border-color": theme.colors.secondary.darken(0.2),
+                "border-color": theme.colors.secondary.darken(0.05),
             }
         }
     )
 
 
 class ButtonSuccess(Button):
     """Simple component creating an HTML button.
@@ -79,16 +81,17 @@
     The component creates a button with the ``btn btn-success`` class.
     """
 
     classes = ["btn", "btn-success"]
     styles = style.use(
         lambda theme: {
             "button.btn-success": {
+                "color": theme.colors.success.readable(),
                 "background-color": theme.colors.success,
-                "border-color": theme.colors.success.darken(0.2),
+                "border-color": theme.colors.success.darken(0.05),
             }
         }
     )
 
 
 class ButtonDanger(Button):
     """Simple component creating an HTML button.
@@ -96,16 +99,17 @@
     The component creates a button with the ``btn btn-danger`` class.
     """
 
     classes = ["btn", "btn-danger"]
     styles = style.use(
         lambda theme: {
             "button.btn-danger": {
+                "color": theme.colors.danger.readable(),
                 "background-color": theme.colors.danger,
-                "border-color": theme.colors.danger.darken(0.2),
+                "border-color": theme.colors.danger.darken(0.05),
             }
         }
     )
 
 
 class ButtonWarning(Button):
     """Simple component creating an HTML button.
@@ -113,16 +117,17 @@
     The component creates a button with the ``btn btn-warning`` class.
     """
 
     classes = ["btn", "btn-warning"]
     styles = style.use(
         lambda theme: {
             "button.btn-warning": {
+                "color": theme.colors.warning.readable(),
                 "background-color": theme.colors.warning,
-                "border-color": theme.colors.warning.darken(0.2),
+                "border-color": theme.colors.warning.darken(0.05),
             }
         }
     )
 
 
 class ButtonInfo(Button):
     """Simple component creating an HTML button.
@@ -130,12 +135,13 @@
     The component creates a button with the ``btn btn-info`` class.
     """
 
     classes = ["btn", "btn-info"]
     styles = style.use(
         lambda theme: {
             "button.btn-info": {
+                "color": theme.colors.info.readable(),
                 "background-color": theme.colors.info,
-                "border-color": theme.colors.info.darken(0.2),
+                "border-color": theme.colors.info.darken(0.05),
             }
         }
     )
```

### Comparing `ludic-0.3.0/ludic/catalog/forms.py` & `ludic-0.3.1/ludic/catalog/forms.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/catalog/items.py` & `ludic-0.3.1/ludic/catalog/items.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/catalog/loaders.py` & `ludic-0.3.1/ludic/catalog/loaders.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/catalog/navigation.py` & `ludic-0.3.1/ludic/catalog/navigation.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/catalog/quotes.py` & `ludic-0.3.1/ludic/catalog/quotes.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 class Quote(ComponentStrict[str, QuoteAttrs]):
     """Simple component rendering as the HTML ``blockquote`` element."""
 
     classes = ["quote"]
     styles = style.use(
         lambda theme: {
             ".quote": {
-                "margin-bottom": "40px",  # type: ignore
+                "margin-bottom": "20px",  # type: ignore
                 "blockquote": {
                     "background-color": theme.colors.light,
                     "border-left": f"8px solid {theme.colors.light.darken(0.1)}",
                     "margin": "0",
                     "margin-bottom": "10px",
                     "padding": "15px",
                 },
                 "blockquote p": {
-                    "font-size": theme.fonts.sizes.large,
+                    "font-size": theme.fonts.sizes.medium,
                     "margin-bottom": "10px",
                 },
                 "footer": {
-                    "font-size": theme.fonts.sizes.medium,
+                    "font-size": theme.fonts.sizes.small,
                     "margin-top": "10px",
                     "color": theme.colors.dark.lighten(0.5),
                 },
                 "footer a": {
                     "text-decoration": "none",
                     "color": theme.colors.dark.darken(0.5),
                 },
@@ -44,13 +44,13 @@
             }
         }
     )
 
     @override
     def render(self) -> div:
         children: list[BaseElement] = [
-            blockquote(*map(p, self.children[0].split("\n")))
+            blockquote(*map(p, self.children[0].split("\n\n")))
         ]
         if source_url := self.attrs.get("source_url"):
             source_text = self.attrs.get("source_text", "Source: ")
             children.append(footer(source_text, a(source_url, href=source_url)))
         return div(*children)
```

### Comparing `ludic-0.3.0/ludic/catalog/tables.py` & `ludic-0.3.1/ludic/catalog/tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
     classes = ["table-row"]
     styles = style.use(
         lambda theme: {
             "tr.table-row td": {
                 "border": f"1px solid {theme.colors.light.darken(0.2)}",
                 "padding": "12px",
+                "font-size": theme.fonts.sizes.medium,
             }
         }
     )
 
     def get_value(self, index: int) -> PrimitiveChildren | None:
         if len(self.children) > index:
             child = self.children[index]
@@ -91,14 +92,15 @@
 
     classes = ["table-head"]
     styles = style.use(
         lambda theme: {
             "tr.table-head th": {
                 "border": f"1px solid {theme.colors.light.darken(0.2)}",
                 "padding": "12px",
+                "font-size": theme.fonts.sizes.medium,
             }
         }
     )
 
     @property
     def header(self) -> tuple[PrimitiveChildren, ...]:
         return tuple(
@@ -147,14 +149,15 @@
 
     classes = ["table"]
     styles = style.use(
         lambda theme: {
             "table.table": {
                 "width": "100%",  # type: ignore
                 "border-collapse": "collapse",  # type: ignore
+                "margin-bottom": "15px",  # type: ignore
                 "thead": {
                     "background-color": theme.colors.light,
                 },
                 "button.btn": {
                     "margin": "0 5px",
                 },
             }
```

### Comparing `ludic-0.3.0/ludic/styles/collect.py` & `ludic-0.3.1/ludic/styles/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     theme = theme or get_default_theme()
 
     for component in components:
         styles = getattr(component, "styles", {})
 
         if not isinstance(styles, Mapping):
             continue
-        elif hasattr(styles, "theme"):
-            styles.theme = theme
+        elif hasattr(styles, "context"):
+            styles.context["theme"] = theme
 
         for key, value in styles.items():
             if isinstance(value, Mapping):
                 all_styles[key] = value
 
     return all_styles
```

### Comparing `ludic-0.3.0/ludic/styles/themes.py` & `ludic-0.3.1/ludic/styles/themes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Literal, Self, TypeVar
 
-from .utils import darken_color, hex_to_rgb, lighten_color
+from .utils import darken_color, hex_to_rgb, lighten_color, pick_readable_color_for
 
 if TYPE_CHECKING:
     from ludic.types import BaseElement
 
 _T = TypeVar("_T", bound="BaseElement")
 
 
@@ -36,14 +36,25 @@
             factor (float, optional): Lightening factor. Defaults to 0.5.
 
         Returns:
             str: Lightened color.
         """
         return type(self)(lighten_color(self, factor))
 
+    def readable(self) -> Self:
+        """Get lighter or darker variant of the given color depending on the luminance.
+
+        Args:
+            color (str): Color to find the readable opposite for.
+
+        Returns:
+            str: Readable opposite of the given color.
+        """
+        return type(self)(pick_readable_color_for(self))
+
 
 class Size(str):
     """Size class."""
 
     value: float
     unit: Literal["px", "em"] = "px"  # Default unit is pixels
 
@@ -83,34 +94,35 @@
         return type(self)(self.value - float(self.value * factor), self.unit)
 
 
 @dataclass
 class Colors:
     """Colors for a theme."""
 
-    primary: Color = Color("#0d6efd")
-    secondary: Color = Color("#6c757d")
-    success: Color = Color("#198754")
-    info: Color = Color("#0dcaf0")
-    warning: Color = Color("#ffc107")
-    danger: Color = Color("#dc3545")
+    primary: Color = Color("#4ecdc4")
+    secondary: Color = Color("#fefefe")
+    success: Color = Color("#c7f464")
+    info: Color = Color("#fce303")
+    warning: Color = Color("#fc9003")
+    danger: Color = Color("#e32929")
+
+    light: Color = Color("#f8f8f8")
+    dark: Color = Color("#414549")
 
-    dark: Color = Color("#313539")
-    light: Color = Color("#f8f9fa")
     white: Color = Color("#fff")
     black: Color = Color("#222")
 
 
 @dataclass
 class FontSizes:
     """Font sizes for a theme."""
 
-    small: Size = Size(12)
-    medium: Size = Size(16)
-    large: Size = Size(20)
+    small: Size = Size(14)
+    medium: Size = Size(18)
+    large: Size = Size(24)
 
 
 @dataclass
 class FontFamilies:
     """Font families for a theme."""
 
     headers: str = "serif"
@@ -147,44 +159,46 @@
 
         Args:
             element (_T): Element to apply the theme to.
 
         Returns:
             _T: The element with the theme applied.
         """
-        element.theme = self
+        element.context["theme"] = self
         return element
 
 
 @dataclass
 class DarkTheme(Theme):
     """The dark theme."""
 
     name: str = "dark"
 
+    colors: Colors = field(
+        default_factory=lambda: Colors(
+            primary=Color("#0d6efd"),
+            secondary=Color("#6c757d"),
+            success=Color("#198754"),
+            info=Color("#0dcaf0"),
+            warning=Color("#ffc107"),
+            danger=Color("#dc3545"),
+            light=Color("#414549"),
+            dark=Color("#f8f8f8"),
+            white=Color("#000"),
+            black=Color("#fff"),
+        )
+    )
+
 
 @dataclass
 class LightTheme(Theme):
     """Light theme."""
 
     name: str = "light"
 
-    colors: Colors = field(
-        default_factory=lambda: Colors(
-            primary=Color("#c2e7fd"),
-            secondary=Color("#fefefe"),
-            success=Color("#c9ffad"),
-            info=Color("#fff080"),
-            warning=Color("#ffc280"),
-            danger=Color("#ffaca1"),
-            light=Color("#f8f8f8"),
-            dark=Color("#414549"),
-        )
-    )
-
 
 _DEFAULT_THEME: Theme = LightTheme()
 
 
 def get_default_theme() -> Theme:
     """Get the default theme."""
     return _DEFAULT_THEME
```

### Comparing `ludic-0.3.0/ludic/styles/types.py` & `ludic-0.3.1/ludic/styles/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/styles/utils.py` & `ludic-0.3.1/ludic/styles/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,28 @@
 
     Returns:
         str: Hex color.
     """
     return f"#{int(rgb[0]):02x}{int(rgb[1]):02x}{int(rgb[2]):02x}"
 
 
+def pick_readable_color_for(color: str) -> str:
+    """Get lighter or darker color variant of the given one depending on the luminance.
+
+    Args:
+        color (str): Color to find the readable opposite for.
+
+    Returns:
+        str: Readable opposite of the given color.
+    """
+    rgb = color if isinstance(color, tuple) else hex_to_rgb(color)
+    _, luminance, _ = colorsys.rgb_to_hls(*rgb)
+    return "#000" if luminance > 140 else "#fff"
+
+
 def scale_color(color: str, factor: float = 0.5) -> str:
     """Scale a color by a given factor.
 
     Args:
         color (str): Color to scale.
         factor (float, optional): Scaling factor. Defaults to 0.5.
 
@@ -50,15 +64,15 @@
     """
     rgb = color if isinstance(color, tuple) else hex_to_rgb(color)
     hue, luminance, saturation = colorsys.rgb_to_hls(*rgb)
 
     if factor < 1:
         new_luminance = luminance * factor
     else:
-        new_luminance = (255 - luminance) * (factor - 1)
+        new_luminance = luminance + (255 - luminance) * (factor - 1)
 
     result = colorsys.hls_to_rgb(hue, min(255, max(1, new_luminance)), saturation)
     return rgb_to_hex(result)
 
 
 def darken_color(color: str, factor: float = 0.5) -> str:
     """Darken a color by a given factor.
```

### Comparing `ludic-0.3.0/ludic/web/app.py` & `ludic-0.3.1/ludic/web/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,14 @@
         path: str,
         include_in_schema: bool = True,
     ) -> Callable[[type[TEndpoint]], type[TEndpoint]]:
         """Register a Ludic class endpoint to the application."""
 
         def register(endpoint: type[TEndpoint]) -> type[TEndpoint]:
             self.add_route(path, endpoint, include_in_schema=include_in_schema)
-            endpoint.app = self
             return endpoint
 
         return register
 
     def add_route(
         self,
         path: str,
```

### Comparing `ludic-0.3.0/ludic/web/endpoints.py` & `ludic-0.3.1/ludic/web/endpoints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import inspect
 from collections.abc import Callable
-from typing import Any, ClassVar, Protocol
+from typing import Any, ClassVar, Protocol, cast
 
+from starlette.datastructures import URL
 from starlette.endpoints import HTTPEndpoint as BaseEndpoint
-from starlette.requests import Request
 from starlette.routing import Route
 
 from ludic.catalog.loaders import LazyLoader
 from ludic.types import AnyChildren, Component, NoChildren, TAttrs
 from ludic.utils import get_element_generic_args
 
-from .datastructures import URLPath
+from .requests import Request
 from .responses import prepare_response
 
 
-class AppProtocol(Protocol):
-    def url_path_for(self, name: str, /, **path_params: Any) -> URLPath: ...
-
-
 class RoutedProtocol(Protocol):
     route: ClassVar[Route]
 
 
 class HTTPEndpoint(BaseEndpoint):
     """Endpoint class for Ludic components.
 
@@ -50,15 +46,14 @@
         await response(self.scope, self.receive, self.send)
 
 
 class Endpoint(Component[NoChildren, TAttrs]):
     """Base class for Ludic endpoints."""
 
     route: ClassVar[Route]
-    app: ClassVar[AppProtocol]
 
     def lazy_load(
         self,
         endpoint: type[RoutedProtocol],
         placeholder: AnyChildren = "Loading ...",
         **kwargs: Any,
     ) -> LazyLoader:
@@ -70,27 +65,27 @@
             **kwargs: URL path parameters.
         """
         return LazyLoader(
             placeholder=placeholder,
             load_url=self.url_for(endpoint, **kwargs),
         )
 
-    def url_for(
-        self, endpoint: type[RoutedProtocol] | str, **path_params: Any
-    ) -> URLPath:
+    def url_for(self, endpoint: type[RoutedProtocol] | str, **path_params: Any) -> URL:
         """Get URL for an endpoint.
 
         Args:
             endpoint: The endpoint.
             **path_params: URL path parameters.
 
         Returns:
             The URL.
         """
-        if not hasattr(self, "app"):
+        request = self.context.get("request")
+
+        if request is None or not isinstance(request, Request):
             raise RuntimeError(
                 f"{type(self).__name__} is not bound to an app, you need to set the"
                 f"{type(self).__name__}.app property in order to use Endpoint.url_for."
             )
 
         if inspect.isclass(endpoint) and issubclass(endpoint, Endpoint):
             endpoint_generic_args = get_element_generic_args(endpoint)
@@ -103,9 +98,8 @@
             ):
                 path_params = {
                     key: value
                     for key, value in {**self.attrs, **path_params}.items()
                     if key in endpoint.route.param_convertors
                 }
 
-        endpoint_name = endpoint if isinstance(endpoint, str) else endpoint.route.name
-        return self.app.url_path_for(endpoint_name, **path_params)
+        return cast(URL, request.url_for(endpoint, **path_params))
```

### Comparing `ludic-0.3.0/ludic/web/exceptions.py` & `ludic-0.3.1/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/web/parsers.py` & `ludic-0.3.1/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/ludic/web/requests.py` & `ludic-0.3.1/ludic/web/requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,67 @@
+import itertools
 from collections.abc import Callable
 from typing import Any
 
+import starlette
 from starlette.datastructures import URL, URLPath
-from starlette.requests import Request as StarletteRequest
-from starlette.routing import Route, Router, get_name
+from starlette.routing import NoMatchFound, Route, Router
 
 
-class Request(StarletteRequest):
+def join_mounts(prefix: str, suffix: str) -> str:
+    """Join mount prefixes and suffixes.
+
+    Args:
+        prefix: The prefix to join.
+        suffix: The suffix to join.
+    """
+    prefixes = prefix.split(":")
+    suffixes = suffix.split(":")
+
+    for part in prefixes:
+        if suffixes and suffixes[0] == part:
+            suffixes.pop(0)
+
+    return ":".join(itertools.chain(prefixes, suffixes))
+
+
+class Request(starlette.requests.Request):
+    def url_path_for(
+        self, endpoint: str | Callable[..., Any], /, **path_params: Any
+    ) -> URLPath:
+        """Get URL path for an endpoint.
+
+        Args:
+            endpoint: The endpoint to get the URL path for, can be name or a registered
+                endpoint class.
+            **path_params: URL path parameters.
+
+        Returns:
+            The URL path.
+        """
+        router: Router = self.scope["router"]
+
+        if isinstance(endpoint, str):
+            endpoint_name = endpoint
+        elif (route := getattr(endpoint, "route", None)) and isinstance(route, Route):
+            endpoint_name = route.name
+        else:
+            raise NoMatchFound(str(endpoint), path_params)
+
+        if partial_mount := self.scope.get("partial_mount"):
+            endpoint_name = join_mounts(partial_mount, endpoint_name)
+
+        return router.url_path_for(endpoint_name, **path_params)
+
     def url_for(self, endpoint: str | Callable[..., Any], /, **path_params: Any) -> URL:
         """Get URL for an endpoint.
 
         Args:
             endpoint: The endpoint to get the URL for, can be name or a registered
                 endpoint class.
             **path_params: URL path parameters.
 
         Returns:
             The URL.
         """
-        url_path: URLPath
-        if (
-            not isinstance(endpoint, str)
-            and (route := getattr(endpoint, "route", None))
-            and isinstance(route, Route)
-        ):
-            url_path = route.url_path_for(route.name, **path_params)
-        else:
-            router: Router = self.scope["router"]
-            if not isinstance(endpoint, str):
-                endpoint = get_name(endpoint)
-            url_path = router.url_path_for(endpoint, **path_params)
+        url_path = self.url_path_for(endpoint, **path_params)
         return url_path.make_absolute_url(base_url=self.base_url)
```

### Comparing `ludic-0.3.0/ludic/web/responses.py` & `ludic-0.3.1/ludic/web/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
             raise ValueError(f"Invalid response tuple: {raw_response}")
 
     if raw_response is None:
         raw_response = ""
 
     response: Response
     if isinstance(raw_response, BaseElement):
+        raw_response.context["request"] = request
         response = LudicResponse(
             raw_response, status_code=status_code or 200, headers=headers
         )
     elif isinstance(raw_response, str | bool | int | float):
         response = PlainTextResponse(
             str(raw_response), status_code=status_code or 200, headers=headers
         )
```

### Comparing `ludic-0.3.0/ludic/web/routing.py` & `ludic-0.3.1/ludic/web/routing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import inspect
 from collections.abc import Callable
 from typing import Any
 
+from starlette import routing
 from starlette.exceptions import HTTPException
 from starlette.responses import PlainTextResponse, Response
-from starlette.routing import Host, Mount, get_name
-from starlette.routing import (
-    Route as StarletteRoute,
-)
-from starlette.routing import (
-    Router as StarletteRouter,
-)
+from starlette.routing import Host
 from starlette.types import Receive, Scope, Send
 
-from .datastructures import URLPath
 from .endpoints import Endpoint
 from .requests import Request
 from .responses import prepare_response
 
 __all__ = (
     "Host",
     "Mount",
     "Route",
     "Router",
 )
 
 
+class Mount(routing.Mount):
+    """Mount class for Ludic components."""
+
+    def matches(self, scope: Scope) -> tuple[routing.Match, Scope]:
+        match, scope = super().matches(scope)
+        if match == routing.Match.FULL:
+            if partial := scope.get("partial_mount"):
+                scope["partial_mount"] = f"{partial}:{self.name}"
+            else:
+                scope["partial_mount"] = self.name
+        return match, scope
+
+
 class _FunctionHandler:
     def __init__(self, handler: Callable[..., Any]) -> None:
         self.handler = handler
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         request = Request(scope, receive)
         response = await prepare_response(self.handler, request)
@@ -70,39 +77,35 @@
             return PlainTextResponse(
                 "Method Not Allowed", status_code=405, headers=headers
             )
 
         return make_response
 
 
-class Route(StarletteRoute):
+class Route(routing.Route):
     def __init__(
         self,
         path: str,
         endpoint: Callable[..., Any],
         *,
         name: str | None = None,
         **kwargs: Any,
     ) -> None:
-        name = get_name(endpoint) if name is None else name
+        name = routing.get_name(endpoint) if name is None else name
         wrapped_route = endpoint
         if inspect.isfunction(endpoint) or inspect.ismethod(endpoint):
             wrapped_route = _FunctionHandler(endpoint)
         elif inspect.isclass(endpoint) and issubclass(endpoint, Endpoint):
             wrapped_route = _EndpointHandler(endpoint)
         if getattr(endpoint, "route", None) is None:
             endpoint.route = self  # type: ignore
         super().__init__(path, wrapped_route, name=name, **kwargs)
 
-    def url_path_for(self, name: str, /, **path_params: Any) -> URLPath:
-        result = super().url_path_for(name, **path_params)
-        return URLPath(result, result.protocol, result.host)
-
 
-class Router(StarletteRouter):
+class Router(routing.Router):
     def add_route(
         self,
         path: str,
         endpoint: Callable[..., Any],
         methods: list[str] | None = None,
         name: str | None = None,
         include_in_schema: bool = True,
@@ -111,10 +114,7 @@
             path,
             endpoint=endpoint,
             methods=methods,
             name=name,
             include_in_schema=include_in_schema,
         )
         self.routes.append(route)
-
-    def url_path_for(self, name: str, /, **path_params: Any) -> URLPath:
-        return super().url_path_for(name, **path_params)  # type: ignore
```

### Comparing `ludic-0.3.0/tests/test_components.py` & `ludic-0.3.1/tests/test_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.catalog.typography import Link, Paragraph
 from ludic.html import b
 
 
 def test_link() -> None:
     link = Link("A link!", to="https://example.com")
-    assert link.to_html() == '<a href="https://example.com">A link!</a>'
+    assert link.to_html() == '<a href="https://example.com" class="link">A link!</a>'
 
 
 def test_paragraph() -> None:
     paragraph = Paragraph(
         "Hello, how ",
         b("are you"),
         "? Click ",
@@ -23,28 +23,31 @@
     assert paragraph.children[3].attrs["to"] == "https://example.com"
     assert paragraph.to_string(pretty=False) == (
         "<Paragraph>"
           'Hello, how <b>are you</b>? Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
-        '<p>Hello, how <b>are you</b>? Click <a href="https://example.com">here</a>.</p>'
-    )
+        '<p class="paragraph">'
+            'Hello, how <b>are you</b>? '
+            'Click <a href="https://example.com" class="link">here</a>.'
+        '</p>'
+    )  # fmt: skip
 
 
 def test_navigation() -> None:
     navigation = Navigation(
         NavItem("Home", to="/"),
         NavItem("About", to="/about"),
         id="nav",
     )
     assert navigation.to_html() == (
         '<ul id="nav" class="navigation">'
-            '<li id="home"><a href="/">Home</a></li>'
-            '<li id="about"><a href="/about">About</a></li>'
+            '<li id="home"><a href="/" class="link">Home</a></li>'
+            '<li id="about"><a href="/about" class="link">About</a></li>'
         "</ul>"
     )  # fmt: skip
 
 
 def test_pairs() -> None:
     pairs = Pairs(
         Key("Name"),
```

#### html2text {}

```diff
@@ -5,18 +5,18 @@
 import b def test_link() -> None: link = Link("A link!", to="https://
 example.com") assert link.to_html() == '_A_ _l_i_n_k_!' def test_paragraph() -> None:
 paragraph = Paragraph( "Hello, how ", b("are you"), "? Click ", Link("here",
 to="https://example.com"), ".", ) assert isinstance(paragraph.children[3],
 Link) assert paragraph.children[3].attrs["to"] == "https://example.com" assert
 paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
 here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
-Hello, how aarree yyoouu? Click _h_e_r_e.
-' ) def test_navigation() -> None: navigation = Navigation( NavItem("Home",
-to="/"), NavItem("About", to="/about"), id="nav", ) assert navigation.to_html()
-== ( '
+' 'Hello, how aarree yyoouu? ' 'Click _h_e_r_e.' '
+' ) # fmt: skip def test_navigation() -> None: navigation = Navigation( NavItem
+("Home", to="/"), NavItem("About", to="/about"), id="nav", ) assert
+navigation.to_html() == ( '
     * ' '
     * _H_o_m_e
     * ' '
     * _A_b_o_u_t
     * ' "
 " ) # fmt: skip def test_pairs() -> None: pairs = Pairs( Key("Name"), Value
 ("John"), Key("Age"), Value(42), ) assert pairs.to_html() == ( '
```

### Comparing `ludic-0.3.0/tests/test_elements.py` & `ludic-0.3.1/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/tests/test_examples.py` & `ludic-0.3.1/tests/test_examples.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from starlette.testclient import TestClient
 
-from examples import app
-
 
 def test_bulk_update() -> None:
-    from examples.bulk_update import db
+    from examples.bulk_update import app, db
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/people/").status_code == 200
         assert db.people["1"].active
         assert db.people["2"].active
         assert db.people["3"].active
@@ -17,19 +15,17 @@
         activate_data = {"active:id:1": "on", "active:id:2": "on"}
         assert client.post("/people/", data=activate_data).status_code == 200
         assert db.people["1"].active
         assert db.people["2"].active
         assert not db.people["3"].active
         assert not db.people["4"].active
 
-    app.routes.clear()
-
 
 def test_click_to_edit() -> None:
-    from examples.click_to_edit import db
+    from examples.click_to_edit import app, db
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/contacts/1").status_code == 200
         assert client.get("/contacts/1/form/").status_code == 200
         assert client.get("/contacts/123").status_code == 404
         assert client.get("/contacts/123/form/").status_code == 404
@@ -39,43 +35,37 @@
             "first_name": "Test",
             "last_name": "Doe",
             "email": "test@example.com",
         }
         assert client.put("/contacts/1", data=edit_data).status_code == 200
         assert db.contacts["1"].first_name == "Test"
 
-    app.routes.clear()
-
 
 def test_click_to_load() -> None:
-    import examples.click_to_load as _  # noqa
+    from examples.click_to_load import app
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/contacts/").status_code == 200
         assert client.get("/contacts/?page=2").status_code == 200
 
-    app.routes.clear()
-
 
 def test_delete_row() -> None:
-    from examples.delete_row import db
+    from examples.delete_row import app, db
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/people/").status_code == 200
         assert client.delete("/people/1").status_code == 200
         assert client.delete("/people/123").status_code == 404
         assert db.people.get("1") is None
 
-    app.routes.clear()
-
 
 def test_edit_row() -> None:
-    from examples.edit_row import db
+    from examples.edit_row import app, db
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/people/").status_code == 200
         assert client.get("/people/1").status_code == 200
         assert client.get("/people/1/form/").status_code == 200
         assert client.get("/people/123").status_code == 404
@@ -83,31 +73,25 @@
 
         assert db.people["1"].name == "Joe Smith"
         edit_data = {"name": "Test", "email": "test@example.com"}
         assert client.put("/people/1", data=edit_data).status_code == 200
         assert db.people["1"].name == "Test"
         assert db.people["1"].email == "test@example.com"
 
-    app.routes.clear()
-
 
 def test_lazy_loading() -> None:
-    import examples.lazy_loading as _  # noqa
+    from examples.lazy_loading import app
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         response = client.get("/load/0")
         assert response.status_code == 200
         assert b"Content Loaded" in response.content
 
-    app.routes.clear()
-
 
 def test_infinite_scroll() -> None:
-    import examples.infinite_scroll as _  # noqa
+    from examples.infinite_scroll import app
 
     with TestClient(app) as client:
         assert client.get("/").status_code == 200
         assert client.get("/contacts/").status_code == 200
         assert client.get("/contacts/?page=2").status_code == 200
-
-    app.routes.clear()
```

### Comparing `ludic-0.3.0/tests/test_exceptions.py` & `ludic-0.3.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/tests/test_formatting.py` & `ludic-0.3.1/tests/test_formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
     assert paragraph.children[3].attrs["to"] == "https://example.com"
     assert paragraph.to_string(pretty=False) == (
         "<Paragraph>"
           'Hello, how <strong>are you</strong>? Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
-        '<p>Hello, how <strong>are you</strong>? Click <a href="https://example.com">here</a>.</p>'
+        '<p class="paragraph">Hello, how <strong>are you</strong>? '
+        'Click <a href="https://example.com" class="link">here</a>.</p>'
     )
 
 
 def test_escaping_works() -> None:
     link = '<a href="https://example.com">test</a>'
     dom = p(f"Hello, how <b>are you</b>? Click {link}.")
     assert dom.to_html() == (
```

#### html2text {}

```diff
@@ -23,15 +23,15 @@
 {i("nested2")}")}") == div( "test ", div("foo ", b("nested"), ", ", i
 ("nested2")), ) assert context.get() == {} def test_component_with_f_string() -
 > None: paragraph = Paragraph( f"Hello, how {strong("are you")}? Click {Link
 ("here", to="https://example.com")}.", ) assert isinstance(paragraph.children
 [3], Link) assert paragraph.children[3].attrs["to"] == "https://example.com"
 assert paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
 here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
-Hello, how aarree yyoouu? Click _h_e_r_e.
+Hello, how aarree yyoouu? ' 'Click _h_e_r_e.
 ' ) def test_escaping_works() -> None: link = '_t_e_s_t' dom = p(f"Hello, how aarree
 yyoouu? Click {link}.") assert dom.to_html() == ( "
 Hello, how <b>are you</b>? " 'Click <a href="https://example.com">test</a>.
 ' ) def test_quotes_not_escaped() -> None: dom = p("It's alive <3.") assert
 dom.to_html() == "
 It's alive <3.
 "
```

### Comparing `ludic-0.3.0/tests/test_styles.py` & `ludic-0.3.1/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/tests/test_themes.py` & `ludic-0.3.1/tests/test_themes.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     assert theme.colors.white.darken(0.5).rgb == (127, 127, 127)
     assert theme.colors.white.darken(1).rgb == (1, 1, 1)
     assert theme.colors.black.lighten(0.5).rgb == (127, 127, 127)
     assert theme.colors.black.lighten(1).rgb == (255, 255, 255)
 
     assert theme.colors.light.darken(0.5).rgb == (119, 119, 119)
-    assert theme.colors.dark.lighten(0.5).rgb == (102, 102, 102)
+    assert theme.colors.dark.lighten(0.5).rgb == (153, 153, 153)
 
     assert theme.colors.primary.darken(0.5).rgb == (97, 115, 126)
 
 
 def test_theme_font_sizes() -> None:
     theme = LightTheme(
         fonts=Fonts(sizes=FontSizes(small=Size(10, "px"), medium=Size(1.2, unit="em"))),
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 theme.colors.white.rgb == (255, 255, 255) assert theme.colors.light.rgb ==
 (238, 238, 238) assert theme.colors.dark.rgb == (51, 51, 51) assert
 theme.colors.black.rgb == (0, 0, 0) assert theme.colors.white.darken(0.5).rgb
 == (127, 127, 127) assert theme.colors.white.darken(1).rgb == (1, 1, 1) assert
 theme.colors.black.lighten(0.5).rgb == (127, 127, 127) assert
 theme.colors.black.lighten(1).rgb == (255, 255, 255) assert
 theme.colors.light.darken(0.5).rgb == (119, 119, 119) assert
-theme.colors.dark.lighten(0.5).rgb == (102, 102, 102) assert
+theme.colors.dark.lighten(0.5).rgb == (153, 153, 153) assert
 theme.colors.primary.darken(0.5).rgb == (97, 115, 126) def
 test_theme_font_sizes() -> None: theme = LightTheme( fonts=Fonts
 (sizes=FontSizes(small=Size(10, "px"), medium=Size(1.2, unit="em"))), ) assert
 theme.fonts.sizes.small == "10px" assert theme.fonts.sizes.medium == "1.2em"
 def test_themes_switching() -> None: dark, light = DarkTheme(), LightTheme()
 assert get_default_theme() == light set_default_theme(dark) assert
 get_default_theme() == dark set_default_theme(light) assert get_default_theme()
```

### Comparing `ludic-0.3.0/tests/test_types.py` & `ludic-0.3.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/.gitignore` & `ludic-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/LICENCE` & `ludic-0.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.3.0/README.md` & `ludic-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Ludic
+<p align="center">
+    <img width="600px" src="./docs/assets/ludic.png" alt="ludic">
+</p>
 
 [![test](https://github.com/paveldedik/ludic/actions/workflows/test.yaml/badge.svg)](https://github.com/paveldedik/ludic/actions) [![codecov](https://codecov.io/gh/paveldedik/ludic/graph/badge.svg?token=BBDNJWHMGX)](https://codecov.io/gh/paveldedik/ludic) [![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-312/) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Documentation Status](https://readthedocs.org/projects/ludic/badge/?version=latest)](https://ludic.readthedocs.io/en/latest/?badge=latest)
 
 **Documentation**: https://ludic.readthedocs.io/
 
 Ludic is a lightweight framework for building HTML pages with a component approach similar to [React](https://react.dev/). It is built to be used together with [htmx.org](https://htmx.org/) so that developers don't need to write almost any JavaScript to create dynamic web services. Its potential can be leveraged together with its web framework which is a wrapper around the powerful [Starlette](https://www.starlette.io/) framework. It is built with the latest Python 3.12 features heavily incorporating typing.
```

### Comparing `ludic-0.3.0/pyproject.toml` & `ludic-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "D213",
     "UP040",
 ]
 fixable = ["ALL"]
 
 [tool.ruff.lint.isort]
 known-first-party = ["ludic"]
+known-third-party = ["examples"]
 
 [tool.mypy]
 python_version = "3.12"
 strict = true
 disallow_subclassing_any = false
 
 [tool.pytest.ini_options]
```

### Comparing `ludic-0.3.0/PKG-INFO` & `ludic-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,17 @@
 Requires-Dist: typeguard>=4.1.5; extra == 'full'
 Provides-Extra: test
 Requires-Dist: httpx; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Ludic
+<p align="center">
+    <img width="600px" src="./docs/assets/ludic.png" alt="ludic">
+</p>
 
 [![test](https://github.com/paveldedik/ludic/actions/workflows/test.yaml/badge.svg)](https://github.com/paveldedik/ludic/actions) [![codecov](https://codecov.io/gh/paveldedik/ludic/graph/badge.svg?token=BBDNJWHMGX)](https://codecov.io/gh/paveldedik/ludic) [![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-312/) [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![Documentation Status](https://readthedocs.org/projects/ludic/badge/?version=latest)](https://ludic.readthedocs.io/en/latest/?badge=latest)
 
 **Documentation**: https://ludic.readthedocs.io/
 
 Ludic is a lightweight framework for building HTML pages with a component approach similar to [React](https://react.dev/). It is built to be used together with [htmx.org](https://htmx.org/) so that developers don't need to write almost any JavaScript to create dynamic web services. Its potential can be leveraged together with its web framework which is a wrapper around the powerful [Starlette](https://www.starlette.io/) framework. It is built with the latest Python 3.12 features heavily incorporating typing.
```

