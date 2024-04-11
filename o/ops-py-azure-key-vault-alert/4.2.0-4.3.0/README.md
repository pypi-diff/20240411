# Comparing `tmp/ops-py-azure-key-vault-alert-4.2.0.tar.gz` & `tmp/ops-py-azure-key-vault-alert-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-alert-4.2.0.tar", last modified: Tue Mar 12 12:50:52 2024, max compression
+gzip compressed data, was "ops-py-azure-key-vault-alert-4.3.0.tar", last modified: Thu Apr 11 12:58:32 2024, max compression
```

## Comparing `ops-py-azure-key-vault-alert-4.2.0.tar` & `ops-py-azure-key-vault-alert-4.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:50:52.559082 ops-py-azure-key-vault-alert-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-12 12:50:50.000000 ops-py-azure-key-vault-alert-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-12 12:50:52.559082 ops-py-azure-key-vault-alert-4.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:50:52.559082 ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-03-12 12:50:45.000000 ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5766 2024-03-12 12:50:45.000000 ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7483 2024-03-12 12:50:45.000000 ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/slack_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-03-12 12:50:45.000000 ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:50:52.559082 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-12 12:50:52.000000 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-12 12:50:52.000000 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:50:52.000000 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-12 12:50:52.000000 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 12:50:52.000000 ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 12:50:50.000000 ops-py-azure-key-vault-alert-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-12 12:50:50.000000 ops-py-azure-key-vault-alert-4.2.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-12 12:50:45.000000 ops-py-azure-key-vault-alert-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 12:50:52.559082 ops-py-azure-key-vault-alert-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 12:50:50.000000 ops-py-azure-key-vault-alert-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.057566 ops-py-azure-key-vault-alert-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6387 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7486 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/slack_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:58:32.057566 ops-py-azure-key-vault-alert-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/setup.py
```

### Comparing `ops-py-azure-key-vault-alert-4.2.0/LICENSE` & `ops-py-azure-key-vault-alert-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.2.0/PKG-INFO` & `ops-py-azure-key-vault-alert-4.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.2.0
+Version: 4.3.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,27 +22,30 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: build==1.1.1
+Requires-Dist: backports.tarfile==1.0.0
+Requires-Dist: build==1.2.1
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: docutils==0.20.1
+Requires-Dist: docutils==0.21.1
 Requires-Dist: idna==3.6
