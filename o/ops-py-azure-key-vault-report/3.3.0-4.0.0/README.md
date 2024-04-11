# Comparing `tmp/ops-py-azure-key-vault-report-3.3.0.tar.gz` & `tmp/ops-py-azure-key-vault-report-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-report-3.3.0.tar", last modified: Tue Mar 12 12:46:26 2024, max compression
+gzip compressed data, was "ops-py-azure-key-vault-report-4.0.0.tar", last modified: Thu Apr 11 12:26:14 2024, max compression
```

## Comparing `ops-py-azure-key-vault-report-3.3.0.tar` & `ops-py-azure-key-vault-report-4.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:26.581772 ops-py-azure-key-vault-report-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 12:46:24.000000 ops-py-azure-key-vault-report-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-03-12 12:46:26.581772 ops-py-azure-key-vault-report-3.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:26.577772 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16212 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      937 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-03-12 12:46:21.000000 ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/set_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:26.577772 ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-03-12 12:46:26.000000 ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-12 12:46:26.000000 ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:46:26.000000 ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-12 12:46:26.000000 ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-12 12:46:24.000000 ops-py-azure-key-vault-report-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-03-12 12:46:24.000000 ops-py-azure-key-vault-report-3.3.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 12:46:26.581772 ops-py-azure-key-vault-report-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 12:46:24.000000 ops-py-azure-key-vault-report-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17664 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1346 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1219 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      949 2024-04-11 12:26:07.000000 ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/set_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-11 12:26:14.000000 ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:26:14.679647 ops-py-azure-key-vault-report-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 12:26:12.000000 ops-py-azure-key-vault-report-4.0.0/setup.py
```

### Comparing `ops-py-azure-key-vault-report-3.3.0/LICENSE` & `ops-py-azure-key-vault-report-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/PKG-INFO` & `ops-py-azure-key-vault-report-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 3.3.0
+Version: 4.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/az_cmd.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/azure_key_vault_report.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 
 import logging
+import datetime
 from .html_table import HTMLTable
 from .ms_teams_json import MSTeamsPayload
 from .set_timestamp import set_timestamp, now
 from .markdown import Markdown
 from .config import *
 
+
 ########################################################################################################################
 
 
 class AzureKeyVaultReport(object):
     """generates a report from the results of 'az keyvault' commands
 
     The values of 'updated', 'created' and 'expires' are converted to date object
@@ -85,19 +87,26 @@
         results : list
             The list of results from the 'az keyvault' commands, enriched with 'vault_name' and 'record_type'
         """
 
         self.results = results
         self.items = []
         self.vaults = []        # The unique list of vaults processed
-        self.report = ""
-        self.summary = ""
+        self.html_table = None  # HTML table object. Used for MS Teams
+        self.report_md = ""
+        self.report = []
+        self.summary = {}
+        self.summary_md = ""
         self.summary_values = config.get("summary")
         self.report_values = config.get("report")
-        self.html_table = None  # HTML table object. Used for MS Teams
+        self.report_full = {
+            "created_at": datetime.datetime.utcnow().isoformat(),
+            "summary": {"rows": []},
+            "report": {"rows": []}
+        }
 
     def sort_items(self, expired_days=7, will_expire_days=14):
         """Sort the list of dict items by days to expiration
 
         If no parameters provided, this method will return a sorted list of all the records.
         The list will be sorted from top and down, by the oldest 'Expiration' date and then followed
         by the oldest 'Last Updated' date and then returns the sorted list.
@@ -202,30 +211,33 @@
                             if "expires" in k and not v:
                                 self.summary_values["missing"]["value"] += 1
 
                 self.items.append(item)
 
     def add_summary(self):
         """adds the summary as Markdown"""
+        self.summary = {}
         self.summary_values["vaults"]["value"] = len(self.vaults)
         self.summary_values["records"]["value"] = len(self.items)
 
         rows = []
         for k, v in self.summary_values.items():
             if "heading" in k:
                 rows.append(v)
             elif isinstance(v, dict):
                 value = v.get("value")
                 if value:
                     text = v.get("text")
                     rows.append([text, value])
+                    self.summary[text] = value
 
         md = Markdown(rows)
         md.set_widths()
-        self.summary = md.get_output(1)
+        self.summary_md = md.get_output(1)
+        self.report_full["summary"]["rows"].append(self.summary)
 
     def add_report(self, expire_threshold=None, ignore_no_expiration=True, include_all=False, teams_json=False):
         """creates a plain text report and initiates ms team report generation if specified.
         returns the plain text report.
 
         Parameters
         ----------
