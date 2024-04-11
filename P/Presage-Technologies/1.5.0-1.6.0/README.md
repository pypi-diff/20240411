# Comparing `tmp/Presage_Technologies-1.5.0-py3-none-any.whl.zip` & `tmp/Presage_Technologies-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9257 bytes, number of entries: 7
--rw-r--r--  2.0 unx       35 b- defN 24-Feb-14 15:16 presage_technologies/__init__.py
--rw-r--r--  2.0 unx     7577 b- defN 24-Feb-14 15:16 presage_technologies/physiology.py
--rw-rw-rw-  2.0 unx     7652 b- defN 24-Feb-14 15:19 Presage_Technologies-1.5.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     7253 b- defN 24-Feb-14 15:19 Presage_Technologies-1.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-14 15:19 Presage_Technologies-1.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 24-Feb-14 15:19 Presage_Technologies-1.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      633 b- defN 24-Feb-14 15:19 Presage_Technologies-1.5.0.dist-info/RECORD
-7 files, 23263 bytes uncompressed, 8115 bytes compressed:  65.1%
+Zip file size: 9671 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       35 b- defN 24-Apr-11 12:08 presage_technologies/__init__.py
+-rw-r--r--  2.0 unx    10088 b- defN 24-Apr-11 12:08 presage_technologies/physiology.py
+-rw-rw-rw-  2.0 unx     7652 b- defN 24-Apr-11 12:10 Presage_Technologies-1.6.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     7873 b- defN 24-Apr-11 12:10 Presage_Technologies-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 12:10 Presage_Technologies-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 24-Apr-11 12:10 Presage_Technologies-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      634 b- defN 24-Apr-11 12:10 Presage_Technologies-1.6.0.dist-info/RECORD
+7 files, 26395 bytes uncompressed, 8529 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: presage_technologies/__init__.py
 Comment: 
 
 Filename: presage_technologies/physiology.py
 Comment: 
 
-Filename: Presage_Technologies-1.5.0.dist-info/LICENSE.txt
+Filename: Presage_Technologies-1.6.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: Presage_Technologies-1.5.0.dist-info/METADATA
+Filename: Presage_Technologies-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: Presage_Technologies-1.5.0.dist-info/WHEEL
+Filename: Presage_Technologies-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: Presage_Technologies-1.5.0.dist-info/top_level.txt
+Filename: Presage_Technologies-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Presage_Technologies-1.5.0.dist-info/RECORD
+Filename: Presage_Technologies-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## presage_technologies/physiology.py

```diff
@@ -66,14 +66,85 @@
                     "Unauthorized error! Please make sure your API key is correct."
                 )
                 return
             else:
                 time.sleep(1)
         return None
 
+    def process_loopv2(self, trace, metrics, compress):
+        parts = []
+        vid_id = None
+        upload_id = None
+        urls = []
+        max_size = 5 * 1024 * 1024
+        url = self.base_api_url + "/v2/upload-url"
+        headers = {"x-api-key": self.api_key}
+        max_size = 5 * 1024 * 1024
+
+        preprocessed_data=trace
+        preprocessed_data = json.dumps(preprocessed_data).encode("utf-8")
+        if compress:
+            preprocessed_data = gzip.compress(preprocessed_data)
+        response = requests.post(
+            url,
+            headers=headers,
+            json={
+                "file_size": sys.getsizeof(preprocessed_data),
+                "metrics": metrics,
+            },
+        )
+        if response.status_code == 401:
+            logging.warning(
+                "Unauthorized error! Please make sure your API key is correct."
+            )
+            return
+        vid_id = response.json()["id"]
+        urls = response.json()["urls"]
+        upload_id = response.json()["upload_id"]
+
+        tracker = 0
+        max_len = len(preprocessed_data)
+        for num, url in enumerate(urls):
+            part = num + 1
+            if (max_len - tracker) < max_size:
+                file_data = preprocessed_data[tracker:max_len]
+            else:
+                file_data = preprocessed_data[tracker:max_size]
+            res = requests.put(url, data=file_data)
+            tracker += max_size
+            if res.status_code != 200:
+                return
+            etag = res.headers["ETag"]
+            parts.append({"ETag": etag, "PartNumber": part})
+        return parts, upload_id, vid_id
+
+    def queue_processing(self, trace=None, metrics=[], preprocess=True, compress=True):
+        """Using the Presage Physiology API, get all metrics
+        of a subject within a video.
+
+        Returns
+        -------
+        str
+            Id for the video uploaded that can be used to later retrieveresults with the retrieve_result function.
+        """
+
+        headers = {"x-api-key": self.api_key}
+        if trace is None:
+            raise Exception("You must pass a trace json")
+        parts, upload_id, vid_id = self.process_loopv2(trace, metrics, compress)
+
+        url = self.base_api_url + "/v2/complete"
+        requests.post(
+            url,
+            headers=headers,
+            json={"id": vid_id, "upload_id": upload_id, "parts": parts},
+        )
+        logging.info("Trace uploaded successfully and is now processing.")
+        return vid_id
+
     def process_loop(self, video_path, preprocess, compress, type, trace=None):
         parts = []
         vid_id = None
         upload_id = None
         urls = []
         max_size = 5 * 1024 * 1024
         url = self.base_api_url + "/v1/upload-url"
```

## Comparing `Presage_Technologies-1.5.0.dist-info/LICENSE.txt` & `Presage_Technologies-1.6.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `Presage_Technologies-1.5.0.dist-info/METADATA` & `Presage_Technologies-1.6.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: Presage-Technologies
-Version: 1.5.0
+Version: 1.6.0
 Summary: A Python client to interface with Presage Technologies' API services.
 Home-page: https://physiology.presagetech.com/
 Author: Presage Technologies
 Author-email: support@presagetech.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Presage-Security/presage_technologies/issues
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
-Requires-Dist: presage-physiology-preprocessing ==1.2.1
+Requires-Dist: presage-physiology-preprocessing ==1.2.6
+Requires-Dist: mediapipe ==0.9.1.0
+Requires-Dist: numpy ==1.26.3
 
 # presage_technologies
 
 **The information contained in this Python client, API, or data responses as expected from normal usage of the data should not be used to diagnose, treat, or prevent any disease or illness whether directly or indirectly. This is for informational and research purposes only.**
 
 A Python client for Presage Technologies' APIs. [Presage Technologies](https://presagetechnologies.com)
 
@@ -59,14 +61,24 @@
 After installation, import the client class into your project and initialize with the API key:
 
 ```python
 from presage_technologies import Physiology
 physio = Physiology("api_key_here")
 ```
 
+Use `.queue_processing()` to upload a trace for processing and return an id for the upload to allow for async processing. .
+
+```python
+id = physio.queue_processing(trace="<dictionary of trace data>", metrics=['hr', 'rr', 'hr_trace', 'rr_trace', 'hr_spec', 'rr_spec', 'hrv', 'phasic', 'rrl', 'apnea', 'ie', 'amplitude', 'baseline'])
+```
+
+metrics is an optional argument that expects a list, each of the above list items is optional. If the list is not supplied all metrics will be calculated.
+
+Use `.retrieve_result()` with your id to return the results.
+
 Use `.queue_processing_hr_rr()` to upload your video for processing and return an id for the upload to allow for async processing. You are able to upload multiple videos as you would like as long as it is within your plan limits.
 
 ```python
 video_id = physio.queue_processing_hr_rr("/path/to/video/file")
 ```
 
 We currently recommend waiting half the length of your video to start checking whether it is not but this is not a hard limit. When you are ready to start checking for the result you can use `.retrieve_result()` with your video_id to return the results.
```

