# Comparing `tmp/airbyte_source_google_sheets-0.5.0.tar.gz` & `tmp/airbyte_source_google_sheets-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_google_sheets-0.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_google_sheets-0.5.1.tar", max compression
```

## Comparing `airbyte_source_google_sheets-0.5.0.tar` & `airbyte_source_google_sheets-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4622 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/README.md
--rw-r--r--   0        0        0      870 2024-04-03 16:59:41.662228 airbyte_source_google_sheets-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       73 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/__init__.py
--rw-r--r--   0        0        0     2390 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/client.py
--rw-r--r--   0        0        0    10501 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/helpers.py
--rw-r--r--   0        0        0       61 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/__init__.py
--rw-r--r--   0        0        0     1109 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet.py
--rw-r--r--   0        0        0      437 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet_values.py
--rw-r--r--   0        0        0      237 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/run.py
--rw-r--r--   0        0        0    11688 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/source.py
--rw-r--r--   0        0        0     4149 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/spec.yaml
--rw-r--r--   0        0        0     2289 2024-04-03 16:36:04.000000 airbyte_source_google_sheets-0.5.0/source_google_sheets/utils.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 airbyte_source_google_sheets-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4622 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/README.md
+-rw-r--r--   0        0        0      870 2024-04-11 15:39:56.451225 airbyte_source_google_sheets-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/__init__.py
+-rw-r--r--   0        0        0     2391 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/client.py
+-rw-r--r--   0        0        0    10501 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/helpers.py
+-rw-r--r--   0        0        0       61 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/models/__init__.py
+-rw-r--r--   0        0        0     1109 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/models/spreadsheet.py
+-rw-r--r--   0        0        0      437 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/models/spreadsheet_values.py
+-rw-r--r--   0        0        0      237 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/run.py
+-rw-r--r--   0        0        0    11758 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/source.py
+-rw-r--r--   0        0        0     5141 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/spec.yaml
+-rw-r--r--   0        0        0     2289 2024-04-11 14:42:24.000000 airbyte_source_google_sheets-0.5.1/source_google_sheets/utils.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 airbyte_source_google_sheets-0.5.1/PKG-INFO
```

### Comparing `airbyte_source_google_sheets-0.5.0/README.md` & `airbyte_source_google_sheets-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.5.0/pyproject.toml` & `airbyte_source_google_sheets-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.5.0"
+version = "0.5.1"
 name = "airbyte-source-google-sheets"
 description = "Source implementation for Google Sheets."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
```

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/client.py` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class GoogleSheetsClient:
     class Backoff:
         row_batch_size = 200
 
         @classmethod
         def increase_row_batch_size(cls, details):
             if details["exception"].status_code == status_codes.TOO_MANY_REQUESTS and cls.row_batch_size < 1000:
-                cls.row_batch_size = cls.row_batch_size + 10
+                cls.row_batch_size = cls.row_batch_size + 100
                 logger.info(f"Increasing number of records fetching due to rate limits. Current value: {cls.row_batch_size}")
 
         @staticmethod
         def give_up(error):
             code = error.resp.status
             # Stop retrying if it's not a problem with the rate limit or on the server end
             return not (code == status_codes.TOO_MANY_REQUESTS or 500 <= code < 600)
```

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/helpers.py` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/models/spreadsheet.py` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/models/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/source.py` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     def _read(
         self,
         logger: AirbyteLogger,
         config: json,
         catalog: ConfiguredAirbyteCatalog,
     ) -> Generator[AirbyteMessage, None, None]:
         client = GoogleSheetsClient(self.get_credentials(config))
+        client.Backoff.row_batch_size = config.get("batch_size", 200)
 
         sheet_to_column_name = Helpers.parse_sheet_and_column_names_from_catalog(catalog)
         stream_name_to_stream = {stream.stream.name: stream for stream in catalog.streams}
         spreadsheet_id = Helpers.get_spreadsheet_id(config["spreadsheet_id"])
 
         logger.info(f"Starting syncing spreadsheet {spreadsheet_id}")
         # For each sheet in the spreadsheet, get a batch of rows, and as long as there hasn't been
```

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/spec.yaml` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/spec.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,29 @@
   title: Google Sheets Source Spec
   type: object
   required:
     - spreadsheet_id
     - credentials
   additionalProperties: true
   properties:
