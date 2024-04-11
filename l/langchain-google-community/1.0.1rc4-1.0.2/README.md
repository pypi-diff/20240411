# Comparing `tmp/langchain_google_community-1.0.1rc4.tar.gz` & `tmp/langchain_google_community-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_community-1.0.1rc4.tar", max compression
+gzip compressed data, was "langchain_google_community-1.0.2.tar", max compression
```

## Comparing `langchain_google_community-1.0.1rc4.tar` & `langchain_google_community-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1072 2024-03-27 11:42:32.291806 langchain_google_community-1.0.1rc4/LICENSE
--rw-r--r--   0        0        0      258 2024-03-27 11:42:32.291806 langchain_google_community-1.0.1rc4/README.md
--rw-r--r--   0        0        0     1767 2024-03-27 11:42:32.291806 langchain_google_community-1.0.1rc4/langchain_google_community/__init__.py
--rw-r--r--   0        0        0     1262 2024-03-27 11:42:32.291806 langchain_google_community-1.0.1rc4/langchain_google_community/_utils.py
--rw-r--r--   0        0        0     3712 2024-03-27 11:42:32.291806 langchain_google_community-1.0.1rc4/langchain_google_community/bigquery.py
--rw-r--r--   0        0        0    34578 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/bigquery_vector_search.py
--rw-r--r--   0        0        0    15569 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/docai.py
--rw-r--r--   0        0        0     4620 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/documentai_warehouse.py
--rw-r--r--   0        0        0    14491 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/drive.py
--rw-r--r--   0        0        0     2123 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gcs_directory.py
--rw-r--r--   0        0        0     3549 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gcs_file.py
--rw-r--r--   0        0        0        0 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/__init__.py
--rw-r--r--   0        0        0     1029 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/base.py
--rw-r--r--   0        0        0     2565 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/create_draft.py
--rw-r--r--   0        0        0     2204 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/get_message.py
--rw-r--r--   0        0        0     1561 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/get_thread.py
--rw-r--r--   0        0        0     4062 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/loader.py
--rw-r--r--   0        0        0     5113 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/search.py
--rw-r--r--   0        0        0     2940 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/send_message.py
--rw-r--r--   0        0        0     2070 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/toolkit.py
--rw-r--r--   0        0        0     4624 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/gmail/utils.py
--rw-r--r--   0        0        0     5099 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/google_speech_to_text.py
--rw-r--r--   0        0        0     5071 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/places_api.py
--rw-r--r--   0        0        0     6413 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/search.py
--rw-r--r--   0        0        0     3217 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/texttospeech.py
--rw-r--r--   0        0        0     4188 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/translate.py
--rw-r--r--   0        0        0    16742 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/langchain_google_community/vertex_ai_search.py
--rw-r--r--   0        0        0     2856 2024-03-27 11:42:32.295806 langchain_google_community-1.0.1rc4/pyproject.toml
--rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 langchain_google_community-1.0.1rc4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/LICENSE
+-rw-r--r--   0        0        0      258 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/README.md
+-rw-r--r--   0        0        0     1964 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/__init__.py
+-rw-r--r--   0        0        0     1262 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/_utils.py
+-rw-r--r--   0        0        0     3712 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/bigquery.py
+-rw-r--r--   0        0        0    34578 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/bigquery_vector_search.py
+-rw-r--r--   0        0        0    15569 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/docai.py
+-rw-r--r--   0        0        0     4620 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/documentai_warehouse.py
+-rw-r--r--   0        0        0    17200 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/drive.py
+-rw-r--r--   0        0        0     2123 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gcs_directory.py
+-rw-r--r--   0        0        0     3549 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gcs_file.py
+-rw-r--r--   0        0        0        0 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/__init__.py
+-rw-r--r--   0        0        0     1029 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/base.py
+-rw-r--r--   0        0        0     2565 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/create_draft.py
+-rw-r--r--   0        0        0     2204 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/get_message.py
+-rw-r--r--   0        0        0     1561 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/get_thread.py
+-rw-r--r--   0        0        0     4062 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/loader.py
+-rw-r--r--   0        0        0     5113 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/search.py
+-rw-r--r--   0        0        0     2940 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/send_message.py
+-rw-r--r--   0        0        0     2070 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/toolkit.py
+-rw-r--r--   0        0        0     4624 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/gmail/utils.py
+-rw-r--r--   0        0        0     5099 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/google_speech_to_text.py
+-rw-r--r--   0        0        0     5071 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/places_api.py
+-rw-r--r--   0        0        0     6413 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/search.py
+-rw-r--r--   0        0        0     3217 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/texttospeech.py
+-rw-r--r--   0        0        0     4188 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/translate.py
+-rw-r--r--   0        0        0    19216 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/vertex_ai_search.py
+-rw-r--r--   0        0        0     2975 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/langchain_google_community/vision.py
+-rw-r--r--   0        0        0     2854 2024-04-11 17:35:44.725732 langchain_google_community-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 langchain_google_community-1.0.2/PKG-INFO
```

### Comparing `langchain_google_community-1.0.1rc4/LICENSE` & `langchain_google_community-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/__init__.py` & `langchain_google_community-1.0.2/langchain_google_community/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,23 @@
     GoogleSearchRun,
 )
 from langchain_google_community.texttospeech import TextToSpeechTool
 from langchain_google_community.translate import GoogleTranslateTransformer
 from langchain_google_community.vertex_ai_search import (
     VertexAIMultiTurnSearchRetriever,
     VertexAISearchRetriever,
+    VertexAISearchSummaryTool,
 )
