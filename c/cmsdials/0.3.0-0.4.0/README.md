# Comparing `tmp/cmsdials-0.3.0.tar.gz` & `tmp/cmsdials-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsdials-0.3.0.tar", max compression
+gzip compressed data, was "cmsdials-0.4.0.tar", max compression
```

## Comparing `cmsdials-0.3.0.tar` & `cmsdials-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,35 @@
--rw-r--r--   0        0        0    35149 2024-03-08 19:19:43.455206 cmsdials-0.3.0/LICENSE
--rw-r--r--   0        0        0     5292 2024-03-08 19:20:02.818221 cmsdials-0.3.0/README.md
--rw-r--r--   0        0        0       49 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/__init__.py
--rw-r--r--   0        0        0     4136 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/_base.py
--rw-r--r--   0        0        0     4998 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/bearer.py
--rw-r--r--   0        0        0     3491 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/client.py
--rw-r--r--   0        0        0      107 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/exceptions.py
--rw-r--r--   0        0        0      425 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/models.py
--rw-r--r--   0        0        0     1041 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/auth/secret_key.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/bad_file_index/__init__.py
--rw-r--r--   0        0        0      343 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/bad_file_index/client.py
--rw-r--r--   0        0        0     1066 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/bad_file_index/models.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/file_index/__init__.py
--rw-r--r--   0        0        0      318 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/file_index/client.py
--rw-r--r--   0        0        0     1520 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/file_index/models.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/h1d/__init__.py
--rw-r--r--   0        0        0      414 2024-03-08 19:19:43.456206 cmsdials-0.3.0/cmsdials/clients/h1d/client.py
--rw-r--r--   0        0        0     1167 2024-03-08 19:20:02.818221 cmsdials-0.3.0/cmsdials/clients/h1d/models.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/h2d/__init__.py
--rw-r--r--   0        0        0      414 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/h2d/client.py
--rw-r--r--   0        0        0     1334 2024-03-08 19:20:02.818221 cmsdials-0.3.0/cmsdials/clients/h2d/models.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/lumisection/__init__.py
--rw-r--r--   0        0        0      737 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/lumisection/client.py
--rw-r--r--   0        0        0      790 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/lumisection/models.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/run/__init__.py
--rw-r--r--   0        0        0      269 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/run/client.py
--rw-r--r--   0        0        0      736 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/clients/run/models.py
--rw-r--r--   0        0        0      986 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/cmsdials.py
--rw-r--r--   0        0        0      529 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/filters.py
--rw-r--r--   0        0        0        0 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/utils/__init__.py
--rw-r--r--   0        0        0      671 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/utils/_json.py
--rw-r--r--   0        0        0     4574 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/utils/api_client.py
--rw-r--r--   0        0        0      174 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/utils/base_model.py
--rw-r--r--   0        0        0      145 2024-03-08 19:19:43.457206 cmsdials-0.3.0/cmsdials/utils/logger.py
--rw-r--r--   0        0        0      784 2024-03-08 19:21:01.601268 cmsdials-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6226 1970-01-01 00:00:00.000000 cmsdials-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-28 16:14:27.566813 cmsdials-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5345 2024-04-11 21:19:49.049949 cmsdials-0.4.0/README.md
+-rw-r--r--   0        0        0       49 2024-03-06 14:04:55.052320 cmsdials-0.4.0/cmsdials/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 11:33:02.539393 cmsdials-0.4.0/cmsdials/auth/__init__.py
+-rw-r--r--   0        0        0     4136 2024-03-06 14:44:11.087545 cmsdials-0.4.0/cmsdials/auth/_base.py
+-rw-r--r--   0        0        0     4998 2024-04-09 11:53:11.488972 cmsdials-0.4.0/cmsdials/auth/bearer.py
+-rw-r--r--   0        0        0     3491 2024-03-06 14:44:11.092545 cmsdials-0.4.0/cmsdials/auth/client.py
+-rw-r--r--   0        0        0      107 2024-03-06 14:46:20.706557 cmsdials-0.4.0/cmsdials/auth/exceptions.py
+-rw-r--r--   0        0        0      425 2024-03-01 14:52:11.874008 cmsdials-0.4.0/cmsdials/auth/models.py
+-rw-r--r--   0        0        0     1041 2024-04-09 10:09:21.911337 cmsdials-0.4.0/cmsdials/auth/secret_key.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:09:10.635273 cmsdials-0.4.0/cmsdials/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:10:09.799214 cmsdials-0.4.0/cmsdials/clients/file_index/__init__.py
+-rw-r--r--   0        0        0      318 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/file_index/client.py
+-rw-r--r--   0        0        0      988 2024-04-11 21:19:49.049949 cmsdials-0.4.0/cmsdials/clients/file_index/models.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:10:14.034210 cmsdials-0.4.0/cmsdials/clients/h1d/__init__.py
+-rw-r--r--   0        0        0      414 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/h1d/client.py
+-rw-r--r--   0        0        0     1143 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/h1d/models.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:10:18.548206 cmsdials-0.4.0/cmsdials/clients/h2d/__init__.py
+-rw-r--r--   0        0        0      414 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/h2d/client.py
+-rw-r--r--   0        0        0     1188 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/h2d/models.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:10:24.058200 cmsdials-0.4.0/cmsdials/clients/lumisection/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/lumisection/client.py
+-rw-r--r--   0        0        0      671 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/lumisection/models.py
+-rw-r--r--   0        0        0        0 2024-02-29 13:10:29.247195 cmsdials-0.4.0/cmsdials/clients/run/__init__.py
+-rw-r--r--   0        0        0      269 2024-03-07 16:12:57.394240 cmsdials-0.4.0/cmsdials/clients/run/client.py
+-rw-r--r--   0        0        0      452 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/clients/run/models.py
+-rw-r--r--   0        0        0      943 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/cmsdials.py
+-rw-r--r--   0        0        0      439 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/filters.py
+-rw-r--r--   0        0        0        0 2024-03-01 09:40:35.448258 cmsdials-0.4.0/cmsdials/utils/__init__.py
+-rw-r--r--   0        0        0      671 2024-03-06 14:48:21.185636 cmsdials-0.4.0/cmsdials/utils/_json.py
+-rw-r--r--   0        0        0     4827 2024-04-11 21:19:49.050949 cmsdials-0.4.0/cmsdials/utils/api_client.py
+-rw-r--r--   0        0        0      174 2024-03-01 09:40:15.133277 cmsdials-0.4.0/cmsdials/utils/base_model.py
+-rw-r--r--   0        0        0      145 2024-03-06 14:44:10.568545 cmsdials-0.4.0/cmsdials/utils/logger.py
+-rw-r--r--   0        0        0      784 2024-04-11 21:19:49.050949 cmsdials-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6279 1970-01-01 00:00:00.000000 cmsdials-0.4.0/PKG-INFO
```

### Comparing `cmsdials-0.3.0/LICENSE` & `cmsdials-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/README.md` & `cmsdials-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -55,46 +55,51 @@
 creds = Credentials.from_creds_file()
 dials = Dials(creds, nthreads=2)
 
 # Getting h1d data
 data = dials.h1d.list_all(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
 ```
 
+### Workspace
+
+Users are automatically routed to a workspace based on e-groups, but it is possible to overwrite this configuration and inspect data from others workspaces:
+
+```python
+dials = Dials(creds, workspace="jetmet", nthreads=2)
+```
+
 ## Available endpoints
 
 This package interacts with DIALS api endpoints using underlying classes in `Dials` object.
 
 ### Retrieving a specific object using `get`
 
 ```python
-dials.bad_file_index.get(id=1)
 dials.file_index.get(id=1)
 dials.h1d.get(id=1)
 dials.h2d.get(id=1)
 dials.lumi.get(id=1)
 dials.run.get(id=1)
 ```
 
 ### Retrieving a list of objects per page using `list`
 
 It is possible to get a list of entries from those endpoint using the `list` and `list_all` methods, the `list` method will fetch only one page and the `list_all` will fetch all available pages:
 
 ```python
-dials.bad_file_index.list()
 dials.file_index.list()
 dials.h1d.list()
 dials.h2d.list()
 dials.lumi.list()
 dials.run.list()
 ```
 
 ### Retrieving all available pages of a list of objects using `list_all`
 
 ```python
-dials.bad_file_index.list_all()
 dials.file_index.list_all()
 dials.h1d.list_all()
 dials.h2d.list_all()
 dials.lumi.list_all()
 dials.run.list_all()
 ```
 
@@ -106,23 +111,21 @@
 
 ### Using filters
 
 Keep in mind that calling those methods without any filter can take a lot of time, because the underlying query will try to load the entire database table through multiple requests, then it is recommended to apply filters according to DIALS [live documentation](https://cmsdials-api.web.cern.ch/api/v1/swagger#/) using filter classes for each table:
 
 ```python
 from cmsdials.filters import (
-    BadFileIndexFilters,
     FileIndexFilters,
     LumisectionHistogram1DFilters,
     LumisectionHistogram2DFilters,
     LumisectionFilters,
     RunFilters
 )
 
-dials.bad_file_index.list(BadFileIndexFilters(path_contains="ZeroBias"))
 
 dials.file_index.list(FileIndexFilters(page="10"))
 
 dials.h1d.list(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2", page="15"))
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
 
@@ -146,15 +149,15 @@
 ```python
 from cmsdials.auth.client import AuthClient
 from cmsdials.auth.bearer import Credentials
 from cmsdials import Dials
 from cmsdials.filters import LumisectionHistogram2DFilters
 
 DEV_URL = "http://localhost:8000/"
-DEV_CACHE_DIR = ".cache-dev
+DEV_CACHE_DIR = ".cache-dev"
 
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
 dials = Dials(creds, nthreads=2, base_url=DEV_URL)
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
 ```
```

### Comparing `cmsdials-0.3.0/cmsdials/auth/_base.py` & `cmsdials-0.4.0/cmsdials/auth/_base.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/cmsdials/auth/bearer.py` & `cmsdials-0.4.0/cmsdials/auth/bearer.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/cmsdials/auth/client.py` & `cmsdials-0.4.0/cmsdials/auth/client.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/cmsdials/auth/secret_key.py` & `cmsdials-0.4.0/cmsdials/auth/secret_key.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/cmsdials/clients/h1d/models.py` & `cmsdials-0.4.0/cmsdials/clients/h1d/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-from datetime import datetime
 from typing import List, Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class LumisectionHistogram1D(BaseModel):
-    id: int
-    ls_number: int
+    hist_id: int
+    file_id: int
     run_number: int
-    date: datetime
+    ls_id: int
     title: str = Field(..., max_length=220)
-    entries: int
-    data: list[float]
     x_min: float
     x_max: float
-    x_bin: int
-    source_data_file: int
-    lumisection: int
+    x_bin: float
+    entries: int
+    data: list[float]
 
 
 class PaginatedLumisectionHistogram1DList(BaseModel):
     count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: List[LumisectionHistogram1D]
 
 
 class LumisectionHistogram1DFilters(OBaseModel):
-    ls_number: Optional[int] = None
-    lumisection_id: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    max_run_number: Optional[int] = None
-    min_entries: Optional[int] = None
-    min_ls_number: Optional[int] = None
-    min_run_number: Optional[int] = None
     page: Optional[str] = None
     run_number: Optional[int] = None
+    ls_number: Optional[int] = None
+    ls_id: Optional[int] = None
     title: Optional[str] = None
+    min_run_number: Optional[int] = None
+    max_run_number: Optional[int] = None
+    min_ls_number: Optional[int] = None
+    max_ls_number: Optional[int] = None
     title_contains: Optional[str] = None
+    min_entries: Optional[int] = None
     era: Optional[str] = None
-    dqmio_filepath_contains: Optional[str] = None
+    campaign: Optional[str] = None
+    primary_dataset: Optional[str] = None
+    file_id: Optional[int] = None
```

### Comparing `cmsdials-0.3.0/cmsdials/clients/h2d/models.py` & `cmsdials-0.4.0/cmsdials/clients/h2d/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,46 @@
-from datetime import datetime
 from typing import Optional
 
 from pydantic import AnyUrl, BaseModel, Field
 
 from ...utils.base_model import OBaseModel
 
 
 class LumisectionHistogram2D(BaseModel):
-    id: int
-    ls_number: int
+    hist_id: int
+    file_id: int
     run_number: int
-    date: datetime
+    ls_id: int
     title: str = Field(..., max_length=220)
-    entries: int
-    data: list[list[float]]
     x_min: float
     x_max: float
-    x_bin: int
-    y_max: float
+    x_bin: float
     y_min: float
-    y_bin: int
-    source_data_file: int = Field(
-        ...,
-        description="Source data file that the specific Histogram was read from, if any",
-    )
-    lumisection: int
+    y_max: float
+    y_bin: float
+    entries: int
+    data: list[float]
 
 
 class PaginatedLumisectionHistogram2DList(BaseModel):
     count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: list[LumisectionHistogram2D]
 
 
 class LumisectionHistogram2DFilters(OBaseModel):
-    ls_number: Optional[int] = None
-    lumisection_id: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    max_run_number: Optional[int] = None
-    min_entries: Optional[int] = None
-    min_ls_number: Optional[int] = None
-    min_run_number: Optional[int] = None
     page: Optional[str] = None
     run_number: Optional[int] = None
+    ls_number: Optional[int] = None
+    ls_id: Optional[int] = None
     title: Optional[str] = None
+    min_run_number: Optional[int] = None
+    max_run_number: Optional[int] = None
+    min_ls_number: Optional[int] = None
+    max_ls_number: Optional[int] = None
     title_contains: Optional[str] = None
+    min_entries: Optional[int] = None
     era: Optional[str] = None
-    dqmio_filepath_contains: Optional[str] = None
+    campaign: Optional[str] = None
+    primary_dataset: Optional[str] = None
+    file_id: Optional[int] = None
```

### Comparing `cmsdials-0.3.0/cmsdials/clients/lumisection/models.py` & `cmsdials-0.4.0/cmsdials/clients/lumisection/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,29 @@
-from datetime import datetime
-from typing import List, Optional
+from typing import Optional
 
 from pydantic import AnyUrl, BaseModel
 
 from ...utils.base_model import OBaseModel
 
 
 class Lumisection(BaseModel):
-    id: int
+    ls_id: int
     ls_number: int
-    date: datetime
-    oms_zerobias_rate: Optional[float]
-    run: int
+    th1_count: int
+    th2_count: int
 
 
 class PaginatedLumisectionList(BaseModel):
     count: int
     next: Optional[AnyUrl]
     previous: Optional[AnyUrl]
     results: list[Lumisection]
 
 
 class LumisectionFilters(OBaseModel):
+    page: Optional[str] = None
+    run_number: Optional[int] = None
     ls_number: Optional[int] = None
-    max_ls_number: Optional[int] = None
-    max_run_number: Optional[int] = None
     min_ls_number: Optional[int] = None
+    max_ls_number: Optional[int] = None
     min_run_number: Optional[int] = None
-    page: Optional[str] = None
-    run_number: Optional[int] = None
-
-
-class ConfiguredMEs(BaseModel):
-    mes: List[str]
+    max_run_number: Optional[int] = None
```

### Comparing `cmsdials-0.3.0/cmsdials/utils/_json.py` & `cmsdials-0.4.0/cmsdials/utils/_json.py`

 * *Files identical despite different names*

### Comparing `cmsdials-0.3.0/cmsdials/utils/api_client.py` & `cmsdials-0.4.0/cmsdials/utils/api_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,39 +34,52 @@
 
 class BaseAuthorizedAPIClient(BaseAPIClient):
     data_model = None
     pagination_model = None
     filter_class = None
     lookup_url = None
 
-    def __init__(self, creds: BaseCredentials, nthreads: Optional[int] = None, *args: str, **kwargs: str) -> None:
+    def __init__(
+        self,
+        creds: BaseCredentials,
+        workspace: Optional[str] = None,
+        nthreads: Optional[int] = None,
+        *args: str,
+        **kwargs: str,
+    ) -> None:
         super().__init__(*args, **kwargs)
         self.creds = creds
+        self.workspace = workspace
         self.nthreads = nthreads or 1
 
+    def __build_headers(self) -> dict:
+        base = {"accept": "application/json"}
+        if self.workspace is not None:
+            base["Workspace"] = self.workspace
+        self.creds.before_request(base)
+        return base
+
     def get(self, id: str):
         endpoint_url = self.api_url + self.lookup_url + str(id) + "/"
-        headers = {"accept": "application/json"}
-        self.creds.before_request(headers)
+        headers = self.__build_headers()
         response = requests.get(endpoint_url, headers=headers)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
 
         response = response.json()
         return self.data_model(**response)
 
     def list(self, filters=None):
         filters = filters or self.filter_class()
         endpoint_url = self.api_url + self.lookup_url
-        headers = {"accept": "application/json"}
-        self.creds.before_request(headers)
+        headers = self.__build_headers()
         response = requests.get(endpoint_url, headers=headers, params=filters.cleandict())
 
         try:
             response.raise_for_status()
         except HTTPError as err:
             logger.info(f"Api raw response: {response.text}")
             raise err
```

### Comparing `cmsdials-0.3.0/pyproject.toml` & `cmsdials-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmsdials"
-version = "0.3.0"
+version = "0.4.0"
 description = "The Python api client interface to DIALS service"
 authors = ["Gabriel Moreira <gabrielmscampos@gmail.com>"]
 readme = "README.md"
 include = ["LICENSE"]
 repository = "https://github.com/cms-DQM/dials-py"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `cmsdials-0.3.0/PKG-INFO` & `cmsdials-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsdials
-Version: 0.3.0
+Version: 0.4.0
 Summary: The Python api client interface to DIALS service
 Home-page: https://github.com/cms-DQM/dials-py
 Author: Gabriel Moreira
 Author-email: gabrielmscampos@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -78,46 +78,51 @@
 creds = Credentials.from_creds_file()
 dials = Dials(creds, nthreads=2)
 
 # Getting h1d data
 data = dials.h1d.list_all(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2"), max_pages=5)
 ```
 
+### Workspace
+
+Users are automatically routed to a workspace based on e-groups, but it is possible to overwrite this configuration and inspect data from others workspaces:
+
+```python
+dials = Dials(creds, workspace="jetmet", nthreads=2)
+```
+
 ## Available endpoints
 
 This package interacts with DIALS api endpoints using underlying classes in `Dials` object.
 
 ### Retrieving a specific object using `get`
 
 ```python
-dials.bad_file_index.get(id=1)
 dials.file_index.get(id=1)
 dials.h1d.get(id=1)
 dials.h2d.get(id=1)
 dials.lumi.get(id=1)
 dials.run.get(id=1)
 ```
 
 ### Retrieving a list of objects per page using `list`
 
 It is possible to get a list of entries from those endpoint using the `list` and `list_all` methods, the `list` method will fetch only one page and the `list_all` will fetch all available pages:
 
 ```python
-dials.bad_file_index.list()
 dials.file_index.list()
 dials.h1d.list()
 dials.h2d.list()
 dials.lumi.list()
 dials.run.list()
 ```
 
 ### Retrieving all available pages of a list of objects using `list_all`
 
 ```python
-dials.bad_file_index.list_all()
 dials.file_index.list_all()
 dials.h1d.list_all()
 dials.h2d.list_all()
 dials.lumi.list_all()
 dials.run.list_all()
 ```
 
@@ -129,23 +134,21 @@
 
 ### Using filters
 
 Keep in mind that calling those methods without any filter can take a lot of time, because the underlying query will try to load the entire database table through multiple requests, then it is recommended to apply filters according to DIALS [live documentation](https://cmsdials-api.web.cern.ch/api/v1/swagger#/) using filter classes for each table:
 
 ```python
 from cmsdials.filters import (
-    BadFileIndexFilters,
     FileIndexFilters,
     LumisectionHistogram1DFilters,
     LumisectionHistogram2DFilters,
     LumisectionFilters,
     RunFilters
 )
 
-dials.bad_file_index.list(BadFileIndexFilters(path_contains="ZeroBias"))
 
 dials.file_index.list(FileIndexFilters(page="10"))
 
 dials.h1d.list(LumisectionHistogram1DFilters(title="PixelPhase1/Tracks/PXBarrel/charge_PXLayer_2", page="15"))
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
 
@@ -169,15 +172,15 @@
 ```python
 from cmsdials.auth.client import AuthClient
 from cmsdials.auth.bearer import Credentials
 from cmsdials import Dials
 from cmsdials.filters import LumisectionHistogram2DFilters
 
 DEV_URL = "http://localhost:8000/"
-DEV_CACHE_DIR = ".cache-dev
+DEV_CACHE_DIR = ".cache-dev"
 
 auth = AuthClient(base_url=DEV_URL)
 creds = Credentials.from_creds_file(cache_dir=DEV_CACHE_DIR, client=auth)  # Make sure to specify the auth client with overwritten values, using another cache_dir is recommended
 dials = Dials(creds, nthreads=2, base_url=DEV_URL)
 
 dials.h2d.list_all(LumisectionHistogram2DFilters(title_contains="EEOT digi occupancy EE +", min_entries=100, min_run_number=360392, max_run_number=365000), max_pages=5)
 ```
```

