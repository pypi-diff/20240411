# Comparing `tmp/smaht_submitr-0.8.0.1b8.tar.gz` & `tmp/smaht_submitr-0.8.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.0.1b8.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.0.1b9.tar", max compression
```

## Comparing `smaht_submitr-0.8.0.1b8.tar` & `smaht_submitr-0.8.0.1b9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1098 2024-04-08 02:25:43.553559 smaht_submitr-0.8.0.1b8/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-04-08 02:25:43.553559 smaht_submitr-0.8.0.1b8/README.rst
--rw-r--r--   0        0        0     3425 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/base.py
--rw-r--r--   0        0        0      294 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/exceptions.py
--rw-r--r--   0        0        0     2628 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/output.py
--rw-r--r--   0        0        0    13423 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/progress_bar.py
--rw-r--r--   0        0        0    10819 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4785 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9846 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     1828 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5709 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    19891 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-04-08 02:25:43.589559 smaht_submitr-0.8.0.1b8/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   152631 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/submission.py
--rw-r--r--   0        0        0        0 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0     1620 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    11606 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0     2478 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_show_upload_info.py
--rw-r--r--   0        0        0   157490 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     3661 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_upload_item_data.py
--rw-r--r--   0        0        0     4353 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0    12167 2024-04-08 02:25:43.593559 smaht_submitr-0.8.0.1b8/submitr/utils.py
--rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.8.0.1b8/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-08 02:27:59.919595 smaht_submitr-0.8.0.1b9/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-04-08 02:27:59.919595 smaht_submitr-0.8.0.1b9/README.rst
+-rw-r--r--   0        0        0     3425 2024-04-08 02:27:59.955594 smaht_submitr-0.8.0.1b9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 02:27:59.955594 smaht_submitr-0.8.0.1b9/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-04-08 02:27:59.955594 smaht_submitr-0.8.0.1b9/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-04-08 02:27:59.955594 smaht_submitr-0.8.0.1b9/submitr/exceptions.py
+-rw-r--r--   0        0        0     2628 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/output.py
+-rw-r--r--   0        0        0    13423 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/progress_bar.py
+-rw-r--r--   0        0        0    10819 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4785 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9846 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     1828 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5709 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    19891 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   152631 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/submission.py
+-rw-r--r--   0        0        0        0 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0      272 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1620 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    11606 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0     2478 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_show_upload_info.py
+-rw-r--r--   0        0        0   157490 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     3661 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_upload_item_data.py
+-rw-r--r--   0        0        0     4353 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0    12167 2024-04-08 02:27:59.959594 smaht_submitr-0.8.0.1b9/submitr/utils.py
+-rw-r--r--   0        0        0     3994 1970-01-01 00:00:00.000000 smaht_submitr-0.8.0.1b9/PKG-INFO
```

### Comparing `smaht_submitr-0.8.0.1b8/LICENSE.txt` & `smaht_submitr-0.8.0.1b9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/README.rst` & `smaht_submitr-0.8.0.1b9/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/pyproject.toml` & `smaht_submitr-0.8.0.1b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.0.1b8"  # TODO: To become 0.8.1
+version = "0.8.0.1b9"  # TODO: To become 0.8.1
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.8.0.1b8/submitr/base.py` & `smaht_submitr-0.8.0.1b9/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/output.py` & `smaht_submitr-0.8.0.1b9/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/progress_bar.py` & `smaht_submitr-0.8.0.1b9/submitr/progress_bar.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/s3_utils.py` & `smaht_submitr-0.8.0.1b9/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.0.1b9/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/submission.py` & `smaht_submitr-0.8.0.1b9/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.0.1b9/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_base.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_misc.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_show_upload_info.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_submission.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_upload_item_data.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/test_utils.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.0.1b9/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/submitr/utils.py` & `smaht_submitr-0.8.0.1b9/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.0.1b8/PKG-INFO` & `smaht_submitr-0.8.0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.0.1b8
+Version: 0.8.0.1b9
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.12
```