+from langchain_google_community.vision import CloudVisionLoader, CloudVisionParser
 
 __all__ = [
     "BigQueryLoader",
     "BigQueryVectorSearch",
+    "CloudVisionLoader",
+    "CloudVisionParser",
     "DocAIParser",
     "DocAIParsingResults",
     "DocumentAIWarehouseRetriever",
     "GCSDirectoryLoader",
     "GCSFileLoader",
     "GMailLoader",
     "GmailToolkit",
@@ -41,8 +45,9 @@
     "GoogleSearchResults",
     "GoogleSearchRun",
     "GoogleTranslateTransformer",
     "SpeechToTextLoader",
     "TextToSpeechTool",
     "VertexAIMultiTurnSearchRetriever",
     "VertexAISearchRetriever",
+    "VertexAISearchSummaryTool",
 ]
```

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/_utils.py` & `langchain_google_community-1.0.2/langchain_google_community/_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/bigquery.py` & `langchain_google_community-1.0.2/langchain_google_community/bigquery.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/bigquery_vector_search.py` & `langchain_google_community-1.0.2/langchain_google_community/bigquery_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/docai.py` & `langchain_google_community-1.0.2/langchain_google_community/docai.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/documentai_warehouse.py` & `langchain_google_community-1.0.2/langchain_google_community/documentai_warehouse.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/drive.py` & `langchain_google_community-1.0.2/langchain_google_community/drive.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,14 +41,60 @@
     """Whether to load trashed files. Only applies when folder_id is given."""
     # NOTE(MthwRobinson) - changing the file_loader_cls to type here currently
     # results in pydantic validation errors
     file_loader_cls: Any = None
     """The file loader class to use."""
     file_loader_kwargs: Dict["str", Any] = {}
     """The file loader kwargs to use."""
+    load_auth: bool = False
+    """Whether to load authorization identities."""
+
+    def _get_identity_metadata_from_id(self, id: str) -> List[str]:
+        """Fetch the list of people having access to ID file."""
+        try:
+            import googleapiclient.errors  # type: ignore[import]
+            from googleapiclient.discovery import build  # type: ignore[import]
+        except ImportError as exc:
+            raise ImportError(
+                "You must run "
+                "`pip install --upgrade "
+                "google-api-python-client` "
+                "to load authorization identities."
+            ) from exc
+
+        authorized_identities: list = []
+        creds = self._load_credentials()
+        service = build("drive", "v3", credentials=creds)  # Build the service
+        try:
+            permissions = service.permissions().list(fileId=id).execute()
+        except googleapiclient.errors.HttpError:
+            print(
+                f"insufficientFilePermissions: The user does not have sufficient \
+                permissions to retrieve permission for the file with fileId: {id}"
+            )
+            return authorized_identities
+        except Exception as exc:
+            print(
+                f"Error occurred while fetching the permissions for the file with \
+                fileId: {id}"
+            )
+            print(f"Error: {exc}")
+            return authorized_identities
+
+        for perm in permissions.get("permissions", {}):
+            email_id = (
+                service.permissions()
+                .get(fileId=id, permissionId=perm.get("id", ""), fields="emailAddress")
+                .execute()
+                .get("emailAddress")
+            )
+            if email_id:
+                authorized_identities.append(email_id)
+
+        return authorized_identities
 
     @root_validator
     def validate_inputs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         """Validate that either folder_id or document_ids is set, but not both."""
         if values.get("folder_id") and (
             values.get("document_ids") or values.get("file_ids")
         ):