-Requires-Dist: importlib_metadata==7.0.2
-Requires-Dist: jaraco.classes==3.3.1
-Requires-Dist: keyring==24.3.1
+Requires-Dist: importlib_metadata==7.1.0
+Requires-Dist: jaraco.classes==3.4.0
+Requires-Dist: jaraco.context==5.3.0
+Requires-Dist: jaraco.functools==4.0.0
+Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
-Requires-Dist: nh3==0.2.15
-Requires-Dist: ops-py-azure-key-vault-report==3.3.0
+Requires-Dist: nh3==0.2.17
+Requires-Dist: ops-py-azure-key-vault-report==4.0.0
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
@@ -51,15 +54,15 @@
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.1.0
 Requires-Dist: twine==5.0.0
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: wheel==0.42.0
-Requires-Dist: zipp==3.17.0
+Requires-Dist: zipp==3.18.1
 
 # azure-key-vault-alert
 
 ## Description
 Generates a **Key Vault** report table and summary table for one more **Key Vaults** using 
 [ops-py-azure-key-vault-report](https://pypi.org/project/ops-py-azure-key-vault-report)
```

### Comparing `ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/azure_key_vault_alert.py` & `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,21 +114,35 @@
     # If success and 'WEBHOOK_NOTIFY' is provided
     # an additional notify will be posted to the 'WEBHOOK_NOTIFY' webhook
     if success and WEBHOOK_NOTIFY:
         logging.info(f"Trigger additional alert about new report message(s)...")
         alert = message_handler.MessageHandler(WEBHOOK_NOTIFY)
         alert.post_payload()
 
+    # Get the full report which will be logged for future references.
+    # Azure resource information are added.
+    report_full = kv_report.get_report_full()
+    if isinstance(report_full, dict):
+        report_full["client_id"] = AZURE_CLIENT_ID
+        report_full["subscription_id"] = AZURE_SUBSCRIPTION_ID
+        report_full["tenant_id"] = AZURE_TENANT_ID
+
+        # Temporarily print to stdout, but will be pushed to db
+        print(report_full)
 
 ########################################################################################################################
 
 
 if __name__ == '__main__':
     # The actual report will be posted to the webhook exported in
     # the following environment variable
     WEBHOOK_REPORT = os.getenv("WEBHOOK_REPORT")
 
     # When all the reports have been posted, an additional POST is performed
     # to the webhook exported in following environment variable:
     WEBHOOK_NOTIFY = os.getenv("WEBHOOK_NOTIFY")
 
+    AZURE_CLIENT_ID = os.getenv("AZURE_CLIENT_ID")
+    AZURE_SUBSCRIPTION_ID = os.getenv("AZURE_SUBSCRIPTION_ID")
+    AZURE_TENANT_ID = os.getenv("AZURE_TENANT_ID")
+
     main()
```

### Comparing `ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/slack_alert.py` & `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/slack_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Returns
     -------
     True
         If response from the POST has return code 200
     """
 
     # Get full report, including the top summary
-    report = kv.get_markdown_report()
+    report = kv.get_report_summary_markdown()
 
     # Return if no report
     if not isinstance(report, str):
         logging.warning("No report")
         return
 
     # If stdout_only the report is printed to standard output only and then return
@@ -137,23 +137,23 @@
     # end of each message. If Slack Workflow, the formatting is handled by the Slack Workflow itself.
     # For Slack App 'payloads' are created. For Slack Workflow 'txt' items are created.
     cb = ""
     if slack_app:
         cb = "```"
 
     # The summary payload is created first and added to the list of results (to be posted)
-    summary = kv.get_markdown_summary()
+    summary = kv.get_summary_markdown()
     if slack_app:
         payload = {"text": f"*{title} - summary*\n{cb}{summary}{cb}"}
         results.append(payload)
     else:
         results.append((f"{title} - summary", summary))
 
     # Then the report is split into chucks
-    report = kv.get_markdown_report_only()
+    report = kv.get_report_markdown()
     report_lines = report.splitlines()
 
     # The two first lines of the report is the header, which will be used in every part
     header = f"{cb}{report_lines.pop(0)}\n{report_lines.pop(0)}\n"
 
     # The first part of the first report payload / txt is initialized
     part = 1
```

### Comparing `ops-py-azure-key-vault-alert-4.2.0/azure_key_vault_alert/teams_alert.py` & `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/teams_alert.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.2.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.2.0
+Version: 4.3.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,27 +22,30 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: build==1.1.1
+Requires-Dist: backports.tarfile==1.0.0
+Requires-Dist: build==1.2.1
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
-Requires-Dist: docutils==0.20.1
+Requires-Dist: docutils==0.21.1
 Requires-Dist: idna==3.6
-Requires-Dist: importlib_metadata==7.0.2
-Requires-Dist: jaraco.classes==3.3.1
-Requires-Dist: keyring==24.3.1
+Requires-Dist: importlib_metadata==7.1.0
+Requires-Dist: jaraco.classes==3.4.0
+Requires-Dist: jaraco.context==5.3.0
+Requires-Dist: jaraco.functools==4.0.0
+Requires-Dist: keyring==25.1.0
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: more-itertools==10.2.0
-Requires-Dist: nh3==0.2.15
-Requires-Dist: ops-py-azure-key-vault-report==3.3.0
+Requires-Dist: nh3==0.2.17
+Requires-Dist: ops-py-azure-key-vault-report==4.0.0
 Requires-Dist: ops-py-generate-pyproject==2.2.3
 Requires-Dist: ops-py-message-handler==1.0.3
 Requires-Dist: packaging==24.0
 Requires-Dist: pip==24.0
 Requires-Dist: pkginfo==1.10.0
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: pyproject_hooks==1.0.0
@@ -51,15 +54,15 @@
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: setuptools==69.1.0
 Requires-Dist: twine==5.0.0
 Requires-Dist: urllib3==2.2.0
 Requires-Dist: wheel==0.42.0
-Requires-Dist: zipp==3.17.0
+Requires-Dist: zipp==3.18.1
 
 # azure-key-vault-alert
 
 ## Description
 Generates a **Key Vault** report table and summary table for one more **Key Vaults** using 
 [ops-py-azure-key-vault-report](https://pypi.org/project/ops-py-azure-key-vault-report)
```

### Comparing `ops-py-azure-key-vault-alert-4.2.0/readme.md` & `ops-py-azure-key-vault-alert-4.3.0/readme.md`

 * *Files identical despite different names*

