# Comparing `tmp/dcm_classifier-0.8.0.tar.gz` & `tmp/dcm_classifier-0.8.1.tar.gz`

## Comparing `dcm_classifier-0.8.0.tar` & `dcm_classifier-0.8.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.git
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/EndNote_citation.enw
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/RIS_citation.ris
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/citations/bib_citation.bib
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/LICENSE
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.git
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/EndNote_citation.enw
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/RIS_citation.ris
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/citations/bib_citation.bib
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18085 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32256 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6185 2020-02-02 00:00:00.000000 dcm_classifier-0.8.1/PKG-INFO
```

### Comparing `dcm_classifier-0.8.0/.pre-commit-config.yaml` & `dcm_classifier-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/CONTRIBUTING.md` & `dcm_classifier-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.8.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.8.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.github/workflows/push_to_main.yml` & `dcm_classifier-0.8.1/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/citations/bib_citation.bib` & `dcm_classifier-0.8.1/citations/bib_citation.bib`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.1/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/models/rf_classifier.onnx` & `dcm_classifier-0.8.1/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.8.1/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/classify_study.py` & `dcm_classifier-0.8.1/scripts/classify_study.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.8.1/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/create_training_sheet.py` & `dcm_classifier-0.8.1/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.8.1/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/modality_classifier_training.py` & `dcm_classifier-0.8.1/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.8.1/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/orientation_model_training.py` & `dcm_classifier-0.8.1/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.8.1/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/running_classifier.ipynb` & `dcm_classifier-0.8.1/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/todo_list` & `dcm_classifier-0.8.1/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/training_config.py` & `dcm_classifier-0.8.1/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/scripts/utilities.py` & `dcm_classifier-0.8.1/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.8.1/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.8.1/src/dcm_classifier/dicom_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
     def organize_volumes(self) -> None:
         """
         Organize the subvolumes within the series based on acquisition time.
         """
         # AcquisitionTime is an optional field, this might need to be changed in the future
         sorted(
             self.volume_info_list,
-            key=lambda x: x.get_volume_dictionary().get("AcquisitionTime", -12345),
+            key=lambda x: x.get_volume_dictionary().get("AcquisitionTime", "000000.00"),
         )
         # assign the index to each volume
         for index, volume in enumerate(self.volume_info_list):
             volume.set_volume_index(index)
 
     def get_series_info_dict(self) -> dict[str, Any]:
         """
```

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.8.1/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.8.1/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.8.1/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.8.1/src/dcm_classifier/image_type_inference.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.8.1/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.8.1/src/dcm_classifier/utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
             else:
                 dataset_dictionary[field] = dataset[field].value
         elif field == "AcquisitionTime":
             if field not in dataset:
                 # AcquisitionTime is not a required field, it can be unknown
-                _default_inferred_value = -12345
+                _default_inferred_value = "000000.00"
                 dataset_dictionary[field] = _default_inferred_value
                 vprint(
                     f"Inferring optional {field} value of '{_default_inferred_value}' for missing field in {dicom_filename}"
                 )
             else:
                 dataset_dictionary[field] = dataset[field].value
```

### Comparing `dcm_classifier-0.8.0/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.8.1/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/conftest.py` & `dcm_classifier-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.8.1/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/testing_data/mock_data.txt` & `dcm_classifier-0.8.1/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.8.1/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.8.1/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.8.1/tests/unit_testing/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/.gitignore` & `dcm_classifier-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/LICENSE` & `dcm_classifier-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/README.md` & `dcm_classifier-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.8.0/pyproject.toml` & `dcm_classifier-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.8.0'
+version = '0.8.1'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
   { name="Cavan Riley", email="cavan-riley@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
```

### Comparing `dcm_classifier-0.8.0/PKG-INFO` & `dcm_classifier-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.8.0
+Version: 0.8.1
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>, Cavan Riley <cavan-riley@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
```