+    batch_size:
+      type: integer
+      title: Row Batch Size
+      description: >-
+        Default value is 200.
+        An integer representing row batch size for each sent request to Google Sheets API.
+        Row batch size means how many rows are processed from the google sheet, for example default value 200
+        would process rows 1-201, then 201-401 and so on.
+        Based on <a href='https://developers.google.com/sheets/api/limits'>Google Sheets API limits documentation</a>,
+        it is possible to send up to 300 requests per minute, but each individual request has to be processed under 180 seconds,
+        otherwise the request returns a timeout error. In regards to this information, consider network speed and
+        number of columns of the google sheet when deciding a batch_size value.
+        Default value should cover most of the cases, but if a google sheet has over 100,000 records or more,
+        consider increasing batch_size value.
+      default: 200
     spreadsheet_id:
       type: string
       title: Spreadsheet Link
       description: >-
         Enter the link to the Google spreadsheet you want to sync. To copy the link, click the 'Share' button in the top-right corner of the spreadsheet, then click 'Copy link'.
       examples:
         - https://docs.google.com/spreadsheets/d/1hLd9Qqti3UyLXZB2aFfUWDT7BG-arw2xy4HR3D-dwUb/edit
```

#### html2text {}

```diff
@@ -1,21 +1,32 @@
 documentationUrl: https://docs.airbyte.com/integrations/sources/google-sheets
 connectionSpecification: $schema: http://json-schema.org/draft-07/schema#
 title: Google Sheets Source Spec type: object required: - spreadsheet_id -
-credentials additionalProperties: true properties: spreadsheet_id: type: string
-title: Spreadsheet Link description: >- Enter the link to the Google
-spreadsheet you want to sync. To copy the link, click the 'Share' button in the
-top-right corner of the spreadsheet, then click 'Copy link'. examples: - https:
-//docs.google.com/spreadsheets/d/1hLd9Qqti3UyLXZB2aFfUWDT7BG-arw2xy4HR3D-dwUb/
-edit names_conversion: type: boolean title: Convert Column Names to SQL-
-Compliant Format description: Enables the conversion of column names to a
-standardized, SQL-compliant format. For example, 'My Name' -> 'my_name'. Enable
-this option if your destination is SQL-based. default: false credentials: type:
-object title: Authentication description: >- Credentials for connecting to the
-Google Sheets API oneOf: - title: Authenticate via Google (OAuth) type: object
+credentials additionalProperties: true properties: batch_size: type: integer
+title: Row Batch Size description: >- Default value is 200. An integer
+representing row batch size for each sent request to Google Sheets API. Row
+batch size means how many rows are processed from the google sheet, for example
+default value 200 would process rows 1-201, then 201-401 and so on. Based on
+_G_o_o_g_l_e_ _S_h_e_e_t_s_ _A_P_I_ _l_i_m_i_t_s_ _d_o_c_u_m_e_n_t_a_t_i_o_n, it is possible to send up to 300
+requests per minute, but each individual request has to be processed under 180
+seconds, otherwise the request returns a timeout error. In regards to this
+information, consider network speed and number of columns of the google sheet
+when deciding a batch_size value. Default value should cover most of the cases,
+but if a google sheet has over 100,000 records or more, consider increasing
+batch_size value. default: 200 spreadsheet_id: type: string title: Spreadsheet
+Link description: >- Enter the link to the Google spreadsheet you want to sync.
+To copy the link, click the 'Share' button in the top-right corner of the
+spreadsheet, then click 'Copy link'. examples: - https://docs.google.com/
+spreadsheets/d/1hLd9Qqti3UyLXZB2aFfUWDT7BG-arw2xy4HR3D-dwUb/edit
+names_conversion: type: boolean title: Convert Column Names to SQL-Compliant
+Format description: Enables the conversion of column names to a standardized,
+SQL-compliant format. For example, 'My Name' -> 'my_name'. Enable this option
+if your destination is SQL-based. default: false credentials: type: object
+title: Authentication description: >- Credentials for connecting to the Google
+Sheets API oneOf: - title: Authenticate via Google (OAuth) type: object
 required: - auth_type - client_id - client_secret - refresh_token properties:
 auth_type: type: string const: Client client_id: title: Client ID type: string
 description: "Enter your Google application's Client ID. See _G_o_o_g_l_e_'_s
 _d_o_c_u_m_e_n_t_a_t_i_o_n for more information." airbyte_secret: true client_secret: title:
 Client Secret type: string description: "Enter your Google application's Client
 Secret. See _G_o_o_g_l_e_'_s_ _d_o_c_u_m_e_n_t_a_t_i_o_n for more information." airbyte_secret: true
 refresh_token: title: Refresh Token type: string description: "Enter your
```

### Comparing `airbyte_source_google_sheets-0.5.0/source_google_sheets/utils.py` & `airbyte_source_google_sheets-0.5.1/source_google_sheets/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_google_sheets-0.5.0/PKG-INFO` & `airbyte_source_google_sheets-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-google-sheets
-Version: 0.5.0
+Version: 0.5.1
 Summary: Source implementation for Google Sheets.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

