# Comparing `tmp/foursight-4.4.4.tar.gz` & `tmp/foursight-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight-4.4.4.tar", max compression
+gzip compressed data, was "foursight-4.4.6.tar", max compression
```

## Comparing `foursight-4.4.4.tar` & `foursight-4.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.4.4/LICENSE.txt
--rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.4.4/chalicelib_fourfront/__init__.py
--rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.4.4/chalicelib_fourfront/app_utils.py
--rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.4.4/chalicelib_fourfront/check_schedules.py
--rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.4.4/chalicelib_fourfront/check_setup.json
--rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.4.4/chalicelib_fourfront/checks/__init__.py
--rw-r--r--   0        0        0    63124 2024-03-22 17:29:19.867219 foursight-4.4.4/chalicelib_fourfront/checks/audit_checks.py
--rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.4.4/chalicelib_fourfront/checks/badge_checks.py
--rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.4.4/chalicelib_fourfront/checks/check_utils.py
--rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.4.4/chalicelib_fourfront/checks/deployment_checks.py
--rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.4.4/chalicelib_fourfront/checks/ecs_checks.py
--rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.4.4/chalicelib_fourfront/checks/es_checks.py
--rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.4.4/chalicelib_fourfront/checks/header_checks.py
--rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.4.4/chalicelib_fourfront/checks/helpers/confchecks.py
--rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.4.4/chalicelib_fourfront/checks/helpers/google_utils.py
--rw-r--r--   0        0        0    95977 2024-03-13 13:41:24.369808 foursight-4.4.4/chalicelib_fourfront/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0    17742 2023-10-31 15:30:23.729379 foursight-4.4.4/chalicelib_fourfront/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.4.4/chalicelib_fourfront/checks/helpers/wrangler_utils.py
--rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.4.4/chalicelib_fourfront/checks/higlass_checks.py
--rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.4.4/chalicelib_fourfront/checks/release_updates_checks.py
--rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-4.4.4/chalicelib_fourfront/checks/system_checks.py
--rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.4.4/chalicelib_fourfront/checks/wfr_checks.py
--rw-r--r--   0        0        0    45274 2023-09-14 15:07:17.524014 foursight-4.4.4/chalicelib_fourfront/checks/wfr_encode_checks.py
--rw-r--r--   0        0        0   141043 2024-03-27 14:34:37.559863 foursight-4.4.4/chalicelib_fourfront/checks/wrangler_checks.py
--rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.4.4/chalicelib_fourfront/gitinfo.json
--rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.4.4/chalicelib_fourfront/package.py
--rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.4.4/chalicelib_fourfront/scripts/local_check_execution.py
--rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.4.4/chalicelib_fourfront/vars.py
--rw-r--r--   0        0        0     1610 2024-03-27 14:34:37.561555 foursight-4.4.4/pyproject.toml
--rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2017-11-21 15:12:01.000000 foursight-4.4.6/LICENSE.txt
+-rw-r--r--   0        0        0        0 2022-11-16 16:53:13.403096 foursight-4.4.6/chalicelib_fourfront/__init__.py
+-rw-r--r--   0        0        0     1088 2023-07-19 18:36:43.842986 foursight-4.4.6/chalicelib_fourfront/app_utils.py
+-rw-r--r--   0        0        0     5405 2022-11-16 16:53:13.404868 foursight-4.4.6/chalicelib_fourfront/check_schedules.py
+-rw-r--r--   0        0        0    54908 2024-03-07 20:51:35.647720 foursight-4.4.6/chalicelib_fourfront/check_setup.json
+-rw-r--r--   0        0        0      249 2022-11-16 16:53:13.406545 foursight-4.4.6/chalicelib_fourfront/checks/__init__.py
+-rw-r--r--   0        0        0    63124 2024-03-22 17:29:19.867219 foursight-4.4.6/chalicelib_fourfront/checks/audit_checks.py
+-rw-r--r--   0        0        0    37729 2023-07-20 15:47:44.788397 foursight-4.4.6/chalicelib_fourfront/checks/badge_checks.py
+-rw-r--r--   0        0        0     1657 2023-09-14 15:07:17.515971 foursight-4.4.6/chalicelib_fourfront/checks/check_utils.py
+-rw-r--r--   0        0        0    11548 2023-01-19 17:19:39.272753 foursight-4.4.6/chalicelib_fourfront/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2939 2023-04-19 19:52:24.091358 foursight-4.4.6/chalicelib_fourfront/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3914 2023-01-19 17:19:39.273550 foursight-4.4.6/chalicelib_fourfront/checks/es_checks.py
+-rw-r--r--   0        0        0    15663 2023-06-09 22:12:58.101520 foursight-4.4.6/chalicelib_fourfront/checks/header_checks.py
+-rw-r--r--   0        0        0      262 2022-11-16 16:53:13.426279 foursight-4.4.6/chalicelib_fourfront/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0    51933 2023-10-10 16:28:17.634518 foursight-4.4.6/chalicelib_fourfront/checks/helpers/google_utils.py
+-rw-r--r--   0        0        0    95977 2024-03-13 13:41:24.369808 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0    17738 2024-04-11 16:56:14.128461 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     3686 2022-11-16 16:53:13.428930 foursight-4.4.6/chalicelib_fourfront/checks/helpers/wrangler_utils.py
+-rw-r--r--   0        0        0    99000 2024-03-22 17:29:19.869545 foursight-4.4.6/chalicelib_fourfront/checks/higlass_checks.py
+-rw-r--r--   0        0        0    32926 2023-01-19 17:19:39.279026 foursight-4.4.6/chalicelib_fourfront/checks/release_updates_checks.py
+-rw-r--r--   0        0        0    45209 2023-04-19 19:52:24.091978 foursight-4.4.6/chalicelib_fourfront/checks/system_checks.py
+-rw-r--r--   0        0        0   131349 2024-03-07 20:07:33.211431 foursight-4.4.6/chalicelib_fourfront/checks/wfr_checks.py
+-rw-r--r--   0        0        0    45350 2024-04-11 16:56:14.129826 foursight-4.4.6/chalicelib_fourfront/checks/wfr_encode_checks.py
+-rw-r--r--   0        0        0   141043 2024-03-27 14:34:37.559863 foursight-4.4.6/chalicelib_fourfront/checks/wrangler_checks.py
+-rw-r--r--   0        0        0       75 2024-03-07 20:07:33.211950 foursight-4.4.6/chalicelib_fourfront/gitinfo.json
+-rw-r--r--   0        0        0      621 2022-11-16 16:53:13.457648 foursight-4.4.6/chalicelib_fourfront/package.py
+-rw-r--r--   0        0        0      327 2023-10-11 18:26:03.611223 foursight-4.4.6/chalicelib_fourfront/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      316 2022-11-16 16:53:13.457903 foursight-4.4.6/chalicelib_fourfront/vars.py
+-rw-r--r--   0        0        0     1610 2024-04-11 16:56:14.130960 foursight-4.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 foursight-4.4.6/PKG-INFO
```

### Comparing `foursight-4.4.4/LICENSE.txt` & `foursight-4.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/app_utils.py` & `foursight-4.4.6/chalicelib_fourfront/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/check_schedules.py` & `foursight-4.4.6/chalicelib_fourfront/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/check_setup.json` & `foursight-4.4.6/chalicelib_fourfront/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/audit_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/badge_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/badge_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/check_utils.py` & `foursight-4.4.6/chalicelib_fourfront/checks/check_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/deployment_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/ecs_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/es_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/header_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/header_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/helpers/google_utils.py` & `foursight-4.4.6/chalicelib_fourfront/checks/helpers/google_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/helpers/wfr_utils.py` & `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/helpers/wfrset_utils.py` & `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wfrset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
     },
     {
         "app_name": "encode-chipseq-aln-ctl",
         "workflow_uuid": "4eb427f1-a7d5-4d74-8cfa-4c77f42d5b43",
         "parameters": {},
         "config":{"instance_type": 'c5.2xlarge', "ebs_size": 70},
         'custom_pf_fields': {
-            'chip.first_ta_ctl': {
+            'chip.first_ta': {
                 'genome_assembly': genome,
                 'file_type': 'read positions',
                 'description': 'Positions of aligned reads in bed format, one line per read mate, for control experiment, from ENCODE ChIP-Seq Pipeline',
                 'disable_wfr_inputs': True}
         }
     },
     {
```

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/helpers/wrangler_utils.py` & `foursight-4.4.6/chalicelib_fourfront/checks/helpers/wrangler_utils.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/higlass_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/higlass_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/release_updates_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/release_updates_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/system_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/wfr_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/wfr_encode_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/wfr_encode_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,16 +641,16 @@
                 # if paired, need to run merge twice for each end
                 for merge_case in input_list:
                     merge_enum += 1
                     # RUN STEP 0
                     s0_input_files = {'input_fastqs': merge_case}
                     s0_tag = exp_id + '_p' + str(merge_enum)
                     keep, step0_status, step0_output = wfr_utils.stepper(library, keep,
-                                                                         'step0', s0_tag, merge_case,
-                                                                         s0_input_files, step0_name, 'merged_fastq')
+                                                                         'step0', s0_tag, merge_case, s0_input_files,
+                                                                         step0_name, 'merged_fastq', organism=organism)
                     if step0_status == 'complete':
                         merged_files.append(step0_output)
                     else:
                         ready_for_step1 = False
 
                 if ready_for_step1:
                     # rewrite exp_files with merged ones
@@ -703,15 +703,15 @@
 
             s1_input_files = input_files
             s1_tag = exp_id
             # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
             keep, step1_status, step1_output = wfr_utils.stepper(library, keep,
                                                                  'step1', s1_tag, exp_files,
                                                                  s1_input_files, step1_name, 'atac.first_ta',
-                                                                 additional_input={'parameters': parameters})
+                                                                 additional_input={'parameters': parameters}, organism=organism)
             if step1_status == 'complete':
                 # accumulate files to patch on experiment
                 patch_data = [step1_output, ]
                 complete['patch_opf'].append([exp_id, patch_data])
                 ta.append(step1_output)
             else:
                 # don't patch anything if at least one exp is still missing
@@ -747,16 +747,16 @@
                     ta = wfr_utils.select_best_2(ta, all_files, all_qcs)
                 else:
                     # run mergebed - default option
                     s2_input_files = {'input_bed': ta}
                     s2_tag = set_acc
                     # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
                     keep, step2_status, step2_output = wfr_utils.stepper(library, keep,
-                                                                         'step2', s2_tag, ta,
-                                                                         s2_input_files, step2_name, 'merged_bed')
+                                                                         'step2', s2_tag, ta, s2_input_files,
+                                                                         step2_name, 'merged_bed', organism=organism)
                     if step2_status == 'complete':
                         ta = [step2_output, ]
                     else:
                         ready_for_step3 = False
             if ready_for_step3:
                 # collect step3 input files
                 s3_input_files = {}
@@ -799,15 +799,15 @@
 
                 s3_tag = set_acc
                 # if complete, step1_output will have a list of 2 files, first_ta, and fist_ta_xcor
                 keep, step3_status, step3_output = wfr_utils.stepper(library, keep,
                                                                      'step3', s3_tag, ta,
                                                                      s3_input_files, step3_name,
                                                                      ['atac.optimal_peak', 'atac.conservative_peak', 'atac.sig_fc'],
-                                                                     additional_input={'parameters': parameters})
+                                                                     additional_input={'parameters': parameters}, organism=organism)
                 if step3_status == 'complete':
                     set_opt_peak = step3_output[0]
                     set_cons_peak = step3_output[1]
                     set_sig_fc = step3_output[2]
                     # accumulate files to patch on experiment
                     patch_data = [set_opt_peak, set_cons_peak, set_sig_fc]
                     complete['patch_opf'].append([set_acc, patch_data])
```

### Comparing `foursight-4.4.4/chalicelib_fourfront/checks/wrangler_checks.py` & `foursight-4.4.6/chalicelib_fourfront/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/chalicelib_fourfront/package.py` & `foursight-4.4.6/chalicelib_fourfront/package.py`

 * *Files identical despite different names*

### Comparing `foursight-4.4.4/pyproject.toml` & `foursight-4.4.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight"
-version = "4.4.4"
+version = "4.4.6"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_fourfront" }
 ]
```

### Comparing `foursight-4.4.4/PKG-INFO` & `foursight-4.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight
-Version: 4.4.4
+Version: 4.4.6
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