@@ -109,15 +155,15 @@
             from google.oauth2 import service_account  # type: ignore[import]
             from google.oauth2.credentials import Credentials  # type: ignore[import]
             from google_auth_oauthlib.flow import (  # type: ignore[import]
                 InstalledAppFlow,
             )
         except ImportError:
             raise ImportError(
-                "You must run "
+                "Install prerequisites by running: "
                 "`pip install --upgrade "
                 "google-api-python-client google-auth-httplib2 "
                 "google-auth-oauthlib` "
                 "to use the Google Drive loader."
             )
 
         creds = None
@@ -153,14 +199,16 @@
 
         from googleapiclient.discovery import build  # type: ignore[import]
 
         creds = self._load_credentials()
         sheets_service = build("sheets", "v4", credentials=creds)
         spreadsheet = sheets_service.spreadsheets().get(spreadsheetId=id).execute()
         sheets = spreadsheet.get("sheets", [])
+        if self.load_auth:
+            authorized_identities = self._get_identity_metadata_from_id(id)
 
         documents = []
         for sheet in sheets:
             sheet_name = sheet["properties"]["title"]
             result = (
                 sheets_service.spreadsheets()
                 .values()
@@ -177,14 +225,16 @@
                     "source": (
                         f"https://docs.google.com/spreadsheets/d/{id}/"
                         f"edit?gid={sheet['properties']['sheetId']}"
                     ),
                     "title": f"{spreadsheet['properties']['title']} - {sheet_name}",
                     "row": i,
                 }
+                if self.load_auth:
+                    metadata["authorized_identities"] = authorized_identities
                 content = []
                 for j, v in enumerate(row):
                     title = header[j].strip() if len(header) > j else ""
                     content.append(f"{title}: {v.strip()}")
 
                 page_content = "\n".join(content)
                 documents.append(Document(page_content=page_content, metadata=metadata))
@@ -197,14 +247,16 @@
 
         from googleapiclient.discovery import build
         from googleapiclient.errors import HttpError  # type: ignore[import]
         from googleapiclient.http import MediaIoBaseDownload  # type: ignore[import]
 
         creds = self._load_credentials()
         service = build("drive", "v3", credentials=creds)
+        if self.load_auth:
+            authorized_identities = self._get_identity_metadata_from_id(id)
 
         file = (
             service.files()
             .get(fileId=id, supportsAllDrives=True, fields="modifiedTime,name")
             .execute()
         )
         request = service.files().export_media(fileId=id, mimeType="text/plain")
@@ -223,14 +275,16 @@
 
         text = fh.getvalue().decode("utf-8")
         metadata = {
             "source": f"https://docs.google.com/document/d/{id}/edit",
             "title": f"{file.get('name')}",
             "when": f"{file.get('modifiedTime')}",
         }
+        if self.load_auth:
+            metadata["authorized_identities"] = authorized_identities  # type: ignore
         return Document(page_content=text, metadata=metadata)
 
     def _load_documents_from_folder(
         self, folder_id: str, *, file_types: Optional[Sequence[str]] = None
     ) -> List[Document]:
         """Load documents from a folder."""
         from googleapiclient.discovery import build
@@ -300,14 +354,17 @@
 
         from googleapiclient.discovery import build
         from googleapiclient.http import MediaIoBaseDownload
 
         creds = self._load_credentials()
         service = build("drive", "v3", credentials=creds)
 
+        if self.load_auth:
+            authorized_identities = self._get_identity_metadata_from_id(id)
+
         file = service.files().get(fileId=id, supportsAllDrives=True).execute()
         request = service.files().get_media(fileId=id)
         fh = BytesIO()
         downloader = MediaIoBaseDownload(fh, request)
         done = False
         while done is False:
             status, done = downloader.next_chunk()
@@ -316,33 +373,40 @@
             fh.seek(0)
             loader = self.file_loader_cls(file=fh, **self.file_loader_kwargs)
             docs = loader.load()
             for doc in docs:
                 doc.metadata["source"] = f"https://drive.google.com/file/d/{id}/view"
                 if "title" not in doc.metadata:
                     doc.metadata["title"] = f"{file.get('name')}"
+                if self.load_auth:
+                    doc.metadata["authorized_identities"] = authorized_identities
             return docs
 
         else:
             from PyPDF2 import PdfReader  # type: ignore[import]
 
             content = fh.getvalue()
             pdf_reader = PdfReader(BytesIO(content))
 