@@ -240,19 +252,20 @@
             If set to True then a report in json format containing a html table will also be generated.
         """
         if not isinstance(self.results, list):
             return
 
         # If argument 'teams_json' is True, then a html table is initialized. To be used with the MS Teams payload
         if teams_json:
-            self.html_table = HTMLTable(self.report_values["heading"])
+            self.html_table = HTMLTable(self.report_values.get("heading"))
             self.html_table.init_html_table()
 
         # Ensure only heading and no data rows
         rows = [self.report_values["heading"]]
+        rows_all = [self.report_values["heading"]]
 
         # Sort the items from top and down
         # First sort by the oldest 'Expiration' date
         # Then sort by the oldest 'Last Updated' date
         items = self.sort_items()
 
         logging.info(f"expire_threshold: {expire_threshold} {type(expire_threshold)} - "
@@ -261,53 +274,26 @@
 
         for item in items:
             # Get name of the record. If no name, we skip to next item in the list
             record_name = item.get("record_name")
             if not record_name:
                 continue
 
-            # Only list disabled entries if set to include_all
-            enabled = item.get("enabled")
-            if not include_all and not enabled:
-                continue
-
             # Get the record type
             record_type = item.get("record_type", "")
 
             # Get the Vault Name
             vault_name = item.get("vault_name", "")
 
-            # Get the expires and update values
+            # Get the expires, update and enabled values
             expires = item.get("expires", "")
             expires_age = item.get("expires_age")
             updated = item.get("updated")
             updated_age = item.get("updated_age")
-
-            # Skip records with no Expiration Date set, only if 'ignore_no_expiration' and not 'include_all'
-            if not expires:
-                if ignore_no_expiration and not include_all:
-                    continue
-
-            # Handle those with Expiration Date
-            if isinstance(expires_age, int):
-
-                # Handle those which has not expired yet
-                if expires_age < 0:
-                    logging.info(f"'{record_name}' has not expired yet. "
-                                 f"It will expire in {abs(expires_age)} days ({expires}).")
-
-                    # Handle those within valid 'expire_threshold'
-                    if isinstance(expire_threshold, int) and expire_threshold < abs(expires_age):
-                        logging.info(f"'{record_name}' Expiration Date is within the valid specified threshold of "
-                                     f"{expire_threshold} days. This record will start to be "
-                                     f"reported in {abs(expires_age) - expire_threshold} days.")
-
-                        # Only skipped if 'include_all' is not specified.
-                        if not include_all:
-                            continue
+            enabled = item.get("enabled")
 
             # Add to row: the values of: 'record_name', 'record_type', 'vault_name' and 'updated'
             row = [record_name, record_type, vault_name, updated]
 
             # Add to row: the value of: 'expires' (if any)
             if expires:
                 row.append(expires)
@@ -334,44 +320,105 @@
 
             # A little cosmetic touch to avoid plural where it should not be used
             comment = comment.replace(" 1 days", " 1 day")
 
             # Add to row: the value of: 'comment'
             row.append(comment)
 
-            # Then finally add the complete 'row' to the 'rows'
+            # Add the row to the rows_all (The ones that will be stored in db, but not necessarily will be alerted on)
+            rows_all.append(row)
+
+            # Only include disabled entries if set to include_all
+            if not include_all and not enabled:
+                continue
+
+            # Skip records with no Expiration Date set, only if 'ignore_no_expiration' and not 'include_all'
+            if not expires:
+                if ignore_no_expiration and not include_all:
+                    continue
+
+            # Handle those with Expiration Date
+            if isinstance(expires_age, int):
+
+                # Handle those which has not expired yet
+                if expires_age < 0:
+                    logging.info(f"'{record_name}' has not expired yet. "
+                                 f"It will expire in {abs(expires_age)} days ({expires}).")
+
+                    # Handle those within valid 'expire_threshold'
+                    if isinstance(expire_threshold, int) and expire_threshold < abs(expires_age):
+                        logging.info(f"'{record_name}' Expiration Date is within the valid specified threshold of "
+                                     f"{expire_threshold} days. This record will start to be "
+                                     f"reported in {abs(expires_age) - expire_threshold} days.")
+
+                        # Only skipped if 'include_all' is not specified.
+                        if not include_all:
+                            continue
+
+            # Then finally add the row to the rows (The ones that will be reported)
             rows.append(row)
 
             # If a html_table is created, then also add the row to the html table. Used in MS Teams payload
             if self.html_table:
                 self.html_table.add_html_row(*row)
 
+        self.report_full["report"]["rows"].append(self.create_kv_rows(rows_all))
+
+        if include_all:
+            rows = rows_all
+
+        if not rows:
+            logging.error("No report generated.")
+            return
+
         # Create markdown of the report
         md = Markdown(rows)
         md.set_widths()
         if len(rows) > 1:
-            self.report = md.get_output()
+            self.report_md = md.get_output()
+
+            # Create json of the report
+            self.report = self.create_kv_rows(rows)
 
         logging.info("report generated.")
 
-    def get_markdown_report(self):
-        """return the plain text report"""
-        if self.report:
-            return f"{self.summary}\n\n{self.report}"
+    def create_kv_rows(self, rows):
+        kv_rows = []
+        for i, r in enumerate(rows):
+            if i > 0:
+                j = {}
+                for n, v in enumerate(self.report_values.get("heading")):
+                    j[v] = r[n]
+                kv_rows.append(j)
+        return kv_rows
 
-        return self.summary
+    def get_report_full(self):
+        return self.report_full
 
-    def get_markdown_report_only(self):
-        """return the Markdown report"""
+    def get_report(self):
         return self.report
 
-    def get_markdown_summary(self):
-        """return the Markdown summary"""
+    def get_summary(self):
         return self.summary
 
+    def get_summary_markdown(self):
+        """return the Markdown summary"""
+        return self.summary_md
+
+    def get_report_markdown(self):
+        """return the Markdown report"""
+        return self.report_md
+
+    def get_report_summary_markdown(self):
+        """return the plain text report"""
+        if self.report_md:
+            return f"{self.summary_md}\n\n{self.report_md}"
+
+        return self.summary_md
+
     def get_teams_payload(self, title, text=""):
         """build and return the MS Teams payload"""
         if not isinstance(self.results, list):
             return
 
         if len(self.items) == 0:
             return
```

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/config.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python
 
 config = {
     "summary":
         {"widths": [],
          "heading": ["Description", "Count"],
-         "vaults": {"text": "Total number of vaults:", "value": 0},
-         "records": {"text": "Total number of records:", "value": 0},
-         "expired": {"text": "Records already expired:", "value": 0},
-         "missing": {"text": "Records missing Expiration Date:", "value": 0},
-         "this_year": {"text": "Records updated in the last year:", "value": 0},
-         "one_year": {"text": "Records NOT updated in the last year:", "value": 0},
-         "two_years": {"text": "Records NOT updated for the last 2 years:", "value": 0},
-         "three_years": {"text": "Records NOT updated for the last 3 years:", "value": 0}
+         "vaults": {"text": "Total number of vaults", "value": 0},
+         "records": {"text": "Total number of records", "value": 0},
+         "expired": {"text": "Records already expired", "value": 0},
+         "missing": {"text": "Records missing Expiration Date", "value": 0},
+         "this_year": {"text": "Records updated in the last year", "value": 0},
+         "one_year": {"text": "Records NOT updated in the last year", "value": 0},
+         "two_years": {"text": "Records NOT updated for the last 2 years", "value": 0},
+         "three_years": {"text": "Records NOT updated for the last 3 years", "value": 0}
          },
     "report":
         {"widths": [],
          "heading": ["Record Name", "Record Type", "Vault Name", "Last Updated", "Expiration",
                      "Comment"]
          }
 }
```

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/html_table.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/markdown.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/markdown.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/ms_teams_json.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/azure_key_vault_report/set_timestamp.py` & `ops-py-azure-key-vault-report-4.0.0/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 3.3.0
+Version: 4.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-report-3.3.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops-py-azure-key-vault-report-4.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-report-3.3.0/readme.md` & `ops-py-azure-key-vault-report-4.0.0/readme.md`

 * *Files identical despite different names*