-            return [
-                Document(
-                    page_content=page.extract_text(),
-                    metadata={
-                        "source": f"https://drive.google.com/file/d/{id}/view",
-                        "title": f"{file.get('name')}",
-                        "page": i,
-                    },
+            docs = []
+            for i, page in enumerate(pdf_reader.pages):
+                metadata = {
+                    "source": f"https://drive.google.com/file/d/{id}/view",
+                    "title": f"{file.get('name')}",
+                    "page": i,
+                }
+                if self.load_auth:
+                    metadata["authorized_identities"] = authorized_identities
+                docs.append(
+                    Document(
+                        page_content=page.extract_text(),
+                        metadata=metadata,
+                    )
                 )
-                for i, page in enumerate(pdf_reader.pages)
-            ]
+            return docs
 
     def _load_file_from_ids(self) -> List[Document]:
         """Load files from a list of IDs."""
         if not self.file_ids:
             raise ValueError("file_ids must be set")
         docs = []
         for file_id in self.file_ids:
```

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gcs_directory.py` & `langchain_google_community-1.0.2/langchain_google_community/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gcs_file.py` & `langchain_google_community-1.0.2/langchain_google_community/gcs_file.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/base.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/base.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/create_draft.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/get_message.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/get_thread.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/loader.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/loader.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/search.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/search.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/send_message.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/toolkit.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/gmail/utils.py` & `langchain_google_community-1.0.2/langchain_google_community/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/google_speech_to_text.py` & `langchain_google_community-1.0.2/langchain_google_community/google_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/places_api.py` & `langchain_google_community-1.0.2/langchain_google_community/places_api.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/search.py` & `langchain_google_community-1.0.2/langchain_google_community/search.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/texttospeech.py` & `langchain_google_community-1.0.2/langchain_google_community/texttospeech.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/translate.py` & `langchain_google_community-1.0.2/langchain_google_community/translate.py`

 * *Files identical despite different names*

### Comparing `langchain_google_community-1.0.1rc4/langchain_google_community/vertex_ai_search.py` & `langchain_google_community-1.0.2/langchain_google_community/vertex_ai_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 from google.api_core.client_options import ClientOptions
 from google.api_core.exceptions import InvalidArgument
 from google.protobuf.json_format import MessageToDict
 from langchain_core.callbacks import CallbackManagerForRetrieverRun
 from langchain_core.documents import Document
 from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
 from langchain_core.retrievers import BaseRetriever
+from langchain_core.tools import BaseTool
 from langchain_core.utils import get_from_dict_or_env
 
 from langchain_google_community._utils import get_client_info
 
 if TYPE_CHECKING:
-    from google.cloud.discoveryengine_v1beta import (  # type: ignore[import]
+    from google.cloud.discoveryengine_v1beta import (  # type: ignore[import, attr-defined]
         ConversationalSearchServiceClient,
         SearchRequest,
         SearchResult,
         SearchServiceClient,
     )
 
 
@@ -266,59 +267,72 @@
         self._serving_config = self._client.serving_config_path(
             project=self.project_id,
             location=self.location_id,
             data_store=self.data_store_id,
             serving_config=self.serving_config_id,
         )
 
-    def _create_search_request(self, query: str) -> SearchRequest:
-        """Prepares a SearchRequest object."""
-        from google.cloud.discoveryengine_v1beta import SearchRequest
-
-        query_expansion_spec = SearchRequest.QueryExpansionSpec(
-            condition=self.query_expansion_condition,
-        )
+    def _get_content_spec_kwargs(self) -> Optional[Dict[str, Any]]:
+        """Prepares a ContentSpec object."""
 
-        spell_correction_spec = SearchRequest.SpellCorrectionSpec(
-            mode=self.spell_correction_mode
-        )
+        from google.cloud.discoveryengine_v1beta import SearchRequest
 
         if self.engine_data_type == 0:
             if self.get_extractive_answers:
                 extractive_content_spec = (
                     SearchRequest.ContentSearchSpec.ExtractiveContentSpec(
                         max_extractive_answer_count=self.max_extractive_answer_count,
                     )
                 )
             else:
                 extractive_content_spec = (
                     SearchRequest.ContentSearchSpec.ExtractiveContentSpec(
                         max_extractive_segment_count=self.max_extractive_segment_count,
                     )
                 )
-            content_search_spec = SearchRequest.ContentSearchSpec(
-                extractive_content_spec=extractive_content_spec
-            )
+            content_search_spec = dict(extractive_content_spec=extractive_content_spec)
         elif self.engine_data_type == 1:
             content_search_spec = None
         elif self.engine_data_type == 2:
-            content_search_spec = SearchRequest.ContentSearchSpec(
+            content_search_spec = dict(
                 extractive_content_spec=SearchRequest.ContentSearchSpec.ExtractiveContentSpec(
                     max_extractive_answer_count=self.max_extractive_answer_count,
                 ),
                 snippet_spec=SearchRequest.ContentSearchSpec.SnippetSpec(
                     return_snippet=True
                 ),
             )
         else:
             raise NotImplementedError(
                 "Only data store type 0 (Unstructured), 1 (Structured),"
                 "or 2 (Website) are supported currently."
                 + f" Got {self.engine_data_type}"
             )
+        return content_search_spec
+
+    def _create_search_request(self, query: str) -> SearchRequest:
+        """Prepares a SearchRequest object."""
+        from google.cloud.discoveryengine_v1beta import SearchRequest
+
+        query_expansion_spec = SearchRequest.QueryExpansionSpec(
+            condition=self.query_expansion_condition,
+        )
+
+        spell_correction_spec = SearchRequest.SpellCorrectionSpec(
+            mode=self.spell_correction_mode
+        )
+
+        content_search_spec_kwargs = self._get_content_spec_kwargs()
+
+        if content_search_spec_kwargs is not None:
+            content_search_spec = SearchRequest.ContentSearchSpec(
+                **content_search_spec_kwargs
+            )
+        else:
+            content_search_spec = None
 
         return SearchRequest(
             query=query,
             filter=self.filter,
             serving_config=self._serving_config,
             page_size=self.max_documents,
             content_search_spec=content_search_spec,
@@ -436,7 +450,61 @@
             return self._convert_website_search_response(
                 response.search_results, "extractive_answers"
             )
 
         return self._convert_unstructured_search_response(
             response.search_results, "extractive_answers"
         )
+
+
+class VertexAISearchSummaryTool(BaseTool, VertexAISearchRetriever):
+    """Class that exposes a tool to interface with an App in Vertex Search and
+    Conversation and get the summary of the documents retrieved.
+    """
+
+    summary_prompt: Optional[str] = None
+    """Prompt for the summarization agent"""
+
+    summary_result_count: int = 3
+    """ Number of documents to include in the summary"""
+
+    summary_include_citations: bool = True
+    """ Whether to include citations in the summary """
+
+    summary_spec_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    """ Additional kwargs for `SearchRequest.ContentSearchSpec.SummarySpec`"""
+
+    class Config(VertexAISearchRetriever.Config):
+        """Redefinition to specify that inherits config from `VertexAISearchRetriever`
+        not BaseTool
+        """
+
+    def _get_content_spec_kwargs(self) -> Optional[Dict[str, Any]]:
+        """Adds additional summary_spec parameters to the configuration of the search.
+        Returns:
+            kwargs for the specification of the content.
+        """
+        from google.cloud.discoveryengine_v1beta import SearchRequest
+
+        kwargs = super()._get_content_spec_kwargs() or {}
+
+        kwargs["summary_spec"] = SearchRequest.ContentSearchSpec.SummarySpec(
+            summary_result_count=self.summary_result_count,
+            include_citations=self.summary_include_citations,
+            model_prompt_spec=SearchRequest.ContentSearchSpec.SummarySpec.ModelPromptSpec(
+                preamble=self.summary_prompt
+            ),
+            **self.summary_spec_kwargs,
+        )
+
+        return kwargs
+
+    def _run(self, user_query: str) -> str:
+        """Runs the tool.
+        Args:
+            search_query: The query to run by the agent.
+        Returns:
+            The response from the agent.
+        """
+        request = self._create_search_request(user_query)
+        response = self._client.search(request)
+        return response.summary.summary_text
```

### Comparing `langchain_google_community-1.0.1rc4/pyproject.toml` & `langchain_google_community-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-google-community"
-version = "1.0.1rc4"
+version = "1.0.2"
 description = "An integration package connecting miscellaneous Google's products and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/community"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = ">=0.1.33,<0.2"
-langchain-community = "^0.0.28"
+langchain-community = ">=0.0.28"
 google-api-core = "^2.17.1"
 google-api-python-client = "^2.122.0"
 grpcio = "^1.62.0"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_google_community-1.0.1rc4/PKG-INFO` & `langchain_google_community-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: langchain-google-community
-Version: 1.0.1rc4
+Version: 1.0.2
 Summary: An integration package connecting miscellaneous Google's products and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: google-api-core (>=2.17.1,<3.0.0)
 Requires-Dist: google-api-python-client (>=2.122.0,<3.0.0)
 Requires-Dist: grpcio (>=1.62.0,<2.0.0)
-Requires-Dist: langchain-community (>=0.0.28,<0.0.29)
+Requires-Dist: langchain-community (>=0.0.28)
 Requires-Dist: langchain-core (>=0.1.33,<0.2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/community
 Description-Content-Type: text/markdown
 
 # langchain-google-community
```

